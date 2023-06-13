# Comparing `tmp/databend-py-0.4.4.tar.gz` & `tmp/databend-py-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databend-py-0.4.4.tar", last modified: Wed Jun  7 04:40:05 2023, max compression
+gzip compressed data, was "databend-py-0.4.5.tar", last modified: Tue Jun 13 03:34:19 2023, max compression
```

## Comparing `databend-py-0.4.4.tar` & `databend-py-0.4.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:40:05.448525 databend-py-0.4.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-07 04:39:52.000000 databend-py-0.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-06-07 04:40:05.448525 databend-py-0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-06-07 04:39:52.000000 databend-py-0.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:40:05.448525 databend-py-0.4.4/databend_py/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-07 04:39:52.000000 databend-py-0.4.4/databend_py/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9756 2023-06-07 04:39:52.000000 databend-py-0.4.4/databend_py/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7348 2023-06-07 04:39:52.000000 databend-py-0.4.4/databend_py/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-06-07 04:39:52.000000 databend-py-0.4.4/databend_py/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-07 04:39:52.000000 databend-py-0.4.4/databend_py/datetypes.py
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-07 04:39:52.000000 databend-py-0.4.4/databend_py/defines.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-06-07 04:39:52.000000 databend-py-0.4.4/databend_py/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-07 04:39:52.000000 databend-py-0.4.4/databend_py/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-06-07 04:39:52.000000 databend-py-0.4.4/databend_py/result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-07 04:39:52.000000 databend-py-0.4.4/databend_py/retry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-06-07 04:39:52.000000 databend-py-0.4.4/databend_py/uploader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:40:05.448525 databend-py-0.4.4/databend_py/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 04:39:52.000000 databend-py-0.4.4/databend_py/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-06-07 04:39:52.000000 databend-py-0.4.4/databend_py/util/escape.py
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-06-07 04:39:52.000000 databend-py-0.4.4/databend_py/util/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:40:05.448525 databend-py-0.4.4/databend_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-06-07 04:40:05.000000 databend-py-0.4.4/databend_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-07 04:40:05.000000 databend-py-0.4.4/databend_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 04:40:05.000000 databend-py-0.4.4/databend_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-07 04:40:05.000000 databend-py-0.4.4/databend_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-07 04:40:05.000000 databend-py-0.4.4/databend_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-07 04:40:05.448525 databend-py-0.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-06-07 04:39:52.000000 databend-py-0.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:34:19.224169 databend-py-0.4.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-13 03:34:07.000000 databend-py-0.4.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-06-13 03:34:19.224169 databend-py-0.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-06-13 03:34:07.000000 databend-py-0.4.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:34:19.224169 databend-py-0.4.5/databend_py/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-13 03:34:07.000000 databend-py-0.4.5/databend_py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10176 2023-06-13 03:34:07.000000 databend-py-0.4.5/databend_py/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7546 2023-06-13 03:34:07.000000 databend-py-0.4.5/databend_py/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-06-13 03:34:07.000000 databend-py-0.4.5/databend_py/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-13 03:34:07.000000 databend-py-0.4.5/databend_py/datetypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-13 03:34:07.000000 databend-py-0.4.5/databend_py/defines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-06-13 03:34:07.000000 databend-py-0.4.5/databend_py/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-13 03:34:07.000000 databend-py-0.4.5/databend_py/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-06-13 03:34:07.000000 databend-py-0.4.5/databend_py/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-13 03:34:07.000000 databend-py-0.4.5/databend_py/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7029 2023-06-13 03:34:07.000000 databend-py-0.4.5/databend_py/uploader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:34:19.224169 databend-py-0.4.5/databend_py/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 03:34:07.000000 databend-py-0.4.5/databend_py/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-06-13 03:34:07.000000 databend-py-0.4.5/databend_py/util/escape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-06-13 03:34:07.000000 databend-py-0.4.5/databend_py/util/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:34:19.224169 databend-py-0.4.5/databend_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-06-13 03:34:19.000000 databend-py-0.4.5/databend_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-13 03:34:19.000000 databend-py-0.4.5/databend_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 03:34:19.000000 databend-py-0.4.5/databend_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-13 03:34:19.000000 databend-py-0.4.5/databend_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-13 03:34:19.000000 databend-py-0.4.5/databend_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-13 03:34:19.224169 databend-py-0.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-06-13 03:34:07.000000 databend-py-0.4.5/setup.py
```

### Comparing `databend-py-0.4.4/LICENSE` & `databend-py-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `databend-py-0.4.4/PKG-INFO` & `databend-py-0.4.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databend-py
-Version: 0.4.4
+Version: 0.4.5
 Summary: Python driver with native interface for Databend
 Home-page: https://github.com/databendcloud/databend-py
 Author: Databend Cloud Team
 Author-email: hantmac@outlook.com
 License: Apache License
 Keywords: databend db database cloud analytics
 Platform: UNKNOWN
@@ -82,14 +82,16 @@
 > ...     'INSERT INTO test (x) VALUES', [(1,)]
 > ... )
 > 1
 > >>> client.execute('INSERT INTO test (x) VALUES', [(200,)])
 > 1
 > ```
 
