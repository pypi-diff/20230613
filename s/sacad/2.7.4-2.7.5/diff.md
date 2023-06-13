# Comparing `tmp/sacad-2.7.4.tar.gz` & `tmp/sacad-2.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sacad-2.7.4.tar", last modified: Sun Feb 19 13:38:37 2023, max compression
+gzip compressed data, was "sacad-2.7.5.tar", last modified: Tue Jun 13 20:55:23 2023, max compression
```

## Comparing `sacad-2.7.4.tar` & `sacad-2.7.5.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 maxime    (1000) maxime    (1000)        0 2023-02-19 13:38:37.606074 sacad-2.7.4/
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    16725 2021-03-22 22:25:00.000000 sacad-2.7.4/LICENSE
--rw-r--r--   0 maxime    (1000) maxime    (1000)       65 2019-07-25 19:04:11.000000 sacad-2.7.4/MANIFEST.in
--rw-r--r--   0 maxime    (1000) maxime    (1000)     6757 2023-02-19 13:38:37.606074 sacad-2.7.4/PKG-INFO
--rw-r--r--   0 maxime    (1000) maxime    (1000)     5615 2023-01-01 13:26:30.000000 sacad-2.7.4/README.md
--rw-r--r--   0 maxime    (1000) maxime    (1000)      148 2022-11-25 19:21:00.000000 sacad-2.7.4/requirements.txt
-drwxr-xr-x   0 maxime    (1000) maxime    (1000)        0 2023-02-19 13:38:37.606074 sacad-2.7.4/sacad/
--rwxr-xr-x   0 maxime    (1000) maxime    (1000)     7477 2023-02-19 13:32:27.000000 sacad-2.7.4/sacad/__init__.py
--rwxr-xr-x   0 maxime    (1000) maxime    (1000)      138 2021-03-23 21:52:59.000000 sacad-2.7.4/sacad/__main__.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)     1040 2022-03-14 16:55:38.000000 sacad-2.7.4/sacad/colored_logging.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)    29963 2022-12-20 22:27:31.000000 sacad-2.7.4/sacad/cover.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)     9531 2022-09-11 21:04:47.000000 sacad-2.7.4/sacad/http_helpers.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)      487 2021-03-23 21:32:50.000000 sacad-2.7.4/sacad/mkstemp_ctx.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)     3235 2022-01-29 19:52:16.000000 sacad-2.7.4/sacad/rate_watcher.py
--rwxr-xr-x   0 maxime    (1000) maxime    (1000)    17443 2023-02-18 20:52:01.000000 sacad-2.7.4/sacad/recurse.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)      742 2022-01-29 19:52:16.000000 sacad-2.7.4/sacad/redo.py
-drwxr-xr-x   0 maxime    (1000) maxime    (1000)        0 2023-02-19 13:38:37.606074 sacad-2.7.4/sacad/sources/
--rw-r--r--   0 maxime    (1000) maxime    (1000)      600 2022-09-11 21:22:43.000000 sacad-2.7.4/sacad/sources/__init__.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)     1592 2023-02-19 13:31:16.000000 sacad-2.7.4/sacad/sources/amazonbase.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)     6465 2022-08-16 13:04:23.000000 sacad-2.7.4/sacad/sources/amazoncd.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)     6423 2022-08-16 13:04:23.000000 sacad-2.7.4/sacad/sources/amazondigital.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)     9337 2022-11-25 19:34:05.000000 sacad-2.7.4/sacad/sources/base.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)     2787 2022-08-16 13:04:23.000000 sacad-2.7.4/sacad/sources/deezer.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)     3047 2022-12-17 14:27:31.000000 sacad-2.7.4/sacad/sources/discogs.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)     2625 2022-09-11 21:33:52.000000 sacad-2.7.4/sacad/sources/itunes.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)     3543 2022-08-16 13:04:23.000000 sacad-2.7.4/sacad/sources/lastfm.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)     1433 2022-01-29 19:52:16.000000 sacad-2.7.4/sacad/tqdm_logging.py
-drwxr-xr-x   0 maxime    (1000) maxime    (1000)        0 2023-02-19 13:38:37.606074 sacad-2.7.4/sacad.egg-info/
--rw-r--r--   0 maxime    (1000) maxime    (1000)     6757 2023-02-19 13:38:37.000000 sacad-2.7.4/sacad.egg-info/PKG-INFO
--rw-r--r--   0 maxime    (1000) maxime    (1000)      677 2023-02-19 13:38:37.000000 sacad-2.7.4/sacad.egg-info/SOURCES.txt
--rw-r--r--   0 maxime    (1000) maxime    (1000)        1 2023-02-19 13:38:37.000000 sacad-2.7.4/sacad.egg-info/dependency_links.txt
--rw-r--r--   0 maxime    (1000) maxime    (1000)       73 2023-02-19 13:38:37.000000 sacad-2.7.4/sacad.egg-info/entry_points.txt
--rw-r--r--   0 maxime    (1000) maxime    (1000)      148 2023-02-19 13:38:37.000000 sacad-2.7.4/sacad.egg-info/requires.txt
--rw-r--r--   0 maxime    (1000) maxime    (1000)        6 2023-02-19 13:38:37.000000 sacad-2.7.4/sacad.egg-info/top_level.txt
--rw-r--r--   0 maxime    (1000) maxime    (1000)       38 2023-02-19 13:38:37.606074 sacad-2.7.4/setup.cfg
--rwxr-xr-x   0 maxime    (1000) maxime    (1000)     2203 2022-08-14 13:39:46.000000 sacad-2.7.4/setup.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)       16 2019-07-25 19:04:11.000000 sacad-2.7.4/test-requirements.txt
+drwxr-xr-x   0 maxime    (1000) maxime    (1000)        0 2023-06-13 20:55:23.835111 sacad-2.7.5/
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    16725 2021-03-22 22:25:00.000000 sacad-2.7.5/LICENSE
+-rw-r--r--   0 maxime    (1000) maxime    (1000)       65 2019-07-25 19:04:11.000000 sacad-2.7.5/MANIFEST.in
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     6720 2023-06-13 20:55:23.835111 sacad-2.7.5/PKG-INFO
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     5615 2023-01-01 13:26:30.000000 sacad-2.7.5/README.md
+-rw-r--r--   0 maxime    (1000) maxime    (1000)      148 2022-11-25 19:21:00.000000 sacad-2.7.5/requirements.txt
+drwxr-xr-x   0 maxime    (1000) maxime    (1000)        0 2023-06-13 20:55:23.835111 sacad-2.7.5/sacad/
+-rwxr-xr-x   0 maxime    (1000) maxime    (1000)     7477 2023-06-13 20:55:01.000000 sacad-2.7.5/sacad/__init__.py
+-rwxr-xr-x   0 maxime    (1000) maxime    (1000)      138 2021-03-23 21:52:59.000000 sacad-2.7.5/sacad/__main__.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     1040 2022-03-14 16:55:38.000000 sacad-2.7.5/sacad/colored_logging.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    29963 2022-12-20 22:27:31.000000 sacad-2.7.5/sacad/cover.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     9531 2022-09-11 21:04:47.000000 sacad-2.7.5/sacad/http_helpers.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)      487 2021-03-23 21:32:50.000000 sacad-2.7.5/sacad/mkstemp_ctx.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     3235 2022-01-29 19:52:16.000000 sacad-2.7.5/sacad/rate_watcher.py
+-rwxr-xr-x   0 maxime    (1000) maxime    (1000)    17443 2023-02-18 20:52:01.000000 sacad-2.7.5/sacad/recurse.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)      742 2022-01-29 19:52:16.000000 sacad-2.7.5/sacad/redo.py
+drwxr-xr-x   0 maxime    (1000) maxime    (1000)        0 2023-06-13 20:55:23.835111 sacad-2.7.5/sacad/sources/
+-rw-r--r--   0 maxime    (1000) maxime    (1000)      600 2022-09-11 21:22:43.000000 sacad-2.7.5/sacad/sources/__init__.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)      998 2023-06-13 17:42:24.000000 sacad-2.7.5/sacad/sources/amazonbase.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     6465 2022-08-16 13:04:23.000000 sacad-2.7.5/sacad/sources/amazoncd.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     6423 2022-08-16 13:04:23.000000 sacad-2.7.5/sacad/sources/amazondigital.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     9337 2022-11-25 19:34:05.000000 sacad-2.7.5/sacad/sources/base.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     2787 2022-08-16 13:04:23.000000 sacad-2.7.5/sacad/sources/deezer.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     3047 2022-12-17 14:27:31.000000 sacad-2.7.5/sacad/sources/discogs.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     2625 2022-09-11 21:33:52.000000 sacad-2.7.5/sacad/sources/itunes.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     3543 2022-08-16 13:04:23.000000 sacad-2.7.5/sacad/sources/lastfm.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     1433 2022-01-29 19:52:16.000000 sacad-2.7.5/sacad/tqdm_logging.py
+drwxr-xr-x   0 maxime    (1000) maxime    (1000)        0 2023-06-13 20:55:23.835111 sacad-2.7.5/sacad.egg-info/
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     6720 2023-06-13 20:55:23.000000 sacad-2.7.5/sacad.egg-info/PKG-INFO
+-rw-r--r--   0 maxime    (1000) maxime    (1000)      677 2023-06-13 20:55:23.000000 sacad-2.7.5/sacad.egg-info/SOURCES.txt
+-rw-r--r--   0 maxime    (1000) maxime    (1000)        1 2023-06-13 20:55:23.000000 sacad-2.7.5/sacad.egg-info/dependency_links.txt
+-rw-r--r--   0 maxime    (1000) maxime    (1000)       72 2023-06-13 20:55:23.000000 sacad-2.7.5/sacad.egg-info/entry_points.txt
+-rw-r--r--   0 maxime    (1000) maxime    (1000)      148 2023-06-13 20:55:23.000000 sacad-2.7.5/sacad.egg-info/requires.txt
+-rw-r--r--   0 maxime    (1000) maxime    (1000)        6 2023-06-13 20:55:23.000000 sacad-2.7.5/sacad.egg-info/top_level.txt
+-rw-r--r--   0 maxime    (1000) maxime    (1000)       38 2023-06-13 20:55:23.835111 sacad-2.7.5/setup.cfg
+-rwxr-xr-x   0 maxime    (1000) maxime    (1000)     2203 2022-08-14 13:39:46.000000 sacad-2.7.5/setup.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)       16 2019-07-25 19:04:11.000000 sacad-2.7.5/test-requirements.txt
```

### Comparing `sacad-2.7.4/LICENSE` & `sacad-2.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sacad-2.7.4/PKG-INFO` & `sacad-2.7.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: sacad
-Version: 2.7.4
+Version: 2.7.5
 Summary: Search and download music album covers
 Home-page: https://github.com/desbma/sacad
