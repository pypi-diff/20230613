# Comparing `tmp/gaohn-common-utils-0.0.41.tar.gz` & `tmp/gaohn-common-utils-0.0.42.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gaohn-common-utils-0.0.41.tar", last modified: Tue Jun 13 06:06:52 2023, max compression
+gzip compressed data, was "gaohn-common-utils-0.0.42.tar", last modified: Tue Jun 13 07:02:03 2023, max compression
```

## Comparing `gaohn-common-utils-0.0.41.tar` & `gaohn-common-utils-0.0.42.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:06:52.125414 gaohn-common-utils-0.0.41/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-13 06:06:29.000000 gaohn-common-utils-0.0.41/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-06-13 06:06:52.125414 gaohn-common-utils-0.0.41/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-06-13 06:06:29.000000 gaohn-common-utils-0.0.41/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:06:52.125414 gaohn-common-utils-0.0.41/common_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 06:06:29.000000 gaohn-common-utils-0.0.41/common_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:06:52.125414 gaohn-common-utils-0.0.41/common_utils/cloud/
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-13 06:06:29.000000 gaohn-common-utils-0.0.41/common_utils/cloud/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:06:52.121414 gaohn-common-utils-0.0.41/common_utils/cloud/gcp/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:06:52.125414 gaohn-common-utils-0.0.41/common_utils/cloud/gcp/database/
--rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-06-13 06:06:29.000000 gaohn-common-utils-0.0.41/common_utils/cloud/gcp/database/bigquery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:06:52.125414 gaohn-common-utils-0.0.41/common_utils/cloud/gcp/storage/
--rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-06-13 06:06:29.000000 gaohn-common-utils-0.0.41/common_utils/cloud/gcp/storage/gcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:06:52.125414 gaohn-common-utils-0.0.41/common_utils/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 06:06:29.000000 gaohn-common-utils-0.0.41/common_utils/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-13 06:06:29.000000 gaohn-common-utils-0.0.41/common_utils/core/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-06-13 06:06:29.000000 gaohn-common-utils-0.0.41/common_utils/core/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-06-13 06:06:29.000000 gaohn-common-utils-0.0.41/common_utils/core/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-06-13 06:06:29.000000 gaohn-common-utils-0.0.41/common_utils/core/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-06-13 06:06:29.000000 gaohn-common-utils-0.0.41/common_utils/core/file_system_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-06-13 06:06:29.000000 gaohn-common-utils-0.0.41/common_utils/core/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:06:52.125414 gaohn-common-utils-0.0.41/common_utils/orchestrator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 06:06:29.000000 gaohn-common-utils-0.0.41/common_utils/orchestrator/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:06:52.125414 gaohn-common-utils-0.0.41/common_utils/versioning/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:06:52.125414 gaohn-common-utils-0.0.41/common_utils/versioning/dvc/
--rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-06-13 06:06:29.000000 gaohn-common-utils-0.0.41/common_utils/versioning/dvc/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:06:52.125414 gaohn-common-utils-0.0.41/gaohn_common_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-06-13 06:06:52.000000 gaohn-common-utils-0.0.41/gaohn_common_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-13 06:06:52.000000 gaohn-common-utils-0.0.41/gaohn_common_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 06:06:52.000000 gaohn-common-utils-0.0.41/gaohn_common_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-13 06:06:52.000000 gaohn-common-utils-0.0.41/gaohn_common_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-13 06:06:52.000000 gaohn-common-utils-0.0.41/gaohn_common_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-06-13 06:06:29.000000 gaohn-common-utils-0.0.41/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 06:06:52.125414 gaohn-common-utils-0.0.41/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:02:03.649492 gaohn-common-utils-0.0.42/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-13 07:01:46.000000 gaohn-common-utils-0.0.42/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-06-13 07:02:03.649492 gaohn-common-utils-0.0.42/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-06-13 07:01:46.000000 gaohn-common-utils-0.0.42/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:02:03.645491 gaohn-common-utils-0.0.42/common_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 07:01:46.000000 gaohn-common-utils-0.0.42/common_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:02:03.645491 gaohn-common-utils-0.0.42/common_utils/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-13 07:01:46.000000 gaohn-common-utils-0.0.42/common_utils/cloud/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:02:03.645491 gaohn-common-utils-0.0.42/common_utils/cloud/gcp/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:02:03.645491 gaohn-common-utils-0.0.42/common_utils/cloud/gcp/database/
+-rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-06-13 07:01:46.000000 gaohn-common-utils-0.0.42/common_utils/cloud/gcp/database/bigquery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:02:03.645491 gaohn-common-utils-0.0.42/common_utils/cloud/gcp/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-06-13 07:01:46.000000 gaohn-common-utils-0.0.42/common_utils/cloud/gcp/storage/gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:02:03.645491 gaohn-common-utils-0.0.42/common_utils/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 07:01:46.000000 gaohn-common-utils-0.0.42/common_utils/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-13 07:01:46.000000 gaohn-common-utils-0.0.42/common_utils/core/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-06-13 07:01:46.000000 gaohn-common-utils-0.0.42/common_utils/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-06-13 07:01:46.000000 gaohn-common-utils-0.0.42/common_utils/core/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-06-13 07:01:46.000000 gaohn-common-utils-0.0.42/common_utils/core/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-06-13 07:01:46.000000 gaohn-common-utils-0.0.42/common_utils/core/file_system_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-06-13 07:01:46.000000 gaohn-common-utils-0.0.42/common_utils/core/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:02:03.645491 gaohn-common-utils-0.0.42/common_utils/orchestrator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 07:01:46.000000 gaohn-common-utils-0.0.42/common_utils/orchestrator/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:02:03.645491 gaohn-common-utils-0.0.42/common_utils/versioning/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:02:03.649492 gaohn-common-utils-0.0.42/common_utils/versioning/dvc/
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-06-13 07:01:46.000000 gaohn-common-utils-0.0.42/common_utils/versioning/dvc/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:02:03.649492 gaohn-common-utils-0.0.42/gaohn_common_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-06-13 07:02:03.000000 gaohn-common-utils-0.0.42/gaohn_common_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-13 07:02:03.000000 gaohn-common-utils-0.0.42/gaohn_common_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 07:02:03.000000 gaohn-common-utils-0.0.42/gaohn_common_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-13 07:02:03.000000 gaohn-common-utils-0.0.42/gaohn_common_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-13 07:02:03.000000 gaohn-common-utils-0.0.42/gaohn_common_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-06-13 07:01:46.000000 gaohn-common-utils-0.0.42/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 07:02:03.649492 gaohn-common-utils-0.0.42/setup.cfg
```

### Comparing `gaohn-common-utils-0.0.41/LICENSE` & `gaohn-common-utils-0.0.42/LICENSE`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.41/PKG-INFO` & `gaohn-common-utils-0.0.42/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaohn-common-utils
-Version: 0.0.41
+Version: 0.0.42
 Summary: A small utility package
 Author-email: Gao Hongnan <hongnangao@gmail.com>
 Project-URL: Homepage, https://github.com/gao-hongnan/common-utils
 Project-URL: Bug Tracker, https://github.com/gao-hongnan/common-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gaohn-common-utils-0.0.41/README.md` & `gaohn-common-utils-0.0.42/README.md`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.41/common_utils/cloud/base.py` & `gaohn-common-utils-0.0.42/common_utils/cloud/base.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.41/common_utils/cloud/gcp/database/bigquery.py` & `gaohn-common-utils-0.0.42/common_utils/cloud/gcp/database/bigquery.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.41/common_utils/cloud/gcp/storage/gcs.py` & `gaohn-common-utils-0.0.42/common_utils/cloud/gcp/storage/gcs.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.41/common_utils/core/artifacts.py` & `gaohn-common-utils-0.0.42/common_utils/core/artifacts.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.41/common_utils/core/base.py` & `gaohn-common-utils-0.0.42/common_utils/core/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,14 +16,17 @@
         """Load a dictionary from a filepath."""
 
 
 class Connection(ABC):
     """Abstract class for database connection.
 
     See common_utils/cloud/gcp/database/bigquery.py for example.
+
+    NOTE:
+        1. In particular, it should have a property or attribute table_name.
     """
 
     @abstractmethod
     def connect(self) -> None:
         """Connect to a database."""
 
     @abstractmethod
