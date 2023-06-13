# Comparing `tmp/py-partiql-parser-0.3.3.tar.gz` & `tmp/py-partiql-parser-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-partiql-parser-0.3.3.tar", last modified: Mon May 29 20:32:37 2023, max compression
+gzip compressed data, was "py-partiql-parser-0.3.4.tar", last modified: Tue Jun 13 20:37:44 2023, max compression
```

## Comparing `py-partiql-parser-0.3.3.tar` & `py-partiql-parser-0.3.4.tar`

### file list

```diff
@@ -1,37 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 20:32:37.674716 py-partiql-parser-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-29 20:32:20.000000 py-partiql-parser-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-05-29 20:32:37.674716 py-partiql-parser-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-05-29 20:32:20.000000 py-partiql-parser-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 20:32:37.670716 py-partiql-parser-0.3.3/py_partiql_parser/
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-29 20:32:20.000000 py-partiql-parser-0.3.3/py_partiql_parser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 20:32:37.674716 py-partiql-parser-0.3.3/py_partiql_parser/_internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 20:32:20.000000 py-partiql-parser-0.3.3/py_partiql_parser/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-05-29 20:32:20.000000 py-partiql-parser-0.3.3/py_partiql_parser/_internal/case_insensitive_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-05-29 20:32:20.000000 py-partiql-parser-0.3.3/py_partiql_parser/_internal/clause_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-29 20:32:20.000000 py-partiql-parser-0.3.3/py_partiql_parser/_internal/csv_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-05-29 20:32:20.000000 py-partiql-parser-0.3.3/py_partiql_parser/_internal/from_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     8488 2023-05-29 20:32:20.000000 py-partiql-parser-0.3.3/py_partiql_parser/_internal/json_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-05-29 20:32:20.000000 py-partiql-parser-0.3.3/py_partiql_parser/_internal/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-05-29 20:32:20.000000 py-partiql-parser-0.3.3/py_partiql_parser/_internal/select_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-05-29 20:32:20.000000 py-partiql-parser-0.3.3/py_partiql_parser/_internal/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-05-29 20:32:20.000000 py-partiql-parser-0.3.3/py_partiql_parser/_internal/where_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 20:32:37.670716 py-partiql-parser-0.3.3/py_partiql_parser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-05-29 20:32:37.000000 py-partiql-parser-0.3.3/py_partiql_parser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-29 20:32:37.000000 py-partiql-parser-0.3.3/py_partiql_parser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 20:32:37.000000 py-partiql-parser-0.3.3/py_partiql_parser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-29 20:32:37.000000 py-partiql-parser-0.3.3/py_partiql_parser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-29 20:32:37.000000 py-partiql-parser-0.3.3/py_partiql_parser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-29 20:32:31.000000 py-partiql-parser-0.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-29 20:32:37.674716 py-partiql-parser-0.3.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 20:32:37.674716 py-partiql-parser-0.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-05-29 20:32:20.000000 py-partiql-parser-0.3.3/tests/test_csv_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-05-29 20:32:20.000000 py-partiql-parser-0.3.3/tests/test_dynamodb_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-05-29 20:32:20.000000 py-partiql-parser-0.3.3/tests/test_from_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-29 20:32:20.000000 py-partiql-parser-0.3.3/tests/test_json_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-05-29 20:32:20.000000 py-partiql-parser-0.3.3/tests/test_json_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-29 20:32:20.000000 py-partiql-parser-0.3.3/tests/test_query_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     6494 2023-05-29 20:32:20.000000 py-partiql-parser-0.3.3/tests/test_s3_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-29 20:32:20.000000 py-partiql-parser-0.3.3/tests/test_select_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-05-29 20:32:20.000000 py-partiql-parser-0.3.3/tests/test_select_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-29 20:32:20.000000 py-partiql-parser-0.3.3/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-05-29 20:32:20.000000 py-partiql-parser-0.3.3/tests/test_where_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:37:44.820882 py-partiql-parser-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-13 20:37:23.000000 py-partiql-parser-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-13 20:37:44.820882 py-partiql-parser-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-06-13 20:37:23.000000 py-partiql-parser-0.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:37:44.816882 py-partiql-parser-0.3.4/py_partiql_parser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-13 20:37:44.000000 py-partiql-parser-0.3.4/py_partiql_parser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-13 20:37:44.000000 py-partiql-parser-0.3.4/py_partiql_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 20:37:44.000000 py-partiql-parser-0.3.4/py_partiql_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-13 20:37:44.000000 py-partiql-parser-0.3.4/py_partiql_parser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-13 20:37:44.000000 py-partiql-parser-0.3.4/py_partiql_parser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-13 20:37:37.000000 py-partiql-parser-0.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-13 20:37:44.820882 py-partiql-parser-0.3.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:37:44.820882 py-partiql-parser-0.3.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-06-13 20:37:23.000000 py-partiql-parser-0.3.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-06-13 20:37:23.000000 py-partiql-parser-0.3.4/tests/test_csv_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-06-13 20:37:23.000000 py-partiql-parser-0.3.4/tests/test_dynamodb_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-06-13 20:37:23.000000 py-partiql-parser-0.3.4/tests/test_from_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-06-13 20:37:23.000000 py-partiql-parser-0.3.4/tests/test_json_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-06-13 20:37:23.000000 py-partiql-parser-0.3.4/tests/test_json_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-06-13 20:37:23.000000 py-partiql-parser-0.3.4/tests/test_query_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6494 2023-06-13 20:37:23.000000 py-partiql-parser-0.3.4/tests/test_s3_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-13 20:37:23.000000 py-partiql-parser-0.3.4/tests/test_select_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-06-13 20:37:23.000000 py-partiql-parser-0.3.4/tests/test_select_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-13 20:37:23.000000 py-partiql-parser-0.3.4/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-06-13 20:37:23.000000 py-partiql-parser-0.3.4/tests/test_where_parser.py
```

### Comparing `py-partiql-parser-0.3.3/LICENSE` & `py-partiql-parser-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.3.3/PKG-INFO` & `py-partiql-parser-0.3.4/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 Metadata-Version: 2.1
 Name: py-partiql-parser
