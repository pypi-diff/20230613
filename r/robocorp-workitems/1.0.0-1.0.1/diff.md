# Comparing `tmp/robocorp_workitems-1.0.0.tar.gz` & `tmp/robocorp_workitems-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robocorp_workitems-1.0.0.tar", max compression
+gzip compressed data, was "robocorp_workitems-1.0.1.tar", max compression
```

## Comparing `robocorp_workitems-1.0.0.tar` & `robocorp_workitems-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     5629 2023-06-09 12:05:44.045382 robocorp_workitems-1.0.0/README.md
--rw-r--r--   0        0        0      819 2023-06-09 12:05:44.045382 robocorp_workitems-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     4980 2023-06-09 12:05:44.045382 robocorp_workitems-1.0.0/src/robocorp/workitems/__init__.py
--rw-r--r--   0        0        0    17330 2023-06-09 12:05:44.045382 robocorp_workitems-1.0.0/src/robocorp/workitems/_adapters.py
--rw-r--r--   0        0        0     2380 2023-06-09 12:05:44.045382 robocorp_workitems-1.0.0/src/robocorp/workitems/_context.py
--rw-r--r--   0        0        0      958 2023-06-09 12:05:44.045382 robocorp_workitems-1.0.0/src/robocorp/workitems/_exceptions.py
--rw-r--r--   0        0        0     6520 2023-06-09 12:05:44.045382 robocorp_workitems-1.0.0/src/robocorp/workitems/_requests.py
--rw-r--r--   0        0        0     1558 2023-06-09 12:05:44.045382 robocorp_workitems-1.0.0/src/robocorp/workitems/_types.py
--rw-r--r--   0        0        0     2331 2023-06-09 12:05:44.045382 robocorp_workitems-1.0.0/src/robocorp/workitems/_utils.py
--rw-r--r--   0        0        0     8652 2023-06-09 12:05:44.045382 robocorp_workitems-1.0.0/src/robocorp/workitems/_workitem.py
--rw-r--r--   0        0        0        0 2023-06-09 12:05:44.045382 robocorp_workitems-1.0.0/src/robocorp/workitems/py.typed
--rw-r--r--   0        0        0     6269 1970-01-01 00:00:00.000000 robocorp_workitems-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     5629 2023-06-13 15:07:46.458620 robocorp_workitems-1.0.1/README.md
+-rw-r--r--   0        0        0      817 2023-06-13 15:07:46.458620 robocorp_workitems-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     4980 2023-06-13 15:07:46.462620 robocorp_workitems-1.0.1/src/robocorp/workitems/__init__.py
+-rw-r--r--   0        0        0    17330 2023-06-13 15:07:46.462620 robocorp_workitems-1.0.1/src/robocorp/workitems/_adapters.py
+-rw-r--r--   0        0        0     2380 2023-06-13 15:07:46.462620 robocorp_workitems-1.0.1/src/robocorp/workitems/_context.py
+-rw-r--r--   0        0        0      958 2023-06-13 15:07:46.462620 robocorp_workitems-1.0.1/src/robocorp/workitems/_exceptions.py
+-rw-r--r--   0        0        0     6520 2023-06-13 15:07:46.462620 robocorp_workitems-1.0.1/src/robocorp/workitems/_requests.py
+-rw-r--r--   0        0        0     1558 2023-06-13 15:07:46.462620 robocorp_workitems-1.0.1/src/robocorp/workitems/_types.py
+-rw-r--r--   0        0        0     2331 2023-06-13 15:07:46.462620 robocorp_workitems-1.0.1/src/robocorp/workitems/_utils.py
+-rw-r--r--   0        0        0     8652 2023-06-13 15:07:46.462620 robocorp_workitems-1.0.1/src/robocorp/workitems/_workitem.py
+-rw-r--r--   0        0        0        0 2023-06-13 15:07:46.462620 robocorp_workitems-1.0.1/src/robocorp/workitems/py.typed
+-rw-r--r--   0        0        0     6265 1970-01-01 00:00:00.000000 robocorp_workitems-1.0.1/PKG-INFO
```

### Comparing `robocorp_workitems-1.0.0/README.md` & `robocorp_workitems-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `robocorp_workitems-1.0.0/pyproject.toml` & `robocorp_workitems-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "robocorp-workitems"
-version = "1.0.0"
+version = "1.0.1"
 description = "Robocorp Work Items library"
 authors = [
 	"Ossi R. <ossi@robocorp.com>",
 	"Fabio Z. <fabio@robocorp.com>",
     "Antero V. <antero@robocorp.com>",
 ]
 readme = "README.md"
@@ -15,15 +15,15 @@
 skip-magic-trailing-comma = false
 
 [tool.isort]
 profile = "black"
 
 [tool.poetry.dependencies]
 python = "^3.9"
-robocorp-tasks = "^0.4"
+robocorp-tasks = "^1"
 requests = "^2.28.2"
 tenacity = "^8.0.1"
 dataclasses-json = "^0.5.7"
 python-dateutil = "^2.8.2"
 
 [tool.poetry.group.dev.dependencies]
 robocorp-devutils = {path = "../devutils/", develop = true}
```

