# Comparing `tmp/dbt_exasol-1.4.1.tar.gz` & `tmp/dbt_exasol-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_exasol-1.4.1.tar", max compression
+gzip compressed data, was "dbt_exasol-1.4.3.tar", max compression
```

## Comparing `dbt_exasol-1.4.1.tar` & `dbt_exasol-1.4.3.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rwxr-xr-x   0        0        0    35148 2021-12-30 07:56:19.472113 dbt_exasol-1.4.1/LICENSE
--rw-r--r--   0        0        0     2366 2023-04-14 09:01:39.934780 dbt_exasol-1.4.1/README.md
--rw-r--r--   0        0        0       65 2022-10-31 12:37:40.605136 dbt_exasol-1.4.1/dbt/__init__.py
--rw-r--r--   0        0        0       65 2022-10-31 12:37:40.605307 dbt_exasol-1.4.1/dbt/adapters/__init__.py
--rw-r--r--   0        0        0      508 2022-09-24 11:49:10.227324 dbt_exasol-1.4.1/dbt/adapters/exasol/__init__.py
--rw-r--r--   0        0        0       21 2023-05-16 12:41:02.600018 dbt_exasol-1.4.1/dbt/adapters/exasol/__version__.py
--rw-r--r--   0        0        0     3779 2023-05-16 12:41:02.600543 dbt_exasol-1.4.1/dbt/adapters/exasol/column.py
--rw-r--r--   0        0        0    10591 2023-05-16 12:41:02.601107 dbt_exasol-1.4.1/dbt/adapters/exasol/connections.py
--rw-r--r--   0        0        0     2893 2023-05-16 12:41:02.601600 dbt_exasol-1.4.1/dbt/adapters/exasol/impl.py
--rw-r--r--   0        0        0     2023 2023-05-16 12:41:02.602078 dbt_exasol-1.4.1/dbt/adapters/exasol/relation.py
--rw-r--r--   0        0        0       65 2022-10-31 12:37:40.606232 dbt_exasol-1.4.1/dbt/include/__init__.py
--rw-r--r--   0        0        0       52 2022-10-31 12:37:40.606685 dbt_exasol-1.4.1/dbt/include/exasol/__init__.py
--rwxr-xr-x   0        0        0      236 2021-12-30 07:56:19.481658 dbt_exasol-1.4.1/dbt/include/exasol/__pycache__/__init__.cpython-37.pyc
--rwxr-xr-x   0        0        0       74 2021-12-30 07:56:19.482361 dbt_exasol-1.4.1/dbt/include/exasol/dbt_project.yml
--rw-r--r--   0        0        0     6416 2023-05-16 12:41:02.602418 dbt_exasol-1.4.1/dbt/include/exasol/macros/adapters.sql
--rw-r--r--   0        0        0      673 2022-09-24 11:49:10.228097 dbt_exasol-1.4.1/dbt/include/exasol/macros/apply_grants.sql
--rwxr-xr-x   0        0        0     1458 2021-12-30 07:56:19.483484 dbt_exasol-1.4.1/dbt/include/exasol/macros/catalog.sql
--rw-r--r--   0        0        0     4239 2023-04-14 09:01:39.935574 dbt_exasol-1.4.1/dbt/include/exasol/macros/materializations/incremental.sql
--rw-r--r--   0        0        0      259 2023-04-14 09:01:39.935866 dbt_exasol-1.4.1/dbt/include/exasol/macros/materializations/incremental_strategies.sql
--rw-r--r--   0        0        0     1059 2023-05-16 12:41:02.602707 dbt_exasol-1.4.1/dbt/include/exasol/macros/materializations/merge.sql
--rwxr-xr-x   0        0        0      470 2021-12-30 07:56:19.484675 dbt_exasol-1.4.1/dbt/include/exasol/macros/materializations/seed.sql
--rw-r--r--   0        0        0     8044 2022-12-14 10:37:34.599267 dbt_exasol-1.4.1/dbt/include/exasol/macros/materializations/snapshot.sql
--rw-r--r--   0        0        0      748 2022-09-23 10:36:06.838210 dbt_exasol-1.4.1/dbt/include/exasol/macros/materializations/snapshot_merge.sql
--rw-r--r--   0        0        0     3258 2023-04-05 08:18:56.802378 dbt_exasol-1.4.1/dbt/include/exasol/macros/materializations/strategies.sql
--rw-r--r--   0        0        0     3524 2023-04-02 07:58:27.134719 dbt_exasol-1.4.1/dbt/include/exasol/macros/materializations/table.sql
--rw-r--r--   0        0        0      178 2022-09-24 11:49:10.228609 dbt_exasol-1.4.1/dbt/include/exasol/macros/utils/any_value.sql
--rw-r--r--   0        0        0       85 2022-09-24 11:49:10.228793 dbt_exasol-1.4.1/dbt/include/exasol/macros/utils/bool_or.sql
--rw-r--r--   0        0        0      469 2023-04-05 08:14:10.615503 dbt_exasol-1.4.1/dbt/include/exasol/macros/utils/dateadd.sql
--rw-r--r--   0        0        0      441 2023-04-04 22:40:13.470680 dbt_exasol-1.4.1/dbt/include/exasol/macros/utils/datediff.sql
--rw-r--r--   0        0        0      130 2022-09-24 11:49:10.229328 dbt_exasol-1.4.1/dbt/include/exasol/macros/utils/hash.sql
--rw-r--r--   0        0        0      381 2023-04-03 10:32:45.345850 dbt_exasol-1.4.1/dbt/include/exasol/macros/utils/last_day.sql
--rw-r--r--   0        0        0      415 2023-04-05 08:14:16.076524 dbt_exasol-1.4.1/dbt/include/exasol/macros/utils/listagg.sql
--rw-r--r--   0        0        0      775 2022-09-24 11:49:10.229642 dbt_exasol-1.4.1/dbt/include/exasol/macros/utils/safe_cast.sql
--rw-r--r--   0        0        0      165 2023-04-04 22:33:31.780189 dbt_exasol-1.4.1/dbt/include/exasol/macros/utils/split_part.sql
--rw-r--r--   0        0        0      539 2023-05-16 12:41:02.602901 dbt_exasol-1.4.1/dbt/include/exasol/macros/utils/timestamps.sql
--rw-r--r--   0        0        0      392 2023-05-16 12:35:48.493310 dbt_exasol-1.4.1/dbt/include/exasol/profile_template.yml
--rw-r--r--   0        0        0      940 2023-05-16 12:41:02.605059 dbt_exasol-1.4.1/pyproject.toml
--rw-r--r--   0        0        0      606 2023-04-03 10:32:45.347355 dbt_exasol-1.4.1/tests/conftest.py
--rw-r--r--   0        0        0     7729 2023-04-03 10:32:45.347626 dbt_exasol-1.4.1/tests/functional/adapter/expected_catalog.py
--rw-r--r--   0        0        0     1438 2023-04-03 10:32:45.347717 dbt_exasol-1.4.1/tests/functional/adapter/files.py
--rw-r--r--   0        0        0      521 2023-04-03 10:32:45.347798 dbt_exasol-1.4.1/tests/functional/adapter/fixtures.py
--rw-r--r--   0        0        0      708 2023-05-16 12:41:02.605287 dbt_exasol-1.4.1/tests/functional/adapter/query_comment_tests/test_query_comment.py
--rw-r--r--   0        0        0      197 2023-05-16 12:41:02.605493 dbt_exasol-1.4.1/tests/functional/adapter/relations/test_changing_relation_type.py
--rw-r--r--   0        0        0     2708 2023-04-03 10:32:45.347983 dbt_exasol-1.4.1/tests/functional/adapter/test_basic.py
--rw-r--r--   0        0        0     1255 2023-04-03 10:32:45.348130 dbt_exasol-1.4.1/tests/functional/adapter/test_concurrency.py
--rw-r--r--   0        0        0    12762 2023-04-03 10:32:45.348333 dbt_exasol-1.4.1/tests/functional/adapter/test_docs_generate.py
--rw-r--r--   0        0        0      457 2023-04-03 10:32:45.348436 dbt_exasol-1.4.1/tests/functional/adapter/test_ephemeral.py
--rw-r--r--   0        0        0     2068 2023-04-03 10:32:45.348518 dbt_exasol-1.4.1/tests/functional/adapter/test_failing_test.py
--rw-r--r--   0        0        0     1400 2023-05-16 12:41:02.606068 dbt_exasol-1.4.1/tests/functional/adapter/utils/data_types/test_data_types.py
--rw-r--r--   0        0        0      591 2023-04-05 08:20:04.514413 dbt_exasol-1.4.1/tests/functional/adapter/utils/data_types/test_type_bigint.py
--rw-r--r--   0        0        0     1200 2023-05-16 12:41:02.606246 dbt_exasol-1.4.1/tests/functional/adapter/utils/test_timestamps.py
--rw-r--r--   0        0        0    12583 2023-05-16 12:41:02.606529 dbt_exasol-1.4.1/tests/functional/adapter/utils/test_utils.py
--rw-r--r--   0        0        0    14496 2023-04-03 10:32:45.349250 dbt_exasol-1.4.1/tests/functional/adapter/utils/utils_fixtures.py
--rw-r--r--   0        0        0      954 2023-05-16 12:41:02.606789 dbt_exasol-1.4.1/tests/functional/test_grants.py
--rw-r--r--   0        0        0     8096 2022-12-14 12:35:07.724147 dbt_exasol-1.4.1/tests/functional/test_incremental.py
--rw-r--r--   0        0        0     1465 2022-12-09 10:46:24.315528 dbt_exasol-1.4.1/tests/functional/test_issues.py
--rw-r--r--   0        0        0     3169 1970-01-01 00:00:00.000000 dbt_exasol-1.4.1/PKG-INFO
+-rwxr-xr-x   0        0        0    35148 2021-12-30 07:56:19.472113 dbt_exasol-1.4.3/LICENSE
+-rw-r--r--   0        0        0     2504 2023-06-12 16:14:26.080747 dbt_exasol-1.4.3/README.md
+-rw-r--r--   0        0        0       65 2023-05-30 21:28:56.423110 dbt_exasol-1.4.3/dbt/__init__.py
+-rw-r--r--   0        0        0       65 2023-05-30 21:28:56.427667 dbt_exasol-1.4.3/dbt/adapters/__init__.py
+-rw-r--r--   0        0        0      508 2023-05-30 21:33:28.065894 dbt_exasol-1.4.3/dbt/adapters/exasol/__init__.py
+-rw-r--r--   0        0        0       19 2023-06-13 06:57:57.600762 dbt_exasol-1.4.3/dbt/adapters/exasol/__version__.py
+-rw-r--r--   0        0        0     3675 2023-06-12 16:35:19.474496 dbt_exasol-1.4.3/dbt/adapters/exasol/column.py
+-rw-r--r--   0        0        0    10688 2023-06-12 16:35:19.475379 dbt_exasol-1.4.3/dbt/adapters/exasol/connections.py
+-rw-r--r--   0        0        0     2806 2023-06-12 16:35:19.476101 dbt_exasol-1.4.3/dbt/adapters/exasol/impl.py
+-rw-r--r--   0        0        0     1959 2023-06-12 16:35:19.476752 dbt_exasol-1.4.3/dbt/adapters/exasol/relation.py
+-rw-r--r--   0        0        0       65 2023-05-30 21:28:56.417362 dbt_exasol-1.4.3/dbt/include/__init__.py
+-rw-r--r--   0        0        0       52 2023-05-30 21:28:56.419671 dbt_exasol-1.4.3/dbt/include/exasol/__init__.py
+-rwxr-xr-x   0        0        0      236 2021-12-30 07:56:19.481658 dbt_exasol-1.4.3/dbt/include/exasol/__pycache__/__init__.cpython-37.pyc
+-rwxr-xr-x   0        0        0       74 2021-12-30 07:56:19.482361 dbt_exasol-1.4.3/dbt/include/exasol/dbt_project.yml
+-rw-r--r--   0        0        0     6240 2023-06-12 16:35:19.477331 dbt_exasol-1.4.3/dbt/include/exasol/macros/adapters.sql
+-rw-r--r--   0        0        0      673 2023-05-30 21:30:19.492885 dbt_exasol-1.4.3/dbt/include/exasol/macros/apply_grants.sql
+-rwxr-xr-x   0        0        0     1458 2023-05-30 21:30:19.489001 dbt_exasol-1.4.3/dbt/include/exasol/macros/catalog.sql
+-rw-r--r--   0        0        0     4239 2023-05-30 21:30:19.462558 dbt_exasol-1.4.3/dbt/include/exasol/macros/materializations/incremental.sql
+-rw-r--r--   0        0        0      259 2023-05-30 21:30:19.453074 dbt_exasol-1.4.3/dbt/include/exasol/macros/materializations/incremental_strategies.sql
+-rw-r--r--   0        0        0     1025 2023-06-12 16:35:19.477809 dbt_exasol-1.4.3/dbt/include/exasol/macros/materializations/merge.sql
+-rwxr-xr-x   0        0        0      470 2023-05-30 21:30:19.450464 dbt_exasol-1.4.3/dbt/include/exasol/macros/materializations/seed.sql
+-rw-r--r--   0        0        0     8044 2023-05-30 21:30:19.464735 dbt_exasol-1.4.3/dbt/include/exasol/macros/materializations/snapshot.sql
+-rw-r--r--   0        0        0      748 2023-05-30 21:30:19.455665 dbt_exasol-1.4.3/dbt/include/exasol/macros/materializations/snapshot_merge.sql
+-rw-r--r--   0        0        0     3258 2023-05-30 21:30:19.457925 dbt_exasol-1.4.3/dbt/include/exasol/macros/materializations/strategies.sql
+-rw-r--r--   0        0        0     3524 2023-05-30 21:30:19.460381 dbt_exasol-1.4.3/dbt/include/exasol/macros/materializations/table.sql
+-rw-r--r--   0        0        0      178 2023-05-30 21:30:19.480626 dbt_exasol-1.4.3/dbt/include/exasol/macros/utils/any_value.sql
+-rw-r--r--   0        0        0       85 2023-05-30 21:30:19.482423 dbt_exasol-1.4.3/dbt/include/exasol/macros/utils/bool_or.sql
+-rw-r--r--   0        0        0      469 2023-05-30 21:30:19.466872 dbt_exasol-1.4.3/dbt/include/exasol/macros/utils/dateadd.sql
+-rw-r--r--   0        0        0      441 2023-05-30 21:30:19.474475 dbt_exasol-1.4.3/dbt/include/exasol/macros/utils/datediff.sql
+-rw-r--r--   0        0        0      130 2023-05-30 21:30:19.478733 dbt_exasol-1.4.3/dbt/include/exasol/macros/utils/hash.sql
+-rw-r--r--   0        0        0      381 2023-05-30 21:30:19.484622 dbt_exasol-1.4.3/dbt/include/exasol/macros/utils/last_day.sql
+-rw-r--r--   0        0        0      415 2023-05-30 21:30:19.471787 dbt_exasol-1.4.3/dbt/include/exasol/macros/utils/listagg.sql
+-rw-r--r--   0        0        0      775 2023-05-30 21:30:19.476801 dbt_exasol-1.4.3/dbt/include/exasol/macros/utils/safe_cast.sql
+-rw-r--r--   0        0        0      165 2023-05-30 21:30:19.486659 dbt_exasol-1.4.3/dbt/include/exasol/macros/utils/split_part.sql
+-rw-r--r--   0        0        0      519 2023-06-12 16:35:19.478151 dbt_exasol-1.4.3/dbt/include/exasol/macros/utils/timestamps.sql
+-rw-r--r--   0        0        0      374 2023-05-31 15:48:24.596080 dbt_exasol-1.4.3/dbt/include/exasol/profile_template.yml
+-rw-r--r--   0        0        0      906 2023-06-13 06:57:43.652646 dbt_exasol-1.4.3/pyproject.toml
+-rw-r--r--   0        0        0      606 2023-05-30 21:28:56.447674 dbt_exasol-1.4.3/tests/conftest.py
+-rw-r--r--   0        0        0     7729 2023-05-30 21:28:56.484385 dbt_exasol-1.4.3/tests/functional/adapter/expected_catalog.py
+-rw-r--r--   0        0        0     1438 2023-05-30 21:28:56.450549 dbt_exasol-1.4.3/tests/functional/adapter/files.py
+-rw-r--r--   0        0        0      521 2023-05-30 21:28:56.489680 dbt_exasol-1.4.3/tests/functional/adapter/fixtures.py
+-rw-r--r--   0        0        0      676 2023-06-12 16:35:19.481459 dbt_exasol-1.4.3/tests/functional/adapter/query_comment_tests/test_query_comment.py
+-rw-r--r--   0        0        0      190 2023-06-12 16:35:19.481812 dbt_exasol-1.4.3/tests/functional/adapter/relations/test_changing_relation_type.py
+-rw-r--r--   0        0        0     2708 2023-05-30 21:28:56.452648 dbt_exasol-1.4.3/tests/functional/adapter/test_basic.py
+-rw-r--r--   0        0        0     1255 2023-05-30 21:28:56.455200 dbt_exasol-1.4.3/tests/functional/adapter/test_concurrency.py
+-rw-r--r--   0        0        0    12762 2023-05-30 21:28:56.486846 dbt_exasol-1.4.3/tests/functional/adapter/test_docs_generate.py
+-rw-r--r--   0        0        0      457 2023-06-12 13:34:48.744670 dbt_exasol-1.4.3/tests/functional/adapter/test_ephemeral.py
+-rw-r--r--   0        0        0     2068 2023-05-30 21:28:56.476133 dbt_exasol-1.4.3/tests/functional/adapter/test_failing_test.py
+-rw-r--r--   0        0        0     1350 2023-06-12 16:35:19.482380 dbt_exasol-1.4.3/tests/functional/adapter/utils/data_types/test_data_types.py
+-rw-r--r--   0        0        0      591 2023-05-30 21:28:56.463459 dbt_exasol-1.4.3/tests/functional/adapter/utils/data_types/test_type_bigint.py
+-rw-r--r--   0        0        0     1167 2023-06-12 16:35:19.482708 dbt_exasol-1.4.3/tests/functional/adapter/utils/test_timestamps.py
+-rw-r--r--   0        0        0    12212 2023-06-12 16:35:19.483126 dbt_exasol-1.4.3/tests/functional/adapter/utils/test_utils.py
+-rw-r--r--   0        0        0    14496 2023-05-30 21:28:56.468780 dbt_exasol-1.4.3/tests/functional/adapter/utils/utils_fixtures.py
+-rw-r--r--   0        0        0      924 2023-06-12 16:35:19.483568 dbt_exasol-1.4.3/tests/functional/test_grants.py
+-rw-r--r--   0        0        0     8096 2023-05-30 21:28:56.496086 dbt_exasol-1.4.3/tests/functional/test_incremental.py
+-rw-r--r--   0        0        0     1465 2023-05-30 21:28:56.492771 dbt_exasol-1.4.3/tests/functional/test_issues.py
+-rw-r--r--   0        0        0     3307 1970-01-01 00:00:00.000000 dbt_exasol-1.4.3/PKG-INFO
```

### Comparing `dbt_exasol-1.4.1/LICENSE` & `dbt_exasol-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.4.1/README.md` & `dbt_exasol-1.4.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -16,14 +16,17 @@
       dsn: HOST:PORT
       user: USERNAME
       password: PASSWORD
       dbname: db
       schema: SCHEMA
 ```
 
+#### Optional login credentials using OpenID for Exasol SaaS
+OpenID login through access_token or refresh_token instead of user+password
+
 #### Optional parameters
 <ul>
   <li><strong>connection_timeout</strong>: defaults to pyexasol default</li>
   <li><strong>socket_timeout</strong>: defaults to pyexasol default</li>
   <li><strong>query_timeout</strong>: defaults to pyexasol default</li>
   <li><strong>compression</strong>: default: False</li>
   <li><strong>encryption</strong>: default: False</li>
```

