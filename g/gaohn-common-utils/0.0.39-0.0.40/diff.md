# Comparing `tmp/gaohn-common-utils-0.0.39.tar.gz` & `tmp/gaohn-common-utils-0.0.40.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gaohn-common-utils-0.0.39.tar", last modified: Tue Jun 13 03:13:15 2023, max compression
+gzip compressed data, was "gaohn-common-utils-0.0.40.tar", last modified: Tue Jun 13 05:04:13 2023, max compression
```

## Comparing `gaohn-common-utils-0.0.39.tar` & `gaohn-common-utils-0.0.40.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:13:15.250583 gaohn-common-utils-0.0.39/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-13 03:12:52.000000 gaohn-common-utils-0.0.39/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-06-13 03:13:15.250583 gaohn-common-utils-0.0.39/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-06-13 03:12:52.000000 gaohn-common-utils-0.0.39/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:13:15.246583 gaohn-common-utils-0.0.39/common_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 03:12:52.000000 gaohn-common-utils-0.0.39/common_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:13:15.246583 gaohn-common-utils-0.0.39/common_utils/cloud/
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-13 03:12:52.000000 gaohn-common-utils-0.0.39/common_utils/cloud/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:13:15.246583 gaohn-common-utils-0.0.39/common_utils/cloud/gcp/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:13:15.246583 gaohn-common-utils-0.0.39/common_utils/cloud/gcp/storage/
--rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-06-13 03:12:52.000000 gaohn-common-utils-0.0.39/common_utils/cloud/gcp/storage/bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-06-13 03:12:52.000000 gaohn-common-utils-0.0.39/common_utils/cloud/gcp/storage/gcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:13:15.250583 gaohn-common-utils-0.0.39/common_utils/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 03:12:52.000000 gaohn-common-utils-0.0.39/common_utils/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-13 03:12:52.000000 gaohn-common-utils-0.0.39/common_utils/core/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-13 03:12:52.000000 gaohn-common-utils-0.0.39/common_utils/core/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-06-13 03:12:52.000000 gaohn-common-utils-0.0.39/common_utils/core/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-06-13 03:12:52.000000 gaohn-common-utils-0.0.39/common_utils/core/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-06-13 03:12:52.000000 gaohn-common-utils-0.0.39/common_utils/core/file_system_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-06-13 03:12:52.000000 gaohn-common-utils-0.0.39/common_utils/core/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:13:15.250583 gaohn-common-utils-0.0.39/common_utils/orchestrator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 03:12:52.000000 gaohn-common-utils-0.0.39/common_utils/orchestrator/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:13:15.246583 gaohn-common-utils-0.0.39/common_utils/versioning/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:13:15.250583 gaohn-common-utils-0.0.39/common_utils/versioning/dvc/
--rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-06-13 03:12:52.000000 gaohn-common-utils-0.0.39/common_utils/versioning/dvc/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:13:15.250583 gaohn-common-utils-0.0.39/gaohn_common_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-06-13 03:13:15.000000 gaohn-common-utils-0.0.39/gaohn_common_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-06-13 03:13:15.000000 gaohn-common-utils-0.0.39/gaohn_common_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 03:13:15.000000 gaohn-common-utils-0.0.39/gaohn_common_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-13 03:13:15.000000 gaohn-common-utils-0.0.39/gaohn_common_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-13 03:13:15.000000 gaohn-common-utils-0.0.39/gaohn_common_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-06-13 03:12:52.000000 gaohn-common-utils-0.0.39/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 03:13:15.250583 gaohn-common-utils-0.0.39/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:04:13.003798 gaohn-common-utils-0.0.40/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-13 05:03:54.000000 gaohn-common-utils-0.0.40/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-06-13 05:04:13.003798 gaohn-common-utils-0.0.40/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-06-13 05:03:54.000000 gaohn-common-utils-0.0.40/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:04:13.003798 gaohn-common-utils-0.0.40/common_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 05:03:54.000000 gaohn-common-utils-0.0.40/common_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:04:13.003798 gaohn-common-utils-0.0.40/common_utils/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-13 05:03:54.000000 gaohn-common-utils-0.0.40/common_utils/cloud/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:04:12.999798 gaohn-common-utils-0.0.40/common_utils/cloud/gcp/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:04:13.003798 gaohn-common-utils-0.0.40/common_utils/cloud/gcp/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-06-13 05:03:54.000000 gaohn-common-utils-0.0.40/common_utils/cloud/gcp/storage/bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-06-13 05:03:54.000000 gaohn-common-utils-0.0.40/common_utils/cloud/gcp/storage/gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:04:13.003798 gaohn-common-utils-0.0.40/common_utils/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 05:03:54.000000 gaohn-common-utils-0.0.40/common_utils/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-13 05:03:54.000000 gaohn-common-utils-0.0.40/common_utils/core/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-06-13 05:03:54.000000 gaohn-common-utils-0.0.40/common_utils/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-06-13 05:03:54.000000 gaohn-common-utils-0.0.40/common_utils/core/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-06-13 05:03:54.000000 gaohn-common-utils-0.0.40/common_utils/core/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-06-13 05:03:54.000000 gaohn-common-utils-0.0.40/common_utils/core/file_system_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-06-13 05:03:54.000000 gaohn-common-utils-0.0.40/common_utils/core/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:04:13.003798 gaohn-common-utils-0.0.40/common_utils/orchestrator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 05:03:54.000000 gaohn-common-utils-0.0.40/common_utils/orchestrator/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:04:12.999798 gaohn-common-utils-0.0.40/common_utils/versioning/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:04:13.003798 gaohn-common-utils-0.0.40/common_utils/versioning/dvc/
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-06-13 05:03:54.000000 gaohn-common-utils-0.0.40/common_utils/versioning/dvc/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:04:13.003798 gaohn-common-utils-0.0.40/gaohn_common_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-06-13 05:04:12.000000 gaohn-common-utils-0.0.40/gaohn_common_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-06-13 05:04:12.000000 gaohn-common-utils-0.0.40/gaohn_common_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 05:04:12.000000 gaohn-common-utils-0.0.40/gaohn_common_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-13 05:04:12.000000 gaohn-common-utils-0.0.40/gaohn_common_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-13 05:04:12.000000 gaohn-common-utils-0.0.40/gaohn_common_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-06-13 05:03:54.000000 gaohn-common-utils-0.0.40/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 05:04:13.003798 gaohn-common-utils-0.0.40/setup.cfg
```

### Comparing `gaohn-common-utils-0.0.39/LICENSE` & `gaohn-common-utils-0.0.40/LICENSE`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.39/PKG-INFO` & `gaohn-common-utils-0.0.40/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaohn-common-utils
-Version: 0.0.39
+Version: 0.0.40
 Summary: A small utility package
 Author-email: Gao Hongnan <hongnangao@gmail.com>
 Project-URL: Homepage, https://github.com/gao-hongnan/common-utils
 Project-URL: Bug Tracker, https://github.com/gao-hongnan/common-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gaohn-common-utils-0.0.39/README.md` & `gaohn-common-utils-0.0.40/README.md`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.39/common_utils/cloud/base.py` & `gaohn-common-utils-0.0.40/common_utils/cloud/base.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.39/common_utils/cloud/gcp/storage/bigquery.py` & `gaohn-common-utils-0.0.40/common_utils/cloud/gcp/storage/bigquery.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.39/common_utils/cloud/gcp/storage/gcs.py` & `gaohn-common-utils-0.0.40/common_utils/cloud/gcp/storage/gcs.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.39/common_utils/core/artifacts.py` & `gaohn-common-utils-0.0.40/common_utils/core/artifacts.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.39/common_utils/core/base.py` & `gaohn-common-utils-0.0.40/common_utils/core/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,52 @@
 from abc import ABC, abstractmethod
 from typing import Any, Dict
 
 
 class DictPersistence(ABC):
