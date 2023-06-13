# Comparing `tmp/fastapi_swagger2-0.0.1b1.tar.gz` & `tmp/fastapi_swagger2-0.0.1b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_swagger2-0.0.1b1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `fastapi_swagger2-0.0.1b1.tar` & `fastapi_swagger2-0.0.1b2.tar`

### file list

```diff
@@ -1,15 +1,26 @@
--rw-r--r--   0        0        0     3089 2023-06-10 05:53:56.048517 fastapi_swagger2-0.0.1b1/.gitignore
--rw-r--r--   0        0        0     1070 2023-06-09 23:07:23.141403 fastapi_swagger2-0.0.1b1/LICENSE
--rw-r--r--   0        0        0     1626 2023-06-10 06:13:47.486469 fastapi_swagger2-0.0.1b1/README.md
--rw-r--r--   0        0        0     2514 2023-06-10 06:13:47.486691 fastapi_swagger2-0.0.1b1/pyproject.toml
--rwxr-xr-x   0        0        0       30 2023-06-10 06:13:47.486854 fastapi_swagger2-0.0.1b1/scripts/build.sh
--rwxr-xr-x   0        0        0       98 2023-06-10 06:13:47.486997 fastapi_swagger2-0.0.1b1/scripts/clean.sh
--rwxr-xr-x   0        0        0      149 2023-06-10 05:53:56.049126 fastapi_swagger2-0.0.1b1/scripts/format.sh
--rwxr-xr-x   0        0        0      197 2023-06-10 05:53:56.049314 fastapi_swagger2-0.0.1b1/scripts/lint.sh
--rwxr-xr-x   0        0        0       42 2023-06-10 05:53:56.049506 fastapi_swagger2-0.0.1b1/scripts/publish.sh
--rwxr-xr-x   0        0        0      175 2023-06-10 05:53:56.049786 fastapi_swagger2-0.0.1b1/scripts/test.sh
--rw-r--r--   0        0        0     4973 2023-06-10 05:53:56.050487 fastapi_swagger2-0.0.1b1/src/fastapi_swagger2/__init__.py
--rw-r--r--   0        0        0       30 2023-06-10 05:53:56.050740 fastapi_swagger2-0.0.1b1/src/fastapi_swagger2/constants.py
--rw-r--r--   0        0        0     7708 2023-06-10 05:53:56.050991 fastapi_swagger2-0.0.1b1/src/fastapi_swagger2/models.py
--rw-r--r--   0        0        0    14886 2023-06-10 05:53:56.051302 fastapi_swagger2-0.0.1b1/src/fastapi_swagger2/utils.py
--rw-r--r--   0        0        0     3670 1970-01-01 00:00:00.000000 fastapi_swagger2-0.0.1b1/PKG-INFO
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b2/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b2/.ruff_cache/.update-informer
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b2/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b2/.ruff_cache/content/10fbfe993ec4be0d
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b2/.ruff_cache/content/1abeadf52d9572ab
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b2/.ruff_cache/content/8cf332caaea8e79b
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b2/.ruff_cache/content/a8a883be09c5919b
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b2/.ruff_cache/content/c180a20ea5e70786
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b2/.ruff_cache/content/f16744491f37c6f5
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b2/.ruff_cache/content/f885759af04f4f9e
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b2/.ruff_cache/content/fbcf51701267e364
+-rwxr-xr-x   0        0        0       30 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b2/scripts/build.sh
+-rwxr-xr-x   0        0        0       98 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b2/scripts/clean.sh
+-rwxr-xr-x   0        0        0      149 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b2/scripts/format.sh
+-rwxr-xr-x   0        0        0      197 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b2/scripts/lint.sh
+-rwxr-xr-x   0        0        0       42 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b2/scripts/publish.sh
+-rwxr-xr-x   0        0        0      175 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b2/scripts/test.sh
+-rw-r--r--   0        0        0     4973 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b2/src/fastapi_swagger2/__init__.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b2/src/fastapi_swagger2/constants.py
+-rw-r--r--   0        0        0     9009 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b2/src/fastapi_swagger2/models.py
+-rw-r--r--   0        0        0    18683 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b2/src/fastapi_swagger2/utils.py
+-rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b2/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b2/LICENSE
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b2/README.md
+-rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b2/pyproject.toml
+-rw-r--r--   0        0        0     4909 2020-02-02 00:00:00.000000 fastapi_swagger2-0.0.1b2/PKG-INFO
```

### Comparing `fastapi_swagger2-0.0.1b1/.gitignore` & `fastapi_swagger2-0.0.1b2/.gitignore`

 * *Files identical despite different names*

