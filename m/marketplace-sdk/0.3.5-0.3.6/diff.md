# Comparing `tmp/marketplace_sdk-0.3.5.tar.gz` & `tmp/marketplace_sdk-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "marketplace_sdk-0.3.5.tar", last modified: Fri Apr 21 15:06:46 2023, max compression
+gzip compressed data, was "marketplace_sdk-0.3.6.tar", last modified: Tue Jun 13 11:59:24 2023, max compression
```

## Comparing `marketplace_sdk-0.3.5.tar` & `marketplace_sdk-0.3.6.tar`

### file list

```diff
@@ -1,38 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:06:46.403979 marketplace_sdk-0.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-21 15:06:37.000000 marketplace_sdk-0.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-21 15:06:37.000000 marketplace_sdk-0.3.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-04-21 15:06:46.403979 marketplace_sdk-0.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-04-21 15:06:37.000000 marketplace_sdk-0.3.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:06:46.399979 marketplace_sdk-0.3.5/logos/
--rw-r--r--   0 runner    (1001) docker     (123)    17494 2023-04-21 15:06:37.000000 marketplace_sdk-0.3.5/logos/MARVEL.png
--rw-r--r--   0 runner    (1001) docker     (123)    27591 2023-04-21 15:06:37.000000 marketplace_sdk-0.3.5/logos/MarketPlace.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:06:46.403979 marketplace_sdk-0.3.5/marketplace/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-21 15:06:37.000000 marketplace_sdk-0.3.5/marketplace/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:06:46.403979 marketplace_sdk-0.3.5/marketplace/app/
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-04-21 15:06:37.000000 marketplace_sdk-0.3.5/marketplace/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-04-21 15:06:37.000000 marketplace_sdk-0.3.5/marketplace/app/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:06:46.403979 marketplace_sdk-0.3.5/marketplace/app/v0/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-21 15:06:37.000000 marketplace_sdk-0.3.5/marketplace/app/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-04-21 15:06:37.000000 marketplace_sdk-0.3.5/marketplace/app/v0/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7496 2023-04-21 15:06:37.000000 marketplace_sdk-0.3.5/marketplace/app/v0/object_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-04-21 15:06:37.000000 marketplace_sdk-0.3.5/marketplace/app/v0/transformation.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-21 15:06:37.000000 marketplace_sdk-0.3.5/marketplace/app/v0/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:06:46.403979 marketplace_sdk-0.3.5/marketplace/app/v0_0_1/
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-04-21 15:06:37.000000 marketplace_sdk-0.3.5/marketplace/app/v0_0_1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-04-21 15:06:37.000000 marketplace_sdk-0.3.5/marketplace/app/v0_0_1/data_sink_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     4917 2023-04-21 15:06:37.000000 marketplace_sdk-0.3.5/marketplace/app/v0_0_1/data_source_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-04-21 15:06:37.000000 marketplace_sdk-0.3.5/marketplace/app/v0_0_1/transformation_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-04-21 15:06:37.000000 marketplace_sdk-0.3.5/marketplace/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:06:46.403979 marketplace_sdk-0.3.5/marketplace/message_broker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 15:06:37.000000 marketplace_sdk-0.3.5/marketplace/message_broker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-04-21 15:06:37.000000 marketplace_sdk-0.3.5/marketplace/message_broker/rpc_server.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-21 15:06:37.000000 marketplace_sdk-0.3.5/marketplace/message_broker/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-21 15:06:37.000000 marketplace_sdk-0.3.5/marketplace/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:06:46.403979 marketplace_sdk-0.3.5/marketplace_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-04-21 15:06:46.000000 marketplace_sdk-0.3.5/marketplace_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-21 15:06:46.000000 marketplace_sdk-0.3.5/marketplace_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 15:06:46.000000 marketplace_sdk-0.3.5/marketplace_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-21 15:06:46.000000 marketplace_sdk-0.3.5/marketplace_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-21 15:06:46.000000 marketplace_sdk-0.3.5/marketplace_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-04-21 15:06:46.403979 marketplace_sdk-0.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-21 15:06:37.000000 marketplace_sdk-0.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:59:24.577458 marketplace_sdk-0.3.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-13 11:59:14.000000 marketplace_sdk-0.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-13 11:59:14.000000 marketplace_sdk-0.3.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-06-13 11:59:24.577458 marketplace_sdk-0.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-06-13 11:59:14.000000 marketplace_sdk-0.3.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:59:24.573458 marketplace_sdk-0.3.6/logos/
+-rw-r--r--   0 runner    (1001) docker     (123)    17494 2023-06-13 11:59:14.000000 marketplace_sdk-0.3.6/logos/MARVEL.png
+-rw-r--r--   0 runner    (1001) docker     (123)    27591 2023-06-13 11:59:14.000000 marketplace_sdk-0.3.6/logos/MarketPlace.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:59:24.573458 marketplace_sdk-0.3.6/marketplace/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-13 11:59:14.000000 marketplace_sdk-0.3.6/marketplace/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:59:24.573458 marketplace_sdk-0.3.6/marketplace/app/
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-13 11:59:14.000000 marketplace_sdk-0.3.6/marketplace/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-13 11:59:14.000000 marketplace_sdk-0.3.6/marketplace/app/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:59:24.577458 marketplace_sdk-0.3.6/marketplace/app/v0/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-13 11:59:14.000000 marketplace_sdk-0.3.6/marketplace/app/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-13 11:59:14.000000 marketplace_sdk-0.3.6/marketplace/app/v0/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7496 2023-06-13 11:59:14.000000 marketplace_sdk-0.3.6/marketplace/app/v0/object_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-06-13 11:59:14.000000 marketplace_sdk-0.3.6/marketplace/app/v0/transformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-13 11:59:14.000000 marketplace_sdk-0.3.6/marketplace/app/v0/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-06-13 11:59:14.000000 marketplace_sdk-0.3.6/marketplace/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:59:24.577458 marketplace_sdk-0.3.6/marketplace/message_broker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 11:59:14.000000 marketplace_sdk-0.3.6/marketplace/message_broker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-06-13 11:59:14.000000 marketplace_sdk-0.3.6/marketplace/message_broker/rpc_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-13 11:59:14.000000 marketplace_sdk-0.3.6/marketplace/message_broker/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-13 11:59:14.000000 marketplace_sdk-0.3.6/marketplace/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:59:24.577458 marketplace_sdk-0.3.6/marketplace_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-06-13 11:59:24.000000 marketplace_sdk-0.3.6/marketplace_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-13 11:59:24.000000 marketplace_sdk-0.3.6/marketplace_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 11:59:24.000000 marketplace_sdk-0.3.6/marketplace_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-13 11:59:24.000000 marketplace_sdk-0.3.6/marketplace_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-13 11:59:24.000000 marketplace_sdk-0.3.6/marketplace_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-06-13 11:59:24.577458 marketplace_sdk-0.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-13 11:59:14.000000 marketplace_sdk-0.3.6/setup.py
```

### Comparing `marketplace_sdk-0.3.5/LICENSE` & `marketplace_sdk-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `marketplace_sdk-0.3.5/PKG-INFO` & `marketplace_sdk-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marketplace_sdk
-Version: 0.3.5
+Version: 0.3.6
 Summary: Software Development Toolkit to communicate with the Materials MarketPlace platform.
 Home-page: https://github.com/materials-marketplace/python-sdk
 Author: Carl Simon Adorf, Pablo de Andres, Pranjali Singh and the AiiDAlab team
 Author-email: simon.adorf@epfl.ch, pablo.de.andres@iwm.fraunhofer.de, pranjali.singh@iwm.fraunhofer.de
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `marketplace_sdk-0.3.5/README.md` & `marketplace_sdk-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `marketplace_sdk-0.3.5/logos/MARVEL.png` & `marketplace_sdk-0.3.6/logos/MARVEL.png`

 * *Files identical despite different names*

