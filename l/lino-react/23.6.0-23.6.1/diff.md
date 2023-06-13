# Comparing `tmp/lino_react-23.6.0.tar.gz` & `tmp/lino_react-23.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lino_react-23.6.0.tar", last modified: Thu Jun  8 14:51:59 2023, max compression
+gzip compressed data, was "lino_react-23.6.1.tar", last modified: Tue Jun 13 10:44:16 2023, max compression
```

## Comparing `lino_react-23.6.0.tar` & `lino_react-23.6.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-06-08 14:51:59.292652 lino_react-23.6.0/
--rw-rw-rw-   0 luc       (1000) www-data    (33)    34523 2021-04-12 19:37:56.000000 lino_react-23.6.0/COPYING
--rw-rw-rw-   0 luc       (1000) www-data    (33)      157 2020-04-27 23:26:14.000000 lino_react-23.6.0/MANIFEST.in
--rw-rw-r--   0 luc       (1000) www-data    (33)     1069 2023-06-08 14:51:59.292652 lino_react-23.6.0/PKG-INFO
--rw-rw-rw-   0 luc       (1000) www-data    (33)      178 2021-05-23 18:57:15.000000 lino_react-23.6.0/README.rst
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-06-08 14:51:59.284652 lino_react-23.6.0/lino_react/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      283 2021-05-23 18:57:15.000000 lino_react-23.6.0/lino_react/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-06-08 14:51:59.288652 lino_react-23.6.0/lino_react/react/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     3843 2023-03-25 09:38:34.000000 lino_react-23.6.0/lino_react/react/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-06-08 14:51:59.288652 lino_react-23.6.0/lino_react/react/__pycache__/
--rw-rw-r--   0 luc       (1000) www-data    (33)     2741 2023-05-02 09:01:04.000000 lino_react-23.6.0/lino_react/react/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 luc       (1000) www-data    (33)     3993 2023-05-02 09:01:06.000000 lino_react-23.6.0/lino_react/react/__pycache__/icons.cpython-310.pyc
--rw-rw-r--   0 luc       (1000) www-data    (33)      140 2023-05-02 09:01:04.000000 lino_react-23.6.0/lino_react/react/__pycache__/models.cpython-310.pyc
--rw-rw-r--   0 luc       (1000) www-data    (33)    18321 2023-06-08 14:51:15.000000 lino_react-23.6.0/lino_react/react/__pycache__/renderer.cpython-310.pyc
--rw-rw-r--   0 luc       (1000) www-data    (33)    20595 2023-05-02 13:45:04.000000 lino_react-23.6.0/lino_react/react/__pycache__/views.cpython-310.pyc
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-06-08 14:51:59.284652 lino_react-23.6.0/lino_react/react/config/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-06-08 14:51:59.288652 lino_react-23.6.0/lino_react/react/config/react/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2018-11-27 12:45:09.000000 lino_react-23.6.0/lino_react/react/config/react/linoweb.json
--rw-rw-r--   0 luc       (1000) www-data    (33)     1797 2023-01-07 15:27:20.000000 lino_react-23.6.0/lino_react/react/config/react/main.html
--rw-rw-r--   0 luc       (1000) www-data    (33)    16246 2022-11-30 04:23:52.000000 lino_react-23.6.0/lino_react/react/config/react/service-worker.js
--rw-rw-rw-   0 luc       (1000) www-data    (33)     3893 2023-04-24 18:09:52.000000 lino_react-23.6.0/lino_react/react/icons.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       36 2018-11-22 22:23:05.000000 lino_react-23.6.0/lino_react/react/index.js
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2023-03-28 18:53:35.000000 lino_react-23.6.0/lino_react/react/models.py
--rw-rw-r--   0 luc       (1000) www-data    (33)    29204 2023-06-08 14:51:12.000000 lino_react-23.6.0/lino_react/react/renderer.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-06-08 14:51:59.284652 lino_react-23.6.0/lino_react/react/static/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-06-08 14:51:59.288652 lino_react-23.6.0/lino_react/react/static/media/
--rw-rw-rw-   0 luc       (1000) www-data    (33)    10355 2021-05-17 15:54:58.000000 lino_react-23.6.0/lino_react/react/static/media/color.6441e63a.png
--rw-rw-rw-   0 luc       (1000) www-data    (33)    10355 2021-01-26 04:29:47.000000 lino_react-23.6.0/lino_react/react/static/media/color.c7a33805.png
--rw-rw-rw-   0 luc       (1000) www-data    (33)    13112 2020-09-29 17:55:04.000000 lino_react-23.6.0/lino_react/react/static/media/line.567f5738.gif
--rw-rw-rw-   0 luc       (1000) www-data    (33)    39748 2021-01-26 04:29:47.000000 lino_react-23.6.0/lino_react/react/static/media/primeicons.2d2afb27.eot
--rw-rw-rw-   0 luc       (1000) www-data    (33)    57384 2021-05-17 15:54:58.000000 lino_react-23.6.0/lino_react/react/static/media/primeicons.3a0d4a58.ttf
--rw-rw-rw-   0 luc       (1000) www-data    (33)    39648 2021-01-26 04:29:47.000000 lino_react-23.6.0/lino_react/react/static/media/primeicons.66ee0deb.woff
--rw-rw-rw-   0 luc       (1000) www-data    (33)   234640 2021-05-17 15:54:58.000000 lino_react-23.6.0/lino_react/react/static/media/primeicons.c55d94a2.svg
--rw-rw-rw-   0 luc       (1000) www-data    (33)    39572 2021-01-26 04:29:47.000000 lino_react-23.6.0/lino_react/react/static/media/primeicons.df0140f8.ttf
--rw-rw-rw-   0 luc       (1000) www-data    (33)    57560 2021-05-17 15:54:58.000000 lino_react-23.6.0/lino_react/react/static/media/primeicons.dfbfef2d.eot
--rw-rw-rw-   0 luc       (1000) www-data    (33)   163568 2021-01-26 04:29:47.000000 lino_react-23.6.0/lino_react/react/static/media/primeicons.e5e0e944.svg
--rw-rw-rw-   0 luc       (1000) www-data    (33)    57460 2021-05-17 15:54:58.000000 lino_react-23.6.0/lino_react/react/static/media/primeicons.e61f3495.woff
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-06-08 14:51:59.292652 lino_react-23.6.0/lino_react/react/static/react/
--rw-rw-r--   0 luc       (1000) www-data    (33)  1776706 2023-04-29 06:53:49.000000 lino_react-23.6.0/lino_react/react/static/react/main.js
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2437 2021-09-23 03:04:12.000000 lino_react-23.6.0/lino_react/react/static/react/main.js.LICENSE.txt
--rw-rw-r--   0 luc       (1000) www-data    (33)    28705 2023-03-24 10:38:37.000000 lino_react-23.6.0/lino_react/react/views.py
--rw-rw-r--   0 luc       (1000) www-data    (33)     1431 2023-06-08 14:51:32.000000 lino_react-23.6.0/lino_react/setup_info.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-06-08 14:51:59.288652 lino_react-23.6.0/lino_react.egg-info/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1069 2023-06-08 14:51:59.000000 lino_react-23.6.0/lino_react.egg-info/PKG-INFO
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1522 2023-06-08 14:51:59.000000 lino_react-23.6.0/lino_react.egg-info/SOURCES.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)        1 2023-06-08 14:51:59.000000 lino_react-23.6.0/lino_react.egg-info/dependency_links.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)        1 2019-01-08 09:40:17.000000 lino_react-23.6.0/lino_react.egg-info/not-zip-safe
--rw-rw-rw-   0 luc       (1000) www-data    (33)        5 2023-06-08 14:51:59.000000 lino_react-23.6.0/lino_react.egg-info/requires.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)       11 2023-06-08 14:51:59.000000 lino_react-23.6.0/lino_react.egg-info/top_level.txt
--rw-rw-r--   0 luc       (1000) www-data    (33)       38 2023-06-08 14:51:59.292652 lino_react-23.6.0/setup.cfg
--rw-rw-rw-   0 luc       (1000) www-data    (33)      183 2021-04-06 11:15:38.000000 lino_react-23.6.0/setup.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      348 2021-05-23 18:57:15.000000 lino_react-23.6.0/tasks.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-06-13 10:44:16.616160 lino_react-23.6.1/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    34523 2021-04-12 19:37:56.000000 lino_react-23.6.1/COPYING
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      157 2020-04-27 23:26:14.000000 lino_react-23.6.1/MANIFEST.in
+-rw-rw-r--   0 luc       (1000) www-data    (33)     1069 2023-06-13 10:44:16.616160 lino_react-23.6.1/PKG-INFO
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      178 2021-05-23 18:57:15.000000 lino_react-23.6.1/README.rst
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-06-13 10:44:16.612160 lino_react-23.6.1/lino_react/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      283 2021-05-23 18:57:15.000000 lino_react-23.6.1/lino_react/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-06-13 10:44:16.612160 lino_react-23.6.1/lino_react/react/
+-rw-rw-r--   0 luc       (1000) www-data    (33)     4628 2023-06-13 10:30:58.000000 lino_react-23.6.1/lino_react/react/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-06-13 10:44:16.612160 lino_react-23.6.1/lino_react/react/__pycache__/
+-rw-rw-r--   0 luc       (1000) www-data    (33)     3362 2023-06-13 10:37:43.000000 lino_react-23.6.1/lino_react/react/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 luc       (1000) www-data    (33)     3993 2023-05-02 09:01:06.000000 lino_react-23.6.1/lino_react/react/__pycache__/icons.cpython-310.pyc
+-rw-rw-r--   0 luc       (1000) www-data    (33)      140 2023-05-02 09:01:04.000000 lino_react-23.6.1/lino_react/react/__pycache__/models.cpython-310.pyc
+-rw-rw-r--   0 luc       (1000) www-data    (33)    18321 2023-06-08 14:52:20.000000 lino_react-23.6.1/lino_react/react/__pycache__/renderer.cpython-310.pyc
+-rw-rw-r--   0 luc       (1000) www-data    (33)    20595 2023-05-02 13:45:04.000000 lino_react-23.6.1/lino_react/react/__pycache__/views.cpython-310.pyc
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-06-13 10:44:16.612160 lino_react-23.6.1/lino_react/react/config/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-06-13 10:44:16.612160 lino_react-23.6.1/lino_react/react/config/react/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2018-11-27 12:45:09.000000 lino_react-23.6.1/lino_react/react/config/react/linoweb.json
+-rw-rw-r--   0 luc       (1000) www-data    (33)     1910 2023-06-11 12:10:21.000000 lino_react-23.6.1/lino_react/react/config/react/main.html
+-rw-rw-r--   0 luc       (1000) www-data    (33)    16246 2022-11-30 04:23:52.000000 lino_react-23.6.1/lino_react/react/config/react/service-worker.js
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     3893 2023-04-24 18:09:52.000000 lino_react-23.6.1/lino_react/react/icons.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       36 2018-11-22 22:23:05.000000 lino_react-23.6.1/lino_react/react/index.js
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2023-03-28 18:53:35.000000 lino_react-23.6.1/lino_react/react/models.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)    29204 2023-06-13 10:43:27.000000 lino_react-23.6.1/lino_react/react/renderer.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-06-13 10:44:16.612160 lino_react-23.6.1/lino_react/react/static/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-06-13 10:44:16.616160 lino_react-23.6.1/lino_react/react/static/media/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    10355 2021-05-17 15:54:58.000000 lino_react-23.6.1/lino_react/react/static/media/color.6441e63a.png
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    10355 2021-01-26 04:29:47.000000 lino_react-23.6.1/lino_react/react/static/media/color.c7a33805.png
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    13112 2020-09-29 17:55:04.000000 lino_react-23.6.1/lino_react/react/static/media/line.567f5738.gif
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    39748 2021-01-26 04:29:47.000000 lino_react-23.6.1/lino_react/react/static/media/primeicons.2d2afb27.eot
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    57384 2021-05-17 15:54:58.000000 lino_react-23.6.1/lino_react/react/static/media/primeicons.3a0d4a58.ttf
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    39648 2021-01-26 04:29:47.000000 lino_react-23.6.1/lino_react/react/static/media/primeicons.66ee0deb.woff
+-rw-rw-rw-   0 luc       (1000) www-data    (33)   234640 2021-05-17 15:54:58.000000 lino_react-23.6.1/lino_react/react/static/media/primeicons.c55d94a2.svg
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    39572 2021-01-26 04:29:47.000000 lino_react-23.6.1/lino_react/react/static/media/primeicons.df0140f8.ttf
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    57560 2021-05-17 15:54:58.000000 lino_react-23.6.1/lino_react/react/static/media/primeicons.dfbfef2d.eot
+-rw-rw-rw-   0 luc       (1000) www-data    (33)   163568 2021-01-26 04:29:47.000000 lino_react-23.6.1/lino_react/react/static/media/primeicons.e5e0e944.svg
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    57460 2021-05-17 15:54:58.000000 lino_react-23.6.1/lino_react/react/static/media/primeicons.e61f3495.woff
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-06-13 10:44:16.616160 lino_react-23.6.1/lino_react/react/static/react/
+-rw-rw-r--   0 luc       (1000) www-data    (33)  1776853 2023-06-13 09:28:20.000000 lino_react-23.6.1/lino_react/react/static/react/main.js
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     2437 2021-09-23 03:04:12.000000 lino_react-23.6.1/lino_react/react/static/react/main.js.LICENSE.txt
+-rw-rw-r--   0 luc       (1000) www-data    (33)    28705 2023-03-24 10:38:37.000000 lino_react-23.6.1/lino_react/react/views.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)     1431 2023-06-13 10:43:55.000000 lino_react-23.6.1/lino_react/setup_info.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-06-13 10:44:16.612160 lino_react-23.6.1/lino_react.egg-info/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1069 2023-06-13 10:44:16.000000 lino_react-23.6.1/lino_react.egg-info/PKG-INFO
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1522 2023-06-13 10:44:16.000000 lino_react-23.6.1/lino_react.egg-info/SOURCES.txt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        1 2023-06-13 10:44:16.000000 lino_react-23.6.1/lino_react.egg-info/dependency_links.txt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        1 2019-01-08 09:40:17.000000 lino_react-23.6.1/lino_react.egg-info/not-zip-safe
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        5 2023-06-13 10:44:16.000000 lino_react-23.6.1/lino_react.egg-info/requires.txt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       11 2023-06-13 10:44:16.000000 lino_react-23.6.1/lino_react.egg-info/top_level.txt
+-rw-rw-r--   0 luc       (1000) www-data    (33)       38 2023-06-13 10:44:16.616160 lino_react-23.6.1/setup.cfg
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      183 2021-04-06 11:15:38.000000 lino_react-23.6.1/setup.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      348 2021-05-23 18:57:15.000000 lino_react-23.6.1/tasks.py
```

### Comparing `lino_react-23.6.0/COPYING` & `lino_react-23.6.1/COPYING`

 * *Files identical despite different names*

### Comparing `lino_react-23.6.0/PKG-INFO` & `lino_react-23.6.1/lino_react.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: lino_react
-Version: 23.6.0
+Name: lino-react
+Version: 23.6.1
 Summary: The React front end for Lino
 Home-page: https://gitlab.com/lino-framework/react
 Author: Rumma & Ko Ltd
 Author-email: info@lino-framework.org
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier:   Programming Language :: Python
```

### Comparing `lino_react-23.6.0/lino_react/react/__pycache__/icons.cpython-310.pyc` & `lino_react-23.6.1/lino_react/react/__pycache__/icons.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `lino_react-23.6.0/lino_react/react/__pycache__/renderer.cpython-310.pyc` & `lino_react-23.6.1/lino_react/react/__pycache__/renderer.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jun  8 14:51:12 2023 UTC, .py size: 29204 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 e0ea 8164 1472 0000  o..........d.r..
+00000000: 6f0d 0d0a 0000 0000 21eb 8164 5472 0000  o.......!..dTr..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 a201 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c03 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 0100 6400 6405 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 0100 6400 6406 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
 00000070: 0100 6400 6407 6c0b 6d0c 5a0c 0100 6400  ..d.d.l.m.Z...d.
@@ -651,16 +651,16 @@
 000028a0: 72b2 0000 00da 0a6a 6176 6173 6372 6970  r......javascrip
 000028b0: 7472 f600 0000 da07 6765 7461 7474 72da  tr......getattr.
 000028c0: 0173 2906 723f 0000 0072 a500 0000 da01  .s).r?...r......
 000028d0: 68da 026a 7372 c900 0000 da03 7572 6c72  h..jsr......urlr
 000028e0: 3600 0000 7236 0000 0072 3700 0000 723e  6...r6...r7...r>
 000028f0: 0000 0052 0100 0073 5400 0000 0c04 0801  ...R...sT.......
 00002900: 0a01 0e01 0c01 0201 0603 0c01 0601 0a01  ................
-00002910: 0801 0a01 0a01 0601 1603 0a02 0a01 1001  ................
-00002920: 0c01 0801 0e01 0a01 0601 1401 0c01 1002  ................
+00002910: 0801 0a01 0a01 0601 1603 0a02 0a02 1001  ................
+00002920: 0c01 0801 0e01 0a01 0601 1401 0c01 1004  ................
 00002930: 1001 0a02 0a01 1001 0a01 0801 0607 0c02  ................
 00002940: 0202 0601 0a02 06fd 0e04 1602 0a02 0402  ................
 00002950: 7a18 5265 6e64 6572 6572 2e70 7932 6a73  z.Renderer.py2js
 00002960: 5f63 6f6e 7665 7274 6572 6304 0000 0000  _converterc.....
 00002970: 0000 0000 0000 0005 0000 0004 0000 0043  ...............C
 00002980: 0000 0073 5000 0000 7400 7c01 6a01 7c02  ...sP...t.|.j.|.
 00002990: 6401 8d02 7d04 7c01 6a02 721a 7c01 6a02  d...}.|.j.r.|.j.
@@ -672,30 +672,30 @@
 000029f0: 2d29 01da 0769 636f 6e43 6c73 2901 da07  -)...iconCls)...
 00002a00: 746f 6f6c 5469 7029 0972 7100 0000 7295  toolTip).rq...r.
 00002a10: 0000 0072 a300 0000 726c 0000 0072 e400  ...r....rl...r..
 00002a20: 0000 7277 0000 0072 0400 0000 726f 0000  ..rw...r....ro..
 00002a30: 00da 0d75 7365 5f71 7569 636b 7469 7073  ...use_quicktips
 00002a40: 2905 723f 0000 00da 026d 6972 f500 0000  ).r?.....mir....
 00002a50: 72b2 0000 00da 0164 7236 0000 0072 3600  r......dr6...r6.
-00002a60: 0000 7237 0000 0072 fd00 0000 a001 0000  ..r7...r........
+00002a60: 0000 7237 0000 0072 fd00 0000 a301 0000  ..r7...r........
 00002a70: 730c 0000 000e 0410 0116 010c 010c 0304  s...............
 00002a80: 017a 1552 656e 6465 7265 722e 6861 6e64  .z.Renderer.hand
 00002a90: 6c65 725f 6974 656d 6302 0000 0000 0000  ler_itemc.......
 00002aa0: 0000 0000 0005 0000 0005 0000 004f 0000  .............O..
 00002ab0: 0073 2000 0000 7c01 6a00 6402 6900 7c03  .s ...|.j.d.i.|.
 00002ac0: a401 8e01 7d04 7c00 a001 7c01 7c01 6a02  ....}.|...|.|.j.
 00002ad0: 7c04 a103 5300 2903 7a36 2047 656e 6572  |...S.).z6 Gener
 00002ae0: 6174 6573 206a 7320 7374 7269 6e67 2066  ates js string f
 00002af0: 6f72 2061 6374 696f 6e20 6275 7474 6f6e  or action button
 00002b00: 2063 616c 6c73 2e0a 2020 2020 2020 2020   calls..        
 00002b10: 4e72 3600 0000 2903 72be 0000 0072 ff00  Nr6...).r....r..
 00002b20: 0000 72a3 0000 0029 0572 3f00 0000 72c9  ..r....).r?...r.
 00002b30: 0000 0072 ca00 0000 72cb 0000 0072 cc00  ...r....r....r..
 00002b40: 0000 7236 0000 0072 3600 0000 7237 0000  ..r6...r6...r7..
-00002b50: 0072 fe00 0000 ae01 0000 7304 0000 0010  .r........s.....
+00002b50: 0072 fe00 0000 b101 0000 7304 0000 0010  .r........s.....
 00002b60: 0410 017a 1852 656e 6465 7265 722e 7265  ...z.Renderer.re
 00002b70: 7175 6573 745f 6861 6e64 6c65 7263 0400  quest_handlerc..
 00002b80: 0000 0000 0000 0000 0000 0800 0000 0800  ................
 00002b90: 0000 4300 0000 739c 0000 007c 026a 007d  ..C...s....|.j.}
 00002ba0: 047c 02a0 01a1 00a0 0264 0164 02a1 025c  .|.......d.d...\
 00002bb0: 027d 057d 067c 0373 1169 007d 037c 0164  .}.}.|.s.i.}.|.d
 00002bc0: 0075 0172 2274 037c 0164 0383 0272 227c  .u.r"t.|.d...r"|
@@ -714,29 +714,29 @@
 00002c90: 0072 be00 0000 da0a 7375 6273 745f 7573  .r......subst_us
 00002ca0: 6572 720c 0000 00da 1455 524c 5f50 4152  err......URL_PAR
 00002cb0: 414d 5f53 5542 5354 5f55 5345 5272 ec00  AM_SUBST_USERr..
 00002cc0: 0000 7226 0000 0072 7100 0000 2908 723f  ..r&...rq...).r?
 00002cd0: 0000 0072 c900 0000 72a3 0000 0072 e000  ...r....r....r..
 00002ce0: 0000 724f 0000 0072 e900 0000 7294 0000  ..rO...r....r...
 00002cf0: 0072 e700 0000 7236 0000 0072 3600 0000  .r....r6...r6...
-00002d00: 7237 0000 0072 ff00 0000 b801 0000 7322  r7...r........s"
+00002d00: 7237 0000 0072 ff00 0000 bb01 0000 7322  r7...r........s"
 00002d10: 0000 0006 0214 0204 0204 0112 0210 010a  ................
 00002d20: 020c 0112 1106 0112 0206 0202 0102 0102  ................
 00002d30: 0102 010a fc7a 1452 656e 6465 7265 722e  .....z.Renderer.
 00002d40: 6163 7469 6f6e 5f63 616c 6c63 0200 0000  action_callc....
 00002d50: 0000 0000 0000 0000 0200 0000 0400 0000  ................
 00002d60: 4300 0000 732e 0000 007c 0173 0464 0053  C...s....|.s.d.S
 00002d70: 0074 007c 0174 0183 0273 0d74 017c 0183  .t.|.t...s.t.|..
 00002d80: 017d 0174 027c 0164 0164 028d 027d 0164  .}.t.|.d.d...}.d
 00002d90: 037c 0117 0053 0029 044e 4629 01da 0571  .|...S.).NF)...q
 00002da0: 756f 7465 7a0b 6a61 7661 7363 7269 7074  uotez.javascript
 00002db0: 3a29 0372 a000 0000 7245 0000 0072 0300  :).r....rE...r..
 00002dc0: 0000 2902 723f 0000 0072 0401 0000 7236  ..).r?...r....r6
 00002dd0: 0000 0072 3600 0000 7237 0000 00da 066a  ...r6...r7.....j
-00002de0: 7332 7572 6ce2 0100 0073 0c00 0000 0401  s2url....s......
+00002de0: 7332 7572 6ce4 0100 0073 0c00 0000 0401  s2url....s......
 00002df0: 0401 0a02 0801 0c01 0801 7a0f 5265 6e64  ..........z.Rend
 00002e00: 6572 6572 2e6a 7332 7572 6c63 0600 0000  erer.js2urlc....
 00002e10: 0000 0000 0000 0000 0700 0000 0400 0000  ................
 00002e20: 4300 0000 7356 0000 0074 006a 016a 0272  C...sV...t.j.j.r
 00002e30: 2774 006a 016a 0372 0f64 017c 047c 0566  't.j.j.r.d.|.|.f
 00002e40: 0216 007d 066e 0264 027d 067c 0272 1974  ...}.n.d.}.|.r.t
 00002e50: 0464 037c 067c 0283 037d 067c 0672 297c  .d.|.|...}.|.r)|
@@ -749,15 +749,15 @@
 00002ec0: 686f 775f 696e 7465 726e 616c 5f66 6965  how_internal_fie
 00002ed0: 6c64 5f6e 616d 6573 7206 0000 0072 7700  ld_namesr....rw.
 00002ee0: 0000 2907 723f 0000 0072 cb00 0000 72b2  ..).r?...r....r.
 00002ef0: 0000 0072 7400 0000 da0a 6461 7461 736f  ...rt.....dataso
 00002f00: 7572 6365 da09 6669 656c 646e 616d 65da  urce..fieldname.
 00002f10: 0374 7474 7236 0000 0072 3600 0000 7237  .tttr6...r6...r7
 00002f20: 0000 00da 0d61 6464 5f68 656c 705f 7465  .....add_help_te
-00002f30: 7874 eb01 0000 7318 0000 0008 0108 010e  xt....s.........
+00002f30: 7874 ed01 0000 7318 0000 0008 0108 010e  xt....s.........
 00002f40: 0104 0204 010c 0104 0108 0402 010e ff04  ................
 00002f50: f504 077a 1652 656e 6465 7265 722e 6164  ...z.Renderer.ad
 00002f60: 645f 6865 6c70 5f74 6578 7463 0200 0000  d_help_textc....
 00002f70: 0000 0000 0000 0000 0500 0000 0300 0000  ................
 00002f80: 4300 0000 7356 0000 0074 0083 007d 0264  C...sV...t...}.d
 00002f90: 017c 0117 0064 0217 007d 037c 006a 01a0  .|...d...}.|.j..
 00002fa0: 0264 03a1 0164 0419 007d 047c 0264 0575  .d...d...}.|.d.u
@@ -773,15 +773,15 @@
 00003040: 706c 6174 6572 0f01 0000 7243 0000 0072  plater....rC...r
 00003050: 0700 0000 da0c 6765 745f 6c61 6e67 7561  ......get_langua
 00003060: 6765 2905 723f 0000 0072 e900 0000 da09  ge).r?...r......
 00003070: 7573 6572 5f74 7970 65da 0866 696c 656e  user_type..filen
 00003080: 616d 65da 0966 696c 655f 7479 7065 7236  ame..file_typer6
 00003090: 0000 0072 3600 0000 7237 0000 00da 156c  ...r6...r7.....l
 000030a0: 696e 6f5f 6a73 5f70 6172 7473 5f63 6875  ino_js_parts_chu
-000030b0: 6e6b 6564 fa01 0000 730e 0000 0006 020c  nked....s.......
+000030b0: 6e6b 6564 fc01 0000 730e 0000 0006 020c  nked....s.......
 000030c0: 0110 0108 010e 0114 010a 017a 1e52 656e  ...........z.Ren
 000030d0: 6465 7265 722e 6c69 6e6f 5f6a 735f 7061  derer.lino_js_pa
 000030e0: 7274 735f 6368 756e 6b65 6463 0200 0000  rts_chunkedc....
 000030f0: 0000 0000 0000 0000 1100 0000 0600 0000  ................
 00003100: 4300 0000 73de 0100 0067 007d 0267 007d  C...s....g.}.g.}
 00003110: 037c 0144 005d e47d 047c 04a0 00a1 007d  .|.D.].}.|.....}
 00003120: 057c 0573 127c 046a 016a 0272 cc74 036a  .|.s.|.j.j.r.t.j
@@ -838,15 +838,15 @@
 00003450: 0768 6f74 6b65 7973 728f 0000 00da 026c  .hotkeysr......l
 00003460: 68da 1161 6374 696f 6e5f 6465 7363 7269  h..action_descri
 00003470: 7074 6f72 da04 7462 6173 da09 636f 6d62  ptor..tbas..comb
 00003480: 6f5f 6d61 7072 4f00 0000 da03 7462 6172  o_maprO.....tbar
 00003490: b200 0000 7224 0100 0072 2b01 0000 7225  ....r$...r+...r%
 000034a0: 0100 0072 2d01 0000 7234 0000 0072 3600  ...r-...r4...r6.
 000034b0: 0000 7236 0000 0072 3700 0000 da0c 6163  ..r6...r7.....ac
-000034c0: 7469 6f6e 7332 6a73 6f6e 0402 0000 7368  tions2json....sh
+000034c0: 7469 6f6e 7332 6a73 6f6e 0602 0000 7368  tions2json....sh
 000034d0: 0000 0004 0404 0108 0208 010c 010e 0204  ................
 000034e0: 0110 0108 0104 0106 0106 0208 0108 ff0e  ................
 000034f0: 0308 010c 0108 0104 0108 0110 0108 020c  ................
 00003500: 0208 0108 0210 010a 020a 010c 010a 0208  ................
 00003510: 020c 010a 010c 0108 010a 0102 8004 0210  ................
 00003520: 010c 0114 0102 8008 020a 0208 020c 010a  ................
 00003530: 010c 0108 010a 0102 8008 027a 1552 656e  ...........z.Ren
@@ -860,25 +860,25 @@
 000035b0: 6405 8d02 7d02 7c02 a000 6400 7c03 6702  d...}.|...d.|.g.
 000035c0: a101 0100 7c02 5300 2906 4e72 0100 0000  ....|.S.).Nr....
 000035d0: 722c 0000 0063 0100 0000 0000 0000 0000  r,...c..........
 000035e0: 0000 0100 0000 0200 0000 5300 0000 7308  ..........S...s.
 000035f0: 0000 007c 0064 0119 0053 0029 024e 7201  ...|.d...S.).Nr.
 00003600: 0000 0072 3600 0000 2901 7235 0000 0072  ...r6...).r5...r
 00003610: 3600 0000 7236 0000 0072 3700 0000 da08  6...r6...r7.....
-00003620: 3c6c 616d 6264 613e 5002 0000 7302 0000  <lambda>P...s...
+00003620: 3c6c 616d 6264 613e 5202 0000 7302 0000  <lambda>R...s...
 00003630: 0008 007a 2c52 656e 6465 7265 722e 6469  ...z,Renderer.di
 00003640: 7370 6c61 795f 6d6f 6465 326a 736f 6e2e  splay_mode2json.
 00003650: 3c6c 6f63 616c 733e 2e3c 6c61 6d62 6461  <locals>.<lambda
 00003660: 3ea9 0172 3300 0000 2903 722c 0100 0072  >..r3...).r,...r
 00003670: 7800 0000 da06 736f 7274 6564 2905 723f  x.....sorted).r?
 00003680: 0000 00da 0c64 6973 706c 6179 5f6d 6f64  .....display_mod
 00003690: 65da 0364 6d73 da03 646d 6472 9200 0000  e..dms..dmdr....
 000036a0: 7236 0000 0072 3600 0000 7237 0000 00da  r6...r6...r7....
 000036b0: 1164 6973 706c 6179 5f6d 6f64 6532 6a73  .display_mode2js
-000036c0: 6f6e 4802 0000 7312 0000 0004 0104 0108  onH...s.........
+000036c0: 6f6e 4a02 0000 7312 0000 0004 0104 0108  onJ...s.........
 000036d0: 010c 010a 0110 0210 010e 0104 017a 1a52  .............z.R
 000036e0: 656e 6465 7265 722e 6469 7370 6c61 795f  enderer.display_
 000036f0: 6d6f 6465 326a 736f 6e63 0200 0000 0000  mode2jsonc......
 00003700: 0000 0000 0000 1100 0000 0800 0000 4300  ..............C.
 00003710: 0000 73fe 0200 0074 007c 0183 0172 0974  ..s....t.|...r.t
 00003720: 017c 0174 0283 0273 0b4a 0082 017c 00a0  .|.t...s.J...|..
 00003730: 037c 016a 04a1 015c 027d 027d 0374 057c  .|.j...\.}.}.t.|
@@ -932,15 +932,15 @@
 00003a30: 0865 6469 7461 626c 6529 0172 3001 0000  .editable).r0...
 00003a40: 7a0f 2573 2068 6173 206e 6f20 7374 6f72  z.%s has no stor
 00003a50: 65da 0b67 6574 5f63 6f6c 756d 6e73 7201  e..get_columnsr.
 00003a60: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
 00003a70: 0100 0000 0100 0000 5300 0000 7306 0000  ........S...s...
 00003a80: 007c 006a 0053 0072 3a00 0000 a901 7252  .|.j.S.r:.....rR
 00003a90: 0000 00a9 0172 8c00 0000 7236 0000 0072  .....r....r6...r
-00003aa0: 3600 0000 7237 0000 0072 3701 0000 6d02  6...r7...r7...m.
+00003aa0: 3600 0000 7237 0000 0072 3701 0000 6f02  6...r7...r7...o.
 00003ab0: 0000 7302 0000 0006 007a 2552 656e 6465  ..s......z%Rende
 00003ac0: 7265 722e 6163 746f 7232 6a73 6f6e 2e3c  rer.actor2json.<
 00003ad0: 6c6f 6361 6c73 3e2e 3c6c 616d 6264 613e  locals>.<lambda>
 00003ae0: 7238 0100 0029 01da 0c66 6965 6c64 735f  r8...)...fields_
 00003af0: 696e 6465 7872 4401 0000 722c 0000 0029  indexrD...r,...)
 00003b00: 01da 1366 6965 6c64 735f 696e 6465 785f  ...fields_index_
 00003b10: 6869 6464 656e e902 0000 00da 0363 6f6c  hidden.......col
@@ -970,37 +970,37 @@
 00003c90: 027c 0164 0064 0184 007c 026a 0044 0083  .|.d.d...|.j.D..
 00003ca0: 0193 0271 0253 0029 0263 0100 0000 0000  ...q.S.).c......
 00003cb0: 0000 0000 0000 0200 0000 0300 0000 5300  ..............S.
 00003cc0: 0000 f312 0000 0067 007c 005d 057d 017c  .......g.|.].}.|
 00003cd0: 016a 0091 0271 0253 0072 3600 0000 7242  .j...q.S.r6...rB
 00003ce0: 0100 0029 0272 4600 0000 da02 6366 7236  ...).rF.....cfr6
 00003cf0: 0000 0072 3600 0000 7237 0000 0072 4800  ...r6...r7...rH.
-00003d00: 0000 a302 0000 f302 0000 0012 007a 3252  .............z2R
+00003d00: 0000 a502 0000 f302 0000 0012 007a 3252  .............z2R
 00003d10: 656e 6465 7265 722e 6163 746f 7232 6a73  enderer.actor2js
 00003d20: 6f6e 2e3c 6c6f 6361 6c73 3e2e 3c64 6963  on.<locals>.<dic
 00003d30: 7463 6f6d 703e 2e3c 6c69 7374 636f 6d70  tcomp>.<listcomp
 00003d40: 3e29 01da 0e63 6f6e 7465 7874 5f66 6965  >)...context_fie
 00003d50: 6c64 7329 0372 4600 0000 da02 666e 7247  lds).rF.....fnrG
 00003d60: 0000 0072 3600 0000 7236 0000 0072 3700  ...r6...r6...r7.
-00003d70: 0000 724c 0000 00a3 0200 0073 0600 0000  ..rL.......s....
+00003d70: 0000 724c 0000 00a5 0200 0073 0600 0000  ..rL.......s....
 00003d80: 0600 0601 16ff 7a27 5265 6e64 6572 6572  ......z'Renderer
 00003d90: 2e61 6374 6f72 326a 736f 6e2e 3c6c 6f63  .actor2json.<loc
 00003da0: 616c 733e 2e3c 6469 6374 636f 6d70 3e29  als>.<dictcomp>)
 00003db0: 01da 0c63 686f 6f73 6572 5f64 6963 74da  ...chooser_dict.
 00003dc0: 0c63 6f6e 7465 6e74 7479 7065 73da 056d  .contenttypes..m
 00003dd0: 6f64 656c da05 5f6d 6574 6129 01da 0c63  odel.._meta)...c
 00003de0: 6f6e 7465 6e74 5f74 7970 6529 03da 0d64  ontent_type)...d
 00003df0: 6574 6169 6c5f 6163 7469 6f6e da0d 696e  etail_action..in
 00003e00: 7365 7274 5f61 6374 696f 6eda 0e64 6566  sert_action..def
 00003e10: 6175 6c74 5f61 6374 696f 6e63 0100 0000  ault_actionc....
 00003e20: 0000 0000 0000 0000 0200 0000 0300 0000  ................
 00003e30: 5300 0000 724f 0100 0072 3600 0000 7242  S...rO...r6...rB
 00003e40: 0100 0029 0272 4600 0000 728c 0000 0072  ...).rF...r....r
 00003e50: 3600 0000 7236 0000 0072 3700 0000 7248  6...r6...r7...rH
-00003e60: 0000 00b3 0200 0072 5101 0000 7a27 5265  .......rQ...z'Re
+00003e60: 0000 00b5 0200 0072 5101 0000 7a27 5265  .......rQ...z'Re
 00003e70: 6e64 6572 6572 2e61 6374 6f72 326a 736f  nderer.actor2jso
 00003e80: 6e2e 3c6c 6f63 616c 733e 2e3c 6c69 7374  n.<locals>.<list
 00003e90: 636f 6d70 3e29 02da 0d70 6172 616d 735f  comp>)...params_
 00003ea0: 6c61 796f 7574 da0d 7061 7261 6d73 5f66  layout..params_f
 00003eb0: 6965 6c64 73da 1070 6172 616d 735f 7061  ields..params_pa
 00003ec0: 6e65 6c5f 706f 7329 0172 5e01 0000 2936  nel_pos).r^...)6
 00003ed0: 722b 0000 0072 b400 0000 721b 0000 0072  r+...r....r....r
@@ -1030,15 +1030,15 @@
 00004050: 0000 00da 0261 6cda 0268 6b72 a600 0000  .....al..hkr....
 00004060: da02 6168 da07 636f 6c75 6d6e 73da 0969  ..ah..columns..i
 00004070: 6e64 6578 5f6d 6f64 da09 636f 6c5f 656c  ndex_mod..col_el
 00004080: 656d 7372 4701 0000 720b 0100 00da 0277  emsrG...r......w
 00004090: 6c72 4c01 0000 724d 0100 0072 5401 0000  lrL...rM...rT...
 000040a0: 72b7 0000 0072 8f00 0000 7236 0000 0072  r....r....r6...r
 000040b0: 3600 0000 7237 0000 00da 0a61 6374 6f72  6...r7.....actor
-000040c0: 326a 736f 6e54 0200 0073 8e00 0000 1601  2jsonT...s......
+000040c0: 326a 736f 6e56 0200 0073 8e00 0000 1601  2jsonV...s......
 000040d0: 1001 0601 0201 0601 0801 0c01 06fc 0807  ................
 000040e0: 0c01 0802 0a01 1201 0a03 0401 0401 0801  ................
 000040f0: 0801 0a01 1201 0601 04ff 0201 08ff 1402  ................
 00004100: 1403 0801 0a01 0801 0c01 0801 1205 1001  ................
 00004110: 0c0d 0c01 0a02 1001 0a02 0a01 0801 0e01  ................
 00004120: 0602 1201 0c02 0801 0e01 0c02 0a01 0e02  ................
 00004130: 0e03 0601 0a01 0601 0aff 2603 0201 06ff  ..........&.....
@@ -1056,28 +1056,28 @@
 000041f0: 0153 0029 054e 5463 0100 0000 0000 0000  .S.).NTc........
 00004200: 0000 0000 0100 0000 0600 0000 1300 0000  ................
 00004210: 7318 0000 007c 00a0 0074 0188 01a0 0288  s....|...t......
 00004220: 00a1 0183 01a1 0101 0064 0053 0072 3a00  .........d.S.r:.
 00004230: 0000 2903 728b 0000 0072 2600 0000 7275  ..).r....r&...ru
 00004240: 0100 0072 4301 0000 a902 7298 0000 0072  ...rC.....r....r
 00004250: 3f00 0000 7236 0000 0072 3700 0000 728b  ?...r6...r7...r.
-00004260: 0000 00c2 0200 0073 0200 0000 1801 7a26  .......s......z&
+00004260: 0000 00c4 0200 0073 0200 0000 1801 7a26  .......s......z&
 00004270: 5265 6e64 6572 6572 2e62 7569 6c64 5f6a  Renderer.build_j
 00004280: 735f 6361 6368 652e 3c6c 6f63 616c 733e  s_cache.<locals>
 00004290: 2e77 7269 7465 4629 0e72 6e00 0000 726a  .writeF).rn...rj
 000042a0: 0000 00da 0f67 6574 5f68 616e 646c 655f  .....get_handle_
 000042b0: 6e61 6d65 727d 0000 00da 0470 6174 68da  namer}.....path.
 000042c0: 046a 6f69 6e72 2201 0000 72ef 0000 0072  .joinr"...r....r
 000042d0: 0400 0000 726f 0000 0072 2300 0000 da0f  ....ro...r#.....
 000042e0: 6d61 6b65 5f63 6163 6865 5f66 696c 6572  make_cache_filer
 000042f0: 3b00 0000 da0e 6275 696c 645f 6a73 5f63  ;.....build_js_c
 00004300: 6163 6865 2904 723f 0000 00da 0566 6f72  ache).r?.....for
 00004310: 6365 7253 0100 0072 8b00 0000 7241 0000  cerS...r....rA..
 00004320: 0072 7601 0000 7237 0000 0072 7b01 0000  .rv...r7...r{...
-00004330: b902 0000 7312 0000 0006 020a 020a 0102  ....s...........
+00004330: bb02 0000 7312 0000 0006 020a 020a 0102  ....s...........
 00004340: 0114 010e 0214 0306 020c 017a 1752 656e  ...........z.Ren
 00004350: 6465 7265 722e 6275 696c 645f 6a73 5f63  derer.build_js_c
 00004360: 6163 6865 723a 0000 0029 2072 b300 0000  acher:...) r....
 00004370: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
 00004380: 7175 616c 6e61 6d65 5f5f da07 5f5f 646f  qualname__..__do
 00004390: 635f 5fda 0e69 735f 696e 7465 7261 6374  c__..is_interact
 000043a0: 6976 65da 0863 616e 5f61 7574 6872 1d01  ive..can_authr..
@@ -1091,15 +1091,15 @@
 00004420: 0072 1901 0000 7222 0100 0072 3601 0000  .r....r"...r6...
 00004430: 723d 0100 0072 7501 0000 727b 0100 00da  r=...ru...r{....
 00004440: 0d5f 5f63 6c61 7373 6365 6c6c 5f5f 7236  .__classcell__r6
 00004450: 0000 0072 3600 0000 7241 0000 0072 3700  ...r6...rA...r7.
 00004460: 0000 7239 0000 003a 0000 0073 3c00 0000  ..r9...:...s<...
 00004470: 0800 0401 0403 0401 0402 0401 0401 0c02  ................
 00004480: 0804 0855 081d 0808 081f 0803 0a18 0212  ...U............
-00004490: 0aff 0815 080e 0821 084e 080e 080a 082a  .......!.N.....*
+00004490: 0aff 0815 080e 0821 0851 080e 080a 0829  .......!.Q.....)
 000044a0: 0809 080f 080a 0844 080c 1465 7239 0000  .......D...er9..
 000044b0: 0072 3a00 0000 2946 727d 0000 00da 0770  .r:...)Fr}.....p
 000044c0: 6174 686c 6962 7202 0000 00da 0468 746d  athlibr......htm
 000044d0: 6c72 0300 0000 da0b 646a 616e 676f 2e63  lr......django.c
 000044e0: 6f6e 6672 0400 0000 da09 646a 616e 676f  onfr......django
 000044f0: 2e64 6272 0500 0000 da11 646a 616e 676f  .dbr......django
 00004500: 2e75 7469 6c73 2e74 6578 7472 0600 0000  .utils.textr....
```

