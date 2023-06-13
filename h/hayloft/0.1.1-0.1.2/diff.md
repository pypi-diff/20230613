# Comparing `tmp/hayloft-0.1.1.tar.gz` & `tmp/hayloft-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hayloft-0.1.1.tar", max compression
+gzip compressed data, was "hayloft-0.1.2.tar", max compression
```

## Comparing `hayloft-0.1.1.tar` & `hayloft-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1074 2023-06-13 15:27:24.809402 hayloft-0.1.1/LICENSE
--rw-r--r--   0        0        0      119 2023-06-13 15:27:19.792693 hayloft-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-06-13 15:23:56.017734 hayloft-0.1.1/hayloft/__init__.py
--rw-r--r--   0        0        0     2927 2023-06-13 15:55:20.682631 hayloft-0.1.1/hayloft/app.py
--rw-r--r--   0        0        0      422 2023-06-13 15:36:14.597620 hayloft-0.1.1/hayloft/logger.py
--rw-r--r--   0        0        0    18046 2023-06-13 15:26:59.212520 hayloft-0.1.1/hayloft/public/assets/index-144454fa.css
--rw-r--r--   0        0        0   174554 2023-06-13 15:26:59.215854 hayloft-0.1.1/hayloft/public/assets/index-efbd5a31.js
--rw-r--r--   0        0        0      442 2023-06-13 15:26:59.215854 hayloft-0.1.1/hayloft/public/index.html
--rw-r--r--   0        0        0     1367 2023-06-13 15:26:48.605765 hayloft-0.1.1/hayloft/schema.py
--rw-r--r--   0        0        0      432 2023-06-13 15:56:10.626484 hayloft-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      703 1970-01-01 00:00:00.000000 hayloft-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-06-13 15:27:24.809402 hayloft-0.1.2/LICENSE
+-rw-r--r--   0        0        0      119 2023-06-13 15:27:19.792693 hayloft-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-06-13 15:23:56.017734 hayloft-0.1.2/hayloft/__init__.py
+-rw-r--r--   0        0        0     3185 2023-06-13 17:03:36.638281 hayloft-0.1.2/hayloft/app.py
+-rw-r--r--   0        0        0      455 2023-06-13 17:02:40.814396 hayloft-0.1.2/hayloft/logger.py
+-rw-r--r--   0        0        0    18046 2023-06-13 15:26:59.212520 hayloft-0.1.2/hayloft/public/assets/index-144454fa.css
+-rw-r--r--   0        0        0   174554 2023-06-13 15:26:59.215854 hayloft-0.1.2/hayloft/public/assets/index-efbd5a31.js
+-rw-r--r--   0        0        0      442 2023-06-13 15:26:59.215854 hayloft-0.1.2/hayloft/public/index.html
+-rw-r--r--   0        0        0     1367 2023-06-13 15:26:48.605765 hayloft-0.1.2/hayloft/schema.py
+-rw-r--r--   0        0        0      430 2023-06-13 17:03:43.625017 hayloft-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      703 1970-01-01 00:00:00.000000 hayloft-0.1.2/PKG-INFO
```

### Comparing `hayloft-0.1.1/LICENSE` & `hayloft-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hayloft-0.1.1/hayloft/app.py` & `hayloft-0.1.2/hayloft/app.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from flask import request, jsonify, send_file, send_from_directory, Response, cli
 from flask_cors import CORS
 from hayloft.schema import app, db, sse, Event, Session
+import argparse
 import time
 
 CORS(app)  # for development
 cli.show_server_banner = lambda *x: None
 
 
 @app.route("/", methods=["GET"])
@@ -100,9 +101,14 @@
         while True:
             msg = messages.get()
             yield msg
 
     return Response(stream(), mimetype="text/event-stream")
 
 
-def start():
-    app.run(host="localhost", port=7000, debug=False)
+def cli():
+    parser = argparse.ArgumentParser(description="Hayloft - UI tool for LLM frameworks")
+    parser.add_argument("command", type=str, help="command to run", choices=["start"])
+    args = parser.parse_args()
+
+    if args.command == "start":
+        app.run(host="localhost", port=7000, debug=False)
```

### Comparing `hayloft-0.1.1/hayloft/public/assets/index-144454fa.css` & `hayloft-0.1.2/hayloft/public/assets/index-144454fa.css`

 * *Files identical despite different names*

### Comparing `hayloft-0.1.1/hayloft/public/assets/index-efbd5a31.js` & `hayloft-0.1.2/hayloft/public/assets/index-efbd5a31.js`

 * *Files identical despite different names*

### Comparing `hayloft-0.1.1/hayloft/schema.py` & `hayloft-0.1.2/hayloft/schema.py`

 * *Files identical despite different names*

### Comparing `hayloft-0.1.1/PKG-INFO` & `hayloft-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hayloft
-Version: 0.1.1
+Version: 0.1.2
 Summary: UI tool for LLM frameworks
 License: MIT
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

