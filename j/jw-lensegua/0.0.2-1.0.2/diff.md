# Comparing `tmp/jw_lensegua-0.0.2.tar.gz` & `tmp/jw_lensegua-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jw_lensegua-0.0.2.tar", last modified: Mon Feb 20 03:26:52 2023, max compression
+gzip compressed data, was "jw_lensegua-1.0.2.tar", last modified: Mon Jun 12 22:41:01 2023, max compression
```

## Comparing `jw_lensegua-0.0.2.tar` & `jw_lensegua-1.0.2.tar`

### file list

```diff
@@ -1,21 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-02-20 03:26:52.550017 jw_lensegua-0.0.2/
--rw-rw-rw-   0        0        0    35821 2023-02-07 04:10:38.000000 jw_lensegua-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      654 2023-02-20 03:26:52.550017 jw_lensegua-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-02-07 03:54:35.000000 jw_lensegua-0.0.2/README.md
--rw-rw-rw-   0        0        0      833 2023-02-20 02:19:43.000000 jw_lensegua-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-02-20 03:26:52.550017 jw_lensegua-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-02-20 03:26:52.504520 jw_lensegua-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-02-20 03:26:52.520543 jw_lensegua-0.0.2/src/jw_lensegua/
--rw-rw-rw-   0        0        0        0 2023-02-09 02:37:15.000000 jw_lensegua-0.0.2/src/jw_lensegua/__init__.py
--rw-rw-rw-   0        0        0    35703 2023-02-20 03:14:00.000000 jw_lensegua-0.0.2/src/jw_lensegua/cam.py
--rw-rw-rw-   0        0        0    20132 2023-02-20 03:03:23.000000 jw_lensegua-0.0.2/src/jw_lensegua/lensegua.py
--rw-rw-rw-   0        0        0      793 2023-02-12 03:28:51.000000 jw_lensegua-0.0.2/src/jw_lensegua/results_model.py
--rw-rw-rw-   0        0        0    67243 2023-02-20 03:02:45.000000 jw_lensegua-0.0.2/src/jw_lensegua/solutions.py
-drwxrwxrwx   0        0        0        0 2023-02-20 03:26:52.546485 jw_lensegua-0.0.2/src/jw_lensegua/tests/
--rw-rw-rw-   0        0        0        0 2023-02-09 02:39:41.000000 jw_lensegua-0.0.2/src/jw_lensegua/tests/__init__.py
--rw-rw-rw-   0        0        0    35757 2023-02-19 22:20:19.000000 jw_lensegua-0.0.2/src/jw_lensegua/tests/test_solution.py
-drwxrwxrwx   0        0        0        0 2023-02-20 03:26:52.526476 jw_lensegua-0.0.2/src/jw_lensegua.egg-info/
--rw-rw-rw-   0        0        0      654 2023-02-20 03:26:52.000000 jw_lensegua-0.0.2/src/jw_lensegua.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      402 2023-02-20 03:26:52.000000 jw_lensegua-0.0.2/src/jw_lensegua.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-20 03:26:52.000000 jw_lensegua-0.0.2/src/jw_lensegua.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-02-20 03:26:52.000000 jw_lensegua-0.0.2/src/jw_lensegua.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-12 22:41:01.105694 jw_lensegua-1.0.2/
+-rw-rw-rw-   0        0        0    35821 2023-02-07 04:10:38.000000 jw_lensegua-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0      666 2023-06-12 22:41:01.104696 jw_lensegua-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-02-07 03:54:35.000000 jw_lensegua-1.0.2/README.md
+-rw-rw-rw-   0        0        0      873 2023-06-12 22:40:37.000000 jw_lensegua-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-12 22:41:01.105694 jw_lensegua-1.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-12 22:41:01.083733 jw_lensegua-1.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-12 22:41:01.088606 jw_lensegua-1.0.2/src/jw_lensegua/
+-rw-rw-rw-   0        0        0        0 2023-02-09 02:37:15.000000 jw_lensegua-1.0.2/src/jw_lensegua/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 22:41:01.095607 jw_lensegua-1.0.2/src/jw_lensegua/tests/
+-rw-rw-rw-   0        0        0        0 2023-02-09 02:39:41.000000 jw_lensegua-1.0.2/src/jw_lensegua/tests/__init__.py
+-rw-rw-rw-   0        0        0    35757 2023-02-19 22:20:19.000000 jw_lensegua-1.0.2/src/jw_lensegua/tests/test_solution.py
+drwxrwxrwx   0        0        0        0 2023-06-12 22:41:01.098693 jw_lensegua-1.0.2/src/jw_lensegua/v1/
+-rw-rw-rw-   0        0        0    35703 2023-02-20 03:14:00.000000 jw_lensegua-1.0.2/src/jw_lensegua/v1/cam.py
+-rw-rw-rw-   0        0        0    20132 2023-02-20 03:03:23.000000 jw_lensegua-1.0.2/src/jw_lensegua/v1/lensegua.py
+-rw-rw-rw-   0        0        0      793 2023-02-12 03:28:51.000000 jw_lensegua-1.0.2/src/jw_lensegua/v1/results_model.py
+-rw-rw-rw-   0        0        0    67243 2023-03-23 04:59:36.000000 jw_lensegua-1.0.2/src/jw_lensegua/v1/solutions.py
+drwxrwxrwx   0        0        0        0 2023-06-12 22:41:01.102694 jw_lensegua-1.0.2/src/jw_lensegua/v2/
+-rw-rw-rw-   0        0        0   108820 2023-06-12 18:13:47.000000 jw_lensegua-1.0.2/src/jw_lensegua/v2/model_class_tf.py
+-rw-rw-rw-   0        0        0     1664 2023-06-09 18:32:08.000000 jw_lensegua-1.0.2/src/jw_lensegua/v2/model_kmean_tf2.py
+-rw-rw-rw-   0        0        0     4129 2023-03-19 22:48:16.000000 jw_lensegua-1.0.2/src/jw_lensegua/v2/model_transfer.py
+-rw-rw-rw-   0        0        0     7627 2023-06-09 21:04:34.000000 jw_lensegua-1.0.2/src/jw_lensegua/v2/sign_language.py
+drwxrwxrwx   0        0        0        0 2023-06-12 22:41:01.093609 jw_lensegua-1.0.2/src/jw_lensegua.egg-info/
+-rw-rw-rw-   0        0        0      666 2023-06-12 22:41:01.000000 jw_lensegua-1.0.2/src/jw_lensegua.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      562 2023-06-12 22:41:01.000000 jw_lensegua-1.0.2/src/jw_lensegua.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 22:41:01.000000 jw_lensegua-1.0.2/src/jw_lensegua.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-06-12 22:41:01.000000 jw_lensegua-1.0.2/src/jw_lensegua.egg-info/top_level.txt
```

### Comparing `jw_lensegua-0.0.2/LICENSE` & `jw_lensegua-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jw_lensegua-0.0.2/PKG-INFO` & `jw_lensegua-1.0.2/src/jw_lensegua.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
-Name: jw_lensegua
-Version: 0.0.2
-Summary: Paquete para administracion de la informacion de datos para reconocer señales, utilizado para LENSEGUA - lenguaje de señas de Guatemala
+Name: jw-lensegua
+Version: 1.0.2
+Summary: Paquete para administracion de la informacion de datos para reconocer señales, utilizado para LENSEGUA - lenguaje de señas de Guatemala - (model-2)
 Author-email: Jose Orlando Wannan Escobar <jwannan13@gmail.com>
 Project-URL: Homepage, https://github.com/JoWan1998/lenguaje_senas
 Project-URL: Bug Tracker, https://github.com/JoWan1998/lenguaje_senas/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `jw_lensegua-0.0.2/pyproject.toml` & `jw_lensegua-1.0.2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
