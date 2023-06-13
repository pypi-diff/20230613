# Comparing `tmp/openapi_to_fastapi-0.8.0.tar.gz` & `tmp/openapi_to_fastapi-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openapi_to_fastapi-0.8.0.tar", max compression
+gzip compressed data, was "openapi_to_fastapi-0.9.0.tar", max compression
```

## Comparing `openapi_to_fastapi-0.8.0.tar` & `openapi_to_fastapi-0.9.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1496 2023-04-26 13:10:57.743727 openapi_to_fastapi-0.8.0/LICENSE
--rw-r--r--   0        0        0     7087 2023-04-26 13:10:57.743727 openapi_to_fastapi-0.8.0/README.md
--rw-r--r--   0        0        0        0 2023-04-26 13:10:57.743727 openapi_to_fastapi-0.8.0/openapi_to_fastapi/__init__.py
--rw-r--r--   0        0        0     2945 2023-04-26 13:10:57.743727 openapi_to_fastapi-0.8.0/openapi_to_fastapi/cli.py
--rw-r--r--   0        0        0       88 2023-04-26 13:10:57.743727 openapi_to_fastapi-0.8.0/openapi_to_fastapi/logger.py
--rw-r--r--   0        0        0     2922 2023-04-26 13:10:57.743727 openapi_to_fastapi-0.8.0/openapi_to_fastapi/model_generator.py
--rw-r--r--   0        0        0      513 2023-04-26 13:10:57.743727 openapi_to_fastapi-0.8.0/openapi_to_fastapi/models.py
--rw-r--r--   0        0        0     3855 2023-04-26 13:10:57.743727 openapi_to_fastapi-0.8.0/openapi_to_fastapi/parser.py
--rw-r--r--   0        0        0     7565 2023-04-26 13:10:57.743727 openapi_to_fastapi-0.8.0/openapi_to_fastapi/routes.py
--rw-r--r--   0        0        0        0 2023-04-26 13:10:57.743727 openapi_to_fastapi-0.8.0/openapi_to_fastapi/tests/__init__.py
--rw-r--r--   0        0        0      576 2023-04-26 13:10:57.743727 openapi_to_fastapi-0.8.0/openapi_to_fastapi/tests/conftest.py
--rw-r--r--   0        0        0     3863 2023-04-26 13:10:57.743727 openapi_to_fastapi-0.8.0/openapi_to_fastapi/tests/data/ihan/CompanyBasicInfo.json
--rw-r--r--   0        0        0     5201 2023-04-26 13:10:57.743727 openapi_to_fastapi-0.8.0/openapi_to_fastapi/tests/data/ihan/WeatherCurrentMetric.json
--rw-r--r--   0        0        0     3845 2023-04-26 13:10:57.743727 openapi_to_fastapi-0.8.0/openapi_to_fastapi/tests/data/pet_store/pet_store.json
--rw-r--r--   0        0        0        0 2023-04-26 13:10:57.743727 openapi_to_fastapi-0.8.0/openapi_to_fastapi/tests/snapshots/__init__.py
--rw-r--r--   0        0        0     1381 2023-04-26 13:10:57.743727 openapi_to_fastapi-0.8.0/openapi_to_fastapi/tests/snapshots/snap_test_router.py
--rw-r--r--   0        0        0     5841 2023-04-26 13:10:57.743727 openapi_to_fastapi-0.8.0/openapi_to_fastapi/tests/test_ihan_standards.py
--rw-r--r--   0        0        0     7022 2023-04-26 13:10:57.743727 openapi_to_fastapi-0.8.0/openapi_to_fastapi/tests/test_router.py
--rw-r--r--   0        0        0     1265 2023-04-26 13:10:57.743727 openapi_to_fastapi-0.8.0/openapi_to_fastapi/utils.py
--rw-r--r--   0        0        0      140 2023-04-26 13:10:57.743727 openapi_to_fastapi-0.8.0/openapi_to_fastapi/validator/__init__.py
--rw-r--r--   0        0        0     1070 2023-04-26 13:10:57.743727 openapi_to_fastapi-0.8.0/openapi_to_fastapi/validator/core.py
--rw-r--r--   0        0        0     3478 2023-04-26 13:10:57.743727 openapi_to_fastapi-0.8.0/openapi_to_fastapi/validator/ihan_standards.py
--rw-r--r--   0        0        0      911 2023-04-26 13:10:57.747727 openapi_to_fastapi-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     8015 1970-01-01 00:00:00.000000 openapi_to_fastapi-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1496 2023-06-07 07:31:51.010432 openapi_to_fastapi-0.9.0/LICENSE
+-rw-r--r--   0        0        0     7087 2023-06-07 07:31:51.010432 openapi_to_fastapi-0.9.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-07 07:31:51.010432 openapi_to_fastapi-0.9.0/openapi_to_fastapi/__init__.py
+-rw-r--r--   0        0        0     2945 2023-06-07 07:31:51.010432 openapi_to_fastapi-0.9.0/openapi_to_fastapi/cli.py
+-rw-r--r--   0        0        0       88 2023-06-07 07:31:51.010432 openapi_to_fastapi-0.9.0/openapi_to_fastapi/logger.py
+-rw-r--r--   0        0        0     2922 2023-06-07 07:31:51.010432 openapi_to_fastapi-0.9.0/openapi_to_fastapi/model_generator.py
+-rw-r--r--   0        0        0      513 2023-06-07 07:31:51.010432 openapi_to_fastapi-0.9.0/openapi_to_fastapi/models.py
+-rw-r--r--   0        0        0     3855 2023-06-07 07:31:51.010432 openapi_to_fastapi-0.9.0/openapi_to_fastapi/parser.py
+-rw-r--r--   0        0        0     7607 2023-06-07 07:31:51.010432 openapi_to_fastapi-0.9.0/openapi_to_fastapi/routes.py
+-rw-r--r--   0        0        0        0 2023-06-07 07:31:51.010432 openapi_to_fastapi-0.9.0/openapi_to_fastapi/tests/__init__.py
+-rw-r--r--   0        0        0      576 2023-06-07 07:31:51.010432 openapi_to_fastapi-0.9.0/openapi_to_fastapi/tests/conftest.py
+-rw-r--r--   0        0        0     3863 2023-06-07 07:31:51.014433 openapi_to_fastapi-0.9.0/openapi_to_fastapi/tests/data/ihan/CompanyBasicInfo.json
+-rw-r--r--   0        0        0     5201 2023-06-07 07:31:51.014433 openapi_to_fastapi-0.9.0/openapi_to_fastapi/tests/data/ihan/WeatherCurrentMetric.json
+-rw-r--r--   0        0        0     3845 2023-06-07 07:31:51.014433 openapi_to_fastapi-0.9.0/openapi_to_fastapi/tests/data/pet_store/pet_store.json
+-rw-r--r--   0        0        0        0 2023-06-07 07:31:51.014433 openapi_to_fastapi-0.9.0/openapi_to_fastapi/tests/snapshots/__init__.py
+-rw-r--r--   0        0        0     1381 2023-06-07 07:31:51.014433 openapi_to_fastapi-0.9.0/openapi_to_fastapi/tests/snapshots/snap_test_router.py
+-rw-r--r--   0        0        0     5841 2023-06-07 07:31:51.014433 openapi_to_fastapi-0.9.0/openapi_to_fastapi/tests/test_ihan_standards.py
+-rw-r--r--   0        0        0     7022 2023-06-07 07:31:51.014433 openapi_to_fastapi-0.9.0/openapi_to_fastapi/tests/test_router.py
+-rw-r--r--   0        0        0     1265 2023-06-07 07:31:51.014433 openapi_to_fastapi-0.9.0/openapi_to_fastapi/utils.py
+-rw-r--r--   0        0        0      140 2023-06-07 07:31:51.014433 openapi_to_fastapi-0.9.0/openapi_to_fastapi/validator/__init__.py
+-rw-r--r--   0        0        0     1070 2023-06-07 07:31:51.014433 openapi_to_fastapi-0.9.0/openapi_to_fastapi/validator/core.py
+-rw-r--r--   0        0        0     3478 2023-06-07 07:31:51.014433 openapi_to_fastapi-0.9.0/openapi_to_fastapi/validator/ihan_standards.py
+-rw-r--r--   0        0        0      911 2023-06-07 07:31:51.014433 openapi_to_fastapi-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     8015 1970-01-01 00:00:00.000000 openapi_to_fastapi-0.9.0/PKG-INFO
```

### Comparing `openapi_to_fastapi-0.8.0/LICENSE` & `openapi_to_fastapi-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openapi_to_fastapi-0.8.0/README.md` & `openapi_to_fastapi-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `openapi_to_fastapi-0.8.0/openapi_to_fastapi/cli.py` & `openapi_to_fastapi-0.9.0/openapi_to_fastapi/cli.py`

 * *Files identical despite different names*

