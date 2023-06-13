# Comparing `tmp/vedro-httpx-0.1.1.tar.gz` & `tmp/vedro-httpx-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vedro-httpx-0.1.1.tar", last modified: Mon Jun 12 15:51:48 2023, max compression
+gzip compressed data, was "vedro-httpx-0.1.2.tar", last modified: Tue Jun 13 15:51:52 2023, max compression
```

## Comparing `vedro-httpx-0.1.1.tar` & `vedro-httpx-0.1.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:51:48.609881 vedro-httpx-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-12 15:51:36.000000 vedro-httpx-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-06-12 15:51:48.609881 vedro-httpx-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-06-12 15:51:36.000000 vedro-httpx-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-06-12 15:51:48.613881 vedro-httpx-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-12 15:51:36.000000 vedro-httpx-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:51:48.609881 vedro-httpx-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-12 15:51:36.000000 vedro-httpx-0.1.1/tests/test_async_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-06-12 15:51:36.000000 vedro-httpx-0.1.1/tests/test_format_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-12 15:51:36.000000 vedro-httpx-0.1.1/tests/test_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-12 15:51:36.000000 vedro-httpx-0.1.1/tests/test_sync_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:51:48.609881 vedro-httpx-0.1.1/vedro_httpx/
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-12 15:51:36.000000 vedro-httpx-0.1.1/vedro_httpx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-06-12 15:51:36.000000 vedro-httpx-0.1.1/vedro_httpx/_async_http_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-06-12 15:51:36.000000 vedro-httpx-0.1.1/vedro_httpx/_render_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-12 15:51:36.000000 vedro-httpx-0.1.1/vedro_httpx/_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-06-12 15:51:36.000000 vedro-httpx-0.1.1/vedro_httpx/_sync_http_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-12 15:51:36.000000 vedro-httpx-0.1.1/vedro_httpx/_vedro_httpx.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:51:36.000000 vedro-httpx-0.1.1/vedro_httpx/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:51:48.609881 vedro-httpx-0.1.1/vedro_httpx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-06-12 15:51:48.000000 vedro-httpx-0.1.1/vedro_httpx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-12 15:51:48.000000 vedro-httpx-0.1.1/vedro_httpx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 15:51:48.000000 vedro-httpx-0.1.1/vedro_httpx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-12 15:51:48.000000 vedro-httpx-0.1.1/vedro_httpx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-12 15:51:48.000000 vedro-httpx-0.1.1/vedro_httpx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:51:52.150869 vedro-httpx-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-13 15:51:39.000000 vedro-httpx-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-06-13 15:51:52.150869 vedro-httpx-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-06-13 15:51:39.000000 vedro-httpx-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-06-13 15:51:52.150869 vedro-httpx-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-13 15:51:39.000000 vedro-httpx-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:51:52.146870 vedro-httpx-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-13 15:51:39.000000 vedro-httpx-0.1.2/tests/test_async_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-06-13 15:51:39.000000 vedro-httpx-0.1.2/tests/test_format_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-13 15:51:39.000000 vedro-httpx-0.1.2/tests/test_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-13 15:51:39.000000 vedro-httpx-0.1.2/tests/test_sync_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:51:52.150869 vedro-httpx-0.1.2/vedro_httpx/
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-13 15:51:39.000000 vedro-httpx-0.1.2/vedro_httpx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-06-13 15:51:39.000000 vedro-httpx-0.1.2/vedro_httpx/_async_http_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-13 15:51:39.000000 vedro-httpx-0.1.2/vedro_httpx/_render_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-13 15:51:39.000000 vedro-httpx-0.1.2/vedro_httpx/_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-06-13 15:51:39.000000 vedro-httpx-0.1.2/vedro_httpx/_sync_http_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-13 15:51:39.000000 vedro-httpx-0.1.2/vedro_httpx/_vedro_httpx.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 15:51:39.000000 vedro-httpx-0.1.2/vedro_httpx/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:51:52.150869 vedro-httpx-0.1.2/vedro_httpx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-06-13 15:51:52.000000 vedro-httpx-0.1.2/vedro_httpx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-13 15:51:52.000000 vedro-httpx-0.1.2/vedro_httpx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 15:51:52.000000 vedro-httpx-0.1.2/vedro_httpx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-13 15:51:52.000000 vedro-httpx-0.1.2/vedro_httpx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-13 15:51:52.000000 vedro-httpx-0.1.2/vedro_httpx.egg-info/top_level.txt
```

### Comparing `vedro-httpx-0.1.1/LICENSE` & `vedro-httpx-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vedro-httpx-0.1.1/PKG-INFO` & `vedro-httpx-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vedro-httpx
-Version: 0.1.1
+Version: 0.1.2
 Summary: Vedro + HTTPX
 Home-page: https://github.com/vedro-universe/vedro-httpx
 Author: Nikita Tsvetkov
 Author-email: tsv1@fastmail.com
 License: Apache-2.0
 Project-URL: GitHub, https://github.com/vedro-universe/vedro-httpx
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `vedro-httpx-0.1.1/README.md` & `vedro-httpx-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `vedro-httpx-0.1.1/setup.cfg` & `vedro-httpx-0.1.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.1.1
+current_version = 0.1.2
 message = bump version → {new_version}
 commit = True
 tag = True
 sign_tags = True
 
 [bumpversion:file:setup.py]
