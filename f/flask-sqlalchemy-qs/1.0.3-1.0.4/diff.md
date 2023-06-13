# Comparing `tmp/flask_sqlalchemy_qs-1.0.3.tar.gz` & `tmp/flask_sqlalchemy_qs-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_sqlalchemy_qs-1.0.3.tar", last modified: Mon Jun 12 19:00:57 2023, max compression
+gzip compressed data, was "flask_sqlalchemy_qs-1.0.4.tar", last modified: Tue Jun 13 21:28:27 2023, max compression
```

## Comparing `flask_sqlalchemy_qs-1.0.3.tar` & `flask_sqlalchemy_qs-1.0.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 marco      (501) staff       (20)        0 2023-06-12 19:00:57.699725 flask_sqlalchemy_qs-1.0.3/
--rw-r--r--   0 marco      (501) staff       (20)     1083 2023-06-08 22:48:59.000000 flask_sqlalchemy_qs-1.0.3/LICENSE
--rw-r--r--   0 marco      (501) staff       (20)     5953 2023-06-12 19:00:57.699610 flask_sqlalchemy_qs-1.0.3/PKG-INFO
--rw-r--r--   0 marco      (501) staff       (20)     5384 2023-06-12 17:46:16.000000 flask_sqlalchemy_qs-1.0.3/README.md
-drwxr-xr-x   0 marco      (501) staff       (20)        0 2023-06-12 19:00:57.697407 flask_sqlalchemy_qs-1.0.3/flask_sqlalchemy_qs/
--rw-r--r--   0 marco      (501) staff       (20)      118 2023-06-06 17:53:38.000000 flask_sqlalchemy_qs-1.0.3/flask_sqlalchemy_qs/__init__.py
-drwxr-xr-x   0 marco      (501) staff       (20)        0 2023-06-12 19:00:57.698321 flask_sqlalchemy_qs-1.0.3/flask_sqlalchemy_qs/qs_parser/
--rw-r--r--   0 marco      (501) staff       (20)     3683 2023-06-07 23:35:08.000000 flask_sqlalchemy_qs-1.0.3/flask_sqlalchemy_qs/qs_parser/main.py
-drwxr-xr-x   0 marco      (501) staff       (20)        0 2023-06-12 19:00:57.698544 flask_sqlalchemy_qs-1.0.3/flask_sqlalchemy_qs/query/
--rw-r--r--   0 marco      (501) staff       (20)      770 2023-06-12 17:46:23.000000 flask_sqlalchemy_qs-1.0.3/flask_sqlalchemy_qs/query/constants.py
--rw-r--r--   0 marco      (501) staff       (20)     8695 2023-06-12 17:46:54.000000 flask_sqlalchemy_qs-1.0.3/flask_sqlalchemy_qs/query/model.py
-drwxr-xr-x   0 marco      (501) staff       (20)        0 2023-06-12 19:00:57.698216 flask_sqlalchemy_qs-1.0.3/flask_sqlalchemy_qs.egg-info/
--rw-r--r--   0 marco      (501) staff       (20)     5953 2023-06-12 19:00:57.000000 flask_sqlalchemy_qs-1.0.3/flask_sqlalchemy_qs.egg-info/PKG-INFO
--rw-r--r--   0 marco      (501) staff       (20)      454 2023-06-12 19:00:57.000000 flask_sqlalchemy_qs-1.0.3/flask_sqlalchemy_qs.egg-info/SOURCES.txt
--rw-r--r--   0 marco      (501) staff       (20)        1 2023-06-12 19:00:57.000000 flask_sqlalchemy_qs-1.0.3/flask_sqlalchemy_qs.egg-info/dependency_links.txt
--rw-r--r--   0 marco      (501) staff       (20)       79 2023-06-12 19:00:57.000000 flask_sqlalchemy_qs-1.0.3/flask_sqlalchemy_qs.egg-info/requires.txt
--rw-r--r--   0 marco      (501) staff       (20)       20 2023-06-12 19:00:57.000000 flask_sqlalchemy_qs-1.0.3/flask_sqlalchemy_qs.egg-info/top_level.txt
--rw-r--r--   0 marco      (501) staff       (20)       38 2023-06-12 19:00:57.699761 flask_sqlalchemy_qs-1.0.3/setup.cfg
--rw-r--r--   0 marco      (501) staff       (20)      985 2023-06-12 18:59:42.000000 flask_sqlalchemy_qs-1.0.3/setup.py
-drwxr-xr-x   0 marco      (501) staff       (20)        0 2023-06-12 19:00:57.699272 flask_sqlalchemy_qs-1.0.3/tests/
--rw-r--r--   0 marco      (501) staff       (20)      722 2023-06-07 23:48:33.000000 flask_sqlalchemy_qs-1.0.3/tests/test_integration.py
--rw-r--r--   0 marco      (501) staff       (20)     6043 2023-06-06 04:36:10.000000 flask_sqlalchemy_qs-1.0.3/tests/test_qs_parser.py
--rw-r--r--   0 marco      (501) staff       (20)     6772 2023-06-06 14:10:19.000000 flask_sqlalchemy_qs-1.0.3/tests/test_query.py
+drwxr-xr-x   0 marco      (501) staff       (20)        0 2023-06-13 21:28:27.485611 flask_sqlalchemy_qs-1.0.4/
+-rw-r--r--   0 marco      (501) staff       (20)     1083 2023-06-08 22:48:59.000000 flask_sqlalchemy_qs-1.0.4/LICENSE
+-rw-r--r--   0 marco      (501) staff       (20)     6058 2023-06-13 21:28:27.485491 flask_sqlalchemy_qs-1.0.4/PKG-INFO
+-rw-r--r--   0 marco      (501) staff       (20)     5490 2023-06-12 23:43:15.000000 flask_sqlalchemy_qs-1.0.4/README.md
+drwxr-xr-x   0 marco      (501) staff       (20)        0 2023-06-13 21:28:27.483978 flask_sqlalchemy_qs-1.0.4/flask_sqlalchemy_qs/
+-rw-r--r--   0 marco      (501) staff       (20)      118 2023-06-06 17:53:38.000000 flask_sqlalchemy_qs-1.0.4/flask_sqlalchemy_qs/__init__.py
+drwxr-xr-x   0 marco      (501) staff       (20)        0 2023-06-13 21:28:27.484668 flask_sqlalchemy_qs-1.0.4/flask_sqlalchemy_qs/qs_parser/
+-rw-r--r--   0 marco      (501) staff       (20)     3752 2023-06-12 23:28:28.000000 flask_sqlalchemy_qs-1.0.4/flask_sqlalchemy_qs/qs_parser/main.py
+drwxr-xr-x   0 marco      (501) staff       (20)        0 2023-06-13 21:28:27.484926 flask_sqlalchemy_qs-1.0.4/flask_sqlalchemy_qs/query/
+-rw-r--r--   0 marco      (501) staff       (20)      812 2023-06-12 23:12:02.000000 flask_sqlalchemy_qs-1.0.4/flask_sqlalchemy_qs/query/constants.py
+-rw-r--r--   0 marco      (501) staff       (20)     7980 2023-06-12 23:29:30.000000 flask_sqlalchemy_qs-1.0.4/flask_sqlalchemy_qs/query/model.py
+drwxr-xr-x   0 marco      (501) staff       (20)        0 2023-06-13 21:28:27.484543 flask_sqlalchemy_qs-1.0.4/flask_sqlalchemy_qs.egg-info/
+-rw-r--r--   0 marco      (501) staff       (20)     6058 2023-06-13 21:28:27.000000 flask_sqlalchemy_qs-1.0.4/flask_sqlalchemy_qs.egg-info/PKG-INFO
+-rw-r--r--   0 marco      (501) staff       (20)      454 2023-06-13 21:28:27.000000 flask_sqlalchemy_qs-1.0.4/flask_sqlalchemy_qs.egg-info/SOURCES.txt
+-rw-r--r--   0 marco      (501) staff       (20)        1 2023-06-13 21:28:27.000000 flask_sqlalchemy_qs-1.0.4/flask_sqlalchemy_qs.egg-info/dependency_links.txt
+-rw-r--r--   0 marco      (501) staff       (20)       79 2023-06-13 21:28:27.000000 flask_sqlalchemy_qs-1.0.4/flask_sqlalchemy_qs.egg-info/requires.txt
+-rw-r--r--   0 marco      (501) staff       (20)       20 2023-06-13 21:28:27.000000 flask_sqlalchemy_qs-1.0.4/flask_sqlalchemy_qs.egg-info/top_level.txt
+-rw-r--r--   0 marco      (501) staff       (20)       38 2023-06-13 21:28:27.485646 flask_sqlalchemy_qs-1.0.4/setup.cfg
+-rw-r--r--   0 marco      (501) staff       (20)      984 2023-06-13 21:27:29.000000 flask_sqlalchemy_qs-1.0.4/setup.py
+drwxr-xr-x   0 marco      (501) staff       (20)        0 2023-06-13 21:28:27.485311 flask_sqlalchemy_qs-1.0.4/tests/
+-rw-r--r--   0 marco      (501) staff       (20)      722 2023-06-07 23:48:33.000000 flask_sqlalchemy_qs-1.0.4/tests/test_integration.py
+-rw-r--r--   0 marco      (501) staff       (20)     6412 2023-06-12 23:40:11.000000 flask_sqlalchemy_qs-1.0.4/tests/test_qs_parser.py
+-rw-r--r--   0 marco      (501) staff       (20)     6772 2023-06-06 14:10:19.000000 flask_sqlalchemy_qs-1.0.4/tests/test_query.py
```

### Comparing `flask_sqlalchemy_qs-1.0.3/LICENSE` & `flask_sqlalchemy_qs-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `flask_sqlalchemy_qs-1.0.3/PKG-INFO` & `flask_sqlalchemy_qs-1.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: flask_sqlalchemy_qs
-Version: 1.0.3
-Summary: Generate and manipulatew SQLAlchemy filters and sorts from query strings in the URL
+Version: 1.0.4
+Summary: Generate and manipulate SQLAlchemy filters and sorts from query strings in the URL
 Home-page: https://github.com/marcogil93/flask-sqlalchemy-qs
 Author: Marco Gil
 Author-email: marcogil93@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Operating System :: OS Independent
@@ -48,14 +48,16 @@
 
 The following operators are available:
 
 | Operator    | Description                        |
 | ----------- | ---------------------------------- |
 | eq          | Equal                              |
 | ne          | Not equal                          |
+| is          | Is                                 |
+| is_not      | Is not                             |
 | lt          | Less than                          |
 | lte         | Less than or equal to              |
 | gt          | Greater than                       |
 | gte         | Greater than or equal to           |
 | in          | Included in an array               |
 | nin         | Not included in an array           |
 | contains    | Contains                           |
@@ -179,15 +181,15 @@
 
   results = query.all()
 
   ...
 ```
 
 ## Version
