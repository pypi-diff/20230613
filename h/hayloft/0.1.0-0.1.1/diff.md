# Comparing `tmp/hayloft-0.1.0.tar.gz` & `tmp/hayloft-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hayloft-0.1.0.tar", max compression
+gzip compressed data, was "hayloft-0.1.1.tar", max compression
```

## Comparing `hayloft-0.1.0.tar` & `hayloft-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1074 2023-06-13 15:27:24.809402 hayloft-0.1.0/LICENSE
--rw-r--r--   0        0        0      119 2023-06-13 15:27:19.792693 hayloft-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-06-13 15:23:56.017734 hayloft-0.1.0/hayloft/__init__.py
--rw-r--r--   0        0        0     2919 2023-06-13 15:37:36.198421 hayloft-0.1.0/hayloft/app.py
--rw-r--r--   0        0        0      422 2023-06-13 15:36:14.597620 hayloft-0.1.0/hayloft/logger.py
--rw-r--r--   0        0        0    18046 2023-06-13 15:26:59.212520 hayloft-0.1.0/hayloft/public/assets/index-144454fa.css
--rw-r--r--   0        0        0   174554 2023-06-13 15:26:59.215854 hayloft-0.1.0/hayloft/public/assets/index-efbd5a31.js
--rw-r--r--   0        0        0      442 2023-06-13 15:26:59.215854 hayloft-0.1.0/hayloft/public/index.html
--rw-r--r--   0        0        0     1367 2023-06-13 15:26:48.605765 hayloft-0.1.0/hayloft/schema.py
--rw-r--r--   0        0        0      478 2023-06-13 15:42:11.427841 hayloft-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      768 1970-01-01 00:00:00.000000 hayloft-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-06-13 15:27:24.809402 hayloft-0.1.1/LICENSE
+-rw-r--r--   0        0        0      119 2023-06-13 15:27:19.792693 hayloft-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-13 15:23:56.017734 hayloft-0.1.1/hayloft/__init__.py
+-rw-r--r--   0        0        0     2927 2023-06-13 15:55:20.682631 hayloft-0.1.1/hayloft/app.py
+-rw-r--r--   0        0        0      422 2023-06-13 15:36:14.597620 hayloft-0.1.1/hayloft/logger.py
+-rw-r--r--   0        0        0    18046 2023-06-13 15:26:59.212520 hayloft-0.1.1/hayloft/public/assets/index-144454fa.css
+-rw-r--r--   0        0        0   174554 2023-06-13 15:26:59.215854 hayloft-0.1.1/hayloft/public/assets/index-efbd5a31.js
+-rw-r--r--   0        0        0      442 2023-06-13 15:26:59.215854 hayloft-0.1.1/hayloft/public/index.html
+-rw-r--r--   0        0        0     1367 2023-06-13 15:26:48.605765 hayloft-0.1.1/hayloft/schema.py
+-rw-r--r--   0        0        0      432 2023-06-13 15:56:10.626484 hayloft-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      703 1970-01-01 00:00:00.000000 hayloft-0.1.1/PKG-INFO
```

### Comparing `hayloft-0.1.0/LICENSE` & `hayloft-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hayloft-0.1.0/hayloft/app.py` & `hayloft-0.1.1/hayloft/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from flask import request, jsonify, send_file, send_from_directory, Response, cli
 from flask_cors import CORS
-from schema import app, db, sse, Event, Session
+from hayloft.schema import app, db, sse, Event, Session
 import time
 
 CORS(app)  # for development
 cli.show_server_banner = lambda *x: None
 
 
 @app.route("/", methods=["GET"])
```

### Comparing `hayloft-0.1.0/hayloft/public/assets/index-144454fa.css` & `hayloft-0.1.1/hayloft/public/assets/index-144454fa.css`

 * *Files identical despite different names*

### Comparing `hayloft-0.1.0/hayloft/public/assets/index-efbd5a31.js` & `hayloft-0.1.1/hayloft/public/assets/index-efbd5a31.js`

 * *Files identical despite different names*

### Comparing `hayloft-0.1.0/hayloft/schema.py` & `hayloft-0.1.1/hayloft/schema.py`

 * *Files identical despite different names*

### Comparing `hayloft-0.1.0/PKG-INFO` & `hayloft-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 Metadata-Version: 2.1
 Name: hayloft
-Version: 0.1.0
+Version: 0.1.1
 Summary: UI tool for LLM frameworks
 License: MIT
-Author: Eugene Turchenkov
-Author-email: e.a.turchenkov@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: flask (>=2.3.2,<3.0.0)
 Requires-Dist: flask-cors (>=3.0.10,<4.0.0)
```

