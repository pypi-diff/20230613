# Comparing `tmp/projen-0.71.91.tar.gz` & `tmp/projen-0.71.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "projen-0.71.91.tar", last modified: Mon Jun 12 12:33:01 2023, max compression
+gzip compressed data, was "projen-0.71.92.tar", last modified: Tue Jun 13 10:58:33 2023, max compression
```

## Comparing `projen-0.71.91.tar` & `projen-0.71.92.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:33:01.615179 projen-0.71.91/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-12 12:32:49.000000 projen-0.71.91/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-12 12:32:49.000000 projen-0.71.91/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    55404 2023-06-12 12:33:01.615179 projen-0.71.91/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    54524 2023-06-12 12:32:49.000000 projen-0.71.91/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-12 12:32:49.000000 projen-0.71.91/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 12:33:01.615179 projen-0.71.91/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-06-12 12:32:49.000000 projen-0.71.91/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:33:01.603179 projen-0.71.91/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:33:01.603179 projen-0.71.91/src/projen/
--rw-r--r--   0 runner    (1001) docker     (123)   593914 2023-06-12 12:32:49.000000 projen-0.71.91/src/projen/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:33:01.603179 projen-0.71.91/src/projen/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-12 12:32:49.000000 projen-0.71.91/src/projen/_jsii/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:33:01.607179 projen-0.71.91/src/projen/_jsii/bin/
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-12 12:32:49.000000 projen-0.71.91/src/projen/_jsii/bin/projen
--rw-r--r--   0 runner    (1001) docker     (123)  2731139 2023-06-12 12:32:49.000000 projen-0.71.91/src/projen/_jsii/projen@0.71.91.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:33:01.607179 projen-0.71.91/src/projen/awscdk/
--rw-r--r--   0 runner    (1001) docker     (123)  1036394 2023-06-12 12:32:49.000000 projen-0.71.91/src/projen/awscdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:33:01.607179 projen-0.71.91/src/projen/build/
--rw-r--r--   0 runner    (1001) docker     (123)    39873 2023-06-12 12:32:49.000000 projen-0.71.91/src/projen/build/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:33:01.611179 projen-0.71.91/src/projen/cdk/
--rw-r--r--   0 runner    (1001) docker     (123)   478039 2023-06-12 12:32:49.000000 projen-0.71.91/src/projen/cdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:33:01.611179 projen-0.71.91/src/projen/cdk8s/
--rw-r--r--   0 runner    (1001) docker     (123)   572593 2023-06-12 12:32:49.000000 projen-0.71.91/src/projen/cdk8s/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:33:01.611179 projen-0.71.91/src/projen/cdktf/
--rw-r--r--   0 runner    (1001) docker     (123)   211860 2023-06-12 12:32:49.000000 projen-0.71.91/src/projen/cdktf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:33:01.611179 projen-0.71.91/src/projen/circleci/
--rw-r--r--   0 runner    (1001) docker     (123)    75837 2023-06-12 12:32:49.000000 projen-0.71.91/src/projen/circleci/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:33:01.611179 projen-0.71.91/src/projen/github/
--rw-r--r--   0 runner    (1001) docker     (123)   275214 2023-06-12 12:32:49.000000 projen-0.71.91/src/projen/github/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:33:01.611179 projen-0.71.91/src/projen/github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)   235582 2023-06-12 12:32:49.000000 projen-0.71.91/src/projen/github/workflows/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:33:01.611179 projen-0.71.91/src/projen/gitlab/
--rw-r--r--   0 runner    (1001) docker     (123)   196190 2023-06-12 12:32:49.000000 projen-0.71.91/src/projen/gitlab/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:33:01.611179 projen-0.71.91/src/projen/java/
--rw-r--r--   0 runner    (1001) docker     (123)   175246 2023-06-12 12:32:49.000000 projen-0.71.91/src/projen/java/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:33:01.611179 projen-0.71.91/src/projen/javascript/
--rw-r--r--   0 runner    (1001) docker     (123)   604594 2023-06-12 12:32:49.000000 projen-0.71.91/src/projen/javascript/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 12:32:49.000000 projen-0.71.91/src/projen/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:33:01.615179 projen-0.71.91/src/projen/python/
--rw-r--r--   0 runner    (1001) docker     (123)   190514 2023-06-12 12:32:49.000000 projen-0.71.91/src/projen/python/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:33:01.615179 projen-0.71.91/src/projen/release/
--rw-r--r--   0 runner    (1001) docker     (123)   246151 2023-06-12 12:32:49.000000 projen-0.71.91/src/projen/release/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:33:01.615179 projen-0.71.91/src/projen/typescript/
--rw-r--r--   0 runner    (1001) docker     (123)   427088 2023-06-12 12:32:49.000000 projen-0.71.91/src/projen/typescript/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:33:01.615179 projen-0.71.91/src/projen/vscode/
--rw-r--r--   0 runner    (1001) docker     (123)    54316 2023-06-12 12:32:49.000000 projen-0.71.91/src/projen/vscode/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:33:01.615179 projen-0.71.91/src/projen/web/
--rw-r--r--   0 runner    (1001) docker     (123)   750808 2023-06-12 12:32:49.000000 projen-0.71.91/src/projen/web/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 12:33:01.603179 projen-0.71.91/src/projen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    55404 2023-06-12 12:33:01.000000 projen-0.71.91/src/projen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-12 12:33:01.000000 projen-0.71.91/src/projen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 12:33:01.000000 projen-0.71.91/src/projen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-12 12:33:01.000000 projen-0.71.91/src/projen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-12 12:33:01.000000 projen-0.71.91/src/projen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:58:33.245155 projen-0.71.92/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-13 10:58:19.000000 projen-0.71.92/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-13 10:58:20.000000 projen-0.71.92/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    55404 2023-06-13 10:58:33.241155 projen-0.71.92/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    54524 2023-06-13 10:58:20.000000 projen-0.71.92/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-13 10:58:20.000000 projen-0.71.92/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 10:58:33.245155 projen-0.71.92/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-06-13 10:58:20.000000 projen-0.71.92/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:58:33.229155 projen-0.71.92/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:58:33.233155 projen-0.71.92/src/projen/
+-rw-r--r--   0 runner    (1001) docker     (123)   593914 2023-06-13 10:58:20.000000 projen-0.71.92/src/projen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:58:33.233155 projen-0.71.92/src/projen/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-13 10:58:20.000000 projen-0.71.92/src/projen/_jsii/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:58:33.233155 projen-0.71.92/src/projen/_jsii/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-13 10:58:20.000000 projen-0.71.92/src/projen/_jsii/bin/projen
+-rw-r--r--   0 runner    (1001) docker     (123)  2731551 2023-06-13 10:58:19.000000 projen-0.71.92/src/projen/_jsii/projen@0.71.92.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:58:33.237155 projen-0.71.92/src/projen/awscdk/
+-rw-r--r--   0 runner    (1001) docker     (123)  1036394 2023-06-13 10:58:20.000000 projen-0.71.92/src/projen/awscdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:58:33.237155 projen-0.71.92/src/projen/build/
+-rw-r--r--   0 runner    (1001) docker     (123)    39873 2023-06-13 10:58:20.000000 projen-0.71.92/src/projen/build/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:58:33.237155 projen-0.71.92/src/projen/cdk/
+-rw-r--r--   0 runner    (1001) docker     (123)   478039 2023-06-13 10:58:20.000000 projen-0.71.92/src/projen/cdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:58:33.237155 projen-0.71.92/src/projen/cdk8s/
+-rw-r--r--   0 runner    (1001) docker     (123)   572593 2023-06-13 10:58:20.000000 projen-0.71.92/src/projen/cdk8s/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:58:33.237155 projen-0.71.92/src/projen/cdktf/
+-rw-r--r--   0 runner    (1001) docker     (123)   211860 2023-06-13 10:58:20.000000 projen-0.71.92/src/projen/cdktf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:58:33.237155 projen-0.71.92/src/projen/circleci/
+-rw-r--r--   0 runner    (1001) docker     (123)    75837 2023-06-13 10:58:20.000000 projen-0.71.92/src/projen/circleci/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:58:33.237155 projen-0.71.92/src/projen/github/
+-rw-r--r--   0 runner    (1001) docker     (123)   275214 2023-06-13 10:58:20.000000 projen-0.71.92/src/projen/github/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:58:33.237155 projen-0.71.92/src/projen/github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)   235582 2023-06-13 10:58:20.000000 projen-0.71.92/src/projen/github/workflows/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:58:33.241155 projen-0.71.92/src/projen/gitlab/
+-rw-r--r--   0 runner    (1001) docker     (123)   196190 2023-06-13 10:58:20.000000 projen-0.71.92/src/projen/gitlab/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:58:33.241155 projen-0.71.92/src/projen/java/
+-rw-r--r--   0 runner    (1001) docker     (123)   175246 2023-06-13 10:58:20.000000 projen-0.71.92/src/projen/java/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:58:33.241155 projen-0.71.92/src/projen/javascript/
+-rw-r--r--   0 runner    (1001) docker     (123)   604594 2023-06-13 10:58:20.000000 projen-0.71.92/src/projen/javascript/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 10:58:20.000000 projen-0.71.92/src/projen/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:58:33.241155 projen-0.71.92/src/projen/python/
+-rw-r--r--   0 runner    (1001) docker     (123)   190514 2023-06-13 10:58:20.000000 projen-0.71.92/src/projen/python/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:58:33.241155 projen-0.71.92/src/projen/release/
+-rw-r--r--   0 runner    (1001) docker     (123)   246151 2023-06-13 10:58:20.000000 projen-0.71.92/src/projen/release/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:58:33.241155 projen-0.71.92/src/projen/typescript/
+-rw-r--r--   0 runner    (1001) docker     (123)   427088 2023-06-13 10:58:20.000000 projen-0.71.92/src/projen/typescript/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:58:33.241155 projen-0.71.92/src/projen/vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)    54316 2023-06-13 10:58:20.000000 projen-0.71.92/src/projen/vscode/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:58:33.241155 projen-0.71.92/src/projen/web/
+-rw-r--r--   0 runner    (1001) docker     (123)   750808 2023-06-13 10:58:20.000000 projen-0.71.92/src/projen/web/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:58:33.233155 projen-0.71.92/src/projen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    55404 2023-06-13 10:58:33.000000 projen-0.71.92/src/projen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-13 10:58:33.000000 projen-0.71.92/src/projen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 10:58:33.000000 projen-0.71.92/src/projen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-13 10:58:33.000000 projen-0.71.92/src/projen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-13 10:58:33.000000 projen-0.71.92/src/projen.egg-info/top_level.txt
```

### Comparing `projen-0.71.91/LICENSE` & `projen-0.71.92/LICENSE`

 * *Files identical despite different names*

### Comparing `projen-0.71.91/PKG-INFO` & `projen-0.71.92/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: projen
-Version: 0.71.91
+Version: 0.71.92
 Summary: CDK for software projects
 Home-page: https://github.com/projen/projen.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/projen/projen.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `projen-0.71.91/README.md` & `projen-0.71.92/README.md`

 * *Files identical despite different names*

