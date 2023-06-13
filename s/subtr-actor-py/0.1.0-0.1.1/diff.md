# Comparing `tmp/subtr_actor_py-0.1.0.tar.gz` & `tmp/subtr_actor_py-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "subtr_actor_py-0.1.0.tar", max compression
+gzip compressed data, was "subtr_actor_py-0.1.1.tar", max compression
```

## Comparing `subtr_actor_py-0.1.0.tar` & `subtr_actor_py-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      100 2023-06-13 08:24:40.792859 subtr_actor_py-0.1.0/README.md
--rw-r--r--   0        0        0      569 2023-06-13 09:13:24.678867 subtr_actor_py-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      143 2023-06-13 08:23:53.279298 subtr_actor_py-0.1.0/subtr_actor/__init__.py
--rw-r--r--   0        0        0      543 2023-06-13 08:16:27.228171 subtr_actor_py-0.1.0/subtr_actor/subtr_actor.pyi
--rw-r--r--   0        0        0      901 1970-01-01 00:00:00.000000 subtr_actor_py-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      100 2023-06-13 08:24:40.792859 subtr_actor_py-0.1.1/README.md
+-rw-r--r--   0        0        0      569 2023-06-13 09:16:20.873912 subtr_actor_py-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      143 2023-06-13 08:23:53.279298 subtr_actor_py-0.1.1/subtr_actor/__init__.py
+-rw-r--r--   0        0        0      543 2023-06-13 08:16:27.228171 subtr_actor_py-0.1.1/subtr_actor/subtr_actor.pyi
+-rw-r--r--   0        0        0      901 1970-01-01 00:00:00.000000 subtr_actor_py-0.1.1/PKG-INFO
```

### Comparing `subtr_actor_py-0.1.0/pyproject.toml` & `subtr_actor_py-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "subtr-actor-py"
-version = "0.1.0"
+version = "0.1.1"
 description = "Python bindings for the Rocket League replay processing library subtr-actor."
 authors = ["Ivan Malison <ivanmalison@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/rlrml/subtr-actor-py"
 packages = [{include = "subtr_actor"}]
```

### Comparing `subtr_actor_py-0.1.0/subtr_actor/subtr_actor.pyi` & `subtr_actor_py-0.1.1/subtr_actor/subtr_actor.pyi`

 * *Files identical despite different names*

### Comparing `subtr_actor_py-0.1.0/PKG-INFO` & `subtr_actor_py-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: subtr-actor-py
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python bindings for the Rocket League replay processing library subtr-actor.
 Home-page: https://github.com/rlrml/subtr-actor-py
 License: MIT
 Author: Ivan Malison
 Author-email: ivanmalison@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

