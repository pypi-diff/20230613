# Comparing `tmp/yplib-1.0.1.tar.gz` & `tmp/yplib-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-1.0.1.tar", last modified: Tue Jun 13 06:24:21 2023, max compression
+gzip compressed data, was "dist\yplib-1.0.2.tar", last modified: Tue Jun 13 06:29:24 2023, max compression
```

## Comparing `yplib-1.0.1.tar` & `yplib-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 06:24:21.107265 yplib-1.0.1/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.0.1/LICENSE
--rw-rw-rw-   0        0        0      567 2023-06-13 06:24:21.106688 yplib-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      178 2023-06-08 01:05:32.000000 yplib-1.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-13 06:24:21.107265 yplib-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      561 2023-06-13 06:24:13.000000 yplib-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-13 06:24:21.103494 yplib-1.0.1/yplib/
--rw-rw-rw-   0        0        0       87 2023-06-13 06:23:51.000000 yplib-1.0.1/yplib/__init__.py
--rw-rw-rw-   0        0        0     3019 2023-06-13 06:22:53.000000 yplib-1.0.1/yplib/file.py
--rw-rw-rw-   0        0        0    15553 2023-06-13 06:23:26.000000 yplib-1.0.1/yplib/index.py
--rw-rw-rw-   0        0        0     2609 2023-06-09 02:24:26.000000 yplib-1.0.1/yplib/line_stack_temp.py
-drwxrwxrwx   0        0        0        0 2023-06-13 06:24:21.105854 yplib-1.0.1/yplib.egg-info/
--rw-rw-rw-   0        0        0      567 2023-06-13 06:24:21.000000 yplib-1.0.1/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      214 2023-06-13 06:24:21.000000 yplib-1.0.1/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 06:24:21.000000 yplib-1.0.1/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-13 06:24:21.000000 yplib-1.0.1/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-13 06:29:24.599662 yplib-1.0.2/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0      567 2023-06-13 06:29:24.599160 yplib-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      178 2023-06-08 01:05:32.000000 yplib-1.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-13 06:29:24.599662 yplib-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      561 2023-06-13 06:29:11.000000 yplib-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 06:29:24.595985 yplib-1.0.2/yplib/
+-rw-rw-rw-   0        0        0       87 2023-06-13 06:23:51.000000 yplib-1.0.2/yplib/__init__.py
+-rw-rw-rw-   0        0        0     3021 2023-06-13 06:29:04.000000 yplib-1.0.2/yplib/file.py
+-rw-rw-rw-   0        0        0    15553 2023-06-13 06:23:26.000000 yplib-1.0.2/yplib/index.py
+-rw-rw-rw-   0        0        0     2609 2023-06-09 02:24:26.000000 yplib-1.0.2/yplib/line_stack_temp.py
+drwxrwxrwx   0        0        0        0 2023-06-13 06:29:24.598255 yplib-1.0.2/yplib.egg-info/
+-rw-rw-rw-   0        0        0      567 2023-06-13 06:29:24.000000 yplib-1.0.2/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      214 2023-06-13 06:29:24.000000 yplib-1.0.2/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 06:29:24.000000 yplib-1.0.2/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-13 06:29:24.000000 yplib-1.0.2/yplib.egg-info/top_level.txt
```

### Comparing `yplib-1.0.1/LICENSE` & `yplib-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-1.0.1/PKG-INFO` & `yplib-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yplib
-Version: 1.0.1
+Version: 1.0.2
 Summary: util
 Home-page: https://github.com/pypa/sampleproject
 Author: yangpu
 Author-email: wantwaterfish@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `yplib-1.0.1/setup.py` & `yplib-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="1.0.1",
+  version="1.0.2",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/pypa/sampleproject",
   packages=setuptools.find_packages(),
```

### Comparing `yplib-1.0.1/yplib/file.py` & `yplib-1.0.2/yplib/file.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,9 +78,9 @@
             to_log(one_file, e)
             continue
 
 
 # get_file_by_content(r'D:\notepad_file\202306', 'a')
 # print(get_file(r'D:\notepad_file\202306', 'a'))
 # print(get_file(r'D:\notepad_file\202306'))
-print(get_file())
+# print(get_file())
 # print(os.path.abspath('.'))
```

### Comparing `yplib-1.0.1/yplib/index.py` & `yplib-1.0.2/yplib/index.py`

 * *Files identical despite different names*

### Comparing `yplib-1.0.1/yplib/line_stack_temp.py` & `yplib-1.0.2/yplib/line_stack_temp.py`

 * *Files identical despite different names*

### Comparing `yplib-1.0.1/yplib.egg-info/PKG-INFO` & `yplib-1.0.2/yplib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yplib
-Version: 1.0.1
+Version: 1.0.2
 Summary: util
 Home-page: https://github.com/pypa/sampleproject
 Author: yangpu
 Author-email: wantwaterfish@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

