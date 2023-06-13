# Comparing `tmp/decimal128-1.0.0.tar.gz` & `tmp/decimal128-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decimal128-1.0.0.tar", max compression
+gzip compressed data, was "decimal128-1.0.1.tar", max compression
```

## Comparing `decimal128-1.0.0.tar` & `decimal128-1.0.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2023-06-10 09:25:30.302765 decimal128-1.0.0/LICENSE
--rw-r--r--   0        0        0     6082 2023-06-12 17:43:43.361192 decimal128-1.0.0/README.md
--rw-r--r--   0        0        0       72 2023-06-10 09:25:30.310572 decimal128-1.0.0/decimal128/__init__.py
--rw-r--r--   0        0        0    10023 2023-06-12 17:58:18.244548 decimal128-1.0.0/decimal128/decimal128.py
--rw-r--r--   0        0        0     1326 2023-06-11 11:30:07.602859 decimal128-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     6770 1970-01-01 00:00:00.000000 decimal128-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-10 09:25:30.302765 decimal128-1.0.1/LICENSE
+-rw-r--r--   0        0        0     6082 2023-06-12 17:43:43.361192 decimal128-1.0.1/README.md
+-rw-r--r--   0        0        0       72 2023-06-10 09:25:30.310572 decimal128-1.0.1/decimal128/__init__.py
+-rw-r--r--   0        0        0    10023 2023-06-12 17:58:18.244548 decimal128-1.0.1/decimal128/decimal128.py
+-rw-r--r--   0        0        0     1333 2023-06-13 13:37:07.337431 decimal128-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     6789 1970-01-01 00:00:00.000000 decimal128-1.0.1/PKG-INFO
```

### Comparing `decimal128-1.0.0/LICENSE` & `decimal128-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `decimal128-1.0.0/README.md` & `decimal128-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `decimal128-1.0.0/decimal128/decimal128.py` & `decimal128-1.0.1/decimal128/decimal128.py`

 * *Files identical despite different names*

### Comparing `decimal128-1.0.0/pyproject.toml` & `decimal128-1.0.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 authors = ["Jon Connell <python@figsandfudge.com>"]
 classifiers = [
   "Programming Language :: Python :: 3",
   "Operating System :: OS Independent",
 ]
 description = ""
 documentation = "https://github.com/masaccio/decimal128/blob/main/README.md"
-license = "MIT"
+license = "Apache-2.0"
 name = "decimal128"
 packages = [{include = "decimal128"}]
 readme = "README.md"
-version = "1.0.0"
+version = "1.0.1"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 
 [tool.poetry.group.dev.dependencies]
 black = {version = "^22.10.0", allow-prereleases = true}
 pylama = "^8.4.1"
```

### Comparing `decimal128-1.0.0/PKG-INFO` & `decimal128-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: decimal128
-Version: 1.0.0
+Version: 1.0.1
 Summary: 
-License: MIT
+License: Apache-2.0
 Author: Jon Connell
 Author-email: python@figsandfudge.com
 Requires-Python: >=3.8,<4.0
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
```