### Comparing `lino_react-23.6.0/lino_react/react/__pycache__/views.cpython-310.pyc` & `lino_react-23.6.1/lino_react/react/__pycache__/views.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `lino_react-23.6.0/lino_react/react/config/react/main.html` & `lino_react-23.6.1/lino_react/react/config/react/main.html`

 * *Files 4% similar despite different names*

```diff
@@ -20,28 +20,37 @@
         <div class="splash-double-bounce1"></div>
         <div class="splash-double-bounce2"></div>
       </div>
     </div>
   </div>
 </body>
 
+
+<script>
+    let Lino = {};
+    window.Lino = Lino
+</script>
+
+
 {%- for p in site.sorted_plugins -%}
     {%- if p.get_js_includes -%}
         {%- for name in p.get_js_includes(settings, language) -%}
             {{ javascript(name) }}
         {%- endfor -%}
     {%- endif -%}
 {%- endfor -%}
 
 {%- for p in site.installed_plugins -%}
     {%- for ln in p.get_head_lines(site, request) %}
         {{ ln }}
     {% endfor -%}
 {%- endfor -%}
 
+{{ front_end.load_site_js_snippets(settings) }}
+
 {%- if front_end.url_prefix -%}
 <script type="application/javascript">
     window.url_prefix = "{{ front_end.url_prefix }}/";
 </script>
 {%- endif -%}
 
 <script src="{{site.build_static_url('react/main.js')}}{{no_cache}}"></script>
```

