# Comparing `tmp/robocorp_tasks-0.4.1.tar.gz` & `tmp/robocorp_tasks-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robocorp_tasks-0.4.1.tar", max compression
+gzip compressed data, was "robocorp_tasks-1.0.0.tar", max compression
```

## Comparing `robocorp_tasks-0.4.1.tar` & `robocorp_tasks-1.0.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     4922 2023-06-09 10:25:27.480553 robocorp_tasks-0.4.1/README.md
--rw-r--r--   0        0        0     1165 2023-06-09 10:25:27.480553 robocorp_tasks-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     3502 2023-06-09 10:25:27.480553 robocorp_tasks-0.4.1/src/robocorp/tasks/__init__.py
--rw-r--r--   0        0        0       79 2023-06-09 10:25:27.480553 robocorp_tasks-0.4.1/src/robocorp/tasks/__main__.py
--rw-r--r--   0        0        0     4495 2023-06-09 10:25:27.480553 robocorp_tasks-0.4.1/src/robocorp/tasks/_argdispatch.py
--rw-r--r--   0        0        0     1457 2023-06-09 10:25:27.480553 robocorp_tasks-0.4.1/src/robocorp/tasks/_callback.py
--rw-r--r--   0        0        0     5121 2023-06-09 10:25:27.480553 robocorp_tasks-0.4.1/src/robocorp/tasks/_collect_tasks.py
--rw-r--r--   0        0        0    10160 2023-06-09 10:25:27.480553 robocorp_tasks-0.4.1/src/robocorp/tasks/_commands.py
--rw-r--r--   0        0        0     2245 2023-06-09 10:25:27.480553 robocorp_tasks-0.4.1/src/robocorp/tasks/_config.py
--rw-r--r--   0        0        0      182 2023-06-09 10:25:27.480553 robocorp_tasks-0.4.1/src/robocorp/tasks/_exceptions.py
--rw-r--r--   0        0        0     1122 2023-06-09 10:25:27.480553 robocorp_tasks-0.4.1/src/robocorp/tasks/_hooks.py
--rw-r--r--   0        0        0     1367 2023-06-09 10:25:27.480553 robocorp_tasks-0.4.1/src/robocorp/tasks/_lifecycle.py
--rw-r--r--   0        0        0     4078 2023-06-09 10:25:27.480553 robocorp_tasks-0.4.1/src/robocorp/tasks/_log_auto_setup.py
--rw-r--r--   0        0        0      461 2023-06-09 10:25:27.480553 robocorp_tasks-0.4.1/src/robocorp/tasks/_log_output_setup.py
--rw-r--r--   0        0        0     3943 2023-06-09 10:25:27.480553 robocorp_tasks-0.4.1/src/robocorp/tasks/_protocols.py
--rw-r--r--   0        0        0     5489 2023-06-09 10:25:27.480553 robocorp_tasks-0.4.1/src/robocorp/tasks/_task.py
--rw-r--r--   0        0        0     2436 2023-06-09 10:25:27.480553 robocorp_tasks-0.4.1/src/robocorp/tasks/_toml_settings.py
--rw-r--r--   0        0        0      869 2023-06-09 10:25:27.484553 robocorp_tasks-0.4.1/src/robocorp/tasks/cli.py
--rw-r--r--   0        0        0        0 2023-06-09 10:25:27.484553 robocorp_tasks-0.4.1/src/robocorp/tasks/py.typed
--rw-r--r--   0        0        0     5517 1970-01-01 00:00:00.000000 robocorp_tasks-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     4871 2023-06-13 15:01:29.774650 robocorp_tasks-1.0.0/README.md
+-rw-r--r--   0        0        0     1162 2023-06-13 15:01:29.774650 robocorp_tasks-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3502 2023-06-13 15:01:29.774650 robocorp_tasks-1.0.0/src/robocorp/tasks/__init__.py
+-rw-r--r--   0        0        0       79 2023-06-13 15:01:29.774650 robocorp_tasks-1.0.0/src/robocorp/tasks/__main__.py
+-rw-r--r--   0        0        0     4495 2023-06-13 15:01:29.774650 robocorp_tasks-1.0.0/src/robocorp/tasks/_argdispatch.py
+-rw-r--r--   0        0        0     1457 2023-06-13 15:01:29.774650 robocorp_tasks-1.0.0/src/robocorp/tasks/_callback.py
+-rw-r--r--   0        0        0     5121 2023-06-13 15:01:29.774650 robocorp_tasks-1.0.0/src/robocorp/tasks/_collect_tasks.py
+-rw-r--r--   0        0        0    10192 2023-06-13 15:01:29.774650 robocorp_tasks-1.0.0/src/robocorp/tasks/_commands.py
+-rw-r--r--   0        0        0     2245 2023-06-13 15:01:29.774650 robocorp_tasks-1.0.0/src/robocorp/tasks/_config.py
+-rw-r--r--   0        0        0      182 2023-06-13 15:01:29.774650 robocorp_tasks-1.0.0/src/robocorp/tasks/_exceptions.py
+-rw-r--r--   0        0        0     1122 2023-06-13 15:01:29.774650 robocorp_tasks-1.0.0/src/robocorp/tasks/_hooks.py
+-rw-r--r--   0        0        0     1367 2023-06-13 15:01:29.774650 robocorp_tasks-1.0.0/src/robocorp/tasks/_lifecycle.py
+-rw-r--r--   0        0        0     4078 2023-06-13 15:01:29.774650 robocorp_tasks-1.0.0/src/robocorp/tasks/_log_auto_setup.py
+-rw-r--r--   0        0        0      461 2023-06-13 15:01:29.774650 robocorp_tasks-1.0.0/src/robocorp/tasks/_log_output_setup.py
+-rw-r--r--   0        0        0     3943 2023-06-13 15:01:29.774650 robocorp_tasks-1.0.0/src/robocorp/tasks/_protocols.py
+-rw-r--r--   0        0        0     5489 2023-06-13 15:01:29.774650 robocorp_tasks-1.0.0/src/robocorp/tasks/_task.py
+-rw-r--r--   0        0        0     2436 2023-06-13 15:01:29.774650 robocorp_tasks-1.0.0/src/robocorp/tasks/_toml_settings.py
+-rw-r--r--   0        0        0      869 2023-06-13 15:01:29.774650 robocorp_tasks-1.0.0/src/robocorp/tasks/cli.py
+-rw-r--r--   0        0        0        0 2023-06-13 15:01:29.774650 robocorp_tasks-1.0.0/src/robocorp/tasks/py.typed
+-rw-r--r--   0        0        0     5461 1970-01-01 00:00:00.000000 robocorp_tasks-1.0.0/PKG-INFO
```

### Comparing `robocorp_tasks-0.4.1/README.md` & `robocorp_tasks-1.0.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # robocorp-tasks
 
 `robocorp-tasks` is a Python framework designed to simplify the development 
 of Python automations.
 
