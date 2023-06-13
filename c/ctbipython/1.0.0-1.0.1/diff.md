# Comparing `tmp/ctbipython-1.0.0.tar.gz` & `tmp/ctbipython-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctbipython-1.0.0.tar", last modified: Tue Jun 13 12:30:48 2023, max compression
+gzip compressed data, was "ctbipython-1.0.1.tar", last modified: Tue Jun 13 14:21:58 2023, max compression
```

## Comparing `ctbipython-1.0.0.tar` & `ctbipython-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 12:30:48.794022 ctbipython-1.0.0/
--rw-rw-rw-   0        0        0      197 2023-06-13 12:30:48.793025 ctbipython-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1355 2023-05-24 14:03:51.000000 ctbipython-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-13 12:30:48.742162 ctbipython-1.0.0/ctbipython/
--rw-rw-rw-   0        0        0        0 2023-05-24 12:22:47.000000 ctbipython-1.0.0/ctbipython/__init__.py
--rw-rw-rw-   0        0        0    78791 2023-05-31 21:59:28.000000 ctbipython-1.0.0/ctbipython/ctbi.py
--rw-rw-rw-   0        0        0     3989 2023-05-31 21:59:32.000000 ctbipython-1.0.0/ctbipython/example.py
-drwxrwxrwx   0        0        0        0 2023-06-13 12:30:48.791030 ctbipython-1.0.0/ctbipython.egg-info/
--rw-rw-rw-   0        0        0      197 2023-06-13 12:30:47.000000 ctbipython-1.0.0/ctbipython.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      251 2023-06-13 12:30:48.000000 ctbipython-1.0.0/ctbipython.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 12:30:47.000000 ctbipython-1.0.0/ctbipython.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-06-13 12:30:47.000000 ctbipython-1.0.0/ctbipython.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-13 12:30:47.000000 ctbipython-1.0.0/ctbipython.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-13 12:30:48.795019 ctbipython-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      348 2023-06-13 12:30:23.000000 ctbipython-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 14:21:58.065994 ctbipython-1.0.1/
+-rw-rw-rw-   0        0        0      197 2023-06-13 14:21:58.065994 ctbipython-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1355 2023-05-24 14:03:51.000000 ctbipython-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-13 14:21:58.040833 ctbipython-1.0.1/ctbipython/
+-rw-rw-rw-   0        0        0        0 2023-05-24 12:22:47.000000 ctbipython-1.0.1/ctbipython/__init__.py
+-rw-rw-rw-   0        0        0    78791 2023-05-31 21:59:28.000000 ctbipython-1.0.1/ctbipython/ctbi.py
+-rw-rw-rw-   0        0        0     3950 2023-06-13 13:13:47.000000 ctbipython-1.0.1/ctbipython/example.py
+drwxrwxrwx   0        0        0        0 2023-06-13 14:21:58.064994 ctbipython-1.0.1/ctbipython.egg-info/
+-rw-rw-rw-   0        0        0      197 2023-06-13 14:21:57.000000 ctbipython-1.0.1/ctbipython.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2023-06-13 14:21:57.000000 ctbipython-1.0.1/ctbipython.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 14:21:57.000000 ctbipython-1.0.1/ctbipython.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-06-13 14:21:57.000000 ctbipython-1.0.1/ctbipython.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-13 14:21:57.000000 ctbipython-1.0.1/ctbipython.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-13 14:21:58.066991 ctbipython-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      348 2023-06-13 13:14:03.000000 ctbipython-1.0.1/setup.py
```

### Comparing `ctbipython-1.0.0/README.md` & `ctbipython-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `ctbipython-1.0.0/ctbipython/ctbi.py` & `ctbipython-1.0.1/ctbipython/ctbi.py`

 * *Files identical despite different names*

### Comparing `ctbipython-1.0.0/ctbipython/example.py` & `ctbipython-1.0.1/ctbipython/example.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#pip install -i https://test.pypi.org/simple/ ctbipython==1.25
+#pip install ctbipython
 import ctbipython.ctbi as ctbi
 
 import pandas as pd
 import numpy as np
 
 # Example 1 : X is numeric
```

