# Comparing `tmp/wcs.adminauth-1.0.0.tar.gz` & `tmp/wcs.adminauth-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wcs.adminauth-1.0.0.tar", last modified: Mon Jun 12 19:05:15 2023, max compression
+gzip compressed data, was "wcs.adminauth-1.0.1.tar", last modified: Tue Jun 13 00:58:46 2023, max compression
```

## Comparing `wcs.adminauth-1.0.0.tar` & `wcs.adminauth-1.0.1.tar`

### file list

```diff
@@ -1,29 +1,34 @@
-drwxr-xr-x   0 maethu     (501) staff       (20)        0 2023-06-12 19:05:15.308519 wcs.adminauth-1.0.0/
--rw-r--r--   0 maethu     (501) staff       (20)       98 2023-06-12 19:05:14.000000 wcs.adminauth-1.0.0/MANIFEST.in
--rw-r--r--   0 maethu     (501) staff       (20)     2874 2023-06-12 19:05:15.308407 wcs.adminauth-1.0.0/PKG-INFO
--rw-r--r--   0 maethu     (501) staff       (20)     2064 2023-06-12 19:05:14.000000 wcs.adminauth-1.0.0/README.rst
-drwxr-xr-x   0 maethu     (501) staff       (20)        0 2023-06-12 19:05:15.306496 wcs.adminauth-1.0.0/docs/
--rw-r--r--   0 maethu     (501) staff       (20)      130 2023-06-12 19:05:14.000000 wcs.adminauth-1.0.0/docs/HISTORY.txt
--rw-r--r--   0 maethu     (501) staff       (20)       38 2023-06-12 19:05:15.308555 wcs.adminauth-1.0.0/setup.cfg
--rw-r--r--   0 maethu     (501) staff       (20)     1513 2023-06-12 19:05:14.000000 wcs.adminauth-1.0.0/setup.py
-drwxr-xr-x   0 maethu     (501) staff       (20)        0 2023-06-12 19:05:15.306607 wcs.adminauth-1.0.0/wcs/
--rw-r--r--   0 maethu     (501) staff       (20)      244 2023-06-12 19:05:14.000000 wcs.adminauth-1.0.0/wcs/__init__.py
-drwxr-xr-x   0 maethu     (501) staff       (20)        0 2023-06-12 19:05:15.307839 wcs.adminauth-1.0.0/wcs/adminauth/
--rw-r--r--   0 maethu     (501) staff       (20)      546 2023-06-12 19:05:14.000000 wcs.adminauth-1.0.0/wcs/adminauth/__init__.py
--rw-r--r--   0 maethu     (501) staff       (20)     5487 2023-06-12 19:05:14.000000 wcs.adminauth-1.0.0/wcs/adminauth/auth.py
--rw-r--r--   0 maethu     (501) staff       (20)     4996 2023-06-12 19:05:14.000000 wcs.adminauth-1.0.0/wcs/adminauth/session.py
--rw-r--r--   0 maethu     (501) staff       (20)      803 2023-06-12 19:05:14.000000 wcs.adminauth-1.0.0/wcs/adminauth/testing.py
-drwxr-xr-x   0 maethu     (501) staff       (20)        0 2023-06-12 19:05:15.308255 wcs.adminauth-1.0.0/wcs/adminauth/tests/
--rw-r--r--   0 maethu     (501) staff       (20)      508 2023-06-12 19:05:14.000000 wcs.adminauth-1.0.0/wcs/adminauth/tests/__init__.py
--rw-r--r--   0 maethu     (501) staff       (20)     5480 2023-06-12 19:05:14.000000 wcs.adminauth-1.0.0/wcs/adminauth/tests/test_auth.py
--rw-r--r--   0 maethu     (501) staff       (20)     3404 2023-06-12 19:05:14.000000 wcs.adminauth-1.0.0/wcs/adminauth/tests/test_session.py
--rw-r--r--   0 maethu     (501) staff       (20)      400 2023-06-12 19:05:14.000000 wcs.adminauth-1.0.0/wcs/adminauth/tests/utils.py
-drwxr-xr-x   0 maethu     (501) staff       (20)        0 2023-06-12 19:05:15.307442 wcs.adminauth-1.0.0/wcs.adminauth.egg-info/
--rw-r--r--   0 maethu     (501) staff       (20)     2874 2023-06-12 19:05:15.000000 wcs.adminauth-1.0.0/wcs.adminauth.egg-info/PKG-INFO
--rw-r--r--   0 maethu     (501) staff       (20)      598 2023-06-12 19:05:15.000000 wcs.adminauth-1.0.0/wcs.adminauth.egg-info/SOURCES.txt
--rw-r--r--   0 maethu     (501) staff       (20)        1 2023-06-12 19:05:15.000000 wcs.adminauth-1.0.0/wcs.adminauth.egg-info/dependency_links.txt
--rw-r--r--   0 maethu     (501) staff       (20)       83 2023-06-12 19:05:15.000000 wcs.adminauth-1.0.0/wcs.adminauth.egg-info/entry_points.txt
--rw-r--r--   0 maethu     (501) staff       (20)        4 2023-06-12 19:05:15.000000 wcs.adminauth-1.0.0/wcs.adminauth.egg-info/namespace_packages.txt
--rw-r--r--   0 maethu     (501) staff       (20)        1 2023-06-12 19:05:15.000000 wcs.adminauth-1.0.0/wcs.adminauth.egg-info/not-zip-safe
--rw-r--r--   0 maethu     (501) staff       (20)       90 2023-06-12 19:05:15.000000 wcs.adminauth-1.0.0/wcs.adminauth.egg-info/requires.txt
--rw-r--r--   0 maethu     (501) staff       (20)        4 2023-06-12 19:05:15.000000 wcs.adminauth-1.0.0/wcs.adminauth.egg-info/top_level.txt
+drwxr-xr-x   0 maethu     (501) staff       (20)        0 2023-06-13 00:58:46.406897 wcs.adminauth-1.0.1/
+-rw-r--r--   0 maethu     (501) staff       (20)      162 2023-06-13 00:58:45.000000 wcs.adminauth-1.0.1/MANIFEST.in
+-rw-r--r--   0 maethu     (501) staff       (20)     2933 2023-06-13 00:58:46.406792 wcs.adminauth-1.0.1/PKG-INFO
+-rw-r--r--   0 maethu     (501) staff       (20)     2064 2023-06-13 00:58:45.000000 wcs.adminauth-1.0.1/README.rst
+drwxr-xr-x   0 maethu     (501) staff       (20)        0 2023-06-13 00:58:46.404467 wcs.adminauth-1.0.1/docs/
+-rw-r--r--   0 maethu     (501) staff       (20)      189 2023-06-13 00:58:46.000000 wcs.adminauth-1.0.1/docs/HISTORY.txt
+-rw-r--r--   0 maethu     (501) staff       (20)       38 2023-06-13 00:58:46.406933 wcs.adminauth-1.0.1/setup.cfg
+-rw-r--r--   0 maethu     (501) staff       (20)     1513 2023-06-13 00:58:46.000000 wcs.adminauth-1.0.1/setup.py
+drwxr-xr-x   0 maethu     (501) staff       (20)        0 2023-06-13 00:58:46.404571 wcs.adminauth-1.0.1/wcs/
+-rw-r--r--   0 maethu     (501) staff       (20)      244 2023-06-13 00:58:46.000000 wcs.adminauth-1.0.1/wcs/__init__.py
+drwxr-xr-x   0 maethu     (501) staff       (20)        0 2023-06-13 00:58:46.406025 wcs.adminauth-1.0.1/wcs/adminauth/
+-rw-r--r--   0 maethu     (501) staff       (20)      546 2023-06-13 00:58:46.000000 wcs.adminauth-1.0.1/wcs/adminauth/__init__.py
+-rw-r--r--   0 maethu     (501) staff       (20)     5487 2023-06-13 00:58:46.000000 wcs.adminauth-1.0.1/wcs/adminauth/auth.py
+-rw-r--r--   0 maethu     (501) staff       (20)      405 2023-06-13 00:58:46.000000 wcs.adminauth-1.0.1/wcs/adminauth/configure.zcml
+-rw-r--r--   0 maethu     (501) staff       (20)     4996 2023-06-13 00:58:46.000000 wcs.adminauth-1.0.1/wcs/adminauth/session.py
+-rw-r--r--   0 maethu     (501) staff       (20)     1004 2023-06-13 00:58:46.000000 wcs.adminauth-1.0.1/wcs/adminauth/session.zpt
+-rw-r--r--   0 maethu     (501) staff       (20)      803 2023-06-13 00:58:46.000000 wcs.adminauth-1.0.1/wcs/adminauth/testing.py
+drwxr-xr-x   0 maethu     (501) staff       (20)        0 2023-06-13 00:58:46.406434 wcs.adminauth-1.0.1/wcs/adminauth/tests/
+-rw-r--r--   0 maethu     (501) staff       (20)      508 2023-06-13 00:58:46.000000 wcs.adminauth-1.0.1/wcs/adminauth/tests/__init__.py
+drwxr-xr-x   0 maethu     (501) staff       (20)        0 2023-06-13 00:58:46.406644 wcs.adminauth-1.0.1/wcs/adminauth/tests/data/
+-rw-r--r--   0 maethu     (501) staff       (20)      210 2023-06-13 00:58:46.000000 wcs.adminauth-1.0.1/wcs/adminauth/tests/data/service_validate_invalid_ticket.xml
+-rw-r--r--   0 maethu     (501) staff       (20)      550 2023-06-13 00:58:46.000000 wcs.adminauth-1.0.1/wcs/adminauth/tests/data/service_validate_success.xml
+-rw-r--r--   0 maethu     (501) staff       (20)     5480 2023-06-13 00:58:46.000000 wcs.adminauth-1.0.1/wcs/adminauth/tests/test_auth.py
+-rw-r--r--   0 maethu     (501) staff       (20)     3404 2023-06-13 00:58:46.000000 wcs.adminauth-1.0.1/wcs/adminauth/tests/test_session.py
+-rw-r--r--   0 maethu     (501) staff       (20)      400 2023-06-13 00:58:46.000000 wcs.adminauth-1.0.1/wcs/adminauth/tests/utils.py
+drwxr-xr-x   0 maethu     (501) staff       (20)        0 2023-06-13 00:58:46.405400 wcs.adminauth-1.0.1/wcs.adminauth.egg-info/
+-rw-r--r--   0 maethu     (501) staff       (20)     2933 2023-06-13 00:58:46.000000 wcs.adminauth-1.0.1/wcs.adminauth.egg-info/PKG-INFO
+-rw-r--r--   0 maethu     (501) staff       (20)      768 2023-06-13 00:58:46.000000 wcs.adminauth-1.0.1/wcs.adminauth.egg-info/SOURCES.txt
+-rw-r--r--   0 maethu     (501) staff       (20)        1 2023-06-13 00:58:46.000000 wcs.adminauth-1.0.1/wcs.adminauth.egg-info/dependency_links.txt
+-rw-r--r--   0 maethu     (501) staff       (20)       83 2023-06-13 00:58:46.000000 wcs.adminauth-1.0.1/wcs.adminauth.egg-info/entry_points.txt
+-rw-r--r--   0 maethu     (501) staff       (20)        4 2023-06-13 00:58:46.000000 wcs.adminauth-1.0.1/wcs.adminauth.egg-info/namespace_packages.txt
+-rw-r--r--   0 maethu     (501) staff       (20)        1 2023-06-13 00:58:46.000000 wcs.adminauth-1.0.1/wcs.adminauth.egg-info/not-zip-safe
+-rw-r--r--   0 maethu     (501) staff       (20)       90 2023-06-13 00:58:46.000000 wcs.adminauth-1.0.1/wcs.adminauth.egg-info/requires.txt
+-rw-r--r--   0 maethu     (501) staff       (20)        4 2023-06-13 00:58:46.000000 wcs.adminauth-1.0.1/wcs.adminauth.egg-info/top_level.txt
```

### Comparing `wcs.adminauth-1.0.0/PKG-INFO` & `wcs.adminauth-1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wcs.adminauth
-Version: 1.0.0
+Version: 1.0.1
 Summary: Administrative login for Plone sites using CAS.
 Home-page: https://github.com/webcloud7/wcs.adminauth
 Author: webcloud7 ag
 Author-email: mailto:m.leimgruber@webcloud7.ch
 License: GPL2
 Classifier: Framework :: Plone
 Classifier: Framework :: Plone :: 6.0