+More usages examples find [here](./examples).
+
 # Features
 
 -   Basic SQL.
 -   TLS support.
 -   Query settings.
 -   Types support:
     -   Float32/64
```

### Comparing `databend-py-0.4.4/README.md` & `databend-py-0.4.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,16 @@
 > ...     'INSERT INTO test (x) VALUES', [(1,)]
 > ... )
 > 1
 > >>> client.execute('INSERT INTO test (x) VALUES', [(200,)])
 > 1
 > ```
 
+More usages examples find [here](./examples).
+
 # Features
 
 -   Basic SQL.
 -   TLS support.
 -   Query settings.
 -   Types support:
     -   Float32/64
```

### Comparing `databend-py-0.4.4/databend_py/client.py` & `databend-py-0.4.5/databend_py/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import json
-import re
 from urllib.parse import urlparse, parse_qs, unquote
 
 from .connection import Connection
 from .uploader import DataUploader
 from .result import QueryResult
 from .util.escape import escape_params
 from .util.helper import asbool, Helper
@@ -17,15 +16,16 @@
 
     def __init__(self, *args, **kwargs):
         self.settings = (kwargs.pop('settings', None) or {}).copy()
         self.connection = Connection(*args, **kwargs)
         self.query_result_cls = QueryResult
         self.helper = Helper
         self._debug = asbool(self.settings.get('debug', False))
-        self._uploader = DataUploader(self, self.settings, debug=self._debug, compress=self.settings.get('compress', False))
+        self._uploader = DataUploader(self, self.connection, self.settings, debug=self._debug,
+                                      compress=self.settings.get('compress', False))
 
     def __enter__(self):
         return self
 
     def disconnect(self):
         self.disconnect_connection()
 
@@ -118,25 +118,22 @@
     # params = [(1,),(2,)] or params = [(1,2),(2,3)]
     def _process_insert_query(self, query, params):
         insert_rows = 0
         if "values" in query:
             query = query.split("values")[0] + 'values'
         elif "VALUES" in query:
             query = query.split("VALUES")[0] + 'VALUES'
-        insert_re = re.compile("(?i)^INSERT INTO\s+\x60?([\w.^\(]+)\x60?\s*(\([^\)]*\))?")
-        match = insert_re.match(query.strip())
-        if len(match.group().split(' ')) < 2:
-            raise Exception("Not standard insert statement")
-        table_name = match[1]
-
+        if len(query.split(' ')) < 3:
+            raise Exception("Not standard insert/replace statement")
+        table_name = query.split(' ')[2]
         batch_size = query.count(',') + 1
         if params is not None:
             tuple_ls = [tuple(params[i:i + batch_size]) for i in range(0, len(params), batch_size)]
             insert_rows = len(tuple_ls)
