# Comparing `tmp/postnormalism-0.0.4.tar.gz` & `tmp/postnormalism-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "postnormalism-0.0.4.tar", last modified: Sun Jun 11 16:01:32 2023, max compression
+gzip compressed data, was "postnormalism-0.0.5.tar", last modified: Tue Jun 13 03:10:55 2023, max compression
```

## Comparing `postnormalism-0.0.4.tar` & `postnormalism-0.0.5.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 16:01:32.918480 postnormalism-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-11 16:01:23.000000 postnormalism-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7564 2023-06-11 16:01:32.918480 postnormalism-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-06-11 16:01:23.000000 postnormalism-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 16:01:32.918480 postnormalism-0.0.4/postnormalism/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-11 16:01:23.000000 postnormalism-0.0.4/postnormalism/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 16:01:23.000000 postnormalism-0.0.4/postnormalism/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-06-11 16:01:23.000000 postnormalism-0.0.4/postnormalism/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 16:01:32.918480 postnormalism-0.0.4/postnormalism/schema/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-11 16:01:23.000000 postnormalism-0.0.4/postnormalism/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4631 2023-06-11 16:01:23.000000 postnormalism-0.0.4/postnormalism/schema/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-06-11 16:01:23.000000 postnormalism-0.0.4/postnormalism/schema/database_item.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-11 16:01:23.000000 postnormalism-0.0.4/postnormalism/schema/function.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-11 16:01:23.000000 postnormalism-0.0.4/postnormalism/schema/migrations.py
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-11 16:01:23.000000 postnormalism-0.0.4/postnormalism/schema/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-11 16:01:23.000000 postnormalism-0.0.4/postnormalism/schema/table.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-11 16:01:23.000000 postnormalism-0.0.4/postnormalism/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 16:01:32.918480 postnormalism-0.0.4/postnormalism.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7564 2023-06-11 16:01:32.000000 postnormalism-0.0.4/postnormalism.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-06-11 16:01:32.000000 postnormalism-0.0.4/postnormalism.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 16:01:32.000000 postnormalism-0.0.4/postnormalism.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-11 16:01:32.000000 postnormalism-0.0.4/postnormalism.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-06-11 16:01:23.000000 postnormalism-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 16:01:32.918480 postnormalism-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 16:01:32.918480 postnormalism-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-06-11 16:01:23.000000 postnormalism-0.0.4/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-06-11 16:01:23.000000 postnormalism-0.0.4/tests/test_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:10:55.550644 postnormalism-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-13 03:10:45.000000 postnormalism-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7622 2023-06-13 03:10:55.546644 postnormalism-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-06-13 03:10:45.000000 postnormalism-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:10:55.546644 postnormalism-0.0.5/postnormalism/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-13 03:10:45.000000 postnormalism-0.0.5/postnormalism/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 03:10:45.000000 postnormalism-0.0.5/postnormalism/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-06-13 03:10:45.000000 postnormalism-0.0.5/postnormalism/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:10:55.546644 postnormalism-0.0.5/postnormalism/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-13 03:10:45.000000 postnormalism-0.0.5/postnormalism/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-06-13 03:10:45.000000 postnormalism-0.0.5/postnormalism/schema/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-06-13 03:10:45.000000 postnormalism-0.0.5/postnormalism/schema/database_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-13 03:10:45.000000 postnormalism-0.0.5/postnormalism/schema/function.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-13 03:10:45.000000 postnormalism-0.0.5/postnormalism/schema/migrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-13 03:10:45.000000 postnormalism-0.0.5/postnormalism/schema/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-13 03:10:45.000000 postnormalism-0.0.5/postnormalism/schema/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-13 03:10:45.000000 postnormalism-0.0.5/postnormalism/schema/trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-13 03:10:45.000000 postnormalism-0.0.5/postnormalism/schema/view.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-13 03:10:45.000000 postnormalism-0.0.5/postnormalism/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:10:55.546644 postnormalism-0.0.5/postnormalism.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7622 2023-06-13 03:10:55.000000 postnormalism-0.0.5/postnormalism.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-13 03:10:55.000000 postnormalism-0.0.5/postnormalism.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 03:10:55.000000 postnormalism-0.0.5/postnormalism.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-13 03:10:55.000000 postnormalism-0.0.5/postnormalism.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-06-13 03:10:45.000000 postnormalism-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 03:10:55.550644 postnormalism-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:10:55.546644 postnormalism-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-06-13 03:10:45.000000 postnormalism-0.0.5/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-06-13 03:10:45.000000 postnormalism-0.0.5/tests/test_database.py
```

### Comparing `postnormalism-0.0.4/LICENSE` & `postnormalism-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `postnormalism-0.0.4/PKG-INFO` & `postnormalism-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: postnormalism
-Version: 0.0.4
+Version: 0.0.5
 Summary: Postnormalism is Not an Object Relational Mapper (NORM) it is a lightweight and simple-to-use Python library for managing PostgreSQL database schemas. It provides an easy way to define tables and functions, organize schema items, and create them in a database with a specified load order.
 Author-email: Zac Miller <zac@informatical.info>
 Maintainer-email: Zac Miller <zac@informatical.info>
 License: MIT License
 Project-URL: Homepage, https://github.com/jzmiller1/postnormalism
 Project-URL: Bug Tracker, https://github.com/jzmiller1/postnormalism/issues
 Project-URL: Repository, https://github.com/jzmiller1/postnormalism.git
@@ -21,19 +21,19 @@
 
 # postnormalism: PostgreSQL Schema Management  
   
 postnormalism is Not an Object Relational Mapper (NORM) it is a lightweight and simple-to-use Python library for managing PostgreSQL database schemas. It provides an easy way to define tables and functions, organize schema items, and create them in a database with a specified load order.  
   
 ## Features  
   
-- Define schemas, tables and functions using Python dataclasses  
-- Create database items (Schemas, Tables, Functions) with comments
+- Define schemas, tables, views, triggers and functions using Python dataclasses  
+- Create database items with comments
 - Group related database items and create them within a single transaction  
 - Create a Database object that allows loading database items in a specified load order and managing database extensions
-- IF NOT EXISTS mode for loading
+- exists mode for loading database items with IF NOT EXISTS and OR REPLACE 
 - SQL Migration Loader
 
   
 ## NORM vs. ORM: Features Comparison  
   
 postnormalism is a lightweight and simple-to-use Python library for managing PostgreSQL database schemas. It does not possess all the characteristics of a full-fledged ORM, focusing mainly on schema management and organization.  
   
@@ -68,15 +68,15 @@
 ## Usage  
   
 ### Defining Database Items  
   
 To define a table or a function, use the `Table` and `Function` dataclasses from the `postnormalism` module:  
   
 ```python  