#### html2text {}

```diff
@@ -1,12 +1,13 @@
 {%- macro javascript(url) -%}
  {%- endmacro -%}
 
 
 
 You need to enable JavaScript to run this app.
-{%- for p in site.sorted_plugins -%} {%- if p.get_js_includes -%} {%- for name
+ {%- for p in site.sorted_plugins -%} {%- if p.get_js_includes -%} {%- for name
 in p.get_js_includes(settings, language) -%} {{ javascript(name) }} {%- endfor
 -%} {%- endif -%} {%- endfor -%} {%- for p in site.installed_plugins -%} {%-
 for ln in p.get_head_lines(site, request) %} {{ ln }} {% endfor -%} {%- endfor
--%} {%- if front_end.url_prefix -%}
+-%} {{ front_end.load_site_js_snippets(settings) }} {%- if front_end.url_prefix
+-%}
  {%- endif -%}
```

### Comparing `lino_react-23.6.0/lino_react/react/config/react/service-worker.js` & `lino_react-23.6.1/lino_react/react/config/react/service-worker.js`

 * *Files identical despite different names*

### Comparing `lino_react-23.6.0/lino_react/react/icons.py` & `lino_react-23.6.1/lino_react/react/icons.py`

 * *Files identical despite different names*

### Comparing `lino_react-23.6.0/lino_react/react/renderer.py` & `lino_react-23.6.1/lino_react/react/renderer.py`

 * *Files identical despite different names*