```

### Comparing `vedro-httpx-0.1.1/setup.py` & `vedro-httpx-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 def find_dev_required():
     with open("requirements-dev.txt") as f:
         return f.read().splitlines()
 
 
 setup(
     name="vedro-httpx",
-    version="0.1.1",
+    version="0.1.2",
     description="Vedro + HTTPX",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Nikita Tsvetkov",
     author_email="tsv1@fastmail.com",
     python_requires=">=3.8",
     url="https://github.com/vedro-universe/vedro-httpx",
```

### Comparing `vedro-httpx-0.1.1/tests/test_async_interface.py` & `vedro-httpx-0.1.2/tests/test_async_interface.py`

 * *Files identical despite different names*

### Comparing `vedro-httpx-0.1.1/tests/test_format_response.py` & `vedro-httpx-0.1.2/tests/test_format_response.py`

 * *Files identical despite different names*

### Comparing `vedro-httpx-0.1.1/tests/test_response.py` & `vedro-httpx-0.1.2/tests/test_response.py`

 * *Files identical despite different names*

### Comparing `vedro-httpx-0.1.1/tests/test_sync_interface.py` & `vedro-httpx-0.1.2/tests/test_sync_interface.py`

 * *Files identical despite different names*

### Comparing `vedro-httpx-0.1.1/vedro_httpx/_async_http_interface.py` & `vedro-httpx-0.1.2/vedro_httpx/_async_http_interface.py`

 * *Files identical despite different names*

### Comparing `vedro-httpx-0.1.1/vedro_httpx/_render_response.py` & `vedro-httpx-0.1.2/vedro_httpx/_render_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,21 +8,23 @@
 from pygments.util import ClassNotFound
 from rich.console import RenderResult
 from rich.syntax import Syntax
 
 __all__ = ("render_response",)
 
 
-def render_response(response: Response, *, theme: str = "ansi_dark") -> RenderResult:
+def render_response(response: Response, *,
+                    theme: str = "ansi_dark", code_width: int = 1024 ** 2) -> RenderResult:
     yield "Response:"
     headers, http_lexer = format_response_headers(response)
-    yield Syntax(headers, http_lexer, theme=theme)
+    yield Syntax(headers, http_lexer, theme=theme, code_width=code_width)
 
     body, lexer = format_response_body(response)
-    yield Syntax(body, lexer, theme=theme, background_color="default", indent_guides=True)
+    yield Syntax(body, lexer, theme=theme, background_color="default",
+                 indent_guides=True, code_width=code_width)
 
 
 def format_response_headers(response: Response) -> Tuple[str, Lexer]:
     lines = [f"{response.http_version} {response.status_code} {response.reason_phrase}"]
     for header in response.headers:
         values = response.headers.get_list(header)
         for value in values:
```

### Comparing `vedro-httpx-0.1.1/vedro_httpx/_sync_http_interface.py` & `vedro-httpx-0.1.2/vedro_httpx/_sync_http_interface.py`

 * *Files identical despite different names*

### Comparing `vedro-httpx-0.1.1/vedro_httpx.egg-info/PKG-INFO` & `vedro-httpx-0.1.2/vedro_httpx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vedro-httpx
-Version: 0.1.1
+Version: 0.1.2
 Summary: Vedro + HTTPX
 Home-page: https://github.com/vedro-universe/vedro-httpx
 Author: Nikita Tsvetkov
 Author-email: tsv1@fastmail.com
 License: Apache-2.0
 Project-URL: GitHub, https://github.com/vedro-universe/vedro-httpx
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `vedro-httpx-0.1.1/vedro_httpx.egg-info/SOURCES.txt` & `vedro-httpx-0.1.2/vedro_httpx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