### Comparing `marketplace_sdk-0.3.5/logos/MarketPlace.png` & `marketplace_sdk-0.3.6/logos/MarketPlace.png`

 * *Files identical despite different names*

### Comparing `marketplace_sdk-0.3.5/marketplace/app/__init__.py` & `marketplace_sdk-0.3.6/marketplace/app/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,19 @@
 """Module for handling the different types of MarketPlace apps and their
 capabilities.
 .. currentmodule:: marketplace.app
 .. moduleauthor:: Pablo de Andres, Pranjali Singh (Fraunhofer IWM)
 """
-import warnings
 from typing import Optional
 
 from packaging.version import parse
 
 from ..client import MarketPlaceClient
 from .utils import camel_to_snake
 from .v0 import MarketPlaceApp as _MarketPlaceApp_v0
-from .v0_0_1 import MarketPlaceApp as _MarketPlaceApp_v0_0_1
-
-
-class MarketPlaceApp(_MarketPlaceApp_v0_0_1):
-    def __init__(self, *args, **kwargs):
-        warnings.warn(
-            "The MarketPlaceApp class is deprecated as of v0.2.0 and will be "
-            "removed in v1. Please use the get_app() function instead."
-        )
-        super().__init__(*args, **kwargs)
 
 
 def get_app(app_id, client: Optional[MarketPlaceClient] = None, **kwargs):
     """Get an app instance.
     Args:
         app_id (str): client id of the app
         **kwargs: keyword arguments for the app
@@ -32,33 +21,21 @@
         MarketPlaceApp: app instance
     """
     client = client or MarketPlaceClient()
 
     # Getting api version and list of capabilities for the application
     app_service_path = f"api/applications/{app_id}"
     app_info: dict = client.get(path=app_service_path).json()
-    app_api_version = parse(app_info.get("api_version", "0.0.1"))
+    app_api_version = parse(app_info.get("api_version", "1.0.0"))
 
     capabilities = []
     for capability in app_info["capabilities"]:
         capabilities.append(camel_to_snake(capability["name"]))
 
