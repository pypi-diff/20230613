# Comparing `tmp/api_gateway_v2_to_wsgi-1.1.0.tar.gz` & `tmp/api_gateway_v2_to_wsgi-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/api_gateway_v2_to_wsgi-1.1.0.tar", last modified: Fri Feb  5 21:48:25 2021, max compression
+gzip compressed data, was "api_gateway_v2_to_wsgi-1.1.1.tar", last modified: Tue Jun 13 16:29:06 2023, max compression
```

## Comparing `api_gateway_v2_to_wsgi-1.1.0.tar` & `api_gateway_v2_to_wsgi-1.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2021-02-05 21:48:25.463349 api_gateway_v2_to_wsgi-1.1.0/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1059 2021-02-05 21:02:10.000000 api_gateway_v2_to_wsgi-1.1.0/LICENSE
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2577 2021-02-05 21:48:25.463349 api_gateway_v2_to_wsgi-1.1.0/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1565 2021-02-05 21:02:10.000000 api_gateway_v2_to_wsgi-1.1.0/README.md
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2021-02-05 21:48:25.463349 api_gateway_v2_to_wsgi-1.1.0/api_gateway_v2_to_wsgi.egg-info/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2577 2021-02-05 21:48:25.000000 api_gateway_v2_to_wsgi-1.1.0/api_gateway_v2_to_wsgi.egg-info/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)      246 2021-02-05 21:48:25.000000 api_gateway_v2_to_wsgi-1.1.0/api_gateway_v2_to_wsgi.egg-info/SOURCES.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2021-02-05 21:48:25.000000 api_gateway_v2_to_wsgi-1.1.0/api_gateway_v2_to_wsgi.egg-info/dependency_links.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)       23 2021-02-05 21:48:25.000000 api_gateway_v2_to_wsgi-1.1.0/api_gateway_v2_to_wsgi.egg-info/top_level.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)     3718 2021-02-05 21:46:33.000000 api_gateway_v2_to_wsgi-1.1.0/api_gateway_v2_to_wsgi.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1070 2021-02-05 21:48:25.463349 api_gateway_v2_to_wsgi-1.1.0/setup.cfg
--rw-r--r--   0 asottile  (1000) asottile  (1000)       37 2021-02-05 21:02:10.000000 api_gateway_v2_to_wsgi-1.1.0/setup.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-06-13 16:29:06.392980 api_gateway_v2_to_wsgi-1.1.1/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1059 2023-06-13 16:23:44.000000 api_gateway_v2_to_wsgi-1.1.1/LICENSE
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1930 2023-06-13 16:29:06.392980 api_gateway_v2_to_wsgi-1.1.1/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1347 2023-06-13 16:23:44.000000 api_gateway_v2_to_wsgi-1.1.1/README.md
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-06-13 16:29:06.392980 api_gateway_v2_to_wsgi-1.1.1/api_gateway_v2_to_wsgi.egg-info/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1930 2023-06-13 16:29:06.000000 api_gateway_v2_to_wsgi-1.1.1/api_gateway_v2_to_wsgi.egg-info/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      246 2023-06-13 16:29:06.000000 api_gateway_v2_to_wsgi-1.1.1/api_gateway_v2_to_wsgi.egg-info/SOURCES.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2023-06-13 16:29:06.000000 api_gateway_v2_to_wsgi-1.1.1/api_gateway_v2_to_wsgi.egg-info/dependency_links.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       23 2023-06-13 16:29:06.000000 api_gateway_v2_to_wsgi-1.1.1/api_gateway_v2_to_wsgi.egg-info/top_level.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     3664 2023-06-13 16:29:06.000000 api_gateway_v2_to_wsgi-1.1.1/api_gateway_v2_to_wsgi.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1020 2023-06-13 16:29:06.392980 api_gateway_v2_to_wsgi-1.1.1/setup.cfg
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       73 2023-06-13 16:23:44.000000 api_gateway_v2_to_wsgi-1.1.1/setup.py
```

### Comparing `api_gateway_v2_to_wsgi-1.1.0/LICENSE` & `api_gateway_v2_to_wsgi-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `api_gateway_v2_to_wsgi-1.1.0/README.md` & `api_gateway_v2_to_wsgi-1.1.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-[![Build Status](https://dev.azure.com/asottile/asottile/_apis/build/status/asottile.api-gateway-v2-to-wsgi?branchName=master)](https://dev.azure.com/asottile/asottile/_build/latest?definitionId=65&branchName=master)
-[![Azure DevOps coverage](https://img.shields.io/azure-devops/coverage/asottile/asottile/65/master.svg)](https://dev.azure.com/asottile/asottile/_build/latest?definitionId=65&branchName=master)
-[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/asottile/api-gateway-v2-to-wsgi/master.svg)](https://results.pre-commit.ci/latest/github/asottile/api-gateway-v2-to-wsgi/master)
+[![build status](https://github.com/asottile/api-gateway-v2-to-wsgi/actions/workflows/main.yml/badge.svg)](https://github.com/asottile/api-gateway-v2-to-wsgi/actions/workflows/main.yml)
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/asottile/api-gateway-v2-to-wsgi/main.svg)](https://results.pre-commit.ci/latest/github/asottile/api-gateway-v2-to-wsgi/main)
 
 api-gateway-v2-to-wsgi
 ======================
 
 translation from the aws api gateway v2.0 lambda event to wsgi
 
 ## installation
 
-`pip install api-gateway-v2-to-wsgi`
+```bash
+pip install api-gateway-v2-to-wsgi
+```
 
 ## usage
 
 ```python
 import api_gateway_v2_to_wsgi
 
 from ... import app
