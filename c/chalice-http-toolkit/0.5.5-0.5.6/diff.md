# Comparing `tmp/chalice-http-toolkit-0.5.5.tar.gz` & `tmp/chalice-http-toolkit-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chalice-http-toolkit-0.5.5.tar", last modified: Sun Apr  2 23:13:42 2023, max compression
+gzip compressed data, was "chalice-http-toolkit-0.5.6.tar", last modified: Tue Jun 13 09:51:07 2023, max compression
```

## Comparing `chalice-http-toolkit-0.5.5.tar` & `chalice-http-toolkit-0.5.6.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 23:13:42.318019 chalice-http-toolkit-0.5.5/
--rw-rw-rw-   0 root         (0) root         (0)    34523 2023-04-02 23:13:29.000000 chalice-http-toolkit-0.5.5/LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)      105 2023-04-02 23:13:29.000000 chalice-http-toolkit-0.5.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1343 2023-04-02 23:13:42.318019 chalice-http-toolkit-0.5.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      666 2023-04-02 23:13:29.000000 chalice-http-toolkit-0.5.5/README.md
--rw-rw-rw-   0 root         (0) root         (0)      192 2023-04-02 23:13:29.000000 chalice-http-toolkit-0.5.5/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 23:13:42.309018 chalice-http-toolkit-0.5.5/chalice_http_toolkit/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-02 23:13:29.000000 chalice-http-toolkit-0.5.5/chalice_http_toolkit/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10548 2023-04-02 23:13:29.000000 chalice-http-toolkit-0.5.5/chalice_http_toolkit/cloudfront.py
--rw-rw-rw-   0 root         (0) root         (0)     8765 2023-04-02 23:13:29.000000 chalice-http-toolkit-0.5.5/chalice_http_toolkit/content.py
--rw-rw-rw-   0 root         (0) root         (0)     1314 2023-04-02 23:13:29.000000 chalice-http-toolkit-0.5.5/chalice_http_toolkit/multipart.py
--rw-rw-rw-   0 root         (0) root         (0)      507 2023-04-02 23:13:29.000000 chalice-http-toolkit-0.5.5/chalice_http_toolkit/response_with_binary.py
--rw-rw-rw-   0 root         (0) root         (0)     4510 2023-04-02 23:13:29.000000 chalice-http-toolkit-0.5.5/chalice_http_toolkit/tasking.py
--rw-r--r--   0 root         (0) root         (0)      160 2023-04-02 23:13:42.000000 chalice-http-toolkit-0.5.5/chalice_http_toolkit/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 23:13:42.311018 chalice-http-toolkit-0.5.5/chalice_http_toolkit.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1343 2023-04-02 23:13:42.000000 chalice-http-toolkit-0.5.5/chalice_http_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      800 2023-04-02 23:13:42.000000 chalice-http-toolkit-0.5.5/chalice_http_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-02 23:13:42.000000 chalice-http-toolkit-0.5.5/chalice_http_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-04-02 23:13:42.000000 chalice-http-toolkit-0.5.5/chalice_http_toolkit.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      113 2023-04-02 23:13:42.000000 chalice-http-toolkit-0.5.5/chalice_http_toolkit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       27 2023-04-02 23:13:42.000000 chalice-http-toolkit-0.5.5/chalice_http_toolkit.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-02 23:13:42.318019 chalice-http-toolkit-0.5.5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1808 2023-04-02 23:13:29.000000 chalice-http-toolkit-0.5.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 23:13:42.312018 chalice-http-toolkit-0.5.5/tools/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 23:13:42.312018 chalice-http-toolkit-0.5.5/tools/assets/
--rw-rw-rw-   0 root         (0) root         (0)     1688 2023-04-02 23:13:29.000000 chalice-http-toolkit-0.5.5/tools/assets/app.py
--rw-rw-rw-   0 root         (0) root         (0)      718 2023-04-02 23:13:29.000000 chalice-http-toolkit-0.5.5/tools/assets/config.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-02 23:13:42.315019 chalice-http-toolkit-0.5.5/tools/assets/magic/
--rw-rw-rw-   0 root         (0) root         (0)      111 2023-04-02 23:13:29.000000 chalice-http-toolkit-0.5.5/tools/assets/magic/etcmagic
--rwxrwxrwx   0 root         (0) root         (0)   111736 2023-04-02 23:13:29.000000 chalice-http-toolkit-0.5.5/tools/assets/magic/libmagic.so.1
--rwxrwxrwx   0 root         (0) root         (0)   111736 2023-04-02 23:13:29.000000 chalice-http-toolkit-0.5.5/tools/assets/magic/libmagic.so.1.0.0
--rw-rw-rw-   0 root         (0) root         (0)   624764 2023-04-02 23:13:29.000000 chalice-http-toolkit-0.5.5/tools/assets/magic/sharemagic
--rw-rw-rw-   0 root         (0) root         (0)  2286360 2023-04-02 23:13:29.000000 chalice-http-toolkit-0.5.5/tools/assets/magic/sharemagic.mgc
--rw-rw-rw-   0 root         (0) root         (0)     5063 2023-04-02 23:13:29.000000 chalice-http-toolkit-0.5.5/tools/chalice_http_toolkit.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:51:07.524757 chalice-http-toolkit-0.5.6/
+-rw-rw-rw-   0 root         (0) root         (0)    34523 2023-06-13 09:50:58.000000 chalice-http-toolkit-0.5.6/LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)      105 2023-06-13 09:50:58.000000 chalice-http-toolkit-0.5.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1343 2023-06-13 09:51:07.524757 chalice-http-toolkit-0.5.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      666 2023-06-13 09:50:58.000000 chalice-http-toolkit-0.5.6/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      192 2023-06-13 09:50:58.000000 chalice-http-toolkit-0.5.6/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:51:07.519757 chalice-http-toolkit-0.5.6/chalice_http_toolkit/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-13 09:50:58.000000 chalice-http-toolkit-0.5.6/chalice_http_toolkit/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10548 2023-06-13 09:50:58.000000 chalice-http-toolkit-0.5.6/chalice_http_toolkit/cloudfront.py
+-rw-rw-rw-   0 root         (0) root         (0)     8726 2023-06-13 09:50:58.000000 chalice-http-toolkit-0.5.6/chalice_http_toolkit/content.py
+-rw-rw-rw-   0 root         (0) root         (0)     1314 2023-06-13 09:50:58.000000 chalice-http-toolkit-0.5.6/chalice_http_toolkit/multipart.py
+-rw-rw-rw-   0 root         (0) root         (0)      507 2023-06-13 09:50:58.000000 chalice-http-toolkit-0.5.6/chalice_http_toolkit/response_with_binary.py
+-rw-rw-rw-   0 root         (0) root         (0)     4510 2023-06-13 09:50:58.000000 chalice-http-toolkit-0.5.6/chalice_http_toolkit/tasking.py
+-rw-r--r--   0 root         (0) root         (0)      160 2023-06-13 09:51:07.000000 chalice-http-toolkit-0.5.6/chalice_http_toolkit/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:51:07.520757 chalice-http-toolkit-0.5.6/chalice_http_toolkit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1343 2023-06-13 09:51:07.000000 chalice-http-toolkit-0.5.6/chalice_http_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      800 2023-06-13 09:51:07.000000 chalice-http-toolkit-0.5.6/chalice_http_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 09:51:07.000000 chalice-http-toolkit-0.5.6/chalice_http_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-13 09:51:07.000000 chalice-http-toolkit-0.5.6/chalice_http_toolkit.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      113 2023-06-13 09:51:07.000000 chalice-http-toolkit-0.5.6/chalice_http_toolkit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2023-06-13 09:51:07.000000 chalice-http-toolkit-0.5.6/chalice_http_toolkit.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-13 09:51:07.524757 chalice-http-toolkit-0.5.6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1808 2023-06-13 09:50:58.000000 chalice-http-toolkit-0.5.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:51:07.520757 chalice-http-toolkit-0.5.6/tools/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:51:07.520757 chalice-http-toolkit-0.5.6/tools/assets/
+-rw-rw-rw-   0 root         (0) root         (0)     1688 2023-06-13 09:50:58.000000 chalice-http-toolkit-0.5.6/tools/assets/app.py
+-rw-rw-rw-   0 root         (0) root         (0)      718 2023-06-13 09:50:58.000000 chalice-http-toolkit-0.5.6/tools/assets/config.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:51:07.522757 chalice-http-toolkit-0.5.6/tools/assets/magic/
+-rw-rw-rw-   0 root         (0) root         (0)      111 2023-06-13 09:50:58.000000 chalice-http-toolkit-0.5.6/tools/assets/magic/etcmagic
+-rwxrwxrwx   0 root         (0) root         (0)   111736 2023-06-13 09:50:58.000000 chalice-http-toolkit-0.5.6/tools/assets/magic/libmagic.so.1
+-rwxrwxrwx   0 root         (0) root         (0)   111736 2023-06-13 09:50:58.000000 chalice-http-toolkit-0.5.6/tools/assets/magic/libmagic.so.1.0.0
+-rw-rw-rw-   0 root         (0) root         (0)   624764 2023-06-13 09:50:58.000000 chalice-http-toolkit-0.5.6/tools/assets/magic/sharemagic
+-rw-rw-rw-   0 root         (0) root         (0)  2286360 2023-06-13 09:50:58.000000 chalice-http-toolkit-0.5.6/tools/assets/magic/sharemagic.mgc
+-rw-rw-rw-   0 root         (0) root         (0)     5063 2023-06-13 09:50:58.000000 chalice-http-toolkit-0.5.6/tools/chalice_http_toolkit.py
```

### Comparing `chalice-http-toolkit-0.5.5/LICENSE.txt` & `chalice-http-toolkit-0.5.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `chalice-http-toolkit-0.5.5/PKG-INFO` & `chalice-http-toolkit-0.5.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chalice-http-toolkit
-Version: 0.5.5
+Version: 0.5.6
 Summary: A Flask-like backend toolkit for building & deploying serverless websites directly to AWS Lambda
 Home-page: https://gitlab.com/chalice-http-toolkit/chalice-http-toolkit
 Author: Chris Lapa
 Author-email: 
 Project-URL: Bug Tracker, https://gitlab.com/chalice-http-toolkit/chalice-http-toolkit/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

### Comparing `chalice-http-toolkit-0.5.5/README.md` & `chalice-http-toolkit-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `chalice-http-toolkit-0.5.5/chalice_http_toolkit/cloudfront.py` & `chalice-http-toolkit-0.5.6/chalice_http_toolkit/cloudfront.py`

 * *Files identical despite different names*

