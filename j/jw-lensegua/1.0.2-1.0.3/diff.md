# Comparing `tmp/jw_lensegua-1.0.2.tar.gz` & `tmp/jw_lensegua-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jw_lensegua-1.0.2.tar", last modified: Mon Jun 12 22:41:01 2023, max compression
+gzip compressed data, was "jw_lensegua-1.0.3.tar", last modified: Tue Jun 13 17:05:58 2023, max compression
```

## Comparing `jw_lensegua-1.0.2.tar` & `jw_lensegua-1.0.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 22:41:01.105694 jw_lensegua-1.0.2/
--rw-rw-rw-   0        0        0    35821 2023-02-07 04:10:38.000000 jw_lensegua-1.0.2/LICENSE
--rw-rw-rw-   0        0        0      666 2023-06-12 22:41:01.104696 jw_lensegua-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-02-07 03:54:35.000000 jw_lensegua-1.0.2/README.md
--rw-rw-rw-   0        0        0      873 2023-06-12 22:40:37.000000 jw_lensegua-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-12 22:41:01.105694 jw_lensegua-1.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-12 22:41:01.083733 jw_lensegua-1.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-06-12 22:41:01.088606 jw_lensegua-1.0.2/src/jw_lensegua/
--rw-rw-rw-   0        0        0        0 2023-02-09 02:37:15.000000 jw_lensegua-1.0.2/src/jw_lensegua/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 22:41:01.095607 jw_lensegua-1.0.2/src/jw_lensegua/tests/
--rw-rw-rw-   0        0        0        0 2023-02-09 02:39:41.000000 jw_lensegua-1.0.2/src/jw_lensegua/tests/__init__.py
--rw-rw-rw-   0        0        0    35757 2023-02-19 22:20:19.000000 jw_lensegua-1.0.2/src/jw_lensegua/tests/test_solution.py
-drwxrwxrwx   0        0        0        0 2023-06-12 22:41:01.098693 jw_lensegua-1.0.2/src/jw_lensegua/v1/
--rw-rw-rw-   0        0        0    35703 2023-02-20 03:14:00.000000 jw_lensegua-1.0.2/src/jw_lensegua/v1/cam.py
--rw-rw-rw-   0        0        0    20132 2023-02-20 03:03:23.000000 jw_lensegua-1.0.2/src/jw_lensegua/v1/lensegua.py
--rw-rw-rw-   0        0        0      793 2023-02-12 03:28:51.000000 jw_lensegua-1.0.2/src/jw_lensegua/v1/results_model.py
--rw-rw-rw-   0        0        0    67243 2023-03-23 04:59:36.000000 jw_lensegua-1.0.2/src/jw_lensegua/v1/solutions.py
-drwxrwxrwx   0        0        0        0 2023-06-12 22:41:01.102694 jw_lensegua-1.0.2/src/jw_lensegua/v2/
--rw-rw-rw-   0        0        0   108820 2023-06-12 18:13:47.000000 jw_lensegua-1.0.2/src/jw_lensegua/v2/model_class_tf.py
--rw-rw-rw-   0        0        0     1664 2023-06-09 18:32:08.000000 jw_lensegua-1.0.2/src/jw_lensegua/v2/model_kmean_tf2.py
--rw-rw-rw-   0        0        0     4129 2023-03-19 22:48:16.000000 jw_lensegua-1.0.2/src/jw_lensegua/v2/model_transfer.py
--rw-rw-rw-   0        0        0     7627 2023-06-09 21:04:34.000000 jw_lensegua-1.0.2/src/jw_lensegua/v2/sign_language.py
-drwxrwxrwx   0        0        0        0 2023-06-12 22:41:01.093609 jw_lensegua-1.0.2/src/jw_lensegua.egg-info/
--rw-rw-rw-   0        0        0      666 2023-06-12 22:41:01.000000 jw_lensegua-1.0.2/src/jw_lensegua.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      562 2023-06-12 22:41:01.000000 jw_lensegua-1.0.2/src/jw_lensegua.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 22:41:01.000000 jw_lensegua-1.0.2/src/jw_lensegua.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-06-12 22:41:01.000000 jw_lensegua-1.0.2/src/jw_lensegua.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-13 17:05:58.023457 jw_lensegua-1.0.3/
+-rw-rw-rw-   0        0        0    35821 2023-02-07 04:10:38.000000 jw_lensegua-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0      983 2023-06-13 17:05:58.022453 jw_lensegua-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      313 2023-06-13 17:05:26.000000 jw_lensegua-1.0.3/README.md
+-rw-rw-rw-   0        0        0      873 2023-06-13 17:01:10.000000 jw_lensegua-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-13 17:05:58.023457 jw_lensegua-1.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-13 17:05:58.003572 jw_lensegua-1.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-06-13 17:05:58.009431 jw_lensegua-1.0.3/src/jw_lensegua/
+-rw-rw-rw-   0        0        0        0 2023-02-09 02:37:15.000000 jw_lensegua-1.0.3/src/jw_lensegua/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 17:05:58.013944 jw_lensegua-1.0.3/src/jw_lensegua/tests/
+-rw-rw-rw-   0        0        0        0 2023-02-09 02:39:41.000000 jw_lensegua-1.0.3/src/jw_lensegua/tests/__init__.py
+-rw-rw-rw-   0        0        0    35757 2023-02-19 22:20:19.000000 jw_lensegua-1.0.3/src/jw_lensegua/tests/test_solution.py
+drwxrwxrwx   0        0        0        0 2023-06-13 17:05:58.016945 jw_lensegua-1.0.3/src/jw_lensegua/v1/
+-rw-rw-rw-   0        0        0    35703 2023-02-20 03:14:00.000000 jw_lensegua-1.0.3/src/jw_lensegua/v1/cam.py
+-rw-rw-rw-   0        0        0    20132 2023-02-20 03:03:23.000000 jw_lensegua-1.0.3/src/jw_lensegua/v1/lensegua.py
+-rw-rw-rw-   0        0        0      793 2023-02-12 03:28:51.000000 jw_lensegua-1.0.3/src/jw_lensegua/v1/results_model.py
+-rw-rw-rw-   0        0        0    67243 2023-03-23 04:59:36.000000 jw_lensegua-1.0.3/src/jw_lensegua/v1/solutions.py
+drwxrwxrwx   0        0        0        0 2023-06-13 17:05:58.021448 jw_lensegua-1.0.3/src/jw_lensegua/v2/
+-rw-rw-rw-   0        0        0   108823 2023-06-13 17:00:58.000000 jw_lensegua-1.0.3/src/jw_lensegua/v2/model_class_tf.py
+-rw-rw-rw-   0        0        0     1664 2023-06-09 18:32:08.000000 jw_lensegua-1.0.3/src/jw_lensegua/v2/model_kmean_tf2.py
+-rw-rw-rw-   0        0        0     4129 2023-03-19 22:48:16.000000 jw_lensegua-1.0.3/src/jw_lensegua/v2/model_transfer.py
+-rw-rw-rw-   0        0        0     7633 2023-06-13 17:00:51.000000 jw_lensegua-1.0.3/src/jw_lensegua/v2/sign_language.py
+drwxrwxrwx   0        0        0        0 2023-06-13 17:05:58.011940 jw_lensegua-1.0.3/src/jw_lensegua.egg-info/
+-rw-rw-rw-   0        0        0      983 2023-06-13 17:05:57.000000 jw_lensegua-1.0.3/src/jw_lensegua.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      562 2023-06-13 17:05:57.000000 jw_lensegua-1.0.3/src/jw_lensegua.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 17:05:57.000000 jw_lensegua-1.0.3/src/jw_lensegua.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-06-13 17:05:57.000000 jw_lensegua-1.0.3/src/jw_lensegua.egg-info/top_level.txt
```

### Comparing `jw_lensegua-1.0.2/LICENSE` & `jw_lensegua-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jw_lensegua-1.0.2/pyproject.toml` & `jw_lensegua-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0","numpy>=1.23","pandas>=1.5"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jw_lensegua"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
   { name="Jose Orlando Wannan Escobar", email="jwannan13@gmail.com" },
 ]
 description = "Paquete para administracion de la informacion de datos para reconocer señales, utilizado para LENSEGUA - lenguaje de señas de Guatemala - (model-2)"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `jw_lensegua-1.0.2/src/jw_lensegua/tests/test_solution.py` & `jw_lensegua-1.0.3/src/jw_lensegua/tests/test_solution.py`

 * *Files identical despite different names*