### Comparing `lino_react-23.6.0/lino_react/react/static/media/color.6441e63a.png` & `lino_react-23.6.1/lino_react/react/static/media/color.6441e63a.png`

 * *Files identical despite different names*

### Comparing `lino_react-23.6.0/lino_react/react/static/media/color.c7a33805.png` & `lino_react-23.6.1/lino_react/react/static/media/color.c7a33805.png`

 * *Files identical despite different names*

### Comparing `lino_react-23.6.0/lino_react/react/static/media/line.567f5738.gif` & `lino_react-23.6.1/lino_react/react/static/media/line.567f5738.gif`

 * *Files identical despite different names*

### Comparing `lino_react-23.6.0/lino_react/react/static/media/primeicons.2d2afb27.eot` & `lino_react-23.6.1/lino_react/react/static/media/primeicons.2d2afb27.eot`

 * *Files identical despite different names*

### Comparing `lino_react-23.6.0/lino_react/react/static/media/primeicons.3a0d4a58.ttf` & `lino_react-23.6.1/lino_react/react/static/media/primeicons.3a0d4a58.ttf`

 * *Files identical despite different names*

### Comparing `lino_react-23.6.0/lino_react/react/static/media/primeicons.66ee0deb.woff` & `lino_react-23.6.1/lino_react/react/static/media/primeicons.66ee0deb.woff`

 * *Files identical despite different names*

