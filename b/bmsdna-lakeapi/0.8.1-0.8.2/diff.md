# Comparing `tmp/bmsdna_lakeapi-0.8.1.tar.gz` & `tmp/bmsdna_lakeapi-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmsdna_lakeapi-0.8.1.tar", max compression
+gzip compressed data, was "bmsdna_lakeapi-0.8.2.tar", max compression
```

## Comparing `bmsdna_lakeapi-0.8.1.tar` & `bmsdna_lakeapi-0.8.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1081 2023-06-12 15:09:21.787349 bmsdna_lakeapi-0.8.1/LICENSE
--rw-r--r--   0        0        0     8929 2023-06-12 15:09:21.787349 bmsdna_lakeapi-0.8.1/README.md
--rw-r--r--   0        0        0      337 2023-06-12 15:09:21.787349 bmsdna_lakeapi-0.8.1/bmsdna/lakeapi/__init__.py
--rw-r--r--   0        0        0        0 2023-06-12 15:09:21.787349 bmsdna_lakeapi-0.8.1/bmsdna/lakeapi/api/__init__.py
--rw-r--r--   0        0        0     1185 2023-06-12 15:09:21.787349 bmsdna_lakeapi-0.8.1/bmsdna/lakeapi/api/api.py
--rw-r--r--   0        0        0      566 2023-06-12 15:09:21.787349 bmsdna_lakeapi-0.8.1/bmsdna/lakeapi/context/__init__.py
--rw-r--r--   0        0        0     6876 2023-06-12 15:09:21.787349 bmsdna_lakeapi-0.8.1/bmsdna/lakeapi/context/df_base.py
--rw-r--r--   0        0        0    10471 2023-06-12 15:09:21.791349 bmsdna_lakeapi-0.8.1/bmsdna/lakeapi/context/df_duckdb.py
--rw-r--r--   0        0        0     6091 2023-06-12 15:09:21.791349 bmsdna_lakeapi-0.8.1/bmsdna/lakeapi/context/df_polars.py
--rw-r--r--   0        0        0        0 2023-06-12 15:09:21.791349 bmsdna_lakeapi-0.8.1/bmsdna/lakeapi/core/__init__.py
--rw-r--r--   0        0        0    11077 2023-06-12 15:09:21.791349 bmsdna_lakeapi-0.8.1/bmsdna/lakeapi/core/config.py
--rw-r--r--   0        0        0    12618 2023-06-12 15:09:21.791349 bmsdna_lakeapi-0.8.1/bmsdna/lakeapi/core/dataframe.py
--rw-r--r--   0        0        0    15585 2023-06-12 15:09:21.791349 bmsdna_lakeapi-0.8.1/bmsdna/lakeapi/core/endpoint.py
--rw-r--r--   0        0        0      187 2023-06-12 15:09:21.791349 bmsdna_lakeapi-0.8.1/bmsdna/lakeapi/core/env.py
--rw-r--r--   0        0        0     1012 2023-06-12 15:09:21.791349 bmsdna_lakeapi-0.8.1/bmsdna/lakeapi/core/log.py
--rw-r--r--   0        0        0     6887 2023-06-12 15:09:21.791349 bmsdna_lakeapi-0.8.1/bmsdna/lakeapi/core/model.py
--rw-r--r--   0        0        0     1479 2023-06-12 15:09:21.791349 bmsdna_lakeapi-0.8.1/bmsdna/lakeapi/core/partition_utils.py
--rw-r--r--   0        0        0     6763 2023-06-12 15:09:21.791349 bmsdna_lakeapi-0.8.1/bmsdna/lakeapi/core/response.py
--rw-r--r--   0        0        0     4291 2023-06-12 15:09:21.791349 bmsdna_lakeapi-0.8.1/bmsdna/lakeapi/core/route.py
--rw-r--r--   0        0        0     3763 2023-06-12 15:09:21.791349 bmsdna_lakeapi-0.8.1/bmsdna/lakeapi/core/sql_endpoint.py
--rw-r--r--   0        0        0     3109 2023-06-12 15:09:21.791349 bmsdna_lakeapi-0.8.1/bmsdna/lakeapi/core/types.py
--rw-r--r--   0        0        0     2478 2023-06-12 15:09:21.791349 bmsdna_lakeapi-0.8.1/bmsdna/lakeapi/core/uservalidation.py
--rw-r--r--   0        0        0      215 2023-06-12 15:09:21.791349 bmsdna_lakeapi-0.8.1/bmsdna/lakeapi/core/yaml.py
--rw-r--r--   0        0        0        0 2023-06-12 15:09:21.791349 bmsdna_lakeapi-0.8.1/bmsdna/lakeapi/polars_extensions/__init__.py
--rw-r--r--   0        0        0     1847 2023-06-12 15:09:21.791349 bmsdna_lakeapi-0.8.1/bmsdna/lakeapi/polars_extensions/delta.py
--rw-r--r--   0        0        0      339 2023-06-12 15:09:21.791349 bmsdna_lakeapi-0.8.1/bmsdna/lakeapi/standalone/__init__.py
--rw-r--r--   0        0        0     1790 2023-06-12 15:09:21.791349 bmsdna_lakeapi-0.8.1/bmsdna/lakeapi/tools/useradd.py
--rw-r--r--   0        0        0     1095 2023-06-12 15:09:21.791349 bmsdna_lakeapi-0.8.1/bmsdna/lakeapi/tools/validateschema.py
--rw-r--r--   0        0        0     3535 2023-06-12 15:09:21.791349 bmsdna_lakeapi-0.8.1/bmsdna/lakeapi/utils/fast_api_utils.py
--rw-r--r--   0        0        0     1999 2023-06-12 15:09:21.791349 bmsdna_lakeapi-0.8.1/pyproject.toml
--rw-r--r--   0        0        0    10127 1970-01-01 00:00:00.000000 bmsdna_lakeapi-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-06-13 04:48:33.999102 bmsdna_lakeapi-0.8.2/LICENSE
+-rw-r--r--   0        0        0     8929 2023-06-13 04:48:33.999102 bmsdna_lakeapi-0.8.2/README.md
+-rw-r--r--   0        0        0      337 2023-06-13 04:48:33.999102 bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-13 04:48:33.999102 bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/api/__init__.py
+-rw-r--r--   0        0        0     1185 2023-06-13 04:48:33.999102 bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/api/api.py
+-rw-r--r--   0        0        0      566 2023-06-13 04:48:33.999102 bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/context/__init__.py
+-rw-r--r--   0        0        0     6876 2023-06-13 04:48:33.999102 bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/context/df_base.py
+-rw-r--r--   0        0        0    10460 2023-06-13 04:48:33.999102 bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/context/df_duckdb.py
+-rw-r--r--   0        0        0     6091 2023-06-13 04:48:33.999102 bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/context/df_polars.py
+-rw-r--r--   0        0        0        0 2023-06-13 04:48:33.999102 bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/core/__init__.py
+-rw-r--r--   0        0        0    11077 2023-06-13 04:48:34.003102 bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/core/config.py
+-rw-r--r--   0        0        0    12618 2023-06-13 04:48:34.003102 bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/core/dataframe.py
+-rw-r--r--   0        0        0    15585 2023-06-13 04:48:34.003102 bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/core/endpoint.py
+-rw-r--r--   0        0        0      187 2023-06-13 04:48:34.003102 bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/core/env.py
+-rw-r--r--   0        0        0     1012 2023-06-13 04:48:34.003102 bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/core/log.py
+-rw-r--r--   0        0        0     6887 2023-06-13 04:48:34.003102 bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/core/model.py
+-rw-r--r--   0        0        0     1479 2023-06-13 04:48:34.003102 bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/core/partition_utils.py
+-rw-r--r--   0        0        0     6763 2023-06-13 04:48:34.003102 bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/core/response.py
+-rw-r--r--   0        0        0     4291 2023-06-13 04:48:34.003102 bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/core/route.py
+-rw-r--r--   0        0        0     3763 2023-06-13 04:48:34.003102 bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/core/sql_endpoint.py
+-rw-r--r--   0        0        0     3109 2023-06-13 04:48:34.003102 bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/core/types.py
+-rw-r--r--   0        0        0     2478 2023-06-13 04:48:34.003102 bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/core/uservalidation.py
+-rw-r--r--   0        0        0      215 2023-06-13 04:48:34.003102 bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/core/yaml.py
+-rw-r--r--   0        0        0        0 2023-06-13 04:48:34.003102 bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/polars_extensions/__init__.py
+-rw-r--r--   0        0        0     1847 2023-06-13 04:48:34.003102 bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/polars_extensions/delta.py
+-rw-r--r--   0        0        0      339 2023-06-13 04:48:34.003102 bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/standalone/__init__.py
+-rw-r--r--   0        0        0     1790 2023-06-13 04:48:34.003102 bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/tools/useradd.py
+-rw-r--r--   0        0        0     1095 2023-06-13 04:48:34.003102 bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/tools/validateschema.py
+-rw-r--r--   0        0        0     3535 2023-06-13 04:48:34.003102 bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/utils/fast_api_utils.py
+-rw-r--r--   0        0        0     1999 2023-06-13 04:48:34.003102 bmsdna_lakeapi-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0    10127 1970-01-01 00:00:00.000000 bmsdna_lakeapi-0.8.2/PKG-INFO
```

### Comparing `bmsdna_lakeapi-0.8.1/LICENSE` & `bmsdna_lakeapi-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.8.1/README.md` & `bmsdna_lakeapi-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.8.1/bmsdna/lakeapi/api/api.py` & `bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/api/api.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.8.1/bmsdna/lakeapi/context/__init__.py` & `bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/context/__init__.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.8.1/bmsdna/lakeapi/context/df_base.py` & `bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/context/df_base.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.8.1/bmsdna/lakeapi/context/df_duckdb.py` & `bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/context/df_duckdb.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,18 +13,20 @@
 import pypika.enums
 import pypika
 import os
 from datetime import datetime, timezone
 from bmsdna.lakeapi.core.config import SearchConfig
 from uuid import uuid4
 