### Comparing `fastapi_swagger2-0.0.1b1/LICENSE` & `fastapi_swagger2-0.0.1b2/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_swagger2-0.0.1b1/README.md` & `fastapi_swagger2-0.0.1b2/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_swagger2-0.0.1b1/pyproject.toml` & `fastapi_swagger2-0.0.1b2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fastapi_swagger2-0.0.1b1/src/fastapi_swagger2/__init__.py` & `fastapi_swagger2-0.0.1b2/src/fastapi_swagger2/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.0.1b1"
+__version__ = "0.0.1b2"
 
 from typing import Any, Dict, List, Optional, TypeVar
 
 from fastapi import FastAPI
 from fastapi.openapi.docs import (
     get_redoc_html,
     get_swagger_ui_html,
```

### Comparing `fastapi_swagger2-0.0.1b1/src/fastapi_swagger2/utils.py` & `fastapi_swagger2-0.0.1b2/src/fastapi_swagger2/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,30 @@
 import http.client
 import inspect
 from enum import Enum
 from typing import Any, Dict, List, Optional, Sequence, Set, Tuple, Type, Union, cast
 
 from fastapi import routing
 from fastapi.datastructures import DefaultPlaceholder
+from fastapi.dependencies.models import Dependant
 from fastapi.dependencies.utils import get_flat_dependant, get_flat_params
 from fastapi.encoders import jsonable_encoder
+from fastapi.logger import logger
 from fastapi.openapi.constants import METHODS_WITH_BODY
 from fastapi.openapi.utils import (
     get_flat_models_from_routes,
     get_openapi_operation_metadata,
-    get_openapi_security_definitions,
     status_code_ranges,
 )
 from fastapi.params import Body, Param
 from fastapi.responses import Response
-from fastapi.utils import (
-    deep_dict_update,
-    get_model_definitions,
-    is_body_allowed_for_status_code,
-)
+from fastapi.utils import deep_dict_update, is_body_allowed_for_status_code
 from pydantic import BaseModel
 from pydantic.fields import ModelField, Undefined
-from pydantic.schema import field_schema, get_model_name_map
+from pydantic.schema import field_schema, get_model_name_map, model_process_schema
 from pydantic.utils import lenient_issubclass
 from starlette.responses import JSONResponse
 from starlette.routing import BaseRoute
 from starlette.status import HTTP_422_UNPROCESSABLE_ENTITY
 
 from fastapi_swagger2.constants import REF_PREFIX
 from fastapi_swagger2.models import Swagger2
@@ -56,14 +53,105 @@
             "type": "array",
             "items": {"$ref": REF_PREFIX + "ValidationError"},
         }
     },
 }
 
 
+def get_model_definitions(
+    *,
+    flat_models: Set[Union[Type[BaseModel], Type[Enum]]],
+    model_name_map: Dict[Union[Type[BaseModel], Type[Enum]], str],
+) -> Dict[str, Any]:
+    definitions: Dict[str, Dict[str, Any]] = {}
+    for model in flat_models:
+        m_schema, m_definitions, m_nested_models = model_process_schema(
+            model, model_name_map=model_name_map, ref_prefix=REF_PREFIX
+        )
+        print(m_schema)
+        definitions.update(m_definitions)
+        model_name = model_name_map[model]
+        if "description" in m_schema:
+            m_schema["description"] = m_schema["description"].split("\f")[0]
+        definitions[model_name] = m_schema
+    return definitions
+
+
+def get_swagger2_security_definitions(
+    flat_dependant: Dependant,
+) -> Tuple[Dict[str, Any], List[Dict[str, Any]]]:
+    def _map_oauth2_flow(flow_key: str, flow: Dict[str, Any]) -> Dict[str, Any]:
+        security_definition = {
+            "type": "oauth2",
+            "flow": flow_key,
+            "scopes": flow["scopes"],
+        }
+        if "authorizationUrl" in flow:
+            security_definition.update({"authorizationUrl": flow["authorizationUrl"]})
+        if "tokenUrl" in flow:
+            security_definition.update({"tokenUrl": flow["tokenUrl"]})
+
+        return security_definition
+
+    oauth2_flows_keys_map = {
+        "implicit": "implicit",
+        "password": "password",
+        "clientCredentials": "application",
+        "authorizationCode": "accessCode",
+    }
+    security_definitions = {}
+    operation_security = []
+    for security_requirement in flat_dependant.security_requirements:
+        # fastapi.security.* which gets model from fastapi.openapi.models
+        security_definition = jsonable_encoder(
+            security_requirement.security_scheme.model,
+            by_alias=True,
+            exclude_none=True,
+        )
+        if security_definition["type"] == "http":
+            if security_definition.get("scheme", "basic") == "basic":
+                security_definition = {"type": "basic"}
+            else:
+                logger.warning(
+                    f"fastapi_swagger2: Unable to handle security_definition: {security_definition}"
+                )
+        elif security_definition["type"] == "apiKey":
+            pass
+        elif security_definition["type"] == "oauth2":
+            _security_definition = security_definition
+            flows = security_definition["flows"]
+            flows_keys = list(flows.keys())
+            if len(flows_keys) >= 1:
+                flow_key_3 = flows_keys[0]
+                flow = flows[flow_key_3]
+                security_definition = _map_oauth2_flow(
+                    oauth2_flows_keys_map[flow_key_3], flow
+                )
+
+                for i in range(1, len(flows_keys)):
+                    flow_key_3 = flows_keys[i]
+                    flow = flows[flow_key_3]
+                    flow_key_2 = oauth2_flows_keys_map[flow_key_3]
+                    security_definition_1 = _map_oauth2_flow(flow_key_2, flow)
+                    security_name = security_requirement.security_scheme.scheme_name
+                    _security_name = security_name + "_" + flow_key_2
+                    security_definitions[_security_name] = security_definition_1
+                    operation_security.append(
+                        {_security_name: security_requirement.scopes}
+                    )
+        else:
+            logger.warning(
+                f"fastapi_swagger2: Unable to handle security_definition: {security_definition}"
+            )
+        security_name = security_requirement.security_scheme.scheme_name
+        security_definitions[security_name] = security_definition
+        operation_security.append({security_name: security_requirement.scopes})
+    return security_definitions, operation_security
+
+
 def get_swagger2_operation_parameters(
     *,
     all_route_params: Sequence[ModelField],
     model_name_map: Dict[Union[Type[BaseModel], Type[Enum]], str],
 ) -> List[Dict[str, Any]]:
     parameters = []
     for param in all_route_params:
