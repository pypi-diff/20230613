# Comparing `tmp/funcStats-0.1.1.tar.gz` & `tmp/funcStats-0.1.10.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funcStats-0.1.1.tar", last modified: Tue Jun 13 02:03:36 2023, max compression
+gzip compressed data, was "funcStats-0.1.10.tar", last modified: Tue Jun 13 02:26:41 2023, max compression
```

## Comparing `funcStats-0.1.1.tar` & `funcStats-0.1.10.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-13 02:03:36.965004 funcStats-0.1.1/
--rw-r--r--   0 tom        (501) staff       (20)     7048 2023-06-13 01:44:59.000000 funcStats-0.1.1/LICENSE
--rw-r--r--   0 tom        (501) staff       (20)     6951 2023-06-13 02:03:36.964219 funcStats-0.1.1/PKG-INFO
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-13 02:03:36.955305 funcStats-0.1.1/config/
--rw-r--r--   0 tom        (501) staff       (20)     6367 2023-06-13 01:50:30.000000 funcStats-0.1.1/config/__init__.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-13 02:03:36.957522 funcStats-0.1.1/funcStats/
--rw-r--r--   0 tom        (501) staff       (20)     3884 2023-06-13 02:02:45.000000 funcStats-0.1.1/funcStats/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     1204 2023-06-13 01:44:59.000000 funcStats-0.1.1/funcStats/log.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-13 02:03:36.963034 funcStats-0.1.1/funcStats.egg-info/
--rw-r--r--   0 tom        (501) staff       (20)     6951 2023-06-13 02:03:36.000000 funcStats-0.1.1/funcStats.egg-info/PKG-INFO
--rw-r--r--   0 tom        (501) staff       (20)      238 2023-06-13 02:03:36.000000 funcStats-0.1.1/funcStats.egg-info/SOURCES.txt
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-06-13 02:03:36.000000 funcStats-0.1.1/funcStats.egg-info/dependency_links.txt
--rw-r--r--   0 tom        (501) staff       (20)        9 2023-06-13 02:03:36.000000 funcStats-0.1.1/funcStats.egg-info/requires.txt
--rw-r--r--   0 tom        (501) staff       (20)       17 2023-06-13 02:03:36.000000 funcStats-0.1.1/funcStats.egg-info/top_level.txt
--rw-r--r--   0 tom        (501) staff       (20)       38 2023-06-13 02:03:36.965253 funcStats-0.1.1/setup.cfg
--rw-r--r--   0 tom        (501) staff       (20)      968 2023-06-13 02:03:18.000000 funcStats-0.1.1/setup.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-13 02:26:41.893768 funcStats-0.1.10/
+-rw-r--r--   0 tom        (501) staff       (20)     7048 2023-06-13 01:44:59.000000 funcStats-0.1.10/LICENSE
+-rw-r--r--   0 tom        (501) staff       (20)     6952 2023-06-13 02:26:41.893316 funcStats-0.1.10/PKG-INFO
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-13 02:26:41.886222 funcStats-0.1.10/config/
+-rw-r--r--   0 tom        (501) staff       (20)     6367 2023-06-13 01:50:30.000000 funcStats-0.1.10/config/__init__.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-13 02:26:41.887902 funcStats-0.1.10/funcStats/
+-rw-r--r--   0 tom        (501) staff       (20)     3884 2023-06-13 02:25:52.000000 funcStats-0.1.10/funcStats/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     1204 2023-06-13 01:44:59.000000 funcStats-0.1.10/funcStats/log.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-13 02:26:41.892663 funcStats-0.1.10/funcStats.egg-info/
+-rw-r--r--   0 tom        (501) staff       (20)     6952 2023-06-13 02:26:41.000000 funcStats-0.1.10/funcStats.egg-info/PKG-INFO
+-rw-r--r--   0 tom        (501) staff       (20)      238 2023-06-13 02:26:41.000000 funcStats-0.1.10/funcStats.egg-info/SOURCES.txt
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-06-13 02:26:41.000000 funcStats-0.1.10/funcStats.egg-info/dependency_links.txt
+-rw-r--r--   0 tom        (501) staff       (20)        9 2023-06-13 02:26:41.000000 funcStats-0.1.10/funcStats.egg-info/requires.txt
+-rw-r--r--   0 tom        (501) staff       (20)       17 2023-06-13 02:26:41.000000 funcStats-0.1.10/funcStats.egg-info/top_level.txt
+-rw-r--r--   0 tom        (501) staff       (20)       38 2023-06-13 02:26:41.893906 funcStats-0.1.10/setup.cfg
+-rw-r--r--   0 tom        (501) staff       (20)      969 2023-06-13 02:26:30.000000 funcStats-0.1.10/setup.py
```

### Comparing `funcStats-0.1.1/LICENSE` & `funcStats-0.1.10/LICENSE`

 * *Files identical despite different names*

### Comparing `funcStats-0.1.1/PKG-INFO` & `funcStats-0.1.10/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funcStats
-Version: 0.1.1
+Version: 0.1.10
 Summary: A module that helps to evaluate functions when some tests are needed
 Author: Elemental (Tom Neto)
 Author-email: <info@elemental.run>
 Keywords: python,functions,cronometer,crono,meter,evaluate functions
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `funcStats-0.1.1/config/__init__.py` & `funcStats-0.1.10/config/__init__.py`

 * *Files identical despite different names*

### Comparing `funcStats-0.1.1/funcStats/__init__.py` & `funcStats-0.1.10/funcStats/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,20 +98,20 @@
 
             self.logStream.skipLine()
             self.logStream.add(f'Meter Execution Count: {self.count}')
             self.logStream.add(f"Meter Execution Starts at: {startTime}")
             self.logStream.add(f"Meter Execution Args: {argPack}")
 
             try:
-                if not isinstance(argPack, str):
+                if argPack is None:
+                    executionResult = str(self.func())
+                elif not isinstance(argPack, str):
                     executionResult = str(self.func(*argPack))
                 elif isinstance(argPack, str):
                     executionResult = str(self.func(argPack))
-                elif argPack is None:
-                    executionResult = str(self.func())
             except Exception as e:
                 executionResult = e
 
             self.logStream.add(f"Meter Execution Returns: {str(executionResult)}...")
 
             endTime = datetime.now()
```

### Comparing `funcStats-0.1.1/funcStats/log.py` & `funcStats-0.1.10/funcStats/log.py`

 * *Files identical despite different names*

### Comparing `funcStats-0.1.1/funcStats.egg-info/PKG-INFO` & `funcStats-0.1.10/funcStats.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funcStats
-Version: 0.1.1
+Version: 0.1.10
 Summary: A module that helps to evaluate functions when some tests are needed
 Author: Elemental (Tom Neto)
 Author-email: <info@elemental.run>
 Keywords: python,functions,cronometer,crono,meter,evaluate functions
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `funcStats-0.1.1/setup.py` & `funcStats-0.1.10/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os.path
 
 from setuptools import setup, find_packages
 from pathlib import Path
 from config import LONG_DESCRIPTION
 this_directory = Path(__file__).parent
 
-VERSION = '0.1.1'
+VERSION = '0.1.10'
 DESCRIPTION = 'A module that helps to evaluate functions when some tests are needed'
 
 setup(
     name="funcStats",
     version=VERSION,
     author="Elemental (Tom Neto)",
     author_email="<info@elemental.run>",
```

