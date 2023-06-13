# Comparing `tmp/jw_lensegua-1.0.4.tar.gz` & `tmp/jw_lensegua-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jw_lensegua-1.0.4.tar", last modified: Tue Jun 13 17:10:22 2023, max compression
+gzip compressed data, was "jw_lensegua-1.0.5.tar", last modified: Tue Jun 13 17:12:30 2023, max compression
```

## Comparing `jw_lensegua-1.0.4.tar` & `jw_lensegua-1.0.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 17:10:22.037907 jw_lensegua-1.0.4/
--rw-rw-rw-   0        0        0    35821 2023-02-07 04:10:38.000000 jw_lensegua-1.0.4/LICENSE
--rw-rw-rw-   0        0        0      983 2023-06-13 17:10:22.037907 jw_lensegua-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      313 2023-06-13 17:05:26.000000 jw_lensegua-1.0.4/README.md
--rw-rw-rw-   0        0        0      873 2023-06-13 17:09:49.000000 jw_lensegua-1.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-13 17:10:22.037907 jw_lensegua-1.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-13 17:10:22.017375 jw_lensegua-1.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-06-13 17:10:22.021889 jw_lensegua-1.0.4/src/jw_lensegua/
--rw-rw-rw-   0        0        0        0 2023-02-09 02:37:15.000000 jw_lensegua-1.0.4/src/jw_lensegua/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 17:10:22.026893 jw_lensegua-1.0.4/src/jw_lensegua/tests/
--rw-rw-rw-   0        0        0        0 2023-02-09 02:39:41.000000 jw_lensegua-1.0.4/src/jw_lensegua/tests/__init__.py
--rw-rw-rw-   0        0        0    35760 2023-06-13 17:09:03.000000 jw_lensegua-1.0.4/src/jw_lensegua/tests/test_solution.py
-drwxrwxrwx   0        0        0        0 2023-06-13 17:10:22.031395 jw_lensegua-1.0.4/src/jw_lensegua/v1/
--rw-rw-rw-   0        0        0    35706 2023-06-13 17:09:18.000000 jw_lensegua-1.0.4/src/jw_lensegua/v1/cam.py
--rw-rw-rw-   0        0        0    20138 2023-06-13 17:09:24.000000 jw_lensegua-1.0.4/src/jw_lensegua/v1/lensegua.py
--rw-rw-rw-   0        0        0      793 2023-02-12 03:28:51.000000 jw_lensegua-1.0.4/src/jw_lensegua/v1/results_model.py
--rw-rw-rw-   0        0        0    67243 2023-03-23 04:59:36.000000 jw_lensegua-1.0.4/src/jw_lensegua/v1/solutions.py
-drwxrwxrwx   0        0        0        0 2023-06-13 17:10:22.036403 jw_lensegua-1.0.4/src/jw_lensegua/v2/
--rw-rw-rw-   0        0        0   108823 2023-06-13 17:00:58.000000 jw_lensegua-1.0.4/src/jw_lensegua/v2/model_class_tf.py
--rw-rw-rw-   0        0        0     1664 2023-06-09 18:32:08.000000 jw_lensegua-1.0.4/src/jw_lensegua/v2/model_kmean_tf2.py
--rw-rw-rw-   0        0        0     4129 2023-03-19 22:48:16.000000 jw_lensegua-1.0.4/src/jw_lensegua/v2/model_transfer.py
--rw-rw-rw-   0        0        0     7657 2023-06-13 17:09:11.000000 jw_lensegua-1.0.4/src/jw_lensegua/v2/sign_language.py
-drwxrwxrwx   0        0        0        0 2023-06-13 17:10:22.025893 jw_lensegua-1.0.4/src/jw_lensegua.egg-info/
--rw-rw-rw-   0        0        0      983 2023-06-13 17:10:22.000000 jw_lensegua-1.0.4/src/jw_lensegua.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      562 2023-06-13 17:10:22.000000 jw_lensegua-1.0.4/src/jw_lensegua.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 17:10:22.000000 jw_lensegua-1.0.4/src/jw_lensegua.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-06-13 17:10:22.000000 jw_lensegua-1.0.4/src/jw_lensegua.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-13 17:12:29.999134 jw_lensegua-1.0.5/
+-rw-rw-rw-   0        0        0    35821 2023-02-07 04:10:38.000000 jw_lensegua-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0      983 2023-06-13 17:12:29.999134 jw_lensegua-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      313 2023-06-13 17:05:26.000000 jw_lensegua-1.0.5/README.md
+-rw-rw-rw-   0        0        0      873 2023-06-13 17:12:09.000000 jw_lensegua-1.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-13 17:12:29.999134 jw_lensegua-1.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-13 17:12:29.977821 jw_lensegua-1.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-06-13 17:12:29.982077 jw_lensegua-1.0.5/src/jw_lensegua/
+-rw-rw-rw-   0        0        0        0 2023-02-09 02:37:15.000000 jw_lensegua-1.0.5/src/jw_lensegua/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 17:12:29.988597 jw_lensegua-1.0.5/src/jw_lensegua/tests/
+-rw-rw-rw-   0        0        0        0 2023-02-09 02:39:41.000000 jw_lensegua-1.0.5/src/jw_lensegua/tests/__init__.py
+-rw-rw-rw-   0        0        0    35760 2023-06-13 17:09:03.000000 jw_lensegua-1.0.5/src/jw_lensegua/tests/test_solution.py
+drwxrwxrwx   0        0        0        0 2023-06-13 17:12:29.994135 jw_lensegua-1.0.5/src/jw_lensegua/v1/
+-rw-rw-rw-   0        0        0    35706 2023-06-13 17:09:18.000000 jw_lensegua-1.0.5/src/jw_lensegua/v1/cam.py
+-rw-rw-rw-   0        0        0    20138 2023-06-13 17:09:24.000000 jw_lensegua-1.0.5/src/jw_lensegua/v1/lensegua.py
+-rw-rw-rw-   0        0        0      793 2023-02-12 03:28:51.000000 jw_lensegua-1.0.5/src/jw_lensegua/v1/results_model.py
+-rw-rw-rw-   0        0        0    67243 2023-03-23 04:59:36.000000 jw_lensegua-1.0.5/src/jw_lensegua/v1/solutions.py
+drwxrwxrwx   0        0        0        0 2023-06-13 17:12:29.998135 jw_lensegua-1.0.5/src/jw_lensegua/v2/
+-rw-rw-rw-   0        0        0   108835 2023-06-13 17:11:54.000000 jw_lensegua-1.0.5/src/jw_lensegua/v2/model_class_tf.py
+-rw-rw-rw-   0        0        0     1664 2023-06-09 18:32:08.000000 jw_lensegua-1.0.5/src/jw_lensegua/v2/model_kmean_tf2.py
+-rw-rw-rw-   0        0        0     4129 2023-03-19 22:48:16.000000 jw_lensegua-1.0.5/src/jw_lensegua/v2/model_transfer.py
+-rw-rw-rw-   0        0        0     7657 2023-06-13 17:09:11.000000 jw_lensegua-1.0.5/src/jw_lensegua/v2/sign_language.py
+drwxrwxrwx   0        0        0        0 2023-06-13 17:12:29.986076 jw_lensegua-1.0.5/src/jw_lensegua.egg-info/
+-rw-rw-rw-   0        0        0      983 2023-06-13 17:12:29.000000 jw_lensegua-1.0.5/src/jw_lensegua.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      562 2023-06-13 17:12:29.000000 jw_lensegua-1.0.5/src/jw_lensegua.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 17:12:29.000000 jw_lensegua-1.0.5/src/jw_lensegua.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-06-13 17:12:29.000000 jw_lensegua-1.0.5/src/jw_lensegua.egg-info/top_level.txt
```

### Comparing `jw_lensegua-1.0.4/LICENSE` & `jw_lensegua-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `jw_lensegua-1.0.4/PKG-INFO` & `jw_lensegua-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jw_lensegua
-Version: 1.0.4
+Version: 1.0.5
 Summary: Paquete para administracion de la informacion de datos para reconocer señales, utilizado para LENSEGUA - lenguaje de señas de Guatemala - (model-2)
 Author-email: Jose Orlando Wannan Escobar <jwannan13@gmail.com>
 Project-URL: Homepage, https://github.com/JoWan1998/lenguaje_senas
 Project-URL: Bug Tracker, https://github.com/JoWan1998/lenguaje_senas/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `jw_lensegua-1.0.4/pyproject.toml` & `jw_lensegua-1.0.5/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0","numpy>=1.23","pandas>=1.5"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jw_lensegua"
