# Comparing `tmp/articat-0.1.8.tar.gz` & `tmp/articat-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "articat-0.1.8.tar", last modified: Fri May 20 01:39:31 2022, max compression
+gzip compressed data, was "articat-0.1.9.tar", last modified: Wed Nov 23 12:18:18 2022, max compression
```

## Comparing `articat-0.1.8.tar` & `articat-0.1.9.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 01:39:31.606126 articat-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-05-20 01:39:13.000000 articat-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      119 2022-05-20 01:39:13.000000 articat-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5364 2022-05-20 01:39:31.606126 articat-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4609 2022-05-20 01:39:13.000000 articat-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 01:39:31.598126 articat-0.1.8/articat/
--rw-r--r--   0 runner    (1001) docker     (121)      430 2022-05-20 01:39:13.000000 articat-0.1.8/articat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13620 2022-05-20 01:39:13.000000 articat-0.1.8/articat/artifact.py
--rw-r--r--   0 runner    (1001) docker     (121)     6761 2022-05-20 01:39:13.000000 articat-0.1.8/articat/bq_artifact.py
--rw-r--r--   0 runner    (1001) docker     (121)     9347 2022-05-20 01:39:13.000000 articat-0.1.8/articat/catalog.py
--rw-r--r--   0 runner    (1001) docker     (121)     7087 2022-05-20 01:39:13.000000 articat-0.1.8/articat/catalog_datastore.py
--rw-r--r--   0 runner    (1001) docker     (121)     3461 2022-05-20 01:39:13.000000 articat-0.1.8/articat/catalog_local.py
--rw-r--r--   0 runner    (1001) docker     (121)     4096 2022-05-20 01:39:13.000000 articat-0.1.8/articat/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     7077 2022-05-20 01:39:13.000000 articat-0.1.8/articat/config.py
--rw-r--r--   0 runner    (1001) docker     (121)    10865 2022-05-20 01:39:13.000000 articat-0.1.8/articat/fs_artifact.py
--rw-r--r--   0 runner    (1001) docker     (121)     1034 2022-05-20 01:39:13.000000 articat-0.1.8/articat/meta_artifact.py
--rw-r--r--   0 runner    (1001) docker     (121)     2689 2022-05-20 01:39:13.000000 articat-0.1.8/articat/notebook_artifact.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-20 01:39:13.000000 articat-0.1.8/articat/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 01:39:31.602126 articat-0.1.8/articat/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-20 01:39:13.000000 articat-0.1.8/articat/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4748 2022-05-20 01:39:13.000000 articat-0.1.8/articat/tests/artifact_test.py
--rw-r--r--   0 runner    (1001) docker     (121)      614 2022-05-20 01:39:13.000000 articat-0.1.8/articat/tests/bq_artifact_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    10009 2022-05-20 01:39:13.000000 articat-0.1.8/articat/tests/catalog_datastore_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     2065 2022-05-20 01:39:13.000000 articat-0.1.8/articat/tests/cli_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     2359 2022-05-20 01:39:13.000000 articat-0.1.8/articat/tests/config_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     3162 2022-05-20 01:39:13.000000 articat-0.1.8/articat/tests/fs_artifact_test.py
--rw-r--r--   0 runner    (1001) docker     (121)      971 2022-05-20 01:39:13.000000 articat-0.1.8/articat/tests/meta_artifact_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1434 2022-05-20 01:39:13.000000 articat-0.1.8/articat/tests/notebook_artifact_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1147 2022-05-20 01:39:13.000000 articat-0.1.8/articat/tests/notebook_utils_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 01:39:31.602126 articat-0.1.8/articat/tests/test_files/
--rw-r--r--   0 runner    (1001) docker     (121)     1544 2022-05-20 01:39:13.000000 articat-0.1.8/articat/tests/test_files/dummy_notebook.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     3498 2022-05-20 01:39:13.000000 articat-0.1.8/articat/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     8352 2022-05-20 01:39:13.000000 articat-0.1.8/articat/tests/utils_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 01:39:31.606126 articat-0.1.8/articat/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-20 01:39:13.000000 articat-0.1.8/articat/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1270 2022-05-20 01:39:13.000000 articat-0.1.8/articat/utils/class_or_instance_method.py
--rw-r--r--   0 runner    (1001) docker     (121)      307 2022-05-20 01:39:13.000000 articat-0.1.8/articat/utils/datetime_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     4860 2022-05-20 01:39:13.000000 articat-0.1.8/articat/utils/notebook_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-05-20 01:39:13.000000 articat-0.1.8/articat/utils/path_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-05-20 01:39:13.000000 articat-0.1.8/articat/utils/typing.py
--rw-r--r--   0 runner    (1001) docker     (121)     6448 2022-05-20 01:39:13.000000 articat-0.1.8/articat/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 01:39:31.602126 articat-0.1.8/articat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5364 2022-05-20 01:39:30.000000 articat-0.1.8/articat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1171 2022-05-20 01:39:31.000000 articat-0.1.8/articat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-20 01:39:31.000000 articat-0.1.8/articat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-20 01:39:29.000000 articat-0.1.8/articat.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      178 2022-05-20 01:39:31.000000 articat-0.1.8/articat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-05-20 01:39:31.000000 articat-0.1.8/articat.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 01:39:31.606126 articat-0.1.8/bin/
--rwxr-xr-x   0 runner    (1001) docker     (121)      300 2022-05-20 01:39:13.000000 articat-0.1.8/bin/articat
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 01:39:31.606126 articat-0.1.8/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     3265 2022-05-20 01:39:13.000000 articat-0.1.8/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (121)      336 2022-05-20 01:39:13.000000 articat-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     2090 2022-05-20 01:39:31.606126 articat-0.1.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-23 12:18:18.507097 articat-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-11-23 12:18:02.000000 articat-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      119 2022-11-23 12:18:02.000000 articat-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     5364 2022-11-23 12:18:18.507097 articat-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4609 2022-11-23 12:18:02.000000 articat-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-23 12:18:18.503097 articat-0.1.9/articat/
+-rw-r--r--   0 runner    (1001) docker     (121)      430 2022-11-23 12:18:02.000000 articat-0.1.9/articat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13620 2022-11-23 12:18:02.000000 articat-0.1.9/articat/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6761 2022-11-23 12:18:02.000000 articat-0.1.9/articat/bq_artifact.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9347 2022-11-23 12:18:02.000000 articat-0.1.9/articat/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7087 2022-11-23 12:18:02.000000 articat-0.1.9/articat/catalog_datastore.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3461 2022-11-23 12:18:02.000000 articat-0.1.9/articat/catalog_local.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4096 2022-11-23 12:18:02.000000 articat-0.1.9/articat/cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7077 2022-11-23 12:18:02.000000 articat-0.1.9/articat/config.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11015 2022-11-23 12:18:02.000000 articat-0.1.9/articat/fs_artifact.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1034 2022-11-23 12:18:02.000000 articat-0.1.9/articat/meta_artifact.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2689 2022-11-23 12:18:02.000000 articat-0.1.9/articat/notebook_artifact.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-23 12:18:02.000000 articat-0.1.9/articat/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-23 12:18:18.503097 articat-0.1.9/articat/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-23 12:18:02.000000 articat-0.1.9/articat/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4748 2022-11-23 12:18:02.000000 articat-0.1.9/articat/tests/artifact_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)      614 2022-11-23 12:18:02.000000 articat-0.1.9/articat/tests/bq_artifact_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10009 2022-11-23 12:18:02.000000 articat-0.1.9/articat/tests/catalog_datastore_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2065 2022-11-23 12:18:02.000000 articat-0.1.9/articat/tests/cli_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2359 2022-11-23 12:18:02.000000 articat-0.1.9/articat/tests/config_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3162 2022-11-23 12:18:02.000000 articat-0.1.9/articat/tests/fs_artifact_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)      971 2022-11-23 12:18:02.000000 articat-0.1.9/articat/tests/meta_artifact_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1434 2022-11-23 12:18:02.000000 articat-0.1.9/articat/tests/notebook_artifact_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1147 2022-11-23 12:18:02.000000 articat-0.1.9/articat/tests/notebook_utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-23 12:18:18.503097 articat-0.1.9/articat/tests/test_files/
+-rw-r--r--   0 runner    (1001) docker     (121)     1544 2022-11-23 12:18:02.000000 articat-0.1.9/articat/tests/test_files/dummy_notebook.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)     3498 2022-11-23 12:18:02.000000 articat-0.1.9/articat/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8352 2022-11-23 12:18:02.000000 articat-0.1.9/articat/tests/utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-23 12:18:18.507097 articat-0.1.9/articat/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-23 12:18:02.000000 articat-0.1.9/articat/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1270 2022-11-23 12:18:02.000000 articat-0.1.9/articat/utils/class_or_instance_method.py
+-rw-r--r--   0 runner    (1001) docker     (121)      307 2022-11-23 12:18:02.000000 articat-0.1.9/articat/utils/datetime_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4860 2022-11-23 12:18:02.000000 articat-0.1.9/articat/utils/notebook_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-11-23 12:18:02.000000 articat-0.1.9/articat/utils/path_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)       79 2022-11-23 12:18:02.000000 articat-0.1.9/articat/utils/typing.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6448 2022-11-23 12:18:02.000000 articat-0.1.9/articat/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-23 12:18:18.503097 articat-0.1.9/articat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     5364 2022-11-23 12:18:18.000000 articat-0.1.9/articat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1171 2022-11-23 12:18:18.000000 articat-0.1.9/articat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-23 12:18:18.000000 articat-0.1.9/articat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-23 12:18:18.000000 articat-0.1.9/articat.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      178 2022-11-23 12:18:18.000000 articat-0.1.9/articat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2022-11-23 12:18:18.000000 articat-0.1.9/articat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-23 12:18:18.507097 articat-0.1.9/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (121)      300 2022-11-23 12:18:02.000000 articat-0.1.9/bin/articat
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-23 12:18:18.507097 articat-0.1.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)     3265 2022-11-23 12:18:02.000000 articat-0.1.9/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (121)      336 2022-11-23 12:18:02.000000 articat-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     2090 2022-11-23 12:18:18.507097 articat-0.1.9/setup.cfg
```

### Comparing `articat-0.1.8/LICENSE` & `articat-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `articat-0.1.8/PKG-INFO` & `articat-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: articat
-Version: 0.1.8
+Version: 0.1.9
 Summary: articat: data artifact catalog
 Home-page: https://github.com/related-sciences/articat
 Author: Related Sciences LLC
 Author-email: rav@related.vc
 License: Apache
 Keywords: data,catalog,metadata,data-discovery,data-catalog
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `articat-0.1.8/README.md` & `articat-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `articat-0.1.8/articat/artifact.py` & `articat-0.1.9/articat/artifact.py`

 * *Files identical despite different names*

