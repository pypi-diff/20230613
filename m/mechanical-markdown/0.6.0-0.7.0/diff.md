# Comparing `tmp/mechanical-markdown-0.6.0.tar.gz` & `tmp/mechanical-markdown-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mechanical-markdown-0.6.0.tar", last modified: Wed Oct  5 20:26:14 2022, max compression
+gzip compressed data, was "dist/mechanical-markdown-0.7.0.tar", last modified: Tue Jun 13 04:46:10 2023, max compression
```

## Comparing `mechanical-markdown-0.6.0.tar` & `mechanical-markdown-0.7.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 20:26:14.000000 mechanical-markdown-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (121)    11412 2022-10-05 20:24:49.000000 mechanical-markdown-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     4018 2022-10-05 20:26:14.000000 mechanical-markdown-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2935 2022-10-05 20:24:49.000000 mechanical-markdown-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 20:26:14.000000 mechanical-markdown-0.6.0/mechanical_markdown/
--rw-r--r--   0 runner    (1001) docker     (121)      291 2022-10-05 20:24:49.000000 mechanical-markdown-0.6.0/mechanical_markdown/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3498 2022-10-05 20:24:49.000000 mechanical-markdown-0.6.0/mechanical_markdown/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1732 2022-10-05 20:24:49.000000 mechanical-markdown-0.6.0/mechanical_markdown/command.py
--rw-r--r--   0 runner    (1001) docker     (121)     2645 2022-10-05 20:24:49.000000 mechanical-markdown-0.6.0/mechanical_markdown/parsers.py
--rw-r--r--   0 runner    (1001) docker     (121)     3034 2022-10-05 20:24:49.000000 mechanical-markdown-0.6.0/mechanical_markdown/recipe.py
--rw-r--r--   0 runner    (1001) docker     (121)     7670 2022-10-05 20:24:49.000000 mechanical-markdown-0.6.0/mechanical_markdown/step.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 20:26:14.000000 mechanical-markdown-0.6.0/mechanical_markdown.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4018 2022-10-05 20:26:14.000000 mechanical-markdown-0.6.0/mechanical_markdown.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      588 2022-10-05 20:26:14.000000 mechanical-markdown-0.6.0/mechanical_markdown.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-05 20:26:14.000000 mechanical-markdown-0.6.0/mechanical_markdown.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-10-05 20:26:14.000000 mechanical-markdown-0.6.0/mechanical_markdown.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-10-05 20:26:14.000000 mechanical-markdown-0.6.0/mechanical_markdown.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-10-05 20:26:14.000000 mechanical-markdown-0.6.0/mechanical_markdown.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-10-05 20:26:14.000000 mechanical-markdown-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1171 2022-10-05 20:24:49.000000 mechanical-markdown-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 20:26:14.000000 mechanical-markdown-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-05 20:24:49.000000 mechanical-markdown-0.6.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1006 2022-10-05 20:24:49.000000 mechanical-markdown-0.6.0/tests/fake_http_server.py
--rw-r--r--   0 runner    (1001) docker     (121)     3432 2022-10-05 20:24:49.000000 mechanical-markdown-0.6.0/tests/test_link_validation.py
--rw-r--r--   0 runner    (1001) docker     (121)    19394 2022-10-05 20:24:49.000000 mechanical-markdown-0.6.0/tests/test_mechanical_markdown.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 04:46:10.000000 mechanical-markdown-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11412 2023-06-13 04:44:39.000000 mechanical-markdown-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-06-13 04:46:10.000000 mechanical-markdown-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-06-13 04:44:39.000000 mechanical-markdown-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 04:46:10.000000 mechanical-markdown-0.7.0/mechanical_markdown/
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-13 04:44:39.000000 mechanical-markdown-0.7.0/mechanical_markdown/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-06-13 04:44:39.000000 mechanical-markdown-0.7.0/mechanical_markdown/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-06-13 04:44:39.000000 mechanical-markdown-0.7.0/mechanical_markdown/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-06-13 04:44:39.000000 mechanical-markdown-0.7.0/mechanical_markdown/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-06-13 04:44:39.000000 mechanical-markdown-0.7.0/mechanical_markdown/recipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7670 2023-06-13 04:44:39.000000 mechanical-markdown-0.7.0/mechanical_markdown/step.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 04:46:10.000000 mechanical-markdown-0.7.0/mechanical_markdown.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-06-13 04:46:10.000000 mechanical-markdown-0.7.0/mechanical_markdown.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-13 04:46:10.000000 mechanical-markdown-0.7.0/mechanical_markdown.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 04:46:10.000000 mechanical-markdown-0.7.0/mechanical_markdown.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-13 04:46:10.000000 mechanical-markdown-0.7.0/mechanical_markdown.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-13 04:46:10.000000 mechanical-markdown-0.7.0/mechanical_markdown.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-13 04:46:10.000000 mechanical-markdown-0.7.0/mechanical_markdown.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-13 04:46:10.000000 mechanical-markdown-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-13 04:44:39.000000 mechanical-markdown-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 04:46:10.000000 mechanical-markdown-0.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 04:44:39.000000 mechanical-markdown-0.7.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-13 04:44:39.000000 mechanical-markdown-0.7.0/tests/fake_http_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-06-13 04:44:39.000000 mechanical-markdown-0.7.0/tests/test_link_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19394 2023-06-13 04:44:39.000000 mechanical-markdown-0.7.0/tests/test_mechanical_markdown.py
```

### Comparing `mechanical-markdown-0.6.0/LICENSE` & `mechanical-markdown-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mechanical-markdown-0.6.0/PKG-INFO` & `mechanical-markdown-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mechanical-markdown
-Version: 0.6.0
+Version: 0.7.0
 Summary: Run markdown recipes as shell scripts
 Home-page: https://github.com/dapr/mechanical-markdown
 Author: Charlie Stanley
 Author-email: Charlie.Stanley@microsoft.com
 License: MIT
 Description: # Mechanical Markdown
