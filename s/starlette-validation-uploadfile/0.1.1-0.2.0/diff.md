# Comparing `tmp/starlette-validation-uploadfile-0.1.1.tar.gz` & `tmp/starlette-validation-uploadfile-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starlette-validation-uploadfile-0.1.1.tar", last modified: Mon Oct 25 03:49:43 2021, max compression
+gzip compressed data, was "starlette-validation-uploadfile-0.2.0.tar", last modified: Tue Jun 13 13:56:16 2023, max compression
```

## Comparing `starlette-validation-uploadfile-0.1.1.tar` & `starlette-validation-uploadfile-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,16 @@
-drwxrwxr-x   0 terib0l   (1000) terib0l   (1000)        0 2021-10-25 03:49:43.712698 starlette-validation-uploadfile-0.1.1/
--rw-rw-r--   0 terib0l   (1000) terib0l   (1000)     2538 2021-10-25 03:49:43.712698 starlette-validation-uploadfile-0.1.1/PKG-INFO
--rw-rw-r--   0 terib0l   (1000) terib0l   (1000)     1426 2021-10-25 03:35:21.000000 starlette-validation-uploadfile-0.1.1/README.md
--rw-rw-r--   0 terib0l   (1000) terib0l   (1000)       38 2021-10-25 03:49:43.712698 starlette-validation-uploadfile-0.1.1/setup.cfg
--rw-rw-r--   0 terib0l   (1000) terib0l   (1000)     1021 2021-10-25 03:31:25.000000 starlette-validation-uploadfile-0.1.1/setup.py
-drwxrwxr-x   0 terib0l   (1000) terib0l   (1000)        0 2021-10-25 03:49:43.712698 starlette-validation-uploadfile-0.1.1/starlette_validation_uploadfile.egg-info/
--rw-rw-r--   0 terib0l   (1000) terib0l   (1000)     2538 2021-10-25 03:49:43.000000 starlette-validation-uploadfile-0.1.1/starlette_validation_uploadfile.egg-info/PKG-INFO
--rw-rw-r--   0 terib0l   (1000) terib0l   (1000)      327 2021-10-25 03:49:43.000000 starlette-validation-uploadfile-0.1.1/starlette_validation_uploadfile.egg-info/SOURCES.txt
--rw-rw-r--   0 terib0l   (1000) terib0l   (1000)        1 2021-10-25 03:49:43.000000 starlette-validation-uploadfile-0.1.1/starlette_validation_uploadfile.egg-info/dependency_links.txt
--rw-rw-r--   0 terib0l   (1000) terib0l   (1000)       19 2021-10-25 03:49:43.000000 starlette-validation-uploadfile-0.1.1/starlette_validation_uploadfile.egg-info/requires.txt
--rw-rw-r--   0 terib0l   (1000) terib0l   (1000)       32 2021-10-25 03:49:43.000000 starlette-validation-uploadfile-0.1.1/starlette_validation_uploadfile.egg-info/top_level.txt
--rw-rw-r--   0 terib0l   (1000) terib0l   (1000)     1886 2021-10-25 03:18:11.000000 starlette-validation-uploadfile-0.1.1/starlette_validation_uploadfile.py
+drwxrwxr-x   0 terib0l   (1000) terib0l   (1000)        0 2023-06-13 13:56:16.503878 starlette-validation-uploadfile-0.2.0/
+-rw-rw-r--   0 terib0l   (1000) terib0l   (1000)     1064 2021-11-30 16:58:35.000000 starlette-validation-uploadfile-0.2.0/LICENSE
+-rw-rw-r--   0 terib0l   (1000) terib0l   (1000)     2399 2023-06-13 13:56:16.503878 starlette-validation-uploadfile-0.2.0/PKG-INFO
+-rw-rw-r--   0 terib0l   (1000) terib0l   (1000)     1692 2023-06-13 13:02:01.000000 starlette-validation-uploadfile-0.2.0/README.md
+-rw-rw-r--   0 terib0l   (1000) terib0l   (1000)      669 2023-06-13 12:56:20.000000 starlette-validation-uploadfile-0.2.0/pyproject.toml
+-rw-rw-r--   0 terib0l   (1000) terib0l   (1000)       38 2023-06-13 13:56:16.503878 starlette-validation-uploadfile-0.2.0/setup.cfg
+-rw-rw-r--   0 terib0l   (1000) terib0l   (1000)     1021 2023-06-13 13:56:02.000000 starlette-validation-uploadfile-0.2.0/setup.py
+drwxrwxr-x   0 terib0l   (1000) terib0l   (1000)        0 2023-06-13 13:56:16.503878 starlette-validation-uploadfile-0.2.0/starlette_validation_uploadfile.egg-info/
+-rw-rw-r--   0 terib0l   (1000) terib0l   (1000)     2399 2023-06-13 13:56:16.000000 starlette-validation-uploadfile-0.2.0/starlette_validation_uploadfile.egg-info/PKG-INFO
+-rw-rw-r--   0 terib0l   (1000) terib0l   (1000)      368 2023-06-13 13:56:16.000000 starlette-validation-uploadfile-0.2.0/starlette_validation_uploadfile.egg-info/SOURCES.txt
+-rw-rw-r--   0 terib0l   (1000) terib0l   (1000)        1 2023-06-13 13:56:16.000000 starlette-validation-uploadfile-0.2.0/starlette_validation_uploadfile.egg-info/dependency_links.txt
+-rw-rw-r--   0 terib0l   (1000) terib0l   (1000)       19 2023-06-13 13:56:16.000000 starlette-validation-uploadfile-0.2.0/starlette_validation_uploadfile.egg-info/requires.txt
+-rw-rw-r--   0 terib0l   (1000) terib0l   (1000)       32 2023-06-13 13:56:16.000000 starlette-validation-uploadfile-0.2.0/starlette_validation_uploadfile.egg-info/top_level.txt
+-rw-rw-r--   0 terib0l   (1000) terib0l   (1000)     2759 2023-06-13 13:00:25.000000 starlette-validation-uploadfile-0.2.0/starlette_validation_uploadfile.py
+drwxrwxr-x   0 terib0l   (1000) terib0l   (1000)        0 2023-06-13 13:56:16.503878 starlette-validation-uploadfile-0.2.0/test/
+-rw-rw-r--   0 terib0l   (1000) terib0l   (1000)     2793 2023-06-13 13:52:58.000000 starlette-validation-uploadfile-0.2.0/test/test_main.py
```

### Comparing `starlette-validation-uploadfile-0.1.1/README.md` & `starlette-validation-uploadfile-0.2.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 # starlette-validation-uploadfile
 
