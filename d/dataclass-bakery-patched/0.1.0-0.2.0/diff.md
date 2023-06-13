# Comparing `tmp/dataclass_bakery_patched-0.1.0.tar.gz` & `tmp/dataclass_bakery_patched-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataclass_bakery_patched-0.1.0.tar", max compression
+gzip compressed data, was "dataclass_bakery_patched-0.2.0.tar", max compression
```

## Comparing `dataclass_bakery_patched-0.1.0.tar` & `dataclass_bakery_patched-0.2.0.tar`

### file list

```diff
@@ -1,45 +1,25 @@
--rw-r--r--   0        0        0    11558 2023-06-13 08:43:13.449996 dataclass_bakery_patched-0.1.0/LICENSE
--rw-r--r--   0        0        0      518 2023-06-13 10:32:46.001385 dataclass_bakery_patched-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1218 2023-06-13 08:43:13.451303 dataclass_bakery_patched-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-06-13 08:43:13.493926 dataclass_bakery_patched-0.1.0/src/dataclass_bakery/__init__.py
--rw-r--r--   0        0        0      691 2023-06-13 08:43:13.493926 dataclass_bakery_patched-0.1.0/src/dataclass_bakery/baker.py
--rw-r--r--   0        0        0        0 2023-06-13 08:43:13.493926 dataclass_bakery_patched-0.1.0/src/dataclass_bakery/generators/__init__.py
--rw-r--r--   0        0        0     2868 2023-06-13 08:43:13.495241 dataclass_bakery_patched-0.1.0/src/dataclass_bakery/generators/defaults.py
--rw-r--r--   0        0        0      145 2023-06-13 08:43:13.495241 dataclass_bakery_patched-0.1.0/src/dataclass_bakery/generators/generators_exceptions.py
--rw-r--r--   0        0        0      326 2023-06-13 08:43:13.496524 dataclass_bakery_patched-0.1.0/src/dataclass_bakery/generators/random_bool_generator.py
--rw-r--r--   0        0        0      876 2023-06-13 08:43:13.496524 dataclass_bakery_patched-0.1.0/src/dataclass_bakery/generators/random_complex_generator.py
--rw-r--r--   0        0        0     3072 2023-06-13 10:21:54.299061 dataclass_bakery_patched-0.1.0/src/dataclass_bakery/generators/random_data_class_generator.py
--rw-r--r--   0        0        0      796 2023-06-13 08:43:13.497964 dataclass_bakery_patched-0.1.0/src/dataclass_bakery/generators/random_decimal_generator.py
--rw-r--r--   0        0        0     1796 2023-06-13 08:43:13.499432 dataclass_bakery_patched-0.1.0/src/dataclass_bakery/generators/random_dict_generator.py
--rw-r--r--   0        0        0      708 2023-06-13 08:43:13.499432 dataclass_bakery_patched-0.1.0/src/dataclass_bakery/generators/random_float_generator.py
--rw-r--r--   0        0        0      178 2023-06-13 08:43:13.499432 dataclass_bakery_patched-0.1.0/src/dataclass_bakery/generators/random_generator.py
--rw-r--r--   0        0        0      571 2023-06-13 08:43:13.500705 dataclass_bakery_patched-0.1.0/src/dataclass_bakery/generators/random_int_generator.py
--rw-r--r--   0        0        0     1195 2023-06-13 08:43:13.500705 dataclass_bakery_patched-0.1.0/src/dataclass_bakery/generators/random_list_generator.py
--rw-r--r--   0        0        0      546 2023-06-13 08:43:13.501776 dataclass_bakery_patched-0.1.0/src/dataclass_bakery/generators/random_option_generator.py
--rw-r--r--   0        0        0      612 2023-06-13 08:43:13.501776 dataclass_bakery_patched-0.1.0/src/dataclass_bakery/generators/random_path_generator.py
--rw-r--r--   0        0        0      681 2023-06-13 08:43:13.503015 dataclass_bakery_patched-0.1.0/src/dataclass_bakery/generators/random_range_generator.py
--rw-r--r--   0        0        0      810 2023-06-13 08:43:13.503015 dataclass_bakery_patched-0.1.0/src/dataclass_bakery/generators/random_set_generator.py
--rw-r--r--   0        0        0      596 2023-06-13 08:43:13.504423 dataclass_bakery_patched-0.1.0/src/dataclass_bakery/generators/random_str_generator.py
--rw-r--r--   0        0        0     1210 2023-06-13 08:43:13.505433 dataclass_bakery_patched-0.1.0/src/dataclass_bakery/generators/random_tuple_generator.py
--rw-r--r--   0        0        0      277 2023-06-13 08:43:13.505433 dataclass_bakery_patched-0.1.0/src/dataclass_bakery/generators/random_uuid_generator.py
--rw-r--r--   0        0        0        0 2023-06-13 08:43:13.506450 dataclass_bakery_patched-0.1.0/src/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-06-13 08:43:13.506450 dataclass_bakery_patched-0.1.0/src/tests/dataclass_bakery/__init__.py
--rw-r--r--   0        0        0        0 2023-06-13 08:43:13.507448 dataclass_bakery_patched-0.1.0/src/tests/dataclass_bakery/generators/__init__.py
--rw-r--r--   0        0        0      395 2023-06-13 08:43:13.507448 dataclass_bakery_patched-0.1.0/src/tests/dataclass_bakery/generators/test_random_bool_generator.py
--rw-r--r--   0        0        0     1903 2023-06-13 08:43:13.508445 dataclass_bakery_patched-0.1.0/src/tests/dataclass_bakery/generators/test_random_complex_generator.py
--rw-r--r--   0        0        0     4745 2023-06-13 10:21:19.540227 dataclass_bakery_patched-0.1.0/src/tests/dataclass_bakery/generators/test_random_data_class_generator.py
--rw-r--r--   0        0        0     1746 2023-06-13 08:43:13.509877 dataclass_bakery_patched-0.1.0/src/tests/dataclass_bakery/generators/test_random_decimal_generator.py
--rw-r--r--   0        0        0     2620 2023-06-13 08:43:13.510985 dataclass_bakery_patched-0.1.0/src/tests/dataclass_bakery/generators/test_random_dict_generator.py
--rw-r--r--   0        0        0     1665 2023-06-13 08:43:13.510985 dataclass_bakery_patched-0.1.0/src/tests/dataclass_bakery/generators/test_random_float_generator.py
--rw-r--r--   0        0        0     1550 2023-06-13 08:43:13.512159 dataclass_bakery_patched-0.1.0/src/tests/dataclass_bakery/generators/test_random_int_generator.py
--rw-r--r--   0        0        0     1722 2023-06-13 08:43:13.512159 dataclass_bakery_patched-0.1.0/src/tests/dataclass_bakery/generators/test_random_list_generator.py
--rw-r--r--   0        0        0      569 2023-06-13 08:43:13.513224 dataclass_bakery_patched-0.1.0/src/tests/dataclass_bakery/generators/test_random_option_generator.py
--rw-r--r--   0        0        0     1171 2023-06-13 08:43:13.513224 dataclass_bakery_patched-0.1.0/src/tests/dataclass_bakery/generators/test_random_path_generator.py
--rw-r--r--   0        0        0     1844 2023-06-13 08:43:13.513224 dataclass_bakery_patched-0.1.0/src/tests/dataclass_bakery/generators/test_random_range_generator.py
--rw-r--r--   0        0        0     1704 2023-06-13 08:43:13.514267 dataclass_bakery_patched-0.1.0/src/tests/dataclass_bakery/generators/test_random_set_generator.py
--rw-r--r--   0        0        0      931 2023-06-13 08:43:13.514267 dataclass_bakery_patched-0.1.0/src/tests/dataclass_bakery/generators/test_random_str_generator.py
--rw-r--r--   0        0        0     1751 2023-06-13 08:43:13.515325 dataclass_bakery_patched-0.1.0/src/tests/dataclass_bakery/generators/test_random_tuple_generator.py
--rw-r--r--   0        0        0      418 2023-06-13 08:43:13.515325 dataclass_bakery_patched-0.1.0/src/tests/dataclass_bakery/generators/test_random_uuid_generator.py
--rw-r--r--   0        0        0      893 2023-06-13 08:43:13.516431 dataclass_bakery_patched-0.1.0/src/tests/dataclass_bakery/test_baker.py
--rw-r--r--   0        0        0      678 2023-06-13 08:43:13.516431 dataclass_bakery_patched-0.1.0/src/tests/testing_dataclasses.py
--rw-r--r--   0        0        0     1559 1970-01-01 00:00:00.000000 dataclass_bakery_patched-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-13 08:43:13.493926 dataclass_bakery_patched-0.2.0/dataclass-bakery-patched/__init__.py
+-rw-r--r--   0        0        0      691 2023-06-13 08:43:13.493926 dataclass_bakery_patched-0.2.0/dataclass-bakery-patched/baker.py
+-rw-r--r--   0        0        0        0 2023-06-13 08:43:13.493926 dataclass_bakery_patched-0.2.0/dataclass-bakery-patched/generators/__init__.py
+-rw-r--r--   0        0        0     2868 2023-06-13 08:43:13.495241 dataclass_bakery_patched-0.2.0/dataclass-bakery-patched/generators/defaults.py
+-rw-r--r--   0        0        0      145 2023-06-13 08:43:13.495241 dataclass_bakery_patched-0.2.0/dataclass-bakery-patched/generators/generators_exceptions.py
+-rw-r--r--   0        0        0      326 2023-06-13 08:43:13.496524 dataclass_bakery_patched-0.2.0/dataclass-bakery-patched/generators/random_bool_generator.py
+-rw-r--r--   0        0        0      876 2023-06-13 08:43:13.496524 dataclass_bakery_patched-0.2.0/dataclass-bakery-patched/generators/random_complex_generator.py
+-rw-r--r--   0        0        0     3072 2023-06-13 10:21:54.299061 dataclass_bakery_patched-0.2.0/dataclass-bakery-patched/generators/random_data_class_generator.py
+-rw-r--r--   0        0        0      796 2023-06-13 08:43:13.497964 dataclass_bakery_patched-0.2.0/dataclass-bakery-patched/generators/random_decimal_generator.py
+-rw-r--r--   0        0        0     1796 2023-06-13 08:43:13.499432 dataclass_bakery_patched-0.2.0/dataclass-bakery-patched/generators/random_dict_generator.py
+-rw-r--r--   0        0        0      708 2023-06-13 08:43:13.499432 dataclass_bakery_patched-0.2.0/dataclass-bakery-patched/generators/random_float_generator.py
+-rw-r--r--   0        0        0      178 2023-06-13 08:43:13.499432 dataclass_bakery_patched-0.2.0/dataclass-bakery-patched/generators/random_generator.py
+-rw-r--r--   0        0        0      571 2023-06-13 08:43:13.500705 dataclass_bakery_patched-0.2.0/dataclass-bakery-patched/generators/random_int_generator.py
+-rw-r--r--   0        0        0     1195 2023-06-13 08:43:13.500705 dataclass_bakery_patched-0.2.0/dataclass-bakery-patched/generators/random_list_generator.py
+-rw-r--r--   0        0        0      546 2023-06-13 08:43:13.501776 dataclass_bakery_patched-0.2.0/dataclass-bakery-patched/generators/random_option_generator.py
+-rw-r--r--   0        0        0      612 2023-06-13 08:43:13.501776 dataclass_bakery_patched-0.2.0/dataclass-bakery-patched/generators/random_path_generator.py
+-rw-r--r--   0        0        0      681 2023-06-13 08:43:13.503015 dataclass_bakery_patched-0.2.0/dataclass-bakery-patched/generators/random_range_generator.py
+-rw-r--r--   0        0        0      810 2023-06-13 08:43:13.503015 dataclass_bakery_patched-0.2.0/dataclass-bakery-patched/generators/random_set_generator.py
+-rw-r--r--   0        0        0      596 2023-06-13 08:43:13.504423 dataclass_bakery_patched-0.2.0/dataclass-bakery-patched/generators/random_str_generator.py
+-rw-r--r--   0        0        0     1210 2023-06-13 08:43:13.505433 dataclass_bakery_patched-0.2.0/dataclass-bakery-patched/generators/random_tuple_generator.py
+-rw-r--r--   0        0        0      277 2023-06-13 08:43:13.505433 dataclass_bakery_patched-0.2.0/dataclass-bakery-patched/generators/random_uuid_generator.py
+-rw-r--r--   0        0        0    11558 2023-06-13 08:43:13.449996 dataclass_bakery_patched-0.2.0/LICENSE
+-rw-r--r--   0        0        0      539 2023-06-13 10:47:00.757265 dataclass_bakery_patched-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1218 2023-06-13 08:43:13.451303 dataclass_bakery_patched-0.2.0/README.md
+-rw-r--r--   0        0        0     1559 1970-01-01 00:00:00.000000 dataclass_bakery_patched-0.2.0/PKG-INFO
```

### Comparing `dataclass_bakery_patched-0.1.0/LICENSE` & `dataclass_bakery_patched-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dataclass_bakery_patched-0.1.0/pyproject.toml` & `dataclass_bakery_patched-0.2.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 name = "dataclass-bakery-patched"
-version = "0.1.0"
+version = "0.2.0"
 description = "A fork from dataclass-bakery, with a tweak to consider inherited attributes when creating dataclasses."
 authors = ["Adam Ruman <469068@muni.cz>"]
 readme = "README.md"