### Comparing `articat-0.1.8/articat/bq_artifact.py` & `articat-0.1.9/articat/bq_artifact.py`

 * *Files identical despite different names*

### Comparing `articat-0.1.8/articat/catalog.py` & `articat-0.1.9/articat/catalog.py`

 * *Files identical despite different names*

### Comparing `articat-0.1.8/articat/catalog_datastore.py` & `articat-0.1.9/articat/catalog_datastore.py`

 * *Files identical despite different names*

### Comparing `articat-0.1.8/articat/catalog_local.py` & `articat-0.1.9/articat/catalog_local.py`

 * *Files identical despite different names*

### Comparing `articat-0.1.8/articat/cli.py` & `articat-0.1.9/articat/cli.py`

 * *Files identical despite different names*

### Comparing `articat-0.1.8/articat/config.py` & `articat-0.1.9/articat/config.py`

 * *Files identical despite different names*

### Comparing `articat-0.1.8/articat/fs_artifact.py` & `articat-0.1.9/articat/fs_artifact.py`

 * *Files 2% similar despite different names*

```diff
@@ -191,14 +191,15 @@
             # NotImplementedError, in which case we just double check
             # if the SUCCESS marker exist, and raise if it not
             fs.touch(f"{actual_prefix}/_SUCCESS", truncate=False)
         except NotImplementedError:
             assert fs.exists(
                 f"{actual_prefix}/_SUCCESS"
             ), "We could not create a SUCCESS marker and it does not exist"
+        object.__setattr__(self, "_file_prefix", None)
         return self
 
     def _get_file_prefix(self, tmp: bool = True) -> str:
         if not self.created:
             raise ValueError("created must be set")
         if not self.id:
             raise ValueError("ID must be set")
@@ -239,15 +240,14 @@
     def __exit__(
         self,
         exc_type: Optional[type[BaseException]],
         exc_val: Optional[BaseException],
         exc_tb: Optional[TracebackType],
     ) -> None:
         super().__exit__(exc_type, exc_val, exc_tb)
-        object.__setattr__(self, "_file_prefix", None)
 
     def browser_url(self) -> str:
         if self.main_dir.startswith("gs://"):
             path = self.main_dir.lstrip("gs://")
             return f"https://console.cloud.google.com/storage/browser/{path}"
         else:
             return self.main_dir
@@ -265,9 +265,11 @@
         if local_path.is_dir():
             fs.upload(
                 local_path.as_posix(),
                 self.staging_file_prefix,
                 recursive=True,
             )
         else:
+            assert local_path.is_file(), "Must be a single regular file or directory"
             fs.upload(local_path.as_posix(), self.joinpath(local_path.name))
+            self.files_pattern = self.joinpath(local_path.name)
         return self
```