-1.0.3
+1.0.4
 
 ## Requirements 
 SQLALCHEMYSQLAlchemy~=2.0
 
 flask~=2.2
 
 flask-sqlalchemy~=3.0
```

### Comparing `flask_sqlalchemy_qs-1.0.3/README.md` & `flask_sqlalchemy_qs-1.0.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -31,14 +31,16 @@
 
 The following operators are available:
 
 | Operator    | Description                        |
 | ----------- | ---------------------------------- |
 | eq          | Equal                              |
 | ne          | Not equal                          |
+| is          | Is                                 |
+| is_not      | Is not                             |
 | lt          | Less than                          |
 | lte         | Less than or equal to              |
 | gt          | Greater than                       |
 | gte         | Greater than or equal to           |
 | in          | Included in an array               |
 | nin         | Not included in an array           |
 | contains    | Contains                           |
@@ -162,15 +164,15 @@
 
   results = query.all()
 
   ...
 ```
 
 ## Version
-1.0.3
+1.0.4
 
 ## Requirements 
 SQLALCHEMYSQLAlchemy~=2.0
 
 flask~=2.2
 
 flask-sqlalchemy~=3.0
```

### Comparing `flask_sqlalchemy_qs-1.0.3/flask_sqlalchemy_qs/qs_parser/main.py` & `flask_sqlalchemy_qs-1.0.4/flask_sqlalchemy_qs/qs_parser/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 
         #is final condition (eq, contains, ...)   index in
         if i == len(parts) -1:
           if value == 'true':
             target_dict[part] = True
           elif value == 'false':
             target_dict[part] = False
