# Comparing `tmp/websocket-tools-0.0.14.tar.gz` & `tmp/websocket-tools-0.0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "websocket-tools-0.0.14.tar", last modified: Sun Apr 30 08:35:39 2023, max compression
+gzip compressed data, was "websocket-tools-0.0.15.tar", last modified: Tue Jun 13 10:15:07 2023, max compression
```

## Comparing `websocket-tools-0.0.14.tar` & `websocket-tools-0.0.15.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:35:39.462972 websocket-tools-0.0.14/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-30 08:35:28.000000 websocket-tools-0.0.14/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-30 08:35:39.462972 websocket-tools-0.0.14/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-30 08:35:28.000000 websocket-tools-0.0.14/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-30 08:35:28.000000 websocket-tools-0.0.14/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 08:35:39.462972 websocket-tools-0.0.14/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:35:39.458972 websocket-tools-0.0.14/websocket_tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 08:35:28.000000 websocket-tools-0.0.14/websocket_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-30 08:35:28.000000 websocket-tools-0.0.14/websocket_tools/websocket_loop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 08:35:39.462972 websocket-tools-0.0.14/websocket_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-30 08:35:39.000000 websocket-tools-0.0.14/websocket_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-30 08:35:39.000000 websocket-tools-0.0.14/websocket_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 08:35:39.000000 websocket-tools-0.0.14/websocket_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-30 08:35:39.000000 websocket-tools-0.0.14/websocket_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:15:07.871672 websocket-tools-0.0.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-13 10:14:55.000000 websocket-tools-0.0.15/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-13 10:15:07.871672 websocket-tools-0.0.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-13 10:14:55.000000 websocket-tools-0.0.15/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-13 10:14:55.000000 websocket-tools-0.0.15/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 10:15:07.871672 websocket-tools-0.0.15/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:15:07.871672 websocket-tools-0.0.15/websocket_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 10:14:55.000000 websocket-tools-0.0.15/websocket_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-13 10:14:55.000000 websocket-tools-0.0.15/websocket_tools/websocket_loop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:15:07.871672 websocket-tools-0.0.15/websocket_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-13 10:15:07.000000 websocket-tools-0.0.15/websocket_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-13 10:15:07.000000 websocket-tools-0.0.15/websocket_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 10:15:07.000000 websocket-tools-0.0.15/websocket_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-13 10:15:07.000000 websocket-tools-0.0.15/websocket_tools.egg-info/top_level.txt
```

### Comparing `websocket-tools-0.0.14/LICENCE` & `websocket-tools-0.0.15/LICENCE`

 * *Files identical despite different names*

### Comparing `websocket-tools-0.0.14/PKG-INFO` & `websocket-tools-0.0.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: websocket-tools
-Version: 0.0.14
+Version: 0.0.15
 Summary: A simple module to wrap web socket connection code.
 Author-email: sir even <sir_even@icloud.com>
 Project-URL: Homepage, https://github.com/sirEven/websocket-tools.git
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `websocket-tools-0.0.14/pyproject.toml` & `websocket-tools-0.0.15/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "websocket-client"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "websocket-tools"
-version = "0.0.14"
+version = "0.0.15"
 authors = [
   { name="sir even", email="sir_even@icloud.com"},
 ]
 description = "A simple module to wrap web socket connection code."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `websocket-tools-0.0.14/websocket_tools/websocket_loop.py` & `websocket-tools-0.0.15/websocket_tools/websocket_loop.py`

 * *Files 11% similar despite different names*

```diff
@@ -27,8 +27,9 @@
             on_message=self.on_message,
             on_error=self.on_error,
             on_close=self.on_close,
         )
         self.ws.run_forever()
 
     def terminate(self):
-        self.ws.close()
+        if self.ws is not None:
+            self.ws.close()
```

### Comparing `websocket-tools-0.0.14/websocket_tools.egg-info/PKG-INFO` & `websocket-tools-0.0.15/websocket_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: websocket-tools
-Version: 0.0.14
+Version: 0.0.15
 Summary: A simple module to wrap web socket connection code.
 Author-email: sir even <sir_even@icloud.com>
 Project-URL: Homepage, https://github.com/sirEven/websocket-tools.git
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