+    """Abstract class for saving and loading dictionary."""
+
     @abstractmethod
     def save_as_dict(
         self, data: Dict[str, Any], filepath: str, **kwargs: Dict[str, Any]
     ) -> None:
         """Save a dictionary to a specific location."""
 
     @abstractmethod
     def load_to_dict(self, filepath: str, **kwargs: Dict[str, Any]) -> Dict[str, Any]:
         """Load a dictionary from a filepath."""
 
+
 class Connection(ABC):
+    """Abstract class for database connection."""
+
     @abstractmethod
     def connect(self) -> None:
         """Connect to a database."""
 
     @abstractmethod
     def disconnect(self) -> None:
         """Disconnect from a database."""
 
     @abstractmethod
     def query(self, query: str) -> Any:
-        """Query a database."""
+        """Query a database."""
+
+
+class Storage(ABC):
+    """Abstract class for storage."""
+
+    @abstractmethod
+    def save_file(self) -> None:
+        """Save a file to a specific location."""
+
+    @abstractmethod
+    def save_files(self) -> None:
+        """Save multiple files to a specific location."""
+
+    @abstractmethod
+    def load_file(self) -> None:
+        """Load a file from a specific location."""
+
+    @abstractmethod
+    def load_files(self) -> None:
+        """Load multiple files from a specific location."""
```

### Comparing `gaohn-common-utils-0.0.39/common_utils/core/common.py` & `gaohn-common-utils-0.0.40/common_utils/core/common.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.39/common_utils/core/decorators.py` & `gaohn-common-utils-0.0.40/common_utils/core/decorators.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.39/common_utils/core/file_system_utils.py` & `gaohn-common-utils-0.0.40/common_utils/core/file_system_utils.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.39/common_utils/core/logger.py` & `gaohn-common-utils-0.0.40/common_utils/core/logger.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.39/common_utils/versioning/dvc/base.py` & `gaohn-common-utils-0.0.40/common_utils/versioning/dvc/base.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.39/gaohn_common_utils.egg-info/PKG-INFO` & `gaohn-common-utils-0.0.40/gaohn_common_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaohn-common-utils
-Version: 0.0.39
+Version: 0.0.40
 Summary: A small utility package
 Author-email: Gao Hongnan <hongnangao@gmail.com>
 Project-URL: Homepage, https://github.com/gao-hongnan/common-utils
 Project-URL: Bug Tracker, https://github.com/gao-hongnan/common-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gaohn-common-utils-0.0.39/gaohn_common_utils.egg-info/SOURCES.txt` & `gaohn-common-utils-0.0.40/gaohn_common_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.39/pyproject.toml` & `gaohn-common-utils-0.0.40/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gaohn-common-utils"
-version = "0.0.39"
+version = "0.0.40"
 authors = [
   { name="Gao Hongnan", email="hongnangao@gmail.com" },
 ]
 description = "A small utility package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

