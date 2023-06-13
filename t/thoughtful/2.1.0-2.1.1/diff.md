# Comparing `tmp/thoughtful-2.1.0.tar.gz` & `tmp/thoughtful-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thoughtful-2.1.0.tar", max compression
+gzip compressed data, was "thoughtful-2.1.1.tar", max compression
```

## Comparing `thoughtful-2.1.0.tar` & `thoughtful-2.1.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0    11358 2023-06-09 17:44:01.401763 thoughtful-2.1.0/LICENSE
--rw-r--r--   0        0        0     2992 2023-06-09 17:44:01.401763 thoughtful-2.1.0/README.md
--rw-r--r--   0        0        0     1935 2023-06-09 17:44:01.405763 thoughtful-2.1.0/pyproject.toml
--rw-r--r--   0        0        0      222 2023-06-09 17:44:01.405763 thoughtful-2.1.0/thoughtful/__init__.py
--rw-r--r--   0        0        0       54 2023-06-09 17:44:01.405763 thoughtful-2.1.0/thoughtful/__version__.py
--rw-r--r--   0        0        0     1070 2023-06-09 17:44:01.405763 thoughtful-2.1.0/thoughtful/environment_variables.py
--rw-r--r--   0        0        0      143 2023-06-09 17:44:01.405763 thoughtful-2.1.0/thoughtful/supervisor/__init__.py
--rw-r--r--   0        0        0     6616 2023-06-09 17:44:01.405763 thoughtful-2.1.0/thoughtful/supervisor/default_instances.py
--rw-r--r--   0        0        0      922 2023-06-09 17:44:01.405763 thoughtful-2.1.0/thoughtful/supervisor/event_bus.py
--rw-r--r--   0        0        0     8756 2023-06-09 17:44:01.405763 thoughtful-2.1.0/thoughtful/supervisor/main_context.py
--rw-r--r--   0        0        0    10567 2023-06-09 17:44:01.405763 thoughtful-2.1.0/thoughtful/supervisor/manifest.py
--rw-r--r--   0        0        0        0 2023-06-09 17:44:01.405763 thoughtful-2.1.0/thoughtful/supervisor/py.typed
--rw-r--r--   0        0        0        0 2023-06-09 17:44:01.405763 thoughtful-2.1.0/thoughtful/supervisor/reporting/__init__.py
--rw-r--r--   0        0        0     2872 2023-06-09 17:44:01.405763 thoughtful-2.1.0/thoughtful/supervisor/reporting/record.py
--rw-r--r--   0        0        0     1189 2023-06-09 17:44:01.405763 thoughtful-2.1.0/thoughtful/supervisor/reporting/record_report.py
--rw-r--r--   0        0        0     2066 2023-06-09 17:44:01.405763 thoughtful-2.1.0/thoughtful/supervisor/reporting/report.py
--rw-r--r--   0        0        0    10118 2023-06-09 17:44:01.405763 thoughtful-2.1.0/thoughtful/supervisor/reporting/report_builder.py
--rw-r--r--   0        0        0      660 2023-06-09 17:44:01.405763 thoughtful-2.1.0/thoughtful/supervisor/reporting/status.py
--rw-r--r--   0        0        0      876 2023-06-09 17:44:01.405763 thoughtful-2.1.0/thoughtful/supervisor/reporting/step_report.py
--rw-r--r--   0        0        0     1541 2023-06-09 17:44:01.405763 thoughtful-2.1.0/thoughtful/supervisor/reporting/timed_report.py
--rw-r--r--   0        0        0     1754 2023-06-09 17:44:01.405763 thoughtful-2.1.0/thoughtful/supervisor/reporting/timer.py
--rw-r--r--   0        0        0     7756 2023-06-09 17:44:01.405763 thoughtful-2.1.0/thoughtful/supervisor/step_context.py
--rw-r--r--   0        0        0     6441 2023-06-09 17:44:01.405763 thoughtful-2.1.0/thoughtful/supervisor/step_decorator_factory.py
--rw-r--r--   0        0        0        0 2023-06-09 17:44:01.405763 thoughtful-2.1.0/thoughtful/supervisor/streaming/__init__.py
--rw-r--r--   0        0        0      736 2023-06-09 17:44:01.405763 thoughtful-2.1.0/thoughtful/supervisor/streaming/action.py
--rw-r--r--   0        0        0     1347 2023-06-09 17:44:01.405763 thoughtful-2.1.0/thoughtful/supervisor/streaming/jwt_auth.py
--rw-r--r--   0        0        0     3124 2023-06-09 17:44:01.405763 thoughtful-2.1.0/thoughtful/supervisor/streaming/payloads.py
--rw-r--r--   0        0        0     4372 2023-06-09 17:44:01.405763 thoughtful-2.1.0/thoughtful/supervisor/streaming/streamer.py
--rw-r--r--   0        0        0     1352 2023-06-09 17:44:01.405763 thoughtful-2.1.0/thoughtful/supervisor/streaming/token.py
--rw-r--r--   0        0        0     4578 1970-01-01 00:00:00.000000 thoughtful-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-06-13 14:57:06.792305 thoughtful-2.1.1/LICENSE
+-rw-r--r--   0        0        0     2992 2023-06-13 14:57:06.792305 thoughtful-2.1.1/README.md
+-rw-r--r--   0        0        0     1935 2023-06-13 14:57:06.792305 thoughtful-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0      222 2023-06-13 14:57:06.796306 thoughtful-2.1.1/thoughtful/__init__.py
+-rw-r--r--   0        0        0       54 2023-06-13 14:57:06.796306 thoughtful-2.1.1/thoughtful/__version__.py
+-rw-r--r--   0        0        0     1070 2023-06-13 14:57:06.796306 thoughtful-2.1.1/thoughtful/environment_variables.py
+-rw-r--r--   0        0        0      143 2023-06-13 14:57:06.796306 thoughtful-2.1.1/thoughtful/supervisor/__init__.py
+-rw-r--r--   0        0        0     6616 2023-06-13 14:57:06.796306 thoughtful-2.1.1/thoughtful/supervisor/default_instances.py
+-rw-r--r--   0        0        0      922 2023-06-13 14:57:06.796306 thoughtful-2.1.1/thoughtful/supervisor/event_bus.py
+-rw-r--r--   0        0        0     8756 2023-06-13 14:57:06.796306 thoughtful-2.1.1/thoughtful/supervisor/main_context.py
+-rw-r--r--   0        0        0    10567 2023-06-13 14:57:06.796306 thoughtful-2.1.1/thoughtful/supervisor/manifest.py
+-rw-r--r--   0        0        0        0 2023-06-13 14:57:06.796306 thoughtful-2.1.1/thoughtful/supervisor/py.typed
+-rw-r--r--   0        0        0        0 2023-06-13 14:57:06.796306 thoughtful-2.1.1/thoughtful/supervisor/reporting/__init__.py
+-rw-r--r--   0        0        0     2872 2023-06-13 14:57:06.796306 thoughtful-2.1.1/thoughtful/supervisor/reporting/record.py
+-rw-r--r--   0        0        0     1189 2023-06-13 14:57:06.796306 thoughtful-2.1.1/thoughtful/supervisor/reporting/record_report.py
+-rw-r--r--   0        0        0     2066 2023-06-13 14:57:06.796306 thoughtful-2.1.1/thoughtful/supervisor/reporting/report.py
+-rw-r--r--   0        0        0    10118 2023-06-13 14:57:06.796306 thoughtful-2.1.1/thoughtful/supervisor/reporting/report_builder.py
+-rw-r--r--   0        0        0      660 2023-06-13 14:57:06.796306 thoughtful-2.1.1/thoughtful/supervisor/reporting/status.py
+-rw-r--r--   0        0        0      876 2023-06-13 14:57:06.796306 thoughtful-2.1.1/thoughtful/supervisor/reporting/step_report.py
+-rw-r--r--   0        0        0     1541 2023-06-13 14:57:06.796306 thoughtful-2.1.1/thoughtful/supervisor/reporting/timed_report.py
+-rw-r--r--   0        0        0     1754 2023-06-13 14:57:06.796306 thoughtful-2.1.1/thoughtful/supervisor/reporting/timer.py
+-rw-r--r--   0        0        0     7756 2023-06-13 14:57:06.796306 thoughtful-2.1.1/thoughtful/supervisor/step_context.py
+-rw-r--r--   0        0        0     6441 2023-06-13 14:57:06.796306 thoughtful-2.1.1/thoughtful/supervisor/step_decorator_factory.py
+-rw-r--r--   0        0        0        0 2023-06-13 14:57:06.796306 thoughtful-2.1.1/thoughtful/supervisor/streaming/__init__.py
+-rw-r--r--   0        0        0      736 2023-06-13 14:57:06.796306 thoughtful-2.1.1/thoughtful/supervisor/streaming/action.py
+-rw-r--r--   0        0        0     1347 2023-06-13 14:57:06.796306 thoughtful-2.1.1/thoughtful/supervisor/streaming/jwt_auth.py
+-rw-r--r--   0        0        0     3124 2023-06-13 14:57:06.796306 thoughtful-2.1.1/thoughtful/supervisor/streaming/payloads.py
+-rw-r--r--   0        0        0     4372 2023-06-13 14:57:06.796306 thoughtful-2.1.1/thoughtful/supervisor/streaming/streamer.py
+-rw-r--r--   0        0        0     1352 2023-06-13 14:57:06.796306 thoughtful-2.1.1/thoughtful/supervisor/streaming/token.py
+-rw-r--r--   0        0        0     4578 1970-01-01 00:00:00.000000 thoughtful-2.1.1/PKG-INFO
```

### Comparing `thoughtful-2.1.0/LICENSE` & `thoughtful-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `thoughtful-2.1.0/README.md` & `thoughtful-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `thoughtful-2.1.0/pyproject.toml` & `thoughtful-2.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "thoughtful"
-version = "2.1.0"
+version = "2.1.1"
 description = "Thoughtful is a python package by Thoughtful for helping manage automations with helpful packages like supervisor"
 authors = ["Thoughtful Automation <care@thoughtful.ai>"]
 license = "Apache-2.0"
 readme = 'README.md'
 homepage = "https://thoughtful.ai"
 repository = "https://github.com/thoughtful-automation/thoughtful"
 documentation = "https://thoughtful-supervisor.readthedocs-hosted.com/en/latest/index.html"
