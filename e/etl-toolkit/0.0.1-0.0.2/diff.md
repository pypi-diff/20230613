# Comparing `tmp/etl_toolkit-0.0.1.tar.gz` & `tmp/etl_toolkit-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etl_toolkit-0.0.1.tar", max compression
+gzip compressed data, was "etl_toolkit-0.0.2.tar", max compression
```

## Comparing `etl_toolkit-0.0.1.tar` & `etl_toolkit-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1074 2023-05-31 03:22:08.390518 etl_toolkit-0.0.1/LICENSE
--rw-r--r--   0        0        0      126 2023-05-31 03:22:08.390518 etl_toolkit-0.0.1/README.md
--rw-r--r--   0        0        0     1355 2023-05-31 03:22:08.402518 etl_toolkit-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      341 2023-05-31 03:22:08.406518 etl_toolkit-0.0.1/src/etl/__init__.py
--rw-r--r--   0        0        0     1271 2023-05-31 03:22:08.406518 etl_toolkit-0.0.1/src/etl/cli/__init__.py
--rw-r--r--   0        0        0      844 2023-05-31 03:22:08.406518 etl_toolkit-0.0.1/src/etl/cli/app.py
--rw-r--r--   0        0        0     1220 2023-05-31 03:22:08.406518 etl_toolkit-0.0.1/src/etl/cli/main.py
--rw-r--r--   0        0        0        0 2023-05-31 03:22:08.406518 etl_toolkit-0.0.1/src/etl/config/__init__.py
--rw-r--r--   0        0        0     4380 2023-05-31 03:22:08.406518 etl_toolkit-0.0.1/src/etl/config/app.py
--rw-r--r--   0        0        0      151 2023-05-31 03:22:08.406518 etl_toolkit-0.0.1/src/etl/config/auth_type.py
--rw-r--r--   0        0        0     3296 2023-05-31 03:22:08.406518 etl_toolkit-0.0.1/src/etl/config/database.py
--rw-r--r--   0        0        0      443 2023-05-31 03:22:08.406518 etl_toolkit-0.0.1/src/etl/config/settings.py
--rw-r--r--   0        0        0      684 2023-05-31 03:22:08.406518 etl_toolkit-0.0.1/src/etl/config/yaml.py
--rw-r--r--   0        0        0      382 2023-05-31 03:22:08.406518 etl_toolkit-0.0.1/src/etl/models/file_parsing_result.py
--rw-r--r--   0        0        0      309 2023-05-31 03:22:08.406518 etl_toolkit-0.0.1/src/etl/paths.py
--rw-r--r--   0        0        0     1503 2023-05-31 03:22:08.406518 etl_toolkit-0.0.1/src/etl/pipeline.py
--rw-r--r--   0        0        0        0 2023-05-31 03:22:08.406518 etl_toolkit-0.0.1/src/etl/py.typed
--rw-r--r--   0        0        0      138 2023-05-31 03:22:08.406518 etl_toolkit-0.0.1/src/etl/std/__init__.py
--rw-r--r--   0        0        0      883 2023-05-31 03:22:08.406518 etl_toolkit-0.0.1/src/etl/std/error.py
--rw-r--r--   0        0        0      334 2023-05-31 03:22:08.406518 etl_toolkit-0.0.1/src/etl/std/error_results.py
--rw-r--r--   0        0        0      194 2023-05-31 03:22:08.406518 etl_toolkit-0.0.1/src/etl/std/exceptions.py
--rw-r--r--   0        0        0     2374 2023-05-31 03:22:08.406518 etl_toolkit-0.0.1/src/etl/std/result.py
--rw-r--r--   0        0        0     1071 1970-01-01 00:00:00.000000 etl_toolkit-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-06-13 18:36:54.087390 etl_toolkit-0.0.2/LICENSE
+-rw-r--r--   0        0        0      126 2023-06-13 18:36:54.087390 etl_toolkit-0.0.2/README.md
+-rw-r--r--   0        0        0     1355 2023-06-13 18:36:54.099390 etl_toolkit-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      341 2023-06-13 18:36:54.099390 etl_toolkit-0.0.2/src/etl/__init__.py
+-rw-r--r--   0        0        0     1271 2023-06-13 18:36:54.099390 etl_toolkit-0.0.2/src/etl/cli/__init__.py
+-rw-r--r--   0        0        0      844 2023-06-13 18:36:54.099390 etl_toolkit-0.0.2/src/etl/cli/app.py
+-rw-r--r--   0        0        0     1220 2023-06-13 18:36:54.099390 etl_toolkit-0.0.2/src/etl/cli/main.py
+-rw-r--r--   0        0        0        0 2023-06-13 18:36:54.099390 etl_toolkit-0.0.2/src/etl/config/__init__.py
+-rw-r--r--   0        0        0     4380 2023-06-13 18:36:54.103390 etl_toolkit-0.0.2/src/etl/config/app.py
+-rw-r--r--   0        0        0      151 2023-06-13 18:36:54.103390 etl_toolkit-0.0.2/src/etl/config/auth_type.py
+-rw-r--r--   0        0        0     3296 2023-06-13 18:36:54.103390 etl_toolkit-0.0.2/src/etl/config/database.py
+-rw-r--r--   0        0        0      443 2023-06-13 18:36:54.103390 etl_toolkit-0.0.2/src/etl/config/settings.py
+-rw-r--r--   0        0        0      684 2023-06-13 18:36:54.103390 etl_toolkit-0.0.2/src/etl/config/yaml.py
+-rw-r--r--   0        0        0      382 2023-06-13 18:36:54.103390 etl_toolkit-0.0.2/src/etl/models/file_parsing_result.py
+-rw-r--r--   0        0        0      309 2023-06-13 18:36:54.103390 etl_toolkit-0.0.2/src/etl/paths.py
+-rw-r--r--   0        0        0     1503 2023-06-13 18:36:54.103390 etl_toolkit-0.0.2/src/etl/pipeline.py
+-rw-r--r--   0        0        0        0 2023-06-13 18:36:54.103390 etl_toolkit-0.0.2/src/etl/py.typed
+-rw-r--r--   0        0        0      138 2023-06-13 18:36:54.103390 etl_toolkit-0.0.2/src/etl/std/__init__.py
+-rw-r--r--   0        0        0      883 2023-06-13 18:36:54.103390 etl_toolkit-0.0.2/src/etl/std/error.py
+-rw-r--r--   0        0        0      334 2023-06-13 18:36:54.103390 etl_toolkit-0.0.2/src/etl/std/error_results.py
+-rw-r--r--   0        0        0      194 2023-06-13 18:36:54.103390 etl_toolkit-0.0.2/src/etl/std/exceptions.py
+-rw-r--r--   0        0        0     2374 2023-06-13 18:36:54.103390 etl_toolkit-0.0.2/src/etl/std/result.py
+-rw-r--r--   0        0        0     1071 1970-01-01 00:00:00.000000 etl_toolkit-0.0.2/PKG-INFO
```

### Comparing `etl_toolkit-0.0.1/LICENSE` & `etl_toolkit-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `etl_toolkit-0.0.1/pyproject.toml` & `etl_toolkit-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "etl-toolkit"
-version = "0.0.1"
+version = "0.0.2"
 description = "ETL CLI Toolkit. Performs common ETL tasks for standard industry and custom files in various formats."
 license = "MIT"
 authors = ["eithery <eithery.pro@gmail.com>"]
 readme = "README.md"
 keywords = ["etl", "file load", "interfaces", "pershing"]
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
```

