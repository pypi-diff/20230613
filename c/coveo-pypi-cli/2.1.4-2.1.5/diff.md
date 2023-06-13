# Comparing `tmp/coveo_pypi_cli-2.1.4.tar.gz` & `tmp/coveo_pypi_cli-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coveo_pypi_cli-2.1.4.tar", max compression
+gzip compressed data, was "coveo_pypi_cli-2.1.5.tar", max compression
```

## Comparing `coveo_pypi_cli-2.1.4.tar` & `coveo_pypi_cli-2.1.5.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     3035 2023-02-16 21:12:53.867776 coveo_pypi_cli-2.1.4/README.md
--rw-r--r--   0        0        0        0 2023-02-16 21:12:53.867776 coveo_pypi_cli-2.1.4/coveo_pypi_cli/__init__.py
--rw-r--r--   0        0        0       79 2023-02-16 21:12:53.867776 coveo_pypi_cli-2.1.4/coveo_pypi_cli/__main__.py
--rw-r--r--   0        0        0     2802 2023-02-16 21:12:53.867776 coveo_pypi_cli-2.1.4/coveo_pypi_cli/cli.py
--rw-r--r--   0        0        0      144 2023-02-16 21:12:53.867776 coveo_pypi_cli-2.1.4/coveo_pypi_cli/exceptions.py
--rw-r--r--   0        0        0        0 2023-02-16 21:12:53.867776 coveo_pypi_cli-2.1.4/coveo_pypi_cli/py.typed
--rw-r--r--   0        0        0     3587 2023-02-16 21:12:53.867776 coveo_pypi_cli-2.1.4/coveo_pypi_cli/pypi.py
--rw-r--r--   0        0        0     2291 2023-02-16 21:12:53.867776 coveo_pypi_cli-2.1.4/coveo_pypi_cli/versions.py
--rw-r--r--   0        0        0     1219 2023-02-16 21:13:25.207724 coveo_pypi_cli-2.1.4/pyproject.toml
--rw-r--r--   0        0        0     3985 1970-01-01 00:00:00.000000 coveo_pypi_cli-2.1.4/setup.py
--rw-r--r--   0        0        0     3903 1970-01-01 00:00:00.000000 coveo_pypi_cli-2.1.4/PKG-INFO
+-rw-r--r--   0        0        0     3035 2023-06-13 15:51:21.749218 coveo_pypi_cli-2.1.5/README.md
+-rw-r--r--   0        0        0        0 2023-06-13 15:51:21.749218 coveo_pypi_cli-2.1.5/coveo_pypi_cli/__init__.py
+-rw-r--r--   0        0        0       79 2023-06-13 15:51:21.749218 coveo_pypi_cli-2.1.5/coveo_pypi_cli/__main__.py
+-rw-r--r--   0        0        0     2802 2023-06-13 15:51:21.749218 coveo_pypi_cli-2.1.5/coveo_pypi_cli/cli.py
+-rw-r--r--   0        0        0      144 2023-06-13 15:51:21.749218 coveo_pypi_cli-2.1.5/coveo_pypi_cli/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-13 15:51:21.749218 coveo_pypi_cli-2.1.5/coveo_pypi_cli/py.typed
+-rw-r--r--   0        0        0     3587 2023-06-13 15:51:21.749218 coveo_pypi_cli-2.1.5/coveo_pypi_cli/pypi.py
+-rw-r--r--   0        0        0     2291 2023-06-13 15:51:21.749218 coveo_pypi_cli-2.1.5/coveo_pypi_cli/versions.py
+-rw-r--r--   0        0        0     1219 2023-06-13 15:51:53.853287 coveo_pypi_cli-2.1.5/pyproject.toml
+-rw-r--r--   0        0        0     3903 1970-01-01 00:00:00.000000 coveo_pypi_cli-2.1.5/PKG-INFO
```

### Comparing `coveo_pypi_cli-2.1.4/README.md` & `coveo_pypi_cli-2.1.5/README.md`

 * *Files identical despite different names*

### Comparing `coveo_pypi_cli-2.1.4/coveo_pypi_cli/cli.py` & `coveo_pypi_cli-2.1.5/coveo_pypi_cli/cli.py`

 * *Files identical despite different names*

### Comparing `coveo_pypi_cli-2.1.4/coveo_pypi_cli/pypi.py` & `coveo_pypi_cli-2.1.5/coveo_pypi_cli/pypi.py`

 * *Files identical despite different names*

### Comparing `coveo_pypi_cli-2.1.4/coveo_pypi_cli/versions.py` & `coveo_pypi_cli-2.1.5/coveo_pypi_cli/versions.py`

 * *Files identical despite different names*

### Comparing `coveo_pypi_cli-2.1.4/pyproject.toml` & `coveo_pypi_cli-2.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "coveo-pypi-cli"
-version = "2.1.4"
+version = "2.1.5"
 description = "Query and compute pypi versions from command line."
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/coveooss/coveo-python-oss/tree/main/coveo-pypi-cli"
 authors = ["Jonathan Piché <tools@coveo.com>"]
 
 [tool.poetry.dependencies]
```

### Comparing `coveo_pypi_cli-2.1.4/PKG-INFO` & `coveo_pypi_cli-2.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coveo-pypi-cli
-Version: 2.1.4
+Version: 2.1.5
 Summary: Query and compute pypi versions from command line.
 Home-page: https://github.com/coveooss/coveo-python-oss/tree/main/coveo-pypi-cli
 License: Apache-2.0
 Author: Jonathan Piché
 Author-email: tools@coveo.com
 Requires-Python: >=3.8,<4
 Classifier: License :: OSI Approved :: Apache Software License
```