### Comparing `projen-0.71.91/setup.py` & `projen-0.71.92/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "projen",
-    "version": "0.71.91",
+    "version": "0.71.92",
     "description": "CDK for software projects",
     "license": "Apache-2.0",
     "url": "https://github.com/projen/projen.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -38,15 +38,15 @@
         "projen.release",
         "projen.typescript",
         "projen.vscode",
         "projen.web"
     ],
     "package_data": {
         "projen._jsii": [
-            "projen@0.71.91.jsii.tgz"
+            "projen@0.71.92.jsii.tgz"
         ],
         "projen": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `projen-0.71.91/src/projen/__init__.py` & `projen-0.71.92/src/projen/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.71.91/src/projen/awscdk/__init__.py` & `projen-0.71.92/src/projen/awscdk/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.71.91/src/projen/build/__init__.py` & `projen-0.71.92/src/projen/build/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.71.91/src/projen/cdk/__init__.py` & `projen-0.71.92/src/projen/cdk/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.71.91/src/projen/cdk8s/__init__.py` & `projen-0.71.92/src/projen/cdk8s/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.71.91/src/projen/cdktf/__init__.py` & `projen-0.71.92/src/projen/cdktf/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.71.91/src/projen/circleci/__init__.py` & `projen-0.71.92/src/projen/circleci/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.71.91/src/projen/github/__init__.py` & `projen-0.71.92/src/projen/github/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.71.91/src/projen/github/workflows/__init__.py` & `projen-0.71.92/src/projen/github/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.71.91/src/projen/gitlab/__init__.py` & `projen-0.71.92/src/projen/gitlab/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.71.91/src/projen/java/__init__.py` & `projen-0.71.92/src/projen/java/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.71.91/src/projen/javascript/__init__.py` & `projen-0.71.92/src/projen/javascript/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.71.91/src/projen/python/__init__.py` & `projen-0.71.92/src/projen/python/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.71.91/src/projen/release/__init__.py` & `projen-0.71.92/src/projen/release/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.71.91/src/projen/typescript/__init__.py` & `projen-0.71.92/src/projen/typescript/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.71.91/src/projen/vscode/__init__.py` & `projen-0.71.92/src/projen/vscode/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.71.91/src/projen/web/__init__.py` & `projen-0.71.92/src/projen/web/__init__.py`

 * *Files identical despite different names*

### Comparing `projen-0.71.91/src/projen.egg-info/PKG-INFO` & `projen-0.71.92/src/projen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: projen
-Version: 0.71.91
+Version: 0.71.92
 Summary: CDK for software projects
 Home-page: https://github.com/projen/projen.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/projen/projen.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `projen-0.71.91/src/projen.egg-info/SOURCES.txt` & `projen-0.71.92/src/projen.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 src/projen/py.typed
 src/projen.egg-info/PKG-INFO
 src/projen.egg-info/SOURCES.txt
 src/projen.egg-info/dependency_links.txt
 src/projen.egg-info/requires.txt
 src/projen.egg-info/top_level.txt
 src/projen/_jsii/__init__.py
-src/projen/_jsii/projen@0.71.91.jsii.tgz
+src/projen/_jsii/projen@0.71.92.jsii.tgz
 src/projen/_jsii/bin/projen
 src/projen/awscdk/__init__.py
 src/projen/build/__init__.py
 src/projen/cdk/__init__.py
 src/projen/cdk8s/__init__.py
 src/projen/cdktf/__init__.py
 src/projen/circleci/__init__.py
```

