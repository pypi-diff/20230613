# Comparing `tmp/xflow-net-0.0.1.tar.gz` & `tmp/xflow-net-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xflow-net-0.0.1.tar", last modified: Tue Jun 13 15:03:40 2023, max compression
+gzip compressed data, was "xflow-net-0.0.2.tar", last modified: Tue Jun 13 15:06:00 2023, max compression
```

## Comparing `xflow-net-0.0.1.tar` & `xflow-net-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 zc347      (503) staff       (20)        0 2023-06-13 15:03:40.991289 xflow-net-0.0.1/
--rw-r--r--   0 zc347      (503) staff       (20)     1066 2023-06-13 14:51:01.000000 xflow-net-0.0.1/LICENSE
--rw-r--r--   0 zc347      (503) staff       (20)     3944 2023-06-13 15:03:40.991168 xflow-net-0.0.1/PKG-INFO
--rw-r--r--   0 zc347      (503) staff       (20)     3327 2023-06-13 14:51:01.000000 xflow-net-0.0.1/README.md
--rw-r--r--   0 zc347      (503) staff       (20)       38 2023-06-13 15:03:40.991333 xflow-net-0.0.1/setup.cfg
--rw-r--r--   0 zc347      (503) staff       (20)     3685 2023-06-13 15:03:30.000000 xflow-net-0.0.1/setup.py
-drwxr-xr-x   0 zc347      (503) staff       (20)        0 2023-06-13 15:03:40.990300 xflow-net-0.0.1/xflow/
--rw-r--r--   0 zc347      (503) staff       (20)       57 2023-06-13 14:51:01.000000 xflow-net-0.0.1/xflow/__init__.py
--rw-r--r--   0 zc347      (503) staff       (20)      294 2023-06-13 14:51:01.000000 xflow-net-0.0.1/xflow/seed.py
--rw-r--r--   0 zc347      (503) staff       (20)     2639 2023-06-13 14:51:01.000000 xflow-net-0.0.1/xflow/visualization.py
-drwxr-xr-x   0 zc347      (503) staff       (20)        0 2023-06-13 15:03:40.990985 xflow-net-0.0.1/xflow_net.egg-info/
--rw-r--r--   0 zc347      (503) staff       (20)     3944 2023-06-13 15:03:40.000000 xflow-net-0.0.1/xflow_net.egg-info/PKG-INFO
--rw-r--r--   0 zc347      (503) staff       (20)      245 2023-06-13 15:03:40.000000 xflow-net-0.0.1/xflow_net.egg-info/SOURCES.txt
--rw-r--r--   0 zc347      (503) staff       (20)        1 2023-06-13 15:03:40.000000 xflow-net-0.0.1/xflow_net.egg-info/dependency_links.txt
--rw-r--r--   0 zc347      (503) staff       (20)       15 2023-06-13 15:03:40.000000 xflow-net-0.0.1/xflow_net.egg-info/requires.txt
--rw-r--r--   0 zc347      (503) staff       (20)        6 2023-06-13 15:03:40.000000 xflow-net-0.0.1/xflow_net.egg-info/top_level.txt
+drwxr-xr-x   0 zc347      (503) staff       (20)        0 2023-06-13 15:06:00.513281 xflow-net-0.0.2/
+-rw-r--r--   0 zc347      (503) staff       (20)     1066 2023-06-13 14:51:01.000000 xflow-net-0.0.2/LICENSE
+-rw-r--r--   0 zc347      (503) staff       (20)     3944 2023-06-13 15:06:00.513139 xflow-net-0.0.2/PKG-INFO
+-rw-r--r--   0 zc347      (503) staff       (20)     3327 2023-06-13 14:51:01.000000 xflow-net-0.0.2/README.md
+-rw-r--r--   0 zc347      (503) staff       (20)       38 2023-06-13 15:06:00.513336 xflow-net-0.0.2/setup.cfg
+-rw-r--r--   0 zc347      (503) staff       (20)     3685 2023-06-13 15:04:14.000000 xflow-net-0.0.2/setup.py
+drwxr-xr-x   0 zc347      (503) staff       (20)        0 2023-06-13 15:06:00.512296 xflow-net-0.0.2/xflow/
+-rw-r--r--   0 zc347      (503) staff       (20)       57 2023-06-13 14:51:01.000000 xflow-net-0.0.2/xflow/__init__.py
+-rw-r--r--   0 zc347      (503) staff       (20)      294 2023-06-13 14:51:01.000000 xflow-net-0.0.2/xflow/seed.py
+-rw-r--r--   0 zc347      (503) staff       (20)     2639 2023-06-13 14:51:01.000000 xflow-net-0.0.2/xflow/visualization.py
+drwxr-xr-x   0 zc347      (503) staff       (20)        0 2023-06-13 15:06:00.512955 xflow-net-0.0.2/xflow_net.egg-info/
+-rw-r--r--   0 zc347      (503) staff       (20)     3944 2023-06-13 15:06:00.000000 xflow-net-0.0.2/xflow_net.egg-info/PKG-INFO
+-rw-r--r--   0 zc347      (503) staff       (20)      245 2023-06-13 15:06:00.000000 xflow-net-0.0.2/xflow_net.egg-info/SOURCES.txt
+-rw-r--r--   0 zc347      (503) staff       (20)        1 2023-06-13 15:06:00.000000 xflow-net-0.0.2/xflow_net.egg-info/dependency_links.txt
+-rw-r--r--   0 zc347      (503) staff       (20)       15 2023-06-13 15:06:00.000000 xflow-net-0.0.2/xflow_net.egg-info/requires.txt
+-rw-r--r--   0 zc347      (503) staff       (20)        6 2023-06-13 15:06:00.000000 xflow-net-0.0.2/xflow_net.egg-info/top_level.txt
```

### Comparing `xflow-net-0.0.1/LICENSE` & `xflow-net-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xflow-net-0.0.1/PKG-INFO` & `xflow-net-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xflow-net
-Version: 0.0.1
+Version: 0.0.2
 Summary: a python library for graph flow
 Home-page: https://xflow.network/
 Author: XGraphing
 Author-email: zchen@cse.msstate.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `xflow-net-0.0.1/README.md` & `xflow-net-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `xflow-net-0.0.1/setup.py` & `xflow-net-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Package meta-data.
 NAME = 'xflow-net'
 DESCRIPTION = 'a python library for graph flow'
 URL = 'https://xflow.network/'
 EMAIL = 'zchen@cse.msstate.edu'
 AUTHOR = 'XGraphing'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
    'networkx', 'ndlib'
 ]
 
 # What packages are optional?
```

### Comparing `xflow-net-0.0.1/xflow/visualization.py` & `xflow-net-0.0.2/xflow/visualization.py`

 * *Files identical despite different names*

### Comparing `xflow-net-0.0.1/xflow_net.egg-info/PKG-INFO` & `xflow-net-0.0.2/xflow_net.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xflow-net
-Version: 0.0.1
+Version: 0.0.2
 Summary: a python library for graph flow
 Home-page: https://xflow.network/
 Author: XGraphing
 Author-email: zchen@cse.msstate.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

