# Comparing `tmp/asgihandler-0.4.7.tar.gz` & `tmp/asgihandler-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asgihandler-0.4.7.tar", last modified: Sat Jun 10 03:18:24 2023, max compression
+gzip compressed data, was "asgihandler-0.4.8.tar", last modified: Tue Jun 13 01:35:47 2023, max compression
```

## Comparing `asgihandler-0.4.7.tar` & `asgihandler-0.4.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-10 03:18:24.092599 asgihandler-0.4.7/
--rw-rw-rw-   0        0        0     1067 2022-07-16 23:50:52.000000 asgihandler-0.4.7/LICENSE
--rw-rw-rw-   0        0        0       27 2022-07-16 23:50:52.000000 asgihandler-0.4.7/MANIFEST.in
--rw-rw-rw-   0        0        0     3117 2023-06-10 03:18:24.092599 asgihandler-0.4.7/PKG-INFO
--rw-rw-rw-   0        0        0     2483 2023-05-02 06:18:39.000000 asgihandler-0.4.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-10 03:18:24.080598 asgihandler-0.4.7/asgihandler/
--rw-rw-rw-   0        0        0       21 2022-07-16 23:50:52.000000 asgihandler-0.4.7/asgihandler/__init__.py
--rw-rw-rw-   0        0        0       68 2022-07-16 23:55:07.000000 asgihandler-0.4.7/asgihandler/__version__.py
--rw-rw-rw-   0        0        0     1260 2023-05-27 01:35:04.000000 asgihandler-0.4.7/asgihandler/core.py
--rw-rw-rw-   0        0        0      460 2023-06-10 03:16:53.000000 asgihandler-0.4.7/asgihandler/userCheck.py
-drwxrwxrwx   0        0        0        0 2023-06-10 03:18:24.091599 asgihandler-0.4.7/asgihandler.egg-info/
--rw-rw-rw-   0        0        0     3117 2023-06-10 03:18:24.000000 asgihandler-0.4.7/asgihandler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      308 2023-06-10 03:18:24.000000 asgihandler-0.4.7/asgihandler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 03:18:24.000000 asgihandler-0.4.7/asgihandler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-10 03:18:24.000000 asgihandler-0.4.7/asgihandler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-10 03:18:24.000000 asgihandler-0.4.7/asgihandler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-10 03:18:24.092599 asgihandler-0.4.7/setup.cfg
--rw-rw-rw-   0        0        0     3878 2023-06-10 03:17:30.000000 asgihandler-0.4.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 01:35:47.805721 asgihandler-0.4.8/
+-rw-rw-rw-   0        0        0     1067 2022-07-16 23:50:52.000000 asgihandler-0.4.8/LICENSE
+-rw-rw-rw-   0        0        0       27 2022-07-16 23:50:52.000000 asgihandler-0.4.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     3117 2023-06-13 01:35:47.805721 asgihandler-0.4.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2483 2023-05-02 06:18:39.000000 asgihandler-0.4.8/README.md
+drwxrwxrwx   0        0        0        0 2023-06-13 01:35:47.790722 asgihandler-0.4.8/asgihandler/
+-rw-rw-rw-   0        0        0       21 2022-07-16 23:50:52.000000 asgihandler-0.4.8/asgihandler/__init__.py
+-rw-rw-rw-   0        0        0       68 2022-07-16 23:55:07.000000 asgihandler-0.4.8/asgihandler/__version__.py
+-rw-rw-rw-   0        0        0     1260 2023-05-27 01:35:04.000000 asgihandler-0.4.8/asgihandler/core.py
+-rw-rw-rw-   0        0        0      460 2023-06-13 01:35:03.000000 asgihandler-0.4.8/asgihandler/userCheck.py
+drwxrwxrwx   0        0        0        0 2023-06-13 01:35:47.803722 asgihandler-0.4.8/asgihandler.egg-info/
+-rw-rw-rw-   0        0        0     3117 2023-06-13 01:35:47.000000 asgihandler-0.4.8/asgihandler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      308 2023-06-13 01:35:47.000000 asgihandler-0.4.8/asgihandler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 01:35:47.000000 asgihandler-0.4.8/asgihandler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-13 01:35:47.000000 asgihandler-0.4.8/asgihandler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-13 01:35:47.000000 asgihandler-0.4.8/asgihandler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-13 01:35:47.805721 asgihandler-0.4.8/setup.cfg
+-rw-rw-rw-   0        0        0     3878 2023-06-13 01:35:42.000000 asgihandler-0.4.8/setup.py
```

### Comparing `asgihandler-0.4.7/LICENSE` & `asgihandler-0.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `asgihandler-0.4.7/PKG-INFO` & `asgihandler-0.4.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asgihandler
-Version: 0.4.7
+Version: 0.4.8
 Summary: ASGIHandler
 Home-page: https://github.com/GreaterWMS/GreaterWMS
 Author: Singosgu
 Author-email: singosgu@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `asgihandler-0.4.7/README.md` & `asgihandler-0.4.8/README.md`

 * *Files identical despite different names*

### Comparing `asgihandler-0.4.7/asgihandler/core.py` & `asgihandler-0.4.8/asgihandler/core.py`

 * *Files identical despite different names*

### Comparing `asgihandler-0.4.7/asgihandler.egg-info/PKG-INFO` & `asgihandler-0.4.8/asgihandler.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asgihandler
-Version: 0.4.7
+Version: 0.4.8
 Summary: ASGIHandler
 Home-page: https://github.com/GreaterWMS/GreaterWMS
 Author: Singosgu
 Author-email: singosgu@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `asgihandler-0.4.7/setup.py` & `asgihandler-0.4.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'asgihandler'
 DESCRIPTION = 'ASGIHandler'
 URL = 'https://github.com/GreaterWMS/GreaterWMS'
 EMAIL = 'singosgu@gmail.com'
 AUTHOR = 'Singosgu'
 REQUIRES_PYTHON = '>=3.7.0'
-VERSION = '0.4.7'
+VERSION = '0.4.8'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'requests',
 ]
 
 # What packages are optional?
```