### Comparing `robocorp_workitems-1.0.0/src/robocorp/workitems/__init__.py` & `robocorp_workitems-1.0.1/src/robocorp/workitems/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     BusinessException,
     EmptyQueue,
     to_exception_type,
 )
 from ._types import ExceptionType, JSONType, State
 from ._workitem import Input, Output
 
-__version__ = "1.0.0"
+__version__ = "1.0.1"
 version_info = [int(x) for x in __version__.split(".")]
 
 LOGGER = logging.getLogger(__name__)
 
 
 @task_cache
 def __ctx():
```

### Comparing `robocorp_workitems-1.0.0/src/robocorp/workitems/_adapters.py` & `robocorp_workitems-1.0.1/src/robocorp/workitems/_adapters.py`

 * *Files identical despite different names*

### Comparing `robocorp_workitems-1.0.0/src/robocorp/workitems/_context.py` & `robocorp_workitems-1.0.1/src/robocorp/workitems/_context.py`

 * *Files identical despite different names*

### Comparing `robocorp_workitems-1.0.0/src/robocorp/workitems/_exceptions.py` & `robocorp_workitems-1.0.1/src/robocorp/workitems/_exceptions.py`

 * *Files identical despite different names*

### Comparing `robocorp_workitems-1.0.0/src/robocorp/workitems/_requests.py` & `robocorp_workitems-1.0.1/src/robocorp/workitems/_requests.py`

 * *Files identical despite different names*

### Comparing `robocorp_workitems-1.0.0/src/robocorp/workitems/_types.py` & `robocorp_workitems-1.0.1/src/robocorp/workitems/_types.py`

 * *Files identical despite different names*

### Comparing `robocorp_workitems-1.0.0/src/robocorp/workitems/_utils.py` & `robocorp_workitems-1.0.1/src/robocorp/workitems/_utils.py`

 * *Files identical despite different names*

### Comparing `robocorp_workitems-1.0.0/src/robocorp/workitems/_workitem.py` & `robocorp_workitems-1.0.1/src/robocorp/workitems/_workitem.py`

 * *Files identical despite different names*

### Comparing `robocorp_workitems-1.0.0/PKG-INFO` & `robocorp_workitems-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: robocorp-workitems
-Version: 1.0.0
+Version: 1.0.1
 Summary: Robocorp Work Items library
 Author: Ossi R.
 Author-email: ossi@robocorp.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: dataclasses-json (>=0.5.7,<0.6.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
-Requires-Dist: robocorp-tasks (>=0.4,<0.5)
+Requires-Dist: robocorp-tasks (>=1,<2)
 Requires-Dist: tenacity (>=8.0.1,<9.0.0)
 Description-Content-Type: text/markdown
 
 # robocorp-workitems
 
 Work items are used in Robocorp Control Room for managing data that go through
 multiple steps and tasks inside a process. Each step of a process receives input
```