-            self._uploader.upload_to_table(table_name, tuple_ls)
+            self._uploader.upload_to_table_by_copy(table_name, tuple_ls)
         return insert_rows
 
     def _process_ordinary_query(self, query, params=None, with_column_types=False,
                                 query_id=None):
         if params is not None:
             query = self._substitute_params(
                 query, params, self.connection.context
@@ -235,18 +232,28 @@
         """
         insert the data into database.table according to the file
         database_name: the target database
         table_name: the table which write into
         data: the data which write into, it's a list of tuple
         """
         # TODO: escape the database & table name
-        self._uploader.upload_to_table("%s.%s" % (database_name, table_name), data)
+        self._uploader.upload_to_table_by_copy("%s.%s" % (database_name, table_name), data)
+
+    def replace(self, database_name, table_name, conflict_keys, data):
+        """
+        replace the data into database.table according to the file
+        database_name: the target database
+        table_name: the table which write into
+        conflict_keys: the key that use to replace into
+        data: the data which write into, it's a list of tuple
+        """
+        self._uploader.upload_to_table_with_attachment("%s.%s" % (database_name, table_name), conflict_keys, data)
 
     def upload_to_stage(self, stage_dir, file_name, data):
         """
         upload the file to user stage
         :param stage_dir: target stage directory
         :param file_name: the target file name which placed into the stage_dir
         :param data: the data value or file handler
         :return:
         """
-        return self._uploader.upload_to_stage(stage_dir, file_name, data)
+        return self._uploader.upload_to_stage(stage_dir, file_name, data)
```

### Comparing `databend-py-0.4.4/databend_py/connection.py` & `databend-py-0.4.5/databend_py/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,16 @@
     # {
     #   'user': 'root',
     #   'host': '127.0.0.1',
     #   'port': 3307,
     #   'database': 'default'
     # }
     def __init__(self, host, port=None, user=defines.DEFAULT_USER, password=defines.DEFAULT_PASSWORD,
-                 database=defines.DEFAULT_DATABASE, secure=False, copy_purge=False, session_settings=None, persist_cookies=False):
+                 database=defines.DEFAULT_DATABASE, secure=False, copy_purge=False, session_settings=None,
+                 persist_cookies=False):
         self.host = host
         self.port = port
         self.user = user
         self.password = password
         self.database = database
         self.secure = secure
         self.copy_purge = copy_purge
@@ -112,24 +113,26 @@
 
     def disconnect(self):
         self.client_session = dict()
 
     @retry(times=5, exceptions=WarehouseTimeoutException)
     def do_query(self, url, query_sql):
         response = self.requests_session.post(url,
-                                 data=json.dumps(query_sql),
-                                 headers=self.make_headers(),
-                                 auth=HTTPBasicAuth(self.user, self.password),
-                                 verify=True)
+                                              data=json.dumps(query_sql),
+                                              headers=self.make_headers(),
+                                              auth=HTTPBasicAuth(self.user, self.password),
+                                              verify=True)
         try:
             resp_dict = json.loads(response.content)
         except json.decoder.JSONDecodeError:
             raise UnexpectedException("failed to parse response: %s" % response.content)
         if resp_dict and resp_dict.get('error') and "no endpoint" in resp_dict.get('error'):
             raise WarehouseTimeoutException
+        if resp_dict and resp_dict.get('error'):
+            raise UnexpectedException("failed to query: %s" % response.content)
         if self.persist_cookies:
             self.cookies = response.cookies
         return resp_dict
 
     def query(self, statement):
         url = self.format_url()
         log.logger.debug(f"http sql: {statement}")
```

### Comparing `databend-py-0.4.4/databend_py/context.py` & `databend-py-0.4.5/databend_py/context.py`

 * *Files identical despite different names*

### Comparing `databend-py-0.4.4/databend_py/datetypes.py` & `databend-py-0.4.5/databend_py/datetypes.py`

 * *Files identical despite different names*

### Comparing `databend-py-0.4.4/databend_py/errors.py` & `databend-py-0.4.5/databend_py/errors.py`

 * *Files identical despite different names*

### Comparing `databend-py-0.4.4/databend_py/result.py` & `databend-py-0.4.5/databend_py/result.py`

 * *Files identical despite different names*

### Comparing `databend-py-0.4.4/databend_py/retry.py` & `databend-py-0.4.5/databend_py/retry.py`

 * *Files identical despite different names*

### Comparing `databend-py-0.4.4/databend_py/uploader.py` & `databend-py-0.4.5/databend_py/uploader.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,50 @@
 import requests
 import io
 import csv
 import uuid
 import json
 import time
 import gzip
+from . import log
 
 
 class DataUploader:
-    def __init__(self, client, settings, default_stage_dir='@~', debug=False, compress=False):
+    def __init__(self, client, connection, settings, default_stage_dir='@~', debug=False, compress=False):
         # TODO: make it depends on Connection instead of Client
         self.client = client
+        self.connection = connection
         self.settings = settings
         self.default_stage_dir = default_stage_dir
         self._compress = compress
         self._debug = debug
 
-    def upload_to_table(self, table_name, data):
+    def upload_to_table_by_copy(self, table_name, data):
         if len(data) == 0:
             return
         stage_path = self._gen_stage_path(self.default_stage_dir)
         presigned_url, headers = self._execute_presign(stage_path)
         self._upload_to_presigned_url(presigned_url, headers, data)
         self._execute_copy(table_name, stage_path, 'CSV')
 