### Comparing `dbt_exasol-1.4.1/dbt/adapters/exasol/column.py` & `dbt_exasol-1.4.3/dbt/adapters/exasol/column.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,104 +1,104 @@
-"""
-dbt exasol adapter column module
-"""
-import re
-from dataclasses import dataclass
-from typing import ClassVar, Dict
-
-from dbt.adapters.base.column import Column
-from dbt.exceptions import DbtRuntimeError
-
-
-@dataclass
-# pylint: disable=missing-function-docstring
-class ExasolColumn(Column):
-    """Column implementation for exasol"""
-
-    # https://docs.exasol.com/db/latest/sql_references/data_types/datatypealiases.htm
-    TYPE_LABELS: ClassVar[Dict[str, str]] = {
-        "STRING": "VARCHAR(2000000) UTF8",
-        "TIMESTAMP": "TIMESTAMP",
-        "FLOAT": "DOUBLE PRECISION",
-        "INTEGER": "DECIMAL(18,0)",
-        "BIGINT": "DECIMAL(36,0)",
-        "NUMERIC": "DECIMAL(18,9)",
-    }
-
-    def is_numeric(self) -> bool:
-        return self.dtype.lower() in ["decimal", "double"]
-
-    def is_integer(self) -> bool:
-        # everything that smells like an int is actually a DECIMAL(18, 0)
-        return self.is_numeric() and self.numeric_scale == 0
-
-    def is_float(self):
-        return self.dtype.lower() == "double"
-
-    def is_string(self) -> bool:
-        return self.dtype.lower() in ["char", "varchar"]
-
-    def is_hashtype(self) -> bool:
-        return self.dtype.lower() == "hashtype"
-
-    def is_boolean(self) -> bool:
-        return self.dtype.lower() == "boolean"
-
-    def is_timestamp(self) -> bool:
-        # handle TIMESTAMP and TIMESTAMP WITH LOCAL TIME ZONE
-        return self.dtype.lower().startswith("timestamp")
-
-    def is_date(self) -> bool:
-        return self.dtype.lower() == "date"
-
-    def string_size(self) -> int:
-        if not self.is_string():
-            raise DbtRuntimeError("Called string_size() on non-string field!")
-        if self.char_size is None:
-            return 2000000
-        return int(self.char_size)
-
-    @classmethod
-    def string_type(cls, size: int) -> str:
-        return f"VARCHAR({size})"
-
-    @classmethod
-    # pylint: disable=raise-missing-from
-    def from_description(cls, name: str, raw_data_type: str) -> "Column":
-        match = re.match(r"([^(]+)(\([^)]+\))?", raw_data_type)
-        if match is None:
-            raise DbtRuntimeError(f'Could not interpret data type "{raw_data_type}"')
-        data_type, size_info = match.groups()
-        char_size = None
-        numeric_precision = None
-        numeric_scale = None
-        if size_info is not None:
-            # strip out the parentheses
-            size_info = size_info[1:-1]
-            parts = size_info.split(",")
-            if len(parts) == 1:
-                try:
-                    # handle things like HASHTYPE(16 BYTE)
-                    size = re.sub(r"[^\d]", "", parts[0])
-                    char_size = int(size)
-                except ValueError:
-                    raise DbtRuntimeError(
-                        f'Could not interpret data_type "{raw_data_type}": '
-                        f'could not convert "{size}" to an integer'
-                    )
-            elif len(parts) == 2:
-                try:
-                    numeric_precision = int(parts[0])
-                except ValueError:
-                    raise DbtRuntimeError(
-                        f'Could not interpret data_type "{raw_data_type}": '
-                        f'could not convert "{parts[0]}" to an integer'
-                    )
-                try:
-                    numeric_scale = int(parts[1])
-                except ValueError:
-                    raise DbtRuntimeError(
-                        f'Could not interpret data_type "{raw_data_type}": '
-                        f'could not convert "{parts[1]}" to an integer'
-                    )
-
-        return cls(name, data_type, char_size, numeric_precision, numeric_scale)
+"""
+dbt exasol adapter column module
+"""
+import re
+from dataclasses import dataclass
+from typing import ClassVar, Dict
+
+from dbt.adapters.base.column import Column
+from dbt.exceptions import DbtRuntimeError
+
+
+@dataclass
+# pylint: disable=missing-function-docstring
+class ExasolColumn(Column):
+    """Column implementation for exasol"""
+
+    # https://docs.exasol.com/db/latest/sql_references/data_types/datatypealiases.htm
+    TYPE_LABELS: ClassVar[Dict[str, str]] = {
+        "STRING": "VARCHAR(2000000) UTF8",
+        "TIMESTAMP": "TIMESTAMP",
+        "FLOAT": "DOUBLE PRECISION",
+        "INTEGER": "DECIMAL(18,0)",
+        "BIGINT": "DECIMAL(36,0)",
+        "NUMERIC": "DECIMAL(18,9)",
+    }
+
+    def is_numeric(self) -> bool:
+        return self.dtype.lower() in ["decimal", "double"]
+
+    def is_integer(self) -> bool:
+        # everything that smells like an int is actually a DECIMAL(18, 0)
+        return self.is_numeric() and self.numeric_scale == 0
+
+    def is_float(self):
+        return self.dtype.lower() == "double"
+
+    def is_string(self) -> bool:
+        return self.dtype.lower() in ["char", "varchar"]
+
+    def is_hashtype(self) -> bool:
+        return self.dtype.lower() == "hashtype"
+
+    def is_boolean(self) -> bool:
+        return self.dtype.lower() == "boolean"
+
+    def is_timestamp(self) -> bool:
+        # handle TIMESTAMP and TIMESTAMP WITH LOCAL TIME ZONE
+        return self.dtype.lower().startswith("timestamp")
+
+    def is_date(self) -> bool:
+        return self.dtype.lower() == "date"
+
+    def string_size(self) -> int:
+        if not self.is_string():
+            raise DbtRuntimeError("Called string_size() on non-string field!")
+        if self.char_size is None:
+            return 2000000
+        return int(self.char_size)
+
+    @classmethod
+    def string_type(cls, size: int) -> str:
+        return f"VARCHAR({size})"
+
+    @classmethod
+    # pylint: disable=raise-missing-from
+    def from_description(cls, name: str, raw_data_type: str) -> "Column":
+        match = re.match(r"([^(]+)(\([^)]+\))?", raw_data_type)
+        if match is None:
+            raise DbtRuntimeError(f'Could not interpret data type "{raw_data_type}"')
+        data_type, size_info = match.groups()
+        char_size = None
+        numeric_precision = None
+        numeric_scale = None
+        if size_info is not None:
+            # strip out the parentheses
+            size_info = size_info[1:-1]
+            parts = size_info.split(",")
+            if len(parts) == 1:
+                try:
+                    # handle things like HASHTYPE(16 BYTE)
+                    size = re.sub(r"[^\d]", "", parts[0])
+                    char_size = int(size)
+                except ValueError:
+                    raise DbtRuntimeError(
+                        f'Could not interpret data_type "{raw_data_type}": '
+                        f'could not convert "{size}" to an integer'
+                    )
+            elif len(parts) == 2:
+                try:
+                    numeric_precision = int(parts[0])
+                except ValueError:
+                    raise DbtRuntimeError(
+                        f'Could not interpret data_type "{raw_data_type}": '
+                        f'could not convert "{parts[0]}" to an integer'
+                    )
+                try:
+                    numeric_scale = int(parts[1])
+                except ValueError:
+                    raise DbtRuntimeError(
+                        f'Could not interpret data_type "{raw_data_type}": '
+                        f'could not convert "{parts[1]}" to an integer'
+                    )
+
+        return cls(name, data_type, char_size, numeric_precision, numeric_scale)
```

### Comparing `dbt_exasol-1.4.1/dbt/adapters/exasol/connections.py` & `dbt_exasol-1.4.3/dbt/adapters/exasol/connections.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,332 +1,340 @@
-# pylint: disable=wrong-import-order
-# pylint: disable=ungrouped-imports
-"""
-DBT adapter connection implementation for Exasol.
-"""
-import decimal
-import os
-from contextlib import contextmanager
-from dataclasses import dataclass
-from typing import Any, List, Optional
-
-import agate
-import dbt.exceptions
-import pyexasol
-from dbt.adapters.base import Credentials  # type: ignore
-from dbt.adapters.sql import SQLConnectionManager  # type: ignore
-from dbt.contracts.connection import AdapterResponse
-from dbt.events import AdapterLogger
-from hologram.helpers import StrEnum
-from pyexasol import ExaConnection
-
-ROW_SEPARATOR_DEFAULT = "LF" if os.linesep == "\n" else "CRLF"
-TIMESTAMP_FORMAT_DEFAULT = "YYYY-MM-DDTHH:MI:SS.FF6"
-
-LOGGER = AdapterLogger("exasol")
-
-
-def connect(**kwargs: bool):
-    """
-    Global connect method initializing ExasolConnection
-    """
-    if "autocommit" not in kwargs:
-        kwargs["autocommit"] = False
-    return ExasolConnection(**kwargs)
-
-
-class ProtocolVersionType(StrEnum):
-    """Exasol protocol versions"""
-
-    V1 = "v1"
-    V2 = "v2"
-    V3 = "v3"
-
-
-class ExasolConnection(ExaConnection):
-    """
-    Override to instantiate ExasolCursor
-    """
-
-    row_separator: str = ROW_SEPARATOR_DEFAULT
-    timestamp_format: str = TIMESTAMP_FORMAT_DEFAULT
-
-    def cursor(self):
-        """Instance of ExasolCursor"""
-        return ExasolCursor(self)
-
-
-@dataclass
-class ExasolAdapterResponse(AdapterResponse):
-    """
-    Override AdapterResponse
-    """
-
-    execution_time: Optional[float] = None
-
-
-# pylint: disable=too-many-instance-attributes
-@dataclass
-class ExasolCredentials(Credentials):
-    """Profile parameters for Exasol in dbt profiles.yml"""
-
-    dsn: str
-    user: str
-    password: str
-    database: str
-    schema: str
-    # optional statements that can be set in profiles.yml
-    # some options might interfere with dbt, so caution is advised
-    connection_timeout: int = pyexasol.constant.DEFAULT_CONNECTION_TIMEOUT
-    socket_timeout: int = pyexasol.constant.DEFAULT_SOCKET_TIMEOUT
-    query_timeout: int = pyexasol.constant.DEFAULT_QUERY_TIMEOUT
-    compression: bool = False
-    encryption: bool = False
-    ## Because of potential interference with dbt,
-    # the following statements are not (yet) implemented
-    # fetch_dict: bool
-    # fetch_size_bytes: int
-    # lower_ident: bool
-    # quote_ident: bool
-    # verbose_error: bool
-    # debug: bool
-    # udf_output_port: int
-    protocol_version: str = "v3"
-    retries: int = 1
-    row_separator: str = ROW_SEPARATOR_DEFAULT
-    timestamp_format: str = TIMESTAMP_FORMAT_DEFAULT
-
-    _ALIASES = {"dbname": "database", "pass": "password"}
-
-    @property
-    def type(self):
-        return "exasol"
-
-    @property
-    def unique_field(self):
-        return self.dsn
-
-    def _connection_keys(self):
-        return (
-            "dsn",
-            "user",
-            "database",
-            "schema",
-            "connection_timeout",
-            "socket_timeout",
-            "query_timeout",
-            "compression",
-            "encryption",
-            "protocol_version",
-            "row_separator",
-            "timestamp_format",
-        )
-
-
-class ExasolConnectionManager(SQLConnectionManager):
-    """Managing Exasol connections"""
-
-    TYPE = "exasol"
-
-    @contextmanager
-    def exception_handler(self, sql):
-        try:
-            yield
-
-        except Exception as yielded_exception:
-            LOGGER.debug(f"Error running SQL: {sql}")
-            LOGGER.debug("Rolling back transaction.")
-            self.rollback_if_open()
-            if isinstance(yielded_exception, dbt.exceptions.DbtRuntimeError):
-                # during a sql query, an internal to dbt exception was raised.
-                # this sounds a lot like a signal handler and probably has
-                # useful information, so raise it without modification.
-                raise
-
-            raise dbt.exceptions.DbtRuntimeError(yielded_exception)
-
-    @classmethod
-    def get_result_from_cursor(cls, cursor: Any) -> agate.Table:
-        data: List[Any] = []
-        column_names: List[str] = []
-
-        if cursor.description is not None:
-            # column_names = [col[0] for col in cursor.description]
-            rows = cursor.fetchall()
-            for idx, col in enumerate(cursor.description):
-                column_names.append(col[0])
-                if len(rows) > 0 and isinstance(rows[0][idx], str):
-                    if col[1] in ["DECIMAL", "BIGINT"]:
-                        for rownum, row in enumerate(rows):
-                            tmp = list(row)
-                            tmp[idx] = decimal.Decimal(row[idx])
-                            rows[rownum] = tmp
-            data = cls.process_results(column_names, rows)
-
-        return dbt.clients.agate_helper.table_from_data_flat(data, column_names)  # type: ignore
-
-    @classmethod
-    # pylint: disable=raise-missing-from
-    def open(cls, connection):
-        if connection.state == "open":
-            LOGGER.debug("Connection is already open, skipping open.")
-            return connection
-        credentials = connection.credentials
-
-        # Support protocol versions
-        try:
-            format_protocol_version = credentials.protocol_version.lower()
-            version = ProtocolVersionType(format_protocol_version)
-
-            if version == ProtocolVersionType.V1:
-                protocol_version = pyexasol.PROTOCOL_V1
-            elif version == ProtocolVersionType.V2:
-                protocol_version = pyexasol.PROTOCOL_V2
-            else:
-                protocol_version = pyexasol.PROTOCOL_V3
-        except:
-            raise dbt.exceptions.DbtRuntimeError(
-                f"{credentials.protocol_version} is not a valid protocol version."
-            )
-
-        def _connect():
-            conn = connect(
-                dsn=credentials.dsn,
-                user=credentials.user,
-                password=credentials.password,
-                autocommit=True,
-                connection_timeout=credentials.connection_timeout,
-                socket_timeout=credentials.socket_timeout,
-                query_timeout=credentials.query_timeout,
-                compression=credentials.compression,
-                encryption=credentials.encryption,
-                protocol_version=protocol_version,
-            )
-            # exasol adapter specific attributes that are unknown to pyexasol
-            # those can be added to ExasolConnection as members
-            conn.row_separator = credentials.row_separator
-            conn.timestamp_format = credentials.timestamp_format
-            conn.execute(
-                f"alter session set NLS_TIMESTAMP_FORMAT='{conn.timestamp_format}'"
-            )
-
-            return conn
-
-        repeatable_exceptions = [pyexasol.ExaError]
-
-        return cls.retry_connection(
-            connection,
-            connect=_connect,
-            logger=LOGGER,
-            retry_limit=credentials.retries,
-            retryable_exceptions=repeatable_exceptions,
-        )
-
-    def add_begin_query(self):
-        return
-
-    def cancel(self, connection):
-        connection.abort_query()  # type: ignore
-
-    @classmethod
-    def get_response(cls, cursor) -> ExasolAdapterResponse:
-        return ExasolAdapterResponse(
-            _message="OK",
-            rows_affected=cursor.rowcount,
-            execution_time=cursor.execution_time,
-        )
-
-
-class ExasolCursor:
-    """Exasol dbt-adapter cursor implementation"""
-
-    array_size = 1
-
-    def __init__(self, connection):
-        self.connection = connection
-        self.stmt = None
-
-    def import_from_file(self, agate_table, table):
-        """importing csv skip=1 parameter for header row"""
-        self.connection.import_from_file(
-            agate_table.original_abspath,
-            (table.split(".")[0], table.split(".")[1]),
-            import_params={"skip": 1, "row_separator": self.connection.row_separator},
-        )
-        return self
-
-    def execute(self, query, bindings: Optional[Any] = None):
-        """executing query"""
-        if query.startswith("0CSV|"):
-            self.import_from_file(bindings, query.split("|", 1)[1])  # type: ignore
-        elif query.__contains__("|SEPARATEMEPLEASE|"):
-            sqls = query.split("|SEPARATEMEPLEASE|")
-            for sql in sqls:
-                self.stmt = self.connection.execute(sql)
-        else:
-            self.stmt = self.connection.execute(query)
-        return self
-
-    def fetchone(self):
-        """fetch single row"""
-        if self.stmt is None:
-            raise RuntimeError("Cannot fetch on unset statement")
-        return self.stmt.fetchone()
-
-    def fetchmany(self, size=None):
-        """fetch single row"""
-        if size is None:
-            size = self.array_size
-
-        if self.stmt is None:
-            raise RuntimeError("Cannot fetch on unset statement")
-        return self.stmt.fetchmany(size)
-
-    def fetchall(self):
-        """fetch single row"""
-        if self.stmt is None:
-            raise RuntimeError("Cannot fetch on unset statement")
-        return self.stmt.fetchall()
-
-    @property
-    def description(self):
-        """columns in cursor"""
-        cols = []
-        if self.stmt is None:
-            return cols
-
-        if "resultSet" != self.stmt.result_type:
-            return None
-
-        for k, value_set in self.stmt.columns().items():
-            cols.append(
-                (
-                    k,
-                    value_set.get("type", None),
-                    value_set.get("size", None),
-                    value_set.get("size", None),
-                    value_set.get("precision", None),
-                    value_set.get("scale", None),
-                    True,
-                )
-            )
-
-        return cols
-
-    @property
-    def rowcount(self):
-        """number of rows in result set"""
-        if self.stmt is not None:
-            return self.stmt.rowcount()
-        return 0
-
-    @property
-    def execution_time(self):
-        """elapsed time for query"""
-        if self.stmt is not None:
-            return self.stmt.execution_time
-        return 0
-
-    def close(self):
-        """closing the cursor / statement"""
-        if self.stmt is not None:
-            self.stmt.close()
+# pylint: disable=wrong-import-order
+# pylint: disable=ungrouped-imports
+"""
+DBT adapter connection implementation for Exasol.
+"""
+import decimal
+import os
+from contextlib import contextmanager
+from dataclasses import dataclass
+from typing import Any, List, Optional
+
+import agate
+import dbt.exceptions
+import pyexasol
+from dbt.adapters.base import Credentials  # type: ignore
+from dbt.adapters.sql import SQLConnectionManager  # type: ignore
+from dbt.contracts.connection import AdapterResponse
+from dbt.events import AdapterLogger
+from hologram.helpers import StrEnum
+from pyexasol import ExaConnection
+
+ROW_SEPARATOR_DEFAULT = "LF" if os.linesep == "\n" else "CRLF"
+TIMESTAMP_FORMAT_DEFAULT = "YYYY-MM-DDTHH:MI:SS.FF6"
+
+LOGGER = AdapterLogger("exasol")
+
+
+def connect(**kwargs: bool):
+    """
+    Global connect method initializing ExasolConnection
+    """
+    if "autocommit" not in kwargs:
+        kwargs["autocommit"] = False
+    return ExasolConnection(**kwargs)
+
+
+class ProtocolVersionType(StrEnum):
+    """Exasol protocol versions"""
+
+    V1 = "v1"
+    V2 = "v2"
+    V3 = "v3"
+
+
+class ExasolConnection(ExaConnection):
+    """
+    Override to instantiate ExasolCursor
+    """
+
+    row_separator: str = ROW_SEPARATOR_DEFAULT
+    timestamp_format: str = TIMESTAMP_FORMAT_DEFAULT
+
+    def cursor(self):
+        """Instance of ExasolCursor"""
+        return ExasolCursor(self)
+
+
+@dataclass
+class ExasolAdapterResponse(AdapterResponse):
+    """
+    Override AdapterResponse
+    """
+
+    execution_time: Optional[float] = None
+
+
+# pylint: disable=too-many-instance-attributes
+@dataclass
+class ExasolCredentials(Credentials):
+    """Profile parameters for Exasol in dbt profiles.yml"""
+
+    dsn: str
+    database: str
+    schema: str
+    # One of user+pass, access_token, or refresh_token needs to be specified in profiles.yml
+    user: str = ""
+    password: str = ""
+    access_token: str = ""
+    refresh_token: str = ""
+    # optional statements that can be set in profiles.yml
+    # some options might interfere with dbt, so caution is advised
+    connection_timeout: int = pyexasol.constant.DEFAULT_CONNECTION_TIMEOUT
+    socket_timeout: int = pyexasol.constant.DEFAULT_SOCKET_TIMEOUT
+    query_timeout: int = pyexasol.constant.DEFAULT_QUERY_TIMEOUT
+    compression: bool = False
+    encryption: bool = False
+    ## Because of potential interference with dbt,
+    # the following statements are not (yet) implemented
+    # fetch_dict: bool
+    # fetch_size_bytes: int
+    # lower_ident: bool
+    # quote_ident: bool
+    # verbose_error: bool
+    # debug: bool
+    # udf_output_port: int
+    protocol_version: str = "v3"
+    retries: int = 1
+    row_separator: str = ROW_SEPARATOR_DEFAULT
+    timestamp_format: str = TIMESTAMP_FORMAT_DEFAULT
+
+    _ALIASES = {"dbname": "database", "pass": "password"}
+
+    @property
+    def type(self):
+        return "exasol"
+
+    @property
+    def unique_field(self):
+        return self.dsn
+
+    def _connection_keys(self):
+        return (
+            "dsn",
+            "user",
+            "database",
+            "schema",
+            "connection_timeout",
+            "socket_timeout",
+            "query_timeout",
+            "compression",
+            "encryption",
+            "protocol_version",
+            "row_separator",
+            "timestamp_format",
+        )
+
+
+class ExasolConnectionManager(SQLConnectionManager):
+    """Managing Exasol connections"""
+
+    TYPE = "exasol"
+
+    @contextmanager
+    def exception_handler(self, sql):
+        try:
+            yield
+
+        except Exception as yielded_exception:
+            LOGGER.debug(f"Error running SQL: {sql}")
+            LOGGER.debug("Rolling back transaction.")
+            self.rollback_if_open()
+            if isinstance(yielded_exception, dbt.exceptions.DbtRuntimeError):
+                # during a sql query, an internal to dbt exception was raised.
+                # this sounds a lot like a signal handler and probably has
+                # useful information, so raise it without modification.
+                raise
+
+            raise dbt.exceptions.DbtRuntimeError(yielded_exception)
+
+    @classmethod
+    def get_result_from_cursor(cls, cursor: Any) -> agate.Table:
+        data: List[Any] = []
+        column_names: List[str] = []
+
+        if cursor.description is not None:
+            # column_names = [col[0] for col in cursor.description]
+            rows = cursor.fetchall()
+            for idx, col in enumerate(cursor.description):
+                column_names.append(col[0])
+                if len(rows) > 0 and isinstance(rows[0][idx], str):
+                    if col[1] in ["DECIMAL", "BIGINT"]:
+                        for rownum, row in enumerate(rows):
+                            tmp = list(row)
+                            tmp[idx] = decimal.Decimal(row[idx])
+                            rows[rownum] = tmp
+            data = cls.process_results(column_names, rows)
+
+        return dbt.clients.agate_helper.table_from_data_flat(data, column_names)  # type: ignore
+
+    @classmethod
+    # pylint: disable=raise-missing-from
+    def open(cls, connection):
+        if connection.state == "open":
+            LOGGER.debug("Connection is already open, skipping open.")
+            return connection
+        credentials = connection.credentials
+
+        # Support protocol versions
+        try:
+            format_protocol_version = credentials.protocol_version.lower()
+            version = ProtocolVersionType(format_protocol_version)
+
+            if version == ProtocolVersionType.V1:
+                protocol_version = pyexasol.PROTOCOL_V1
+            elif version == ProtocolVersionType.V2:
+                protocol_version = pyexasol.PROTOCOL_V2
+            else:
+                protocol_version = pyexasol.PROTOCOL_V3
+        except:
+            raise dbt.exceptions.DbtRuntimeError(
+                f"{credentials.protocol_version} is not a valid protocol version."
+            )
+
+        def _connect():
+            conn = connect(
+                dsn=credentials.dsn,
+                user=credentials.user,
+                password=credentials.password,
+                access_token=credentials.access_token,
+                refresh_token=credentials.refresh_token,
+                autocommit=True,
+                connection_timeout=credentials.connection_timeout,
+                socket_timeout=credentials.socket_timeout,
+                query_timeout=credentials.query_timeout,
+                compression=credentials.compression,
+                encryption=credentials.encryption,
+                protocol_version=protocol_version,
+            )
+            # exasol adapter specific attributes that are unknown to pyexasol
+            # those can be added to ExasolConnection as members
+            conn.row_separator = credentials.row_separator
+            conn.timestamp_format = credentials.timestamp_format
+            conn.execute(
+                f"alter session set NLS_TIMESTAMP_FORMAT='{conn.timestamp_format}'"
+            )
+
+            return conn
+
+        repeatable_exceptions = [pyexasol.ExaError]
+
+        return cls.retry_connection(
+            connection,
+            connect=_connect,
+            logger=LOGGER,
+            retry_limit=credentials.retries,
+            retryable_exceptions=repeatable_exceptions,
+        )
+
+    def add_begin_query(self):
+        return
+
+    def cancel(self, connection):
+        connection.abort_query()  # type: ignore
+
+    @classmethod
+    def get_response(cls, cursor) -> ExasolAdapterResponse:
+        return ExasolAdapterResponse(
+            _message="OK",
+            rows_affected=cursor.rowcount,
+            execution_time=cursor.execution_time,
+        )
+
+
+class ExasolCursor:
+    """Exasol dbt-adapter cursor implementation"""
+
+    array_size = 1
+
+    def __init__(self, connection):
+        self.connection = connection
+        self.stmt = None
+
+    def import_from_file(self, agate_table, table):
+        """importing csv skip=1 parameter for header row"""
+        self.connection.import_from_file(
+            agate_table.original_abspath,
+            (table.split(".")[0], table.split(".")[1]),
+            import_params={"skip": 1, "row_separator": self.connection.row_separator},
+        )
+        return self
+
+    def execute(self, query, bindings: Optional[Any] = None):
+        """executing query"""
+        if query.startswith("0CSV|"):
+            self.import_from_file(bindings, query.split("|", 1)[1])  # type: ignore
+        elif query.__contains__("|SEPARATEMEPLEASE|"):
+            sqls = query.split("|SEPARATEMEPLEASE|")
+            for sql in sqls:
+                self.stmt = self.connection.execute(sql)
+        else:
+            try:
+                self.stmt = self.connection.execute(query)
+            except pyexasol.ExaQueryError as e:
+                raise dbt.exceptions.DbtDatabaseError("Exasol Query Error: " + e.message)
+        return self
+
+    def fetchone(self):
+        """fetch single row"""
+        if self.stmt is None:
+            raise RuntimeError("Cannot fetch on unset statement")
+        return self.stmt.fetchone()
+
+    def fetchmany(self, size=None):
+        """fetch single row"""
+        if size is None:
+            size = self.array_size
+
+        if self.stmt is None:
+            raise RuntimeError("Cannot fetch on unset statement")
+        return self.stmt.fetchmany(size)
+
+    def fetchall(self):
+        """fetch single row"""
+        if self.stmt is None:
+            raise RuntimeError("Cannot fetch on unset statement")
+        return self.stmt.fetchall()
+
+    @property
+    def description(self):
+        """columns in cursor"""
+        cols = []
+        if self.stmt is None:
+            return cols
+
+        if "resultSet" != self.stmt.result_type:
+            return None
+
+        for k, value_set in self.stmt.columns().items():
+            cols.append(
+                (
+                    k,
+                    value_set.get("type", None),
+                    value_set.get("size", None),
+                    value_set.get("size", None),
+                    value_set.get("precision", None),
+                    value_set.get("scale", None),
+                    True,
+                )
+            )
+
+        return cols
+
+    @property
+    def rowcount(self):
+        """number of rows in result set"""
+        if self.stmt is not None:
+            return self.stmt.rowcount()
+        return 0
+
+    @property
+    def execution_time(self):
+        """elapsed time for query"""
+        if self.stmt is not None:
+            return self.stmt.execution_time
+        return 0
+
+    def close(self):
+        """closing the cursor / statement"""
+        if self.stmt is not None:
+            self.stmt.close()
```

### Comparing `dbt_exasol-1.4.1/dbt/adapters/exasol/impl.py` & `dbt_exasol-1.4.3/dbt/adapters/exasol/impl.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,88 +1,88 @@
-"""dbt-exasol Adapter implementation extending SQLAdapter"""
-from __future__ import absolute_import
-
-from typing import Dict, Optional
-
-import agate
-from dbt.adapters.sql import SQLAdapter
-from dbt.exceptions import CompilationError
-from dbt.utils import filter_null_values
-
-from dbt.adapters.exasol import (ExasolColumn, ExasolConnectionManager,
-                                 ExasolRelation)
-
-
-class ExasolAdapter(SQLAdapter):
-    """Exasol SQLAdapter extension"""
-
-    Relation = ExasolRelation
-    Column = ExasolColumn
-    ConnectionManager = ExasolConnectionManager
-
-    @classmethod
-    def date_function(cls):
-        return "current_timestamp()"
-
-    @classmethod
-    def is_cancelable(cls):
-        return False
-
-    @classmethod
-    def convert_text_type(cls, agate_table, col_idx):
-        return f"varchar({2000000})"
-
-    def _make_match_kwargs(
-        self, database: str, schema: str, identifier: str
-    ) -> Dict[str, str]:
-        quoting = self.config.quoting
-        if identifier is not None and quoting["identifier"] is False:
-            identifier = identifier.lower()
-
-        if schema is not None and quoting["schema"] is False:
-            schema = schema.lower()
-
-        if database is not None and quoting["database"] is False:
-            database = database.lower()
-
-        return filter_null_values(
-            {
-                "identifier": identifier,
-                "schema": schema,
-            }
-        )
-
-    @classmethod
-    def convert_number_type(cls, agate_table: agate.Table, col_idx: int) -> str:
-        decimals = agate_table.aggregate(agate.MaxPrecision(col_idx))
-        return "float" if decimals else "integer"
-
-    def timestamp_add_sql(
-        self, add_to: str, number: int = 1, interval: str = "hour"
-    ) -> str:
-        """
-        Overriding BaseAdapter default method because Exasol's syntax expects
-        the number in quotes without the interval
-        """
-        return f"{add_to} + interval '{number}' {interval}"
-
-    def quote_seed_column(self, column: str, quote_config: Optional[bool]) -> str:  # type: ignore
-        quote_columns: bool = False
-        if isinstance(quote_config, bool):
-            quote_columns = quote_config
-        elif quote_config is None:
-            pass
-        else:
-            raise CompilationError(
-                f'The seed configuration value of "quote_columns" has an '
-                f"invalid type {type(quote_config)}"
-            )
-
-        if quote_columns:
-            return self.quote(column)
-        return column
-
-    def valid_incremental_strategies(self):
-        """The set of standard builtin strategies which this adapter supports out-of-the-box.
-        Not used to validate custom strategies defined by end users.
-        """
+"""dbt-exasol Adapter implementation extending SQLAdapter"""
+from __future__ import absolute_import
+
+from typing import Dict, Optional
+
+import agate
+from dbt.adapters.sql import SQLAdapter
+from dbt.exceptions import CompilationError
+from dbt.utils import filter_null_values
+
+from dbt.adapters.exasol import (ExasolColumn, ExasolConnectionManager,
+                                 ExasolRelation)
+
+
+class ExasolAdapter(SQLAdapter):
+    """Exasol SQLAdapter extension"""
+
+    Relation = ExasolRelation
+    Column = ExasolColumn
+    ConnectionManager = ExasolConnectionManager
+
+    @classmethod
+    def date_function(cls):
+        return "current_timestamp()"
+
+    @classmethod
+    def is_cancelable(cls):
+        return False
+
+    @classmethod
+    def convert_text_type(cls, agate_table, col_idx):
+        return f"varchar({2000000})"
+
+    def _make_match_kwargs(
+        self, database: str, schema: str, identifier: str
+    ) -> Dict[str, str]:
+        quoting = self.config.quoting
+        if identifier is not None and quoting["identifier"] is False:
+            identifier = identifier.lower()
+
+        if schema is not None and quoting["schema"] is False:
+            schema = schema.lower()
+
+        if database is not None and quoting["database"] is False:
+            database = database.lower()
+
+        return filter_null_values(
+            {
+                "identifier": identifier,
+                "schema": schema,
+            }
+        )
+
+    @classmethod
+    def convert_number_type(cls, agate_table: agate.Table, col_idx: int) -> str:
+        decimals = agate_table.aggregate(agate.MaxPrecision(col_idx))
+        return "float" if decimals else "integer"
+
+    def timestamp_add_sql(
+        self, add_to: str, number: int = 1, interval: str = "hour"
+    ) -> str:
+        """
+        Overriding BaseAdapter default method because Exasol's syntax expects
+        the number in quotes without the interval
+        """
+        return f"{add_to} + interval '{number}' {interval}"
+
+    def quote_seed_column(self, column: str, quote_config: Optional[bool]) -> str:  # type: ignore
+        quote_columns: bool = False
+        if isinstance(quote_config, bool):
+            quote_columns = quote_config
+        elif quote_config is None:
+            pass
+        else:
+            raise CompilationError(
+                f'The seed configuration value of "quote_columns" has an '
+                f"invalid type {type(quote_config)}"
+            )
+
+        if quote_columns:
+            return self.quote(column)
+        return column
+
+    def valid_incremental_strategies(self):
+        """The set of standard builtin strategies which this adapter supports out-of-the-box.
+        Not used to validate custom strategies defined by end users.
+        """
         return ["append", "delete+insert"]
