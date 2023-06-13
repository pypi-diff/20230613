# Comparing `tmp/teritorio-2023.4.28.tar.gz` & `tmp/teritorio-2023.6.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "teritorio-2023.4.28.tar", max compression
+gzip compressed data, was "teritorio-2023.6.13.tar", max compression
```

## Comparing `teritorio-2023.4.28.tar` & `teritorio-2023.6.13.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     7652 2023-01-28 23:28:39.058913 teritorio-2023.4.28/LICENSE.txt
--rw-r--r--   0        0        0     2377 2023-03-12 00:03:02.409875 teritorio-2023.4.28/README.rst
--rw-r--r--   0        0        0     2845 2023-04-28 14:54:20.747121 teritorio-2023.4.28/pyproject.toml
--rw-r--r--   0        0        0      115 2023-01-28 23:28:39.059785 teritorio-2023.4.28/src/teritorio/__init__.py
--rw-r--r--   0        0        0    48421 2023-04-28 14:44:19.353103 teritorio-2023.4.28/src/teritorio/_data/country.json
--rw-r--r--   0        0        0    37324 2023-04-28 13:07:47.892608 teritorio-2023.4.28/src/teritorio/_data/currency.json
--rw-r--r--   0        0        0     2219 2023-04-28 11:59:18.006870 teritorio-2023.4.28/src/teritorio/main.py
--rw-r--r--   0        0        0        0 2023-01-28 23:28:39.060375 teritorio-2023.4.28/src/teritorio/py.typed
--rw-r--r--   0        0        0     3414 1970-01-01 00:00:00.000000 teritorio-2023.4.28/PKG-INFO
+-rw-r--r--   0        0        0     7652 2023-01-28 23:28:39.058913 teritorio-2023.6.13/LICENSE.txt
+-rw-r--r--   0        0        0     2377 2023-03-12 00:03:02.409875 teritorio-2023.6.13/README.rst
+-rw-r--r--   0        0        0     2845 2023-06-13 10:15:33.548999 teritorio-2023.6.13/pyproject.toml
+-rw-r--r--   0        0        0      115 2023-06-13 10:15:33.535018 teritorio-2023.6.13/src/teritorio/__init__.py
+-rw-r--r--   0        0        0    48421 2023-06-13 10:03:35.128241 teritorio-2023.6.13/src/teritorio/_data/country.json
+-rw-r--r--   0        0        0    37324 2023-06-13 09:56:39.706171 teritorio-2023.6.13/src/teritorio/_data/currency.json
+-rw-r--r--   0        0        0     2495 2023-06-13 09:47:45.163616 teritorio-2023.6.13/src/teritorio/main.py
+-rw-r--r--   0        0        0        0 2023-01-28 23:28:39.060375 teritorio-2023.6.13/src/teritorio/py.typed
+-rw-r--r--   0        0        0     3414 1970-01-01 00:00:00.000000 teritorio-2023.6.13/PKG-INFO
```

### Comparing `teritorio-2023.4.28/LICENSE.txt` & `teritorio-2023.6.13/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `teritorio-2023.4.28/README.rst` & `teritorio-2023.6.13/README.rst`

 * *Files identical despite different names*

### Comparing `teritorio-2023.4.28/pyproject.toml` & `teritorio-2023.6.13/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -101,15 +101,15 @@
 [tool.coverage.report]
 show_missing = true
 skip_covered = true
 skip_empty = true
 
 [tool.poetry]
 name = "teritorio"
-version = "2023.04.28"
+version = "2023.06.13"
 description = "A library for country and currency ISO codes"
 authors = [
     "Stephanos Kuma <stephanos@kuma.ai>",
 ]
 
 license = "LGPL-3.0+"
 readme = "README.rst"
```

### Comparing `teritorio-2023.4.28/src/teritorio/_data/country.json` & `teritorio-2023.6.13/src/teritorio/_data/country.json`

 * *Files identical despite different names*

### Comparing `teritorio-2023.4.28/src/teritorio/_data/currency.json` & `teritorio-2023.6.13/src/teritorio/_data/currency.json`

 * *Files identical despite different names*

### Comparing `teritorio-2023.4.28/src/teritorio/main.py` & `teritorio-2023.6.13/src/teritorio/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 from __future__ import annotations
 
 import json
 from dataclasses import dataclass
 from pathlib import Path
-from typing import Any, Generic, TypeVar, cast
+from typing import Any, Generic, TypeVar
 
 T = TypeVar("T")
 
 
 class Singleton(type):
-    def __init__(cls, name: str, bases: tuple[type, ...], dict_: dict[str, Any]):
+    instance: type[Singleton] | None
+
+    def __init__(
+        cls, name: str, bases: tuple[type[Singleton], ...], dict_: dict[str, Any]
+    ):
         super().__init__(name, bases, dict_)
-        cls.instance: Singleton | None = None
+        cls.instance = None
 
-    def __call__(cls) -> Singleton:
+    def __call__(cls) -> type[Singleton]:
         if cls.instance is None:
-            cls.instance = cast(Singleton, super().__call__())
+            cls.instance = super().__call__()
         return cls.instance
 
 
 class DataListIterator(Generic[T]):
     def __init__(self, data: dict[str, T]) -> None:
         self.values = (data[key] for key in sorted(data))
 
@@ -32,15 +36,15 @@
 
 class DataList(Generic[T]):
     _data_path: Path
     _object_class: type[T]
 
     def __init__(self) -> None:
         with self._data_path.open() as file:
-            data = json.load(file)
+            data = json.load(file, object_hook=_list_to_tuple)
 
         self._data: dict[str, T] = {}
         for key, raw_obj in data.items():
             obj = self._object_class(**raw_obj)
             self._data[key] = obj
             setattr(self, key, obj)
 
@@ -74,15 +78,23 @@
     _object_class = Country
 
 
 @dataclass(frozen=True, order=True)
 class Currency:
     code: str
     name: str
-    entities: list[str]
+    entities: tuple[str, ...]
     numeric_code: int
     minor_units: int | None
 
 
 class Currencies(DataList[Currency], metaclass=Singleton):
     _data_path = Path(__file__).parent.joinpath("_data/currency.json")
     _object_class = Currency
+
+
+def _list_to_tuple(obj: Any) -> Any:
+    if isinstance(obj, list):
+        return tuple(obj)
+    if isinstance(obj, dict):
+        return {key: _list_to_tuple(value) for key, value in obj.items()}
+    return obj
```

### Comparing `teritorio-2023.4.28/PKG-INFO` & `teritorio-2023.6.13/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teritorio
-Version: 2023.4.28
+Version: 2023.6.13
 Summary: A library for country and currency ISO codes
 Home-page: https://teritorio.readthedocs.io/en/stable/
 License: LGPL-3.0+
 Keywords: iso,currency,country
 Author: Stephanos Kuma
 Author-email: stephanos@kuma.ai
 Requires-Python: >=3.7,<4.0
```

