# Comparing `tmp/yplib-1.0.0.tar.gz` & `tmp/yplib-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-1.0.0.tar", last modified: Tue Jun 13 06:21:58 2023, max compression
+gzip compressed data, was "dist\yplib-1.0.1.tar", last modified: Tue Jun 13 06:24:21 2023, max compression
```

## Comparing `yplib-1.0.0.tar` & `yplib-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 06:21:58.062173 yplib-1.0.0/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      567 2023-06-13 06:21:58.061967 yplib-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      178 2023-06-08 01:05:32.000000 yplib-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2023-06-13 06:21:58.062797 yplib-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      561 2023-06-13 06:21:48.000000 yplib-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-13 06:21:58.058838 yplib-1.0.0/yplib/
--rw-rw-rw-   0        0        0    15573 2023-06-13 06:20:59.000000 yplib-1.0.0/yplib/__init__.py
--rw-rw-rw-   0        0        0     3013 2023-06-13 06:19:43.000000 yplib-1.0.0/yplib/file.py
--rw-rw-rw-   0        0        0    15573 2023-06-13 00:29:50.000000 yplib-1.0.0/yplib/index.py
--rw-rw-rw-   0        0        0     2609 2023-06-09 02:24:26.000000 yplib-1.0.0/yplib/line_stack_temp.py
-drwxrwxrwx   0        0        0        0 2023-06-13 06:21:58.061214 yplib-1.0.0/yplib.egg-info/
--rw-rw-rw-   0        0        0      567 2023-06-13 06:21:58.000000 yplib-1.0.0/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      214 2023-06-13 06:21:58.000000 yplib-1.0.0/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 06:21:58.000000 yplib-1.0.0/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-13 06:21:58.000000 yplib-1.0.0/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-13 06:24:21.107265 yplib-1.0.1/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      567 2023-06-13 06:24:21.106688 yplib-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      178 2023-06-08 01:05:32.000000 yplib-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-13 06:24:21.107265 yplib-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      561 2023-06-13 06:24:13.000000 yplib-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 06:24:21.103494 yplib-1.0.1/yplib/
+-rw-rw-rw-   0        0        0       87 2023-06-13 06:23:51.000000 yplib-1.0.1/yplib/__init__.py
+-rw-rw-rw-   0        0        0     3019 2023-06-13 06:22:53.000000 yplib-1.0.1/yplib/file.py
+-rw-rw-rw-   0        0        0    15553 2023-06-13 06:23:26.000000 yplib-1.0.1/yplib/index.py
+-rw-rw-rw-   0        0        0     2609 2023-06-09 02:24:26.000000 yplib-1.0.1/yplib/line_stack_temp.py
+drwxrwxrwx   0        0        0        0 2023-06-13 06:24:21.105854 yplib-1.0.1/yplib.egg-info/
+-rw-rw-rw-   0        0        0      567 2023-06-13 06:24:21.000000 yplib-1.0.1/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      214 2023-06-13 06:24:21.000000 yplib-1.0.1/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 06:24:21.000000 yplib-1.0.1/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-13 06:24:21.000000 yplib-1.0.1/yplib.egg-info/top_level.txt
```

### Comparing `yplib-1.0.0/LICENSE` & `yplib-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-1.0.0/PKG-INFO` & `yplib-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yplib
-Version: 1.0.0
+Version: 1.0.1
 Summary: util
 Home-page: https://github.com/pypa/sampleproject
 Author: yangpu
 Author-email: wantwaterfish@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `yplib-1.0.0/setup.py` & `yplib-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="1.0.0",
+  version="1.0.1",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/pypa/sampleproject",
   packages=setuptools.find_packages(),
```

### Comparing `yplib-1.0.0/yplib/__init__.py` & `yplib-1.0.1/yplib/index.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# name = "yplib"
-
 import json
 import os
 import uuid
 from datetime import datetime
 from datetime import timedelta
 
 import xlrd
```

### Comparing `yplib-1.0.0/yplib/file.py` & `yplib-1.0.1/yplib/file.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from yplib import *
+from yplib.index import *
 
 
 # 有关文件的操作
 # 查询指定文件夹下面的所有的文件信息, 也可以是指定的文件
 # param list
 # return list
 def get_file(file_path=None, prefix=None, contain=None, suffix=None):
```

### Comparing `yplib-1.0.0/yplib/line_stack_temp.py` & `yplib-1.0.1/yplib/line_stack_temp.py`

 * *Files identical despite different names*

### Comparing `yplib-1.0.0/yplib.egg-info/PKG-INFO` & `yplib-1.0.1/yplib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yplib
-Version: 1.0.0
+Version: 1.0.1
 Summary: util
 Home-page: https://github.com/pypa/sampleproject
 Author: yangpu
 Author-email: wantwaterfish@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

