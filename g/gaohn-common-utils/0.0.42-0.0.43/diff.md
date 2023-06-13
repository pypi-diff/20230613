# Comparing `tmp/gaohn-common-utils-0.0.42.tar.gz` & `tmp/gaohn-common-utils-0.0.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gaohn-common-utils-0.0.42.tar", last modified: Tue Jun 13 07:02:03 2023, max compression
+gzip compressed data, was "gaohn-common-utils-0.0.43.tar", last modified: Tue Jun 13 07:23:39 2023, max compression
```

## Comparing `gaohn-common-utils-0.0.42.tar` & `gaohn-common-utils-0.0.43.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:02:03.649492 gaohn-common-utils-0.0.42/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-13 07:01:46.000000 gaohn-common-utils-0.0.42/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-06-13 07:02:03.649492 gaohn-common-utils-0.0.42/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-06-13 07:01:46.000000 gaohn-common-utils-0.0.42/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:02:03.645491 gaohn-common-utils-0.0.42/common_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 07:01:46.000000 gaohn-common-utils-0.0.42/common_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:02:03.645491 gaohn-common-utils-0.0.42/common_utils/cloud/
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-13 07:01:46.000000 gaohn-common-utils-0.0.42/common_utils/cloud/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:02:03.645491 gaohn-common-utils-0.0.42/common_utils/cloud/gcp/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:02:03.645491 gaohn-common-utils-0.0.42/common_utils/cloud/gcp/database/
--rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-06-13 07:01:46.000000 gaohn-common-utils-0.0.42/common_utils/cloud/gcp/database/bigquery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:02:03.645491 gaohn-common-utils-0.0.42/common_utils/cloud/gcp/storage/
--rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-06-13 07:01:46.000000 gaohn-common-utils-0.0.42/common_utils/cloud/gcp/storage/gcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:02:03.645491 gaohn-common-utils-0.0.42/common_utils/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 07:01:46.000000 gaohn-common-utils-0.0.42/common_utils/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-13 07:01:46.000000 gaohn-common-utils-0.0.42/common_utils/core/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-06-13 07:01:46.000000 gaohn-common-utils-0.0.42/common_utils/core/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-06-13 07:01:46.000000 gaohn-common-utils-0.0.42/common_utils/core/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-06-13 07:01:46.000000 gaohn-common-utils-0.0.42/common_utils/core/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-06-13 07:01:46.000000 gaohn-common-utils-0.0.42/common_utils/core/file_system_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-06-13 07:01:46.000000 gaohn-common-utils-0.0.42/common_utils/core/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:02:03.645491 gaohn-common-utils-0.0.42/common_utils/orchestrator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 07:01:46.000000 gaohn-common-utils-0.0.42/common_utils/orchestrator/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:02:03.645491 gaohn-common-utils-0.0.42/common_utils/versioning/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:02:03.649492 gaohn-common-utils-0.0.42/common_utils/versioning/dvc/
--rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-06-13 07:01:46.000000 gaohn-common-utils-0.0.42/common_utils/versioning/dvc/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:02:03.649492 gaohn-common-utils-0.0.42/gaohn_common_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-06-13 07:02:03.000000 gaohn-common-utils-0.0.42/gaohn_common_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-13 07:02:03.000000 gaohn-common-utils-0.0.42/gaohn_common_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 07:02:03.000000 gaohn-common-utils-0.0.42/gaohn_common_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-13 07:02:03.000000 gaohn-common-utils-0.0.42/gaohn_common_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-13 07:02:03.000000 gaohn-common-utils-0.0.42/gaohn_common_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-06-13 07:01:46.000000 gaohn-common-utils-0.0.42/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 07:02:03.649492 gaohn-common-utils-0.0.42/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:23:39.120857 gaohn-common-utils-0.0.43/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-13 07:23:18.000000 gaohn-common-utils-0.0.43/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-06-13 07:23:39.120857 gaohn-common-utils-0.0.43/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-06-13 07:23:18.000000 gaohn-common-utils-0.0.43/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:23:39.116857 gaohn-common-utils-0.0.43/common_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 07:23:18.000000 gaohn-common-utils-0.0.43/common_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:23:39.116857 gaohn-common-utils-0.0.43/common_utils/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-13 07:23:18.000000 gaohn-common-utils-0.0.43/common_utils/cloud/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:23:39.112857 gaohn-common-utils-0.0.43/common_utils/cloud/gcp/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:23:39.116857 gaohn-common-utils-0.0.43/common_utils/cloud/gcp/database/
+-rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-06-13 07:23:18.000000 gaohn-common-utils-0.0.43/common_utils/cloud/gcp/database/bigquery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:23:39.116857 gaohn-common-utils-0.0.43/common_utils/cloud/gcp/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-06-13 07:23:18.000000 gaohn-common-utils-0.0.43/common_utils/cloud/gcp/storage/gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:23:39.116857 gaohn-common-utils-0.0.43/common_utils/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 07:23:18.000000 gaohn-common-utils-0.0.43/common_utils/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-13 07:23:18.000000 gaohn-common-utils-0.0.43/common_utils/core/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-06-13 07:23:18.000000 gaohn-common-utils-0.0.43/common_utils/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-06-13 07:23:18.000000 gaohn-common-utils-0.0.43/common_utils/core/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-06-13 07:23:18.000000 gaohn-common-utils-0.0.43/common_utils/core/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-06-13 07:23:18.000000 gaohn-common-utils-0.0.43/common_utils/core/file_system_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-06-13 07:23:18.000000 gaohn-common-utils-0.0.43/common_utils/core/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:23:39.120857 gaohn-common-utils-0.0.43/common_utils/orchestrator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 07:23:18.000000 gaohn-common-utils-0.0.43/common_utils/orchestrator/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:23:39.112857 gaohn-common-utils-0.0.43/common_utils/versioning/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:23:39.120857 gaohn-common-utils-0.0.43/common_utils/versioning/dvc/
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-06-13 07:23:18.000000 gaohn-common-utils-0.0.43/common_utils/versioning/dvc/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:23:39.120857 gaohn-common-utils-0.0.43/gaohn_common_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-06-13 07:23:39.000000 gaohn-common-utils-0.0.43/gaohn_common_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-13 07:23:39.000000 gaohn-common-utils-0.0.43/gaohn_common_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 07:23:39.000000 gaohn-common-utils-0.0.43/gaohn_common_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-13 07:23:39.000000 gaohn-common-utils-0.0.43/gaohn_common_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-13 07:23:39.000000 gaohn-common-utils-0.0.43/gaohn_common_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-06-13 07:23:18.000000 gaohn-common-utils-0.0.43/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 07:23:39.120857 gaohn-common-utils-0.0.43/setup.cfg
```

### Comparing `gaohn-common-utils-0.0.42/LICENSE` & `gaohn-common-utils-0.0.43/LICENSE`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.42/PKG-INFO` & `gaohn-common-utils-0.0.43/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaohn-common-utils
-Version: 0.0.42
+Version: 0.0.43
 Summary: A small utility package
 Author-email: Gao Hongnan <hongnangao@gmail.com>
 Project-URL: Homepage, https://github.com/gao-hongnan/common-utils
 Project-URL: Bug Tracker, https://github.com/gao-hongnan/common-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gaohn-common-utils-0.0.42/README.md` & `gaohn-common-utils-0.0.43/README.md`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.42/common_utils/cloud/base.py` & `gaohn-common-utils-0.0.43/common_utils/cloud/base.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.42/common_utils/cloud/gcp/database/bigquery.py` & `gaohn-common-utils-0.0.43/common_utils/cloud/gcp/database/bigquery.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.42/common_utils/cloud/gcp/storage/gcs.py` & `gaohn-common-utils-0.0.43/common_utils/cloud/gcp/storage/gcs.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.42/common_utils/core/artifacts.py` & `gaohn-common-utils-0.0.43/common_utils/core/artifacts.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.42/common_utils/core/base.py` & `gaohn-common-utils-0.0.43/common_utils/core/base.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.42/common_utils/core/common.py` & `gaohn-common-utils-0.0.43/common_utils/core/common.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.42/common_utils/core/decorators.py` & `gaohn-common-utils-0.0.43/common_utils/core/decorators.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.42/common_utils/core/file_system_utils.py` & `gaohn-common-utils-0.0.43/common_utils/core/file_system_utils.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.42/common_utils/core/logger.py` & `gaohn-common-utils-0.0.43/common_utils/core/logger.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,26 @@
 """Logger class for logging to console and file."""
 import logging
