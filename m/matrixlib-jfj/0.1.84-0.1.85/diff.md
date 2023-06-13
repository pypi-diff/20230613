# Comparing `tmp/matrixlib_jfj-0.1.84.tar.gz` & `tmp/matrixlib_jfj-0.1.85.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matrixlib_jfj-0.1.84.tar", last modified: Wed Jun  7 20:20:58 2023, max compression
+gzip compressed data, was "matrixlib_jfj-0.1.85.tar", last modified: Wed Jun  7 20:44:20 2023, max compression
```

## Comparing `matrixlib_jfj-0.1.84.tar` & `matrixlib_jfj-0.1.85.tar`

### file list

```diff
@@ -1,19 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 20:20:58.820527 matrixlib_jfj-0.1.84/
--rw-rw-rw-   0        0        0    35148 2023-06-07 14:44:29.000000 matrixlib_jfj-0.1.84/LICENSE.md
--rw-rw-rw-   0        0        0     3391 2023-06-07 20:20:58.822519 matrixlib_jfj-0.1.84/PKG-INFO
--rw-rw-rw-   0        0        0     2504 2023-06-07 20:02:38.000000 matrixlib_jfj-0.1.84/README.md
--rw-rw-rw-   0        0        0     1014 2023-06-07 14:44:29.000000 matrixlib_jfj-0.1.84/pyproject.toml
--rw-rw-rw-   0        0        0     1003 2023-06-07 20:20:58.828503 matrixlib_jfj-0.1.84/setup.cfg
--rw-rw-rw-   0        0        0       65 2023-06-07 14:44:29.000000 matrixlib_jfj-0.1.84/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-07 20:20:58.636941 matrixlib_jfj-0.1.84/src/
-drwxrwxrwx   0        0        0        0 2023-06-07 20:20:58.756703 matrixlib_jfj-0.1.84/src/matrixlib_jfj/
--rw-rw-rw-   0        0        0      962 2023-06-07 20:20:50.000000 matrixlib_jfj-0.1.84/src/matrixlib_jfj/__init__.py
--rw-rw-rw-   0        0        0    14804 2023-06-07 20:19:47.000000 matrixlib_jfj-0.1.84/src/matrixlib_jfj/matrix.py
--rw-rw-rw-   0        0        0       35 2023-06-07 19:57:42.000000 matrixlib_jfj-0.1.84/src/matrixlib_jfj/utils.py
--rw-rw-rw-   0        0        0      213 2023-06-07 14:44:28.000000 matrixlib_jfj-0.1.84/src/matrixlib_jfj/vector.py
-drwxrwxrwx   0        0        0        0 2023-06-07 20:20:58.811558 matrixlib_jfj-0.1.84/src/matrixlib_jfj.egg-info/
--rw-rw-rw-   0        0        0     3391 2023-06-07 20:20:58.000000 matrixlib_jfj-0.1.84/src/matrixlib_jfj.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      371 2023-06-07 20:20:58.000000 matrixlib_jfj-0.1.84/src/matrixlib_jfj.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 20:20:58.000000 matrixlib_jfj-0.1.84/src/matrixlib_jfj.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-06-07 20:20:58.000000 matrixlib_jfj-0.1.84/src/matrixlib_jfj.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-07 20:20:58.000000 matrixlib_jfj-0.1.84/src/matrixlib_jfj.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-07 20:44:20.401119 matrixlib_jfj-0.1.85/
+-rw-rw-rw-   0        0        0     3077 2023-06-07 14:44:29.000000 matrixlib_jfj-0.1.85/.gitignore
+-rw-rw-rw-   0        0        0    35148 2023-06-07 14:44:29.000000 matrixlib_jfj-0.1.85/LICENSE.md
+-rw-rw-rw-   0        0        0     3391 2023-06-07 20:44:20.401119 matrixlib_jfj-0.1.85/PKG-INFO
+-rw-rw-rw-   0        0        0     2504 2023-06-07 20:02:38.000000 matrixlib_jfj-0.1.85/README.md
+-rw-rw-rw-   0        0        0       98 2023-06-07 14:44:29.000000 matrixlib_jfj-0.1.85/build.py
+-rw-rw-rw-   0        0        0     1014 2023-06-07 14:44:29.000000 matrixlib_jfj-0.1.85/pyproject.toml
+-rw-rw-rw-   0        0        0       31 2023-06-07 14:44:29.000000 matrixlib_jfj-0.1.85/requirements.txt
+-rw-rw-rw-   0        0        0     1003 2023-06-07 20:44:20.409104 matrixlib_jfj-0.1.85/setup.cfg
+-rw-rw-rw-   0        0        0       65 2023-06-07 14:44:29.000000 matrixlib_jfj-0.1.85/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 20:44:20.273295 matrixlib_jfj-0.1.85/src/
+drwxrwxrwx   0        0        0        0 2023-06-07 20:44:20.362373 matrixlib_jfj-0.1.85/src/matrixlib_jfj/
+-rw-rw-rw-   0        0        0      962 2023-06-07 20:44:16.000000 matrixlib_jfj-0.1.85/src/matrixlib_jfj/__init__.py
+-rw-rw-rw-   0        0        0    14804 2023-06-07 20:19:47.000000 matrixlib_jfj-0.1.85/src/matrixlib_jfj/matrix.py
+-rw-rw-rw-   0        0        0       35 2023-06-07 19:57:42.000000 matrixlib_jfj-0.1.85/src/matrixlib_jfj/utils.py
+-rw-rw-rw-   0        0        0      213 2023-06-07 14:44:28.000000 matrixlib_jfj-0.1.85/src/matrixlib_jfj/vector.py
+drwxrwxrwx   0        0        0        0 2023-06-07 20:44:20.398123 matrixlib_jfj-0.1.85/src/matrixlib_jfj.egg-info/
+-rw-rw-rw-   0        0        0     3391 2023-06-07 20:44:19.000000 matrixlib_jfj-0.1.85/src/matrixlib_jfj.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      408 2023-06-07 20:44:20.000000 matrixlib_jfj-0.1.85/src/matrixlib_jfj.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 20:44:19.000000 matrixlib_jfj-0.1.85/src/matrixlib_jfj.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-06-07 20:44:19.000000 matrixlib_jfj-0.1.85/src/matrixlib_jfj.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-07 20:44:19.000000 matrixlib_jfj-0.1.85/src/matrixlib_jfj.egg-info/top_level.txt
```

### Comparing `matrixlib_jfj-0.1.84/LICENSE.md` & `matrixlib_jfj-0.1.85/LICENSE.md`

 * *Files identical despite different names*

### Comparing `matrixlib_jfj-0.1.84/PKG-INFO` & `matrixlib_jfj-0.1.85/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matrixlib_jfj
-Version: 0.1.84
+Version: 0.1.85
 Summary: A library that deals with matrix and vector operations.
 Author: Jemma Starecki
 Author-email: Jemma Starecki <starecki.j@shaw.ca>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: homepage, https://github.com/JemmaFromJupiter/Matrixlib
 Project-URL: Issue Tracker, https://github.com/JemmaFromJupiter/Matrixlib/issues
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `matrixlib_jfj-0.1.84/README.md` & `matrixlib_jfj-0.1.85/README.md`

 * *Files identical despite different names*