### Comparing `lino_react-23.6.0/lino_react/react/static/media/primeicons.c55d94a2.svg` & `lino_react-23.6.1/lino_react/react/static/media/primeicons.c55d94a2.svg`

 * *Files identical despite different names*

### Comparing `lino_react-23.6.0/lino_react/react/static/media/primeicons.df0140f8.ttf` & `lino_react-23.6.1/lino_react/react/static/media/primeicons.df0140f8.ttf`

 * *Files identical despite different names*

### Comparing `lino_react-23.6.0/lino_react/react/static/media/primeicons.dfbfef2d.eot` & `lino_react-23.6.1/lino_react/react/static/media/primeicons.dfbfef2d.eot`

 * *Files identical despite different names*

### Comparing `lino_react-23.6.0/lino_react/react/static/media/primeicons.e5e0e944.svg` & `lino_react-23.6.1/lino_react/react/static/media/primeicons.e5e0e944.svg`

 * *Files identical despite different names*

### Comparing `lino_react-23.6.0/lino_react/react/static/media/primeicons.e61f3495.woff` & `lino_react-23.6.1/lino_react/react/static/media/primeicons.e61f3495.woff`

 * *Files identical despite different names*

### Comparing `lino_react-23.6.0/lino_react/react/static/react/main.js` & `lino_react-23.6.1/lino_react/react/static/react/main.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -201,32 +201,32 @@
                     _App_css__WEBPACK_IMPORTED_MODULE_30__ = __webpack_require__(9638),
                     react_router_dom__WEBPACK_IMPORTED_MODULE_35__ = __webpack_require__(9394),
                     react_router_dom__WEBPACK_IMPORTED_MODULE_36__ = __webpack_require__(1399),
                     whatwg_fetch__WEBPACK_IMPORTED_MODULE_31__ = __webpack_require__(8404),
                     reconnecting_websocket__WEBPACK_IMPORTED_MODULE_32__ = __webpack_require__(7956),
                     _SiteContext__WEBPACK_IMPORTED_MODULE_33__ = __webpack_require__(7239);
 