```

### Comparing `mechanical-markdown-0.6.0/README.md` & `mechanical-markdown-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `mechanical-markdown-0.6.0/mechanical_markdown/__main__.py` & `mechanical-markdown-0.7.0/mechanical_markdown/__main__.py`

 * *Files identical despite different names*

### Comparing `mechanical-markdown-0.6.0/mechanical_markdown/command.py` & `mechanical-markdown-0.7.0/mechanical_markdown/command.py`

 * *Files identical despite different names*

### Comparing `mechanical-markdown-0.6.0/mechanical_markdown/parsers.py` & `mechanical-markdown-0.7.0/mechanical_markdown/parsers.py`

 * *Files 10% similar despite different names*

```diff
@@ -36,23 +36,25 @@
         super().__init__(**kwargs)
         self.current_step = None
         self.all_steps = []
         self.external_links = []
         self.ignore_links = False
         self.shell = shell
 
-    def block_code(self, text, lang=None):
-        if (lang is not None and lang.strip() in ('bash', 'sh', 'shell-script', 'shell')
-                and self.current_step is not None):
-            self.current_step.add_command_block(text)
+    def block_code(self, code: str, info=None):
+        if info:
+            lang = info.split(None, 1)[0]
+            if (lang is not None and lang.strip() in ('bash', 'sh', 'shell-script', 'shell')
+                    and self.current_step is not None):
+                self.current_step.add_command_block(code)
         return ""
 
-    def block_html(self, text):
+    def block_html(self, html: str):
         comment_parser = HTMLCommentParser()
-        comment_parser.feed(text)
+        comment_parser.feed(html)
 
         comment_body = comment_parser.comment_text
         if comment_body.find(end_token) >= 0:
             if self.current_step is None:
                 raise MarkdownAnnotationError("Unexpected <!-- {} --> found".format(end_token))
             self.all_steps.append(self.current_step)
             self.current_step = None
@@ -77,12 +79,12 @@
             raise MarkdownAnnotationError(f"<!-- {start_token} --> found while still processing previous step")
 
         start_pos += len(start_token)
         self.current_step = Step(yaml.safe_load(comment_body[start_pos:]), self.shell)
 
         return ""
 
-    def link(self, link, text=None, title=None):
-        if re.match("https?://", link) is not None:
-            self.external_links.append((link, self.ignore_links))
+    def link(self, text, url=None, title=None):
+        if re.match("https?://", url) is not None:
+            self.external_links.append((url, self.ignore_links))
 
         return ""
```

