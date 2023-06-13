# Comparing `tmp/acapela_downloader_py-0.1.3.tar.gz` & `tmp/acapela_downloader_py-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acapela_downloader_py-0.1.3.tar", last modified: Tue Jun 13 15:38:33 2023, max compression
+gzip compressed data, was "acapela_downloader_py-0.1.4.tar", last modified: Tue Jun 13 15:45:37 2023, max compression
```

## Comparing `acapela_downloader_py-0.1.3.tar` & `acapela_downloader_py-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:38:33.604509 acapela_downloader_py-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-13 15:38:23.000000 acapela_downloader_py-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-13 15:38:33.604509 acapela_downloader_py-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-13 15:38:23.000000 acapela_downloader_py-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-13 15:38:23.000000 acapela_downloader_py-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 15:38:33.604509 acapela_downloader_py-0.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:38:33.604509 acapela_downloader_py-0.1.3/src/
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-13 15:38:23.000000 acapela_downloader_py-0.1.3/src/acapela.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:38:33.604509 acapela_downloader_py-0.1.3/src/acapela_downloader_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-13 15:38:33.000000 acapela_downloader_py-0.1.3/src/acapela_downloader_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-13 15:38:33.000000 acapela_downloader_py-0.1.3/src/acapela_downloader_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 15:38:33.000000 acapela_downloader_py-0.1.3/src/acapela_downloader_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-13 15:38:33.000000 acapela_downloader_py-0.1.3/src/acapela_downloader_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-06-13 15:38:23.000000 acapela_downloader_py-0.1.3/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:45:37.862642 acapela_downloader_py-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-13 15:45:20.000000 acapela_downloader_py-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-13 15:45:37.862642 acapela_downloader_py-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-13 15:45:20.000000 acapela_downloader_py-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-13 15:45:20.000000 acapela_downloader_py-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 15:45:37.862642 acapela_downloader_py-0.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:45:37.862642 acapela_downloader_py-0.1.4/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-13 15:45:20.000000 acapela_downloader_py-0.1.4/src/acapela.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:45:37.862642 acapela_downloader_py-0.1.4/src/acapela_downloader_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-13 15:45:37.000000 acapela_downloader_py-0.1.4/src/acapela_downloader_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-13 15:45:37.000000 acapela_downloader_py-0.1.4/src/acapela_downloader_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 15:45:37.000000 acapela_downloader_py-0.1.4/src/acapela_downloader_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-13 15:45:37.000000 acapela_downloader_py-0.1.4/src/acapela_downloader_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-06-13 15:45:20.000000 acapela_downloader_py-0.1.4/src/utils.py
```

### Comparing `acapela_downloader_py-0.1.3/LICENSE` & `acapela_downloader_py-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `acapela_downloader_py-0.1.3/PKG-INFO` & `acapela_downloader_py-0.1.4/src/acapela_downloader_py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: acapela_downloader_py
-Version: 0.1.3
+Name: acapela-downloader-py
+Version: 0.1.4
 Summary: Acapela pwned but in Python.
 Author: JWKK
 Project-URL: Homepage, https://memerdev.com
 Project-URL: GitHub, https://memerdev.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `acapela_downloader_py-0.1.3/src/acapela_downloader_py.egg-info/PKG-INFO` & `acapela_downloader_py-0.1.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: acapela-downloader-py
-Version: 0.1.3
+Name: acapela_downloader_py
+Version: 0.1.4
 Summary: Acapela pwned but in Python.
 Author: JWKK
 Project-URL: Homepage, https://memerdev.com
 Project-URL: GitHub, https://memerdev.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `acapela_downloader_py-0.1.3/src/utils.py` & `acapela_downloader_py-0.1.4/src/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,17 +4,14 @@
 from datetime import time
 from time import sleep
 
 from requests import post
 
 debug_mode = False
 
-def set_debug_mode(active):
-    global debug_mode
-    debug_mode = active
 
 NONCE_ENDPOINT = "https://acapelavoices.acapela-group.com/index/getnonce/"
 SYNTHESIZER_ENDPOINT = "https://www.acapela-group.com:8443/Services/Synthesizer"
 cached_nonce = ""
 cached_email = ""
```

