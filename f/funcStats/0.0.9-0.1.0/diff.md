# Comparing `tmp/funcStats-0.0.9.tar.gz` & `tmp/funcStats-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funcStats-0.0.9.tar", last modified: Sun Jun 11 05:50:28 2023, max compression
+gzip compressed data, was "funcStats-0.1.0.tar", last modified: Tue Jun 13 01:52:05 2023, max compression
```

## Comparing `funcStats-0.0.9.tar` & `funcStats-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-11 05:50:28.543279 funcStats-0.0.9/
--rw-r--r--   0 tom        (501) staff       (20)     7048 2023-06-10 01:28:38.000000 funcStats-0.0.9/LICENSE
--rw-r--r--   0 tom        (501) staff       (20)     6951 2023-06-11 05:50:28.542869 funcStats-0.0.9/PKG-INFO
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-11 05:50:28.538689 funcStats-0.0.9/funcStats/
--rw-r--r--   0 tom        (501) staff       (20)     4196 2023-06-11 05:47:21.000000 funcStats-0.0.9/funcStats/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     1204 2023-06-11 02:10:01.000000 funcStats-0.0.9/funcStats/log.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-11 05:50:28.542286 funcStats-0.0.9/funcStats.egg-info/
--rw-r--r--   0 tom        (501) staff       (20)     6951 2023-06-11 05:50:28.000000 funcStats-0.0.9/funcStats.egg-info/PKG-INFO
--rw-r--r--   0 tom        (501) staff       (20)      219 2023-06-11 05:50:28.000000 funcStats-0.0.9/funcStats.egg-info/SOURCES.txt
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-06-11 05:50:28.000000 funcStats-0.0.9/funcStats.egg-info/dependency_links.txt
--rw-r--r--   0 tom        (501) staff       (20)        9 2023-06-11 05:50:28.000000 funcStats-0.0.9/funcStats.egg-info/requires.txt
--rw-r--r--   0 tom        (501) staff       (20)       10 2023-06-11 05:50:28.000000 funcStats-0.0.9/funcStats.egg-info/top_level.txt
--rw-r--r--   0 tom        (501) staff       (20)       38 2023-06-11 05:50:28.543396 funcStats-0.0.9/setup.cfg
--rw-r--r--   0 tom        (501) staff       (20)     1018 2023-06-11 05:49:53.000000 funcStats-0.0.9/setup.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-13 01:52:05.370698 funcStats-0.1.0/
+-rw-r--r--   0 tom        (501) staff       (20)     7048 2023-06-13 01:44:59.000000 funcStats-0.1.0/LICENSE
+-rw-r--r--   0 tom        (501) staff       (20)     6951 2023-06-13 01:52:05.370321 funcStats-0.1.0/PKG-INFO
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-13 01:52:05.366378 funcStats-0.1.0/config/
+-rw-r--r--   0 tom        (501) staff       (20)     6367 2023-06-13 01:50:30.000000 funcStats-0.1.0/config/__init__.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-13 01:52:05.367457 funcStats-0.1.0/funcStats/
+-rw-r--r--   0 tom        (501) staff       (20)     4196 2023-06-13 01:44:59.000000 funcStats-0.1.0/funcStats/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     1204 2023-06-13 01:44:59.000000 funcStats-0.1.0/funcStats/log.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-13 01:52:05.369763 funcStats-0.1.0/funcStats.egg-info/
+-rw-r--r--   0 tom        (501) staff       (20)     6951 2023-06-13 01:52:05.000000 funcStats-0.1.0/funcStats.egg-info/PKG-INFO
+-rw-r--r--   0 tom        (501) staff       (20)      238 2023-06-13 01:52:05.000000 funcStats-0.1.0/funcStats.egg-info/SOURCES.txt
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-06-13 01:52:05.000000 funcStats-0.1.0/funcStats.egg-info/dependency_links.txt
+-rw-r--r--   0 tom        (501) staff       (20)        9 2023-06-13 01:52:05.000000 funcStats-0.1.0/funcStats.egg-info/requires.txt
+-rw-r--r--   0 tom        (501) staff       (20)       17 2023-06-13 01:52:05.000000 funcStats-0.1.0/funcStats.egg-info/top_level.txt
+-rw-r--r--   0 tom        (501) staff       (20)       38 2023-06-13 01:52:05.370829 funcStats-0.1.0/setup.cfg
+-rw-r--r--   0 tom        (501) staff       (20)      968 2023-06-13 01:51:53.000000 funcStats-0.1.0/setup.py
```

### Comparing `funcStats-0.0.9/LICENSE` & `funcStats-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `funcStats-0.0.9/PKG-INFO` & `funcStats-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funcStats
-Version: 0.0.9
+Version: 0.1.0
 Summary: A module that helps to evaluate functions when some tests are needed
 Author: Elemental (Tom Neto)
 Author-email: <info@elemental.run>
 Keywords: python,functions,cronometer,crono,meter,evaluate functions
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `funcStats-0.0.9/funcStats/__init__.py` & `funcStats-0.1.0/funcStats/__init__.py`

 * *Files identical despite different names*

### Comparing `funcStats-0.0.9/funcStats/log.py` & `funcStats-0.1.0/funcStats/log.py`

 * *Files identical despite different names*

### Comparing `funcStats-0.0.9/funcStats.egg-info/PKG-INFO` & `funcStats-0.1.0/funcStats.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funcStats
-Version: 0.0.9
+Version: 0.1.0
 Summary: A module that helps to evaluate functions when some tests are needed
 Author: Elemental (Tom Neto)
 Author-email: <info@elemental.run>
 Keywords: python,functions,cronometer,crono,meter,evaluate functions
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `funcStats-0.0.9/setup.py` & `funcStats-0.1.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import os.path
 
 from setuptools import setup, find_packages
 from pathlib import Path
+from config import LONG_DESCRIPTION
 this_directory = Path(__file__).parent
 
-VERSION = '0.0.9'
+VERSION = '0.1.0'
 DESCRIPTION = 'A module that helps to evaluate functions when some tests are needed'
-LONG_DESCRIPTION = str(open('/Volumes/Projetos/Git/funcStats/README.MD', 'r').read())
 
 setup(
     name="funcStats",
     version=VERSION,
     author="Elemental (Tom Neto)",
     author_email="<info@elemental.run>",
     description=DESCRIPTION,
```

