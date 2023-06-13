# Comparing `tmp/pitop.core-0.31.0.post2.tar.gz` & `tmp/pitop.core-0.31.0.post3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pitop.core-0.31.0.post2.tar", last modified: Mon May 22 19:13:11 2023, max compression
+gzip compressed data, was "dist/pitop.core-0.31.0.post3.tar", last modified: Tue Jun 13 16:41:52 2023, max compression
```

## Comparing `pitop.core-0.31.0.post2.tar` & `pitop.core-0.31.0.post3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:13:11.000000 pitop.core-0.31.0.post2/
--rw-r--r--   0 runner    (1001) docker     (122)       32 2023-05-22 19:12:55.000000 pitop.core-0.31.0.post2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      962 2023-05-22 19:13:11.000000 pitop.core-0.31.0.post2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      130 2023-05-22 19:12:55.000000 pitop.core-0.31.0.post2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:13:11.000000 pitop.core-0.31.0.post2/pitop/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:13:11.000000 pitop.core-0.31.0.post2/pitop/core/
--rw-r--r--   0 runner    (1001) docker     (122)     1663 2023-05-22 19:12:55.000000 pitop.core-0.31.0.post2/pitop/core/ImageFunctions.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-22 19:12:55.000000 pitop.core-0.31.0.post2/pitop/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      175 2023-05-22 19:12:55.000000 pitop.core-0.31.0.post2/pitop/core/data_structures.py
--rw-r--r--   0 runner    (1001) docker     (122)      100 2023-05-22 19:12:55.000000 pitop.core-0.31.0.post2/pitop/core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)      308 2023-05-22 19:12:55.000000 pitop.core-0.31.0.post2/pitop/core/import_opencv.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:13:11.000000 pitop.core-0.31.0.post2/pitop/core/mixins/
--rw-r--r--   0 runner    (1001) docker     (122)      207 2023-05-22 19:12:55.000000 pitop.core-0.31.0.post2/pitop/core/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3309 2023-05-22 19:12:55.000000 pitop.core-0.31.0.post2/pitop/core/mixins/componentable.py
--rw-r--r--   0 runner    (1001) docker     (122)     2737 2023-05-22 19:12:55.000000 pitop.core-0.31.0.post2/pitop/core/mixins/recreatable.py
--rw-r--r--   0 runner    (1001) docker     (122)     1143 2023-05-22 19:12:55.000000 pitop.core-0.31.0.post2/pitop/core/mixins/stateful.py
--rw-r--r--   0 runner    (1001) docker     (122)      532 2023-05-22 19:12:55.000000 pitop.core-0.31.0.post2/pitop/core/mixins/supports_battery.py
--rw-r--r--   0 runner    (1001) docker     (122)      625 2023-05-22 19:12:55.000000 pitop.core-0.31.0.post2/pitop/core/mixins/supports_miniscreen.py
--rw-r--r--   0 runner    (1001) docker     (122)      325 2023-05-22 19:12:55.000000 pitop.core-0.31.0.post2/pitop/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:13:11.000000 pitop.core-0.31.0.post2/pitop.core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      962 2023-05-22 19:13:11.000000 pitop.core-0.31.0.post2/pitop.core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      562 2023-05-22 19:13:11.000000 pitop.core-0.31.0.post2/pitop.core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-22 19:13:11.000000 pitop.core-0.31.0.post2/pitop.core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       90 2023-05-22 19:13:11.000000 pitop.core-0.31.0.post2/pitop.core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-05-22 19:13:11.000000 pitop.core-0.31.0.post2/pitop.core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-22 19:13:11.000000 pitop.core-0.31.0.post2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2017 2023-05-22 19:12:55.000000 pitop.core-0.31.0.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 16:41:52.000000 pitop.core-0.31.0.post3/
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-06-13 16:41:37.000000 pitop.core-0.31.0.post3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      962 2023-06-13 16:41:52.000000 pitop.core-0.31.0.post3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      130 2023-06-13 16:41:37.000000 pitop.core-0.31.0.post3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 16:41:52.000000 pitop.core-0.31.0.post3/pitop/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 16:41:52.000000 pitop.core-0.31.0.post3/pitop/core/
+-rw-r--r--   0 runner    (1001) docker     (122)     1663 2023-06-13 16:41:37.000000 pitop.core-0.31.0.post3/pitop/core/ImageFunctions.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-13 16:41:37.000000 pitop.core-0.31.0.post3/pitop/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      175 2023-06-13 16:41:37.000000 pitop.core-0.31.0.post3/pitop/core/data_structures.py
+-rw-r--r--   0 runner    (1001) docker     (122)      100 2023-06-13 16:41:37.000000 pitop.core-0.31.0.post3/pitop/core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)      308 2023-06-13 16:41:37.000000 pitop.core-0.31.0.post3/pitop/core/import_opencv.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 16:41:52.000000 pitop.core-0.31.0.post3/pitop/core/mixins/
+-rw-r--r--   0 runner    (1001) docker     (122)      207 2023-06-13 16:41:37.000000 pitop.core-0.31.0.post3/pitop/core/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3309 2023-06-13 16:41:37.000000 pitop.core-0.31.0.post3/pitop/core/mixins/componentable.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2737 2023-06-13 16:41:37.000000 pitop.core-0.31.0.post3/pitop/core/mixins/recreatable.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1143 2023-06-13 16:41:37.000000 pitop.core-0.31.0.post3/pitop/core/mixins/stateful.py
+-rw-r--r--   0 runner    (1001) docker     (122)      532 2023-06-13 16:41:37.000000 pitop.core-0.31.0.post3/pitop/core/mixins/supports_battery.py
+-rw-r--r--   0 runner    (1001) docker     (122)      625 2023-06-13 16:41:37.000000 pitop.core-0.31.0.post3/pitop/core/mixins/supports_miniscreen.py
+-rw-r--r--   0 runner    (1001) docker     (122)      325 2023-06-13 16:41:37.000000 pitop.core-0.31.0.post3/pitop/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 16:41:52.000000 pitop.core-0.31.0.post3/pitop.core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      962 2023-06-13 16:41:52.000000 pitop.core-0.31.0.post3/pitop.core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      562 2023-06-13 16:41:52.000000 pitop.core-0.31.0.post3/pitop.core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-13 16:41:52.000000 pitop.core-0.31.0.post3/pitop.core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       90 2023-06-13 16:41:52.000000 pitop.core-0.31.0.post3/pitop.core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-06-13 16:41:52.000000 pitop.core-0.31.0.post3/pitop.core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-13 16:41:52.000000 pitop.core-0.31.0.post3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2017 2023-06-13 16:41:37.000000 pitop.core-0.31.0.post3/setup.py
```

### Comparing `pitop.core-0.31.0.post2/PKG-INFO` & `pitop.core-0.31.0.post3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pitop.core
-Version: 0.31.0.post2
+Version: 0.31.0.post3
 Summary: pi-top Python SDK.
 Home-page: https://github.com/pi-top/pi-top-Python-SDK
 Author: pi-top
 Author-email: deb-maintainers@pi-top.com
 License: Apache Software License
 Description: ===========================
         pi-top Python Core
