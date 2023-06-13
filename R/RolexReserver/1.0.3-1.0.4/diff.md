# Comparing `tmp/RolexReserver-1.0.3.tar.gz` & `tmp/RolexReserver-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RolexReserver-1.0.3.tar", last modified: Tue May 23 13:03:31 2023, max compression
+gzip compressed data, was "RolexReserver-1.0.4.tar", last modified: Tue Jun 13 13:01:54 2023, max compression
```

## Comparing `RolexReserver-1.0.3.tar` & `RolexReserver-1.0.4.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 13:03:31.751072 RolexReserver-1.0.3/
--rw-rw-rw-   0        0        0      887 2023-05-23 13:03:31.750072 RolexReserver-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       17 2023-05-09 13:04:12.000000 RolexReserver-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-23 13:03:31.734072 RolexReserver-1.0.3/RolexReserver/
-drwxrwxrwx   0        0        0        0 2023-05-23 13:03:31.740070 RolexReserver-1.0.3/RolexReserver/Getter/
-drwxrwxrwx   0        0        0        0 2023-05-23 13:03:31.741071 RolexReserver-1.0.3/RolexReserver/Getter/Base/
--rw-rw-rw-   0        0        0     1417 2023-05-09 13:09:11.000000 RolexReserver-1.0.3/RolexReserver/Getter/Base/baseGetter.py
--rw-rw-rw-   0        0        0     5828 2023-05-22 10:11:15.000000 RolexReserver-1.0.3/RolexReserver/Getter/getter_rolexReserve.py
-drwxrwxrwx   0        0        0        0 2023-05-23 13:03:31.749074 RolexReserver-1.0.3/RolexReserver/Library/
--rw-rw-rw-   0        0        0     4820 2023-05-20 08:30:17.000000 RolexReserver-1.0.3/RolexReserver/Library/rolexReserverConfig.py
--rw-rw-rw-   0        0        0      704 2023-05-13 05:47:49.000000 RolexReserver-1.0.3/RolexReserver/Library/rolexReserverConfiger.py
--rw-rw-rw-   0        0        0     1538 2023-05-10 13:23:34.000000 RolexReserver-1.0.3/RolexReserver/Library/rolexReserverController.py
--rw-rw-rw-   0        0        0      164 2023-05-09 12:52:25.000000 RolexReserver-1.0.3/RolexReserver/Library/rolexReserverDeclare.py
--rw-rw-rw-   0        0        0     2092 2023-01-06 13:54:01.000000 RolexReserver-1.0.3/RolexReserver/Library/rolexReserverException.py
--rw-rw-rw-   0        0        0      573 2023-05-09 13:01:02.000000 RolexReserver-1.0.3/RolexReserver/Library/rolexReserverGlobals.py
--rw-rw-rw-   0        0        0     4731 2023-05-09 13:01:02.000000 RolexReserver-1.0.3/RolexReserver/Library/rolexReserverMailer.py
--rw-rw-rw-   0        0        0      261 2023-05-22 10:12:16.000000 RolexReserver-1.0.3/RolexReserver/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-23 13:03:31.739072 RolexReserver-1.0.3/RolexReserver.egg-info/
--rw-rw-rw-   0        0        0      887 2023-05-23 13:03:31.000000 RolexReserver-1.0.3/RolexReserver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      638 2023-05-23 13:03:31.000000 RolexReserver-1.0.3/RolexReserver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 13:03:31.000000 RolexReserver-1.0.3/RolexReserver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      784 2023-05-23 13:03:31.000000 RolexReserver-1.0.3/RolexReserver.egg-info/requires.txt
--rw-rw-rw-   0        0        0      105 2023-05-23 13:03:31.000000 RolexReserver-1.0.3/RolexReserver.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-23 13:03:31.751072 RolexReserver-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     2523 2023-05-09 12:42:27.000000 RolexReserver-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 13:01:54.325291 RolexReserver-1.0.4/
+-rw-rw-rw-   0        0        0      887 2023-06-13 13:01:54.325291 RolexReserver-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       17 2023-05-09 13:04:12.000000 RolexReserver-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-13 13:01:54.300284 RolexReserver-1.0.4/RolexReserver/
+drwxrwxrwx   0        0        0        0 2023-06-13 13:01:54.308289 RolexReserver-1.0.4/RolexReserver/Getter/
+drwxrwxrwx   0        0        0        0 2023-06-13 13:01:54.310288 RolexReserver-1.0.4/RolexReserver/Getter/Base/
+-rw-rw-rw-   0        0        0     1417 2023-05-09 13:09:11.000000 RolexReserver-1.0.4/RolexReserver/Getter/Base/baseGetter.py
+-rw-rw-rw-   0        0        0     7479 2023-06-13 13:00:37.000000 RolexReserver-1.0.4/RolexReserver/Getter/getter_rolexReserve.py
+drwxrwxrwx   0        0        0        0 2023-06-13 13:01:54.322292 RolexReserver-1.0.4/RolexReserver/Library/
+-rw-rw-rw-   0        0        0     4820 2023-05-23 13:18:26.000000 RolexReserver-1.0.4/RolexReserver/Library/rolexReserverConfig.py
+-rw-rw-rw-   0        0        0      704 2023-05-13 05:47:49.000000 RolexReserver-1.0.4/RolexReserver/Library/rolexReserverConfiger.py
+-rw-rw-rw-   0        0        0     1538 2023-05-10 13:23:34.000000 RolexReserver-1.0.4/RolexReserver/Library/rolexReserverController.py
+-rw-rw-rw-   0        0        0      164 2023-05-09 12:52:25.000000 RolexReserver-1.0.4/RolexReserver/Library/rolexReserverDeclare.py
+-rw-rw-rw-   0        0        0     2092 2023-01-06 13:54:01.000000 RolexReserver-1.0.4/RolexReserver/Library/rolexReserverException.py
+-rw-rw-rw-   0        0        0      573 2023-05-09 13:01:02.000000 RolexReserver-1.0.4/RolexReserver/Library/rolexReserverGlobals.py
+-rw-rw-rw-   0        0        0     4731 2023-05-09 13:01:02.000000 RolexReserver-1.0.4/RolexReserver/Library/rolexReserverMailer.py
+drwxrwxrwx   0        0        0        0 2023-06-13 13:01:54.323300 RolexReserver-1.0.4/RolexReserver/Models/
+-rw-rw-rw-   0        0        0      669 2023-06-13 12:51:31.000000 RolexReserver-1.0.4/RolexReserver/Models/log_reserve.py
+-rw-rw-rw-   0        0        0      261 2023-06-13 13:01:42.000000 RolexReserver-1.0.4/RolexReserver/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 13:01:54.306285 RolexReserver-1.0.4/RolexReserver.egg-info/
+-rw-rw-rw-   0        0        0      887 2023-06-13 13:01:54.000000 RolexReserver-1.0.4/RolexReserver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      674 2023-06-13 13:01:54.000000 RolexReserver-1.0.4/RolexReserver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 13:01:54.000000 RolexReserver-1.0.4/RolexReserver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      784 2023-06-13 13:01:54.000000 RolexReserver-1.0.4/RolexReserver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      105 2023-06-13 13:01:54.000000 RolexReserver-1.0.4/RolexReserver.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-13 13:01:54.326295 RolexReserver-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     2523 2023-05-09 12:42:27.000000 RolexReserver-1.0.4/setup.py
```

### Comparing `RolexReserver-1.0.3/PKG-INFO` & `RolexReserver-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RolexReserver
-Version: 1.0.3
+Version: 1.0.4
 Summary: RolexReserver Package
 Home-page: https://github.com/kaioman/RolexReserver.git
 Author: unchainworks
 Author-email: kajin0318@gmail.com
 License: BSD-3-Clause
 Keywords: RolexReserver
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `RolexReserver-1.0.3/RolexReserver/Getter/Base/baseGetter.py` & `RolexReserver-1.0.4/RolexReserver/Getter/Base/baseGetter.py`

 * *Files identical despite different names*