-> Note: The current version is still alpha but its public API is already meant
-> to be stable and new releases should keep backward compatibility.
+> Note: The current version (1.0.0) is now in beta. Semantic versioning is used in the project.
 
 ## Why
 
 While Python is widely used in the automation world, many solutions end up being 
 ad-hoc, making it difficult to navigate different projects and keep up with the
 features required for analysing the results of such automations afterwards.
```

### Comparing `robocorp_tasks-0.4.1/pyproject.toml` & `robocorp_tasks-1.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [tool.poetry]
 name = "robocorp-tasks"
-version = "0.4.1"
+version = "1.0.0"
 description = "The automation framework for Python"
 authors = [
 	"Fabio Zadrozny <fabio@robocorp.com>",
 ]
 readme = "README.md"
 packages = [{include = "robocorp/tasks", from = "src"}]
 classifiers = [
-    "Development Status :: 3 - Alpha",
+    "Development Status :: 4 - Beta",
     "Topic :: Software Development :: Libraries :: Application Frameworks",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-robocorp-log = "^0.3"
+robocorp-log = "^1"
 
 [tool.poetry.group.dev.dependencies]
 robocorp-devutils = {path = "../devutils/", develop = true}
 
 [tool.mypy]
 mypy_path = "src:tests"
```

### Comparing `robocorp_tasks-0.4.1/src/robocorp/tasks/__init__.py` & `robocorp_tasks-1.0.0/src/robocorp/tasks/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 automatically logged is not imported prior the the `cli.main` call.
 """
 from pathlib import Path
 from typing import Optional
 
 from ._protocols import ITask
 
-__version__ = "0.4.1"
+__version__ = "1.0.0"
 version_info = [int(x) for x in __version__.split(".")]
 
 
 def task(func):
     """
     Decorator for tasks (entry points) which can be executed by `robocorp.tasks`.
```

### Comparing `robocorp_tasks-0.4.1/src/robocorp/tasks/_argdispatch.py` & `robocorp_tasks-1.0.0/src/robocorp/tasks/_argdispatch.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-0.4.1/src/robocorp/tasks/_callback.py` & `robocorp_tasks-1.0.0/src/robocorp/tasks/_callback.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-0.4.1/src/robocorp/tasks/_collect_tasks.py` & `robocorp_tasks-1.0.0/src/robocorp/tasks/_collect_tasks.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-0.4.1/src/robocorp/tasks/_commands.py` & `robocorp_tasks-1.0.0/src/robocorp/tasks/_commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,14 +53,15 @@
                     "line": task.lineno,
                     "file": task.filename,
                     "docs": getattr(task.method, "__doc__") or "",
                 }
             )
 
         original_stdout.write(json.dumps(tasks_found))