+    def upload_to_table_with_attachment(self, table_name, conflict_keys, data):
+        """
+        :param table_name: table name
+        :param conflict_keys: if use replace, the conflict_keys can't be None
+        :param data: list data to insert/replace
+        :return:
+        """
+        if len(data) == 0:
+            return
+        stage_path = self._gen_stage_path(self.default_stage_dir)
+        presigned_url, headers = self._execute_presign(stage_path)
+        self._upload_to_presigned_url(presigned_url, headers, data)
+        sql_statement = f"REPLACE INTO {table_name} ON ({','.join(conflict_keys)}) VALUES"
+        self._execute_with_attachment(sql_statement, stage_path, "CSV")
+
     def upload_to_stage(self, stage_dir, filename, data):
         stage_path = self._gen_stage_path(stage_dir, filename)
         presigned_url, headers = self._execute_presign(stage_path)
         self._upload_to_presigned_url(presigned_url, headers, data)
         return stage_path
 
     def _gen_stage_path(self, stage_dir, stage_filename=None):
@@ -102,7 +119,40 @@
         copy_options["SIZE_LIMIT"] = self.settings.get("size_limit",
                                                        0)  # TODO: is this correct to set size_limit = 100?
         copy_options["ON_ERROR"] = self.settings.get("on_error", "abort")
         return f"COPY INTO {table_name} FROM {stage_path} " \
                f"FILE_FORMAT = (type = {file_type} RECORD_DELIMITER = '\\r\\n' COMPRESSION = AUTO) " \
                f"PURGE = {copy_options['PURGE']} FORCE = {copy_options['FORCE']} " \
                f"SIZE_LIMIT={copy_options['SIZE_LIMIT']} ON_ERROR = {copy_options['ON_ERROR']}"
+
+    def _execute_with_attachment(self, sql_statement, stage_path, file_type):
+        start_time = time.time()
+        data = self._make_attachment(sql_statement, stage_path, file_type)
+        url = self.connection.format_url()
+
+        try:
+            resp_dict = self.connection.do_query(url, data)
+            self.client_session = resp_dict.get("session", self.connection.default_session())
+            if self._debug:
+                print('upload:_execute_attachment sql=%s %s' % (sql_statement, time.time() - start_time))
+        except Exception as e:
+            log.logger.error(
+                f"http error on {url}, SQL: {sql_statement} error msg:{str(e)}"
+            )
+            raise
+
+    def _make_attachment(self, sql_statement, stage_path, file_type):
+        copy_options = {}
+        copy_options["PURGE"] = self.settings.get("copy_purge", "False")
+        copy_options["FORCE"] = self.settings.get("force", "False")
+        copy_options["SIZE_LIMIT"] = self.settings.get("size_limit", "0")
+        copy_options["ON_ERROR"] = self.settings.get("on_error", "abort")
+
+        file_format_options = {}
+        file_format_options["type"] = file_type
+
+        data = {
+            "sql": sql_statement,
+            "stage_attachment": {"location": stage_path, "file_format_options": file_format_options,
+                                 "copy_options": copy_options}
+        }
+        return data
```

### Comparing `databend-py-0.4.4/databend_py/util/escape.py` & `databend-py-0.4.5/databend_py/util/escape.py`

 * *Files identical despite different names*

### Comparing `databend-py-0.4.4/databend_py/util/helper.py` & `databend-py-0.4.5/databend_py/util/helper.py`

 * *Files identical despite different names*

### Comparing `databend-py-0.4.4/databend_py.egg-info/PKG-INFO` & `databend-py-0.4.5/databend_py.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databend-py
-Version: 0.4.4
+Version: 0.4.5
 Summary: Python driver with native interface for Databend
 Home-page: https://github.com/databendcloud/databend-py
 Author: Databend Cloud Team
 Author-email: hantmac@outlook.com
 License: Apache License
 Keywords: databend db database cloud analytics
 Platform: UNKNOWN
@@ -82,14 +82,16 @@
 > ...     'INSERT INTO test (x) VALUES', [(1,)]
 > ... )
 > 1
 > >>> client.execute('INSERT INTO test (x) VALUES', [(200,)])
 > 1
 > ```
 
+More usages examples find [here](./examples).
+
 # Features
 
 -   Basic SQL.
 -   TLS support.
 -   Query settings.
 -   Types support:
     -   Float32/64
```

### Comparing `databend-py-0.4.4/databend_py.egg-info/SOURCES.txt` & `databend-py-0.4.5/databend_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `databend-py-0.4.4/setup.py` & `databend-py-0.4.5/setup.py`

 * *Files identical despite different names*

