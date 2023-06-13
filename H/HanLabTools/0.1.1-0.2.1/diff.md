# Comparing `tmp/HanLabTools-0.1.1.tar.gz` & `tmp/HanLabTools-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HanLabTools-0.1.1.tar", last modified: Tue Jun 13 00:35:40 2023, max compression
+gzip compressed data, was "HanLabTools-0.2.1.tar", last modified: Tue Jun 13 00:44:24 2023, max compression
```

## Comparing `HanLabTools-0.1.1.tar` & `HanLabTools-0.2.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:35:39.996290 HanLabTools-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:35:39.996290 HanLabTools-0.1.1/HanLabTools/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-13 00:35:30.000000 HanLabTools-0.1.1/HanLabTools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:35:39.996290 HanLabTools-0.1.1/HanLabTools/config/
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-13 00:35:30.000000 HanLabTools-0.1.1/HanLabTools/config/HanLab.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-13 00:35:30.000000 HanLabTools-0.1.1/HanLabTools/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-13 00:35:30.000000 HanLabTools-0.1.1/HanLabTools/config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-06-13 00:35:30.000000 HanLabTools-0.1.1/HanLabTools/io.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-13 00:35:30.000000 HanLabTools-0.1.1/HanLabTools/processing.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-13 00:35:30.000000 HanLabTools-0.1.1/HanLabTools/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:35:39.996290 HanLabTools-0.1.1/HanLabTools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-13 00:35:39.000000 HanLabTools-0.1.1/HanLabTools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-13 00:35:39.000000 HanLabTools-0.1.1/HanLabTools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 00:35:39.000000 HanLabTools-0.1.1/HanLabTools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-13 00:35:39.000000 HanLabTools-0.1.1/HanLabTools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-13 00:35:39.000000 HanLabTools-0.1.1/HanLabTools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-13 00:35:30.000000 HanLabTools-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-13 00:35:39.996290 HanLabTools-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-13 00:35:30.000000 HanLabTools-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-13 00:35:30.000000 HanLabTools-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 00:35:39.996290 HanLabTools-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-13 00:35:30.000000 HanLabTools-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:44:24.471544 HanLabTools-0.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:44:24.471544 HanLabTools-0.2.1/HanLabTools/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-13 00:44:12.000000 HanLabTools-0.2.1/HanLabTools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:44:24.471544 HanLabTools-0.2.1/HanLabTools/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-13 00:44:12.000000 HanLabTools-0.2.1/HanLabTools/config/HanLab.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-13 00:44:12.000000 HanLabTools-0.2.1/HanLabTools/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-13 00:44:12.000000 HanLabTools-0.2.1/HanLabTools/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-06-13 00:44:12.000000 HanLabTools-0.2.1/HanLabTools/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-13 00:44:12.000000 HanLabTools-0.2.1/HanLabTools/processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-13 00:44:12.000000 HanLabTools-0.2.1/HanLabTools/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 00:44:24.471544 HanLabTools-0.2.1/HanLabTools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-13 00:44:24.000000 HanLabTools-0.2.1/HanLabTools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-13 00:44:24.000000 HanLabTools-0.2.1/HanLabTools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 00:44:24.000000 HanLabTools-0.2.1/HanLabTools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-13 00:44:24.000000 HanLabTools-0.2.1/HanLabTools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-13 00:44:24.000000 HanLabTools-0.2.1/HanLabTools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-13 00:44:12.000000 HanLabTools-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-13 00:44:24.471544 HanLabTools-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-13 00:44:12.000000 HanLabTools-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-13 00:44:12.000000 HanLabTools-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 00:44:24.471544 HanLabTools-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-13 00:44:12.000000 HanLabTools-0.2.1/setup.py
```

### Comparing `HanLabTools-0.1.1/HanLabTools/config/HanLab.cfg` & `HanLabTools-0.2.1/HanLabTools/config/HanLab.cfg`

 * *Files identical despite different names*

### Comparing `HanLabTools-0.1.1/HanLabTools/config/config.py` & `HanLabTools-0.2.1/HanLabTools/config/config.py`

 * *Files identical despite different names*

### Comparing `HanLabTools-0.1.1/HanLabTools/io.py` & `HanLabTools-0.2.1/HanLabTools/io.py`

 * *Files identical despite different names*

### Comparing `HanLabTools-0.1.1/HanLabTools.egg-info/PKG-INFO` & `HanLabTools-0.2.1/HanLabTools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HanLabTools
-Version: 0.1.1
+Version: 0.2.1
 Summary: Import tools for DNPLab specific to the Han Lab
 Home-page: https://github.com/Bridge12Technologies/HanLabTools
 Author: Thorsten Maly
 Author-email: tmaly@bridge12.com
 Project-URL: Tracker, https://github.com/Bridge12Technologies/HanLabTools/issues
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `HanLabTools-0.1.1/LICENSE` & `HanLabTools-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `HanLabTools-0.1.1/PKG-INFO` & `HanLabTools-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HanLabTools
-Version: 0.1.1
+Version: 0.2.1
 Summary: Import tools for DNPLab specific to the Han Lab
 Home-page: https://github.com/Bridge12Technologies/HanLabTools
 Author: Thorsten Maly
 Author-email: tmaly@bridge12.com
 Project-URL: Tracker, https://github.com/Bridge12Technologies/HanLabTools/issues
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `HanLabTools-0.1.1/README.md` & `HanLabTools-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `HanLabTools-0.1.1/setup.py` & `HanLabTools-0.2.1/setup.py`

 * *Files identical despite different names*

