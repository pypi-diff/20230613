# Comparing `tmp/boxfs-0.1a1.tar.gz` & `tmp/boxfs-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boxfs-0.1a1.tar", max compression
+gzip compressed data, was "boxfs-0.2.0.tar", max compression
```

## Comparing `boxfs-0.1a1.tar` & `boxfs-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,8 @@
--rw-r--r--   0        0        0     1109 2023-05-11 19:02:55.323065 boxfs-0.1a1/LICENSE
--rw-r--r--   0        0        0     1105 2023-05-12 15:02:00.753230 boxfs-0.1a1/pyproject.toml
--rw-r--r--   0        0        0       34 2023-05-12 13:46:02.149383 boxfs-0.1a1/src/boxfs/__init__.py
--rw-r--r--   0        0        0    17437 2023-05-12 14:00:34.245785 boxfs-0.1a1/src/boxfs/boxfs.py
--rw-r--r--   0        0        0      807 1970-01-01 00:00:00.000000 boxfs-0.1a1/setup.py
--rw-r--r--   0        0        0      514 1970-01-01 00:00:00.000000 boxfs-0.1a1/PKG-INFO
+-rw-r--r--   0        0        0     1109 2023-05-11 19:02:55.323065 boxfs-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1532 2023-06-13 13:20:56.069213 boxfs-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3788 2023-06-13 13:20:56.050230 boxfs-0.2.0/README.md
+-rw-r--r--   0        0        0       34 2023-05-12 15:59:55.744647 boxfs-0.2.0/src/boxfs/__init__.py
+-rw-r--r--   0        0        0      592 2023-06-13 13:20:56.079625 boxfs-0.2.0/src/boxfs/_upath.py
+-rw-r--r--   0        0        0    18878 2023-06-13 13:20:56.091053 boxfs-0.2.0/src/boxfs/boxfs.py
+-rw-r--r--   0        0        0     4746 1970-01-01 00:00:00.000000 boxfs-0.2.0/setup.py
+-rw-r--r--   0        0        0     4805 1970-01-01 00:00:00.000000 boxfs-0.2.0/PKG-INFO
```

### Comparing `boxfs-0.1a1/LICENSE` & `boxfs-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `boxfs-0.1a1/src/boxfs/boxfs.py` & `boxfs-0.2.0/src/boxfs/boxfs.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,20 @@
 )
 
 from boxsdk import BoxAPIException, Client, OAuth2
 from boxsdk.auth.oauth2 import TokenScope
 from boxsdk.object.item import Item
 from fsspec.spec import AbstractBufferedFile, AbstractFileSystem
 
+try:
+    import boxfs._upath  # noqa: F401
+except ModuleNotFoundError:
+    # Optional dependency not found
+    pass
+
 
 __all__ = ["BoxFileSystem"]
 
 logger = logging.getLogger(__name__)
 
 _PathLike = str
 _ObjectId = str
@@ -45,25 +51,24 @@
     ]
     # fmt: on
 
     def __init__(
         self,
         client: Optional[Client] = None,
         oauth: Optional[OAuth2] = None,
-        # access="full_control",
         client_type: Type[Client] = Client,
         root_id: _ObjectId = None,
         root_path: _PathLike = None,
         path_map: Optional[Mapping[_PathLike, _ObjectId]] = None,
         scopes: Optional[Iterable[TokenScope]] = None,
         **kwargs,
     ):
         """Instantiate BoxFileSystem
 
-        Creates a BoxFileSystem using the 
+        Creates a BoxFileSystem using the boxsdk interface
 
         Parameters
         ----------
         oauth : OAuth2, optional
             Box app OAuth2 configuration, e.g. loaded from `JWTAuth.from_settings_file`,
             by default None
         client : Client, optional
@@ -74,19 +79,21 @@
         If `client` is provided, it is used for handling API calls. Otherwise, the file
         system to instantiate a new client connection, of type `client_type`, using the
         provided `oauth` configuration.
 
         root_id : Object ID string, optional
             Box ID of folder where file system root is placed, by default None
         root_path : path string, optional
-            Path to Box root folder, relative to token root (e.g. "All Files")  
-            # TODO: Is this correct? Add a test
+            Path to Box root folder, must be relative to token root (e.g. "All Files").
+            The client must have access to the application user's root folder (i.e., it
+            cannot be downscoped to a subfolder)
         
         If only `root_id` is provided, the `root_path` is determined from API calls. If 
-        only `root_path` is provided, the `root_id` is determined from API calls.
+        only `root_path` is provided, the `root_id` is determined from API calls. If
+        neither is provided, the application user's root folder is used.
             
         path_map : Mapping[path string -> object ID string], optional
             Mapping of paths to object ID strings, used to populate initial lookup cache
             for quick directory navigation
         scopes : Iterable[TokenScope], optional
             List of permissions to which the API token should be restricted. If None
             (default), no restrictions are applied. If scopes are provided, the client
@@ -97,39 +104,54 @@
         if path_map is None:
             path_map = {}
         self.path_map = path_map
         if client is None:
             self.connect(oauth, client_type)
         else:
             self.client = client.clone()
-        self.set_root_folder(root_id, root_path)
+        self.root_id = self._get_root_id(root_id, root_path)
+        self.root_path = self._get_root_path(self.root_id)
 
         self._original_client = self.client
         self.scopes = scopes
         if scopes:
             self.downscope_token(self.scopes)
 
         self._cache = {}
 
     def connect(self, config, client_type):
         self.client: Client = client_type(config)
 
-    def set_root_folder(self, root_id=None, root_path=None):
-        if root_id is None and root_path is not None:
-            root_id = self._get_absolute_path_id(root_path)
+    def _get_root_id(self, root_id: _ObjectId = None, root_path: _PathLike = None):
+        """Gets the root folder ID
 
-        if root_id is None:
-            root_id = self.root_id
+        If root_id is not None, it is returned. Otherwise, if root path is not None, the
+        ID of the corresponding folder is determined. If both are None, return the
+        default root id of "0"
 
-        if root_path is None:
-            folder = self.client.folder(root_id).get(fields=["name", "path_collection"])
-            root_path = self._construct_path(folder, relative=False)
+        Parameters
+        ----------
+        root_id : _ObjectId, optional
+            Root ID if provided, by default None
+        root_path : _PathLike, optional
+            Root Path if provided, by default None
+        """
+        if root_id is not None:
+            return root_id
+        else:
+            if root_path is not None:
+                root_id = self._get_absolute_path_id(root_path)
+            else:
+                root_id = self.root_id
 
-        self.root_id = root_id
-        self.root_path = root_path
+        return root_id
+    
+    def _get_root_path(self, root_id):
+        folder = self.client.folder(root_id).get(fields=["name", "path_collection"])
+        return self._construct_path(folder, relative=False)
 
     def downscope_token(self, scopes: Iterable[TokenScope]):
         """Downscope permissions for the underlying client
 
         Parameters
         ----------
         scopes : Iterable[boxsdk.auth.oath2.TokenScope]
@@ -144,15 +166,15 @@
                 client_id=None,
                 client_secret=None,
                 access_token=downscoped_token.access_token,
             )
         )
         # The root path changes after downscoping, because the "All Files" folder
         # is hidden
-        self.set_root_folder(root_id=self.root_id)
+        self.root_path = self._get_root_path(self.root_id)
 
     def refresh_token(self):
         self._original_client = self._original_client.auth.refresh(
             self._original_client.auth.access_token
         )
         if self.scopes:
             self.downscope_token(self.scopes)
@@ -180,15 +202,24 @@
             return self.path_map[path]
 
         parent = self._parent(path)
         return self.seek_closest_known_path(parent)
 
     def _get_absolute_path_id(self, path: str):
         _closest = self.client.folder(self._default_root_id)
-        _closest_path = ""
+
+        try:
+            _closest = _closest.get(fields=self._fields)
+        except BoxAPIException as error:
+            if error.status == 403:
+                raise PermissionError("Could not access user root folder ('All Files')")
+            else:
+                raise
+
+        _closest_path = _closest.name
         path = self._strip_protocol(path)
         try:
             for part in path.split("/"):
                 error = True
                 items = _closest.get_items(fields=self._fields)
                 for item in items:
                     item_path = "/".join((_closest_path, part))
@@ -220,15 +251,15 @@
         _closest_id = self.seek_closest_known_path(path)
         _closest = self.client.folder(_closest_id)
         _closest_path = self._construct_path(_closest)
         remaining_path = path.lstrip(self.root_marker).replace(_closest_path, "", 1)
         if remaining_path == "":
             return _closest_id
         try:
-            for part in remaining_path.split("/"):
+            for part in remaining_path.lstrip("/").split("/"):
                 error = True
                 items = _closest.get_items(fields=self._fields)
                 for item in items:
                     item_path = "/".join((_closest_path, part))
                     self.path_map[item_path] = item.id
                     if item.type in ("folder", "file") and item.name == part:
                         _closest = item
@@ -316,20 +347,20 @@
         else:
             items = list(items)
             self.dircache[cache_path] = items
 
         fs_items = []
         if not detail:
             for item in items:
-                item_path = self._construct_path(item)
+                item_path = self._construct_path(item, relative=True)
                 self.path_map[item_path] = item.id
                 fs_items.append(item_path)
         else:
             for item in items:
-                item_path = self._construct_path(item)
+                item_path = self._construct_path(item, relative=True)
                 self.path_map[item_path] = item.id
                 fs_items.append(
                     {
                         "name": item_path,
                         "size": item.size,
                         "type": FS_TYPES[item.type],
                         "id": item.id,
@@ -392,26 +423,36 @@
     def _open(self, *args, **kwargs):
         return BoxFile(self, *args, **kwargs)
 
 
 class BoxFile(AbstractBufferedFile):
     def __init__(
         self,
-        fs,
+        fs: BoxFileSystem,
         path,
         mode="rb",
         block_size="default",
         autocommit=True,
         cache_type="readahead",
         cache_options=None,
         size=None,
         **kwargs,
     ):
-        super().__init__(fs, path, mode, block_size, autocommit=autocommit, **kwargs)
-        self.fs: BoxFileSystem
+        super().__init__(
+            fs,
+            fs._get_relative_path(path),
+            mode,
+            block_size,
+            autocommit=autocommit,
+            cache_type=cache_type,
+            cache_options=cache_options,
+            size=size,
+            **kwargs
+        )
+        self.exists = False
 
         if self.writable():
             self.location = None
             self._folder_path = fs._parent(path)
             self.name = path.rsplit("/", maxsplit=1)[-1]
             self.folder_id = fs.path_to_file_id(self._folder_path)
             self.exists = fs.exists(path)
```

