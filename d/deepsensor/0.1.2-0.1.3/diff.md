# Comparing `tmp/deepsensor-0.1.2.tar.gz` & `tmp/deepsensor-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepsensor-0.1.2.tar", last modified: Sun Jun 11 22:56:26 2023, max compression
+gzip compressed data, was "deepsensor-0.1.3.tar", last modified: Tue Jun 13 14:45:52 2023, max compression
```

## Comparing `deepsensor-0.1.2.tar` & `deepsensor-0.1.3.tar`

### file list

```diff
@@ -1,48 +1,42 @@
-drwxrwxr-x   0 tomand    (1001) tomand    (1001)        0 2023-06-11 22:56:26.066173 deepsensor-0.1.2/
--rw-rw-r--   0 tomand    (1001) tomand    (1001)     1076 2023-05-16 13:27:41.000000 deepsensor-0.1.2/LICENSE
--rw-rw-r--   0 tomand    (1001) tomand    (1001)     4957 2023-06-11 22:56:26.066173 deepsensor-0.1.2/PKG-INFO
--rw-rw-r--   0 tomand    (1001) tomand    (1001)     4560 2023-06-10 16:25:41.000000 deepsensor-0.1.2/README.md
-drwxrwxr-x   0 tomand    (1001) tomand    (1001)        0 2023-06-11 22:56:26.062173 deepsensor-0.1.2/deepsensor/
--rw-rw-r--   0 tomand    (1001) tomand    (1001)      329 2023-06-11 17:55:57.000000 deepsensor-0.1.2/deepsensor/__init__.py
--rw-rw-r--   0 tomand    (1001) tomand    (1001)      278 2023-06-11 21:28:07.000000 deepsensor-0.1.2/deepsensor/_version.py
-drwxrwxr-x   0 tomand    (1001) tomand    (1001)        0 2023-06-11 22:56:26.062173 deepsensor-0.1.2/deepsensor/active_learning/
--rw-rw-r--   0 tomand    (1001) tomand    (1001)        0 2023-05-19 14:49:00.000000 deepsensor-0.1.2/deepsensor/active_learning/__init__.py
--rw-rw-r--   0 tomand    (1001) tomand    (1001)     8772 2023-05-22 14:39:54.000000 deepsensor-0.1.2/deepsensor/active_learning/acquisition_fns.py
--rw-rw-r--   0 tomand    (1001) tomand    (1001)      170 2023-06-09 15:07:15.000000 deepsensor-0.1.2/deepsensor/config.py
-drwxrwxr-x   0 tomand    (1001) tomand    (1001)        0 2023-06-11 22:56:26.062173 deepsensor-0.1.2/deepsensor/data/
--rw-rw-r--   0 tomand    (1001) tomand    (1001)        0 2023-05-24 11:14:34.000000 deepsensor-0.1.2/deepsensor/data/__init__.py
--rw-rw-r--   0 tomand    (1001) tomand    (1001)    22102 2023-06-07 17:20:41.000000 deepsensor-0.1.2/deepsensor/data/loader.py
--rw-rw-r--   0 tomand    (1001) tomand    (1001)    14246 2023-06-09 15:07:15.000000 deepsensor-0.1.2/deepsensor/data/processor.py
--rw-rw-r--   0 tomand    (1001) tomand    (1001)     3509 2023-05-31 22:34:31.000000 deepsensor-0.1.2/deepsensor/data/task.py
--rw-rw-r--   0 tomand    (1001) tomand    (1001)     3717 2023-06-07 17:20:41.000000 deepsensor-0.1.2/deepsensor/data/utils.py
-drwxrwxr-x   0 tomand    (1001) tomand    (1001)        0 2023-06-11 22:56:26.062173 deepsensor-0.1.2/deepsensor/model/
--rw-rw-r--   0 tomand    (1001) tomand    (1001)        0 2023-05-24 11:14:34.000000 deepsensor-0.1.2/deepsensor/model/__init__.py
--rw-rw-r--   0 tomand    (1001) tomand    (1001)     2830 2023-06-11 18:38:33.000000 deepsensor-0.1.2/deepsensor/model/defaults.py
--rw-rw-r--   0 tomand    (1001) tomand    (1001)    28006 2023-06-10 13:53:55.000000 deepsensor-0.1.2/deepsensor/model/models.py
--rw-rw-r--   0 tomand    (1001) tomand    (1001)     8042 2023-06-10 14:54:25.000000 deepsensor-0.1.2/deepsensor/model/nps.py
--rw-rw-r--   0 tomand    (1001) tomand    (1001)     7376 2023-06-11 20:24:15.000000 deepsensor-0.1.2/deepsensor/plot.py
--rw-rw-r--   0 tomand    (1001) tomand    (1001)        0 2023-06-05 14:47:21.000000 deepsensor-0.1.2/deepsensor/py.typed
-drwxrwxr-x   0 tomand    (1001) tomand    (1001)        0 2023-06-11 22:56:26.062173 deepsensor-0.1.2/deepsensor/tensorflow/
--rw-rw-r--   0 tomand    (1001) tomand    (1001)      826 2023-06-09 15:07:15.000000 deepsensor-0.1.2/deepsensor/tensorflow/__init__.py
-drwxrwxr-x   0 tomand    (1001) tomand    (1001)        0 2023-06-11 22:56:26.062173 deepsensor-0.1.2/deepsensor/torch/
--rw-rw-r--   0 tomand    (1001) tomand    (1001)      788 2023-06-09 15:03:43.000000 deepsensor-0.1.2/deepsensor/torch/__init__.py
-drwxrwxr-x   0 tomand    (1001) tomand    (1001)        0 2023-06-11 22:56:26.066173 deepsensor-0.1.2/deepsensor/train/
--rw-rw-r--   0 tomand    (1001) tomand    (1001)        0 2023-06-06 13:04:03.000000 deepsensor-0.1.2/deepsensor/train/__init__.py
--rw-rw-r--   0 tomand    (1001) tomand    (1001)     3770 2023-06-09 17:05:13.000000 deepsensor-0.1.2/deepsensor/train/train.py
--rw-rw-r--   0 tomand    (1001) tomand    (1001)        0 2023-05-17 10:49:11.000000 deepsensor-0.1.2/deepsensor/utils.py
-drwxrwxr-x   0 tomand    (1001) tomand    (1001)        0 2023-06-11 22:56:26.062173 deepsensor-0.1.2/deepsensor.egg-info/
--rw-rw-r--   0 tomand    (1001) tomand    (1001)     4957 2023-06-11 22:56:26.000000 deepsensor-0.1.2/deepsensor.egg-info/PKG-INFO
--rw-rw-r--   0 tomand    (1001) tomand    (1001)      931 2023-06-11 22:56:26.000000 deepsensor-0.1.2/deepsensor.egg-info/SOURCES.txt
--rw-rw-r--   0 tomand    (1001) tomand    (1001)        1 2023-06-11 22:56:26.000000 deepsensor-0.1.2/deepsensor.egg-info/dependency_links.txt
--rw-rw-r--   0 tomand    (1001) tomand    (1001)        1 2023-06-10 14:42:57.000000 deepsensor-0.1.2/deepsensor.egg-info/not-zip-safe
--rw-rw-r--   0 tomand    (1001) tomand    (1001)      127 2023-06-11 22:56:26.000000 deepsensor-0.1.2/deepsensor.egg-info/requires.txt
--rw-rw-r--   0 tomand    (1001) tomand    (1001)       17 2023-06-11 22:56:26.000000 deepsensor-0.1.2/deepsensor.egg-info/top_level.txt
--rw-rw-r--   0 tomand    (1001) tomand    (1001)      471 2023-06-10 15:57:32.000000 deepsensor-0.1.2/pyproject.toml
--rw-rw-r--   0 tomand    (1001) tomand    (1001)      882 2023-06-11 22:56:26.066173 deepsensor-0.1.2/setup.cfg
--rw-rw-r--   0 tomand    (1001) tomand    (1001)       69 2023-06-11 22:18:42.000000 deepsensor-0.1.2/setup.py
-drwxrwxr-x   0 tomand    (1001) tomand    (1001)        0 2023-06-11 22:56:26.066173 deepsensor-0.1.2/tests/
--rw-rw-r--   0 tomand    (1001) tomand    (1001)        0 2023-06-05 15:06:33.000000 deepsensor-0.1.2/tests/__init__.py
--rw-rw-r--   0 tomand    (1001) tomand    (1001)     7896 2023-06-09 15:07:18.000000 deepsensor-0.1.2/tests/test_data_processor.py
--rw-rw-r--   0 tomand    (1001) tomand    (1001)     8740 2023-06-07 17:20:41.000000 deepsensor-0.1.2/tests/test_model.py
--rw-rw-r--   0 tomand    (1001) tomand    (1001)     5845 2023-06-07 17:20:41.000000 deepsensor-0.1.2/tests/test_task_loader.py
--rw-rw-r--   0 tomand    (1001) tomand    (1001)     2028 2023-06-08 17:10:45.000000 deepsensor-0.1.2/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:45:52.329380 deepsensor-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-06-13 14:45:52.329380 deepsensor-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-06-13 14:45:41.000000 deepsensor-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:45:52.325380 deepsensor-0.1.3/deepsensor/
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-13 14:45:41.000000 deepsensor-0.1.3/deepsensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-13 14:45:41.000000 deepsensor-0.1.3/deepsensor/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:45:52.329380 deepsensor-0.1.3/deepsensor/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 14:45:41.000000 deepsensor-0.1.3/deepsensor/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22102 2023-06-13 14:45:41.000000 deepsensor-0.1.3/deepsensor/data/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14246 2023-06-13 14:45:41.000000 deepsensor-0.1.3/deepsensor/data/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-06-13 14:45:41.000000 deepsensor-0.1.3/deepsensor/data/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-06-13 14:45:41.000000 deepsensor-0.1.3/deepsensor/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:45:52.329380 deepsensor-0.1.3/deepsensor/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 14:45:41.000000 deepsensor-0.1.3/deepsensor/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-06-13 14:45:41.000000 deepsensor-0.1.3/deepsensor/model/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28006 2023-06-13 14:45:41.000000 deepsensor-0.1.3/deepsensor/model/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8042 2023-06-13 14:45:41.000000 deepsensor-0.1.3/deepsensor/model/nps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7376 2023-06-13 14:45:41.000000 deepsensor-0.1.3/deepsensor/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 14:45:41.000000 deepsensor-0.1.3/deepsensor/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:45:52.329380 deepsensor-0.1.3/deepsensor/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-13 14:45:41.000000 deepsensor-0.1.3/deepsensor/tensorflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:45:52.329380 deepsensor-0.1.3/deepsensor/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-13 14:45:41.000000 deepsensor-0.1.3/deepsensor/torch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:45:52.329380 deepsensor-0.1.3/deepsensor/train/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 14:45:41.000000 deepsensor-0.1.3/deepsensor/train/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-06-13 14:45:41.000000 deepsensor-0.1.3/deepsensor/train/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:45:52.329380 deepsensor-0.1.3/deepsensor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-06-13 14:45:52.000000 deepsensor-0.1.3/deepsensor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-13 14:45:52.000000 deepsensor-0.1.3/deepsensor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 14:45:52.000000 deepsensor-0.1.3/deepsensor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 14:45:52.000000 deepsensor-0.1.3/deepsensor.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-13 14:45:52.000000 deepsensor-0.1.3/deepsensor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-13 14:45:52.000000 deepsensor-0.1.3/deepsensor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-13 14:45:41.000000 deepsensor-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-06-13 14:45:52.329380 deepsensor-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-13 14:45:41.000000 deepsensor-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:45:52.329380 deepsensor-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 14:45:41.000000 deepsensor-0.1.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7896 2023-06-13 14:45:41.000000 deepsensor-0.1.3/tests/test_data_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8740 2023-06-13 14:45:41.000000 deepsensor-0.1.3/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-06-13 14:45:41.000000 deepsensor-0.1.3/tests/test_task_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-06-13 14:45:41.000000 deepsensor-0.1.3/tests/utils.py
```

### Comparing `deepsensor-0.1.2/PKG-INFO` & `deepsensor-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepsensor
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python package for modelling xarray and pandas data with neural processes.
 Home-page: https://github.com/tom-andersson/deepsensor
 Author: Tom R. Andersson
 Author-email: tomand@bas.ac.uk
 License: MIT
 Platform: unix
 Platform: linux
