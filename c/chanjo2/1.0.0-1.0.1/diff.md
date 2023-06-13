# Comparing `tmp/chanjo2-1.0.0.tar.gz` & `tmp/chanjo2-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chanjo2-1.0.0.tar", max compression
+gzip compressed data, was "chanjo2-1.0.1.tar", max compression
```

## Comparing `chanjo2-1.0.0.tar` & `chanjo2-1.0.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      729 2023-06-12 11:23:58.810682 chanjo2-1.0.0/pyproject.toml
--rw-r--r--   0        0        0       68 2023-06-12 11:23:58.810682 chanjo2-1.0.0/src/chanjo2/__init__.py
--rw-r--r--   0        0        0     3099 2023-06-12 11:23:58.810682 chanjo2-1.0.0/src/chanjo2/constants.py
--rw-r--r--   0        0        0     2743 2023-06-12 11:23:58.810682 chanjo2-1.0.0/src/chanjo2/crud/cases.py
--rw-r--r--   0        0        0     5309 2023-06-12 11:23:58.810682 chanjo2-1.0.0/src/chanjo2/crud/intervals.py
--rw-r--r--   0        0        0     3110 2023-06-12 11:23:58.810682 chanjo2-1.0.0/src/chanjo2/crud/samples.py
--rw-r--r--   0        0        0     1067 2023-06-12 11:23:58.810682 chanjo2-1.0.0/src/chanjo2/dbutil.py
--rw-r--r--   0        0        0      346 2023-06-12 11:23:58.810682 chanjo2-1.0.0/src/chanjo2/demo/109_green.bed
--rw-r--r--   0        0        0      292 2023-06-12 11:23:58.810682 chanjo2-1.0.0/src/chanjo2/demo/__init__.py
--rw-r--r--   0        0        0   450444 2023-06-12 11:23:58.810682 chanjo2-1.0.0/src/chanjo2/demo/panelapp_109_example.d4
--rw-r--r--   0        0        0        0 2023-06-12 11:23:58.810682 chanjo2-1.0.0/src/chanjo2/endpoints/__init__.py
--rw-r--r--   0        0        0     1588 2023-06-12 11:23:58.810682 chanjo2-1.0.0/src/chanjo2/endpoints/cases.py
--rw-r--r--   0        0        0     6649 2023-06-12 11:23:58.810682 chanjo2-1.0.0/src/chanjo2/endpoints/coverage.py
--rw-r--r--   0        0        0     5278 2023-06-12 11:23:58.810682 chanjo2-1.0.0/src/chanjo2/endpoints/intervals.py
--rw-r--r--   0        0        0     2018 2023-06-12 11:23:58.810682 chanjo2-1.0.0/src/chanjo2/endpoints/samples.py
--rw-r--r--   0        0        0     1690 2023-06-12 11:23:58.810682 chanjo2-1.0.0/src/chanjo2/main.py
--rw-r--r--   0        0        0        0 2023-06-12 11:23:58.810682 chanjo2-1.0.0/src/chanjo2/meta/__init__.py
--rw-r--r--   0        0        0      694 2023-06-12 11:23:58.810682 chanjo2-1.0.0/src/chanjo2/meta/handle_bed.py
--rw-r--r--   0        0        0     6816 2023-06-12 11:23:58.810682 chanjo2-1.0.0/src/chanjo2/meta/handle_d4.py
--rw-r--r--   0        0        0     7707 2023-06-12 11:23:58.810682 chanjo2-1.0.0/src/chanjo2/meta/handle_load_intervals.py
--rw-r--r--   0        0        0        0 2023-06-12 11:23:58.810682 chanjo2-1.0.0/src/chanjo2/meta/handle_query_intervals.py
--rw-r--r--   0        0        0        0 2023-06-12 11:23:58.810682 chanjo2-1.0.0/src/chanjo2/models/__init__.py
--rw-r--r--   0        0        0     3913 2023-06-12 11:23:58.810682 chanjo2-1.0.0/src/chanjo2/models/pydantic_models.py
--rw-r--r--   0        0        0     4360 2023-06-12 11:23:58.810682 chanjo2-1.0.0/src/chanjo2/models/sql_models.py
--rw-r--r--   0        0        0     2999 2023-06-12 11:23:58.810682 chanjo2-1.0.0/src/chanjo2/populate_demo.py
--rw-r--r--   0        0        0     1061 1970-01-01 00:00:00.000000 chanjo2-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      734 2023-06-13 08:09:50.153914 chanjo2-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0       68 2023-06-13 08:09:50.153914 chanjo2-1.0.1/src/chanjo2/__init__.py
+-rw-r--r--   0        0        0     3099 2023-06-13 08:09:50.153914 chanjo2-1.0.1/src/chanjo2/constants.py
+-rw-r--r--   0        0        0     2743 2023-06-13 08:09:50.153914 chanjo2-1.0.1/src/chanjo2/crud/cases.py
+-rw-r--r--   0        0        0     5309 2023-06-13 08:09:50.153914 chanjo2-1.0.1/src/chanjo2/crud/intervals.py
+-rw-r--r--   0        0        0     3110 2023-06-13 08:09:50.153914 chanjo2-1.0.1/src/chanjo2/crud/samples.py
+-rw-r--r--   0        0        0     1067 2023-06-13 08:09:50.153914 chanjo2-1.0.1/src/chanjo2/dbutil.py
+-rw-r--r--   0        0        0      346 2023-06-13 08:09:50.153914 chanjo2-1.0.1/src/chanjo2/demo/109_green.bed
+-rw-r--r--   0        0        0      292 2023-06-13 08:09:50.153914 chanjo2-1.0.1/src/chanjo2/demo/__init__.py
+-rw-r--r--   0        0        0   450444 2023-06-13 08:09:50.157914 chanjo2-1.0.1/src/chanjo2/demo/panelapp_109_example.d4
+-rw-r--r--   0        0        0        0 2023-06-13 08:09:50.157914 chanjo2-1.0.1/src/chanjo2/endpoints/__init__.py
+-rw-r--r--   0        0        0     1588 2023-06-13 08:09:50.157914 chanjo2-1.0.1/src/chanjo2/endpoints/cases.py
+-rw-r--r--   0        0        0     6649 2023-06-13 08:09:50.157914 chanjo2-1.0.1/src/chanjo2/endpoints/coverage.py
+-rw-r--r--   0        0        0     5278 2023-06-13 08:09:50.157914 chanjo2-1.0.1/src/chanjo2/endpoints/intervals.py
+-rw-r--r--   0        0        0     2018 2023-06-13 08:09:50.157914 chanjo2-1.0.1/src/chanjo2/endpoints/samples.py
+-rw-r--r--   0        0        0     1690 2023-06-13 08:09:50.157914 chanjo2-1.0.1/src/chanjo2/main.py
+-rw-r--r--   0        0        0        0 2023-06-13 08:09:50.157914 chanjo2-1.0.1/src/chanjo2/meta/__init__.py
+-rw-r--r--   0        0        0      694 2023-06-13 08:09:50.157914 chanjo2-1.0.1/src/chanjo2/meta/handle_bed.py
+-rw-r--r--   0        0        0     6816 2023-06-13 08:09:50.157914 chanjo2-1.0.1/src/chanjo2/meta/handle_d4.py
+-rw-r--r--   0        0        0     7707 2023-06-13 08:09:50.157914 chanjo2-1.0.1/src/chanjo2/meta/handle_load_intervals.py
+-rw-r--r--   0        0        0        0 2023-06-13 08:09:50.157914 chanjo2-1.0.1/src/chanjo2/meta/handle_query_intervals.py
+-rw-r--r--   0        0        0        0 2023-06-13 08:09:50.157914 chanjo2-1.0.1/src/chanjo2/models/__init__.py
+-rw-r--r--   0        0        0     3913 2023-06-13 08:09:50.157914 chanjo2-1.0.1/src/chanjo2/models/pydantic_models.py
+-rw-r--r--   0        0        0     4360 2023-06-13 08:09:50.157914 chanjo2-1.0.1/src/chanjo2/models/sql_models.py
+-rw-r--r--   0        0        0     2999 2023-06-13 08:09:50.157914 chanjo2-1.0.1/src/chanjo2/populate_demo.py
+-rw-r--r--   0        0        0     1066 1970-01-01 00:00:00.000000 chanjo2-1.0.1/PKG-INFO
```

### Comparing `chanjo2-1.0.0/pyproject.toml` & `chanjo2-1.0.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "chanjo2"
-version = "1.0.0"
+version = "1.0.1"
 description = "Next generation coverage analysis"
