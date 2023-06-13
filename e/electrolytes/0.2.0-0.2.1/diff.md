# Comparing `tmp/electrolytes-0.2.0.tar.gz` & `tmp/electrolytes-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "electrolytes-0.2.0.tar", last modified: Wed Dec 28 19:58:45 2022, max compression
+gzip compressed data, was "electrolytes-0.2.1.tar", last modified: Tue Jun 13 16:59:56 2023, max compression
```

## Comparing `electrolytes-0.2.0.tar` & `electrolytes-0.2.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 19:58:45.924449 electrolytes-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35130 2022-12-28 19:58:35.000000 electrolytes-0.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2022-12-28 19:58:35.000000 electrolytes-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5278 2022-12-28 19:58:45.928449 electrolytes-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4095 2022-12-28 19:58:35.000000 electrolytes-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 19:58:45.924449 electrolytes-0.2.0/electrolytes/
--rw-r--r--   0 runner    (1001) docker     (123)     6394 2022-12-28 19:58:35.000000 electrolytes-0.2.0/electrolytes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6196 2022-12-28 19:58:35.000000 electrolytes-0.2.0/electrolytes/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 19:58:45.924449 electrolytes-0.2.0/electrolytes/data/
--rw-r--r--   0 runner    (1001) docker     (123)   174238 2022-12-28 19:58:35.000000 electrolytes-0.2.0/electrolytes/data/db1.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 19:58:45.924449 electrolytes-0.2.0/electrolytes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5278 2022-12-28 19:58:45.000000 electrolytes-0.2.0/electrolytes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      416 2022-12-28 19:58:45.000000 electrolytes-0.2.0/electrolytes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-28 19:58:45.000000 electrolytes-0.2.0/electrolytes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2022-12-28 19:58:45.000000 electrolytes-0.2.0/electrolytes.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2022-12-28 19:58:45.000000 electrolytes-0.2.0/electrolytes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2022-12-28 19:58:45.000000 electrolytes-0.2.0/electrolytes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2022-12-28 19:58:35.000000 electrolytes-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2022-12-28 19:58:45.928449 electrolytes-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       36 2022-12-28 19:58:35.000000 electrolytes-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 19:58:45.924449 electrolytes-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-28 19:58:35.000000 electrolytes-0.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2022-12-28 19:58:35.000000 electrolytes-0.2.0/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2022-12-28 19:58:35.000000 electrolytes-0.2.0/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:59:56.571194 electrolytes-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35130 2023-06-13 16:59:39.000000 electrolytes-0.2.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-13 16:59:39.000000 electrolytes-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5274 2023-06-13 16:59:56.571194 electrolytes-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-06-13 16:59:39.000000 electrolytes-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:59:56.567194 electrolytes-0.2.1/electrolytes/
+-rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-06-13 16:59:39.000000 electrolytes-0.2.1/electrolytes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-06-13 16:59:39.000000 electrolytes-0.2.1/electrolytes/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:59:56.567194 electrolytes-0.2.1/electrolytes/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   174238 2023-06-13 16:59:39.000000 electrolytes-0.2.1/electrolytes/data/db1.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:59:56.567194 electrolytes-0.2.1/electrolytes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5274 2023-06-13 16:59:56.000000 electrolytes-0.2.1/electrolytes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-13 16:59:56.000000 electrolytes-0.2.1/electrolytes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 16:59:56.000000 electrolytes-0.2.1/electrolytes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-13 16:59:56.000000 electrolytes-0.2.1/electrolytes.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-13 16:59:56.000000 electrolytes-0.2.1/electrolytes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-13 16:59:56.000000 electrolytes-0.2.1/electrolytes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-13 16:59:39.000000 electrolytes-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-13 16:59:56.571194 electrolytes-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-13 16:59:39.000000 electrolytes-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:59:56.567194 electrolytes-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 16:59:39.000000 electrolytes-0.2.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-13 16:59:39.000000 electrolytes-0.2.1/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-06-13 16:59:39.000000 electrolytes-0.2.1/tests/test_cli.py
```

### Comparing `electrolytes-0.2.0/LICENSE.txt` & `electrolytes-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `electrolytes-0.2.0/PKG-INFO` & `electrolytes-0.2.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: electrolytes
-Version: 0.2.0
+Version: 0.2.1
 Summary: Electrolyte database manager
 Home-page: https://github.com/microfluidica/electrolytes
 Author: Gabriel S. Gerlero
 Author-email: ggerlero@cimec.unl.edu.ar
 Project-URL: Source Code, https://github.com/microfluidica/electrolytes
 Project-URL: Bug Tracker, https://github.com/microfluidica/electrolytes/issues
 Classifier: Development Status :: 4 - Beta
@@ -90,16 +90,16 @@
     def __init__(self,
                  *,
                  name: str,
                  u_neg: Sequence[float],  # [-neg_count, -neg_count+1, -neg_count+2, ..., -1]
                  u_pos: Sequence[float],  # [+1, +2, +3, ..., +pos_count]
                  pkas_neg: Sequence[float],  # [-neg_count, -neg_count+1, -neg_count+2, ..., -1]
                  pkas_pos: Sequence[float],  # [+1, +2, +3, ..., +pos_count]
-                 neg_count: int = None,
-                 pos_count: int = None): ...
+                 neg_count: int = -1,
+                 pos_count: int = -1): ...
 
     # Interface for electroMicroTransport
     def mobilities(self) -> Sequence[float]: ...  # [+n, ..., +3, +2, +1, -1, -2, -3, ..., -n] (with n >= 3), SI units
     def pkas(self) -> Sequence[float]: ...  # [+n, ..., +3, +2, +1, -1, -2, -3, ..., -n] (with n >= 3)
     def diffusivity(self) -> float: ...  # SI units
 ```
