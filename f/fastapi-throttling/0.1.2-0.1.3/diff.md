# Comparing `tmp/fastapi_throttling-0.1.2.tar.gz` & `tmp/fastapi_throttling-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_throttling-0.1.2.tar", max compression
+gzip compressed data, was "fastapi_throttling-0.1.3.tar", max compression
```

## Comparing `fastapi_throttling-0.1.2.tar` & `fastapi_throttling-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    26526 2023-06-12 21:39:39.132727 fastapi_throttling-0.1.2/LICENSE
--rw-r--r--   0        0        0     1343 2023-06-12 21:39:39.132727 fastapi_throttling-0.1.2/README.md
--rw-r--r--   0        0        0     1803 2023-06-12 21:39:39.132727 fastapi_throttling-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       79 2023-06-12 21:39:39.132727 fastapi_throttling-0.1.2/src/fastapi_throttling/__init__.py
--rw-r--r--   0        0        0     3068 2023-06-12 21:39:39.132727 fastapi_throttling-0.1.2/src/fastapi_throttling/throttle.py
--rw-r--r--   0        0        0     1818 1970-01-01 00:00:00.000000 fastapi_throttling-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    26526 2023-06-13 07:34:09.687722 fastapi_throttling-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1347 2023-06-13 07:34:09.687722 fastapi_throttling-0.1.3/README.md
+-rw-r--r--   0        0        0     1779 2023-06-13 07:34:09.687722 fastapi_throttling-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       79 2023-06-13 07:34:09.687722 fastapi_throttling-0.1.3/src/fastapi_throttling/__init__.py
+-rw-r--r--   0        0        0     3068 2023-06-13 07:34:09.687722 fastapi_throttling-0.1.3/src/fastapi_throttling/throttle.py
+-rw-r--r--   0        0        0     1822 1970-01-01 00:00:00.000000 fastapi_throttling-0.1.3/PKG-INFO
```

### Comparing `fastapi_throttling-0.1.2/LICENSE` & `fastapi_throttling-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_throttling-0.1.2/README.md` & `fastapi_throttling-0.1.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 Usage
 
 Here's a basic example of how to use the middleware:
 
 ```python
 
 from fastapi import FastAPI, Request, HTTPException
-from middleware_lib import ThrottlingMiddleware
+from fastapi_throttling import ThrottlingMiddleware
 
 app = FastAPI()
 app.add_middleware(ThrottlingMiddleware, limit=100, window=60)
 ```
 
 In this example, the middleware will limit to 100 requests per 60 seconds, either by IP or by user token.
```

### Comparing `fastapi_throttling-0.1.2/pyproject.toml` & `fastapi_throttling-0.1.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastapi-throttling"
-version = "0.1.2"
+version = "0.1.3"
 description = "Limit amount of requests to your FastAPI."
 authors = ["wwnbb <wwnbb1@gmail.com>"]
 license = "GPLv2"
 readme = "README.md"
 packages = [{include = "fastapi_throttling", from = "src"}]
 
 [tool.poetry.dependencies]
@@ -15,15 +15,14 @@
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 black = "^23.3.0"
 mypy = "^1.3.0"
 flake8 = "^6.0.0"
 isort = "^5.12.0"
 httpx = "^0.24.1"
-pytest-redis = "^3.0.2"
 debugpy = "^1.6.7"
 types-redis = "^4.5.5.2"
 pytest-asyncio = "^0.21.0"
 asgi-lifespan = "^2.1.0"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `fastapi_throttling-0.1.2/src/fastapi_throttling/throttle.py` & `fastapi_throttling-0.1.3/src/fastapi_throttling/throttle.py`

 * *Files identical despite different names*

### Comparing `fastapi_throttling-0.1.2/PKG-INFO` & `fastapi_throttling-0.1.3/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-throttling
-Version: 0.1.2
+Version: 0.1.3
 Summary: Limit amount of requests to your FastAPI.
 License: GPLv2
 Author: wwnbb
 Author-email: wwnbb1@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -40,15 +40,15 @@
 Usage
 
 Here's a basic example of how to use the middleware:
 
 ```python
 
 from fastapi import FastAPI, Request, HTTPException
-from middleware_lib import ThrottlingMiddleware
+from fastapi_throttling import ThrottlingMiddleware
 
 app = FastAPI()
 app.add_middleware(ThrottlingMiddleware, limit=100, window=60)
 ```
 
 In this example, the middleware will limit to 100 requests per 60 seconds, either by IP or by user token.
```