-ENABLE_COPY_TO = os.environ.get("ENABLE_COPY_TO", "1") == "1"
+ENABLE_COPY_TO = os.environ.get("ENABLE_COPY_TO", "0") == "1"
+
 
 def _get_temp_table_name():
-    return "temp_" + str(uuid4()).replace("-","")
+    return "temp_" + str(uuid4()).replace("-", "")
+
 
 class DuckDBResultData(ResultData):
     def __init__(
         self,
         original_sql: Union[pypika.queries.QueryBuilder, str],
         con: duckdb.DuckDBPyConnection,
     ) -> None:
@@ -76,23 +78,23 @@
         if not ENABLE_COPY_TO:
             return super().write_nd_json(file_name)
         query = get_sql(self.original_sql)
         uuidstr = _get_temp_table_name()
         full_query = f"CREATE TEMP VIEW {uuidstr} AS {query}; COPY (SELECT *FROM {uuidstr}) TO '{file_name}' (FORMAT JSON); DROP VIEW {uuidstr}"
         self.con.execute(full_query)
 
-    def write_csv(self, file_name: str, *, separator: str):        
+    def write_csv(self, file_name: str, *, separator: str):
         if not ENABLE_COPY_TO:
             return super().write_csv(file_name, separator=separator)
         query = get_sql(self.original_sql)
         uuidstr = _get_temp_table_name()
         full_query = f"CREATE TEMP VIEW {uuidstr} AS {query};  COPY (SELECT *FROM {uuidstr}) TO '{file_name}' (FORMAT CSV, delim '{separator}', header True); DROP VIEW {uuidstr}"
         self.con.execute(full_query)
 