-version = "1.0.4"
+version = "1.0.5"
 authors = [
   { name="Jose Orlando Wannan Escobar", email="jwannan13@gmail.com" },
 ]
 description = "Paquete para administracion de la informacion de datos para reconocer señales, utilizado para LENSEGUA - lenguaje de señas de Guatemala - (model-2)"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `jw_lensegua-1.0.4/src/jw_lensegua/tests/test_solution.py` & `jw_lensegua-1.0.5/src/jw_lensegua/tests/test_solution.py`

 * *Files identical despite different names*

### Comparing `jw_lensegua-1.0.4/src/jw_lensegua/v1/cam.py` & `jw_lensegua-1.0.5/src/jw_lensegua/v1/cam.py`

 * *Files identical despite different names*

### Comparing `jw_lensegua-1.0.4/src/jw_lensegua/v1/lensegua.py` & `jw_lensegua-1.0.5/src/jw_lensegua/v1/lensegua.py`

 * *Files identical despite different names*

### Comparing `jw_lensegua-1.0.4/src/jw_lensegua/v1/results_model.py` & `jw_lensegua-1.0.5/src/jw_lensegua/v1/results_model.py`

 * *Files identical despite different names*

### Comparing `jw_lensegua-1.0.4/src/jw_lensegua/v1/solutions.py` & `jw_lensegua-1.0.5/src/jw_lensegua/v1/solutions.py`

 * *Files identical despite different names*