### Comparing `articat-0.1.8/articat/meta_artifact.py` & `articat-0.1.9/articat/meta_artifact.py`

 * *Files identical despite different names*

### Comparing `articat-0.1.8/articat/notebook_artifact.py` & `articat-0.1.9/articat/notebook_artifact.py`

 * *Files identical despite different names*

### Comparing `articat-0.1.8/articat/tests/artifact_test.py` & `articat-0.1.9/articat/tests/artifact_test.py`

 * *Files identical despite different names*

### Comparing `articat-0.1.8/articat/tests/bq_artifact_test.py` & `articat-0.1.9/articat/tests/bq_artifact_test.py`

 * *Files identical despite different names*

### Comparing `articat-0.1.8/articat/tests/catalog_datastore_test.py` & `articat-0.1.9/articat/tests/catalog_datastore_test.py`

 * *Files identical despite different names*

### Comparing `articat-0.1.8/articat/tests/cli_test.py` & `articat-0.1.9/articat/tests/cli_test.py`

 * *Files identical despite different names*

### Comparing `articat-0.1.8/articat/tests/config_test.py` & `articat-0.1.9/articat/tests/config_test.py`

 * *Files identical despite different names*

### Comparing `articat-0.1.8/articat/tests/fs_artifact_test.py` & `articat-0.1.9/articat/tests/fs_artifact_test.py`

 * *Files identical despite different names*