-    def write_json(self, file_name: str):        
+    def write_json(self, file_name: str):
         if not ENABLE_COPY_TO:
             return super().write_json(file_name)
         query = get_sql(self.original_sql)
         uuidstr = _get_temp_table_name()
         full_query = f"CREATE TEMP VIEW {uuidstr} AS {query}; COPY (SELECT *FROM {uuidstr})  TO '{file_name}' (FORMAT JSON, Array True); DROP VIEW {uuidstr}"
         self.con.execute(full_query)
```

### Comparing `bmsdna_lakeapi-0.8.1/bmsdna/lakeapi/context/df_polars.py` & `bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/context/df_polars.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.8.1/bmsdna/lakeapi/core/config.py` & `bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/core/config.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.8.1/bmsdna/lakeapi/core/dataframe.py` & `bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/core/dataframe.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.8.1/bmsdna/lakeapi/core/endpoint.py` & `bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/core/endpoint.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.8.1/bmsdna/lakeapi/core/log.py` & `bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/core/log.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.8.1/bmsdna/lakeapi/core/model.py` & `bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/core/model.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.8.1/bmsdna/lakeapi/core/partition_utils.py` & `bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/core/partition_utils.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.8.1/bmsdna/lakeapi/core/response.py` & `bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/core/response.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.8.1/bmsdna/lakeapi/core/route.py` & `bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/core/route.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.8.1/bmsdna/lakeapi/core/sql_endpoint.py` & `bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/core/sql_endpoint.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.8.1/bmsdna/lakeapi/core/types.py` & `bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/core/types.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.8.1/bmsdna/lakeapi/core/uservalidation.py` & `bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/core/uservalidation.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.8.1/bmsdna/lakeapi/polars_extensions/delta.py` & `bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/polars_extensions/delta.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.8.1/bmsdna/lakeapi/tools/useradd.py` & `bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/tools/useradd.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.8.1/bmsdna/lakeapi/tools/validateschema.py` & `bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/tools/validateschema.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.8.1/bmsdna/lakeapi/utils/fast_api_utils.py` & `bmsdna_lakeapi-0.8.2/bmsdna/lakeapi/utils/fast_api_utils.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.8.1/pyproject.toml` & `bmsdna_lakeapi-0.8.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bmsdna-lakeapi"
-version = "0.8.1"
+version = "0.8.2"
 description = ""
 authors = ["DWH Team <you@example.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "bmsdna"}]
 
 [tool.poetry.dependencies]
```

### Comparing `bmsdna_lakeapi-0.8.1/PKG-INFO` & `bmsdna_lakeapi-0.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmsdna-lakeapi
-Version: 0.8.1
+Version: 0.8.2
 Summary: 
 License: MIT
 Author: DWH Team
 Author-email: you@example.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