-***--- Now, in progress. ---***
-
-[![PyPI](https://img.shields.io/pypi/v/starlette-validation-uploadfile?color=orange)](https://pypi.org/project/starlette-validation-uploadfile/)
-[![License](https://img.shields.io/github/license/terib0l/starlette-validation-uploadfile)](https://github.com/terib0l/starlette-validation-uploadfile/blob/main/LICENSE)
+![PyPI](https://img.shields.io/pypi/v/starlette-validation-uploadfile?color=orange)
+![License](https://img.shields.io/github/license/terib0l/starlette-validation-uploadfile)
 
 Middleware for validation upload-file in FastAPI and Starlette.
 
 ## Installation
 
 ```bash
 pip install starlette-validation-uploadfile
@@ -28,25 +26,41 @@
 
 from starlette_validation_uploadfile import ValidateUploadFileMiddleware
 
 app = FastAPI()
 
 app.add_middleware(
         ValidateUploadFileMiddleware,
-        app_path="/upload/",
-        max_size=120000,
+        app_path=[
+            "/upload/first",
+            "/upload/second",
+        ],
+        max_size=16777216,
         file_type=["image/png", "image/jpeg"]
 )
 
-@app.post("/upload/")
-def upload_file(request: Request, file: UploadFile = File(...)):
-    form = request.form()
+@app.post("/upload/first")
+async def upload_file(request: Request, file: UploadFile = File(...)):
+    form = await request.form()
+    content_type = form[next(iter(form))].content_type
+
+    size = request.headers["content-length"]
+
+    return {
+        "filename": file.filename,
+        "content_type": content_type,
+        "file_size": size,
+    }
+
+@app.post("/upload/second")
+async def upload_file_second(request: Request, file: UploadFile = File(...)):
+    form = await request.form()
     content_type = form[next(iter(form))].content_type
 
     size = request.headers["content-length"]
 
     return {
         "filename": file.filename,
         "content_type": content_type,
-        "file_size": size
+        "file_size": size,
     }
 ```
```

### Comparing `starlette-validation-uploadfile-0.1.1/setup.py` & `starlette-validation-uploadfile-0.2.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-VERSION = "0.1.1"
+VERSION = "0.2.0"
 
 def get_long_description():
     with open("README.md", encoding="utf8") as f:
         return f.read()
 
 setup(
     name="starlette-validation-uploadfile",
```