### Comparing `chalice-http-toolkit-0.5.5/chalice_http_toolkit/content.py` & `chalice-http-toolkit-0.5.6/chalice_http_toolkit/content.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,16 +9,15 @@
 import json
 from PIL import Image, UnidentifiedImageError
 
 class ContentManager:
     ACCEPTS2PIL = {'image/jpeg': 'JPEG',
                    'image/jpg': 'JPEG',
                    'image/webp': 'WEBP',
-                   'image/png': 'PNG',
-                   'image/gif': 'GIF'}
+                   'image/png': 'PNG'}
 
     """
     Creates a ContentManager instance which allows rendering templates, returning static content
     and dynamic assets plus more. Generally after a ContentManager is called, set_static_handler_prefix()
     should be called directlty after to setup your static() handler in Jinja templates.
 
     :param templates_dir: Base path for templates
```

### Comparing `chalice-http-toolkit-0.5.5/chalice_http_toolkit/multipart.py` & `chalice-http-toolkit-0.5.6/chalice_http_toolkit/multipart.py`

 * *Files identical despite different names*

### Comparing `chalice-http-toolkit-0.5.5/chalice_http_toolkit/tasking.py` & `chalice-http-toolkit-0.5.6/chalice_http_toolkit/tasking.py`

 * *Files identical despite different names*

### Comparing `chalice-http-toolkit-0.5.5/chalice_http_toolkit.egg-info/PKG-INFO` & `chalice-http-toolkit-0.5.6/chalice_http_toolkit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chalice-http-toolkit
-Version: 0.5.5
+Version: 0.5.6
 Summary: A Flask-like backend toolkit for building & deploying serverless websites directly to AWS Lambda
 Home-page: https://gitlab.com/chalice-http-toolkit/chalice-http-toolkit
 Author: Chris Lapa
 Author-email: 
 Project-URL: Bug Tracker, https://gitlab.com/chalice-http-toolkit/chalice-http-toolkit/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

### Comparing `chalice-http-toolkit-0.5.5/chalice_http_toolkit.egg-info/SOURCES.txt` & `chalice-http-toolkit-0.5.6/chalice_http_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chalice-http-toolkit-0.5.5/setup.py` & `chalice-http-toolkit-0.5.6/setup.py`

 * *Files identical despite different names*

### Comparing `chalice-http-toolkit-0.5.5/tools/assets/app.py` & `chalice-http-toolkit-0.5.6/tools/assets/app.py`

 * *Files identical despite different names*

### Comparing `chalice-http-toolkit-0.5.5/tools/assets/config.json` & `chalice-http-toolkit-0.5.6/tools/assets/config.json`

 * *Files identical despite different names*

### Comparing `chalice-http-toolkit-0.5.5/tools/assets/magic/libmagic.so.1` & `chalice-http-toolkit-0.5.6/tools/assets/magic/libmagic.so.1`

 * *Files identical despite different names*

### Comparing `chalice-http-toolkit-0.5.5/tools/assets/magic/libmagic.so.1.0.0` & `chalice-http-toolkit-0.5.6/tools/assets/magic/libmagic.so.1.0.0`

 * *Files identical despite different names*

### Comparing `chalice-http-toolkit-0.5.5/tools/assets/magic/sharemagic` & `chalice-http-toolkit-0.5.6/tools/assets/magic/sharemagic`

 * *Files identical despite different names*

### Comparing `chalice-http-toolkit-0.5.5/tools/assets/magic/sharemagic.mgc` & `chalice-http-toolkit-0.5.6/tools/assets/magic/sharemagic.mgc`

 * *Files identical despite different names*

### Comparing `chalice-http-toolkit-0.5.5/tools/chalice_http_toolkit.py` & `chalice-http-toolkit-0.5.6/tools/chalice_http_toolkit.py`

 * *Files identical despite different names*