+          elif value == 'null':
+            target_dict[part] = None
           else:
             if part.isdigit(): #Case in, nin
               target_dict[int(part)] = value
             else:
               target_dict[part] = value
         
         elif part in ["in", "nin"]:
```

### Comparing `flask_sqlalchemy_qs-1.0.3/flask_sqlalchemy_qs/query/constants.py` & `flask_sqlalchemy_qs-1.0.4/flask_sqlalchemy_qs/query/constants.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 
 # Types
 FilterType = Dict[str, Union[bool, str, Dict]]
 SortType = Dict[str, Union[str, Dict]]
 BooleanExpression = Union[or_, and_, not_]
 
 CONDITIONS = {
+    "is": "is_",
+    "is_not": "is_not",
     "eq": "__eq__",
     "ne": "__ne__",
     "lt": "__lt__",
     "lte": "__le__",
     "gt": "__gt__",
     "gte": "__ge__",
     "in": "in_",
@@ -26,8 +28,8 @@
     "ilike": "ilike",
     "not_like": "not_like",
     "not_ilike": "not_ilike",
     "startswith": "startswith",
     "istartswith": "istartswith",
     "endswith": "endswith",
     "iendswith": "iendswith"
-}
+}
```

### Comparing `flask_sqlalchemy_qs-1.0.3/flask_sqlalchemy_qs/query/model.py` & `flask_sqlalchemy_qs-1.0.4/flask_sqlalchemy_qs/query/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,39 +46,26 @@
                         idx = column_names.index(key)
                         column = mapper.columns[idx]
 
                         # Set all the property filters
                         for condition, filter_value in value.items():
                             if condition in CONDITIONS:
                                 column_condition = CONDITIONS[condition]