-from postnormalism.schema import Schema, Table, Function  
+from postnormalism.schema import Schema, Table, Function, View, Trigger  
 ```
 
 ### Define a Schema
 ```python
 from postnormalism import schema
 
 create = """
@@ -155,15 +155,15 @@
 universe.create(cursor)  
 
 connection.commit()  
 connection.close()  
 ```  
 
 ### Using exists Mode
-Calling Database.create with exists=True inserts a IF NOT EXISTS into all of your CREATE statements allowing you to easily add new items.
+Calling Database.create with exists=True inserts IF NOT EXISTS or OR REPLACE into all of your CREATE statements allowing you to easily add new items.
 
 ```python
 universe.create(cursor, exists=True)
 ```
 
 ### Doing migrations
 Update your `DatabaseItem`s and write your SQL migration transaction.  If you create your Database instance with
```

### Comparing `postnormalism-0.0.4/README.md` & `postnormalism-0.0.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # postnormalism: PostgreSQL Schema Management  
   
 postnormalism is Not an Object Relational Mapper (NORM) it is a lightweight and simple-to-use Python library for managing PostgreSQL database schemas. It provides an easy way to define tables and functions, organize schema items, and create them in a database with a specified load order.  
   
 ## Features  
   
-- Define schemas, tables and functions using Python dataclasses  
-- Create database items (Schemas, Tables, Functions) with comments
+- Define schemas, tables, views, triggers and functions using Python dataclasses  
+- Create database items with comments
 - Group related database items and create them within a single transaction  
 - Create a Database object that allows loading database items in a specified load order and managing database extensions
-- IF NOT EXISTS mode for loading
+- exists mode for loading database items with IF NOT EXISTS and OR REPLACE 
 - SQL Migration Loader
 
   
 ## NORM vs. ORM: Features Comparison  
   
 postnormalism is a lightweight and simple-to-use Python library for managing PostgreSQL database schemas. It does not possess all the characteristics of a full-fledged ORM, focusing mainly on schema management and organization.  
   
@@ -47,15 +47,15 @@
 ## Usage  
   
 ### Defining Database Items  
   
 To define a table or a function, use the `Table` and `Function` dataclasses from the `postnormalism` module:  
   
 ```python  
-from postnormalism.schema import Schema, Table, Function  
+from postnormalism.schema import Schema, Table, Function, View, Trigger  
 ```
 
 ### Define a Schema
 ```python
 from postnormalism import schema
 
 create = """
