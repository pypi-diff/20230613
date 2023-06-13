# Comparing `tmp/cdk-monitoring-constructs-5.1.2.tar.gz` & `tmp/cdk-monitoring-constructs-5.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-monitoring-constructs-5.1.2.tar", last modified: Mon Jun 12 00:39:27 2023, max compression
+gzip compressed data, was "cdk-monitoring-constructs-5.1.3.tar", last modified: Tue Jun 13 18:19:26 2023, max compression
```

## Comparing `cdk-monitoring-constructs-5.1.2.tar` & `cdk-monitoring-constructs-5.1.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 00:39:27.972058 cdk-monitoring-constructs-5.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-12 00:39:14.000000 cdk-monitoring-constructs-5.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-12 00:39:14.000000 cdk-monitoring-constructs-5.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-12 00:39:14.000000 cdk-monitoring-constructs-5.1.2/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)    18058 2023-06-12 00:39:27.972058 cdk-monitoring-constructs-5.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17059 2023-06-12 00:39:14.000000 cdk-monitoring-constructs-5.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-12 00:39:14.000000 cdk-monitoring-constructs-5.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 00:39:27.972058 cdk-monitoring-constructs-5.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-06-12 00:39:14.000000 cdk-monitoring-constructs-5.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 00:39:27.964058 cdk-monitoring-constructs-5.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 00:39:27.968058 cdk-monitoring-constructs-5.1.2/src/cdk_monitoring_constructs/
--rw-r--r--   0 runner    (1001) docker     (123)  4432233 2023-06-12 00:39:14.000000 cdk-monitoring-constructs-5.1.2/src/cdk_monitoring_constructs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 00:39:27.968058 cdk-monitoring-constructs-5.1.2/src/cdk_monitoring_constructs/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-12 00:39:14.000000 cdk-monitoring-constructs-5.1.2/src/cdk_monitoring_constructs/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   773381 2023-06-12 00:39:14.000000 cdk-monitoring-constructs-5.1.2/src/cdk_monitoring_constructs/_jsii/cdk-monitoring-constructs@5.1.2.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 00:39:14.000000 cdk-monitoring-constructs-5.1.2/src/cdk_monitoring_constructs/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 00:39:27.968058 cdk-monitoring-constructs-5.1.2/src/cdk_monitoring_constructs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18058 2023-06-12 00:39:27.000000 cdk-monitoring-constructs-5.1.2/src/cdk_monitoring_constructs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-12 00:39:27.000000 cdk-monitoring-constructs-5.1.2/src/cdk_monitoring_constructs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 00:39:27.000000 cdk-monitoring-constructs-5.1.2/src/cdk_monitoring_constructs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-12 00:39:27.000000 cdk-monitoring-constructs-5.1.2/src/cdk_monitoring_constructs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-12 00:39:27.000000 cdk-monitoring-constructs-5.1.2/src/cdk_monitoring_constructs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:19:26.158814 cdk-monitoring-constructs-5.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-13 18:19:06.000000 cdk-monitoring-constructs-5.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-13 18:19:06.000000 cdk-monitoring-constructs-5.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-13 18:19:06.000000 cdk-monitoring-constructs-5.1.3/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)    18058 2023-06-13 18:19:26.158814 cdk-monitoring-constructs-5.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17059 2023-06-13 18:19:06.000000 cdk-monitoring-constructs-5.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-13 18:19:06.000000 cdk-monitoring-constructs-5.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 18:19:26.158814 cdk-monitoring-constructs-5.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-06-13 18:19:06.000000 cdk-monitoring-constructs-5.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:19:26.146813 cdk-monitoring-constructs-5.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:19:26.154814 cdk-monitoring-constructs-5.1.3/src/cdk_monitoring_constructs/
+-rw-r--r--   0 runner    (1001) docker     (123)  4432233 2023-06-13 18:19:06.000000 cdk-monitoring-constructs-5.1.3/src/cdk_monitoring_constructs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:19:26.154814 cdk-monitoring-constructs-5.1.3/src/cdk_monitoring_constructs/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-13 18:19:06.000000 cdk-monitoring-constructs-5.1.3/src/cdk_monitoring_constructs/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   773393 2023-06-13 18:19:06.000000 cdk-monitoring-constructs-5.1.3/src/cdk_monitoring_constructs/_jsii/cdk-monitoring-constructs@5.1.3.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 18:19:06.000000 cdk-monitoring-constructs-5.1.3/src/cdk_monitoring_constructs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:19:26.154814 cdk-monitoring-constructs-5.1.3/src/cdk_monitoring_constructs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18058 2023-06-13 18:19:26.000000 cdk-monitoring-constructs-5.1.3/src/cdk_monitoring_constructs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-13 18:19:26.000000 cdk-monitoring-constructs-5.1.3/src/cdk_monitoring_constructs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 18:19:26.000000 cdk-monitoring-constructs-5.1.3/src/cdk_monitoring_constructs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-13 18:19:26.000000 cdk-monitoring-constructs-5.1.3/src/cdk_monitoring_constructs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-13 18:19:26.000000 cdk-monitoring-constructs-5.1.3/src/cdk_monitoring_constructs.egg-info/top_level.txt
```

### Comparing `cdk-monitoring-constructs-5.1.2/LICENSE` & `cdk-monitoring-constructs-5.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-monitoring-constructs-5.1.2/PKG-INFO` & `cdk-monitoring-constructs-5.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-monitoring-constructs
-Version: 5.1.2
+Version: 5.1.3
 Summary: cdk-monitoring-constructs
 Home-page: https://github.com/cdklabs/cdk-monitoring-constructs
 Author: CDK Monitoring Constructs Team<monitoring-cdk-constructs@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-monitoring-constructs
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-monitoring-constructs-5.1.2/README.md` & `cdk-monitoring-constructs-5.1.3/README.md`

 * *Files identical despite different names*

### Comparing `cdk-monitoring-constructs-5.1.2/setup.py` & `cdk-monitoring-constructs-5.1.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-monitoring-constructs",
-    "version": "5.1.2",
+    "version": "5.1.3",
     "description": "cdk-monitoring-constructs",
     "license": "Apache-2.0",
     "url": "https://github.com/cdklabs/cdk-monitoring-constructs",
     "long_description_content_type": "text/markdown",
     "author": "CDK Monitoring Constructs Team<monitoring-cdk-constructs@amazon.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk_monitoring_constructs",
         "cdk_monitoring_constructs._jsii"
     ],
     "package_data": {
         "cdk_monitoring_constructs._jsii": [
-            "cdk-monitoring-constructs@5.1.2.jsii.tgz"
+            "cdk-monitoring-constructs@5.1.3.jsii.tgz"
         ],
         "cdk_monitoring_constructs": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdk-monitoring-constructs-5.1.2/src/cdk_monitoring_constructs/__init__.py` & `cdk-monitoring-constructs-5.1.3/src/cdk_monitoring_constructs/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-monitoring-constructs-5.1.2/src/cdk_monitoring_constructs.egg-info/PKG-INFO` & `cdk-monitoring-constructs-5.1.3/src/cdk_monitoring_constructs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-monitoring-constructs
-Version: 5.1.2
+Version: 5.1.3
 Summary: cdk-monitoring-constructs
 Home-page: https://github.com/cdklabs/cdk-monitoring-constructs
 Author: CDK Monitoring Constructs Team<monitoring-cdk-constructs@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-monitoring-constructs
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-monitoring-constructs-5.1.2/src/cdk_monitoring_constructs.egg-info/SOURCES.txt` & `cdk-monitoring-constructs-5.1.3/src/cdk_monitoring_constructs.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 src/cdk_monitoring_constructs/py.typed
 src/cdk_monitoring_constructs.egg-info/PKG-INFO
 src/cdk_monitoring_constructs.egg-info/SOURCES.txt
 src/cdk_monitoring_constructs.egg-info/dependency_links.txt
 src/cdk_monitoring_constructs.egg-info/requires.txt
 src/cdk_monitoring_constructs.egg-info/top_level.txt
 src/cdk_monitoring_constructs/_jsii/__init__.py
-src/cdk_monitoring_constructs/_jsii/cdk-monitoring-constructs@5.1.2.jsii.tgz
+src/cdk_monitoring_constructs/_jsii/cdk-monitoring-constructs@5.1.3.jsii.tgz
```