```

### Comparing `deepsensor-0.1.2/README.md` & `deepsensor-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `deepsensor-0.1.2/deepsensor/data/loader.py` & `deepsensor-0.1.3/deepsensor/data/loader.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.1.2/deepsensor/data/processor.py` & `deepsensor-0.1.3/deepsensor/data/processor.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.1.2/deepsensor/data/task.py` & `deepsensor-0.1.3/deepsensor/data/task.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.1.2/deepsensor/data/utils.py` & `deepsensor-0.1.3/deepsensor/data/utils.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.1.2/deepsensor/model/defaults.py` & `deepsensor-0.1.3/deepsensor/model/defaults.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.1.2/deepsensor/model/models.py` & `deepsensor-0.1.3/deepsensor/model/models.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.1.2/deepsensor/model/nps.py` & `deepsensor-0.1.3/deepsensor/model/nps.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.1.2/deepsensor/plot.py` & `deepsensor-0.1.3/deepsensor/plot.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.1.2/deepsensor/tensorflow/__init__.py` & `deepsensor-0.1.3/deepsensor/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.1.2/deepsensor/torch/__init__.py` & `deepsensor-0.1.3/deepsensor/torch/__init__.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.1.2/deepsensor/train/train.py` & `deepsensor-0.1.3/deepsensor/train/train.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.1.2/deepsensor.egg-info/PKG-INFO` & `deepsensor-0.1.3/deepsensor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepsensor
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python package for modelling xarray and pandas data with neural processes.
 Home-page: https://github.com/tom-andersson/deepsensor
 Author: Tom R. Andersson
 Author-email: tomand@bas.ac.uk
 License: MIT
 Platform: unix
 Platform: linux
```