+                                condition_func = getattr(
+                                    column, column_condition
+                                )
 
-                                if (
-                                    condition in {"eq", "ne"}
-                                    and filter_value == "null"
-                                ):
-                                    condition_func = (
-                                        column.is_
-                                        if condition == "eq"
-                                        else column.is_not
-                                    )
-                                    conditions.append(condition_func(None))
-                                elif condition in {"ncontains", "nicontains"}:
-                                    #No native ncontains, nor nicontains attr.
-                                    #Use of contains, and icontains attrs. to 
-                                    #negate them 
-                                    condition_func = getattr(
-                                        column, column_condition
-                                    )
+                                if condition in {"ncontains", "nicontains"}:
+                                    # No native ncontains, nor nicontains attr.
+                                    # Use of a not and the contains, and 
+                                    # icontains attrs.
                                     conditions.append(
                                         not_(condition_func(filter_value))
                                     )
                                 else:
-                                    condition_func = getattr(
-                                        column, column_condition
-                                    )
                                     conditions.append(
                                         condition_func(filter_value)
                                     )
                             else:
                                 raise Exception(
                                     f"'{condition}' is not a supported condition."
                                 )
```

### Comparing `flask_sqlalchemy_qs-1.0.3/flask_sqlalchemy_qs.egg-info/PKG-INFO` & `flask_sqlalchemy_qs-1.0.4/flask_sqlalchemy_qs.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: flask-sqlalchemy-qs
-Version: 1.0.3
-Summary: Generate and manipulatew SQLAlchemy filters and sorts from query strings in the URL
+Version: 1.0.4
+Summary: Generate and manipulate SQLAlchemy filters and sorts from query strings in the URL
 Home-page: https://github.com/marcogil93/flask-sqlalchemy-qs
 Author: Marco Gil
 Author-email: marcogil93@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Operating System :: OS Independent
@@ -48,14 +48,16 @@
 
 The following operators are available:
 
 | Operator    | Description                        |
 | ----------- | ---------------------------------- |
 | eq          | Equal                              |
 | ne          | Not equal                          |
+| is          | Is                                 |
+| is_not      | Is not                             |
 | lt          | Less than                          |
 | lte         | Less than or equal to              |
 | gt          | Greater than                       |
 | gte         | Greater than or equal to           |
 | in          | Included in an array               |
 | nin         | Not included in an array           |
 | contains    | Contains                           |
@@ -179,15 +181,15 @@
 
   results = query.all()
 
   ...
 ```
 
 ## Version
-1.0.3
+1.0.4
 
 ## Requirements 
 SQLALCHEMYSQLAlchemy~=2.0
 
 flask~=2.2
 
 flask-sqlalchemy~=3.0
```

### Comparing `flask_sqlalchemy_qs-1.0.3/setup.py` & `flask_sqlalchemy_qs-1.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="flask_sqlalchemy_qs",
-    version="1.0.3",
-    description="Generate and manipulatew SQLAlchemy filters and sorts from query strings in the URL",
+    version="1.0.4",
+    description="Generate and manipulate SQLAlchemy filters and sorts from query strings in the URL",
     packages=["flask_sqlalchemy_qs", "flask_sqlalchemy_qs.qs_parser", "flask_sqlalchemy_qs.query"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/marcogil93/flask-sqlalchemy-qs",
     author="Marco Gil",
     author_email="marcogil93@gmail.com",
     license="MIT",
```

### Comparing `flask_sqlalchemy_qs-1.0.3/tests/test_integration.py` & `flask_sqlalchemy_qs-1.0.4/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `flask_sqlalchemy_qs-1.0.3/tests/test_qs_parser.py` & `flask_sqlalchemy_qs-1.0.4/tests/test_qs_parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -88,14 +88,30 @@
       "foo": {"eq":False}
     },
     "offset": 0,
     "limit": 10,
     "sorts": []
   }
 
+#Test null 
+def test_qs_parser_null_value_filtering(client):
+  response = client.get("/endpoint?filters[baz][is]=null&filters[foo][is_not]=null")
+  assert response.status_code == 200
+
+  data = response.json
+  assert data["ctx"] == {
+    "filters": {
+      "baz": {"is": None},
+      "foo": {"is_not": None}
+    },
+    "offset": 0,
+    "limit": 10,
+    "sorts": []
+  }
+
 #Boolean expressions filtering
 def test_qs_parser_boolean_expressions_filter(client):
   response = client.get("/endpoint?" +
     "filters[or][0][baz][eq]=value_baz&" +
     "filters[or][1][foo][bar][eq]=value_bar")
   assert response.status_code == 200
```

### Comparing `flask_sqlalchemy_qs-1.0.3/tests/test_query.py` & `flask_sqlalchemy_qs-1.0.4/tests/test_query.py`

 * *Files identical despite different names*

