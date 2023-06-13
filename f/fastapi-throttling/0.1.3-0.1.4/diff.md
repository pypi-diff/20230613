# Comparing `tmp/fastapi_throttling-0.1.3.tar.gz` & `tmp/fastapi_throttling-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_throttling-0.1.3.tar", max compression
+gzip compressed data, was "fastapi_throttling-0.1.4.tar", max compression
```

## Comparing `fastapi_throttling-0.1.3.tar` & `fastapi_throttling-0.1.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    26526 2023-06-13 07:34:09.687722 fastapi_throttling-0.1.3/LICENSE
--rw-r--r--   0        0        0     1347 2023-06-13 07:34:09.687722 fastapi_throttling-0.1.3/README.md
--rw-r--r--   0        0        0     1779 2023-06-13 07:34:09.687722 fastapi_throttling-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       79 2023-06-13 07:34:09.687722 fastapi_throttling-0.1.3/src/fastapi_throttling/__init__.py
--rw-r--r--   0        0        0     3068 2023-06-13 07:34:09.687722 fastapi_throttling-0.1.3/src/fastapi_throttling/throttle.py
--rw-r--r--   0        0        0     1822 1970-01-01 00:00:00.000000 fastapi_throttling-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    26526 2023-06-13 12:47:19.739928 fastapi_throttling-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1347 2023-06-13 12:47:19.739928 fastapi_throttling-0.1.4/README.md
+-rw-r--r--   0        0        0     1779 2023-06-13 12:47:19.739928 fastapi_throttling-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0       79 2023-06-13 12:47:19.739928 fastapi_throttling-0.1.4/src/fastapi_throttling/__init__.py
+-rw-r--r--   0        0        0     2957 2023-06-13 12:47:19.739928 fastapi_throttling-0.1.4/src/fastapi_throttling/throttle.py
+-rw-r--r--   0        0        0     1822 1970-01-01 00:00:00.000000 fastapi_throttling-0.1.4/PKG-INFO
```

### Comparing `fastapi_throttling-0.1.3/LICENSE` & `fastapi_throttling-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_throttling-0.1.3/README.md` & `fastapi_throttling-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_throttling-0.1.3/pyproject.toml` & `fastapi_throttling-0.1.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "fastapi-throttling"
-version = "0.1.3"
+version = "0.1.4"
 description = "Limit amount of requests to your FastAPI."
 authors = ["wwnbb <wwnbb1@gmail.com>"]
 license = "GPLv2"
 readme = "README.md"
 packages = [{include = "fastapi_throttling", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
-fastapi = "^0.96.0"
+fastapi = "^0.94.0"
 py-redis = "^1.1.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 black = "^23.3.0"
 mypy = "^1.3.0"
 flake8 = "^6.0.0"
```

### Comparing `fastapi_throttling-0.1.3/src/fastapi_throttling/throttle.py` & `fastapi_throttling-0.1.4/src/fastapi_throttling/throttle.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,12 @@
-from typing import Any, Awaitable
-
-from redis.asyncio import Redis
+from redis import Redis
 from starlette.datastructures import Headers
 from starlette.responses import JSONResponse
 from starlette.types import ASGIApp, Receive, Scope, Send
 
-ResponseT = Awaitable | Any
-
 
 class ThrottlingResponse(JSONResponse):
     def __init__(self):
         content = {"detail": "Too Many Requests"}
         status_code = 429
         super().__init__(status_code=status_code, content=content)
 
@@ -43,27 +39,26 @@
         token_header: str = "Authorization",
         redis: Redis | None = None,
     ) -> None:
         self.app = app
         self.token_header = token_header
         self.limit = limit
         self.window = window
-        if redis:
-            self.redis = redis
-        else:
+        self.redis = redis
+        if not self.redis:
             self.redis = Redis()
 
     async def __call__(
         self, scope: Scope, receive: Receive, send: Send
     ) -> None:
         if scope["type"] != "http":
             await self.app(scope, receive, send)
+            return
 
         headers = Headers(scope=scope)
-
         client_ip = headers.get(
             "x-forwarded-for", next(iter(scope["client"][0]), None)
         )
         # Throttle by IP
         if client_ip and await self.has_exceeded_rate_limit(client_ip):
             response = ThrottlingResponse()
             await response(scope, receive, send)
@@ -76,22 +71,20 @@
             await response(scope, receive, send)
             return
 
         await self.app(scope, receive, send)
         return
 
     async def has_exceeded_rate_limit(self, identifier: str) -> bool:
-        current_count = await self.redis.get(identifier)
+        current_count = self.redis.get(identifier)
 
         if current_count is None:
             # This is the first request with this identifier within the window
-            await self.redis.set(
-                identifier, 1, ex=self.window
-            )  # Start a new window
+            self.redis.set(identifier, 1, ex=self.window)  # Start a new window
             return False
 
         if int(current_count) < self.limit:
             # Increase the request count
-            await self.redis.incr(identifier)
+            self.redis.incr(identifier)
             return False
 
         return True
```

### Comparing `fastapi_throttling-0.1.3/PKG-INFO` & `fastapi_throttling-0.1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: fastapi-throttling
-Version: 0.1.3
+Version: 0.1.4
 Summary: Limit amount of requests to your FastAPI.
 License: GPLv2
 Author: wwnbb
 Author-email: wwnbb1@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: fastapi (>=0.96.0,<0.97.0)
+Requires-Dist: fastapi (>=0.94.0,<0.95.0)
 Requires-Dist: py-redis (>=1.1.1,<2.0.0)
 Description-Content-Type: text/markdown
 
 [![Upload Python Package](https://github.com/wwnbb/fastapi-throttling/actions/workflows/publish.yml/badge.svg?branch=master)](https://github.com/wwnbb/fastapi-throttling/actions/workflows/publish.yml)
 
 ## FastAPI Throttling Middleware
```