### Comparing `jw_lensegua-1.0.4/src/jw_lensegua/v2/model_class_tf.py` & `jw_lensegua-1.0.5/src/jw_lensegua/v2/model_class_tf.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import abc
 import pandas as pd
 import numpy as np
-import v2.model_kmean_tf2 as mk
+import jw_lensegua.v2.model_kmean_tf2 as mk
 
 ## interface models
 
 class Imodel:
     @abc.abstractmethod
     def get_result(self, data) -> object:
         raise NotImplementedError
```

### Comparing `jw_lensegua-1.0.4/src/jw_lensegua/v2/model_kmean_tf2.py` & `jw_lensegua-1.0.5/src/jw_lensegua/v2/model_kmean_tf2.py`

 * *Files identical despite different names*

### Comparing `jw_lensegua-1.0.4/src/jw_lensegua/v2/model_transfer.py` & `jw_lensegua-1.0.5/src/jw_lensegua/v2/model_transfer.py`

 * *Files identical despite different names*

### Comparing `jw_lensegua-1.0.4/src/jw_lensegua/v2/sign_language.py` & `jw_lensegua-1.0.5/src/jw_lensegua/v2/sign_language.py`

 * *Files identical despite different names*

### Comparing `jw_lensegua-1.0.4/src/jw_lensegua.egg-info/PKG-INFO` & `jw_lensegua-1.0.5/src/jw_lensegua.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jw-lensegua
-Version: 1.0.4
+Version: 1.0.5
 Summary: Paquete para administracion de la informacion de datos para reconocer señales, utilizado para LENSEGUA - lenguaje de señas de Guatemala - (model-2)
 Author-email: Jose Orlando Wannan Escobar <jwannan13@gmail.com>
 Project-URL: Homepage, https://github.com/JoWan1998/lenguaje_senas
 Project-URL: Bug Tracker, https://github.com/JoWan1998/lenguaje_senas/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `jw_lensegua-1.0.4/src/jw_lensegua.egg-info/SOURCES.txt` & `jw_lensegua-1.0.5/src/jw_lensegua.egg-info/SOURCES.txt`

 * *Files identical despite different names*