@@ -33,8 +34,8 @@
 
 additionally, see the [api gateway documentation] (though it's not very good
 at the time of writing so glhf)
 
 seems the [lambda integration guide] is slightly better
 
 [api gateway documentation]: https://docs.aws.amazon.com/apigateway/index.html
-[lambda integratio guide]: https://docs.aws.amazon.com/apigateway/latest/developerguide/http-api-develop-integrations-lambda.html
+[lambda integration guide]: https://docs.aws.amazon.com/apigateway/latest/developerguide/http-api-develop-integrations-lambda.html
```

### Comparing `api_gateway_v2_to_wsgi-1.1.0/api_gateway_v2_to_wsgi.py` & `api_gateway_v2_to_wsgi-1.1.1/api_gateway_v2_to_wsgi.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,63 +1,62 @@
+from __future__ import annotations
+
 import base64
 import collections
 import io
 import sys
 from types import TracebackType
 from typing import Any
 from typing import Callable
 from typing import Dict
 from typing import Iterable
-from typing import List
-from typing import Optional
 from typing import Protocol
 from typing import Tuple
 from typing import Type
-from typing import Union
 
 _ExcInfo = Tuple[Type[BaseException], BaseException, TracebackType]
 
 
 class _StartResponse(Protocol):
     def __call__(
             self,
             status: str,
-            headers: List[Tuple[str, str]],
-            exc_info: Optional[_ExcInfo] = ...,
-    ) -> Callable[[Union[bytes, bytearray]], Any]:
+            headers: list[tuple[str, str]],
+            exc_info: _ExcInfo | None = ...,
+    ) -> Callable[[bytes | bytearray], Any]:
         ...
 
 
 _App = Callable[[Dict[str, Any], _StartResponse], Iterable[bytes]]
 _Handler = Callable[[Dict[str, Any], Dict[str, Any]], Dict[str, str]]
 
 
 class _Responder:
     def __init__(self) -> None:
         self.status_code = 500
         self.body = io.BytesIO()
