# Comparing `tmp/fastapi_throttling-0.1.5.tar.gz` & `tmp/fastapi_throttling-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_throttling-0.1.5.tar", max compression
+gzip compressed data, was "fastapi_throttling-0.1.6.tar", max compression
```

## Comparing `fastapi_throttling-0.1.5.tar` & `fastapi_throttling-0.1.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    26526 2023-06-13 13:00:44.925756 fastapi_throttling-0.1.5/LICENSE
--rw-r--r--   0        0        0     1347 2023-06-13 13:00:44.925756 fastapi_throttling-0.1.5/README.md
--rw-r--r--   0        0        0     1754 2023-06-13 13:00:44.925756 fastapi_throttling-0.1.5/pyproject.toml
--rw-r--r--   0        0        0       79 2023-06-13 13:00:44.925756 fastapi_throttling-0.1.5/src/fastapi_throttling/__init__.py
--rw-r--r--   0        0        0     2957 2023-06-13 13:00:44.925756 fastapi_throttling-0.1.5/src/fastapi_throttling/throttle.py
--rw-r--r--   0        0        0     1822 1970-01-01 00:00:00.000000 fastapi_throttling-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    26526 2023-06-13 21:18:26.393691 fastapi_throttling-0.1.6/LICENSE
+-rw-r--r--   0        0        0     1347 2023-06-13 21:18:26.393691 fastapi_throttling-0.1.6/README.md
+-rw-r--r--   0        0        0     1753 2023-06-13 21:18:26.393691 fastapi_throttling-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0       79 2023-06-13 21:18:26.393691 fastapi_throttling-0.1.6/src/fastapi_throttling/__init__.py
+-rw-r--r--   0        0        0     2949 2023-06-13 21:18:26.393691 fastapi_throttling-0.1.6/src/fastapi_throttling/throttle.py
+-rw-r--r--   0        0        0     1772 1970-01-01 00:00:00.000000 fastapi_throttling-0.1.6/PKG-INFO
```

### Comparing `fastapi_throttling-0.1.5/LICENSE` & `fastapi_throttling-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_throttling-0.1.5/README.md` & `fastapi_throttling-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_throttling-0.1.5/pyproject.toml` & `fastapi_throttling-0.1.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "fastapi-throttling"
-version = "0.1.5"
+version = "0.1.6"
 description = "Limit amount of requests to your FastAPI."
 authors = ["wwnbb <wwnbb1@gmail.com>"]
 license = "GPLv2"
 readme = "README.md"
 packages = [{include = "fastapi_throttling", from = "src"}]
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = "^3.11.4"
 fastapi = "^0.96.0"
-py-redis = "^1.1.1"
+redis = "^4.5.5"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 black = "^23.3.0"
 mypy = "^1.3.0"
 flake8 = "^6.0.0"
 isort = "^5.12.0"
```

### Comparing `fastapi_throttling-0.1.5/src/fastapi_throttling/throttle.py` & `fastapi_throttling-0.1.6/src/fastapi_throttling/throttle.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from redis import Redis
+from redis.asyncio import Redis
 from starlette.datastructures import Headers
 from starlette.responses import JSONResponse
 from starlette.types import ASGIApp, Receive, Scope, Send
 
 
 class ThrottlingResponse(JSONResponse):
     def __init__(self):
@@ -33,23 +33,21 @@
 
     def __init__(
         self,
         app: ASGIApp,
         limit: int = 100,
         window: int = 60,
         token_header: str = "Authorization",
-        redis: Redis | None = None,
+        redis: Redis = Redis(),
     ) -> None:
         self.app = app
         self.token_header = token_header
         self.limit = limit
         self.window = window
         self.redis = redis
-        if not self.redis:
-            self.redis = Redis()
 
     async def __call__(
         self, scope: Scope, receive: Receive, send: Send
     ) -> None:
         if scope["type"] != "http":
             await self.app(scope, receive, send)
             return
@@ -71,20 +69,22 @@
             await response(scope, receive, send)
             return
 
         await self.app(scope, receive, send)
         return
 
     async def has_exceeded_rate_limit(self, identifier: str) -> bool:
-        current_count = self.redis.get(identifier)
+        current_count = await self.redis.get(identifier)
 
         if current_count is None:
             # This is the first request with this identifier within the window
-            self.redis.set(identifier, 1, ex=self.window)  # Start a new window
+            await self.redis.set(
+                identifier, 1, ex=self.window
+            )  # Start a new window
             return False
 
         if int(current_count) < self.limit:
             # Increase the request count
-            self.redis.incr(identifier)
+            await self.redis.incr(identifier)
             return False
 
         return True
```

### Comparing `fastapi_throttling-0.1.5/PKG-INFO` & `fastapi_throttling-0.1.6/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: fastapi-throttling
-Version: 0.1.5
+Version: 0.1.6
 Summary: Limit amount of requests to your FastAPI.
 License: GPLv2
 Author: wwnbb
 Author-email: wwnbb1@gmail.com
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.11.4,<4.0.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: fastapi (>=0.96.0,<0.97.0)
-Requires-Dist: py-redis (>=1.1.1,<2.0.0)
+Requires-Dist: redis (>=4.5.5,<5.0.0)
 Description-Content-Type: text/markdown
 
 [![Upload Python Package](https://github.com/wwnbb/fastapi-throttling/actions/workflows/publish.yml/badge.svg?branch=master)](https://github.com/wwnbb/fastapi-throttling/actions/workflows/publish.yml)
 
 ## FastAPI Throttling Middleware
 
 FastAPI Throttling Middleware is a rate-limiting middleware for the FastAPI web framework. It uses a Redis server for request tracking and allows you to throttle incoming requests based on IP address and access token.
```

