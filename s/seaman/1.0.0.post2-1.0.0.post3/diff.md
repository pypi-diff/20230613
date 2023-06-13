# Comparing `tmp/seaman-1.0.0.post2.tar.gz` & `tmp/seaman-1.0.0.post3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seaman-1.0.0.post2.tar", last modified: Tue Jun 13 02:02:28 2023, max compression
+gzip compressed data, was "seaman-1.0.0.post3.tar", last modified: Tue Jun 13 02:05:36 2023, max compression
```

## Comparing `seaman-1.0.0.post2.tar` & `seaman-1.0.0.post3.tar`

### file list

```diff
@@ -1,37 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 02:02:28.957959 seaman-1.0.0.post2/
--rw-rw-rw-   0        0        0     1085 2023-06-13 01:10:29.000000 seaman-1.0.0.post2/LICENSE
--rw-rw-rw-   0        0        0      695 2023-06-13 02:02:28.956962 seaman-1.0.0.post2/PKG-INFO
--rw-rw-rw-   0        0        0       49 2023-06-12 06:38:34.000000 seaman-1.0.0.post2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-13 02:02:28.909088 seaman-1.0.0.post2/seaman/
--rw-rw-rw-   0        0        0      116 2023-06-13 02:01:51.000000 seaman-1.0.0.post2/seaman/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 02:02:28.916070 seaman-1.0.0.post2/seaman/cache/
--rw-rw-rw-   0        0        0     1019 2023-03-10 01:59:28.000000 seaman-1.0.0.post2/seaman/cache/CacheUtil.py
--rw-rw-rw-   0        0        0        0 2023-06-12 06:36:59.000000 seaman-1.0.0.post2/seaman/cache/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 02:02:28.950976 seaman-1.0.0.post2/seaman/core/
--rw-rw-rw-   0        0        0     1445 2023-02-24 02:21:22.000000 seaman-1.0.0.post2/seaman/core/DateUtil.py
--rw-rw-rw-   0        0        0      954 2023-06-13 01:35:50.000000 seaman-1.0.0.post2/seaman/core/FileUtil.py
--rw-rw-rw-   0        0        0      843 2023-02-27 01:00:25.000000 seaman-1.0.0.post2/seaman/core/HashUtil.py
--rw-rw-rw-   0        0        0     1306 2023-02-27 00:48:29.000000 seaman-1.0.0.post2/seaman/core/HexUtil.py
--rw-rw-rw-   0        0        0     1238 2023-06-13 01:35:50.000000 seaman-1.0.0.post2/seaman/core/IdUtil.py
--rw-rw-rw-   0        0        0      998 2023-03-13 02:42:47.000000 seaman-1.0.0.post2/seaman/core/JsonUtil.py
--rw-rw-rw-   0        0        0     3730 2023-03-10 08:30:31.000000 seaman-1.0.0.post2/seaman/core/OsUtil.py
--rw-rw-rw-   0        0        0     2038 2023-04-09 07:04:28.000000 seaman-1.0.0.post2/seaman/core/StrUtil.py
--rw-rw-rw-   0        0        0      446 2023-02-27 02:11:44.000000 seaman-1.0.0.post2/seaman/core/UrlUtil.py
--rw-rw-rw-   0        0        0     2164 2023-03-10 08:10:29.000000 seaman-1.0.0.post2/seaman/core/Validator.py
--rw-rw-rw-   0        0        0        0 2023-06-12 06:36:49.000000 seaman-1.0.0.post2/seaman/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 02:02:28.952972 seaman-1.0.0.post2/seaman/extra/
--rw-rw-rw-   0        0        0     1478 2023-03-12 01:51:43.000000 seaman-1.0.0.post2/seaman/extra/ExcelUtil.py
--rw-rw-rw-   0        0        0        0 2023-06-12 06:54:35.000000 seaman-1.0.0.post2/seaman/extra/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 02:02:28.954967 seaman-1.0.0.post2/seaman/http/
--rw-rw-rw-   0        0        0     2713 2023-06-13 01:35:50.000000 seaman-1.0.0.post2/seaman/http/HttpUtil.py
--rw-rw-rw-   0        0        0        0 2023-06-12 06:56:05.000000 seaman-1.0.0.post2/seaman/http/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 02:02:28.914075 seaman-1.0.0.post2/seaman.egg-info/
--rw-rw-rw-   0        0        0      695 2023-06-13 02:02:28.000000 seaman-1.0.0.post2/seaman.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      619 2023-06-13 02:02:28.000000 seaman-1.0.0.post2/seaman.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 02:02:28.000000 seaman-1.0.0.post2/seaman.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-06-13 02:02:28.000000 seaman-1.0.0.post2/seaman.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-13 02:02:28.000000 seaman-1.0.0.post2/seaman.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-13 02:02:28.957959 seaman-1.0.0.post2/setup.cfg
--rw-rw-rw-   0        0        0     3922 2023-06-13 02:01:37.000000 seaman-1.0.0.post2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-13 02:02:28.955964 seaman-1.0.0.post2/test/
--rw-rw-rw-   0        0        0       58 2023-06-13 01:40:42.000000 seaman-1.0.0.post2/test/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 02:05:36.363648 seaman-1.0.0.post3/
+-rw-rw-rw-   0        0        0     1085 2023-06-13 01:10:29.000000 seaman-1.0.0.post3/LICENSE
+-rw-rw-rw-   0        0        0      695 2023-06-13 02:05:36.363148 seaman-1.0.0.post3/PKG-INFO
+-rw-rw-rw-   0        0        0       49 2023-06-12 06:38:34.000000 seaman-1.0.0.post3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-13 02:05:36.316489 seaman-1.0.0.post3/seaman/
+-rw-rw-rw-   0        0        0      116 2023-06-13 02:01:51.000000 seaman-1.0.0.post3/seaman/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 02:05:36.322475 seaman-1.0.0.post3/seaman/cache/
+-rw-rw-rw-   0        0        0     1019 2023-03-10 01:59:28.000000 seaman-1.0.0.post3/seaman/cache/CacheUtil.py
+-rw-rw-rw-   0        0        0        0 2023-06-12 06:36:59.000000 seaman-1.0.0.post3/seaman/cache/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 02:05:36.357010 seaman-1.0.0.post3/seaman/core/
+-rw-rw-rw-   0        0        0     1445 2023-02-24 02:21:22.000000 seaman-1.0.0.post3/seaman/core/DateUtil.py
+-rw-rw-rw-   0        0        0      954 2023-06-13 01:35:50.000000 seaman-1.0.0.post3/seaman/core/FileUtil.py
+-rw-rw-rw-   0        0        0      843 2023-02-27 01:00:25.000000 seaman-1.0.0.post3/seaman/core/HashUtil.py
+-rw-rw-rw-   0        0        0     1306 2023-02-27 00:48:29.000000 seaman-1.0.0.post3/seaman/core/HexUtil.py
+-rw-rw-rw-   0        0        0     1238 2023-06-13 01:35:50.000000 seaman-1.0.0.post3/seaman/core/IdUtil.py
+-rw-rw-rw-   0        0        0      998 2023-03-13 02:42:47.000000 seaman-1.0.0.post3/seaman/core/JsonUtil.py
+-rw-rw-rw-   0        0        0     3730 2023-03-10 08:30:31.000000 seaman-1.0.0.post3/seaman/core/OsUtil.py
+-rw-rw-rw-   0        0        0     2038 2023-04-09 07:04:28.000000 seaman-1.0.0.post3/seaman/core/StrUtil.py
+-rw-rw-rw-   0        0        0      446 2023-02-27 02:11:44.000000 seaman-1.0.0.post3/seaman/core/UrlUtil.py
+-rw-rw-rw-   0        0        0     2164 2023-03-10 08:10:29.000000 seaman-1.0.0.post3/seaman/core/Validator.py
+-rw-rw-rw-   0        0        0        0 2023-06-12 06:36:49.000000 seaman-1.0.0.post3/seaman/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 02:05:36.358967 seaman-1.0.0.post3/seaman/extra/
+-rw-rw-rw-   0        0        0     1478 2023-03-12 01:51:43.000000 seaman-1.0.0.post3/seaman/extra/ExcelUtil.py
+-rw-rw-rw-   0        0        0        0 2023-06-12 06:54:35.000000 seaman-1.0.0.post3/seaman/extra/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 02:05:36.360974 seaman-1.0.0.post3/seaman/http/
+-rw-rw-rw-   0        0        0     2713 2023-06-13 01:35:50.000000 seaman-1.0.0.post3/seaman/http/HttpUtil.py
+-rw-rw-rw-   0        0        0        0 2023-06-12 06:56:05.000000 seaman-1.0.0.post3/seaman/http/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 02:05:36.320509 seaman-1.0.0.post3/seaman.egg-info/
+-rw-rw-rw-   0        0        0      695 2023-06-13 02:05:36.000000 seaman-1.0.0.post3/seaman.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      590 2023-06-13 02:05:36.000000 seaman-1.0.0.post3/seaman.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 02:05:36.000000 seaman-1.0.0.post3/seaman.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-06-13 02:05:36.000000 seaman-1.0.0.post3/seaman.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-13 02:05:36.363648 seaman-1.0.0.post3/setup.cfg
+-rw-rw-rw-   0        0        0     3868 2023-06-13 02:05:23.000000 seaman-1.0.0.post3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 02:05:36.361976 seaman-1.0.0.post3/test/
+-rw-rw-rw-   0        0        0       58 2023-06-13 01:40:42.000000 seaman-1.0.0.post3/test/__init__.py
```

### Comparing `seaman-1.0.0.post2/LICENSE` & `seaman-1.0.0.post3/LICENSE`

 * *Files identical despite different names*

### Comparing `seaman-1.0.0.post2/PKG-INFO` & `seaman-1.0.0.post3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seaman
-Version: 1.0.0.post2
+Version: 1.0.0.post3
 Summary: a python tool like java hutool
 Home-page: https://gitee.com/Kindear/seaman
 Author: kindear
 Author-email: kindear@foxmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `seaman-1.0.0.post2/seaman/cache/CacheUtil.py` & `seaman-1.0.0.post3/seaman/cache/CacheUtil.py`

 * *Files identical despite different names*