```

### Comparing `thoughtful-2.1.0/thoughtful/environment_variables.py` & `thoughtful-2.1.1/thoughtful/environment_variables.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.1.0/thoughtful/supervisor/default_instances.py` & `thoughtful-2.1.1/thoughtful/supervisor/default_instances.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.1.0/thoughtful/supervisor/event_bus.py` & `thoughtful-2.1.1/thoughtful/supervisor/event_bus.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.1.0/thoughtful/supervisor/main_context.py` & `thoughtful-2.1.1/thoughtful/supervisor/main_context.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.1.0/thoughtful/supervisor/manifest.py` & `thoughtful-2.1.1/thoughtful/supervisor/manifest.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.1.0/thoughtful/supervisor/reporting/record.py` & `thoughtful-2.1.1/thoughtful/supervisor/reporting/record.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.1.0/thoughtful/supervisor/reporting/record_report.py` & `thoughtful-2.1.1/thoughtful/supervisor/reporting/record_report.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.1.0/thoughtful/supervisor/reporting/report.py` & `thoughtful-2.1.1/thoughtful/supervisor/reporting/report.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.1.0/thoughtful/supervisor/reporting/report_builder.py` & `thoughtful-2.1.1/thoughtful/supervisor/reporting/report_builder.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.1.0/thoughtful/supervisor/reporting/status.py` & `thoughtful-2.1.1/thoughtful/supervisor/reporting/status.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.1.0/thoughtful/supervisor/reporting/step_report.py` & `thoughtful-2.1.1/thoughtful/supervisor/reporting/step_report.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.1.0/thoughtful/supervisor/reporting/timed_report.py` & `thoughtful-2.1.1/thoughtful/supervisor/reporting/timed_report.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.1.0/thoughtful/supervisor/reporting/timer.py` & `thoughtful-2.1.1/thoughtful/supervisor/reporting/timer.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.1.0/thoughtful/supervisor/step_context.py` & `thoughtful-2.1.1/thoughtful/supervisor/step_context.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.1.0/thoughtful/supervisor/step_decorator_factory.py` & `thoughtful-2.1.1/thoughtful/supervisor/step_decorator_factory.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.1.0/thoughtful/supervisor/streaming/action.py` & `thoughtful-2.1.1/thoughtful/supervisor/streaming/action.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.1.0/thoughtful/supervisor/streaming/jwt_auth.py` & `thoughtful-2.1.1/thoughtful/supervisor/streaming/jwt_auth.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.1.0/thoughtful/supervisor/streaming/payloads.py` & `thoughtful-2.1.1/thoughtful/supervisor/streaming/payloads.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.1.0/thoughtful/supervisor/streaming/streamer.py` & `thoughtful-2.1.1/thoughtful/supervisor/streaming/streamer.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.1.0/thoughtful/supervisor/streaming/token.py` & `thoughtful-2.1.1/thoughtful/supervisor/streaming/token.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.1.0/PKG-INFO` & `thoughtful-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thoughtful
-Version: 2.1.0
+Version: 2.1.1
 Summary: Thoughtful is a python package by Thoughtful for helping manage automations with helpful packages like supervisor
 Home-page: https://thoughtful.ai
 License: Apache-2.0
 Keywords: rpa,robot-framework,robocorp,automation
 Author: Thoughtful Automation
 Author-email: care@thoughtful.ai
 Requires-Python: >=3.8,<3.12
```