### Comparing `openapi_to_fastapi-0.8.0/openapi_to_fastapi/model_generator.py` & `openapi_to_fastapi-0.9.0/openapi_to_fastapi/model_generator.py`

 * *Files identical despite different names*

### Comparing `openapi_to_fastapi-0.8.0/openapi_to_fastapi/models.py` & `openapi_to_fastapi-0.9.0/openapi_to_fastapi/models.py`

 * *Files identical despite different names*

### Comparing `openapi_to_fastapi-0.8.0/openapi_to_fastapi/parser.py` & `openapi_to_fastapi-0.9.0/openapi_to_fastapi/parser.py`

 * *Files identical despite different names*

### Comparing `openapi_to_fastapi-0.8.0/openapi_to_fastapi/routes.py` & `openapi_to_fastapi-0.9.0/openapi_to_fastapi/routes.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,16 +46,16 @@
             another_value = getattr(another_route, v)
             if another_value is not None:
                 setattr(self, v, another_value)
 
 
 @dataclass
 class RoutesMapping:
-    default_get: RouteInfo = RouteInfo()
-    default_post: RouteInfo = RouteInfo()
+    default_get: RouteInfo = field(default_factory=RouteInfo)
+    default_post: RouteInfo = field(default_factory=RouteInfo)
     get_map: Optional[Dict[str, RouteInfo]] = None
     post_map: Optional[Dict[str, RouteInfo]] = None
 
 
 class SpecRouter:
     def __init__(
         self,
```

### Comparing `openapi_to_fastapi-0.8.0/openapi_to_fastapi/tests/conftest.py` & `openapi_to_fastapi-0.9.0/openapi_to_fastapi/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `openapi_to_fastapi-0.8.0/openapi_to_fastapi/tests/data/ihan/CompanyBasicInfo.json` & `openapi_to_fastapi-0.9.0/openapi_to_fastapi/tests/data/ihan/CompanyBasicInfo.json`

 * *Files identical despite different names*

### Comparing `openapi_to_fastapi-0.8.0/openapi_to_fastapi/tests/data/ihan/WeatherCurrentMetric.json` & `openapi_to_fastapi-0.9.0/openapi_to_fastapi/tests/data/ihan/WeatherCurrentMetric.json`

 * *Files identical despite different names*

### Comparing `openapi_to_fastapi-0.8.0/openapi_to_fastapi/tests/data/pet_store/pet_store.json` & `openapi_to_fastapi-0.9.0/openapi_to_fastapi/tests/data/pet_store/pet_store.json`

 * *Files identical despite different names*

### Comparing `openapi_to_fastapi-0.8.0/openapi_to_fastapi/tests/snapshots/snap_test_router.py` & `openapi_to_fastapi-0.9.0/openapi_to_fastapi/tests/snapshots/snap_test_router.py`

 * *Files identical despite different names*

### Comparing `openapi_to_fastapi-0.8.0/openapi_to_fastapi/tests/test_ihan_standards.py` & `openapi_to_fastapi-0.9.0/openapi_to_fastapi/tests/test_ihan_standards.py`

 * *Files identical despite different names*

### Comparing `openapi_to_fastapi-0.8.0/openapi_to_fastapi/tests/test_router.py` & `openapi_to_fastapi-0.9.0/openapi_to_fastapi/tests/test_router.py`

 * *Files identical despite different names*

### Comparing `openapi_to_fastapi-0.8.0/openapi_to_fastapi/utils.py` & `openapi_to_fastapi-0.9.0/openapi_to_fastapi/utils.py`

 * *Files identical despite different names*

### Comparing `openapi_to_fastapi-0.8.0/openapi_to_fastapi/validator/core.py` & `openapi_to_fastapi-0.9.0/openapi_to_fastapi/validator/core.py`

 * *Files identical despite different names*

### Comparing `openapi_to_fastapi-0.8.0/openapi_to_fastapi/validator/ihan_standards.py` & `openapi_to_fastapi-0.9.0/openapi_to_fastapi/validator/ihan_standards.py`

 * *Files identical despite different names*

### Comparing `openapi_to_fastapi-0.8.0/pyproject.toml` & `openapi_to_fastapi-0.9.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [tool.poetry]
 name = "openapi-to-fastapi"
-version = "0.8.0"
+version = "0.9.0"
 description = "Create FastAPI routes from OpenAPI spec"
 authors = ["IOXIO Ltd"]
 license = "BSD-3-Clause"
 readme = "README.md"
 repository = "https://github.com/ioxiocom/openapi-to-fastapi"
 packages = [
     {include="openapi_to_fastapi", from="."}
 ]
 
 [tool.poetry.scripts]
 openapi-validator = "openapi_to_fastapi.cli:cli_validate_specs"
 
 [tool.poetry.dependencies]
 python = ">=3.7,<4.0.0"
-datamodel-code-generator = "^0.17.1"
-fastapi = "^0.94.0"
+datamodel-code-generator = "^0.19.0"
+fastapi = "^0.95.2"
 genson = "^1.2.2"
 click = "^8.1.3"
 coloredlogs = "^15.0.1"
 
 [tool.poetry.dev-dependencies]
 isort = "^5.10.1"
 pytest = "^7.2.2"
```

### Comparing `openapi_to_fastapi-0.8.0/PKG-INFO` & `openapi_to_fastapi-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: openapi-to-fastapi
-Version: 0.8.0
+Version: 0.9.0
 Summary: Create FastAPI routes from OpenAPI spec
 Home-page: https://github.com/ioxiocom/openapi-to-fastapi
 License: BSD-3-Clause
 Author: IOXIO Ltd
 Requires-Python: >=3.7,<4.0.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: coloredlogs (>=15.0.1,<16.0.0)
-Requires-Dist: datamodel-code-generator (>=0.17.1,<0.18.0)
-Requires-Dist: fastapi (>=0.94.0,<0.95.0)
+Requires-Dist: datamodel-code-generator (>=0.19.0,<0.20.0)
+Requires-Dist: fastapi (>=0.95.2,<0.96.0)
 Requires-Dist: genson (>=1.2.2,<2.0.0)
 Project-URL: Repository, https://github.com/ioxiocom/openapi-to-fastapi
 Description-Content-Type: text/markdown
 
 ## Reasoning
 
 [FastAPI](https://github.com/tiangolo/fastapi) is an awesome framework that simplifies
```

