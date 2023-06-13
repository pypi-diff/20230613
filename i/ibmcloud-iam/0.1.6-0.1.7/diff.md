# Comparing `tmp/ibmcloud-iam-0.1.6.tar.gz` & `tmp/ibmcloud-iam-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ibmcloud-iam-0.1.6.tar", last modified: Fri Nov 12 22:16:46 2021, max compression
+gzip compressed data, was "dist/ibmcloud-iam-0.1.7.tar", last modified: Tue Jun 13 17:20:19 2023, max compression
```

## Comparing `ibmcloud-iam-0.1.6.tar` & `ibmcloud-iam-0.1.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2021-11-12 22:16:46.000000 ibmcloud-iam-0.1.6/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2842 2021-09-01 22:25:25.000000 ibmcloud-iam-0.1.6/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2021-11-12 22:16:46.000000 ibmcloud-iam-0.1.6/ibmcloud_iam.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2021-11-12 22:16:45.000000 ibmcloud-iam-0.1.6/ibmcloud_iam.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3514 2021-11-12 22:16:45.000000 ibmcloud-iam-0.1.6/ibmcloud_iam.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2021-09-13 18:27:07.000000 ibmcloud-iam-0.1.6/ibmcloud_iam.egg-info/not-zip-safe
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       13 2021-11-12 22:16:45.000000 ibmcloud-iam-0.1.6/ibmcloud_iam.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      307 2021-11-12 22:16:45.000000 ibmcloud-iam-0.1.6/ibmcloud_iam.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       78 2021-11-12 22:16:45.000000 ibmcloud-iam-0.1.6/ibmcloud_iam.egg-info/requires.txt
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2021-11-12 22:16:46.000000 ibmcloud-iam-0.1.6/ibmcloud_iam/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3566 2021-09-09 20:43:50.000000 ibmcloud-iam-0.1.6/ibmcloud_iam/pdp.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2266 2021-09-09 20:37:01.000000 ibmcloud-iam-0.1.6/ibmcloud_iam/token.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      576 2021-09-01 02:31:24.000000 ibmcloud-iam-0.1.6/ibmcloud_iam/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11357 2021-09-01 02:31:24.000000 ibmcloud-iam-0.1.6/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3514 2021-11-12 22:16:46.000000 ibmcloud-iam-0.1.6/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2021-11-12 22:16:46.000000 ibmcloud-iam-0.1.6/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1696 2021-11-12 22:15:57.000000 ibmcloud-iam-0.1.6/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-13 17:20:19.000000 ibmcloud-iam-0.1.7/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2842 2021-09-01 22:25:25.000000 ibmcloud-iam-0.1.7/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-13 17:20:19.000000 ibmcloud-iam-0.1.7/ibmcloud_iam.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-13 17:20:19.000000 ibmcloud-iam-0.1.7/ibmcloud_iam.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3514 2023-06-13 17:20:19.000000 ibmcloud-iam-0.1.7/ibmcloud_iam.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-13 17:20:11.000000 ibmcloud-iam-0.1.7/ibmcloud_iam.egg-info/not-zip-safe
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       13 2023-06-13 17:20:19.000000 ibmcloud-iam-0.1.7/ibmcloud_iam.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      307 2023-06-13 17:20:19.000000 ibmcloud-iam-0.1.7/ibmcloud_iam.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       83 2023-06-13 17:20:19.000000 ibmcloud-iam-0.1.7/ibmcloud_iam.egg-info/requires.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-13 17:20:19.000000 ibmcloud-iam-0.1.7/ibmcloud_iam/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3566 2021-09-09 20:43:50.000000 ibmcloud-iam-0.1.7/ibmcloud_iam/pdp.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2266 2021-09-09 20:37:01.000000 ibmcloud-iam-0.1.7/ibmcloud_iam/token.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      576 2021-09-01 02:31:24.000000 ibmcloud-iam-0.1.7/ibmcloud_iam/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11357 2021-09-01 02:31:24.000000 ibmcloud-iam-0.1.7/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3514 2023-06-13 17:20:19.000000 ibmcloud-iam-0.1.7/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-06-13 17:20:19.000000 ibmcloud-iam-0.1.7/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1701 2023-06-13 17:19:07.000000 ibmcloud-iam-0.1.7/setup.py
```

### Comparing `ibmcloud-iam-0.1.6/README.md` & `ibmcloud-iam-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `ibmcloud-iam-0.1.6/ibmcloud_iam.egg-info/PKG-INFO` & `ibmcloud-iam-0.1.7/ibmcloud_iam.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibmcloud-iam
-Version: 0.1.6
+Version: 0.1.7
 Summary: A collection of Python modules used for interacting with IBMCloud IAM API services
 Home-page: https://github.com/mrodden/ibmcloud-iam-python-client
 Author: Mathew Odden
 Author-email: mrodden@us.ibm.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ibmcloud-iam-0.1.6/ibmcloud_iam/pdp.py` & `ibmcloud-iam-0.1.7/ibmcloud_iam/pdp.py`

 * *Files identical despite different names*

### Comparing `ibmcloud-iam-0.1.6/ibmcloud_iam/token.py` & `ibmcloud-iam-0.1.7/ibmcloud_iam/token.py`

 * *Files identical despite different names*

### Comparing `ibmcloud-iam-0.1.6/ibmcloud_iam/__init__.py` & `ibmcloud-iam-0.1.7/ibmcloud_iam/__init__.py`

 * *Files identical despite different names*

### Comparing `ibmcloud-iam-0.1.6/LICENSE` & `ibmcloud-iam-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ibmcloud-iam-0.1.6/PKG-INFO` & `ibmcloud-iam-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibmcloud-iam
-Version: 0.1.6
+Version: 0.1.7
 Summary: A collection of Python modules used for interacting with IBMCloud IAM API services
 Home-page: https://github.com/mrodden/ibmcloud-iam-python-client
 Author: Mathew Odden
 Author-email: mrodden@us.ibm.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ibmcloud-iam-0.1.6/setup.py` & `ibmcloud-iam-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,26 +15,26 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf8") as fh:
     long_desc = fh.read()
 
 setup(
     name="ibmcloud-iam",
-    version="0.1.6",
+    version="0.1.7",
     author="Mathew Odden",
     author_email="mrodden@us.ibm.com",
     url="https://github.com/mrodden/ibmcloud-iam-python-client",
     description="A collection of Python modules used for interacting with IBMCloud IAM API services",
     long_description=long_desc,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     package_data={"ibmcloud_iam": ["py.typed", "*.pyi"]},
     include_package_data=True,
     zip_safe=False,
-    install_requires=["requests[security]", "pyjwt>=2.1.0", "redstone"],
+    install_requires=["requests[security]", "pyjwt>=2.1.0,<2.5", "redstone"],
     extras_require={
         "docs": ["sphinx>=3.1", "sphinx_rtd_theme"],
     },
     entry_points={},
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.5",
```