+Download-URL: https://github.com/desbma/sacad/archive/2.7.5.tar.gz
 Author: desbma
-License: UNKNOWN
-Download-URL: https://github.com/desbma/sacad/archive/2.7.4.tar.gz
 Keywords: download,album,cover,art,albumart,music
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -133,9 +131,7 @@
 - `updateHttpHeaders(self, headers)` (optional)
 
 See comments in the code for more information.
 
 ## License
 
 [Mozilla Public License Version 2.0](https://www.mozilla.org/MPL/2.0/)
-
-
```

### Comparing `sacad-2.7.4/README.md` & `sacad-2.7.5/README.md`

 * *Files identical despite different names*

### Comparing `sacad-2.7.4/sacad/__init__.py` & `sacad-2.7.5/sacad/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 
 """ Smart Automatic Cover Art Downloader : search and download music album covers. """
 
-__version__ = "2.7.4"
+__version__ = "2.7.5"
 __author__ = "desbma"
 __license__ = "MPL 2.0"
 
 import argparse
 import asyncio
 import functools
 import inspect
```

### Comparing `sacad-2.7.4/sacad/colored_logging.py` & `sacad-2.7.5/sacad/colored_logging.py`

 * *Files identical despite different names*

### Comparing `sacad-2.7.4/sacad/cover.py` & `sacad-2.7.5/sacad/cover.py`

 * *Files identical despite different names*

### Comparing `sacad-2.7.4/sacad/http_helpers.py` & `sacad-2.7.5/sacad/http_helpers.py`

 * *Files identical despite different names*

### Comparing `sacad-2.7.4/sacad/rate_watcher.py` & `sacad-2.7.5/sacad/rate_watcher.py`

 * *Files identical despite different names*

### Comparing `sacad-2.7.4/sacad/recurse.py` & `sacad-2.7.5/sacad/recurse.py`

 * *Files identical despite different names*

### Comparing `sacad-2.7.4/sacad/redo.py` & `sacad-2.7.5/sacad/redo.py`

 * *Files identical despite different names*

### Comparing `sacad-2.7.4/sacad/sources/__init__.py` & `sacad-2.7.5/sacad/sources/__init__.py`

 * *Files identical despite different names*

### Comparing `sacad-2.7.4/sacad/sources/amazoncd.py` & `sacad-2.7.5/sacad/sources/amazoncd.py`

 * *Files identical despite different names*

### Comparing `sacad-2.7.4/sacad/sources/amazondigital.py` & `sacad-2.7.5/sacad/sources/amazondigital.py`

 * *Files identical despite different names*

### Comparing `sacad-2.7.4/sacad/sources/base.py` & `sacad-2.7.5/sacad/sources/base.py`

 * *Files identical despite different names*

### Comparing `sacad-2.7.4/sacad/sources/deezer.py` & `sacad-2.7.5/sacad/sources/deezer.py`

 * *Files identical despite different names*

### Comparing `sacad-2.7.4/sacad/sources/discogs.py` & `sacad-2.7.5/sacad/sources/discogs.py`

 * *Files identical despite different names*

### Comparing `sacad-2.7.4/sacad/sources/itunes.py` & `sacad-2.7.5/sacad/sources/itunes.py`

 * *Files identical despite different names*

### Comparing `sacad-2.7.4/sacad/sources/lastfm.py` & `sacad-2.7.5/sacad/sources/lastfm.py`

 * *Files identical despite different names*

### Comparing `sacad-2.7.4/sacad/tqdm_logging.py` & `sacad-2.7.5/sacad/tqdm_logging.py`

 * *Files identical despite different names*

### Comparing `sacad-2.7.4/sacad.egg-info/PKG-INFO` & `sacad-2.7.5/sacad.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: sacad
-Version: 2.7.4
+Version: 2.7.5
 Summary: Search and download music album covers
 Home-page: https://github.com/desbma/sacad
+Download-URL: https://github.com/desbma/sacad/archive/2.7.5.tar.gz
 Author: desbma
-License: UNKNOWN
-Download-URL: https://github.com/desbma/sacad/archive/2.7.4.tar.gz
 Keywords: download,album,cover,art,albumart,music
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -133,9 +131,7 @@
 - `updateHttpHeaders(self, headers)` (optional)
 
 See comments in the code for more information.
 
 ## License
 
 [Mozilla Public License Version 2.0](https://www.mozilla.org/MPL/2.0/)
-
-
```

### Comparing `sacad-2.7.4/sacad.egg-info/SOURCES.txt` & `sacad-2.7.5/sacad.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sacad-2.7.4/setup.py` & `sacad-2.7.5/setup.py`

 * *Files identical despite different names*