```

### Comparing `dbt_exasol-1.4.1/dbt/include/exasol/macros/adapters.sql` & `dbt_exasol-1.4.3/dbt/include/exasol/macros/adapters.sql`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,177 +1,177 @@
-
-/* 
-LIST_RELATIONS_MACRO_NAME = 'list_relations_without_caching'
-GET_COLUMNS_IN_RELATION_MACRO_NAME = 'get_columns_in_relation'
-LIST_SCHEMAS_MACRO_NAME = 'list_schemas'
-CHECK_SCHEMA_EXISTS_MACRO_NAME = 'check_schema_exists'
-CREATE_SCHEMA_MACRO_NAME = 'create_schema'
-DROP_SCHEMA_MACRO_NAME = 'drop_schema'
-RENAME_RELATION_MACRO_NAME = 'rename_relation'
-TRUNCATE_RELATION_MACRO_NAME = 'truncate_relation'
-DROP_RELATION_MACRO_NAME = 'drop_relation'
-ALTER_COLUMN_TYPE_MACRO_NAME = 'alter_column_type'
- */
-
-
-{% macro exasol__list_relations_without_caching(schema) %}
-{% call statement('list_relations_without_caching', fetch_result=True) -%}
-    select
-      'db' as [database],
-      lower(table_name) as [name],
-      lower(table_schema) as [schema],
-  	  lower(table_type) as table_type
-    from (
-		select table_name,table_schema,'table' as table_type from sys.exa_all_tables
-		union
-		select view_name, view_schema,'view' from sys.exa_all_views
-	  )
-    where upper(table_schema) = '{{ schema |upper }}'
-{% endcall %}  
-{{ return(load_result('list_relations_without_caching').table) }}
-{% endmacro %}
-
-{% macro exasol__list_schemas(database) %}
-  {% call statement('list_schemas', fetch_result=True, auto_begin=False) -%}
-    select schema_name as [schema] from exa_schemas
-  {% endcall %}
-  {{ return(load_result('list_schemas').table) }}
-{% endmacro %}
-
-{% macro exasol__create_schema(relation) -%}  
-  {%- call statement('create_schema') -%}
-    create schema if not exists {{ relation.without_identifier() }}
-  {% endcall %}
-{% endmacro %}
-
-{% macro exasol__drop_schema(relation) -%}
-  {% call statement('drop_schema') -%}
-    drop schema if exists {{relation}} cascade
-  {% endcall %}
-{% endmacro %}
-
-{% macro exasol__drop_relation(relation) -%}
-  {% call statement('drop_relation', fetch_result=True) -%}
-    drop {{ relation.type }} if exists {{ relation.schema }}.{{ relation.identifier }}
-  {%- endcall %}
-{% endmacro %}
-
-{% macro exasol__check_schema_exists(database, schema) -%}
-  {% call statement('check_schema_exists', fetch_result=True, auto_begin=False) -%}
-    select count(*) as schema_exist from (
-		select schema_name as [schema] from exa_schemas
-    ) WHERE upper([schema]) = '{{ schema | upper }}'
-  {%- endcall %}
-  {{ return(load_result('check_schema_exists').table) }}
-{% endmacro %}
-
-{% macro exasol__create_view_as(relation, sql) -%}
-CREATE OR REPLACE VIEW {{ relation.schema }}.{{ relation.identifier }} 
-{{- persist_view_column_docs(relation, sql) }}
-AS 
-(
-    {{ sql | indent(4) }}
-)
-{{ persist_view_relation_docs() }}
-{% endmacro %}
-
-{% macro exasol__rename_relation(from_relation, to_relation) -%}
-  {% call statement('rename_relation') -%}
-    RENAME {{ from_relation.type }} {{ from_relation.schema }}.{{ from_relation.identifier }} TO {{ to_relation.identifier }}
-  {%- endcall %}
-{% endmacro %}
-
-{% macro exasol__create_table_as(temporary, relation, sql) -%}
-    CREATE OR REPLACE TABLE {{ relation.schema }}.{{ relation.identifier }} AS 
-    {{ sql }}
-{% endmacro %}
-
-{% macro exasol__truncate_relation(relation) -%}
-  {% call statement('truncate_relation') -%}
-    truncate table {{ relation | replace('"', '') }}
-  {%- endcall %}
-{% endmacro %}
-
-{% macro exasol__get_columns_in_relation(relation) -%}
-  {% call statement('get_columns_in_relation', fetch_result=True) %}
-      select
-          column_name,
-          regexp_substr(column_type, '[A-Za-z]+', 1) as column_type,
-          column_maxsize,
-          column_num_prec,
-          column_num_scale
-      from exa_all_columns
-      where upper(column_table) = '{{ relation.identifier|upper }}'
-        and upper(column_schema) = '{{ relation.schema|upper }}'
-      order by column_ordinal_position
-
-  {% endcall %}
-  {% set table = load_result('get_columns_in_relation').table %}
-  {{ return(sql_convert_columns_in_relation(table)) }}
-{% endmacro %}
-
-{% macro exasol__get_columns_in_query(select_sql) %}
-    {% call statement('get_columns_in_query', fetch_result=True, auto_begin=False) -%}
-        select * from (
-            {{ select_sql }}
-        ) as dbt_sbq
-        where false
-        limit 0
-    {% endcall %}
-
-    {{ return(load_result('get_columns_in_query').table.columns | map(attribute='name') | list) }}
-{% endmacro %}
-
-{% macro exasol__alter_relation_comment(relation, relation_comment) -%}
-  {%- set comment = relation_comment | replace("'", '"') %}
-  COMMENT ON {{ relation.type }} {{ relation }} IS '{{ comment }}';
-{% endmacro %}
-
-{% macro get_column_comment_sql(column_name, column_dict, apply_comment=false) -%}
-  {% if (column_name|upper in column_dict) -%}
-    {% set matched_column = column_name|upper -%}
-  {% elif (column_name|lower in column_dict) -%}
-    {% set matched_column = column_name|lower -%}
-  {% elif (column_name in column_dict) -%}
-    {% set matched_column = column_name -%}
-  {% else -%}
-    {% set matched_column = None -%}
-  {% endif -%}
-  {% if matched_column -%}
-    {% set comment = column_dict[matched_column]['description'] | replace("'", '"') -%}
-  {% else -%}
-    {% set comment = "" -%}
-  {% endif -%}
-  {{ adapter.quote(column_name) }} {{ "COMMENT" if apply_comment }} IS '{{ comment }}'
-{%- endmacro %}
-
-{% macro exasol__alter_column_comment(relation, column_dict) -%}
-    {% set query_columns = get_columns_in_query(sql) %} 
-    COMMENT ON {{ relation.type }} {{ relation }} (
-    {% for column_name in query_columns %}
-        {{ get_column_comment_sql(column_name, column_dict) }} {{- ',' if not loop.last }}
-    {% endfor %}
-    );
-{% endmacro %}
-
-{% macro persist_view_column_docs(relation, sql) %}
-{%- if config.persist_column_docs() %}
-(
-  {% set query_columns = get_columns_in_query(sql) %}
-  {%- for column_name in query_columns %}
-      {{ get_column_comment_sql(column_name, model.columns, true) -}}{{ ',' if not loop.last -}}
-  {%- endfor %}
-)
-{%- endif %}
-{%- endmacro %}
-
-{% macro persist_view_relation_docs() %}
-{%- if config.persist_relation_docs() %}
-COMMENT IS '{{ model.description }}'
-{%- endif %}
-{% endmacro %}
-
-{% macro exasol__alter_column_type(relation, column_name, new_column_type) -%}
-  {% call statement('alter_column_type') %}
-    alter table {{ relation }} modify column {{ adapter.quote(column_name) }} {{ new_column_type }};
-  {% endcall %}
+
+/* 
+LIST_RELATIONS_MACRO_NAME = 'list_relations_without_caching'
+GET_COLUMNS_IN_RELATION_MACRO_NAME = 'get_columns_in_relation'
+LIST_SCHEMAS_MACRO_NAME = 'list_schemas'
+CHECK_SCHEMA_EXISTS_MACRO_NAME = 'check_schema_exists'
+CREATE_SCHEMA_MACRO_NAME = 'create_schema'
+DROP_SCHEMA_MACRO_NAME = 'drop_schema'
+RENAME_RELATION_MACRO_NAME = 'rename_relation'
+TRUNCATE_RELATION_MACRO_NAME = 'truncate_relation'
+DROP_RELATION_MACRO_NAME = 'drop_relation'
+ALTER_COLUMN_TYPE_MACRO_NAME = 'alter_column_type'
+ */
+
+
+{% macro exasol__list_relations_without_caching(schema) %}
+{% call statement('list_relations_without_caching', fetch_result=True) -%}
+    select
+      'db' as [database],
+      lower(table_name) as [name],
+      lower(table_schema) as [schema],
+  	  lower(table_type) as table_type
+    from (
+		select table_name,table_schema,'table' as table_type from sys.exa_all_tables
+		union
+		select view_name, view_schema,'view' from sys.exa_all_views
+	  )
+    where upper(table_schema) = '{{ schema |upper }}'
+{% endcall %}  
+{{ return(load_result('list_relations_without_caching').table) }}
+{% endmacro %}
+
+{% macro exasol__list_schemas(database) %}
+  {% call statement('list_schemas', fetch_result=True, auto_begin=False) -%}
+    select schema_name as [schema] from exa_schemas
+  {% endcall %}
+  {{ return(load_result('list_schemas').table) }}
+{% endmacro %}
+
+{% macro exasol__create_schema(relation) -%}  
+  {%- call statement('create_schema') -%}
+    create schema if not exists {{ relation.without_identifier() }}
+  {% endcall %}
+{% endmacro %}
+
+{% macro exasol__drop_schema(relation) -%}
+  {% call statement('drop_schema') -%}
+    drop schema if exists {{relation}} cascade
+  {% endcall %}
+{% endmacro %}
+
+{% macro exasol__drop_relation(relation) -%}
+  {% call statement('drop_relation', fetch_result=True) -%}
+    drop {{ relation.type }} if exists {{ relation.schema }}.{{ relation.identifier }}
+  {%- endcall %}
+{% endmacro %}
+
+{% macro exasol__check_schema_exists(database, schema) -%}
+  {% call statement('check_schema_exists', fetch_result=True, auto_begin=False) -%}
+    select count(*) as schema_exist from (
+		select schema_name as [schema] from exa_schemas
+    ) WHERE upper([schema]) = '{{ schema | upper }}'
+  {%- endcall %}
+  {{ return(load_result('check_schema_exists').table) }}
+{% endmacro %}
+
+{% macro exasol__create_view_as(relation, sql) -%}
+CREATE OR REPLACE VIEW {{ relation.schema }}.{{ relation.identifier }} 
+{{- persist_view_column_docs(relation, sql) }}
+AS 
+(
+    {{ sql | indent(4) }}
+)
+{{ persist_view_relation_docs() }}
+{% endmacro %}
+
+{% macro exasol__rename_relation(from_relation, to_relation) -%}
+  {% call statement('rename_relation') -%}
+    RENAME {{ from_relation.type }} {{ from_relation.schema }}.{{ from_relation.identifier }} TO {{ to_relation.identifier }}
+  {%- endcall %}
+{% endmacro %}
+
+{% macro exasol__create_table_as(temporary, relation, sql) -%}
+    CREATE OR REPLACE TABLE {{ relation.schema }}.{{ relation.identifier }} AS 
+    {{ sql }}
+{% endmacro %}
+
+{% macro exasol__truncate_relation(relation) -%}
+  {% call statement('truncate_relation') -%}
+    truncate table {{ relation | replace('"', '') }}
+  {%- endcall %}
+{% endmacro %}
+
+{% macro exasol__get_columns_in_relation(relation) -%}
+  {% call statement('get_columns_in_relation', fetch_result=True) %}
+      select
+          column_name,
+          regexp_substr(column_type, '[A-Za-z]+', 1) as column_type,
+          column_maxsize,
+          column_num_prec,
+          column_num_scale
+      from exa_all_columns
+      where upper(column_table) = '{{ relation.identifier|upper }}'
+        and upper(column_schema) = '{{ relation.schema|upper }}'
+      order by column_ordinal_position
+
+  {% endcall %}
+  {% set table = load_result('get_columns_in_relation').table %}
+  {{ return(sql_convert_columns_in_relation(table)) }}
+{% endmacro %}
+
+{% macro exasol__get_columns_in_query(select_sql) %}
+    {% call statement('get_columns_in_query', fetch_result=True, auto_begin=False) -%}
+        select * from (
+            {{ select_sql }}
+        ) as dbt_sbq
+        where false
+        limit 0
+    {% endcall %}
+
+    {{ return(load_result('get_columns_in_query').table.columns | map(attribute='name') | list) }}
+{% endmacro %}
+
+{% macro exasol__alter_relation_comment(relation, relation_comment) -%}
+  {%- set comment = relation_comment | replace("'", '"') %}
+  COMMENT ON {{ relation.type }} {{ relation }} IS '{{ comment }}';
+{% endmacro %}
+
+{% macro get_column_comment_sql(column_name, column_dict, apply_comment=false) -%}
+  {% if (column_name|upper in column_dict) -%}
+    {% set matched_column = column_name|upper -%}
+  {% elif (column_name|lower in column_dict) -%}
+    {% set matched_column = column_name|lower -%}
+  {% elif (column_name in column_dict) -%}
+    {% set matched_column = column_name -%}
+  {% else -%}
+    {% set matched_column = None -%}
+  {% endif -%}
+  {% if matched_column -%}
+    {% set comment = column_dict[matched_column]['description'] | replace("'", '"') -%}
+  {% else -%}
+    {% set comment = "" -%}
+  {% endif -%}
+  {{ adapter.quote(column_name) }} {{ "COMMENT" if apply_comment }} IS '{{ comment }}'
+{%- endmacro %}
+
+{% macro exasol__alter_column_comment(relation, column_dict) -%}
+    {% set query_columns = get_columns_in_query(sql) %} 
+    COMMENT ON {{ relation.type }} {{ relation }} (
+    {% for column_name in query_columns %}
+        {{ get_column_comment_sql(column_name, column_dict) }} {{- ',' if not loop.last }}
+    {% endfor %}
+    );
+{% endmacro %}
+
+{% macro persist_view_column_docs(relation, sql) %}
+{%- if config.persist_column_docs() %}
+(
+  {% set query_columns = get_columns_in_query(sql) %}
+  {%- for column_name in query_columns %}
+      {{ get_column_comment_sql(column_name, model.columns, true) -}}{{ ',' if not loop.last -}}
+  {%- endfor %}
+)
+{%- endif %}
+{%- endmacro %}
+
+{% macro persist_view_relation_docs() %}
+{%- if config.persist_relation_docs() %}
+COMMENT IS '{{ model.description }}'
+{%- endif %}
+{% endmacro %}
+
+{% macro exasol__alter_column_type(relation, column_name, new_column_type) -%}
+  {% call statement('alter_column_type') %}
+    alter table {{ relation }} modify column {{ adapter.quote(column_name) }} {{ new_column_type }};
+  {% endcall %}
 {% endmacro %}
```