@@ -78,15 +166,15 @@
         }
         schema: Dict[str, Any] = field_schema(
             param, model_name_map=model_name_map, ref_prefix=REF_PREFIX
         )[0]
         if field_info.in_.value == "body":
             parameter["schema"] = schema
         else:
-            parameter.update({"type": schema["type"]})
+            parameter.update({k: v for (k, v) in schema.items() if k != "title"})
         if field_info.description:
             parameter["description"] = field_info.description
         if field_info.examples:
             parameter["examples"] = jsonable_encoder(field_info.examples)
         elif field_info.example != Undefined:
             parameter["example"] = jsonable_encoder(field_info.example)
         if field_info.deprecated:
@@ -144,17 +232,18 @@
         for method in route.methods:
             operation = get_openapi_operation_metadata(
                 route=route, method=method, operation_ids=operation_ids
             )
 
             parameters: List[Dict[str, Any]] = []
             flat_dependant = get_flat_dependant(route.dependant, skip_repeats=True)
-            security_definitions, operation_security = get_openapi_security_definitions(
-                flat_dependant=flat_dependant
-            )
+            (
+                security_definitions,
+                operation_security,
+            ) = get_swagger2_security_definitions(flat_dependant=flat_dependant)
 
             if operation_security:
                 operation.setdefault("security", []).extend(operation_security)
 
             if security_definitions:
                 security_schemes.update(security_definitions)
 
@@ -255,20 +344,16 @@
                     ), "An additional response must be a dict"
                     field = route.response_fields.get(additional_status_code)
                     additional_field_schema: Optional[Dict[str, Any]] = None
                     if field:
                         additional_field_schema, _, _ = field_schema(
                             field, model_name_map=model_name_map, ref_prefix=REF_PREFIX
                         )
-                        media_type = route_response_media_type or "application/json"
-                        additional_schema = (
-                            process_response.setdefault("content", {})
-                            .setdefault(media_type, {})
-                            .setdefault("schema", {})
-                        )
+                        # media_type = route_response_media_type or "application/json"
+                        additional_schema = process_response.setdefault("schema", {})
                         deep_dict_update(additional_schema, additional_field_schema)
                     status_text: Optional[str] = status_code_ranges.get(
                         str(additional_status_code).upper()
                     ) or http.client.responses.get(int(additional_status_code))
                     description = (
                         process_response.get("description")
                         or openapi_response.get("description")
@@ -344,15 +429,17 @@
             if result:
                 path, security_schemes, path_definitions = result
 
                 if path:
                     paths.setdefault(route.path_format, {}).update(path)
 
                 if security_schemes:
-                    output.setdefault("securitySchemes", {}).update(security_schemes)
+                    output.setdefault("securityDefinitions", {}).update(
+                        security_schemes
+                    )
 
                 if path_definitions:
                     definitions.update(path_definitions)
 
     output["paths"] = paths
 
     if definitions:
```

