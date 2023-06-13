# Comparing `tmp/sqlalchemy_mock-1.0.2.tar.gz` & `tmp/sqlalchemy_mock-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy_mock-1.0.2.tar", max compression
+gzip compressed data, was "sqlalchemy_mock-1.0.3.tar", max compression
```

## Comparing `sqlalchemy_mock-1.0.2.tar` & `sqlalchemy_mock-1.0.3.tar`

### file list

```diff
@@ -1,7 +1,9 @@
--rw-r--r--   0        0        0     1647 2023-05-13 14:38:38.650122 sqlalchemy_mock-1.0.2/README.md
--rw-r--r--   0        0        0      448 2023-05-17 19:53:35.084165 sqlalchemy_mock-1.0.2/pyproject.toml
--rw-r--r--   0        0        0       43 2023-05-13 14:38:38.650764 sqlalchemy_mock-1.0.2/sqlalchemy_mock/__init__.py
--rw-r--r--   0        0        0     2077 2023-05-13 14:38:38.650922 sqlalchemy_mock-1.0.2/sqlalchemy_mock/query.py
--rw-r--r--   0        0        0     1314 2023-05-13 14:38:38.651032 sqlalchemy_mock-1.0.2/sqlalchemy_mock/session.py
--rw-r--r--   0        0        0     2182 2023-05-17 19:53:10.850350 sqlalchemy_mock-1.0.2/sqlalchemy_mock/utils.py
--rw-r--r--   0        0        0     2345 1970-01-01 00:00:00.000000 sqlalchemy_mock-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1647 2023-05-13 14:38:38.650122 sqlalchemy_mock-1.0.3/README.md
+-rw-r--r--   0        0        0      448 2023-06-13 08:15:28.453757 sqlalchemy_mock-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0       98 2023-06-13 08:13:20.212930 sqlalchemy_mock-1.0.3/sqlalchemy_mock/__init__.py
+-rw-r--r--   0        0        0      183 2023-06-13 08:13:20.213067 sqlalchemy_mock-1.0.3/sqlalchemy_mock/async_session.py
+-rw-r--r--   0        0        0     4341 2023-06-13 08:13:20.213214 sqlalchemy_mock-1.0.3/sqlalchemy_mock/execute.py
+-rw-r--r--   0        0        0     1427 2023-06-13 08:13:20.213390 sqlalchemy_mock-1.0.3/sqlalchemy_mock/query.py
+-rw-r--r--   0        0        0     3258 2023-06-13 08:13:20.213584 sqlalchemy_mock-1.0.3/sqlalchemy_mock/session.py
+-rw-r--r--   0        0        0     4407 2023-06-13 08:13:20.213788 sqlalchemy_mock-1.0.3/sqlalchemy_mock/utils.py
+-rw-r--r--   0        0        0     2345 1970-01-01 00:00:00.000000 sqlalchemy_mock-1.0.3/PKG-INFO
```

### Comparing `sqlalchemy_mock-1.0.2/README.md` & `sqlalchemy_mock-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `sqlalchemy_mock-1.0.2/sqlalchemy_mock/session.py` & `sqlalchemy_mock-1.0.3/sqlalchemy_mock/query.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,40 +1,50 @@
-import uuid
-from .query import Query
-from .utils import set_choice_fields_to_record, set_primary_key_to_record, mock_sessions_methods
+from .utils import filter_records, set_choice_fields_to_record, sort_records
 
 
-class Session:
-    def __init__(self, primary_key: str = "uuid", primary_key_generate: object = lambda: str(uuid.uuid4())):
-        self.__storage = {}
-        self.primary_key = primary_key
-        self.primary_key_generate = primary_key_generate
+class Query:
+    def __init__(self, session: object, instance: object, records: list):
+        self.session = session
+        self.instance = instance
+        self.records = records
+        self.limit_value = self.offset_value = None
 
-    def add(self, record: object):
-        set_primary_key_to_record(record, self.primary_key, self.primary_key_generate)
-        set_choice_fields_to_record(record)
+    def __iter__(self):
+        for record in self.records: yield record
 
-        record_table = str(type(record))
-        if not record_table in self.__storage:
-            self.__storage[record_table] = [record]
-        else:
-            self.__storage[record_table].append(record)
+    def filter(self, *filters: tuple):
+        self.records = filter_records(filters, self.records)
+        return self
 
-    def add_all(self, records: list):
-        for record in records: self.add(record)
+    def count(self): return len(self.records)
 
-    def query(self, instance: object):
-        records = self.__storage.get(str(instance), [])
-        return Query(self, instance, records)
+    def all(self):
+        offset = self.limit_value * self.offset_value if self.limit_value and self.offset_value else None
+        limit = self.limit_value
 
-    def delete(self, instance: object, records: list):
-        for record in records:
-            self.__storage[str(instance)].remove(record)
+        return self.records[offset:limit]
 
-    def commit(self): ...
+    def limit(self, size: int):
+        self.limit_value = size
+        return self
 
-    def flush(self): ...
+    def offset(self, value: int):
+        self.offset_value = value
+        return self
 
-    def refresh(self, record: object): return record
+    def order_by(self, field: object):
+        self.records = sort_records(field, self.records)
+        return self
 
-    def mock_session(self):
-        return mock_sessions_methods(self)
+    def first(self):
+        if self.records:
+            return self.records[0]
+        return
+
+    def update(self, data: dict):
+        for record in self.records:
+            for key in data.keys():
+                setattr(record, key, data[key])
+            set_choice_fields_to_record(record)
+
+    def delete(self):
+        self.session.delete(self.instance, self.records)
```

### Comparing `sqlalchemy_mock-1.0.2/PKG-INFO` & `sqlalchemy_mock-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-mock
-Version: 1.0.2
+Version: 1.0.3
 Summary: The package for working with SQLAlchemy in unit tests
 Author: ivanostapiuk
 Author-email: ost.ivan13@gmail.com
 Requires-Python: >=3.0,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
```