### Comparing `etl_toolkit-0.0.1/src/etl/cli/__init__.py` & `etl_toolkit-0.0.2/src/etl/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `etl_toolkit-0.0.1/src/etl/cli/app.py` & `etl_toolkit-0.0.2/src/etl/cli/app.py`

 * *Files identical despite different names*

### Comparing `etl_toolkit-0.0.1/src/etl/cli/main.py` & `etl_toolkit-0.0.2/src/etl/cli/main.py`

 * *Files identical despite different names*

### Comparing `etl_toolkit-0.0.1/src/etl/config/app.py` & `etl_toolkit-0.0.2/src/etl/config/app.py`

 * *Files identical despite different names*

### Comparing `etl_toolkit-0.0.1/src/etl/config/database.py` & `etl_toolkit-0.0.2/src/etl/config/database.py`

 * *Files identical despite different names*

### Comparing `etl_toolkit-0.0.1/src/etl/config/yaml.py` & `etl_toolkit-0.0.2/src/etl/config/yaml.py`

 * *Files identical despite different names*

### Comparing `etl_toolkit-0.0.1/src/etl/pipeline.py` & `etl_toolkit-0.0.2/src/etl/pipeline.py`

 * *Files identical despite different names*

### Comparing `etl_toolkit-0.0.1/src/etl/std/error.py` & `etl_toolkit-0.0.2/src/etl/std/error.py`

 * *Files identical despite different names*

### Comparing `etl_toolkit-0.0.1/src/etl/std/result.py` & `etl_toolkit-0.0.2/src/etl/std/result.py`

 * *Files identical despite different names*

### Comparing `etl_toolkit-0.0.1/PKG-INFO` & `etl_toolkit-0.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etl-toolkit
-Version: 0.0.1
+Version: 0.0.2
 Summary: ETL CLI Toolkit. Performs common ETL tasks for standard industry and custom files in various formats.
 License: MIT
 Keywords: etl,file load,interfaces,pershing
 Author: eithery
 Author-email: eithery.pro@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

