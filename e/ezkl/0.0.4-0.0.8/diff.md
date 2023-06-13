# Comparing `tmp/ezkl-0.0.4.tar.gz` & `tmp/ezkl-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezkl-0.0.4.tar", max compression
+gzip compressed data, was "ezkl-0.0.8.tar", max compression
```

## Comparing `ezkl-0.0.4.tar` & `ezkl-0.0.8.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2023-06-07 15:16:07.799754 ezkl-0.0.4/LICENSE
--rw-r--r--   0        0        0     2307 2023-06-07 15:16:07.799754 ezkl-0.0.4/README.md
--rw-r--r--   0        0        0      273 2023-06-07 15:16:07.799754 ezkl-0.0.4/ezkl/__init__.py
--rw-r--r--   0        0        0     3232 2023-06-07 15:16:07.799754 ezkl-0.0.4/ezkl/export.py
--rw-r--r--   0        0        0      879 2023-06-07 15:16:20.439833 ezkl-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     3182 1970-01-01 00:00:00.000000 ezkl-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-13 19:36:57.630006 ezkl-0.0.8/LICENSE
+-rw-r--r--   0        0        0     2412 2023-06-13 19:36:57.630006 ezkl-0.0.8/README.md
+-rw-r--r--   0        0        0      273 2023-06-13 19:36:57.630006 ezkl-0.0.8/ezkl/__init__.py
+-rw-r--r--   0        0        0     3232 2023-06-13 19:36:57.630006 ezkl-0.0.8/ezkl/export.py
+-rw-r--r--   0        0        0      890 2023-06-13 19:37:11.898189 ezkl-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     3307 1970-01-01 00:00:00.000000 ezkl-0.0.8/PKG-INFO
```

### Comparing `ezkl-0.0.4/LICENSE` & `ezkl-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ezkl-0.0.4/README.md` & `ezkl-0.0.8/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,11 @@
-# ezkl_python
-A library for using and testing ezkl from Python. The main purpose of this repository is to provide Python bindings for [ezkl](https://github.com/zkonduit/ezkl) and to provide simple tools for generating `.onnx` and `.json` input files that can be ingested by it.
+# ezkl
+`pip install ezkl` lets you use [ezkl](https://github.com/zkonduit/ezkl) directly from Python. It also contains an `export` function to generate `.onnx` and `.json` input files that can be ingested by the `ezkl` cli or from Python. [Here is colab notebook](https://colab.research.google.com/drive/1XuXNKqH7axOelZXyU3gpoTOCvFetIsKu?usp=sharing) that shows how to produce and verify a proof from Python.
 
-
-```
-pyezkl/
-├── ezkl/
-|
-└── examples/
-    └── tutorial/ (a tutorial for generating ezkl .onnx and .json inputs)
-```
+Check out [the docs](https://docs.ezkl.xyz) for more. If you want to *develop* the Python bindings, read on.
 
 ## development setup
 
 ### poetry
 
 Use this following setup if you would like to access developmental features in the main ezkl repo that is not released yet.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `ezkl-0.0.4/ezkl/export.py` & `ezkl-0.0.8/ezkl/export.py`

 * *Files identical despite different names*

### Comparing `ezkl-0.0.4/pyproject.toml` & `ezkl-0.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ezkl"
-version = "0.0.4"
+version = "0.0.8"
 description = "Easy zero-knowledge learning in Python"
 authors = [
   "Jason Morton <jason@zkonduit.com>",
   "Dante Camuto <jason@zkonduit.com>",
 ]
 readme = "README.md"
 license = "Apache-2.0"
@@ -17,14 +17,15 @@
     "Operating System :: OS Independent",
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.7"
 numpy = "*"
 torch = "*"
+onnx = "*"
 ezkl_lib = ">=0.1.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 
 [build-system]
 requires = ["poetry-core>=1.4.2"]
```