### Comparing `RolexReserver-1.0.3/RolexReserver/Library/rolexReserverConfig.py` & `RolexReserver-1.0.4/RolexReserver/Library/rolexReserverConfig.py`

 * *Files identical despite different names*

### Comparing `RolexReserver-1.0.3/RolexReserver/Library/rolexReserverConfiger.py` & `RolexReserver-1.0.4/RolexReserver/Library/rolexReserverConfiger.py`

 * *Files identical despite different names*

### Comparing `RolexReserver-1.0.3/RolexReserver/Library/rolexReserverController.py` & `RolexReserver-1.0.4/RolexReserver/Library/rolexReserverController.py`

 * *Files identical despite different names*

### Comparing `RolexReserver-1.0.3/RolexReserver/Library/rolexReserverException.py` & `RolexReserver-1.0.4/RolexReserver/Library/rolexReserverException.py`

 * *Files identical despite different names*

### Comparing `RolexReserver-1.0.3/RolexReserver/Library/rolexReserverGlobals.py` & `RolexReserver-1.0.4/RolexReserver/Library/rolexReserverGlobals.py`

 * *Files identical despite different names*

### Comparing `RolexReserver-1.0.3/RolexReserver/Library/rolexReserverMailer.py` & `RolexReserver-1.0.4/RolexReserver/Library/rolexReserverMailer.py`

 * *Files identical despite different names*

### Comparing `RolexReserver-1.0.3/RolexReserver.egg-info/PKG-INFO` & `RolexReserver-1.0.4/RolexReserver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RolexReserver
-Version: 1.0.3
+Version: 1.0.4
 Summary: RolexReserver Package
 Home-page: https://github.com/kaioman/RolexReserver.git
 Author: unchainworks
 Author-email: kajin0318@gmail.com
 License: BSD-3-Clause
 Keywords: RolexReserver
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `RolexReserver-1.0.3/RolexReserver.egg-info/SOURCES.txt` & `RolexReserver-1.0.4/RolexReserver.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -10,8 +10,9 @@
 RolexReserver/Getter/Base/baseGetter.py
 RolexReserver/Library/rolexReserverConfig.py
 RolexReserver/Library/rolexReserverConfiger.py
 RolexReserver/Library/rolexReserverController.py
 RolexReserver/Library/rolexReserverDeclare.py
 RolexReserver/Library/rolexReserverException.py
 RolexReserver/Library/rolexReserverGlobals.py
-RolexReserver/Library/rolexReserverMailer.py
+RolexReserver/Library/rolexReserverMailer.py
+RolexReserver/Models/log_reserve.py
```

### Comparing `RolexReserver-1.0.3/RolexReserver.egg-info/requires.txt` & `RolexReserver-1.0.4/RolexReserver.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `RolexReserver-1.0.3/setup.py` & `RolexReserver-1.0.4/setup.py`

 * *Files identical despite different names*