-packages = [{include = "src"}]
+packages = [{include = "dataclass-bakery-patched"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.2"
 black = "^23.3.0"
```

### Comparing `dataclass_bakery_patched-0.1.0/README.md` & `dataclass_bakery_patched-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `dataclass_bakery_patched-0.1.0/src/dataclass_bakery/baker.py` & `dataclass_bakery_patched-0.2.0/dataclass-bakery-patched/baker.py`

 * *Files identical despite different names*

### Comparing `dataclass_bakery_patched-0.1.0/src/dataclass_bakery/generators/defaults.py` & `dataclass_bakery_patched-0.2.0/dataclass-bakery-patched/generators/defaults.py`

 * *Files identical despite different names*

### Comparing `dataclass_bakery_patched-0.1.0/src/dataclass_bakery/generators/random_complex_generator.py` & `dataclass_bakery_patched-0.2.0/dataclass-bakery-patched/generators/random_complex_generator.py`

 * *Files identical despite different names*

### Comparing `dataclass_bakery_patched-0.1.0/src/dataclass_bakery/generators/random_data_class_generator.py` & `dataclass_bakery_patched-0.2.0/dataclass-bakery-patched/generators/random_data_class_generator.py`

 * *Files identical despite different names*

### Comparing `dataclass_bakery_patched-0.1.0/src/dataclass_bakery/generators/random_decimal_generator.py` & `dataclass_bakery_patched-0.2.0/dataclass-bakery-patched/generators/random_decimal_generator.py`

 * *Files identical despite different names*

### Comparing `dataclass_bakery_patched-0.1.0/src/dataclass_bakery/generators/random_dict_generator.py` & `dataclass_bakery_patched-0.2.0/dataclass-bakery-patched/generators/random_dict_generator.py`

 * *Files identical despite different names*

### Comparing `dataclass_bakery_patched-0.1.0/src/dataclass_bakery/generators/random_float_generator.py` & `dataclass_bakery_patched-0.2.0/dataclass-bakery-patched/generators/random_float_generator.py`

 * *Files identical despite different names*

### Comparing `dataclass_bakery_patched-0.1.0/src/dataclass_bakery/generators/random_int_generator.py` & `dataclass_bakery_patched-0.2.0/dataclass-bakery-patched/generators/random_int_generator.py`

 * *Files identical despite different names*

### Comparing `dataclass_bakery_patched-0.1.0/src/dataclass_bakery/generators/random_list_generator.py` & `dataclass_bakery_patched-0.2.0/dataclass-bakery-patched/generators/random_list_generator.py`

 * *Files identical despite different names*

### Comparing `dataclass_bakery_patched-0.1.0/src/dataclass_bakery/generators/random_option_generator.py` & `dataclass_bakery_patched-0.2.0/dataclass-bakery-patched/generators/random_option_generator.py`

 * *Files identical despite different names*

### Comparing `dataclass_bakery_patched-0.1.0/src/dataclass_bakery/generators/random_path_generator.py` & `dataclass_bakery_patched-0.2.0/dataclass-bakery-patched/generators/random_path_generator.py`

 * *Files identical despite different names*

### Comparing `dataclass_bakery_patched-0.1.0/src/dataclass_bakery/generators/random_range_generator.py` & `dataclass_bakery_patched-0.2.0/dataclass-bakery-patched/generators/random_range_generator.py`

 * *Files identical despite different names*

### Comparing `dataclass_bakery_patched-0.1.0/src/dataclass_bakery/generators/random_set_generator.py` & `dataclass_bakery_patched-0.2.0/dataclass-bakery-patched/generators/random_set_generator.py`

 * *Files identical despite different names*

### Comparing `dataclass_bakery_patched-0.1.0/src/dataclass_bakery/generators/random_str_generator.py` & `dataclass_bakery_patched-0.2.0/dataclass-bakery-patched/generators/random_str_generator.py`

 * *Files identical despite different names*

### Comparing `dataclass_bakery_patched-0.1.0/src/dataclass_bakery/generators/random_tuple_generator.py` & `dataclass_bakery_patched-0.2.0/dataclass-bakery-patched/generators/random_tuple_generator.py`

 * *Files identical despite different names*

### Comparing `dataclass_bakery_patched-0.1.0/PKG-INFO` & `dataclass_bakery_patched-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataclass-bakery-patched
-Version: 0.1.0
+Version: 0.2.0
 Summary: A fork from dataclass-bakery, with a tweak to consider inherited attributes when creating dataclasses.
 Author: Adam Ruman
 Author-email: 469068@muni.cz
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
```