```

### Comparing `electrolytes-0.2.0/README.md` & `electrolytes-0.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -62,16 +62,16 @@
     def __init__(self,
                  *,
                  name: str,
                  u_neg: Sequence[float],  # [-neg_count, -neg_count+1, -neg_count+2, ..., -1]
                  u_pos: Sequence[float],  # [+1, +2, +3, ..., +pos_count]
                  pkas_neg: Sequence[float],  # [-neg_count, -neg_count+1, -neg_count+2, ..., -1]
                  pkas_pos: Sequence[float],  # [+1, +2, +3, ..., +pos_count]
-                 neg_count: int = None,
-                 pos_count: int = None): ...
+                 neg_count: int = -1,
+                 pos_count: int = -1): ...
 
     # Interface for electroMicroTransport
     def mobilities(self) -> Sequence[float]: ...  # [+n, ..., +3, +2, +1, -1, -2, -3, ..., -n] (with n >= 3), SI units
     def pkas(self) -> Sequence[float]: ...  # [+n, ..., +3, +2, +1, -1, -2, -3, ..., -n] (with n >= 3)
     def diffusivity(self) -> float: ...  # SI units
 ```
```

### Comparing `electrolytes-0.2.0/electrolytes/__init__.py` & `electrolytes-0.2.1/electrolytes/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,26 +4,26 @@
 from typing import Iterable, Iterator, List, Sequence, Dict, Optional
 
 from pydantic import BaseModel, Field, validator, root_validator, parse_file_as, parse_raw_as
 from typer import get_app_dir
 
 _APP_NAME = "electrolytes"
 
-__version__ = "0.2.0"
+__version__ = "0.2.1"
 
 
 class Constituent(BaseModel):
     id: int = -1
     name: str
     u_neg: List[float] = Field([], alias="uNeg") # [-neg_count, -neg_count+1, -neg_count+2, ..., -1]
     u_pos: List[float] = Field([], alias="uPos") # [+1, +2, +3, ..., +pos_count]
     pkas_neg: List[float] = Field([], alias="pKaNeg") # [-neg_count, -neg_count+1, -neg_count+2, ..., -1]
     pkas_pos: List[float] = Field([], alias="pKaPos") # [+1, +2, +3, ..., +pos_count]
-    neg_count: int = Field(None, alias="negCount")
-    pos_count: int = Field(None, alias="posCount")
+    neg_count: int = Field(-1, alias="negCount")
+    pos_count: int = Field(-1, alias="posCount")
 
     @property
     def charges_neg(self) -> range:
         return range(-self.neg_count, 0)
 
     @property
     def charges_pos(self) -> range:
@@ -69,15 +69,15 @@
     def pka_lengths(cls, v, values, field):
         if len(v) != len(values[f"u_{field.name[5:]}"]):
             raise ValueError(f"len({field.name}) != len(u_{field.name[5:]})")
         return v
  
     @validator("neg_count", "pos_count", always=True)
     def counts(cls, v, values, field):
-        if v is None:
+        if v == -1:
             v = len(values[f"u_{field.name[:3]}"])
         elif v != len(values[f"u_{field.name[:3]}"]):
             raise ValueError(f"{field.name} != len(u_{field.name[:3]})")
         return v
 
     @root_validator
     def pkas_not_increasing(cls, values):
```

### Comparing `electrolytes-0.2.0/electrolytes/__main__.py` & `electrolytes-0.2.1/electrolytes/__main__.py`

 * *Files identical despite different names*

### Comparing `electrolytes-0.2.0/electrolytes/data/db1.json` & `electrolytes-0.2.1/electrolytes/data/db1.json`

 * *Files identical despite different names*

### Comparing `electrolytes-0.2.0/electrolytes.egg-info/PKG-INFO` & `electrolytes-0.2.1/electrolytes.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: electrolytes
-Version: 0.2.0
+Version: 0.2.1
 Summary: Electrolyte database manager
 Home-page: https://github.com/microfluidica/electrolytes
 Author: Gabriel S. Gerlero
 Author-email: ggerlero@cimec.unl.edu.ar
 Project-URL: Source Code, https://github.com/microfluidica/electrolytes
 Project-URL: Bug Tracker, https://github.com/microfluidica/electrolytes/issues
 Classifier: Development Status :: 4 - Beta
@@ -90,16 +90,16 @@
     def __init__(self,
                  *,
                  name: str,
                  u_neg: Sequence[float],  # [-neg_count, -neg_count+1, -neg_count+2, ..., -1]
                  u_pos: Sequence[float],  # [+1, +2, +3, ..., +pos_count]
                  pkas_neg: Sequence[float],  # [-neg_count, -neg_count+1, -neg_count+2, ..., -1]
                  pkas_pos: Sequence[float],  # [+1, +2, +3, ..., +pos_count]
-                 neg_count: int = None,
-                 pos_count: int = None): ...
+                 neg_count: int = -1,
+                 pos_count: int = -1): ...
 
     # Interface for electroMicroTransport
     def mobilities(self) -> Sequence[float]: ...  # [+n, ..., +3, +2, +1, -1, -2, -3, ..., -n] (with n >= 3), SI units
     def pkas(self) -> Sequence[float]: ...  # [+n, ..., +3, +2, +1, -1, -2, -3, ..., -n] (with n >= 3)
     def diffusivity(self) -> float: ...  # SI units
 ```
```

### Comparing `electrolytes-0.2.0/setup.cfg` & `electrolytes-0.2.1/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -41,11 +41,14 @@
 	pytest>=6.2.4,<8
 	pytest-cov
 lint = 
 	%(test)s
 	mypy
 	check-manifest
 
+[mypy]
+plugins = pydantic.mypy
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `electrolytes-0.2.0/tests/test_api.py` & `electrolytes-0.2.1/tests/test_api.py`

 * *Files 14% similar despite different names*

```diff
@@ -45,10 +45,13 @@
         del database["NONEXISTENT2424612644"]
         
 
 def test_try_add_default() -> None:
     assert "SILVER" in database
     assert not database.is_user_defined("SILVER")
     assert "SILVER" not in database.user_defined()
-    with pytest.raises(ValueError):
-        database.add(Constituent(u_pos=[64.50],
-                                 pkas_pos=[11.70]))
+    database.add(Constituent(name="SILVER",
+                                u_pos=[64.50],
+                                pkas_pos=[11.70]))
+    assert "SILVER" in database
+    assert not database.is_user_defined("SILVER")
+    assert "SILVER" not in database.user_defined()
```

### Comparing `electrolytes-0.2.0/tests/test_cli.py` & `electrolytes-0.2.1/tests/test_cli.py`

 * *Files identical despite different names*