@@ -36,16 +39,17 @@
 
 
 class Storage(ABC):
     """Abstract class for storage.
 
     See common_utils/cloud/gcp/storage/gcs.py for example.
 
-    Subsequent cloud storages should abide by this interface. This means
-    turning S3, Azure, etc. into a class that inherits from this class.
+    NOTE:
+        1. Subsequent cloud storages should abide by this interface. This means
+            turning S3, Azure, etc. into a class that inherits from this class.
     """
 
     @abstractmethod
     def upload_blob(self) -> None:
         """Save a file to a specific location."""
 
     @abstractmethod
```

### Comparing `gaohn-common-utils-0.0.41/common_utils/core/common.py` & `gaohn-common-utils-0.0.42/common_utils/core/common.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.41/common_utils/core/decorators.py` & `gaohn-common-utils-0.0.42/common_utils/core/decorators.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.41/common_utils/core/file_system_utils.py` & `gaohn-common-utils-0.0.42/common_utils/core/file_system_utils.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.41/common_utils/versioning/dvc/base.py` & `gaohn-common-utils-0.0.42/common_utils/versioning/dvc/base.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.41/gaohn_common_utils.egg-info/PKG-INFO` & `gaohn-common-utils-0.0.42/gaohn_common_utils.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaohn-common-utils
-Version: 0.0.41
+Version: 0.0.42
 Summary: A small utility package
 Author-email: Gao Hongnan <hongnangao@gmail.com>
 Project-URL: Homepage, https://github.com/gao-hongnan/common-utils
 Project-URL: Bug Tracker, https://github.com/gao-hongnan/common-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gaohn-common-utils-0.0.41/gaohn_common_utils.egg-info/SOURCES.txt` & `gaohn-common-utils-0.0.42/gaohn_common_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.41/pyproject.toml` & `gaohn-common-utils-0.0.42/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gaohn-common-utils"
-version = "0.0.41"
+version = "0.0.42"
 authors = [
   { name="Gao Hongnan", email="hongnangao@gmail.com" },
 ]
 description = "A small utility package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