```

### Comparing `pitop.core-0.31.0.post2/pitop/core/ImageFunctions.py` & `pitop.core-0.31.0.post3/pitop/core/ImageFunctions.py`

 * *Files identical despite different names*

### Comparing `pitop.core-0.31.0.post2/pitop/core/mixins/componentable.py` & `pitop.core-0.31.0.post3/pitop/core/mixins/componentable.py`

 * *Files identical despite different names*

### Comparing `pitop.core-0.31.0.post2/pitop/core/mixins/recreatable.py` & `pitop.core-0.31.0.post3/pitop/core/mixins/recreatable.py`

 * *Files identical despite different names*

### Comparing `pitop.core-0.31.0.post2/pitop/core/mixins/stateful.py` & `pitop.core-0.31.0.post3/pitop/core/mixins/stateful.py`

 * *Files identical despite different names*

### Comparing `pitop.core-0.31.0.post2/pitop/core/mixins/supports_battery.py` & `pitop.core-0.31.0.post3/pitop/core/mixins/supports_battery.py`

 * *Files identical despite different names*

### Comparing `pitop.core-0.31.0.post2/pitop/core/mixins/supports_miniscreen.py` & `pitop.core-0.31.0.post3/pitop/core/mixins/supports_miniscreen.py`

 * *Files identical despite different names*

### Comparing `pitop.core-0.31.0.post2/pitop.core.egg-info/PKG-INFO` & `pitop.core-0.31.0.post3/pitop.core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pitop.core
-Version: 0.31.0.post2
+Version: 0.31.0.post3
 Summary: pi-top Python SDK.
 Home-page: https://github.com/pi-top/pi-top-Python-SDK
 Author: pi-top
 Author-email: deb-maintainers@pi-top.com
 License: Apache Software License
 Description: ===========================
         pi-top Python Core
```

### Comparing `pitop.core-0.31.0.post2/pitop.core.egg-info/SOURCES.txt` & `pitop.core-0.31.0.post3/pitop.core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pitop.core-0.31.0.post2/setup.py` & `pitop.core-0.31.0.post3/setup.py`

 * *Files identical despite different names*