### Comparing `mechanical-markdown-0.6.0/mechanical_markdown/recipe.py` & `mechanical-markdown-0.7.0/mechanical_markdown/recipe.py`

 * *Files identical despite different names*

### Comparing `mechanical-markdown-0.6.0/mechanical_markdown/step.py` & `mechanical-markdown-0.7.0/mechanical_markdown/step.py`

 * *Files identical despite different names*

### Comparing `mechanical-markdown-0.6.0/mechanical_markdown.egg-info/PKG-INFO` & `mechanical-markdown-0.7.0/mechanical_markdown.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mechanical-markdown
-Version: 0.6.0
+Version: 0.7.0
 Summary: Run markdown recipes as shell scripts
 Home-page: https://github.com/dapr/mechanical-markdown
 Author: Charlie Stanley
 Author-email: Charlie.Stanley@microsoft.com
 License: MIT
 Description: # Mechanical Markdown
```

### Comparing `mechanical-markdown-0.6.0/mechanical_markdown.egg-info/SOURCES.txt` & `mechanical-markdown-0.7.0/mechanical_markdown.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mechanical-markdown-0.6.0/setup.py` & `mechanical-markdown-0.7.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,14 +30,14 @@
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7"
     ],
     packages=find_packages(exclude='tests'),
     include_package_data=True,
-    install_requires=["termcolor", "pyyaml", "mistune", "requests", "colorama"],
+    install_requires=["termcolor", "pyyaml", "mistune>=3.0.0", "requests", "colorama"],
     entry_points={
         "console_scripts": [
             "mm.py = mechanical_markdown.__main__:main"
         ]
     },
 )
```

### Comparing `mechanical-markdown-0.6.0/tests/fake_http_server.py` & `mechanical-markdown-0.7.0/tests/fake_http_server.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 
 
 from threading import Thread
-from http.server import BaseHTTPRequestHandler, HTTPServer
+from http.server import BaseHTTPRequestHandler, ThreadingHTTPServer
 
 
 class EmptyReplyHandler(BaseHTTPRequestHandler):
     protocol_version = 'HTTP/1.1'
 
     def do_GET(self):
         self.send_response(next(self.server.response_code_generator))
         self.send_header('Content-Length', 0)
         self.end_headers()
 
 
 class FakeHttpServer(Thread):
     def __init__(self):
         super().__init__()
-        self.server = HTTPServer(('localhost', 0), EmptyReplyHandler)
+        self.server = ThreadingHTTPServer(('localhost', 0), EmptyReplyHandler)
         self.response_codes = []
 
     def set_response_codes(self, codes):
         def response_code_generator():
             for response_code in codes:
                 yield response_code
         self.server.response_code_generator = response_code_generator()
 
     def get_port(self):
         return self.server.socket.getsockname()[1]
 
-    def shutdown_server(self):
+    def shutdown_server(self, timeout=5):
         self.server.shutdown()
         self.server.socket.close()
-        self.join()
+        self.join(timeout=timeout)
 
     def run(self):
         self.server.serve_forever()
```

### Comparing `mechanical-markdown-0.6.0/tests/test_link_validation.py` & `mechanical-markdown-0.7.0/tests/test_link_validation.py`

 * *Files identical despite different names*

### Comparing `mechanical-markdown-0.6.0/tests/test_mechanical_markdown.py` & `mechanical-markdown-0.7.0/tests/test_mechanical_markdown.py`

 * *Files identical despite different names*