### Comparing `deepsensor-0.1.2/deepsensor.egg-info/SOURCES.txt` & `deepsensor-0.1.3/deepsensor.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,21 @@
-LICENSE
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 deepsensor/__init__.py
-deepsensor/_version.py
 deepsensor/config.py
 deepsensor/plot.py
 deepsensor/py.typed
-deepsensor/utils.py
 deepsensor.egg-info/PKG-INFO
 deepsensor.egg-info/SOURCES.txt
 deepsensor.egg-info/dependency_links.txt
 deepsensor.egg-info/not-zip-safe
 deepsensor.egg-info/requires.txt
 deepsensor.egg-info/top_level.txt
-deepsensor/active_learning/__init__.py
-deepsensor/active_learning/acquisition_fns.py
 deepsensor/data/__init__.py
 deepsensor/data/loader.py
 deepsensor/data/processor.py
 deepsensor/data/task.py
 deepsensor/data/utils.py
 deepsensor/model/__init__.py
 deepsensor/model/defaults.py
```

### Comparing `deepsensor-0.1.2/setup.cfg` & `deepsensor-0.1.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = deepsensor
-version = 0.1.2
+version = 0.1.3
 author = Tom R. Andersson
 author_email = tomand@bas.ac.uk
 description = A Python package for modelling xarray and pandas data with neural processes.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/tom-andersson/deepsensor
 license = MIT
@@ -27,14 +27,15 @@
 	numpy
 	pandas
 	xarray
 	dask
 	distributed
 	pyshp
 	tqdm
+	pooch
 
 [options.extras_require]
 testing = 
 	pytest
 	pytest-cov
 	mypy
 	tox
```

### Comparing `deepsensor-0.1.2/tests/test_data_processor.py` & `deepsensor-0.1.3/tests/test_data_processor.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.1.2/tests/test_model.py` & `deepsensor-0.1.3/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.1.2/tests/test_task_loader.py` & `deepsensor-0.1.3/tests/test_task_loader.py`

 * *Files identical despite different names*

### Comparing `deepsensor-0.1.2/tests/utils.py` & `deepsensor-0.1.3/tests/utils.py`

 * *Files identical despite different names*