### Comparing `dbt_exasol-1.4.1/dbt/include/exasol/macros/apply_grants.sql` & `dbt_exasol-1.4.3/dbt/include/exasol/macros/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.4.1/dbt/include/exasol/macros/catalog.sql` & `dbt_exasol-1.4.3/dbt/include/exasol/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.4.1/dbt/include/exasol/macros/materializations/incremental.sql` & `dbt_exasol-1.4.3/dbt/include/exasol/macros/materializations/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.4.1/dbt/include/exasol/macros/materializations/merge.sql` & `dbt_exasol-1.4.3/dbt/include/exasol/macros/materializations/merge.sql`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-{% macro exasol__get_delete_insert_merge_sql(target, source, unique_key, dest_columns,incremental_predicates=none) -%}
-
-    {%- set dest_cols_csv = get_quoted_csv(dest_columns | map(attribute="name")) -%}
-
-    {% if unique_key %}
-        {% if unique_key is sequence and unique_key is not string %}
-            delete from {{ target }}
-            where exists ( select 1 from {{ source }}
-                where
-                {% for key in unique_key %}
-                    {{ source }}.{{ key }} = {{ target }}.{{ key }}
-                    {{ "and " if not loop.last }}
-                {% endfor %}
-            )
-        {% else %}
-            delete from {{ target }}
-            where (
-                {{ unique_key }}) in (
-                select ({{ unique_key }})
-                from {{ source }}
-            )
-
-        {% endif %}
-    {% endif %}
-
-    |SEPARATEMEPLEASE|
-
-    insert into {{ target }} ({{ dest_cols_csv }})
-    (
-        select {{ dest_cols_csv }}
-        from {{ source }}
-    )
-
-{%- endmacro %}
+{% macro exasol__get_delete_insert_merge_sql(target, source, unique_key, dest_columns,incremental_predicates=none) -%}
+
+    {%- set dest_cols_csv = get_quoted_csv(dest_columns | map(attribute="name")) -%}
+
+    {% if unique_key %}
+        {% if unique_key is sequence and unique_key is not string %}
+            delete from {{ target }}
+            where exists ( select 1 from {{ source }}
+                where
+                {% for key in unique_key %}
+                    {{ source }}.{{ key }} = {{ target }}.{{ key }}
+                    {{ "and " if not loop.last }}
+                {% endfor %}
+            )
+        {% else %}
+            delete from {{ target }}
+            where (
+                {{ unique_key }}) in (
+                select ({{ unique_key }})
+                from {{ source }}
+            )
+
+        {% endif %}
+    {% endif %}
+
+    |SEPARATEMEPLEASE|
+
+    insert into {{ target }} ({{ dest_cols_csv }})
+    (
+        select {{ dest_cols_csv }}
+        from {{ source }}
+    )
+
+{%- endmacro %}
```

### Comparing `dbt_exasol-1.4.1/dbt/include/exasol/macros/materializations/snapshot.sql` & `dbt_exasol-1.4.3/dbt/include/exasol/macros/materializations/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.4.1/dbt/include/exasol/macros/materializations/snapshot_merge.sql` & `dbt_exasol-1.4.3/dbt/include/exasol/macros/materializations/snapshot_merge.sql`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.4.1/dbt/include/exasol/macros/materializations/strategies.sql` & `dbt_exasol-1.4.3/dbt/include/exasol/macros/materializations/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.4.1/dbt/include/exasol/macros/materializations/table.sql` & `dbt_exasol-1.4.3/dbt/include/exasol/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.4.1/dbt/include/exasol/macros/utils/safe_cast.sql` & `dbt_exasol-1.4.3/dbt/include/exasol/macros/utils/safe_cast.sql`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.4.1/pyproject.toml` & `dbt_exasol-1.4.3/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-[tool.poetry]
-name = "dbt-exasol"
-version = "1.4.1"
-description = "Adapter to dbt-core for warehouse Exasol"
-authors = ["Torsten Glunde <torsten.glunde@alligator-company.com>", "Ilija Kutle <ilija.kutle@alligator-company.com>"]
-homepage = "https://alligatorcompany.gitlab.io/dbt-exasol"
-repository = "https://github.com/tglunde/dbt-exasol"
-packages = [
-  { include = "dbt" },
-  { include = "dbt/**/*.py" },
-  { include = "tests/**/*.py"}
-]
-license = "GPL3"
-readme = "README.md"
-
-[tool.poetry.dependencies]
-python = "^3.8, <3.12"
-dbt-core = "^1.4, <1.5"
-pyexasol = "^0.25.0"
-sqlfluff = "^2.0.2"
-
-[tool.poetry.group.dev.dependencies]
-pylint = "^2.15.8"
-exceptiongroup = "^1.1.1"
-black = "^22.8.0"
-pytest = "^7.1.3"
-pytest-dotenv = "^0.5.2"
-tox = "^3.26.0"
-dbt-tests-adapter = "^1.4, <1.5"
-pytest-parallel = "^0.1.1"
-
-[build-system]
-requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
+[tool.poetry]
+name = "dbt-exasol"
+version = "1.4.3"
+description = "Adapter to dbt-core for warehouse Exasol"
+authors = ["Torsten Glunde <torsten.glunde@alligator-company.com>", "Ilija Kutle <ilija.kutle@alligator-company.com>"]
+homepage = "https://alligatorcompany.gitlab.io/dbt-exasol"
+repository = "https://github.com/tglunde/dbt-exasol"
+packages = [
+  { include = "dbt" },
+  { include = "dbt/**/*.py" },
+  { include = "tests/**/*.py"}
+]
+license = "GPL3"
+readme = "README.md"
+
+[tool.poetry.dependencies]
+python = "^3.8, <3.12"
+dbt-core = "^1.4, <1.5"
+pyexasol = "^0.25.0"
+sqlfluff = "^2.0.2"
+
+[tool.poetry.group.dev.dependencies]
+pylint = "^2.15.8"
+exceptiongroup = "^1.1.1"
+black = "^22.8.0"
+pytest = "^7.1.3"
+pytest-dotenv = "^0.5.2"
+tox = "^3.26.0"
+dbt-tests-adapter = "^1.4, <1.5"
+pytest-parallel = "^0.1.1"
+
+[build-system]
+requires = ["poetry-core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `dbt_exasol-1.4.1/tests/conftest.py` & `dbt_exasol-1.4.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.4.1/tests/functional/adapter/expected_catalog.py` & `dbt_exasol-1.4.3/tests/functional/adapter/expected_catalog.py`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.4.1/tests/functional/adapter/files.py` & `dbt_exasol-1.4.3/tests/functional/adapter/files.py`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.4.1/tests/functional/adapter/fixtures.py` & `dbt_exasol-1.4.3/tests/functional/adapter/fixtures.py`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.4.1/tests/functional/adapter/query_comment_tests/test_query_comment.py` & `dbt_exasol-1.4.3/tests/functional/adapter/query_comment_tests/test_query_comment.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-from dbt.tests.adapter.query_comment.test_query_comment import (
-    BaseEmptyQueryComments,
-    BaseMacroArgsQueryComments,
-    BaseMacroInvalidQueryComments,
-    BaseMacroQueryComments,
-    BaseNullQueryComments,
-    BaseQueryComments,
-)
-
-
-class TestQueryCommentsExasol(BaseQueryComments):
-    pass
-
-
-class TestMacroQueryCommentsExasol(BaseMacroQueryComments):
-    pass
-
-
-class TestMacroArgsQueryCommentsExasol(BaseMacroArgsQueryComments):
-    pass
-
-
-class TestMacroInvalidQueryCommentsExasol(BaseMacroInvalidQueryComments):
-    pass
-
-
-class TestNullQueryCommentsExasol(BaseNullQueryComments):
-    pass
-
-
-class TestEmptyQueryCommentsExasol(BaseEmptyQueryComments):
-    pass
+from dbt.tests.adapter.query_comment.test_query_comment import (
+    BaseEmptyQueryComments,
+    BaseMacroArgsQueryComments,
+    BaseMacroInvalidQueryComments,
+    BaseMacroQueryComments,
+    BaseNullQueryComments,
+    BaseQueryComments,
+)
+
+
+class TestQueryCommentsExasol(BaseQueryComments):
+    pass
+
+
+class TestMacroQueryCommentsExasol(BaseMacroQueryComments):
+    pass
+
+
+class TestMacroArgsQueryCommentsExasol(BaseMacroArgsQueryComments):
+    pass
+
+
+class TestMacroInvalidQueryCommentsExasol(BaseMacroInvalidQueryComments):
+    pass
+
+
+class TestNullQueryCommentsExasol(BaseNullQueryComments):
+    pass
+
+
+class TestEmptyQueryCommentsExasol(BaseEmptyQueryComments):
+    pass
```

### Comparing `dbt_exasol-1.4.1/tests/functional/adapter/test_basic.py` & `dbt_exasol-1.4.3/tests/functional/adapter/test_basic.py`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.4.1/tests/functional/adapter/test_concurrency.py` & `dbt_exasol-1.4.3/tests/functional/adapter/test_concurrency.py`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.4.1/tests/functional/adapter/test_docs_generate.py` & `dbt_exasol-1.4.3/tests/functional/adapter/test_docs_generate.py`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.4.1/tests/functional/adapter/test_failing_test.py` & `dbt_exasol-1.4.3/tests/functional/adapter/test_failing_test.py`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.4.1/tests/functional/adapter/utils/data_types/test_type_bigint.py` & `dbt_exasol-1.4.3/tests/functional/adapter/utils/data_types/test_type_bigint.py`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.4.1/tests/functional/adapter/utils/test_timestamps.py` & `dbt_exasol-1.4.3/tests/functional/adapter/utils/test_timestamps.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-import pytest
-from dbt.tests.adapter.utils.test_timestamps import BaseCurrentTimestamps
-
-_MODEL_CURRENT_TIMESTAMP = """
-select {{ current_timestamp() }} as curr_timestamp,
-       {{ current_timestamp_in_utc_backcompat() }} as current_timestamp_in_utc_backcompat,
-       {{ current_timestamp_backcompat() }} as current_timestamp_backcompat
-"""
-
-_MODEL_EXPECTED_SQL = """
-select current_timestamp() as curr_timestamp,
-       current_timestamp() as current_timestamp_in_utc_backcompat,
-       current_timestamp() as current_timestamp_backcompat
-"""
-
-
-class TestCurrentTimestampsExasol(BaseCurrentTimestamps):
-    @pytest.fixture(scope="class")
-    def models(self):
-        return {"get_current_timestamp.sql": _MODEL_CURRENT_TIMESTAMP}
-
-    # any adapters that don't want to check can set expected schema to None
-    @pytest.fixture(scope="class")
-    def expected_sql(self):
-        return _MODEL_EXPECTED_SQL
-
-    @pytest.fixture(scope="class")
-    def expected_schema(self):
-        return {
-            "CURR_TIMESTAMP": "TIMESTAMP",
-            "CURRENT_TIMESTAMP_IN_UTC_BACKCOMPAT": "TIMESTAMP",
-            "CURRENT_TIMESTAMP_BACKCOMPAT": "TIMESTAMP",
-        }
+import pytest
+from dbt.tests.adapter.utils.test_timestamps import BaseCurrentTimestamps
+
+_MODEL_CURRENT_TIMESTAMP = """
+select {{ current_timestamp() }} as curr_timestamp,
+       {{ current_timestamp_in_utc_backcompat() }} as current_timestamp_in_utc_backcompat,
+       {{ current_timestamp_backcompat() }} as current_timestamp_backcompat
+"""
+
+_MODEL_EXPECTED_SQL = """
+select current_timestamp() as curr_timestamp,
+       current_timestamp() as current_timestamp_in_utc_backcompat,
+       current_timestamp() as current_timestamp_backcompat
+"""
+
+
+class TestCurrentTimestampsExasol(BaseCurrentTimestamps):
+    @pytest.fixture(scope="class")
+    def models(self):
+        return {"get_current_timestamp.sql": _MODEL_CURRENT_TIMESTAMP}
+
+    # any adapters that don't want to check can set expected schema to None
+    @pytest.fixture(scope="class")
+    def expected_sql(self):
+        return _MODEL_EXPECTED_SQL
+
+    @pytest.fixture(scope="class")
+    def expected_schema(self):
+        return {
+            "CURR_TIMESTAMP": "TIMESTAMP",
+            "CURRENT_TIMESTAMP_IN_UTC_BACKCOMPAT": "TIMESTAMP",
+            "CURRENT_TIMESTAMP_BACKCOMPAT": "TIMESTAMP",
+        }
```

