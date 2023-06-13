# Comparing `tmp/permit-2.0.4.tar.gz` & `tmp/permit-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "permit-2.0.4.tar", last modified: Sun Jun 11 08:57:44 2023, max compression
+gzip compressed data, was "permit-2.0.5.tar", last modified: Tue Jun 13 07:23:11 2023, max compression
```

## Comparing `permit-2.0.4.tar` & `permit-2.0.5.tar`

### file list

```diff
@@ -1,58 +1,59 @@
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-06-11 08:57:44.261546 permit-2.0.4/
--rw-r--r--   0 asafc      (501) staff       (20)    11357 2023-05-22 06:43:35.000000 permit-2.0.4/LICENSE
--rw-r--r--   0 asafc      (501) staff       (20)       30 2022-10-01 21:14:31.000000 permit-2.0.4/MANIFEST.in
--rw-r--r--   0 asafc      (501) staff       (20)      478 2023-06-11 08:57:44.261401 permit-2.0.4/PKG-INFO
--rw-r--r--   0 asafc      (501) staff       (20)      268 2023-05-22 06:43:35.000000 permit-2.0.4/README.md
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-06-11 08:57:44.256623 permit-2.0.4/permit/
--rw-r--r--   0 asafc      (501) staff       (20)      373 2023-05-22 06:43:35.000000 permit-2.0.4/permit/__init__.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-06-11 08:57:44.259779 permit-2.0.4/permit/api/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2023-05-22 06:43:35.000000 permit-2.0.4/permit/api/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     4185 2023-06-07 19:13:45.000000 permit-2.0.4/permit/api/api_client.py
--rw-r--r--   0 asafc      (501) staff       (20)     9966 2023-06-10 13:49:09.000000 permit-2.0.4/permit/api/base.py
--rw-r--r--   0 asafc      (501) staff       (20)     3601 2023-05-22 06:43:35.000000 permit-2.0.4/permit/api/condition_set_rules.py
--rw-r--r--   0 asafc      (501) staff       (20)     5424 2023-05-22 06:43:35.000000 permit-2.0.4/permit/api/condition_sets.py
--rw-r--r--   0 asafc      (501) staff       (20)     3686 2023-06-10 13:49:09.000000 permit-2.0.4/permit/api/context.py
--rw-r--r--   0 asafc      (501) staff       (20)     6805 2023-05-22 12:10:06.000000 permit-2.0.4/permit/api/deprecated.py
--rw-r--r--   0 asafc      (501) staff       (20)     1946 2023-05-22 12:10:06.000000 permit-2.0.4/permit/api/elements.py
--rw-r--r--   0 asafc      (501) staff       (20)     8771 2023-06-10 13:49:09.000000 permit-2.0.4/permit/api/environments.py
--rw-r--r--   0 asafc      (501) staff       (20)   137660 2023-06-07 19:13:45.000000 permit-2.0.4/permit/api/models.py
--rw-r--r--   0 asafc      (501) staff       (20)     5063 2023-06-10 13:49:09.000000 permit-2.0.4/permit/api/projects.py
--rw-r--r--   0 asafc      (501) staff       (20)     5378 2023-06-07 19:13:45.000000 permit-2.0.4/permit/api/resource_action_groups.py
--rw-r--r--   0 asafc      (501) staff       (20)     6010 2023-05-22 06:43:35.000000 permit-2.0.4/permit/api/resource_actions.py
--rw-r--r--   0 asafc      (501) staff       (20)     6310 2023-05-22 06:43:35.000000 permit-2.0.4/permit/api/resource_attributes.py
--rw-r--r--   0 asafc      (501) staff       (20)     5971 2023-05-22 06:43:35.000000 permit-2.0.4/permit/api/resources.py
--rw-r--r--   0 asafc      (501) staff       (20)     5397 2023-06-07 19:13:45.000000 permit-2.0.4/permit/api/role_assignments.py
--rw-r--r--   0 asafc      (501) staff       (20)     6647 2023-05-22 06:43:35.000000 permit-2.0.4/permit/api/roles.py
--rw-r--r--   0 asafc      (501) staff       (20)     5318 2023-05-22 06:43:35.000000 permit-2.0.4/permit/api/sync_api_client.py
--rw-r--r--   0 asafc      (501) staff       (20)     6705 2023-05-22 06:43:35.000000 permit-2.0.4/permit/api/tenants.py
--rw-r--r--   0 asafc      (501) staff       (20)     8875 2023-05-22 12:10:06.000000 permit-2.0.4/permit/api/users.py
--rw-r--r--   0 asafc      (501) staff       (20)     2039 2023-05-22 06:43:35.000000 permit-2.0.4/permit/config.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-06-11 08:57:44.260141 permit-2.0.4/permit/enforcement/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:14:31.000000 permit-2.0.4/permit/enforcement/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     7073 2023-05-22 06:43:35.000000 permit-2.0.4/permit/enforcement/enforcer.py
--rw-r--r--   0 asafc      (501) staff       (20)      742 2022-10-01 21:14:31.000000 permit-2.0.4/permit/enforcement/interfaces.py
--rw-r--r--   0 asafc      (501) staff       (20)     2849 2023-06-11 08:57:33.000000 permit-2.0.4/permit/exceptions.py
--rw-r--r--   0 asafc      (501) staff       (20)      212 2023-05-22 06:43:35.000000 permit-2.0.4/permit/logger.py
--rw-r--r--   0 asafc      (501) staff       (20)     3116 2023-05-22 06:43:35.000000 permit-2.0.4/permit/permit.py
--rw-r--r--   0 asafc      (501) staff       (20)     2494 2023-05-22 06:43:35.000000 permit-2.0.4/permit/sync.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-06-11 08:57:44.260544 permit-2.0.4/permit/utils/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:14:31.000000 permit-2.0.4/permit/utils/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)      836 2023-05-22 06:43:35.000000 permit-2.0.4/permit/utils/context.py
--rw-r--r--   0 asafc      (501) staff       (20)      444 2022-10-01 21:14:31.000000 permit-2.0.4/permit/utils/dicts.py
--rw-r--r--   0 asafc      (501) staff       (20)     1496 2023-05-22 06:43:35.000000 permit-2.0.4/permit/utils/sync.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-06-11 08:57:44.257196 permit-2.0.4/permit.egg-info/
--rw-r--r--   0 asafc      (501) staff       (20)      478 2023-06-11 08:57:44.000000 permit-2.0.4/permit.egg-info/PKG-INFO
--rw-r--r--   0 asafc      (501) staff       (20)     1142 2023-06-11 08:57:44.000000 permit-2.0.4/permit.egg-info/SOURCES.txt
--rw-r--r--   0 asafc      (501) staff       (20)        1 2023-06-11 08:57:44.000000 permit-2.0.4/permit.egg-info/dependency_links.txt
--rw-r--r--   0 asafc      (501) staff       (20)      107 2023-06-11 08:57:44.000000 permit-2.0.4/permit.egg-info/requires.txt
--rw-r--r--   0 asafc      (501) staff       (20)       13 2023-06-11 08:57:44.000000 permit-2.0.4/permit.egg-info/top_level.txt
--rw-r--r--   0 asafc      (501) staff       (20)      107 2023-05-22 06:43:35.000000 permit-2.0.4/requirements.txt
--rw-r--r--   0 asafc      (501) staff       (20)       38 2023-06-11 08:57:44.261585 permit-2.0.4/setup.cfg
--rw-r--r--   0 asafc      (501) staff       (20)      793 2023-06-11 08:57:33.000000 permit-2.0.4/setup.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-06-11 08:57:44.261216 permit-2.0.4/tests/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:14:31.000000 permit-2.0.4/tests/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     1191 2023-05-22 11:43:03.000000 permit-2.0.4/tests/conftest.py
--rw-r--r--   0 asafc      (501) staff       (20)     9377 2023-06-11 08:57:33.000000 permit-2.0.4/tests/test_abac_e2e.py
--rw-r--r--   0 asafc      (501) staff       (20)     8890 2023-06-11 08:57:33.000000 permit-2.0.4/tests/test_rbac_e2e.py
--rw-r--r--   0 asafc      (501) staff       (20)     8811 2023-06-11 08:57:33.000000 permit-2.0.4/tests/test_rbac_e2e_sync.py
--rw-r--r--   0 asafc      (501) staff       (20)      323 2023-05-22 06:43:35.000000 permit-2.0.4/tests/utils.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-06-13 07:23:11.562352 permit-2.0.5/
+-rw-r--r--   0 asafc      (501) staff       (20)    11357 2023-05-22 06:43:35.000000 permit-2.0.5/LICENSE
+-rw-r--r--   0 asafc      (501) staff       (20)       30 2022-10-01 21:14:31.000000 permit-2.0.5/MANIFEST.in
+-rw-r--r--   0 asafc      (501) staff       (20)      478 2023-06-13 07:23:11.562226 permit-2.0.5/PKG-INFO
+-rw-r--r--   0 asafc      (501) staff       (20)      268 2023-05-22 06:43:35.000000 permit-2.0.5/README.md
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-06-13 07:23:11.558046 permit-2.0.5/permit/
+-rw-r--r--   0 asafc      (501) staff       (20)      373 2023-05-22 06:43:35.000000 permit-2.0.5/permit/__init__.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-06-13 07:23:11.560785 permit-2.0.5/permit/api/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2023-05-22 06:43:35.000000 permit-2.0.5/permit/api/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)     4185 2023-06-07 19:13:45.000000 permit-2.0.5/permit/api/api_client.py
+-rw-r--r--   0 asafc      (501) staff       (20)    11803 2023-06-13 07:23:03.000000 permit-2.0.5/permit/api/base.py
+-rw-r--r--   0 asafc      (501) staff       (20)     3862 2023-06-13 07:23:03.000000 permit-2.0.5/permit/api/condition_set_rules.py
+-rw-r--r--   0 asafc      (501) staff       (20)     6060 2023-06-13 07:23:03.000000 permit-2.0.5/permit/api/condition_sets.py
+-rw-r--r--   0 asafc      (501) staff       (20)     8347 2023-06-13 07:23:03.000000 permit-2.0.5/permit/api/context.py
+-rw-r--r--   0 asafc      (501) staff       (20)     6493 2023-06-13 07:23:03.000000 permit-2.0.5/permit/api/deprecated.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1946 2023-05-22 12:10:06.000000 permit-2.0.5/permit/api/elements.py
+-rw-r--r--   0 asafc      (501) staff       (20)     9660 2023-06-13 07:23:03.000000 permit-2.0.5/permit/api/environments.py
+-rw-r--r--   0 asafc      (501) staff       (20)   137660 2023-06-07 19:13:45.000000 permit-2.0.5/permit/api/models.py
+-rw-r--r--   0 asafc      (501) staff       (20)     5706 2023-06-13 07:23:03.000000 permit-2.0.5/permit/api/projects.py
+-rw-r--r--   0 asafc      (501) staff       (20)     5975 2023-06-13 07:23:03.000000 permit-2.0.5/permit/api/resource_action_groups.py
+-rw-r--r--   0 asafc      (501) staff       (20)     6667 2023-06-13 07:23:03.000000 permit-2.0.5/permit/api/resource_actions.py
+-rw-r--r--   0 asafc      (501) staff       (20)     6990 2023-06-13 07:23:03.000000 permit-2.0.5/permit/api/resource_attributes.py
+-rw-r--r--   0 asafc      (501) staff       (20)     6656 2023-06-13 07:23:03.000000 permit-2.0.5/permit/api/resources.py
+-rw-r--r--   0 asafc      (501) staff       (20)     5784 2023-06-13 07:23:03.000000 permit-2.0.5/permit/api/role_assignments.py
+-rw-r--r--   0 asafc      (501) staff       (20)     7383 2023-06-13 07:23:03.000000 permit-2.0.5/permit/api/roles.py
+-rw-r--r--   0 asafc      (501) staff       (20)     5318 2023-05-22 06:43:35.000000 permit-2.0.5/permit/api/sync_api_client.py
+-rw-r--r--   0 asafc      (501) staff       (20)     7447 2023-06-13 07:23:03.000000 permit-2.0.5/permit/api/tenants.py
+-rw-r--r--   0 asafc      (501) staff       (20)     9737 2023-06-13 07:23:03.000000 permit-2.0.5/permit/api/users.py
+-rw-r--r--   0 asafc      (501) staff       (20)     2039 2023-05-22 06:43:35.000000 permit-2.0.5/permit/config.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-06-13 07:23:11.561059 permit-2.0.5/permit/enforcement/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:14:31.000000 permit-2.0.5/permit/enforcement/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)     7440 2023-06-13 07:23:03.000000 permit-2.0.5/permit/enforcement/enforcer.py
+-rw-r--r--   0 asafc      (501) staff       (20)      742 2022-10-01 21:14:31.000000 permit-2.0.5/permit/enforcement/interfaces.py
+-rw-r--r--   0 asafc      (501) staff       (20)     3125 2023-06-13 07:23:03.000000 permit-2.0.5/permit/exceptions.py
+-rw-r--r--   0 asafc      (501) staff       (20)      212 2023-05-22 06:43:35.000000 permit-2.0.5/permit/logger.py
+-rw-r--r--   0 asafc      (501) staff       (20)     3116 2023-05-22 06:43:35.000000 permit-2.0.5/permit/permit.py
+-rw-r--r--   0 asafc      (501) staff       (20)     2494 2023-05-22 06:43:35.000000 permit-2.0.5/permit/sync.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-06-13 07:23:11.561517 permit-2.0.5/permit/utils/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:14:31.000000 permit-2.0.5/permit/utils/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)      836 2023-05-22 06:43:35.000000 permit-2.0.5/permit/utils/context.py
+-rw-r--r--   0 asafc      (501) staff       (20)      625 2023-06-13 07:23:03.000000 permit-2.0.5/permit/utils/deprecation.py
+-rw-r--r--   0 asafc      (501) staff       (20)      444 2022-10-01 21:14:31.000000 permit-2.0.5/permit/utils/dicts.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1130 2023-06-13 07:23:03.000000 permit-2.0.5/permit/utils/sync.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-06-13 07:23:11.558717 permit-2.0.5/permit.egg-info/
+-rw-r--r--   0 asafc      (501) staff       (20)      478 2023-06-13 07:23:11.000000 permit-2.0.5/permit.egg-info/PKG-INFO
+-rw-r--r--   0 asafc      (501) staff       (20)     1170 2023-06-13 07:23:11.000000 permit-2.0.5/permit.egg-info/SOURCES.txt
+-rw-r--r--   0 asafc      (501) staff       (20)        1 2023-06-13 07:23:11.000000 permit-2.0.5/permit.egg-info/dependency_links.txt
+-rw-r--r--   0 asafc      (501) staff       (20)      107 2023-06-13 07:23:11.000000 permit-2.0.5/permit.egg-info/requires.txt
+-rw-r--r--   0 asafc      (501) staff       (20)       13 2023-06-13 07:23:11.000000 permit-2.0.5/permit.egg-info/top_level.txt
+-rw-r--r--   0 asafc      (501) staff       (20)      107 2023-05-22 06:43:35.000000 permit-2.0.5/requirements.txt
+-rw-r--r--   0 asafc      (501) staff       (20)       38 2023-06-13 07:23:11.562388 permit-2.0.5/setup.cfg
+-rw-r--r--   0 asafc      (501) staff       (20)      793 2023-06-13 07:23:03.000000 permit-2.0.5/setup.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-06-13 07:23:11.562077 permit-2.0.5/tests/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:14:31.000000 permit-2.0.5/tests/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1191 2023-05-22 11:43:03.000000 permit-2.0.5/tests/conftest.py
+-rw-r--r--   0 asafc      (501) staff       (20)     9506 2023-06-13 07:23:03.000000 permit-2.0.5/tests/test_abac_e2e.py
+-rw-r--r--   0 asafc      (501) staff       (20)     8890 2023-06-11 08:57:33.000000 permit-2.0.5/tests/test_rbac_e2e.py
+-rw-r--r--   0 asafc      (501) staff       (20)     8811 2023-06-12 11:54:30.000000 permit-2.0.5/tests/test_rbac_e2e_sync.py
+-rw-r--r--   0 asafc      (501) staff       (20)      323 2023-05-22 06:43:35.000000 permit-2.0.5/tests/utils.py
```

### Comparing `permit-2.0.4/LICENSE` & `permit-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `permit-2.0.4/permit/api/api_client.py` & `permit-2.0.5/permit/api/api_client.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.4/permit/api/base.py` & `permit-2.0.5/permit/api/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,60 +1,72 @@
 import functools
-from typing import Optional, Type, TypeVar, Union
+from typing import Callable, Optional, Type, TypeVar, Union
 
 import aiohttp
 from loguru import logger
 from pydantic import BaseModel, Extra, Field, parse_obj_as
 
 from ..config import PermitConfig
 from ..exceptions import PermitContextError, handle_api_error, handle_client_error
-from .context import API_ACCESS_LEVELS, ApiKeyLevel
+from .context import API_ACCESS_LEVELS, ApiContextLevel, ApiKeyAccessLevel
 from .models import APIKeyScopeRead
 
+T = TypeVar("T", bound=Callable)
+TModel = TypeVar("TModel", bound=BaseModel)
+TData = TypeVar("TData", bound=BaseModel)
 
-class ClientConfig(BaseModel):
-    class Config:
-        extra = Extra.allow
 
-    base_url: str = Field(
-        ...,
-        description="base url that will prefix the url fragment sent via the client",
-    )
-    headers: dict = Field(..., description="http headers sent to the API server")
+def required_permissions(access_level: ApiKeyAccessLevel):
+    def decorator(func: T) -> T:
+        @functools.wraps(func)
+        async def wrapped(self: BasePermitApi, *args, **kwargs):
+            await self._ensure_access_level(access_level)
+            return await func(self, *args, **kwargs)
+
+        return wrapped
+
+    return decorator
 
 
-def ensure_context(call_level: ApiKeyLevel):
+def required_context(context: ApiContextLevel):
     """
     a decorator that ensures that an API endpoint is called only after the SDK has initialized
     an API context (authorization level) by inferring it from the API key or manually by the user.
 
     Args:
         call_level: The required API key level for the endpoint.
 
     Raises:
         PermitContextError: If the API context does not match the required endpoint context.
     """
 
-    def decorator(func):
+    def decorator(func: T) -> T:
         @functools.wraps(func)
         async def wrapped(self: BasePermitApi, *args, **kwargs):
-            await self.ensure_context(call_level)
+            await self._ensure_context(context)
             return await func(self, *args, **kwargs)
 
         return wrapped
 
     return decorator
 
 
 def pagination_params(page: int, per_page: int) -> dict:
     return {"page": page, "per_page": per_page}
 
 
-TModel = TypeVar("TModel", bound=BaseModel)
-TData = TypeVar("TData", bound=BaseModel)
+class ClientConfig(BaseModel):
+    class Config:
+        extra = Extra.allow
+
+    base_url: str = Field(
+        ...,
+        description="base url that will prefix the url fragment sent via the client",
+    )
+    headers: dict = Field(..., description="http headers sent to the API server")
 
 
 class SimpleHttpClient:
     """
     wraps aiohttp client to reduce boilerplace
     """
 
@@ -202,80 +214,114 @@
         return SimpleHttpClient(
             client_config,
             base_url=endpoint_url,
         )
 
     async def _set_context_from_api_key(self) -> None:
         """
-        Set the API context based on the API key scope.
+        Set the API context and permitted access level based on the API key scope.
         """
+        logger.debug("Fetching api key scope")
         scope = await self.__api_keys.get("/scope", model=APIKeyScopeRead)
 
         if scope.organization_id is not None:
+            # saves the permitted access level by that api key
+            self.config.api_context._save_api_key_accessible_scope(
+                org=str(scope.organization_id),
+                project=(
+                    str(scope.project_id) if scope.project_id is not None else None
+                ),
+                environment=(
+                    str(scope.environment_id)
+                    if scope.environment_id is not None
+                    else None
+                ),
+            )
+
             if scope.project_id is not None:
                 if scope.environment_id is not None:
                     # Set environment level context
                     self.config.api_context.set_environment_level_context(
-                        scope.organization_id, scope.project_id, scope.environment_id
+                        str(scope.organization_id),
+                        str(scope.project_id),
+                        str(scope.environment_id),
                     )
                     return
 
                 # Set project level context
                 self.config.api_context.set_project_level_context(
-                    scope.organization_id, scope.project_id
+                    str(scope.organization_id), str(scope.project_id)
                 )
                 return
 
             # Set org level context
             self.config.api_context.set_organization_level_context(
-                scope.organization_id
+                str(scope.organization_id)
             )
             return
 
         raise PermitContextError("Could not set API context level")
 
-    async def ensure_context(self, call_level: ApiKeyLevel) -> None:
+    async def _ensure_access_level(
+        self, required_access_level: ApiKeyAccessLevel
+    ) -> None:
         """
-        Ensure that the API context matches the required endpoint context.
+        Ensure that the API Key has the necessary permissions to successfully call the API endpoint.
+
+        Note that this check is not full proof, and the API may still throw 401.
 
         Args:
-            call_level: The required API key level for the endpoint.
+            required_access_level: The required API Key Access level for the endpoint.
 
         Raises:
-            PermitContextError: If the API context does not match the required endpoint context.
+            PermitContextError: If the currently set API key access level does not match the required access level.
         """
-        if self.config.api_context.level == ApiKeyLevel.WAIT_FOR_INIT:
+        # should only happen once in the lifetime of the sdk
+        if (
+            self.config.api_context.level == ApiContextLevel.WAIT_FOR_INIT
+            or self.config.api_context.permitted_access_level
+            == ApiKeyAccessLevel.WAIT_FOR_INIT
+        ):
             await self._set_context_from_api_key()
 
-        if call_level != self.config.api_context.level:
-            if API_ACCESS_LEVELS.index(call_level) < API_ACCESS_LEVELS.index(
-                self.config.api_context.level
+        if required_access_level != self.config.api_context.permitted_access_level:
+            if API_ACCESS_LEVELS.index(required_access_level) < API_ACCESS_LEVELS.index(
+                self.config.api_context.permitted_access_level
             ):
                 raise PermitContextError(
-                    f"You're trying to use an SDK method that requires an API Key with level: {call_level}, "
-                    + f"however the SDK is running with an API key with level {self.config.api_context.level}."
+                    f"You're trying to use an SDK method that requires an API Key with access level: {required_access_level}, "
+                    + f"however the SDK is running with an API key with level {self.config.api_context.permitted_access_level}."
                 )
             return
 
         if (
-            call_level == ApiKeyLevel.PROJECT_LEVEL_API_KEY
-            and self.config.api_context.project is None
+            self.config.api_context.permitted_access_level.value
+            < required_access_level.value
         ):
             raise PermitContextError(
-                "You're trying to use an SDK method that's specific to a project, "
-                + "but you haven't set the current project in your client's context yet, "
-                + "or you are using an organization level API key. "
-                + "Please set the context to a specific "
-                + "project using `permit.set_context()` method."
+                f"You're trying to use an SDK method that requires an api context of {required_context.name}, "
+                + f"however the SDK is running in a less specific context level: {self.config.api_context.level}."
             )
 
-        if call_level == ApiKeyLevel.ENVIRONMENT_LEVEL_API_KEY and (
-            self.config.api_context.project is None
-            or self.config.api_context.environment is None
+    async def _ensure_context(self, required_context: ApiContextLevel) -> None:
+        """
+        Ensure that the API context matches the required endpoint context.
+
+        Args:
+            context: The required API context level for the endpoint.
+
+        Raises:
+            PermitContextError: If the currently set API context level does not match the required context level.
+        """
+        # should only happen once in the lifetime of the sdk
+        if (
+            self.config.api_context.level == ApiContextLevel.WAIT_FOR_INIT
+            or self.config.api_context.permitted_access_level
+            == ApiKeyAccessLevel.WAIT_FOR_INIT
         ):
+            await self._set_context_from_api_key()
+
+        if self.config.api_context.level.value < required_context.value:
             raise PermitContextError(
-                "You're trying to use an SDK method that's specific to an environment, "
-                + "but you haven't set the current environment in your client's context yet, "
-                + "or you are using an organization/project level API key. "
-                + "Please set the context to a specific "
-                + "environment using `permit.set_context()` method."
+                f"You're trying to use an SDK method that requires an api context of {required_context.name}, "
+                + f"however the SDK is running in a less specific context level: {self.config.api_context.level}."
             )
```

