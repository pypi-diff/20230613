# Comparing `tmp/phub-2.1.tar.gz` & `tmp/phub-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phub-2.1.tar", last modified: Mon Jun 12 19:20:20 2023, max compression
+gzip compressed data, was "phub-2.2.tar", last modified: Tue Jun 13 07:52:50 2023, max compression
```

## Comparing `phub-2.1.tar` & `phub-2.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:20:20.017775 phub-2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-12 19:20:05.000000 phub-2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-06-12 19:20:20.017775 phub-2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-06-12 19:20:05.000000 phub-2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-12 19:20:05.000000 phub-2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-12 19:20:20.017775 phub-2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-12 19:20:05.000000 phub-2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:20:20.013775 phub-2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:20:20.017775 phub-2.1/src/phub/
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-12 19:20:05.000000 phub-2.1/src/phub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17067 2023-06-12 19:20:05.000000 phub-2.1/src/phub/classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-06-12 19:20:05.000000 phub-2.1/src/phub/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)    10469 2023-06-12 19:20:05.000000 phub-2.1/src/phub/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-12 19:20:05.000000 phub-2.1/src/phub/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     7742 2023-06-12 19:20:05.000000 phub-2.1/src/phub/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 19:20:20.017775 phub-2.1/src/phub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-06-12 19:20:20.000000 phub-2.1/src/phub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-12 19:20:20.000000 phub-2.1/src/phub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 19:20:20.000000 phub-2.1/src/phub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-12 19:20:20.000000 phub-2.1/src/phub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-12 19:20:20.000000 phub-2.1/src/phub.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:52:50.160314 phub-2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-13 07:52:40.000000 phub-2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-06-13 07:52:50.160314 phub-2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-06-13 07:52:40.000000 phub-2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-13 07:52:40.000000 phub-2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-13 07:52:50.160314 phub-2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-13 07:52:40.000000 phub-2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:52:50.156314 phub-2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:52:50.160314 phub-2.2/src/phub/
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-13 07:52:40.000000 phub-2.2/src/phub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17284 2023-06-13 07:52:40.000000 phub-2.2/src/phub/classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-06-13 07:52:40.000000 phub-2.2/src/phub/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10462 2023-06-13 07:52:40.000000 phub-2.2/src/phub/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-13 07:52:40.000000 phub-2.2/src/phub/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7742 2023-06-13 07:52:40.000000 phub-2.2/src/phub/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:52:50.160314 phub-2.2/src/phub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-06-13 07:52:50.000000 phub-2.2/src/phub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-13 07:52:50.000000 phub-2.2/src/phub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 07:52:50.000000 phub-2.2/src/phub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-13 07:52:50.000000 phub-2.2/src/phub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-13 07:52:50.000000 phub-2.2/src/phub.egg-info/top_level.txt
```

### Comparing `phub-2.1/LICENSE` & `phub-2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `phub-2.1/PKG-INFO` & `phub-2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phub
-Version: 2.1
+Version: 2.2
 Summary: An API for PornHub
 Home-page: https://github.com/Egsagon/PHUB/
 Author: Egsagon
 Author-email: egsagon12@gmail.com
 License: GPLv3
 Platform: unix
 Platform: linux
```

### Comparing `phub-2.1/README.md` & `phub-2.2/README.md`

 * *Files identical despite different names*

### Comparing `phub-2.1/setup.cfg` & `phub-2.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = phub
-version = 2.1
+version = 2.2
 description = An API for PornHub
 author = Egsagon
 author_email = egsagon12@gmail.com
 url = https://github.com/Egsagon/PHUB/
 license = GPLv3
 license_file = LICENSE
 long_description = file: README.md
```

### Comparing `phub-2.1/src/phub/__init__.py` & `phub-2.2/src/phub/__init__.py`

 * *Files identical despite different names*

### Comparing `phub-2.1/src/phub/classes.py` & `phub-2.2/src/phub/classes.py`

 * *Files 2% similar despite different names*

```diff
@@ -242,53 +242,56 @@
         log('video', f'Parsed {len(segments)} video segments', level = 3)
         return segments
 
     def download(self,
                  path: str,
                  quality: utils.Quality,
                  quiet: bool = False,
+                 callback: Callable = None,
                  max_retries: int = 5) -> str:
         '''
         #### Download the video locally. ####
         -------------------------------------
         
         Arguments:
         - `path`               -- Directory or file to write to.
         - `quality`            -- Desired video quality.
         - `quiet`   (=`False`) -- Whether to enable logs to view download progress.
+        - `callback` (=`None`) -- Function to call to update download progress.
         - `max_retries` (=`5`) -- Maximum retries per segment request.
         
         NOTE 1 - If `path` is a directory, will create a new file in that directory
                  with the name of the video.
         NOTE 2 - Slow download. To use threaded downloads, call `get_M3U` instead.
+        NOTE 3 - Glitchy logs.
         -------------------------------------
         Returns the path of the file.
         '''
         
         log('video', f'Downloading {self} at', path, level = 5)
         
         # Append name if path is directory
         if os.path.isdir(path):
             path += ('' if path.endswith('/') else '/') + utils.pathify(self.title) + '.mp4'
             log('video', f'Changing path to', path, level = 2)
         
-        
         # Exceptionally allow debugging
         is_logging = utils.DEBUG
         if not quiet: utils.DEBUG = True
         
         log(' D L ', 'Starting video download for', self)
         
         segments = self.get_M3U(quality, process = True)
         
         # Start downloading
         with open(path, 'wb') as output:
             
             for index, url in enumerate(segments):
-                log(' D L ', f'Downloading {index + 1}/{len(segments)}', level = 3, r = 1)
+                log(' D L ', f'Downloading {index + 1}/{len(segments)}', level = 3, r = 0) # TODO
+                if callback: callback(index + 1, len(segments))
                 
                 for i in range(max_retries):
                     res = self.client._call('GET', url, simple_url = False, throw = False)
                     
                     if not res.ok:                        
                         log(' D L ', f'Segment download failed, retrying ({i}/{max_retries})', level = 1)
                         continue
```

### Comparing `phub-2.1/src/phub/consts.py` & `phub-2.2/src/phub/consts.py`

 * *Files identical despite different names*

### Comparing `phub-2.1/src/phub/core.py` & `phub-2.2/src/phub/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -303,10 +303,10 @@
         
         -----------------------------------------------
         Returns a `VideoIterator` object.
         '''
         
         log('client', 'Opening new search query:', query, level = 6)
         url = consts.ROOT + 'video/search?search=' + query
-        return classes.VideoIterator(self.client, url)
+        return classes.VideoIterator(self, url)
 
 # EOF
```

### Comparing `phub-2.1/src/phub/parser.py` & `phub-2.2/src/phub/parser.py`

 * *Files identical despite different names*

### Comparing `phub-2.1/src/phub/utils.py` & `phub-2.2/src/phub/utils.py`

 * *Files identical despite different names*

### Comparing `phub-2.1/src/phub.egg-info/PKG-INFO` & `phub-2.2/src/phub.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phub
-Version: 2.1
+Version: 2.2
 Summary: An API for PornHub
 Home-page: https://github.com/Egsagon/PHUB/
 Author: Egsagon
 Author-email: egsagon12@gmail.com
 License: GPLv3
 Platform: unix
 Platform: linux
```