-                function _typeof(e) {
-                    return _typeof = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
-                        return typeof e
-                    } : function(e) {
-                        return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
-                    }, _typeof(e)
-                }
-
                 function _extends() {
                     return _extends = Object.assign || function(e) {
                         for (var t = 1; t < arguments.length; t++) {
                             var n = arguments[t];
                             for (var o in n) Object.prototype.hasOwnProperty.call(n, o) && (e[o] = n[o])
                         }
                         return e
                     }, _extends.apply(this, arguments)
                 }
 
+                function _typeof(e) {
+                    return _typeof = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
+                        return typeof e
+                    } : function(e) {
+                        return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
+                    }, _typeof(e)
+                }
+
                 function ownKeys(e, t) {
                     var n = Object.keys(e);
                     if (Object.getOwnPropertySymbols) {
                         var o = Object.getOwnPropertySymbols(e);
                         t && (o = o.filter((function(t) {
                             return Object.getOwnPropertyDescriptor(e, t).enumerable
                         }))), n.push.apply(n, o)
@@ -327,20 +327,20 @@
                 }
 
                 function _getPrototypeOf(e) {
                     return _getPrototypeOf = Object.setPrototypeOf ? Object.getPrototypeOf : function(e) {
                         return e.__proto__ || Object.getPrototypeOf(e)
                     }, _getPrototypeOf(e)
                 }
-                var Lino = {
-                        get_current_grid_config: function(e, t) {
-                            return e.get_current_grid_config(t)
-                        }
-                    },
-                    App = function(_React$Component) {
+                if (void 0 === window.Lino) var _Lino = {};
+                else Lino = window.Lino;
+                Lino.get_current_grid_config = function(e, t) {
+                    return e.get_current_grid_config(t)
+                };
+                var App = function(_React$Component) {
                         _inherits(App, _React$Component);
                         var _super = _createSuper(App);
 
                         function App() {
                             var _this;
                             return _classCallCheck(this, App), _this = _super.call(this), _this.fetch_user_settings = function(e, t, n) {
                                 t || _this.setState({
@@ -587,15 +587,18 @@
                                         var r = rp_obj.data.data[t];
                                         return [null, void 0].includes(r) && (r = ""), r.toJSON && (r = r.toJSON()), e[t] = r, e
                                     }), {});
                                     Object.assign(args, changes)
                                 }
                                 if ("submit_insert" === an && Object.assign(args, rp_obj.props.data), data && Object.assign(args, data), "GET" === action.http_method && (args.fmt = "json"), action.preprocessor) {
                                     var func = eval(action.preprocessor);
-                                    func && func(rp_obj, args)
+                                    if (func) {
+                                        var res = func(rp_obj, args);
+                                        "object" != _typeof(res) || res.hasOwnProperty("length") || Object.assign(args, res)
+                                    }
                                 }
                                 if ("submit_insert" === an && rp_obj.state.FileUploadRequest) {
                                     var _rp_obj$state$FileUpl = rp_obj.state.FileUploadRequest,
                                         xhr = _rp_obj$state$FileUpl.xhr,
                                         formData = _rp_obj$state$FileUpl.formData;
                                     return Object.keys(args).forEach((function(e) {
                                         return null != args[e] && formData.append(e, args[e])
```

### Comparing `lino_react-23.6.0/lino_react/react/static/react/main.js.LICENSE.txt` & `lino_react-23.6.1/lino_react/react/static/react/main.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lino_react-23.6.0/lino_react/react/views.py` & `lino_react-23.6.1/lino_react/react/views.py`

 * *Files identical despite different names*

### Comparing `lino_react-23.6.0/lino_react/setup_info.py` & `lino_react-23.6.1/lino_react/setup_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: UTF-8 -*-
 # Copyright 2015-2023 Rumma & Ko Ltd
 # License: GNU Affero General Public License v3 (see file COPYING for details)
 
 SETUP_INFO = dict(
     name='lino_react',
-    version='23.6.0',
+    version='23.6.1',
     install_requires=['lino'],
     tests_require=[],
     test_suite='tests',
     description="The React front end for Lino",
     license_files=['COPYING'],
     include_package_data=False,
     zip_safe=False,
```

### Comparing `lino_react-23.6.0/lino_react.egg-info/PKG-INFO` & `lino_react-23.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: lino-react
-Version: 23.6.0
+Name: lino_react
+Version: 23.6.1
 Summary: The React front end for Lino
 Home-page: https://gitlab.com/lino-framework/react
 Author: Rumma & Ko Ltd
 Author-email: info@lino-framework.org
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier:   Programming Language :: Python
```

### Comparing `lino_react-23.6.0/lino_react.egg-info/SOURCES.txt` & `lino_react-23.6.1/lino_react.egg-info/SOURCES.txt`

 * *Files identical despite different names*