### Comparing `dbt_exasol-1.4.1/tests/functional/adapter/utils/utils_fixtures.py` & `dbt_exasol-1.4.3/tests/functional/adapter/utils/utils_fixtures.py`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.4.1/tests/functional/test_incremental.py` & `dbt_exasol-1.4.3/tests/functional/test_incremental.py`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.4.1/tests/functional/test_issues.py` & `dbt_exasol-1.4.3/tests/functional/test_issues.py`

 * *Files identical despite different names*

### Comparing `dbt_exasol-1.4.1/PKG-INFO` & `dbt_exasol-1.4.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-exasol
-Version: 1.4.1
+Version: 1.4.3
 Summary: Adapter to dbt-core for warehouse Exasol
 Home-page: https://alligatorcompany.gitlab.io/dbt-exasol
 License: GPL3
 Author: Torsten Glunde
 Author-email: torsten.glunde@alligator-company.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: Other/Proprietary License
@@ -37,14 +37,17 @@
       dsn: HOST:PORT
       user: USERNAME
       password: PASSWORD
       dbname: db
       schema: SCHEMA
 ```
 
+#### Optional login credentials using OpenID for Exasol SaaS
+OpenID login through access_token or refresh_token instead of user+password
+
 #### Optional parameters
 <ul>
   <li><strong>connection_timeout</strong>: defaults to pyexasol default</li>
   <li><strong>socket_timeout</strong>: defaults to pyexasol default</li>
   <li><strong>query_timeout</strong>: defaults to pyexasol default</li>
   <li><strong>compression</strong>: default: False</li>
   <li><strong>encryption</strong>: default: False</li>
```