@@ -134,15 +134,15 @@
 universe.create(cursor)  
 
 connection.commit()  
 connection.close()  
 ```  
 
 ### Using exists Mode
-Calling Database.create with exists=True inserts a IF NOT EXISTS into all of your CREATE statements allowing you to easily add new items.
+Calling Database.create with exists=True inserts IF NOT EXISTS or OR REPLACE into all of your CREATE statements allowing you to easily add new items.
 
 ```python
 universe.create(cursor, exists=True)
 ```
 
 ### Doing migrations
 Update your `DatabaseItem`s and write your SQL migration transaction.  If you create your Database instance with
```

### Comparing `postnormalism-0.0.4/postnormalism/core.py` & `postnormalism-0.0.5/postnormalism/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     Create database items in a specified load order.
     """
     for item_or_group in load_order:
         if isinstance(item_or_group, list):
             # For related tables or functions, create them within a single transaction
             transaction_sql = create_schema_items_in_transaction(item_or_group, exists=exists)
             cursor.execute(transaction_sql)
-        elif isinstance(item_or_group, (schema.Schema, schema.Table, schema.Function)):
+        elif isinstance(item_or_group, schema.DatabaseItem):
             # For tables and functions, execute the full_sql
             cursor.execute(item_or_group.full_sql(exists=exists))
         else:
             raise ValueError(f"Unsupported type in load_order: {type(item_or_group)}")
 
 
 def create_extensions(extensions: list[str], cursor):
```

### Comparing `postnormalism-0.0.4/postnormalism/schema/database.py` & `postnormalism-0.0.5/postnormalism/schema/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 from dataclasses import dataclass, field
 from ..core import create_items, create_extensions
-from . import DatabaseItem, Table, Function, PostnormalismMigrations, Schema
+from . import DatabaseItem, Table, Function, PostnormalismMigrations, Schema, View, Trigger
 
 
 @dataclass
 class Database:
     migrations_folder: str = field(default=None)
     items: dict[str, DatabaseItem] = field(default_factory=dict)
     load_order: list[DatabaseItem | list[DatabaseItem]] = field(default_factory=list)
@@ -26,22 +26,24 @@
             self.items[item.name] = item
 
     def get_items_by_type(self, item_type: str):
         type_mapping = {
             "table": Table,
             "function": Function,
             "schema": Schema,
+            "view": View,
+            "trigger": Trigger,
         }
 
         if item_type not in type_mapping:
             raise ValueError(f"Invalid item_type: {item_type}")
 
         lookup_type = type_mapping[item_type]
         return [
-            name for name, item in self.items.items()
+            item for name, item in self.items.items()
             if isinstance(item, lookup_type)
         ]
 
     def __getattr__(self, name: str):
         if name in self.items:
             return self.items[name]
         raise AttributeError(f"Schema object has no attribute '{name}'")
```

### Comparing `postnormalism-0.0.4/postnormalism/schema/database_item.py` & `postnormalism-0.0.5/postnormalism/schema/database_item.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 @dataclass(frozen=True)
 class DatabaseItem:
     """
     A base data class for schema items like tables and functions.
     """
     create: str
     comment: str = field(default=None)
+    _item_type: str = field(default=None)
     _name_pattern: str = field(default=None)
     _name: str = field(init=False, default=None)
     _schema_pattern: str = field(default=None)
     _schema: str = field(init=False, default=None)
 
     def __post_init__(self):
         create = self.create.upper()
@@ -44,7 +45,11 @@
     @property
     def name(self) -> str:
         return self._name
 
     @property
     def schema(self) -> str:
         return self._schema
+
+    @property
+    def itype(self) -> str:
+        return self._item_type
```

### Comparing `postnormalism-0.0.4/postnormalism/schema/schema.py` & `postnormalism-0.0.5/postnormalism/schema/schema.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 
 @dataclass(frozen=True)
 class Schema(DatabaseItem):
     """
     A data class for schema.
     """
+    _item_type: str = 'schema'
     _name_pattern: str = field(default=r'CREATE\s+SCHEMA\s+(?:IF\s+NOT\s+EXISTS\s+)?(\w+)')
     alter: str = field(default=None)
 
     def full_sql(self, exists=False) -> str:
         sql_parts = super().full_sql().split("\n\n")
 
         if exists:
```

### Comparing `postnormalism-0.0.4/postnormalism/schema/table.py` & `postnormalism-0.0.5/postnormalism/schema/table.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 
 @dataclass(frozen=True)
 class Table(DatabaseItem):
     """
     A data class for tables.
     """
+    _item_type: str = 'table'
     _name_pattern: str = field(default=r'CREATE\s+(?:OR\s+REPLACE\s+)?(?:TEMP\s+)?(?:TABLE)\s+(?:IF\s+NOT\s+EXISTS\s+)?(?:\w+\.)?(\w+)')
     _schema_pattern: str = field(default=r'CREATE\s+TABLE\s+(?:IF\s+NOT\s+EXISTS\s+)?(\w+)\.\w+')
     alter: str = field(default=None)
 
     def full_sql(self, exists=False) -> str:
         sql_parts = super().full_sql().split("\n\n")
```

### Comparing `postnormalism-0.0.4/postnormalism/utils.py` & `postnormalism-0.0.5/postnormalism/utils.py`

 * *Files identical despite different names*

### Comparing `postnormalism-0.0.4/postnormalism.egg-info/PKG-INFO` & `postnormalism-0.0.5/postnormalism.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: postnormalism
-Version: 0.0.4
+Version: 0.0.5
 Summary: Postnormalism is Not an Object Relational Mapper (NORM) it is a lightweight and simple-to-use Python library for managing PostgreSQL database schemas. It provides an easy way to define tables and functions, organize schema items, and create them in a database with a specified load order.
 Author-email: Zac Miller <zac@informatical.info>
 Maintainer-email: Zac Miller <zac@informatical.info>
 License: MIT License
 Project-URL: Homepage, https://github.com/jzmiller1/postnormalism
 Project-URL: Bug Tracker, https://github.com/jzmiller1/postnormalism/issues
 Project-URL: Repository, https://github.com/jzmiller1/postnormalism.git
@@ -21,19 +21,19 @@
 
 # postnormalism: PostgreSQL Schema Management  
   
 postnormalism is Not an Object Relational Mapper (NORM) it is a lightweight and simple-to-use Python library for managing PostgreSQL database schemas. It provides an easy way to define tables and functions, organize schema items, and create them in a database with a specified load order.  
   
 ## Features  
   
-- Define schemas, tables and functions using Python dataclasses  
-- Create database items (Schemas, Tables, Functions) with comments
+- Define schemas, tables, views, triggers and functions using Python dataclasses  
+- Create database items with comments
 - Group related database items and create them within a single transaction  
 - Create a Database object that allows loading database items in a specified load order and managing database extensions
-- IF NOT EXISTS mode for loading
+- exists mode for loading database items with IF NOT EXISTS and OR REPLACE 
 - SQL Migration Loader
 
   
 ## NORM vs. ORM: Features Comparison  
   
 postnormalism is a lightweight and simple-to-use Python library for managing PostgreSQL database schemas. It does not possess all the characteristics of a full-fledged ORM, focusing mainly on schema management and organization.  
   
@@ -68,15 +68,15 @@
 ## Usage  
   
 ### Defining Database Items  
   
 To define a table or a function, use the `Table` and `Function` dataclasses from the `postnormalism` module:  
   
 ```python  
-from postnormalism.schema import Schema, Table, Function  
+from postnormalism.schema import Schema, Table, Function, View, Trigger  
 ```
 
 ### Define a Schema
 ```python
 from postnormalism import schema
 
 create = """