@@ -94,11 +94,17 @@
 
 ``wcs.adminauth`` is licensed under GNU General Public License, version 2.
 
 Changelog
 =========
 
 
+1.0.1 (2023-06-12)
+------------------
+
+- Fix Manifest.in
+
+
 1.0.0 (2023-06-12)
 ------------------
 
 - Initial release based on ftw.zopemaster 1.4.x and python-cas 1.6.0
```

### Comparing `wcs.adminauth-1.0.0/README.rst` & `wcs.adminauth-1.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `wcs.adminauth-1.0.0/setup.py` & `wcs.adminauth-1.0.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import os
 
 
-version = '1.0.0'
+version = '1.0.1'
 
 tests_require = [
     'Plone',
     'plone.app.testing',
     'responses',
 ]
```

### Comparing `wcs.adminauth-1.0.0/wcs/adminauth/__init__.py` & `wcs.adminauth-1.0.1/wcs/adminauth/__init__.py`

 * *Files identical despite different names*

### Comparing `wcs.adminauth-1.0.0/wcs/adminauth/auth.py` & `wcs.adminauth-1.0.1/wcs/adminauth/auth.py`

 * *Files identical despite different names*

### Comparing `wcs.adminauth-1.0.0/wcs/adminauth/session.py` & `wcs.adminauth-1.0.1/wcs/adminauth/session.py`

 * *Files identical despite different names*