+import os
 from dataclasses import dataclass, field
 from datetime import datetime
 from pathlib import Path
 from typing import Optional, Union
 
 from rich.logging import RichHandler
 
 
+class CustomFormatter(logging.Formatter):
+    """This class overrides logging.Formatter's pathname to be relative path."""
+
+    def format(self, record):
+        record.pathname = os.path.relpath(record.pathname)
+        return super().format(record)
+
+
 @dataclass
 class Logger:
     """Class for logger. Consider using singleton design to
     maintain only one instance of logger (i.e. shared logger)."""
 
     log_file: Optional[str] = "log.txt"
     module_name: Optional[str] = None
@@ -38,26 +47,26 @@
             self.log_output_dir = self._create_log_output_dir()
             return self.log_output_dir / self.log_file
         return None
 
     def _create_stream_handler(self) -> RichHandler:
         stream_handler = RichHandler(rich_tracebacks=True, level=self.level)
         stream_handler.setFormatter(
-            logging.Formatter(
-                "%(asctime)s [%(levelname)s] %(name)s: %(message)s",
+            CustomFormatter(
+                "%(asctime)s [%(levelname)s] %(pathname)s %(funcName)s L%(lineno)d: %(message)s",
                 "%Y-%m-%d %H:%M:%S",
             )
         )
         return stream_handler
 
     def _create_file_handler(self, log_file_path: Path) -> logging.FileHandler:
         file_handler = logging.FileHandler(filename=str(log_file_path))
         file_handler.setFormatter(
-            logging.Formatter(
-                "%(asctime)s [%(levelname)s] %(name)s: %(message)s",
+            CustomFormatter(
+                "%(asctime)s [%(levelname)s] %(pathname)s %(funcName)s L%(lineno)d: %(message)s",
                 "%Y-%m-%d %H:%M:%S",
             )
         )
         return file_handler
 
     def _init_logger(self) -> logging.Logger:
         # get module name, useful for multi-module logging
```

### Comparing `gaohn-common-utils-0.0.42/common_utils/versioning/dvc/base.py` & `gaohn-common-utils-0.0.43/common_utils/versioning/dvc/base.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.42/gaohn_common_utils.egg-info/PKG-INFO` & `gaohn-common-utils-0.0.43/gaohn_common_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaohn-common-utils
-Version: 0.0.42
+Version: 0.0.43
 Summary: A small utility package
 Author-email: Gao Hongnan <hongnangao@gmail.com>
 Project-URL: Homepage, https://github.com/gao-hongnan/common-utils
 Project-URL: Bug Tracker, https://github.com/gao-hongnan/common-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gaohn-common-utils-0.0.42/gaohn_common_utils.egg-info/SOURCES.txt` & `gaohn-common-utils-0.0.43/gaohn_common_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.42/pyproject.toml` & `gaohn-common-utils-0.0.43/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gaohn-common-utils"
-version = "0.0.42"
+version = "0.0.43"
 authors = [
   { name="Gao Hongnan", email="hongnangao@gmail.com" },
 ]
 description = "A small utility package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