### Comparing `matrixlib_jfj-0.1.84/pyproject.toml` & `matrixlib_jfj-0.1.85/pyproject.toml`

 * *Files identical despite different names*

### Comparing `matrixlib_jfj-0.1.84/setup.cfg` & `matrixlib_jfj-0.1.85/setup.cfg`

 * *Files identical despite different names*

### Comparing `matrixlib_jfj-0.1.84/src/matrixlib_jfj/__init__.py` & `matrixlib_jfj-0.1.85/src/matrixlib_jfj/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,26 +27,26 @@
 
  	print(transposed) # Output:
 
  	0 0 0\n
 	0 0 0\n
  	6 0 0
 
-Version: 0.1.84
+Version: 0.1.85
 
 Author: Jemma Starecki
 
 Made By <a href="https://github.com/JemmaFromJupiter" target="_blank">JemmaFromJupiter</a> On Github.
 """
 from __future__ import annotations
 from . import matrix
 from . import vector
 from . import utils
 
-__version__ = "0.1.84"
+__version__ = "0.1.85"
 __author__ = "JemmaFromJupiter"
 
 __all__ = [
 	"matrix",
 	"vector",
 	"utils"
 ]
```

### Comparing `matrixlib_jfj-0.1.84/src/matrixlib_jfj/matrix.py` & `matrixlib_jfj-0.1.85/src/matrixlib_jfj/matrix.py`

 * *Files identical despite different names*

### Comparing `matrixlib_jfj-0.1.84/src/matrixlib_jfj.egg-info/PKG-INFO` & `matrixlib_jfj-0.1.85/src/matrixlib_jfj.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matrixlib-jfj
-Version: 0.1.84
+Version: 0.1.85
 Summary: A library that deals with matrix and vector operations.
 Author: Jemma Starecki
 Author-email: Jemma Starecki <starecki.j@shaw.ca>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: homepage, https://github.com/JemmaFromJupiter/Matrixlib
 Project-URL: Issue Tracker, https://github.com/JemmaFromJupiter/Matrixlib/issues
 Classifier: Development Status :: 3 - Alpha
```