### Comparing `seaman-1.0.0.post2/seaman/core/DateUtil.py` & `seaman-1.0.0.post3/seaman/core/DateUtil.py`

 * *Files identical despite different names*

### Comparing `seaman-1.0.0.post2/seaman/core/FileUtil.py` & `seaman-1.0.0.post3/seaman/core/FileUtil.py`

 * *Files identical despite different names*

### Comparing `seaman-1.0.0.post2/seaman/core/HashUtil.py` & `seaman-1.0.0.post3/seaman/core/HashUtil.py`

 * *Files identical despite different names*

### Comparing `seaman-1.0.0.post2/seaman/core/HexUtil.py` & `seaman-1.0.0.post3/seaman/core/HexUtil.py`

 * *Files identical despite different names*

### Comparing `seaman-1.0.0.post2/seaman/core/IdUtil.py` & `seaman-1.0.0.post3/seaman/core/IdUtil.py`

 * *Files identical despite different names*

### Comparing `seaman-1.0.0.post2/seaman/core/JsonUtil.py` & `seaman-1.0.0.post3/seaman/core/JsonUtil.py`

 * *Files identical despite different names*

### Comparing `seaman-1.0.0.post2/seaman/core/OsUtil.py` & `seaman-1.0.0.post3/seaman/core/OsUtil.py`

 * *Files identical despite different names*

