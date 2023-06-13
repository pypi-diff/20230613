# Comparing `tmp/pymavlog-0.3.0.tar.gz` & `tmp/pymavlog-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymavlog-0.3.0.tar", max compression
+gzip compressed data, was "pymavlog-0.3.1.tar", max compression
```

## Comparing `pymavlog-0.3.0.tar` & `pymavlog-0.3.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1073 2023-05-22 14:09:21.329705 pymavlog-0.3.0/LICENSE
--rw-r--r--   0        0        0     1993 2023-05-22 14:09:21.329705 pymavlog-0.3.0/README.md
--rw-r--r--   0        0        0      196 2023-05-22 14:09:21.329705 pymavlog-0.3.0/pymavlog/__init__.py
--rw-r--r--   0        0        0     9086 2023-05-22 14:09:21.329705 pymavlog-0.3.0/pymavlog/core.py
--rw-r--r--   0        0        0      137 2023-05-22 14:09:21.329705 pymavlog-0.3.0/pymavlog/errors.py
--rw-r--r--   0        0        0      121 2023-05-22 14:09:21.329705 pymavlog-0.3.0/pymavlog/helpers.py
--rw-r--r--   0        0        0     1072 2023-05-22 14:09:32.002008 pymavlog-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     3110 1970-01-01 00:00:00.000000 pymavlog-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-13 07:27:16.807077 pymavlog-0.3.1/LICENSE
+-rw-r--r--   0        0        0     1993 2023-06-13 07:27:16.807077 pymavlog-0.3.1/README.md
+-rw-r--r--   0        0        0      196 2023-06-13 07:27:16.807077 pymavlog-0.3.1/pymavlog/__init__.py
+-rw-r--r--   0        0        0     9086 2023-06-13 07:27:16.807077 pymavlog-0.3.1/pymavlog/core.py
+-rw-r--r--   0        0        0      137 2023-06-13 07:27:16.807077 pymavlog-0.3.1/pymavlog/errors.py
+-rw-r--r--   0        0        0      121 2023-06-13 07:27:16.807077 pymavlog-0.3.1/pymavlog/helpers.py
+-rw-r--r--   0        0        0     1072 2023-06-13 07:27:26.143138 pymavlog-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     3110 1970-01-01 00:00:00.000000 pymavlog-0.3.1/PKG-INFO
```

### Comparing `pymavlog-0.3.0/LICENSE` & `pymavlog-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pymavlog-0.3.0/README.md` & `pymavlog-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `pymavlog-0.3.0/pymavlog/core.py` & `pymavlog-0.3.1/pymavlog/core.py`

 * *Files identical despite different names*

### Comparing `pymavlog-0.3.0/pyproject.toml` & `pymavlog-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pymavlog"
-version = "0.3.0"
+version = "0.3.1"
 description = "A lightweight python library to parse MavLink log files"
 readme = "README.md"
 license = "MIT"
 authors = [
     "Ricardo Martinez <rik@rmargar.net>"
 ]
 classifiers = [
```

### Comparing `pymavlog-0.3.0/PKG-INFO` & `pymavlog-0.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymavlog
-Version: 0.3.0
+Version: 0.3.1
 Summary: A lightweight python library to parse MavLink log files
 Home-page: https://github.com/rmargar/pymavlog
 License: MIT
 Author: Ricardo Martinez
 Author-email: rik@rmargar.net
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 1 - Planning
```