### Comparing `articat-0.1.8/articat/tests/meta_artifact_test.py` & `articat-0.1.9/articat/tests/meta_artifact_test.py`

 * *Files identical despite different names*

### Comparing `articat-0.1.8/articat/tests/notebook_artifact_test.py` & `articat-0.1.9/articat/tests/notebook_artifact_test.py`

 * *Files identical despite different names*

### Comparing `articat-0.1.8/articat/tests/notebook_utils_test.py` & `articat-0.1.9/articat/tests/notebook_utils_test.py`

 * *Files identical despite different names*

### Comparing `articat-0.1.8/articat/tests/test_files/dummy_notebook.ipynb` & `articat-0.1.9/articat/tests/test_files/dummy_notebook.ipynb`

 * *Files identical despite different names*

### Comparing `articat-0.1.8/articat/tests/utils.py` & `articat-0.1.9/articat/tests/utils.py`

 * *Files identical despite different names*

### Comparing `articat-0.1.8/articat/tests/utils_test.py` & `articat-0.1.9/articat/tests/utils_test.py`

 * *Files identical despite different names*

### Comparing `articat-0.1.8/articat/utils/class_or_instance_method.py` & `articat-0.1.9/articat/utils/class_or_instance_method.py`

 * *Files identical despite different names*

### Comparing `articat-0.1.8/articat/utils/notebook_utils.py` & `articat-0.1.9/articat/utils/notebook_utils.py`

 * *Files identical despite different names*

### Comparing `articat-0.1.8/articat/utils/path_utils.py` & `articat-0.1.9/articat/utils/path_utils.py`

 * *Files identical despite different names*

### Comparing `articat-0.1.8/articat/utils/utils.py` & `articat-0.1.9/articat/utils/utils.py`

 * *Files identical despite different names*

### Comparing `articat-0.1.8/articat.egg-info/PKG-INFO` & `articat-0.1.9/articat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: articat
-Version: 0.1.8
+Version: 0.1.9
 Summary: articat: data artifact catalog
 Home-page: https://github.com/related-sciences/articat
 Author: Related Sciences LLC
 Author-email: rav@related.vc
 License: Apache
 Keywords: data,catalog,metadata,data-discovery,data-catalog
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `articat-0.1.8/articat.egg-info/SOURCES.txt` & `articat-0.1.9/articat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `articat-0.1.8/docs/contributing.md` & `articat-0.1.9/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `articat-0.1.8/setup.cfg` & `articat-0.1.9/setup.cfg`

 * *Files identical despite different names*