-requires = ["setuptools>=61.0"]
+requires = ["setuptools>=61.0","numpy>=1.23","pandas>=1.5"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jw_lensegua"
-version = "0.0.2"
+version = "1.0.2"
 authors = [
   { name="Jose Orlando Wannan Escobar", email="jwannan13@gmail.com" },
 ]
-description = "Paquete para administracion de la informacion de datos para reconocer señales, utilizado para LENSEGUA - lenguaje de señas de Guatemala"
+description = "Paquete para administracion de la informacion de datos para reconocer señales, utilizado para LENSEGUA - lenguaje de señas de Guatemala - (model-2)"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `jw_lensegua-0.0.2/src/jw_lensegua/cam.py` & `jw_lensegua-1.0.2/src/jw_lensegua/v1/cam.py`

 * *Files identical despite different names*

### Comparing `jw_lensegua-0.0.2/src/jw_lensegua/lensegua.py` & `jw_lensegua-1.0.2/src/jw_lensegua/v1/lensegua.py`

 * *Files identical despite different names*

### Comparing `jw_lensegua-0.0.2/src/jw_lensegua/results_model.py` & `jw_lensegua-1.0.2/src/jw_lensegua/v1/results_model.py`

 * *Files identical despite different names*

### Comparing `jw_lensegua-0.0.2/src/jw_lensegua/solutions.py` & `jw_lensegua-1.0.2/src/jw_lensegua/v1/solutions.py`

 * *Files identical despite different names*

### Comparing `jw_lensegua-0.0.2/src/jw_lensegua/tests/test_solution.py` & `jw_lensegua-1.0.2/src/jw_lensegua/tests/test_solution.py`

 * *Files identical despite different names*

### Comparing `jw_lensegua-0.0.2/src/jw_lensegua.egg-info/PKG-INFO` & `jw_lensegua-1.0.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
-Name: jw-lensegua
-Version: 0.0.2
-Summary: Paquete para administracion de la informacion de datos para reconocer señales, utilizado para LENSEGUA - lenguaje de señas de Guatemala
+Name: jw_lensegua
+Version: 1.0.2
+Summary: Paquete para administracion de la informacion de datos para reconocer señales, utilizado para LENSEGUA - lenguaje de señas de Guatemala - (model-2)
 Author-email: Jose Orlando Wannan Escobar <jwannan13@gmail.com>
 Project-URL: Homepage, https://github.com/JoWan1998/lenguaje_senas
 Project-URL: Bug Tracker, https://github.com/JoWan1998/lenguaje_senas/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