-Version: 0.3.3
+Version: 0.3.4
 Summary: Pure Python PartiQL Parser
 Author-email: Bert Blommers <info@bertblommers.nl>
 License: MIT
+Project-URL: Homepage, https://github.com/getmoto/py-partiql-parser
+Project-URL: Bug Tracker, https://github.com/getmoto/py-partiql-parser/issues
+Project-URL: ChangeLog, https://github.com/getmoto/py-partiql-parser/blob/main/CHANGELOG.md
 Keywords: pypartiql,parser
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # py-partiql-parser
 A tokenizer/parser/executor for the PartiQL-language, in Python.
```

### Comparing `py-partiql-parser-0.3.3/README.md` & `py-partiql-parser-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.3.3/py_partiql_parser.egg-info/PKG-INFO` & `py-partiql-parser-0.3.4/py_partiql_parser.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 Metadata-Version: 2.1
 Name: py-partiql-parser
-Version: 0.3.3
+Version: 0.3.4
 Summary: Pure Python PartiQL Parser
 Author-email: Bert Blommers <info@bertblommers.nl>
 License: MIT
+Project-URL: Homepage, https://github.com/getmoto/py-partiql-parser
+Project-URL: Bug Tracker, https://github.com/getmoto/py-partiql-parser/issues
+Project-URL: ChangeLog, https://github.com/getmoto/py-partiql-parser/blob/main/CHANGELOG.md
 Keywords: pypartiql,parser
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # py-partiql-parser
 A tokenizer/parser/executor for the PartiQL-language, in Python.
```

### Comparing `py-partiql-parser-0.3.3/tests/test_csv_converter.py` & `py-partiql-parser-0.3.4/tests/test_csv_converter.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.3.3/tests/test_dynamodb_examples.py` & `py-partiql-parser-0.3.4/tests/test_dynamodb_examples.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.3.3/tests/test_from_parser.py` & `py-partiql-parser-0.3.4/tests/test_from_parser.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.3.3/tests/test_json_encoder.py` & `py-partiql-parser-0.3.4/tests/test_json_encoder.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.3.3/tests/test_json_parser.py` & `py-partiql-parser-0.3.4/tests/test_json_parser.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.3.3/tests/test_query_metadata.py` & `py-partiql-parser-0.3.4/tests/test_query_metadata.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.3.3/tests/test_s3_examples.py` & `py-partiql-parser-0.3.4/tests/test_s3_examples.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.3.3/tests/test_select_functions.py` & `py-partiql-parser-0.3.4/tests/test_select_functions.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.3.3/tests/test_select_parser.py` & `py-partiql-parser-0.3.4/tests/test_select_parser.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.3.3/tests/test_utils.py` & `py-partiql-parser-0.3.4/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.3.3/tests/test_where_parser.py` & `py-partiql-parser-0.3.4/tests/test_where_parser.py`

 * *Files identical despite different names*

