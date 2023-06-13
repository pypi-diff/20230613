# Comparing `tmp/dtfield-0.1.8.tar.gz` & `tmp/dtfield-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dtfield-0.1.8.tar", max compression
+gzip compressed data, was "dtfield-0.1.9.tar", max compression
```

## Comparing `dtfield-0.1.8.tar` & `dtfield-0.1.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      116 2023-06-12 03:54:19.665800 dtfield-0.1.8/dtfield/__init__.py
--rw-r--r--   0        0        0     2014 2023-06-12 14:04:46.335668 dtfield-0.1.8/dtfield/_imports.py
--rw-r--r--   0        0        0     1389 2023-06-12 03:54:59.665860 dtfield-0.1.8/dtfield/base_enum.py
--rw-r--r--   0        0        0    21781 2023-06-12 16:27:27.493539 dtfield-0.1.8/dtfield/engine.py
--rw-r--r--   0        0        0     2526 2023-06-12 01:02:37.187182 dtfield-0.1.8/dtfield/functions.py
--rw-r--r--   0        0        0      159 2023-06-11 22:28:46.644614 dtfield-0.1.8/dtfield/parse/__init__.py
--rw-r--r--   0        0        0      340 2023-06-11 22:28:46.790548 dtfield-0.1.8/dtfield/parse/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      443 2023-06-11 22:28:46.791054 dtfield-0.1.8/dtfield/parse/__pycache__/_types.cpython-39.pyc
--rw-r--r--   0        0        0      777 2023-06-11 19:47:04.574010 dtfield-0.1.8/dtfield/parse/__pycache__/dates.cpython-39.pyc
--rw-r--r--   0        0        0     1728 2023-06-11 22:26:00.687944 dtfield-0.1.8/dtfield/parse/__pycache__/json_encoder.cpython-39.pyc
--rw-r--r--   0        0        0      526 2023-06-11 19:47:01.431654 dtfield-0.1.8/dtfield/parse/__pycache__/null.cpython-39.pyc
--rw-r--r--   0        0        0     1280 2023-06-11 19:47:04.492588 dtfield-0.1.8/dtfield/parse/__pycache__/number.cpython-39.pyc
--rw-r--r--   0        0        0      802 2023-06-11 19:47:04.487489 dtfield-0.1.8/dtfield/parse/__pycache__/string.cpython-39.pyc
--rw-r--r--   0        0        0    11644 2023-06-12 05:40:54.569591 dtfield-0.1.8/dtfield/parse/__pycache__/type_hint.cpython-39.pyc
--rw-r--r--   0        0        0      321 2023-06-11 22:28:46.640186 dtfield-0.1.8/dtfield/parse/_types.py
--rw-r--r--   0        0        0      694 2023-06-11 02:28:20.159802 dtfield-0.1.8/dtfield/parse/dates.py
--rw-r--r--   0        0        0     1543 2023-06-11 22:26:00.531404 dtfield-0.1.8/dtfield/parse/json_encoder.py
--rw-r--r--   0        0        0      346 2023-06-11 02:36:40.384030 dtfield-0.1.8/dtfield/parse/null.py
--rw-r--r--   0        0        0     1260 2023-06-11 02:29:46.320272 dtfield-0.1.8/dtfield/parse/number.py
--rw-r--r--   0        0        0      627 2023-06-11 02:34:21.462547 dtfield-0.1.8/dtfield/parse/string.py
--rw-r--r--   0        0        0    10839 2023-06-12 04:07:43.884069 dtfield-0.1.8/dtfield/parse/type_hint.py
--rw-r--r--   0        0        0      387 2023-06-12 17:15:19.554397 dtfield-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      715 2023-06-12 17:15:24.642666 dtfield-0.1.8/setup.py
--rw-r--r--   0        0        0      503 2023-06-12 17:15:24.642883 dtfield-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      116 2023-06-12 03:54:19.665800 dtfield-0.1.9/dtfield/__init__.py
+-rw-r--r--   0        0        0     2014 2023-06-12 14:04:46.335668 dtfield-0.1.9/dtfield/_imports.py
+-rw-r--r--   0        0        0     1389 2023-06-12 03:54:59.665860 dtfield-0.1.9/dtfield/base_enum.py
+-rw-r--r--   0        0        0    21791 2023-06-13 02:35:07.521474 dtfield-0.1.9/dtfield/engine.py
+-rw-r--r--   0        0        0     2526 2023-06-12 01:02:37.187182 dtfield-0.1.9/dtfield/functions.py
+-rw-r--r--   0        0        0      159 2023-06-11 22:28:46.644614 dtfield-0.1.9/dtfield/parse/__init__.py
+-rw-r--r--   0        0        0      340 2023-06-11 22:28:46.790548 dtfield-0.1.9/dtfield/parse/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      443 2023-06-11 22:28:46.791054 dtfield-0.1.9/dtfield/parse/__pycache__/_types.cpython-39.pyc
+-rw-r--r--   0        0        0      777 2023-06-11 19:47:04.574010 dtfield-0.1.9/dtfield/parse/__pycache__/dates.cpython-39.pyc
+-rw-r--r--   0        0        0     1728 2023-06-11 22:26:00.687944 dtfield-0.1.9/dtfield/parse/__pycache__/json_encoder.cpython-39.pyc
+-rw-r--r--   0        0        0      526 2023-06-11 19:47:01.431654 dtfield-0.1.9/dtfield/parse/__pycache__/null.cpython-39.pyc
+-rw-r--r--   0        0        0     1280 2023-06-11 19:47:04.492588 dtfield-0.1.9/dtfield/parse/__pycache__/number.cpython-39.pyc
+-rw-r--r--   0        0        0      802 2023-06-11 19:47:04.487489 dtfield-0.1.9/dtfield/parse/__pycache__/string.cpython-39.pyc
+-rw-r--r--   0        0        0    11644 2023-06-12 05:40:54.569591 dtfield-0.1.9/dtfield/parse/__pycache__/type_hint.cpython-39.pyc
+-rw-r--r--   0        0        0      321 2023-06-11 22:28:46.640186 dtfield-0.1.9/dtfield/parse/_types.py
+-rw-r--r--   0        0        0      694 2023-06-11 02:28:20.159802 dtfield-0.1.9/dtfield/parse/dates.py
+-rw-r--r--   0        0        0     1543 2023-06-11 22:26:00.531404 dtfield-0.1.9/dtfield/parse/json_encoder.py
+-rw-r--r--   0        0        0      346 2023-06-11 02:36:40.384030 dtfield-0.1.9/dtfield/parse/null.py
+-rw-r--r--   0        0        0     1260 2023-06-11 02:29:46.320272 dtfield-0.1.9/dtfield/parse/number.py
+-rw-r--r--   0        0        0      627 2023-06-11 02:34:21.462547 dtfield-0.1.9/dtfield/parse/string.py
+-rw-r--r--   0        0        0    10839 2023-06-12 04:07:43.884069 dtfield-0.1.9/dtfield/parse/type_hint.py
+-rw-r--r--   0        0        0      387 2023-06-13 02:35:07.524633 dtfield-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      715 2023-06-13 02:35:11.747697 dtfield-0.1.9/setup.py
+-rw-r--r--   0        0        0      503 2023-06-13 02:35:11.747905 dtfield-0.1.9/PKG-INFO
```

### Comparing `dtfield-0.1.8/dtfield/_imports.py` & `dtfield-0.1.9/dtfield/_imports.py`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.8/dtfield/base_enum.py` & `dtfield-0.1.9/dtfield/base_enum.py`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.8/dtfield/engine.py` & `dtfield-0.1.9/dtfield/engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -262,15 +262,15 @@
     
     @classmethod
     def model_dependants(cls, collection: list = None):
         return model_dependants(cls, collection or list())
 
     @classmethod
     def from_context(cls, key: str) -> Self:
-        data = cls.get_context()[key]
+        data = cls.get_context().get(key, None)
         if data:
             return cls.safe_create(**data)
         return None
     
     @classmethod
     async def set_context(cls):
         context.run(cls.CTXVAR.set, make_dict(await cls.fetch_all()))
```

### Comparing `dtfield-0.1.8/dtfield/functions.py` & `dtfield-0.1.9/dtfield/functions.py`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.8/dtfield/parse/__pycache__/dates.cpython-39.pyc` & `dtfield-0.1.9/dtfield/parse/__pycache__/dates.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.8/dtfield/parse/__pycache__/json_encoder.cpython-39.pyc` & `dtfield-0.1.9/dtfield/parse/__pycache__/json_encoder.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.8/dtfield/parse/__pycache__/null.cpython-39.pyc` & `dtfield-0.1.9/dtfield/parse/__pycache__/null.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.8/dtfield/parse/__pycache__/number.cpython-39.pyc` & `dtfield-0.1.9/dtfield/parse/__pycache__/number.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.8/dtfield/parse/__pycache__/string.cpython-39.pyc` & `dtfield-0.1.9/dtfield/parse/__pycache__/string.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.8/dtfield/parse/__pycache__/type_hint.cpython-39.pyc` & `dtfield-0.1.9/dtfield/parse/__pycache__/type_hint.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.8/dtfield/parse/dates.py` & `dtfield-0.1.9/dtfield/parse/dates.py`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.8/dtfield/parse/json_encoder.py` & `dtfield-0.1.9/dtfield/parse/json_encoder.py`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.8/dtfield/parse/number.py` & `dtfield-0.1.9/dtfield/parse/number.py`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.8/dtfield/parse/string.py` & `dtfield-0.1.9/dtfield/parse/string.py`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.8/dtfield/parse/type_hint.py` & `dtfield-0.1.9/dtfield/parse/type_hint.py`

 * *Files identical despite different names*

### Comparing `dtfield-0.1.8/setup.py` & `dtfield-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
  'anyio>=3.7.0,<4.0.0',
  'dtbase>=0.0.4,<0.0.5',
  'typing-extensions>=4.6.3,<5.0.0',
  'uvicorn>=0.22.0,<0.23.0']
 
 setup_kwargs = {
     'name': 'dtfield',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': '',
     'long_description': None,
     'author': 'Daniel Arantes',
     'author_email': 'arantesdv@me.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

