# Comparing `tmp/kraky-2023.2.22.tar.gz` & `tmp/kraky-2023.6.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kraky-2023.2.22.tar", max compression
+gzip compressed data, was "kraky-2023.6.13.tar", max compression
```

## Comparing `kraky-2023.2.22.tar` & `kraky-2023.6.13.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     1069 2023-02-22 01:00:03.954280 kraky-2023.2.22/LICENSE
--rw-r--r--   0        0        0     3496 2023-02-22 01:00:03.954280 kraky-2023.2.22/README.md
--rw-r--r--   0        0        0      123 2023-02-22 01:00:03.954280 kraky-2023.2.22/kraky/__init__.py
--rw-r--r--   0        0        0    48358 2023-02-22 01:00:03.954280 kraky-2023.2.22/kraky/api.py
--rw-r--r--   0        0        0     1598 2023-02-22 01:00:03.954280 kraky-2023.2.22/kraky/cli.py
--rw-r--r--   0        0        0      471 2023-02-22 01:00:03.954280 kraky-2023.2.22/kraky/log.py
--rw-r--r--   0        0        0        1 2023-02-22 01:00:03.954280 kraky-2023.2.22/kraky/py.typed
--rw-r--r--   0        0        0    12560 2023-02-22 01:00:03.954280 kraky-2023.2.22/kraky/ws.py
--rw-r--r--   0        0        0     1067 2023-02-22 01:00:03.954280 kraky-2023.2.22/pyproject.toml
--rw-r--r--   0        0        0     4583 1970-01-01 00:00:00.000000 kraky-2023.2.22/setup.py
--rw-r--r--   0        0        0     4591 1970-01-01 00:00:00.000000 kraky-2023.2.22/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-13 10:34:50.829974 kraky-2023.6.13/LICENSE
+-rw-r--r--   0        0        0     3496 2023-06-13 10:34:50.829974 kraky-2023.6.13/README.md
+-rw-r--r--   0        0        0      123 2023-06-13 10:34:50.829974 kraky-2023.6.13/kraky/__init__.py
+-rw-r--r--   0        0        0    48358 2023-06-13 10:34:50.829974 kraky-2023.6.13/kraky/api.py
+-rw-r--r--   0        0        0     1598 2023-06-13 10:34:50.829974 kraky-2023.6.13/kraky/cli.py
+-rw-r--r--   0        0        0      471 2023-06-13 10:34:50.829974 kraky-2023.6.13/kraky/log.py
+-rw-r--r--   0        0        0        1 2023-06-13 10:34:50.829974 kraky-2023.6.13/kraky/py.typed
+-rw-r--r--   0        0        0    12560 2023-06-13 10:34:50.829974 kraky-2023.6.13/kraky/ws.py
+-rw-r--r--   0        0        0     1098 2023-06-13 10:34:50.829974 kraky-2023.6.13/pyproject.toml
+-rw-r--r--   0        0        0     4490 1970-01-01 00:00:00.000000 kraky-2023.6.13/PKG-INFO
```

### Comparing `kraky-2023.2.22/LICENSE` & `kraky-2023.6.13/LICENSE`

 * *Files identical despite different names*

### Comparing `kraky-2023.2.22/README.md` & `kraky-2023.6.13/README.md`

 * *Files identical despite different names*

### Comparing `kraky-2023.2.22/kraky/api.py` & `kraky-2023.6.13/kraky/api.py`

 * *Files identical despite different names*

### Comparing `kraky-2023.2.22/kraky/cli.py` & `kraky-2023.6.13/kraky/cli.py`

 * *Files identical despite different names*

### Comparing `kraky-2023.2.22/kraky/ws.py` & `kraky-2023.6.13/kraky/ws.py`

 * *Files identical despite different names*

### Comparing `kraky-2023.2.22/pyproject.toml` & `kraky-2023.6.13/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kraky"
-version = "2023.02.22"
+version = "2023.06.13"
 description = "Python client for Kraken API REST and Kraken Websockets API using httpx and websockets. Supports both sync and async for API REST."
 authors = ["Atem18 <contact@atemlire.io>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://kraky.readthedocs.io/en/latest"
 repository = "https://github.com/Atem18/kraky"
 keywords = ["asyncio", "httpx", "websockets", "kraken"]
@@ -12,27 +12,27 @@
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
-httpx = "^0.23.3"
-websockets = "^10.4"
-typer = {extras = ["all"], version = "^0.7.0"}
+httpx = ">=0.23.3,<0.25.0"
+websockets = ">=10.4,<12.0"
+typer = {extras = ["all"], version = ">=0.7,<0.10"}
 python-dotenv = "^0.21.1"
 
 [tool.poetry.scripts]
 kraky = 'kraky.cli:app'
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.0.0"
-pytest-asyncio = "^0.20.0"
+pytest-asyncio = ">=0.20,<0.22"
 mkdocs = "^1.2.2"
 mkdocs-material = "^9.0.0"
-mkdocstrings = "^0.19.0"
+mkdocstrings = ">=0.19,<0.23"
 black = "^23.1.0"
 tox = "^4.4.6"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `kraky-2023.2.22/PKG-INFO` & `kraky-2023.6.13/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 Metadata-Version: 2.1
 Name: kraky
-Version: 2023.2.22
+Version: 2023.6.13
 Summary: Python client for Kraken API REST and Kraken Websockets API using httpx and websockets. Supports both sync and async for API REST.
 Home-page: https://kraky.readthedocs.io/en/latest
 License: MIT
 Keywords: asyncio,httpx,websockets,kraken
 Author: Atem18
 Author-email: contact@atemlire.io
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Requires-Dist: httpx (>=0.23.3,<0.24.0)
+Requires-Dist: httpx (>=0.23.3,<0.25.0)
 Requires-Dist: python-dotenv (>=0.21.1,<0.22.0)
-Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
-Requires-Dist: websockets (>=10.4,<11.0)
+Requires-Dist: typer[all] (>=0.7,<0.10)
+Requires-Dist: websockets (>=10.4,<12.0)
 Project-URL: Repository, https://github.com/Atem18/kraky
 Description-Content-Type: text/markdown
 
 # Kraky
 Python client for Kraken API REST and Kraken Websockets API using httpx and websockets.
 Supports both sync and async for API REST.
```