@@ -155,15 +155,15 @@
 universe.create(cursor)  
 
 connection.commit()  
 connection.close()  
 ```  
 
 ### Using exists Mode
-Calling Database.create with exists=True inserts a IF NOT EXISTS into all of your CREATE statements allowing you to easily add new items.
+Calling Database.create with exists=True inserts IF NOT EXISTS or OR REPLACE into all of your CREATE statements allowing you to easily add new items.
 
 ```python
 universe.create(cursor, exists=True)
 ```
 
 ### Doing migrations
 Update your `DatabaseItem`s and write your SQL migration transaction.  If you create your Database instance with
```

### Comparing `postnormalism-0.0.4/postnormalism.egg-info/SOURCES.txt` & `postnormalism-0.0.5/postnormalism.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -12,9 +12,11 @@
 postnormalism/schema/__init__.py
 postnormalism/schema/database.py
 postnormalism/schema/database_item.py
 postnormalism/schema/function.py
 postnormalism/schema/migrations.py
 postnormalism/schema/schema.py
 postnormalism/schema/table.py
+postnormalism/schema/trigger.py
+postnormalism/schema/view.py
 tests/test_core.py
-tests/test_schema.py
+tests/test_database.py
```

### Comparing `postnormalism-0.0.4/pyproject.toml` & `postnormalism-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `postnormalism-0.0.4/tests/test_core.py` & `postnormalism-0.0.5/tests/test_core.py`

 * *Files identical despite different names*