### Comparing `permit-2.0.4/permit/api/condition_set_rules.py` & `permit-2.0.5/permit/api/condition_set_rules.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,34 @@
 from typing import List, Optional
 
 from pydantic import validate_arguments
 
-from .base import BasePermitApi, SimpleHttpClient, ensure_context, pagination_params
-from .context import ApiKeyLevel
+from .base import (
+    BasePermitApi,
+    SimpleHttpClient,
+    pagination_params,
+    required_context,
+    required_permissions,
+)
+from .context import ApiContextLevel, ApiKeyAccessLevel
 from .models import ConditionSetRuleCreate, ConditionSetRuleRead, ConditionSetRuleRemove
 
 
 class ConditionSetRulesApi(BasePermitApi):
     @property
     def __condition_set_rules(self) -> SimpleHttpClient:
         return self._build_http_client(
             "/v2/facts/{proj_id}/{env_id}/set_rules".format(
                 proj_id=self.config.api_context.project,
                 env_id=self.config.api_context.environment,
             )
         )
 
-    @ensure_context(ApiKeyLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_context(ApiContextLevel.ENVIRONMENT)
     @validate_arguments
     async def list(
         self,
         user_set_key: Optional[str] = None,
         permission_key: Optional[str] = None,
         resource_set_key: Optional[str] = None,
         page: int = 1,
@@ -54,15 +61,16 @@
             params.update(dict(resource_set=resource_set_key))
         return await self.__condition_set_rules.get(
             "",
             model=List[ConditionSetRuleRead],
             params=params,
         )
 
-    @ensure_context(ApiKeyLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_context(ApiContextLevel.ENVIRONMENT)
     @validate_arguments
     async def create(self, rule: ConditionSetRuleCreate) -> List[ConditionSetRuleRead]:
         """
         Creates a new condition set rule.
 
         Args:
             rule: The condition set rule to create.
@@ -74,15 +82,16 @@
             PermitApiError: If the API returns an error HTTP status code.
             PermitContextError: If the configured ApiContext does not match the required endpoint context.
         """
         return await self.__condition_set_rules.post(
             "", model=List[ConditionSetRuleRead], json=rule
         )
 
-    @ensure_context(ApiKeyLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_context(ApiContextLevel.ENVIRONMENT)
     @validate_arguments
     async def delete(self, rule: ConditionSetRuleRemove) -> None:
         """
         Deletes a condition set rule.
 
         Args:
             rule: The condition set rule to delete.
```

### Comparing `permit-2.0.4/permit/api/condition_sets.py` & `permit-2.0.5/permit/api/condition_sets.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,34 @@
 from typing import List
 
 from pydantic import validate_arguments
 
-from .base import BasePermitApi, SimpleHttpClient, ensure_context, pagination_params
-from .context import ApiKeyLevel
+from .base import (
+    BasePermitApi,
+    SimpleHttpClient,
+    pagination_params,
+    required_context,
+    required_permissions,
+)
+from .context import ApiContextLevel, ApiKeyAccessLevel
 from .models import ConditionSetCreate, ConditionSetRead, ConditionSetUpdate
 
 
 class ConditionSetsApi(BasePermitApi):
     @property
     def __condition_sets(self) -> SimpleHttpClient:
         return self._build_http_client(
             "/v2/schema/{proj_id}/{env_id}/condition_sets".format(
                 proj_id=self.config.api_context.project,
                 env_id=self.config.api_context.environment,
             )
         )
 
-    @ensure_context(ApiKeyLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_context(ApiContextLevel.ENVIRONMENT)
     @validate_arguments
     async def list(self, page: int = 1, per_page: int = 100) -> List[ConditionSetRead]:
         """
         Retrieves a list of condition sets.
 
         Args:
             page: The page number to fetch (default: 1).
@@ -34,15 +41,21 @@
             PermitApiError: If the API returns an error HTTP status code.
             PermitContextError: If the configured ApiContext does not match the required endpoint context.
         """
         return await self.__condition_sets.get(
             "", model=List[ConditionSetRead], params=pagination_params(page, per_page)
         )
 
-    @ensure_context(ApiKeyLevel.ENVIRONMENT_LEVEL_API_KEY)
+    async def _get(self, condition_set_key: str) -> ConditionSetRead:
+        return await self.__condition_sets.get(
+            f"/{condition_set_key}", model=ConditionSetRead
+        )
+
+    @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_context(ApiContextLevel.ENVIRONMENT)
     @validate_arguments
     async def get(self, condition_set_key: str) -> ConditionSetRead:
         """
         Retrieves a condition set by its key.
 
         Args:
             condition_set_key: The key of the condition set.
@@ -50,19 +63,18 @@
         Returns:
             the condition set.
 
         Raises:
             PermitApiError: If the API returns an error HTTP status code.
             PermitContextError: If the configured ApiContext does not match the required endpoint context.
         """
-        return await self.__condition_sets.get(
-            f"/{condition_set_key}", model=ConditionSetRead
-        )
+        return await self._get(condition_set_key)
 
-    @ensure_context(ApiKeyLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_context(ApiContextLevel.ENVIRONMENT)
     @validate_arguments
     async def get_by_key(self, condition_set_key: str) -> ConditionSetRead:
         """
         Retrieves a condition set by its key.
         Alias for the get method.
 
         Args:
@@ -71,17 +83,18 @@
         Returns:
             the condition set.
 
         Raises:
             PermitApiError: If the API returns an error HTTP status code.
             PermitContextError: If the configured ApiContext does not match the required endpoint context.
         """
-        return await self.get(condition_set_key)
+        return await self._get(condition_set_key)
 
-    @ensure_context(ApiKeyLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_context(ApiContextLevel.ENVIRONMENT)
     @validate_arguments
     async def get_by_id(self, condition_set_id: str) -> ConditionSetRead:
         """
         Retrieves a condition set by its ID.
         Alias for the get method.
 
         Args:
@@ -90,17 +103,18 @@
         Returns:
             the condition set.
 
         Raises:
             PermitApiError: If the API returns an error HTTP status code.
             PermitContextError: If the configured ApiContext does not match the required endpoint context.
         """
-        return await self.get(condition_set_id)
+        return await self._get(condition_set_id)
 
-    @ensure_context(ApiKeyLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_context(ApiContextLevel.ENVIRONMENT)
     @validate_arguments
     async def create(self, condition_set_data: ConditionSetCreate) -> ConditionSetRead:
         """
         Creates a new condition set.
 
         Args:
             condition_set_data: The data for the new condition set.
@@ -112,15 +126,16 @@
             PermitApiError: If the API returns an error HTTP status code.
             PermitContextError: If the configured ApiContext does not match the required endpoint context.
         """
         return await self.__condition_sets.post(
             "", model=ConditionSetRead, json=condition_set_data
         )
 
-    @ensure_context(ApiKeyLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_context(ApiContextLevel.ENVIRONMENT)
     @validate_arguments
     async def update(
         self, condition_set_key: str, condition_set_data: ConditionSetUpdate
     ) -> ConditionSetRead:
         """
         Updates a condition set.
 
@@ -137,15 +152,16 @@
         """
         return await self.__condition_sets.patch(
             f"/{condition_set_key}",
             model=ConditionSetRead,
             json=condition_set_data,
         )
 
-    @ensure_context(ApiKeyLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_context(ApiContextLevel.ENVIRONMENT)
     @validate_arguments
     async def delete(self, condition_set_key: str) -> None:
         """
         Deletes a condition set.
 
         Args:
             condition_set_key: The key of the condition set to delete.
```

### Comparing `permit-2.0.4/permit/api/deprecated.py` & `permit-2.0.5/permit/api/deprecated.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-import functools
 from typing import List, Optional, Union
 from uuid import UUID
-from warnings import warn
 
 from ..config import PermitConfig
+from ..utils.deprecation import deprecated
 from .base import BasePermitApi
 from .elements import ElementsApi
 from .models import (
     EmbeddedLoginRequestOutput,
     ResourceCreate,
     ResourceRead,
     ResourceUpdate,
@@ -26,26 +25,14 @@
 from .resources import ResourcesApi
 from .role_assignments import RoleAssignmentsApi
 from .roles import RolesApi
 from .tenants import TenantsApi
 from .users import UsersApi
 
 
-def deprecated(message: str):
-    def decorator(func):
-        @functools.wraps(func)
-        async def wrapped(self: BasePermitApi, *args, **kwargs):
-            warn(message, DeprecationWarning, stacklevel=2)
-            return await func(self, *args, **kwargs)
-
-        return wrapped
-
-    return decorator
-
-
 class DeprecatedApi(BasePermitApi):
     """
     Represents the interface for managing roles.
     """
 
     def __init__(self, config: PermitConfig):
         super().__init__(config)
```

### Comparing `permit-2.0.4/permit/api/elements.py` & `permit-2.0.5/permit/api/elements.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.4/permit/api/environments.py` & `permit-2.0.5/permit/api/environments.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 from typing import List
 
 from pydantic import validate_arguments
 
 from ..config import PermitConfig
-from .base import BasePermitApi, ensure_context, pagination_params
-from .context import ApiKeyLevel
+from .base import (
+    BasePermitApi,
+    pagination_params,
+    required_context,
+    required_permissions,
+)
+from .context import ApiContextLevel, ApiKeyAccessLevel
 from .models import (
     APIKeyRead,
     EnvironmentCopy,
     EnvironmentCreate,
     EnvironmentRead,
     EnvironmentStats,
     EnvironmentUpdate,
@@ -16,15 +21,16 @@
 
 
 class EnvironmentsApi(BasePermitApi):
     def __init__(self, config: PermitConfig):
         super().__init__(config)
         self.__environments = self._build_http_client("")
 
-    @ensure_context(ApiKeyLevel.PROJECT_LEVEL_API_KEY)
+    @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_context(ApiContextLevel.ORGANIZATION)
     @validate_arguments
     async def list(
         self, project_key: str, page: int = 1, per_page: int = 100
     ) -> List[EnvironmentRead]:
         """
         Retrieves a list of environments.
 
@@ -40,15 +46,21 @@
         """
         return await self.__environments.get(
             f"/v2/projects/{project_key}/envs",
             model=List[EnvironmentRead],
             params=pagination_params(page, per_page),
         )
 
-    @ensure_context(ApiKeyLevel.PROJECT_LEVEL_API_KEY)
+    async def _get(self, project_key: str, environment_key: str) -> EnvironmentRead:
+        return await self.__environments.get(
+            f"/v2/projects/{project_key}/envs/{environment_key}", model=EnvironmentRead
+        )
+
+    @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_context(ApiContextLevel.ORGANIZATION)
     @validate_arguments
     async def get(self, project_key: str, environment_key: str) -> EnvironmentRead:
         """
         Gets an environment by project key and environment key.
 
         Args:
             project_key: The project key.
@@ -57,19 +69,18 @@
         Returns:
             an EnvironmentRead object representing the retrieved environment.
 
         Raises:
             PermitApiError: If the API returns an error HTTP status code.
             PermitContextError: If the configured ApiContext does not match the required endpoint context.
         """
-        return await self.__environments.get(
-            f"/v2/projects/{project_key}/envs/{environment_key}", model=EnvironmentRead
-        )
+        return await self._get(project_key, environment_key)
 
-    @ensure_context(ApiKeyLevel.PROJECT_LEVEL_API_KEY)
+    @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_context(ApiContextLevel.ORGANIZATION)
     @validate_arguments
     async def get_by_key(
         self, project_key: str, environment_key: str
     ) -> EnvironmentRead:
         """
         Gets an environment by project key and environment key.
         Alias for the get method.
@@ -81,17 +92,18 @@
         Returns:
             an EnvironmentRead object representing the retrieved environment.
 
         Raises:
             PermitApiError: If the API returns an error HTTP status code.
             PermitContextError: If the configured ApiContext does not match the required endpoint context.
         """
-        return await self.get(project_key, environment_key)
+        return await self._get(project_key, environment_key)
 
-    @ensure_context(ApiKeyLevel.PROJECT_LEVEL_API_KEY)
+    @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_context(ApiContextLevel.ORGANIZATION)
     @validate_arguments
     async def get_by_id(self, project_id: str, environment_id: str) -> EnvironmentRead:
         """
         Gets an environment by project ID and environment ID.
         Alias for the get method.
 
         Args:
@@ -101,17 +113,18 @@
         Returns:
             an EnvironmentRead object representing the retrieved environment.
 
         Raises:
             PermitApiError: If the API returns an error HTTP status code.
             PermitContextError: If the configured ApiContext does not match the required endpoint context.
         """
-        return await self.get(project_id, environment_id)
+        return await self._get(project_id, environment_id)
 
-    @ensure_context(ApiKeyLevel.PROJECT_LEVEL_API_KEY)
+    @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_context(ApiContextLevel.ORGANIZATION)
     @validate_arguments
     async def get_stats(
         self, project_key: str, environment_key: str
     ) -> EnvironmentStats:
         """
         Retrieves statistics and metadata for an environment.
 
@@ -127,15 +140,16 @@
             PermitContextError: If the configured ApiContext does not match the required endpoint context.
         """
         return await self.__environments.get(
             f"/v2/projects/{project_key}/envs/{environment_key}/stats",
             model=EnvironmentStats,
         )
 
-    @ensure_context(ApiKeyLevel.PROJECT_LEVEL_API_KEY)
+    @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_context(ApiContextLevel.ORGANIZATION)
     @validate_arguments
     async def get_api_key(self, project_key: str, environment_key: str) -> APIKeyRead:
         """
         Retrieves the API key that grants access for an environment.
 
         Args:
             project_key: The project key.
@@ -149,15 +163,16 @@
             PermitContextError: If the configured ApiContext does not match the required endpoint context.
         """
         return await self.__environments.get(
             f"/v2/api-key/{project_key}/{environment_key}",
             model=APIKeyRead,
         )
 
-    @ensure_context(ApiKeyLevel.PROJECT_LEVEL_API_KEY)
+    @required_permissions(ApiKeyAccessLevel.PROJECT_LEVEL_API_KEY)
+    @required_context(ApiContextLevel.ORGANIZATION)
     @validate_arguments
     async def create(
         self, project_key: str, environment_data: EnvironmentCreate
     ) -> EnvironmentRead:
         """
         Creates a new environment.
 
@@ -174,15 +189,16 @@
         """
         return await self.__environments.post(
             f"/v2/projects/{project_key}/envs",
             model=EnvironmentRead,
             json=environment_data,
         )
 
-    @ensure_context(ApiKeyLevel.PROJECT_LEVEL_API_KEY)
+    @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_context(ApiContextLevel.ORGANIZATION)
     @validate_arguments
     async def update(
         self,
         project_key: str,
         environment_key: str,
         environment_data: EnvironmentUpdate,
     ) -> EnvironmentRead:
@@ -203,15 +219,16 @@
         """
         return await self.__environments.patch(
             f"/v2/projects/{project_key}/envs/{environment_key}",
             model=EnvironmentRead,
             json=environment_data,
         )
 
-    @ensure_context(ApiKeyLevel.PROJECT_LEVEL_API_KEY)
+    @required_permissions(ApiKeyAccessLevel.PROJECT_LEVEL_API_KEY)
+    @required_context(ApiContextLevel.ORGANIZATION)
     @validate_arguments
     async def copy(
         self, project_key: str, environment_key: str, copy_params: EnvironmentCopy
     ) -> EnvironmentRead:
         """
         Clones data from a source specified environment into a different target environment in the same project.
 
@@ -229,15 +246,16 @@
         """
         return await self.__environments.post(
             f"/v2/projects/{project_key}/envs/{environment_key}/copy",
             model=EnvironmentRead,
             json=copy_params,
         )
 
-    @ensure_context(ApiKeyLevel.PROJECT_LEVEL_API_KEY)
+    @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_context(ApiContextLevel.ORGANIZATION)
     @validate_arguments
     async def delete(self, project_key: str, environment_key: str) -> None:
         """
         Deletes an environment.
 
         Args:
             project_key: The project key.
```

### Comparing `permit-2.0.4/permit/api/models.py` & `permit-2.0.5/permit/api/models.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.4/permit/api/resource_action_groups.py` & `permit-2.0.5/permit/api/resource_action_groups.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,34 @@
 from typing import List
 
 from pydantic import validate_arguments
 
-from .base import BasePermitApi, SimpleHttpClient, ensure_context, pagination_params
-from .context import ApiKeyLevel
+from .base import (
+    BasePermitApi,
+    SimpleHttpClient,
+    pagination_params,
+    required_context,
+    required_permissions,
+)
+from .context import ApiContextLevel, ApiKeyAccessLevel
 from .models import ResourceActionGroupCreate, ResourceActionGroupRead
 
 
 class ResourceActionGroupsApi(BasePermitApi):
     @property
     def __action_groups(self) -> SimpleHttpClient:
         return self._build_http_client(
             "/v2/schema/{proj_id}/{env_id}/resources".format(
                 proj_id=self.config.api_context.project,
                 env_id=self.config.api_context.environment,
             )
         )
 
-    @ensure_context(ApiKeyLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_context(ApiContextLevel.ENVIRONMENT)
     @validate_arguments
     async def list(
         self, resource_key: str, page: int = 1, per_page: int = 100
     ) -> List[ResourceActionGroupRead]:
         """
         Retrieves a list of action groups.
 
@@ -39,15 +46,22 @@
         """
         return await self.__action_groups.get(
             f"/{resource_key}/action_groups",
             model=List[ResourceActionGroupRead],
             params=pagination_params(page, per_page),
         )
 
-    @ensure_context(ApiKeyLevel.ENVIRONMENT_LEVEL_API_KEY)
+    async def _get(self, resource_key: str, group_key: str) -> ResourceActionGroupRead:
+        return await self.__action_groups.get(
+            f"/{resource_key}/action_groups/{group_key}",
+            model=ResourceActionGroupRead,
+        )
+
+    @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_context(ApiContextLevel.ENVIRONMENT)
     @validate_arguments
     async def get(self, resource_key: str, group_key: str) -> ResourceActionGroupRead:
         """
         Retrieves a action group by its key.
 
         Args:
             resource_key: The key of the resource the action group belongs to.
@@ -56,20 +70,18 @@
         Returns:
             the action group.
 
         Raises:
             PermitApiError: If the API returns an error HTTP status code.
             PermitContextError: If the configured ApiContext does not match the required endpoint context.
         """
-        return await self.__action_groups.get(
-            f"/{resource_key}/action_groups/{group_key}",
-            model=ResourceActionGroupRead,
-        )
+        return await self._get(resource_key, group_key)
 
-    @ensure_context(ApiKeyLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_context(ApiContextLevel.ENVIRONMENT)
     @validate_arguments
     async def get_by_key(
         self, resource_key: str, group_key: str
     ) -> ResourceActionGroupRead:
         """
         Retrieves a action group by its key.
         Alias for the get method.
@@ -81,17 +93,18 @@
         Returns:
             the action group.
 
         Raises:
             PermitApiError: If the API returns an error HTTP status code.
             PermitContextError: If the configured ApiContext does not match the required endpoint context.
         """
-        return await self.get(resource_key, group_key)
+        return await self._get(resource_key, group_key)
 
-    @ensure_context(ApiKeyLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_context(ApiContextLevel.ENVIRONMENT)
     @validate_arguments
     async def get_by_id(
         self, resource_id: str, group_id: str
     ) -> ResourceActionGroupRead:
         """
         Retrieves a action group by its ID.
         Alias for the get method.
@@ -103,17 +116,18 @@
         Returns:
             the action group.
 
         Raises:
             PermitApiError: If the API returns an error HTTP status code.
             PermitContextError: If the configured ApiContext does not match the required endpoint context.
         """
-        return await self.get(resource_id, group_id)
+        return await self._get(resource_id, group_id)
 
-    @ensure_context(ApiKeyLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_context(ApiContextLevel.ENVIRONMENT)
     @validate_arguments
     async def create(
         self, resource_key: str, group_data: ResourceActionGroupCreate
     ) -> ResourceActionGroupRead:
         """
         Creates a new action group.
 
@@ -130,15 +144,16 @@
         """
         return await self.__action_groups.post(
             f"/{resource_key}/action_groups",
             model=ResourceActionGroupRead,
             json=group_data,
         )
 
-    @ensure_context(ApiKeyLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_context(ApiContextLevel.ENVIRONMENT)
     @validate_arguments
     async def delete(self, resource_key: str, group_key: str) -> None:
         """
         Deletes a action group.
 
         Args:
             resource_key: The key of the resource the action group belongs to.
```

### Comparing `permit-2.0.4/permit/api/resource_actions.py` & `permit-2.0.5/permit/api/resource_actions.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,34 @@
 from typing import List
 
 from pydantic import validate_arguments
 
-from .base import BasePermitApi, SimpleHttpClient, ensure_context, pagination_params
-from .context import ApiKeyLevel
+from .base import (
+    BasePermitApi,
+    SimpleHttpClient,
+    pagination_params,
+    required_context,
+    required_permissions,
+)
+from .context import ApiContextLevel, ApiKeyAccessLevel
 from .models import ResourceActionCreate, ResourceActionRead, ResourceActionUpdate
 
 
 class ResourceActionsApi(BasePermitApi):
     @property
     def __actions(self) -> SimpleHttpClient:
         return self._build_http_client(
             "/v2/schema/{proj_id}/{env_id}/resources".format(
                 proj_id=self.config.api_context.project,
                 env_id=self.config.api_context.environment,
             )
         )
 
-    @ensure_context(ApiKeyLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_context(ApiContextLevel.ENVIRONMENT)
     @validate_arguments
     async def list(
         self, resource_key: str, page: int = 1, per_page: int = 100
     ) -> List[ResourceActionRead]:
         """
         Retrieves a list of actions.
 
@@ -39,15 +46,21 @@
         """
         return await self.__actions.get(
             f"/{resource_key}/actions",
             model=List[ResourceActionRead],
             params=pagination_params(page, per_page),
         )
 
-    @ensure_context(ApiKeyLevel.ENVIRONMENT_LEVEL_API_KEY)
+    async def _get(self, resource_key: str, action_key: str) -> ResourceActionRead:
+        return await self.__actions.get(
+            f"/{resource_key}/actions/{action_key}", model=ResourceActionRead
+        )
+
+    @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_context(ApiContextLevel.ENVIRONMENT)
     @validate_arguments
     async def get(self, resource_key: str, action_key: str) -> ResourceActionRead:
         """
         Retrieves a action by its key.
 
         Args:
             resource_key: The key of the resource the action belongs to.
@@ -56,19 +69,18 @@
         Returns:
             the action.
 
         Raises:
             PermitApiError: If the API returns an error HTTP status code.
             PermitContextError: If the configured ApiContext does not match the required endpoint context.
         """
-        return await self.__actions.get(
-            f"/{resource_key}/actions/{action_key}", model=ResourceActionRead
-        )
+        return await self._get(resource_key, action_key)
 
-    @ensure_context(ApiKeyLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_context(ApiContextLevel.ENVIRONMENT)
     @validate_arguments
     async def get_by_key(
         self, resource_key: str, action_key: str
     ) -> ResourceActionRead:
         """
         Retrieves a action by its key.
         Alias for the get method.
@@ -80,17 +92,18 @@
         Returns:
             the action.
 
         Raises:
             PermitApiError: If the API returns an error HTTP status code.
             PermitContextError: If the configured ApiContext does not match the required endpoint context.
         """
-        return await self.get(resource_key, action_key)
+        return await self._get(resource_key, action_key)
 
-    @ensure_context(ApiKeyLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_context(ApiContextLevel.ENVIRONMENT)
     @validate_arguments
     async def get_by_id(self, resource_id: str, action_id: str) -> ResourceActionRead:
         """
         Retrieves a action by its ID.
         Alias for the get method.
 
         Args:
@@ -100,17 +113,18 @@
         Returns:
             the action.
 
         Raises:
             PermitApiError: If the API returns an error HTTP status code.
             PermitContextError: If the configured ApiContext does not match the required endpoint context.
         """
-        return await self.get(resource_id, action_id)
+        return await self._get(resource_id, action_id)
 
-    @ensure_context(ApiKeyLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_context(ApiContextLevel.ENVIRONMENT)
     @validate_arguments
     async def create(
         self, resource_key: str, action_data: ResourceActionCreate
     ) -> ResourceActionRead:
         """
         Creates a new action.
 
@@ -127,15 +141,16 @@
         """
         return await self.__actions.post(
             f"/{resource_key}/actions",
             model=ResourceActionRead,
             json=action_data,
         )
 
-    @ensure_context(ApiKeyLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_context(ApiContextLevel.ENVIRONMENT)
     @validate_arguments
     async def update(
         self, resource_key: str, action_key: str, action_data: ResourceActionUpdate
     ) -> ResourceActionRead:
         """
         Updates a action.
 
@@ -153,15 +168,16 @@
         """
         return await self.__actions.patch(
             f"/{resource_key}/actions/{action_key}",
             model=ResourceActionRead,
             json=action_data,
         )
 
-    @ensure_context(ApiKeyLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_context(ApiContextLevel.ENVIRONMENT)
     @validate_arguments
     async def delete(self, resource_key: str, action_key: str) -> None:
         """
         Deletes a action.
 
         Args:
             resource_key: The key of the resource the action belongs to.
```

### Comparing `permit-2.0.4/permit/api/resource_attributes.py` & `permit-2.0.5/permit/api/resource_attributes.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 from typing import List
 
 from pydantic import validate_arguments
 
-from .base import BasePermitApi, SimpleHttpClient, ensure_context, pagination_params
-from .context import ApiKeyLevel
+from .base import (
+    BasePermitApi,
+    SimpleHttpClient,
+    pagination_params,
+    required_context,
+    required_permissions,
+)
+from .context import ApiContextLevel, ApiKeyAccessLevel
 from .models import (
     ResourceAttributeCreate,
     ResourceAttributeRead,
     ResourceAttributeUpdate,
 )
 
 
@@ -17,15 +23,16 @@
         return self._build_http_client(
             "/v2/schema/{proj_id}/{env_id}/resources".format(
                 proj_id=self.config.api_context.project,
                 env_id=self.config.api_context.environment,
             )
         )
 
-    @ensure_context(ApiKeyLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_context(ApiContextLevel.ENVIRONMENT)
     @validate_arguments
     async def list(
         self, resource_key: str, page: int = 1, per_page: int = 100
     ) -> List[ResourceAttributeRead]:
         """
         Retrieves a list of attributes.
 
@@ -43,15 +50,23 @@
         """
         return await self.__attributes.get(
             f"/{resource_key}/attributes",
             model=List[ResourceAttributeRead],
             params=pagination_params(page, per_page),
         )
 
-    @ensure_context(ApiKeyLevel.ENVIRONMENT_LEVEL_API_KEY)
+    async def _get(
+        self, resource_key: str, attribute_key: str
+    ) -> ResourceAttributeRead:
+        return await self.__attributes.get(
+            f"/{resource_key}/attributes/{attribute_key}", model=ResourceAttributeRead
+        )
+
+    @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_context(ApiContextLevel.ENVIRONMENT)
     @validate_arguments
     async def get(self, resource_key: str, attribute_key: str) -> ResourceAttributeRead:
         """
         Retrieves a attribute by its key.
 
         Args:
             resource_key: The key of the resource the attribute belongs to.
@@ -60,19 +75,18 @@
         Returns:
             the attribute.
 
         Raises:
             PermitApiError: If the API returns an error HTTP status code.
             PermitContextError: If the configured ApiContext does not match the required endpoint context.
         """
-        return await self.__attributes.get(
-            f"/{resource_key}/attributes/{attribute_key}", model=ResourceAttributeRead
-        )
+        return await self._get(resource_key, attribute_key)
 
-    @ensure_context(ApiKeyLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_context(ApiContextLevel.ENVIRONMENT)
     @validate_arguments
     async def get_by_key(
         self, resource_key: str, attribute_key: str
     ) -> ResourceAttributeRead:
         """
         Retrieves a attribute by its key.
         Alias for the get method.
@@ -84,17 +98,18 @@
         Returns:
             the attribute.
 
         Raises:
             PermitApiError: If the API returns an error HTTP status code.
             PermitContextError: If the configured ApiContext does not match the required endpoint context.
         """
-        return await self.get(resource_key, attribute_key)
+        return await self._get(resource_key, attribute_key)
 
-    @ensure_context(ApiKeyLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_context(ApiContextLevel.ENVIRONMENT)
     @validate_arguments
     async def get_by_id(
         self, resource_id: str, attribute_id: str
     ) -> ResourceAttributeRead:
         """
         Retrieves a attribute by its ID.
         Alias for the get method.
@@ -106,17 +121,18 @@
         Returns:
             the attribute.
 
         Raises:
             PermitApiError: If the API returns an error HTTP status code.
             PermitContextError: If the configured ApiContext does not match the required endpoint context.
         """
-        return await self.get(resource_id, attribute_id)
+        return await self._get(resource_id, attribute_id)
 
-    @ensure_context(ApiKeyLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_context(ApiContextLevel.ENVIRONMENT)
     @validate_arguments
     async def create(
         self, resource_key: str, attribute_data: ResourceAttributeCreate
     ) -> ResourceAttributeRead:
         """
         Creates a new attribute.
 
@@ -133,15 +149,16 @@
         """
         return await self.__attributes.post(
             f"/{resource_key}/attributes",
             model=ResourceAttributeRead,
             json=attribute_data,
         )
 
-    @ensure_context(ApiKeyLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_context(ApiContextLevel.ENVIRONMENT)
     @validate_arguments
     async def update(
         self,
         resource_key: str,
         attribute_key: str,
         attribute_data: ResourceAttributeUpdate,
     ) -> ResourceAttributeRead:
@@ -162,15 +179,16 @@
         """
         return await self.__attributes.patch(
             f"/{resource_key}/attributes/{attribute_key}",
             model=ResourceAttributeRead,
             json=attribute_data,
         )
 
-    @ensure_context(ApiKeyLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_context(ApiContextLevel.ENVIRONMENT)
     @validate_arguments
     async def delete(self, resource_key: str, attribute_key: str) -> None:
         """
         Deletes a attribute.
 
         Args:
             resource_key: The key of the resource the attribute belongs to.
```

### Comparing `permit-2.0.4/permit/api/resources.py` & `permit-2.0.5/permit/api/resources.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,34 @@
 from typing import List
 
 from pydantic import validate_arguments
 
-from .base import BasePermitApi, SimpleHttpClient, ensure_context, pagination_params
-from .context import ApiKeyLevel
+from .base import (
+    BasePermitApi,
+    SimpleHttpClient,
+    pagination_params,
+    required_context,
+    required_permissions,
+)
+from .context import ApiContextLevel, ApiKeyAccessLevel
 from .models import ResourceCreate, ResourceRead, ResourceReplace, ResourceUpdate
 
 
 class ResourcesApi(BasePermitApi):
     @property
     def __resources(self) -> SimpleHttpClient:
         return self._build_http_client(
             "/v2/schema/{proj_id}/{env_id}/resources".format(
                 proj_id=self.config.api_context.project,
                 env_id=self.config.api_context.environment,
             )
         )
 
-    @ensure_context(ApiKeyLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_context(ApiContextLevel.ENVIRONMENT)
     @validate_arguments
     async def list(self, page: int = 1, per_page: int = 100) -> List[ResourceRead]:
         """
         Retrieves a list of resources.
 
         Args:
             page: The page number to fetch (default: 1).
@@ -36,15 +43,19 @@
         """
         return await self.__resources.get(
             "",
             model=List[ResourceRead],
             params=pagination_params(page, per_page),
         )
 
-    @ensure_context(ApiKeyLevel.ENVIRONMENT_LEVEL_API_KEY)
+    async def _get(self, resource_key: str) -> ResourceRead:
+        return await self.__resources.get(f"/{resource_key}", model=ResourceRead)
+
+    @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_context(ApiContextLevel.ENVIRONMENT)
     @validate_arguments
     async def get(self, resource_key: str) -> ResourceRead:
         """
         Retrieves a resource by its key.
 
         Args:
             resource_key: The key of the resource.
@@ -52,17 +63,18 @@
         Returns:
             the resource.
 
         Raises:
             PermitApiError: If the API returns an error HTTP status code.
             PermitContextError: If the configured ApiContext does not match the required endpoint context.
         """
-        return await self.__resources.get(f"/{resource_key}", model=ResourceRead)
+        return await self._get(resource_key)
 
-    @ensure_context(ApiKeyLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_context(ApiContextLevel.ENVIRONMENT)
     @validate_arguments
     async def get_by_key(self, resource_key: str) -> ResourceRead:
         """
         Retrieves a resource by its key.
         Alias for the get method.
 
         Args:
@@ -71,17 +83,18 @@
         Returns:
             the resource.
 
         Raises:
             PermitApiError: If the API returns an error HTTP status code.
             PermitContextError: If the configured ApiContext does not match the required endpoint context.
         """
-        return await self.get(resource_key)
+        return await self._get(resource_key)
 
-    @ensure_context(ApiKeyLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_context(ApiContextLevel.ENVIRONMENT)
     @validate_arguments
     async def get_by_id(self, resource_id: str) -> ResourceRead:
         """
         Retrieves a resource by its ID.
         Alias for the get method.
 
         Args:
@@ -90,17 +103,18 @@
         Returns:
             the resource.
 
         Raises:
             PermitApiError: If the API returns an error HTTP status code.
             PermitContextError: If the configured ApiContext does not match the required endpoint context.
         """
-        return await self.get(resource_id)
+        return await self._get(resource_id)
 
-    @ensure_context(ApiKeyLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_context(ApiContextLevel.ENVIRONMENT)
     @validate_arguments
     async def create(self, resource_data: ResourceCreate) -> ResourceRead:
         """
         Creates a new resource.
 
         Args:
             resource_data: The data for the new resource.
@@ -110,15 +124,16 @@
 
         Raises:
             PermitApiError: If the API returns an error HTTP status code.
             PermitContextError: If the configured ApiContext does not match the required endpoint context.
         """
         return await self.__resources.post("", model=ResourceRead, json=resource_data)
 
-    @ensure_context(ApiKeyLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_context(ApiContextLevel.ENVIRONMENT)
     @validate_arguments
     async def update(
         self, resource_key: str, resource_data: ResourceUpdate
     ) -> ResourceRead:
         """
         Updates a resource.
 
@@ -135,15 +150,16 @@
         """
         return await self.__resources.patch(
             f"/{resource_key}",
             model=ResourceRead,
             json=resource_data,
         )
 
-    @ensure_context(ApiKeyLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_context(ApiContextLevel.ENVIRONMENT)
     @validate_arguments
     async def replace(
         self, resource_key: str, resource_data: ResourceReplace
     ) -> ResourceRead:
         """
         Creates a resource if no such resource exists, otherwise completely replaces the resource in place.
 
@@ -160,15 +176,16 @@
         """
         return await self.__resources.put(
             f"/{resource_key}",
             model=ResourceRead,
             json=resource_data,
         )
 
-    @ensure_context(ApiKeyLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_context(ApiContextLevel.ENVIRONMENT)
     @validate_arguments
     async def delete(self, resource_key: str) -> None:
         """
         Deletes a resource.
 
         Args:
             resource_key: The key of the resource to delete.
```

### Comparing `permit-2.0.4/permit/api/role_assignments.py` & `permit-2.0.5/permit/api/role_assignments.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 from typing import List, Optional
 
 from pydantic import validate_arguments
 
 from ..config import PermitConfig
-from .base import BasePermitApi, SimpleHttpClient, ensure_context, pagination_params
-from .context import ApiKeyLevel
+from .base import (
+    BasePermitApi,
+    SimpleHttpClient,
+    pagination_params,
+    required_context,
+    required_permissions,
+)
+from .context import ApiContextLevel, ApiKeyAccessLevel
 from .models import (
     BulkRoleAssignmentReport,
     BulkRoleUnAssignmentReport,
     RoleAssignmentCreate,
     RoleAssignmentRead,
     RoleAssignmentRemove,
 )
@@ -20,15 +26,16 @@
         return self._build_http_client(
             "/v2/facts/{proj_id}/{env_id}/role_assignments".format(
                 proj_id=self.config.api_context.project,
                 env_id=self.config.api_context.environment,
             )
         )
 
-    @ensure_context(ApiKeyLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_context(ApiContextLevel.ENVIRONMENT)
     @validate_arguments
     async def list(
         self,
         user_key: Optional[str] = None,
         tenant_key: Optional[str] = None,
         role_key: Optional[str] = None,
         page: int = 1,
@@ -60,15 +67,16 @@
             params.update(dict(role=role_key))
         return await self.__role_assignments.get(
             "",
             model=List[RoleAssignmentRead],
             params=params,
         )
 
-    @ensure_context(ApiKeyLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_context(ApiContextLevel.ENVIRONMENT)
     @validate_arguments
     async def assign(self, assignment: RoleAssignmentCreate) -> RoleAssignmentRead:
         """
         Assigns a role to a user in the scope of a given tenant.
 
         Args:
             assignment: The role assignment details.
@@ -80,30 +88,32 @@
             PermitApiError: If the API returns an error HTTP status code.
             PermitContextError: If the configured ApiContext does not match the required endpoint context.
         """
         return await self.__role_assignments.post(
             "", model=RoleAssignmentRead, json=assignment
         )
 
-    @ensure_context(ApiKeyLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_context(ApiContextLevel.ENVIRONMENT)
     @validate_arguments
     async def unassign(self, unassignment: RoleAssignmentRemove) -> None:
         """
         Unassigns a role from a user in the scope of a given tenant.
 
         Args:
             unassignment: The role unassignment details.
 
         Raises:
             PermitApiError: If the API returns an error HTTP status code.
             PermitContextError: If the configured ApiContext does not match the required endpoint context.
         """
         return await self.__role_assignments.delete("", json=unassignment)
 
-    @ensure_context(ApiKeyLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_context(ApiContextLevel.ENVIRONMENT)
     @validate_arguments
     async def bulk_assign(
         self, assignments: List[RoleAssignmentCreate]
     ) -> BulkRoleAssignmentReport:
         """
         Assigns multiple roles in bulk using the provided role assignments data.
         Each role assignment is a tuple of (user, role, tenant).
@@ -120,15 +130,16 @@
         """
         return await self.__role_assignments.post(
             "/bulk",
             model=BulkRoleAssignmentReport,
             json=[assignment for assignment in assignments],
         )
 
-    @ensure_context(ApiKeyLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_context(ApiContextLevel.ENVIRONMENT)
     @validate_arguments
     async def bulk_unassign(
         self, unassignments: List[RoleAssignmentRemove]
     ) -> BulkRoleUnAssignmentReport:
         """
         Removes multiple role assignments in bulk using the provided unassignment data.
         Each role to unassign is a tuple of (user, role, tenant).
```

### Comparing `permit-2.0.4/permit/api/roles.py` & `permit-2.0.5/permit/api/roles.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 from typing import List
 
 from pydantic import validate_arguments
 
-from .base import BasePermitApi, SimpleHttpClient, ensure_context, pagination_params
-from .context import ApiKeyLevel
+from .base import (
+    BasePermitApi,
+    SimpleHttpClient,
+    pagination_params,
+    required_context,
+    required_permissions,
+)
+from .context import ApiContextLevel, ApiKeyAccessLevel
 from .models import (
     AddRolePermissions,
     RemoveRolePermissions,
     RoleCreate,
     RoleRead,
     RoleUpdate,
 )
@@ -23,15 +29,16 @@
         return self._build_http_client(
             "/v2/schema/{proj_id}/{env_id}/roles".format(
                 proj_id=self.config.api_context.project,
                 env_id=self.config.api_context.environment,
             )
         )
 
-    @ensure_context(ApiKeyLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_context(ApiContextLevel.ENVIRONMENT)
     @validate_arguments
     async def list(self, page: int = 1, per_page: int = 100) -> List[RoleRead]:
         """
         Retrieves a list of roles.
 
         Args:
             page: The page number to fetch (default: 1).
@@ -44,15 +51,19 @@
             PermitApiError: If the API returns an error HTTP status code.
             PermitContextError: If the configured ApiContext does not match the required endpoint context.
         """
         return await self.__roles.get(
             "", model=List[RoleRead], params=pagination_params(page, per_page)
         )
 
-    @ensure_context(ApiKeyLevel.ENVIRONMENT_LEVEL_API_KEY)
+    async def _get(self, role_key: str) -> RoleRead:
+        return await self.__roles.get(f"/{role_key}", model=RoleRead)
+
+    @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_context(ApiContextLevel.ENVIRONMENT)
     @validate_arguments
     async def get(self, role_key: str) -> RoleRead:
         """
         Retrieves a role by its key.
 
         Args:
             role_key: The key of the role.
@@ -60,17 +71,18 @@
         Returns:
             The role.
 
         Raises:
             PermitApiError: If the API returns an error HTTP status code.
             PermitContextError: If the configured ApiContext does not match the required endpoint context.
         """
-        return await self.__roles.get(f"/{role_key}", model=RoleRead)
+        return await self._get(role_key)
 
-    @ensure_context(ApiKeyLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_context(ApiContextLevel.ENVIRONMENT)
     @validate_arguments
     async def get_by_key(self, role_key: str) -> RoleRead:
         """
         Retrieves a role by its key.
         Alias for the get method.
 
         Args:
@@ -79,17 +91,18 @@
         Returns:
             The role.
 
         Raises:
             PermitApiError: If the API returns an error HTTP status code.
             PermitContextError: If the configured ApiContext does not match the required endpoint context.
         """
-        return await self.get(role_key)
+        return await self._get(role_key)
 
-    @ensure_context(ApiKeyLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_context(ApiContextLevel.ENVIRONMENT)
     @validate_arguments
     async def get_by_id(self, role_id: str) -> RoleRead:
         """
         Retrieves a role by its ID.
         Alias for the get method.
 
         Args:
@@ -98,17 +111,18 @@
         Returns:
             The role.
 
         Raises:
             PermitApiError: If the API returns an error HTTP status code.
             PermitContextError: If the configured ApiContext does not match the required endpoint context.
         """
-        return await self.get(role_id)
+        return await self._get(role_id)
 
-    @ensure_context(ApiKeyLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_context(ApiContextLevel.ENVIRONMENT)
     @validate_arguments
     async def create(self, role_data: RoleCreate) -> RoleRead:
         """
         Creates a new role.
 
         Args:
             role_data: The data for the new role.
@@ -118,15 +132,16 @@
 
         Raises:
             PermitApiError: If the API returns an error HTTP status code.
             PermitContextError: If the configured ApiContext does not match the required endpoint context.
         """
         return await self.__roles.post("", model=RoleRead, json=role_data)
 
-    @ensure_context(ApiKeyLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_context(ApiContextLevel.ENVIRONMENT)
     @validate_arguments
     async def update(self, role_key: str, role_data: RoleUpdate) -> RoleRead:
         """
         Updates a role.
 
         Args:
             role_key: The key of the role.
@@ -137,30 +152,32 @@
 
         Raises:
             PermitApiError: If the API returns an error HTTP status code.
             PermitContextError: If the configured ApiContext does not match the required endpoint context.
         """
         return await self.__roles.patch(f"/{role_key}", model=RoleRead, json=role_data)
 
-    @ensure_context(ApiKeyLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_context(ApiContextLevel.ENVIRONMENT)
     @validate_arguments
     async def delete(self, role_key: str) -> None:
         """
         Deletes a role.
 
         Args:
             role_key: The key of the role to delete.
 
         Raises:
             PermitApiError: If the API returns an error HTTP status code.
             PermitContextError: If the configured ApiContext does not match the required endpoint context.
         """
         return await self.__roles.delete(f"/{role_key}")
 
-    @ensure_context(ApiKeyLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_context(ApiContextLevel.ENVIRONMENT)
     @validate_arguments
     async def assign_permissions(
         self, role_key: str, permissions: List[str]
     ) -> RoleRead:
         """
         Assigns permissions to a role.
 
@@ -177,15 +194,16 @@
         """
         return await self.__roles.post(
             f"/{role_key}/permissions",
             model=RoleRead,
             json=AddRolePermissions(permissions=permissions),
         )
 
-    @ensure_context(ApiKeyLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_context(ApiContextLevel.ENVIRONMENT)
     @validate_arguments
     async def remove_permissions(
         self, role_key: str, permissions: List[str]
     ) -> RoleRead:
         """
         Removes permissions from a role.
```

### Comparing `permit-2.0.4/permit/api/sync_api_client.py` & `permit-2.0.5/permit/api/sync_api_client.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.4/permit/api/tenants.py` & `permit-2.0.5/permit/api/tenants.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,34 @@
 from typing import List
 
 from pydantic import validate_arguments
 
-from .base import BasePermitApi, SimpleHttpClient, ensure_context, pagination_params
-from .context import ApiKeyLevel
+from .base import (
+    BasePermitApi,
+    SimpleHttpClient,
+    pagination_params,
+    required_context,
+    required_permissions,
+)
+from .context import ApiContextLevel, ApiKeyAccessLevel
 from .models import PaginatedResultUserRead, TenantCreate, TenantRead, TenantUpdate
 
 
 class TenantsApi(BasePermitApi):
     @property
     def __tenants(self) -> SimpleHttpClient:
         return self._build_http_client(
             "/v2/facts/{proj_id}/{env_id}/tenants".format(
                 proj_id=self.config.api_context.project,
                 env_id=self.config.api_context.environment,
             )
         )
 
-    @ensure_context(ApiKeyLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_context(ApiContextLevel.ENVIRONMENT)
     @validate_arguments
     async def list(self, page: int = 1, per_page: int = 100) -> List[TenantRead]:
         """
         Retrieves a list of tenants.
 
         Args:
             page: The page number to fetch (default: 1).
@@ -34,15 +41,16 @@
             PermitApiError: If the API returns an error HTTP status code.
             PermitContextError: If the configured ApiContext does not match the required endpoint context.
         """
         return await self.__tenants.get(
             "", model=List[TenantRead], params=pagination_params(page, per_page)
         )
 
-    @ensure_context(ApiKeyLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_context(ApiContextLevel.ENVIRONMENT)
     @validate_arguments
     async def list_tenant_users(
         self, tenant_key: str, page: int = 1, per_page: int = 100
     ) -> PaginatedResultUserRead:
         """
         Retrieves a list of users for a given tenant.
 
@@ -60,15 +68,19 @@
         """
         return await self.__tenants.get(
             f"/{tenant_key}/users",
             model=PaginatedResultUserRead,
             params=pagination_params(page, per_page),
         )
 
-    @ensure_context(ApiKeyLevel.ENVIRONMENT_LEVEL_API_KEY)
+    async def _get(self, tenant_key: str) -> TenantRead:
+        return await self.__tenants.get(f"/{tenant_key}", model=TenantRead)
+
+    @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_context(ApiContextLevel.ENVIRONMENT)
     @validate_arguments
     async def get(self, tenant_key: str) -> TenantRead:
         """
         Retrieves a tenant by its key.
 
         Args:
             tenant_key: The key of the tenant.
@@ -76,17 +88,18 @@
         Returns:
             the tenant.
 
         Raises:
             PermitApiError: If the API returns an error HTTP status code.
             PermitContextError: If the configured ApiContext does not match the required endpoint context.
         """
-        return await self.__tenants.get(f"/{tenant_key}", model=TenantRead)
+        return await self._get(tenant_key)
 
-    @ensure_context(ApiKeyLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_context(ApiContextLevel.ENVIRONMENT)
     @validate_arguments
     async def get_by_key(self, tenant_key: str) -> TenantRead:
         """
         Retrieves a tenant by its key.
         Alias for the get method.
 
         Args:
@@ -95,17 +108,18 @@
         Returns:
             the tenant.
 
         Raises:
             PermitApiError: If the API returns an error HTTP status code.
             PermitContextError: If the configured ApiContext does not match the required endpoint context.
         """
-        return await self.get(tenant_key)
+        return await self._get(tenant_key)
 
-    @ensure_context(ApiKeyLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_context(ApiContextLevel.ENVIRONMENT)
     @validate_arguments
     async def get_by_id(self, tenant_id: str) -> TenantRead:
         """
         Retrieves a tenant by its ID.
         Alias for the get method.
 
         Args:
@@ -114,17 +128,18 @@
         Returns:
             the tenant.
 
         Raises:
             PermitApiError: If the API returns an error HTTP status code.
             PermitContextError: If the configured ApiContext does not match the required endpoint context.
         """
-        return await self.get(tenant_id)
+        return await self._get(tenant_id)
 
-    @ensure_context(ApiKeyLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_context(ApiContextLevel.ENVIRONMENT)
     @validate_arguments
     async def create(self, tenant_data: TenantCreate) -> TenantRead:
         """
         Creates a new tenant.
 
         Args:
             tenant_data: The data for the new tenant.
@@ -134,15 +149,16 @@
 
         Raises:
             PermitApiError: If the API returns an error HTTP status code.
             PermitContextError: If the configured ApiContext does not match the required endpoint context.
         """
         return await self.__tenants.post("", model=TenantRead, json=tenant_data)
 
-    @ensure_context(ApiKeyLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_context(ApiContextLevel.ENVIRONMENT)
     @validate_arguments
     async def update(self, tenant_key: str, tenant_data: TenantUpdate) -> TenantRead:
         """
         Updates a tenant.
 
         Args:
             tenant_key: The key of the tenant.
@@ -155,15 +171,16 @@
             PermitApiError: If the API returns an error HTTP status code.
             PermitContextError: If the configured ApiContext does not match the required endpoint context.
         """
         return await self.__tenants.patch(
             f"/{tenant_key}", model=TenantRead, json=tenant_data
         )
 
-    @ensure_context(ApiKeyLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_context(ApiContextLevel.ENVIRONMENT)
     @validate_arguments
     async def delete(self, tenant_key: str) -> None:
         """
         Deletes a tenant.
 
         Args:
             tenant_key: The key of the tenant to delete.
@@ -173,15 +190,16 @@
 
         Raises:
             PermitApiError: If the API returns an error HTTP status code.
             PermitContextError: If the configured ApiContext does not match the required endpoint context.
         """
         return await self.__tenants.delete(f"/{tenant_key}")
 
-    @ensure_context(ApiKeyLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_context(ApiContextLevel.ENVIRONMENT)
     @validate_arguments
     async def delete_tenant_user(self, tenant_key: str, user_key: str) -> None:
         """
         Deletes a user from a given tenant (also removes all roles granted to the user in that tenant).
 
         Args:
             tenant_key: The key of the tenant from which the user will be deleted.
```

### Comparing `permit-2.0.4/permit/api/users.py` & `permit-2.0.5/permit/api/users.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 from typing import List, Optional, Union
 
 from pydantic import validate_arguments
 
-from .base import BasePermitApi, SimpleHttpClient, ensure_context, pagination_params
-from .context import ApiKeyLevel
+from .base import (
+    BasePermitApi,
+    SimpleHttpClient,
+    pagination_params,
+    required_context,
+    required_permissions,
+)
+from .context import ApiContextLevel, ApiKeyAccessLevel
 from .models import (
     PaginatedResultUserRead,
     RoleAssignmentCreate,
     RoleAssignmentRead,
     RoleAssignmentRemove,
     UserCreate,
     UserRead,
@@ -30,15 +36,16 @@
         return self._build_http_client(
             "/v2/facts/{proj_id}/{env_id}/role_assignments".format(
                 proj_id=self.config.api_context.project,
                 env_id=self.config.api_context.environment,
             )
         )
 
-    @ensure_context(ApiKeyLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_context(ApiContextLevel.ENVIRONMENT)
     @validate_arguments
     async def list(self, page: int = 1, per_page: int = 100) -> PaginatedResultUserRead:
         """
         Retrieves a list of users.
 
         Args:
             page: The page number to fetch (default: 1).
@@ -53,15 +60,19 @@
         """
         return await self.__users.get(
             "",
             model=PaginatedResultUserRead,
             params=pagination_params(page, per_page),
         )
 
-    @ensure_context(ApiKeyLevel.ENVIRONMENT_LEVEL_API_KEY)
+    async def _get(self, user_key: str) -> UserRead:
+        return await self.__users.get(f"/{user_key}", model=UserRead)
+
+    @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_context(ApiContextLevel.ENVIRONMENT)
     @validate_arguments
     async def get(self, user_key: str) -> UserRead:
         """
         Retrieves a user by its key.
 
         Args:
             user_key: The key of the user.
@@ -69,17 +80,18 @@
         Returns:
             the user object.
 
         Raises:
             PermitApiError: If the API returns an error HTTP status code.
             PermitContextError: If the configured ApiContext does not match the required endpoint context.
         """
-        return await self.__users.get(f"/{user_key}", model=UserRead)
+        return await self._get(user_key)
 
-    @ensure_context(ApiKeyLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_context(ApiContextLevel.ENVIRONMENT)
     @validate_arguments
     async def get_by_key(self, user_key: str) -> UserRead:
         """
         Retrieves a user by its key.
         Alias for the get method.
 
         Args:
@@ -88,17 +100,18 @@
         Returns:
             the user object.
 
         Raises:
             PermitApiError: If the API returns an error HTTP status code.
             PermitContextError: If the configured ApiContext does not match the required endpoint context.
         """
-        return await self.get(user_key)
+        return await self._get(user_key)
 
-    @ensure_context(ApiKeyLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_context(ApiContextLevel.ENVIRONMENT)
     @validate_arguments
     async def get_by_id(self, user_id: str) -> UserRead:
         """
         Retrieves a user by its ID.
         Alias for the get method.
 
         Args:
@@ -107,17 +120,18 @@
         Returns:
             the user object.
 
         Raises:
             PermitApiError: If the API returns an error HTTP status code.
             PermitContextError: If the configured ApiContext does not match the required endpoint context.
         """
-        return await self.get(user_id)
+        return await self._get(user_id)
 
-    @ensure_context(ApiKeyLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_context(ApiContextLevel.ENVIRONMENT)
     @validate_arguments
     async def create(self, user_data: UserCreate) -> UserRead:
         """
         Creates a new user.
 
         Args:
             user_data: The data for the new user.
@@ -127,15 +141,16 @@
 
         Raises:
             PermitApiError: If the API returns an error HTTP status code.
             PermitContextError: If the configured ApiContext does not match the required endpoint context.
         """
         return await self.__users.post("", model=UserRead, json=user_data)
 
-    @ensure_context(ApiKeyLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_context(ApiContextLevel.ENVIRONMENT)
     @validate_arguments
     async def update(self, user_key: str, user_data: UserUpdate) -> UserRead:
         """
         Updates a user.
 
         Args:
             user_key: The key of the user.
@@ -146,15 +161,16 @@
 
         Raises:
             PermitApiError: If the API returns an error HTTP status code.
             PermitContextError: If the configured ApiContext does not match the required endpoint context.
         """
         return await self.__users.patch(f"/{user_key}", model=UserRead, json=user_data)
 
-    @ensure_context(ApiKeyLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_context(ApiContextLevel.ENVIRONMENT)
     @validate_arguments
     async def sync(self, user: Union[UserCreate, dict]) -> UserRead:
         """
         Synchronizes user data by creating or updating a user.
 
         Args:
             user: The data of the user to be synchronized.
@@ -170,30 +186,32 @@
             user_key = user.pop("key", None)
             if user_key is None:
                 raise KeyError("required 'key' in input dictionary")
         else:
             user_key = user.key
         return await self.__users.put(f"/{user_key}", model=UserRead, json=user)
 
-    @ensure_context(ApiKeyLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_context(ApiContextLevel.ENVIRONMENT)
     @validate_arguments
     async def delete(self, user_key: str) -> None:
         """
         Deletes a user.
 
         Args:
             user_key: The key of the user to delete.
 
         Raises:
             PermitApiError: If the API returns an error HTTP status code.
             PermitContextError: If the configured ApiContext does not match the required endpoint context.
         """
         return await self.__users.delete(f"/{user_key}")
 
-    @ensure_context(ApiKeyLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_context(ApiContextLevel.ENVIRONMENT)
     @validate_arguments
     async def assign_role(self, assignment: RoleAssignmentCreate) -> RoleAssignmentRead:
         """
         Assigns a role to a user in the scope of a given tenant.
 
         Args:
             assignment: The role assignment details.
@@ -207,15 +225,16 @@
         """
         return await self.__users.post(
             f"/{assignment.user}/roles",
             model=RoleAssignmentRead,
             json=assignment.dict(exclude={"user"}),
         )
 
-    @ensure_context(ApiKeyLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_context(ApiContextLevel.ENVIRONMENT)
     @validate_arguments
     async def unassign_role(self, unassignment: RoleAssignmentRemove) -> None:
         """
         Unassigns a role from a user in the scope of a given tenant.
 
         Args:
             unassignment: The role unassignment details.
@@ -225,15 +244,16 @@
             PermitContextError: If the configured ApiContext does not match the required endpoint context.
         """
         return await self.__users.delete(
             f"/{unassignment.user}/roles",
             json=unassignment.dict(exclude={"user"}),
         )
 
-    @ensure_context(ApiKeyLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_context(ApiContextLevel.ENVIRONMENT)
     @validate_arguments
     async def get_assigned_roles(
         self,
         user: str,
         tenant: Optional[str] = None,
         page: int = 1,
         per_page: int = 100,
```

### Comparing `permit-2.0.4/permit/config.py` & `permit-2.0.5/permit/config.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.4/permit/enforcement/enforcer.py` & `permit-2.0.5/permit/enforcement/enforcer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import json
+from pprint import pformat
 from typing import Union
 
 import aiohttp
 from loguru import logger
 
 from ..config import PermitConfig
 from ..exceptions import PermitConnectionError
@@ -71,14 +72,15 @@
             # can the user close any issue who's id is 1234?
             await permit.check(user, 'close', 'issue:1234')
 
             # can the user close (any) issues belonging to the 't1' tenant?
             # (in a multi tenant application)
             await permit.check(user, 'close', {'type': 'issue', 'tenant': 't1'})
         """
+
         normalized_user: UserInput = (
             UserInput(key=user) if isinstance(user, str) else UserInput(**user)
         )
         normalized_resource: ResourceInput = self._normalize_resource(
             (
                 self._resource_from_string(resource)
                 if isinstance(resource, str)
@@ -90,17 +92,18 @@
             user=normalized_user.dict(),
             action=action,
             resource=normalized_resource.dict(),
             context=query_context,
         )
 
         async with aiohttp.ClientSession(headers=self._headers) as session:
+            check_url = f"{self._base_url}/allowed"
             try:
                 async with session.post(
-                    f"{self._base_url}/allowed",
+                    check_url,
                     data=json.dumps(input),
                 ) as response:
                     if response.status != 200:
                         error_json: dict = await response.json()
                         logger.error(
                             "error in permit.check({}, {}, {}):\n{}\n{}".format(
                                 normalized_user,
@@ -112,23 +115,27 @@
                         )
                         raise PermitConnectionError(
                             f"Permit SDK got unexpected status code: {response.status}, please check your Permit SDK class init and PDP container are configured correctly. \n\
                             Read more about setting up the PDP at https://docs.permit.io/reference/SDKs/Python/quickstart_python"
                         )
 
                     content: dict = await response.json()
-                    decision: bool = bool(content.get("allow", False))
                     logger.debug(
-                        "permit.check({}, {}, {}) = {}".format(
-                            normalized_user,
-                            action,
-                            self._resource_repr(normalized_resource),
-                            repr(decision),
-                        )
+                        f"permit.check() response:\ninput: {pformat(input, indent=2)}\nresponse status: {response.status}\nresponse data: {pformat(content, indent=2)}"
                     )
+                    decision: bool = bool(content.get("allow", False))
+                    # TODO: restore simple log when PDP is fixed
+                    # logger.debug(
+                    #     "permit.check({}, {}, {}) = {}".format(
+                    #         normalized_user,
+                    #         action,
+                    #         self._resource_repr(normalized_resource),
+                    #         repr(decision),
+                    #     )
+                    # )
                     return decision
             except aiohttp.ClientError as err:
                 logger.error(
                     "error in permit.check({}, {}, {}):\n{}".format(
                         normalized_user,
                         action,
                         self._resource_repr(normalized_resource),
```

### Comparing `permit-2.0.4/permit/enforcement/interfaces.py` & `permit-2.0.5/permit/enforcement/interfaces.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.4/permit/permit.py` & `permit-2.0.5/permit/permit.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.4/permit/sync.py` & `permit-2.0.5/permit/sync.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.4/permit/utils/context.py` & `permit-2.0.5/permit/utils/context.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.4/permit/utils/sync.py` & `permit-2.0.5/permit/utils/sync.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,29 +5,18 @@
 
 from typing_extensions import ParamSpec, TypeGuard
 
 P = ParamSpec("P")
 T = TypeVar("T")
 
 
-def run_sync(callback: Awaitable[T]) -> T:
-    try:
-        loop = asyncio.get_running_loop()
-    except RuntimeError:
-        # there is no running event loop, so it's safe to use `asyncio.run`
-        return asyncio.run(callback)
-    else:
-        # there *is* a running event loop, so use `loop.run_until_complete`
-        return loop.run_until_complete(callback)
-
-
 def async_to_sync(func: Callable[P, Awaitable[T]]) -> Callable[P, T]:
     @wraps(func)
     def wrapper(*args: P.args, **kwargs: P.kwargs) -> T:
-        return run_sync(func(*args, **kwargs))
+        return asyncio.run(func(*args, **kwargs))
 
     return wrapper
 
 
 def iscoroutine_func(callable: Callable) -> TypeGuard[Callable[..., Awaitable]]:
     return iscoroutinefunction(callable)
```

### Comparing `permit-2.0.4/permit.egg-info/SOURCES.txt` & `permit-2.0.5/permit.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 permit/api/tenants.py
 permit/api/users.py
 permit/enforcement/__init__.py
 permit/enforcement/enforcer.py
 permit/enforcement/interfaces.py
 permit/utils/__init__.py
 permit/utils/context.py
+permit/utils/deprecation.py
 permit/utils/dicts.py
 permit/utils/sync.py
 tests/__init__.py
 tests/conftest.py
 tests/test_abac_e2e.py
 tests/test_rbac_e2e.py
 tests/test_rbac_e2e_sync.py
```

### Comparing `permit-2.0.4/setup.py` & `permit-2.0.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
         env = "-{}".format(env)
     with open("requirements{}.txt".format(env)) as fp:
         return [x.strip() for x in fp.read().split("\n") if not x.startswith("#")]
 
 
 setup(
     name="permit",
-    version="2.0.4",
+    version="2.0.5",
     packages=find_packages(),
     author="Asaf Cohen",
     author_email="asaf@permit.io",
     license="Apache 2.0",
     python_requires=">=3.8",
     description="Permit.io python sdk",
     install_requires=get_requirements(),
```

### Comparing `permit-2.0.4/tests/conftest.py` & `permit-2.0.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.4/tests/test_abac_e2e.py` & `permit-2.0.5/tests/test_abac_e2e.py`

 * *Files 2% similar despite different names*

```diff
@@ -235,39 +235,42 @@
         print_break()
 
         logger.info(
             f"sleeping {ABAC_SLEEP_TIME} seconds before permit.check() to make sure all writes propagated from cloud to PDP"
         )
         time.sleep(ABAC_SLEEP_TIME)
 
+        def abac_user(user: UserCreate):
+            return user.dict(exclude={"first_name", "last_name"})
+
         logger.info("testing that users over 30 can sign public documents")
         assert await permit.check(
-            USER_A.key,
+            abac_user(USER_A),
             "sign",
             {
                 "type": "document",
                 "tenant": TESLA.key,
                 "attributes": {"private": False},
             },
         )
 
         logger.info("testing that users under 30 cannot sign public documents")
         assert not await permit.check(
-            USER_B.key,
+            abac_user(USER_B),
             "sign",
             {
                 "type": "document",
                 "tenant": TESLA.key,
                 "attributes": {"private": False},
             },
         )
 
         logger.info("testing that users over 30 cannot sign private documents")
         assert not await permit.check(
-            USER_A.key,
+            abac_user(USER_A),
             "sign",
             {
                 "type": "document",
                 "tenant": TESLA.key,
                 "attributes": {"private": True},
             },
         )
```

### Comparing `permit-2.0.4/tests/test_rbac_e2e.py` & `permit-2.0.5/tests/test_rbac_e2e.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.4/tests/test_rbac_e2e_sync.py` & `permit-2.0.5/tests/test_rbac_e2e_sync.py`

 * *Files identical despite different names*

