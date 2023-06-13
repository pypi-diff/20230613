# Comparing `tmp/yplib-0.2.6.tar.gz` & `tmp/yplib-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-0.2.6.tar", last modified: Tue Jun 13 00:30:38 2023, max compression
+gzip compressed data, was "dist\yplib-0.2.7.tar", last modified: Tue Jun 13 03:21:49 2023, max compression
```

## Comparing `yplib-0.2.6.tar` & `yplib-0.2.7.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 00:30:38.957977 yplib-0.2.6/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-0.2.6/LICENSE
--rw-rw-rw-   0        0        0      567 2023-06-13 00:30:38.957977 yplib-0.2.6/PKG-INFO
--rw-rw-rw-   0        0        0      178 2023-06-08 01:05:32.000000 yplib-0.2.6/README.md
--rw-rw-rw-   0        0        0       42 2023-06-13 00:30:38.957977 yplib-0.2.6/setup.cfg
--rw-rw-rw-   0        0        0      561 2023-06-13 00:30:19.000000 yplib-0.2.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-13 00:30:38.954763 yplib-0.2.6/yplib/
--rw-rw-rw-   0        0        0    15573 2023-06-13 00:29:50.000000 yplib-0.2.6/yplib/__init__.py
--rw-rw-rw-   0        0        0     2609 2023-06-09 02:24:26.000000 yplib-0.2.6/yplib/line_stack_temp.py
-drwxrwxrwx   0        0        0        0 2023-06-13 00:30:38.957343 yplib-0.2.6/yplib.egg-info/
--rw-rw-rw-   0        0        0      567 2023-06-13 00:30:38.000000 yplib-0.2.6/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      185 2023-06-13 00:30:38.000000 yplib-0.2.6/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 00:30:38.000000 yplib-0.2.6/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-13 00:30:38.000000 yplib-0.2.6/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-13 03:21:49.346133 yplib-0.2.7/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-0.2.7/LICENSE
+-rw-rw-rw-   0        0        0      567 2023-06-13 03:21:49.346133 yplib-0.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0      178 2023-06-08 01:05:32.000000 yplib-0.2.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-13 03:21:49.346133 yplib-0.2.7/setup.cfg
+-rw-rw-rw-   0        0        0      561 2023-06-13 03:21:07.000000 yplib-0.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 03:21:49.342583 yplib-0.2.7/yplib/
+-rw-rw-rw-   0        0        0    15573 2023-06-13 00:29:50.000000 yplib-0.2.7/yplib/__init__.py
+-rw-rw-rw-   0        0        0     2989 2023-06-13 03:19:00.000000 yplib-0.2.7/yplib/file.py
+-rw-rw-rw-   0        0        0     2609 2023-06-09 02:24:26.000000 yplib-0.2.7/yplib/line_stack_temp.py
+drwxrwxrwx   0        0        0        0 2023-06-13 03:21:49.345212 yplib-0.2.7/yplib.egg-info/
+-rw-rw-rw-   0        0        0      567 2023-06-13 03:21:49.000000 yplib-0.2.7/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      199 2023-06-13 03:21:49.000000 yplib-0.2.7/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 03:21:49.000000 yplib-0.2.7/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-13 03:21:49.000000 yplib-0.2.7/yplib.egg-info/top_level.txt
```

### Comparing `yplib-0.2.6/LICENSE` & `yplib-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-0.2.6/PKG-INFO` & `yplib-0.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yplib
-Version: 0.2.6
+Version: 0.2.7
 Summary: util
 Home-page: https://github.com/pypa/sampleproject
 Author: yangpu
 Author-email: wantwaterfish@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `yplib-0.2.6/setup.py` & `yplib-0.2.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="0.2.6",
+  version="0.2.7",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/pypa/sampleproject",
   packages=setuptools.find_packages(),
```

### Comparing `yplib-0.2.6/yplib/__init__.py` & `yplib-0.2.7/yplib/__init__.py`

 * *Files identical despite different names*

### Comparing `yplib-0.2.6/yplib/line_stack_temp.py` & `yplib-0.2.7/yplib/line_stack_temp.py`

 * *Files identical despite different names*

### Comparing `yplib-0.2.6/yplib.egg-info/PKG-INFO` & `yplib-0.2.7/yplib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yplib
-Version: 0.2.6
+Version: 0.2.7
 Summary: util
 Home-page: https://github.com/pypa/sampleproject
 Author: yangpu
 Author-email: wantwaterfish@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

