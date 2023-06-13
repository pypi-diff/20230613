# Comparing `tmp/fyntex-drf-pagination-utils-1.3.1.tar.gz` & `tmp/fyntex-drf-pagination-utils-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fyntex-drf-pagination-utils-1.3.1.tar", last modified: Tue Mar  7 15:53:17 2023, max compression
+gzip compressed data, was "fyntex-drf-pagination-utils-1.3.2.tar", last modified: Tue Jun 13 16:22:47 2023, max compression
```

## Comparing `fyntex-drf-pagination-utils-1.3.1.tar` & `fyntex-drf-pagination-utils-1.3.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 15:53:17.927503 fyntex-drf-pagination-utils-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-07 15:52:54.000000 fyntex-drf-pagination-utils-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-03-07 15:52:54.000000 fyntex-drf-pagination-utils-1.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-03-07 15:53:17.927503 fyntex-drf-pagination-utils-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-03-07 15:52:54.000000 fyntex-drf-pagination-utils-1.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 15:53:17.927503 fyntex-drf-pagination-utils-1.3.1/fyntex/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-03-07 15:52:54.000000 fyntex-drf-pagination-utils-1.3.1/fyntex/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 15:53:17.927503 fyntex-drf-pagination-utils-1.3.1/fyntex/drf_pagination_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 15:52:54.000000 fyntex-drf-pagination-utils-1.3.1/fyntex/drf_pagination_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 15:52:54.000000 fyntex-drf-pagination-utils-1.3.1/fyntex/drf_pagination_utils/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    11917 2023-03-07 15:52:54.000000 fyntex-drf-pagination-utils-1.3.1/fyntex/drf_pagination_utils/styles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 15:53:17.927503 fyntex-drf-pagination-utils-1.3.1/fyntex/drf_pagination_utils/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 15:52:54.000000 fyntex-drf-pagination-utils-1.3.1/fyntex/drf_pagination_utils/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-03-07 15:52:54.000000 fyntex-drf-pagination-utils-1.3.1/fyntex/drf_pagination_utils/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-03-07 15:52:54.000000 fyntex-drf-pagination-utils-1.3.1/fyntex/drf_pagination_utils/tests/test_styles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 15:53:17.927503 fyntex-drf-pagination-utils-1.3.1/fyntex_drf_pagination_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-03-07 15:53:17.000000 fyntex-drf-pagination-utils-1.3.1/fyntex_drf_pagination_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-03-07 15:53:17.000000 fyntex-drf-pagination-utils-1.3.1/fyntex_drf_pagination_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-07 15:53:17.000000 fyntex-drf-pagination-utils-1.3.1/fyntex_drf_pagination_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-07 15:53:17.000000 fyntex-drf-pagination-utils-1.3.1/fyntex_drf_pagination_utils.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-07 15:53:17.000000 fyntex-drf-pagination-utils-1.3.1/fyntex_drf_pagination_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-07 15:53:17.000000 fyntex-drf-pagination-utils-1.3.1/fyntex_drf_pagination_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-03-07 15:53:17.927503 fyntex-drf-pagination-utils-1.3.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)       62 2023-03-07 15:52:54.000000 fyntex-drf-pagination-utils-1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:22:47.743444 fyntex-drf-pagination-utils-1.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-13 16:22:19.000000 fyntex-drf-pagination-utils-1.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-13 16:22:19.000000 fyntex-drf-pagination-utils-1.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-13 16:22:47.743444 fyntex-drf-pagination-utils-1.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-06-13 16:22:19.000000 fyntex-drf-pagination-utils-1.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:22:47.743444 fyntex-drf-pagination-utils-1.3.2/fyntex/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-13 16:22:19.000000 fyntex-drf-pagination-utils-1.3.2/fyntex/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:22:47.743444 fyntex-drf-pagination-utils-1.3.2/fyntex/drf_pagination_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 16:22:19.000000 fyntex-drf-pagination-utils-1.3.2/fyntex/drf_pagination_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 16:22:19.000000 fyntex-drf-pagination-utils-1.3.2/fyntex/drf_pagination_utils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    11917 2023-06-13 16:22:19.000000 fyntex-drf-pagination-utils-1.3.2/fyntex/drf_pagination_utils/styles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:22:47.743444 fyntex-drf-pagination-utils-1.3.2/fyntex/drf_pagination_utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 16:22:19.000000 fyntex-drf-pagination-utils-1.3.2/fyntex/drf_pagination_utils/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-13 16:22:19.000000 fyntex-drf-pagination-utils-1.3.2/fyntex/drf_pagination_utils/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-13 16:22:19.000000 fyntex-drf-pagination-utils-1.3.2/fyntex/drf_pagination_utils/tests/test_styles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:22:47.743444 fyntex-drf-pagination-utils-1.3.2/fyntex_drf_pagination_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-13 16:22:47.000000 fyntex-drf-pagination-utils-1.3.2/fyntex_drf_pagination_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-13 16:22:47.000000 fyntex-drf-pagination-utils-1.3.2/fyntex_drf_pagination_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 16:22:47.000000 fyntex-drf-pagination-utils-1.3.2/fyntex_drf_pagination_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 16:22:46.000000 fyntex-drf-pagination-utils-1.3.2/fyntex_drf_pagination_utils.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-13 16:22:47.000000 fyntex-drf-pagination-utils-1.3.2/fyntex_drf_pagination_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-13 16:22:47.000000 fyntex-drf-pagination-utils-1.3.2/fyntex_drf_pagination_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-13 16:22:47.743444 fyntex-drf-pagination-utils-1.3.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)       62 2023-06-13 16:22:19.000000 fyntex-drf-pagination-utils-1.3.2/setup.py
```

### Comparing `fyntex-drf-pagination-utils-1.3.1/LICENSE` & `fyntex-drf-pagination-utils-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fyntex-drf-pagination-utils-1.3.1/PKG-INFO` & `fyntex-drf-pagination-utils-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fyntex-drf-pagination-utils
-Version: 1.3.1
+Version: 1.3.2
 Summary: A library that provides custom pagination styles and pagination-related
 Home-page: https://github.com/fyntex/drf-pagination-utils/
 Author: Fyntex TI SpA
 Author-email: no-reply@fyntex.ai
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
```

### Comparing `fyntex-drf-pagination-utils-1.3.1/README.md` & `fyntex-drf-pagination-utils-1.3.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,19 @@
 
 | VCS Branch | Deployment Environment | VCS Repository | CI/CD Status |
 | ---------- | ---------------------- | -------------- | ------------ |
 | `develop` | Staging | [GitHub](https://github.com/fyntex/drf-pagination-utils/tree/develop) | [![GitHub Actions](https://github.com/fyntex/drf-pagination-utils/actions/workflows/ci-cd.yaml/badge.svg?branch=develop)](https://github.com/fyntex/drf-pagination-utils/actions/workflows/ci-cd.yaml?query=branch:develop) |
 | `master` | Production | [GitHub](https://github.com/fyntex/drf-pagination-utils/tree/master)  | [![GitHub Actions](https://github.com/fyntex/drf-pagination-utils/actions/workflows/ci-cd.yaml/badge.svg?branch=master)](https://github.com/fyntex/drf-pagination-utils/actions/workflows/ci-cd.yaml?query=branch:master) |
 
 
+| Code Coverage |
+| ------------- |
+| [![Codecov](https://codecov.io/gh/fyntex/drf-pagination-utils/branch/develop/graph/badge.svg)](https://codecov.io/gh/fyntex/drf-pagination-utils) |
+
+
 ### Hosting
 
 | Deployment Environment | Python Package Registry |
 | ---------------------- | ----------------------- |
 | Production | [PyPI](https://pypi.org/project/fyntex-drf-pagination-utils/)  |
```

### Comparing `fyntex-drf-pagination-utils-1.3.1/fyntex/drf_pagination_utils/styles.py` & `fyntex-drf-pagination-utils-1.3.2/fyntex/drf_pagination_utils/styles.py`

 * *Files identical despite different names*

### Comparing `fyntex-drf-pagination-utils-1.3.1/fyntex/drf_pagination_utils/tests/settings.py` & `fyntex-drf-pagination-utils-1.3.2/fyntex/drf_pagination_utils/tests/settings.py`

 * *Files identical despite different names*

### Comparing `fyntex-drf-pagination-utils-1.3.1/fyntex/drf_pagination_utils/tests/test_styles.py` & `fyntex-drf-pagination-utils-1.3.2/fyntex/drf_pagination_utils/tests/test_styles.py`

 * *Files identical despite different names*

### Comparing `fyntex-drf-pagination-utils-1.3.1/fyntex_drf_pagination_utils.egg-info/PKG-INFO` & `fyntex-drf-pagination-utils-1.3.2/fyntex_drf_pagination_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fyntex-drf-pagination-utils
-Version: 1.3.1
+Version: 1.3.2
 Summary: A library that provides custom pagination styles and pagination-related
 Home-page: https://github.com/fyntex/drf-pagination-utils/
 Author: Fyntex TI SpA
 Author-email: no-reply@fyntex.ai
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
```

### Comparing `fyntex-drf-pagination-utils-1.3.1/fyntex_drf_pagination_utils.egg-info/SOURCES.txt` & `fyntex-drf-pagination-utils-1.3.2/fyntex_drf_pagination_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fyntex-drf-pagination-utils-1.3.1/setup.cfg` & `fyntex-drf-pagination-utils-1.3.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = fyntex-drf-pagination-utils
-version = 1.3.1
+version = 1.3.2
 description = 
 	A library that provides custom pagination styles and pagination-related
 	utilities for Django REST Framework.
 author = Fyntex TI SpA
 author_email = no-reply@fyntex.ai
 url = https://github.com/fyntex/drf-pagination-utils/
 license = MIT
```