-authors = ["moonso <mans.magnusson@scilifelab.se>"]
+authors = ["northwestwitch <chiara.rasi@scilifelab.se>"]
 
 [tool.poetry_bumpversion.file."src/chanjo2/__init__.py"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 fastapi = "^0.68.1"
 sqlmodel = "^0.0.4"
```

### Comparing `chanjo2-1.0.0/src/chanjo2/constants.py` & `chanjo2-1.0.1/src/chanjo2/constants.py`

 * *Files identical despite different names*

### Comparing `chanjo2-1.0.0/src/chanjo2/crud/cases.py` & `chanjo2-1.0.1/src/chanjo2/crud/cases.py`

 * *Files identical despite different names*

### Comparing `chanjo2-1.0.0/src/chanjo2/crud/intervals.py` & `chanjo2-1.0.1/src/chanjo2/crud/intervals.py`

 * *Files identical despite different names*

### Comparing `chanjo2-1.0.0/src/chanjo2/crud/samples.py` & `chanjo2-1.0.1/src/chanjo2/crud/samples.py`

 * *Files identical despite different names*

### Comparing `chanjo2-1.0.0/src/chanjo2/dbutil.py` & `chanjo2-1.0.1/src/chanjo2/dbutil.py`

 * *Files identical despite different names*

### Comparing `chanjo2-1.0.0/src/chanjo2/demo/panelapp_109_example.d4` & `chanjo2-1.0.1/src/chanjo2/demo/panelapp_109_example.d4`

 * *Files identical despite different names*

### Comparing `chanjo2-1.0.0/src/chanjo2/endpoints/cases.py` & `chanjo2-1.0.1/src/chanjo2/endpoints/cases.py`

 * *Files identical despite different names*

### Comparing `chanjo2-1.0.0/src/chanjo2/endpoints/coverage.py` & `chanjo2-1.0.1/src/chanjo2/endpoints/coverage.py`

 * *Files identical despite different names*

### Comparing `chanjo2-1.0.0/src/chanjo2/endpoints/intervals.py` & `chanjo2-1.0.1/src/chanjo2/endpoints/intervals.py`

 * *Files identical despite different names*

### Comparing `chanjo2-1.0.0/src/chanjo2/endpoints/samples.py` & `chanjo2-1.0.1/src/chanjo2/endpoints/samples.py`

 * *Files identical despite different names*

### Comparing `chanjo2-1.0.0/src/chanjo2/main.py` & `chanjo2-1.0.1/src/chanjo2/main.py`

 * *Files identical despite different names*

### Comparing `chanjo2-1.0.0/src/chanjo2/meta/handle_bed.py` & `chanjo2-1.0.1/src/chanjo2/meta/handle_bed.py`

 * *Files identical despite different names*

### Comparing `chanjo2-1.0.0/src/chanjo2/meta/handle_d4.py` & `chanjo2-1.0.1/src/chanjo2/meta/handle_d4.py`

 * *Files identical despite different names*

### Comparing `chanjo2-1.0.0/src/chanjo2/meta/handle_load_intervals.py` & `chanjo2-1.0.1/src/chanjo2/meta/handle_load_intervals.py`

 * *Files identical despite different names*

### Comparing `chanjo2-1.0.0/src/chanjo2/models/pydantic_models.py` & `chanjo2-1.0.1/src/chanjo2/models/pydantic_models.py`

 * *Files identical despite different names*

### Comparing `chanjo2-1.0.0/src/chanjo2/models/sql_models.py` & `chanjo2-1.0.1/src/chanjo2/models/sql_models.py`

 * *Files identical despite different names*

### Comparing `chanjo2-1.0.0/src/chanjo2/populate_demo.py` & `chanjo2-1.0.1/src/chanjo2/populate_demo.py`

 * *Files identical despite different names*

### Comparing `chanjo2-1.0.0/PKG-INFO` & `chanjo2-1.0.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: chanjo2
-Version: 1.0.0
+Version: 1.0.1
 Summary: Next generation coverage analysis
-Author: moonso
-Author-email: mans.magnusson@scilifelab.se
+Author: northwestwitch
+Author-email: chiara.rasi@scilifelab.se
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: m1
```