### Comparing `jw_lensegua-1.0.2/src/jw_lensegua/v1/cam.py` & `jw_lensegua-1.0.3/src/jw_lensegua/v1/cam.py`

 * *Files identical despite different names*

### Comparing `jw_lensegua-1.0.2/src/jw_lensegua/v1/lensegua.py` & `jw_lensegua-1.0.3/src/jw_lensegua/v1/lensegua.py`

 * *Files identical despite different names*

### Comparing `jw_lensegua-1.0.2/src/jw_lensegua/v1/results_model.py` & `jw_lensegua-1.0.3/src/jw_lensegua/v1/results_model.py`

 * *Files identical despite different names*

### Comparing `jw_lensegua-1.0.2/src/jw_lensegua/v1/solutions.py` & `jw_lensegua-1.0.3/src/jw_lensegua/v1/solutions.py`

 * *Files identical despite different names*

### Comparing `jw_lensegua-1.0.2/src/jw_lensegua/v2/model_class_tf.py` & `jw_lensegua-1.0.3/src/jw_lensegua/v2/model_class_tf.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import abc
 import pandas as pd
 import numpy as np
-import model_kmean_tf2 as mk
+import v2.model_kmean_tf2 as mk
 
 ## interface models
 
 class Imodel:
     @abc.abstractmethod
     def get_result(self, data) -> object:
         raise NotImplementedError
```

### Comparing `jw_lensegua-1.0.2/src/jw_lensegua/v2/model_kmean_tf2.py` & `jw_lensegua-1.0.3/src/jw_lensegua/v2/model_kmean_tf2.py`

 * *Files identical despite different names*

### Comparing `jw_lensegua-1.0.2/src/jw_lensegua/v2/model_transfer.py` & `jw_lensegua-1.0.3/src/jw_lensegua/v2/model_transfer.py`

 * *Files identical despite different names*

### Comparing `jw_lensegua-1.0.2/src/jw_lensegua/v2/sign_language.py` & `jw_lensegua-1.0.3/src/jw_lensegua/v2/sign_language.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-import model_class_tf as mc
-import model_transfer as mf
+import v2.model_class_tf as mc
+import v2.model_transfer as mf
 import json
 
 class sign_language:
     def __init__(self):
         self.__sign_models_ev = []
         self.__sign_models_mov = []
```

### Comparing `jw_lensegua-1.0.2/src/jw_lensegua.egg-info/SOURCES.txt` & `jw_lensegua-1.0.3/src/jw_lensegua.egg-info/SOURCES.txt`

 * *Files identical despite different names*

