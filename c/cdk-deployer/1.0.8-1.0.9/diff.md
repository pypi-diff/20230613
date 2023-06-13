# Comparing `tmp/cdk-deployer-1.0.8.tar.gz` & `tmp/cdk-deployer-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/__w/cdk-deployer/cdk-deployer/dist/python/cdk-deployer-1.0.8.tar", last modified: Mon Dec  6 01:33:59 2021, max compression
+gzip compressed data, was "/__w/cdk-deployer/cdk-deployer/dist/python/cdk-deployer-1.0.9.tar", last modified: Thu Dec  9 14:23:33 2021, max compression
```

## Comparing `cdk-deployer-1.0.8.tar` & `cdk-deployer-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-06 01:33:59.000000 cdk-deployer-1.0.8/
--rw-r--r--   0 root         (0) root         (0)    10142 2021-12-06 01:33:54.000000 cdk-deployer-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2021-12-06 01:33:54.000000 cdk-deployer-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)       67 2021-12-06 01:33:54.000000 cdk-deployer-1.0.8/NOTICE
--rw-r--r--   0 root         (0) root         (0)     4312 2021-12-06 01:33:59.000000 cdk-deployer-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3361 2021-12-06 01:33:54.000000 cdk-deployer-1.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)      106 2021-12-06 01:33:54.000000 cdk-deployer-1.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2021-12-06 01:33:59.000000 cdk-deployer-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2100 2021-12-06 01:33:54.000000 cdk-deployer-1.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-06 01:33:59.000000 cdk-deployer-1.0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-06 01:33:59.000000 cdk-deployer-1.0.8/src/cdk_deployer/
--rw-r--r--   0 root         (0) root         (0)    28086 2021-12-06 01:33:54.000000 cdk-deployer-1.0.8/src/cdk_deployer/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-06 01:33:59.000000 cdk-deployer-1.0.8/src/cdk_deployer/_jsii/
--rw-r--r--   0 root         (0) root         (0)      626 2021-12-06 01:33:54.000000 cdk-deployer-1.0.8/src/cdk_deployer/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26633 2021-12-06 01:33:54.000000 cdk-deployer-1.0.8/src/cdk_deployer/_jsii/cdk-deployer@1.0.8.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2021-12-06 01:33:54.000000 cdk-deployer-1.0.8/src/cdk_deployer/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-06 01:33:59.000000 cdk-deployer-1.0.8/src/cdk_deployer.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4312 2021-12-06 01:33:59.000000 cdk-deployer-1.0.8/src/cdk_deployer.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      400 2021-12-06 01:33:59.000000 cdk-deployer-1.0.8/src/cdk_deployer.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-12-06 01:33:59.000000 cdk-deployer-1.0.8/src/cdk_deployer.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      382 2021-12-06 01:33:59.000000 cdk-deployer-1.0.8/src/cdk_deployer.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2021-12-06 01:33:59.000000 cdk-deployer-1.0.8/src/cdk_deployer.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-09 14:23:33.000000 cdk-deployer-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)    10142 2021-12-09 14:23:28.000000 cdk-deployer-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2021-12-09 14:23:28.000000 cdk-deployer-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)       67 2021-12-09 14:23:28.000000 cdk-deployer-1.0.9/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     4312 2021-12-09 14:23:33.000000 cdk-deployer-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3361 2021-12-09 14:23:28.000000 cdk-deployer-1.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      106 2021-12-09 14:23:28.000000 cdk-deployer-1.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2021-12-09 14:23:33.000000 cdk-deployer-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2100 2021-12-09 14:23:28.000000 cdk-deployer-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-09 14:23:33.000000 cdk-deployer-1.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-09 14:23:33.000000 cdk-deployer-1.0.9/src/cdk_deployer/
+-rw-r--r--   0 root         (0) root         (0)    28086 2021-12-09 14:23:28.000000 cdk-deployer-1.0.9/src/cdk_deployer/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-09 14:23:33.000000 cdk-deployer-1.0.9/src/cdk_deployer/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      626 2021-12-09 14:23:28.000000 cdk-deployer-1.0.9/src/cdk_deployer/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26637 2021-12-09 14:23:28.000000 cdk-deployer-1.0.9/src/cdk_deployer/_jsii/cdk-deployer@1.0.9.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2021-12-09 14:23:28.000000 cdk-deployer-1.0.9/src/cdk_deployer/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-09 14:23:33.000000 cdk-deployer-1.0.9/src/cdk_deployer.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4312 2021-12-09 14:23:33.000000 cdk-deployer-1.0.9/src/cdk_deployer.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      400 2021-12-09 14:23:33.000000 cdk-deployer-1.0.9/src/cdk_deployer.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-12-09 14:23:33.000000 cdk-deployer-1.0.9/src/cdk_deployer.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      382 2021-12-09 14:23:33.000000 cdk-deployer-1.0.9/src/cdk_deployer.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2021-12-09 14:23:33.000000 cdk-deployer-1.0.9/src/cdk_deployer.egg-info/top_level.txt
```

### Comparing `cdk-deployer-1.0.8/LICENSE` & `cdk-deployer-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-deployer-1.0.8/PKG-INFO` & `cdk-deployer-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-deployer
-Version: 1.0.8
+Version: 1.0.9
 Summary: A construct library for deploying artifacts via CodeDeploy inside of a AWS CDK application.
 Home-page: https://github.com/cdklabs/cdk-deployer
 Author: Jeff Gardner
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-deployer
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `cdk-deployer-1.0.8/README.md` & `cdk-deployer-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `cdk-deployer-1.0.8/setup.py` & `cdk-deployer-1.0.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-deployer",
-    "version": "1.0.8",
+    "version": "1.0.9",
     "description": "A construct library for deploying artifacts via CodeDeploy inside of a AWS CDK application.",
     "license": "Apache-2.0",
     "url": "https://github.com/cdklabs/cdk-deployer",
     "long_description_content_type": "text/markdown",
     "author": "Jeff Gardner",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk_deployer",
         "cdk_deployer._jsii"
     ],
     "package_data": {
         "cdk_deployer._jsii": [
-            "cdk-deployer@1.0.8.jsii.tgz"
+            "cdk-deployer@1.0.9.jsii.tgz"
         ],
         "cdk_deployer": [
             "py.typed"
         ]
     },
     "python_requires": ">=3.6",
     "install_requires": [
@@ -40,15 +40,15 @@
         "aws-cdk.aws-iam>=1.116.0, <2.0.0",
         "aws-cdk.aws-lambda>=1.116.0, <2.0.0",
         "aws-cdk.aws-s3-assets>=1.116.0, <2.0.0",
         "aws-cdk.aws-s3>=1.116.0, <2.0.0",
         "aws-cdk.core>=1.116.0, <2.0.0",
         "aws-cdk.custom-resources>=1.116.0, <2.0.0",
         "constructs>=3.2.27, <4.0.0",
-        "jsii>=1.46.0, <2.0.0",
+        "jsii>=1.47.0, <2.0.0",
         "publication>=0.0.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
         "Programming Language :: Python :: 3 :: Only",
```

### Comparing `cdk-deployer-1.0.8/src/cdk_deployer/__init__.py` & `cdk-deployer-1.0.9/src/cdk_deployer/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-deployer-1.0.8/src/cdk_deployer/_jsii/__init__.py` & `cdk-deployer-1.0.9/src/cdk_deployer/_jsii/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import aws_cdk.aws_s3._jsii
 import aws_cdk.aws_s3_assets._jsii
 import aws_cdk.core._jsii
 import aws_cdk.custom_resources._jsii
 import constructs._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
-    "cdk-deployer", "1.0.8", __name__[0:-6], "cdk-deployer@1.0.8.jsii.tgz"
+    "cdk-deployer", "1.0.9", __name__[0:-6], "cdk-deployer@1.0.9.jsii.tgz"
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `cdk-deployer-1.0.8/src/cdk_deployer.egg-info/PKG-INFO` & `cdk-deployer-1.0.9/src/cdk_deployer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-deployer
-Version: 1.0.8
+Version: 1.0.9
 Summary: A construct library for deploying artifacts via CodeDeploy inside of a AWS CDK application.
 Home-page: https://github.com/cdklabs/cdk-deployer
 Author: Jeff Gardner
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-deployer
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