-    if app_api_version == parse("0.0.1"):
-        if client is not None:
-            raise RuntimeError(
-                "Cannot use existing client for apps with API version 0.0.1."
-            )
-        return _MarketPlaceApp_v0_0_1(
-            app_id,
-            marketplace_host_url=kwargs.get("marketplace_host_url"),
-            access_token=kwargs.get("access_token"),
-            capabilities=capabilities,
-            **kwargs,
-        )
-    elif parse("0.0.1") < app_api_version <= parse("0.3.0"):
+    if app_api_version < parse("1.0.0"):
         return _MarketPlaceApp_v0(app_id, app_info, client, **kwargs)
     else:
         raise RuntimeError(f"App API version ({app_api_version}) not supported.")
 
 
 __all__ = [
     "MarketPlaceApp",
```

### Comparing `marketplace_sdk-0.3.5/marketplace/app/utils.py` & `marketplace_sdk-0.3.6/marketplace/app/utils.py`

 * *Files identical despite different names*

### Comparing `marketplace_sdk-0.3.5/marketplace/app/v0/base.py` & `marketplace_sdk-0.3.6/marketplace/app/v0/base.py`

 * *Files identical despite different names*

### Comparing `marketplace_sdk-0.3.5/marketplace/app/v0/object_storage.py` & `marketplace_sdk-0.3.6/marketplace/app/v0/object_storage.py`

 * *Files identical despite different names*

### Comparing `marketplace_sdk-0.3.5/marketplace/app/v0/transformation.py` & `marketplace_sdk-0.3.6/marketplace/app/v0/transformation.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         transformation_id: transformation.TransformationId,
         update: transformation.TransformationUpdateModel,
     ) -> transformation.TransformationUpdateResponse:
         return transformation.TransformationUpdateResponse.parse_obj(
             self._client.patch(
                 self._proxy_path("updateTransformation"),
                 params={"transformation_id": transformation_id},
-                json=update.json(),
+                json=update.dict(),
             ).json()
         )
 
     def start_transformation(
         self, transformation_id: transformation.TransformationId
     ) -> transformation.TransformationStateResponse:
         update: transformation.TransformationUpdateModel = (
```

### Comparing `marketplace_sdk-0.3.5/marketplace/client.py` & `marketplace_sdk-0.3.6/marketplace/client.py`

 * *Files identical despite different names*

### Comparing `marketplace_sdk-0.3.5/marketplace/message_broker/rpc_server.py` & `marketplace_sdk-0.3.6/marketplace/message_broker/rpc_server.py`

 * *Files identical despite different names*

### Comparing `marketplace_sdk-0.3.5/marketplace_sdk.egg-info/PKG-INFO` & `marketplace_sdk-0.3.6/marketplace_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marketplace-sdk
-Version: 0.3.5
+Version: 0.3.6
 Summary: Software Development Toolkit to communicate with the Materials MarketPlace platform.
 Home-page: https://github.com/materials-marketplace/python-sdk
 Author: Carl Simon Adorf, Pablo de Andres, Pranjali Singh and the AiiDAlab team
 Author-email: simon.adorf@epfl.ch, pablo.de.andres@iwm.fraunhofer.de, pranjali.singh@iwm.fraunhofer.de
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `marketplace_sdk-0.3.5/marketplace_sdk.egg-info/SOURCES.txt` & `marketplace_sdk-0.3.6/marketplace_sdk.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -11,18 +11,14 @@
 marketplace/app/__init__.py
 marketplace/app/utils.py
 marketplace/app/v0/__init__.py
 marketplace/app/v0/base.py
 marketplace/app/v0/object_storage.py
 marketplace/app/v0/transformation.py
 marketplace/app/v0/utils.py
-marketplace/app/v0_0_1/__init__.py
-marketplace/app/v0_0_1/data_sink_app.py
-marketplace/app/v0_0_1/data_source_app.py
-marketplace/app/v0_0_1/transformation_app.py
 marketplace/message_broker/__init__.py
 marketplace/message_broker/rpc_server.py
 marketplace/message_broker/utils.py
 marketplace_sdk.egg-info/PKG-INFO
 marketplace_sdk.egg-info/SOURCES.txt
 marketplace_sdk.egg-info/dependency_links.txt
 marketplace_sdk.egg-info/requires.txt
```

### Comparing `marketplace_sdk-0.3.5/setup.cfg` & `marketplace_sdk-0.3.6/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [metadata]
 name = marketplace_sdk
-version = v0.3.5
+version = v0.3.6
 description = Software Development Toolkit to communicate with the Materials MarketPlace platform.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/materials-marketplace/python-sdk
 author = Carl Simon Adorf, Pablo de Andres, Pranjali Singh and the AiiDAlab team
 author_email = simon.adorf@epfl.ch, pablo.de.andres@iwm.fraunhofer.de, pranjali.singh@iwm.fraunhofer.de
 license = MIT
-license_file = LICENSE
+license_files = LICENSE
 classifiers = 
 	Development Status :: 2 - Pre-Alpha
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: Implementation :: CPython
```