### Comparing `seaman-1.0.0.post2/seaman/core/StrUtil.py` & `seaman-1.0.0.post3/seaman/core/StrUtil.py`

 * *Files identical despite different names*

### Comparing `seaman-1.0.0.post2/seaman/core/Validator.py` & `seaman-1.0.0.post3/seaman/core/Validator.py`

 * *Files identical despite different names*

### Comparing `seaman-1.0.0.post2/seaman/extra/ExcelUtil.py` & `seaman-1.0.0.post3/seaman/extra/ExcelUtil.py`

 * *Files identical despite different names*

### Comparing `seaman-1.0.0.post2/seaman/http/HttpUtil.py` & `seaman-1.0.0.post3/seaman/http/HttpUtil.py`

 * *Files identical despite different names*

### Comparing `seaman-1.0.0.post2/seaman.egg-info/PKG-INFO` & `seaman-1.0.0.post3/seaman.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seaman
-Version: 1.0.0.post2
+Version: 1.0.0.post3
 Summary: a python tool like java hutool
 Home-page: https://gitee.com/Kindear/seaman
 Author: kindear
 Author-email: kindear@foxmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `seaman-1.0.0.post2/seaman.egg-info/SOURCES.txt` & `seaman-1.0.0.post3/seaman.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 LICENSE
 README.md
 setup.py
 seaman/__init__.py
 seaman.egg-info/PKG-INFO
 seaman.egg-info/SOURCES.txt
 seaman.egg-info/dependency_links.txt
-seaman.egg-info/requires.txt
 seaman.egg-info/top_level.txt
 seaman/cache/CacheUtil.py
 seaman/cache/__init__.py
 seaman/core/DateUtil.py
 seaman/core/FileUtil.py
 seaman/core/HashUtil.py
 seaman/core/HexUtil.py
```

### Comparing `seaman-1.0.0.post2/setup.py` & `seaman-1.0.0.post3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,19 +14,19 @@
 # Package meta-data.
 NAME = 'seaman'
 DESCRIPTION = 'a python tool like java hutool'
 URL = 'https://gitee.com/Kindear/seaman'
 EMAIL = 'kindear@foxmail.com'
 AUTHOR = 'kindear'
 REQUIRES_PYTHON = '>=3.7.0'
-VERSION = '1.0.0-r2'
+VERSION = '1.0.0-r3'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
-    'requests', 'cachetools', 'pandas', 'uuid', 'json'
+
 ]
 
 # What packages are optional?
 EXTRAS = {
     # 'fancy feature': ['django'],
 }
```