-        self.headers: Dict[str, List[str]] = collections.defaultdict(list)
+        self.headers: dict[str, list[str]] = collections.defaultdict(list)
 
     def __call__(
             self,
             status: str,
-            headers: List[Tuple[str, str]],
-            exc_info: Optional[_ExcInfo] = None,
-    ) -> Callable[[Union[bytes, bytearray]], Any]:
+            headers: list[tuple[str, str]],
+            exc_info: _ExcInfo | None = None,
+    ) -> Callable[[bytes | bytearray], Any]:
         if exc_info is not None:
             _, e, tb = exc_info
             raise e.with_traceback(tb)
 
         code, _, _ = status.partition(' ')
         self.status_code = int(code)
         for k, v in headers:
             self.headers[k].append(v)
         return self.body.write
 
-    def response(self) -> Dict[str, Any]:
+    def response(self) -> dict[str, Any]:
         body_b = self.body.getvalue()
         try:
             body = body_b.decode()
             is_base64_encoded = False
         except UnicodeDecodeError:
             body = base64.b64encode(body_b).decode()
             is_base64_encoded = True
@@ -66,23 +65,23 @@
             'isBase64Encoded': is_base64_encoded,
             'statusCode': self.status_code,
             'body': body,
             'headers': {k: ','.join(v) for k, v in self.headers.items()},
         }
 
 
-def _environ(event: Dict[str, Any], context: Dict[str, Any]) -> Dict[str, Any]:
+def _environ(event: dict[str, Any], context: dict[str, Any]) -> dict[str, Any]:
     body = event.get('body', '')
     if event['isBase64Encoded']:
         body_b = base64.b64decode(body)
     else:
         body_b = body.encode()
 
     environ = {
-        'CONTENT_LENGTH': len(body_b),
+        'CONTENT_LENGTH': str(len(body_b)),
         'CONTENT_TYPE': event['headers'].get('content-type', ''),
         # cookies are stripped out of the headers mapping
         'HTTP_COOKIE': ';'.join(event.get('cookies', [])),
         'PATH_INFO': event['rawPath'],
         'QUERY_STRING': event['rawQueryString'],
         'REMOTE_ADDR': event['requestContext']['http']['sourceIp'],
         'REQUEST_METHOD': event['requestContext']['http']['method'],
@@ -105,15 +104,15 @@
         environ[f'HTTP_{k.upper().replace("-", "_")}'] = v
 
     return environ
 
 
 def make_lambda_handler(app: _App) -> _Handler:
     def handler(
-            event: Dict[str, Any],
-            context: Dict[str, Any],
-    ) -> Dict[str, Any]:
+            event: dict[str, Any],
+            context: dict[str, Any],
+    ) -> dict[str, Any]:
         responder = _Responder()
         for data in app(_environ(event, context), responder):
             responder.body.write(data)
         return responder.response()
     return handler
```

### Comparing `api_gateway_v2_to_wsgi-1.1.0/setup.cfg` & `api_gateway_v2_to_wsgi-1.1.1/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 [metadata]
 name = api_gateway_v2_to_wsgi
-version = 1.1.0
+version = 1.1.1
 description = translation from the aws api gateway v2.0 lambda event to wsgi
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/asottile/api-gateway-v2-to-wsgi
 author = Anthony Sottile
 author_email = asottile@umich.edu
 license = MIT
-license_file = LICENSE
+license_files = LICENSE
 classifiers = 
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.8
-	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: Implementation :: CPython
 
 [options]
 py_modules = api_gateway_v2_to_wsgi
 python_requires = >=3.8
 
 [bdist_wheel]
@@ -28,15 +26,16 @@
 plugins = covdefaults
 
 [mypy]
 check_untyped_defs = true
 disallow_any_generics = true
 disallow_incomplete_defs = true
 disallow_untyped_defs = true
-no_implicit_optional = true
+warn_redundant_casts = true
+warn_unused_ignores = true
 
 [mypy-testing.*]
 disallow_untyped_defs = false
 
 [mypy-tests.*]
 disallow_untyped_defs = false
```