### Comparing `wcs.adminauth-1.0.0/wcs/adminauth/testing.py` & `wcs.adminauth-1.0.1/wcs/adminauth/testing.py`

 * *Files identical despite different names*

### Comparing `wcs.adminauth-1.0.0/wcs/adminauth/tests/test_auth.py` & `wcs.adminauth-1.0.1/wcs/adminauth/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `wcs.adminauth-1.0.0/wcs/adminauth/tests/test_session.py` & `wcs.adminauth-1.0.1/wcs/adminauth/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `wcs.adminauth-1.0.0/wcs.adminauth.egg-info/PKG-INFO` & `wcs.adminauth-1.0.1/wcs.adminauth.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wcs.adminauth
-Version: 1.0.0
+Version: 1.0.1
 Summary: Administrative login for Plone sites using CAS.
 Home-page: https://github.com/webcloud7/wcs.adminauth
 Author: webcloud7 ag
 Author-email: mailto:m.leimgruber@webcloud7.ch
 License: GPL2
 Classifier: Framework :: Plone
 Classifier: Framework :: Plone :: 6.0
@@ -94,11 +94,17 @@
 
 ``wcs.adminauth`` is licensed under GNU General Public License, version 2.
 
 Changelog
 =========
 
 
+1.0.1 (2023-06-12)
+------------------
+
+- Fix Manifest.in
+
+
 1.0.0 (2023-06-12)
 ------------------
 
 - Initial release based on ftw.zopemaster 1.4.x and python-cas 1.6.0
```

### Comparing `wcs.adminauth-1.0.0/wcs.adminauth.egg-info/SOURCES.txt` & `wcs.adminauth-1.0.1/wcs.adminauth.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -9,13 +9,17 @@
 wcs.adminauth.egg-info/entry_points.txt
 wcs.adminauth.egg-info/namespace_packages.txt
 wcs.adminauth.egg-info/not-zip-safe
 wcs.adminauth.egg-info/requires.txt
 wcs.adminauth.egg-info/top_level.txt
 wcs/adminauth/__init__.py
 wcs/adminauth/auth.py
+wcs/adminauth/configure.zcml
 wcs/adminauth/session.py
+wcs/adminauth/session.zpt
 wcs/adminauth/testing.py
 wcs/adminauth/tests/__init__.py
 wcs/adminauth/tests/test_auth.py
 wcs/adminauth/tests/test_session.py
-wcs/adminauth/tests/utils.py
+wcs/adminauth/tests/utils.py
+wcs/adminauth/tests/data/service_validate_invalid_ticket.xml
+wcs/adminauth/tests/data/service_validate_success.xml
```