+        original_stdout.flush()
     return 0
 
 
 # Note: the args must match the 'dest' on the configured argparser.
 @_arg_dispatch.register()
 def run(
     output_dir: str,
```

### Comparing `robocorp_tasks-0.4.1/src/robocorp/tasks/_config.py` & `robocorp_tasks-1.0.0/src/robocorp/tasks/_config.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-0.4.1/src/robocorp/tasks/_hooks.py` & `robocorp_tasks-1.0.0/src/robocorp/tasks/_hooks.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-0.4.1/src/robocorp/tasks/_lifecycle.py` & `robocorp_tasks-1.0.0/src/robocorp/tasks/_lifecycle.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-0.4.1/src/robocorp/tasks/_log_auto_setup.py` & `robocorp_tasks-1.0.0/src/robocorp/tasks/_log_auto_setup.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-0.4.1/src/robocorp/tasks/_protocols.py` & `robocorp_tasks-1.0.0/src/robocorp/tasks/_protocols.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-0.4.1/src/robocorp/tasks/_task.py` & `robocorp_tasks-1.0.0/src/robocorp/tasks/_task.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-0.4.1/src/robocorp/tasks/_toml_settings.py` & `robocorp_tasks-1.0.0/src/robocorp/tasks/_toml_settings.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-0.4.1/src/robocorp/tasks/cli.py` & `robocorp_tasks-1.0.0/src/robocorp/tasks/cli.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-0.4.1/PKG-INFO` & `robocorp_tasks-1.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
 Name: robocorp-tasks
-Version: 0.4.1
+Version: 1.0.0
 Summary: The automation framework for Python
 Author: Fabio Zadrozny
 Author-email: fabio@robocorp.com
 Requires-Python: >=3.9,<4.0
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Requires-Dist: robocorp-log (>=0.3,<0.4)
+Requires-Dist: robocorp-log (>=1,<2)
 Description-Content-Type: text/markdown
 
 # robocorp-tasks
 
 `robocorp-tasks` is a Python framework designed to simplify the development 
 of Python automations.
 
-> Note: The current version is still alpha but its public API is already meant
-> to be stable and new releases should keep backward compatibility.
+> Note: The current version (1.0.0) is now in beta. Semantic versioning is used in the project.
 
 ## Why
 
 While Python is widely used in the automation world, many solutions end up being 
 ad-hoc, making it difficult to navigate different projects and keep up with the
 features required for analysing the results of such automations afterwards.
```

