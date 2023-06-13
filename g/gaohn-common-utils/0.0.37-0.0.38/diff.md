# Comparing `tmp/gaohn-common-utils-0.0.37.tar.gz` & `tmp/gaohn-common-utils-0.0.38.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gaohn-common-utils-0.0.37.tar", last modified: Sun Jun 11 09:32:36 2023, max compression
+gzip compressed data, was "gaohn-common-utils-0.0.38.tar", last modified: Tue Jun 13 02:20:08 2023, max compression
```

## Comparing `gaohn-common-utils-0.0.37.tar` & `gaohn-common-utils-0.0.38.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 09:32:36.305037 gaohn-common-utils-0.0.37/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-11 09:32:15.000000 gaohn-common-utils-0.0.37/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-11 09:32:36.305037 gaohn-common-utils-0.0.37/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-11 09:32:15.000000 gaohn-common-utils-0.0.37/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 09:32:36.305037 gaohn-common-utils-0.0.37/common_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 09:32:15.000000 gaohn-common-utils-0.0.37/common_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 09:32:36.305037 gaohn-common-utils-0.0.37/common_utils/cloud/
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-11 09:32:15.000000 gaohn-common-utils-0.0.37/common_utils/cloud/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 09:32:36.301037 gaohn-common-utils-0.0.37/common_utils/cloud/gcp/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 09:32:36.305037 gaohn-common-utils-0.0.37/common_utils/cloud/gcp/storage/
--rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-06-11 09:32:15.000000 gaohn-common-utils-0.0.37/common_utils/cloud/gcp/storage/bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-06-11 09:32:15.000000 gaohn-common-utils-0.0.37/common_utils/cloud/gcp/storage/gcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 09:32:36.305037 gaohn-common-utils-0.0.37/common_utils/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 09:32:15.000000 gaohn-common-utils-0.0.37/common_utils/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-11 09:32:15.000000 gaohn-common-utils-0.0.37/common_utils/core/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-11 09:32:15.000000 gaohn-common-utils-0.0.37/common_utils/core/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-06-11 09:32:15.000000 gaohn-common-utils-0.0.37/common_utils/core/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-06-11 09:32:15.000000 gaohn-common-utils-0.0.37/common_utils/core/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-06-11 09:32:15.000000 gaohn-common-utils-0.0.37/common_utils/core/file_system_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-06-11 09:32:15.000000 gaohn-common-utils-0.0.37/common_utils/core/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 09:32:36.305037 gaohn-common-utils-0.0.37/common_utils/orchestrator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 09:32:15.000000 gaohn-common-utils-0.0.37/common_utils/orchestrator/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 09:32:36.301037 gaohn-common-utils-0.0.37/common_utils/versioning/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 09:32:36.305037 gaohn-common-utils-0.0.37/common_utils/versioning/dvc/
--rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-06-11 09:32:15.000000 gaohn-common-utils-0.0.37/common_utils/versioning/dvc/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 09:32:36.305037 gaohn-common-utils-0.0.37/gaohn_common_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-11 09:32:36.000000 gaohn-common-utils-0.0.37/gaohn_common_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-06-11 09:32:36.000000 gaohn-common-utils-0.0.37/gaohn_common_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 09:32:36.000000 gaohn-common-utils-0.0.37/gaohn_common_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-11 09:32:36.000000 gaohn-common-utils-0.0.37/gaohn_common_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-11 09:32:36.000000 gaohn-common-utils-0.0.37/gaohn_common_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-06-11 09:32:15.000000 gaohn-common-utils-0.0.37/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 09:32:36.305037 gaohn-common-utils-0.0.37/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:20:08.791229 gaohn-common-utils-0.0.38/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-13 02:19:47.000000 gaohn-common-utils-0.0.38/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-06-13 02:20:08.791229 gaohn-common-utils-0.0.38/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-06-13 02:19:47.000000 gaohn-common-utils-0.0.38/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:20:08.787228 gaohn-common-utils-0.0.38/common_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 02:19:47.000000 gaohn-common-utils-0.0.38/common_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:20:08.787228 gaohn-common-utils-0.0.38/common_utils/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-13 02:19:47.000000 gaohn-common-utils-0.0.38/common_utils/cloud/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:20:08.787228 gaohn-common-utils-0.0.38/common_utils/cloud/gcp/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:20:08.787228 gaohn-common-utils-0.0.38/common_utils/cloud/gcp/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-06-13 02:19:47.000000 gaohn-common-utils-0.0.38/common_utils/cloud/gcp/storage/bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-06-13 02:19:47.000000 gaohn-common-utils-0.0.38/common_utils/cloud/gcp/storage/gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:20:08.787228 gaohn-common-utils-0.0.38/common_utils/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 02:19:47.000000 gaohn-common-utils-0.0.38/common_utils/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-13 02:19:47.000000 gaohn-common-utils-0.0.38/common_utils/core/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-13 02:19:47.000000 gaohn-common-utils-0.0.38/common_utils/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-06-13 02:19:47.000000 gaohn-common-utils-0.0.38/common_utils/core/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-06-13 02:19:47.000000 gaohn-common-utils-0.0.38/common_utils/core/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-06-13 02:19:47.000000 gaohn-common-utils-0.0.38/common_utils/core/file_system_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-06-13 02:19:47.000000 gaohn-common-utils-0.0.38/common_utils/core/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:20:08.787228 gaohn-common-utils-0.0.38/common_utils/orchestrator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 02:19:47.000000 gaohn-common-utils-0.0.38/common_utils/orchestrator/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:20:08.787228 gaohn-common-utils-0.0.38/common_utils/versioning/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:20:08.787228 gaohn-common-utils-0.0.38/common_utils/versioning/dvc/
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-06-13 02:19:47.000000 gaohn-common-utils-0.0.38/common_utils/versioning/dvc/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:20:08.791229 gaohn-common-utils-0.0.38/gaohn_common_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-06-13 02:20:08.000000 gaohn-common-utils-0.0.38/gaohn_common_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-06-13 02:20:08.000000 gaohn-common-utils-0.0.38/gaohn_common_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 02:20:08.000000 gaohn-common-utils-0.0.38/gaohn_common_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-13 02:20:08.000000 gaohn-common-utils-0.0.38/gaohn_common_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-13 02:20:08.000000 gaohn-common-utils-0.0.38/gaohn_common_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-06-13 02:19:47.000000 gaohn-common-utils-0.0.38/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 02:20:08.791229 gaohn-common-utils-0.0.38/setup.cfg
```

### Comparing `gaohn-common-utils-0.0.37/LICENSE` & `gaohn-common-utils-0.0.38/LICENSE`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.37/common_utils/cloud/base.py` & `gaohn-common-utils-0.0.38/common_utils/cloud/base.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.37/common_utils/cloud/gcp/storage/bigquery.py` & `gaohn-common-utils-0.0.38/common_utils/cloud/gcp/storage/bigquery.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.37/common_utils/cloud/gcp/storage/gcs.py` & `gaohn-common-utils-0.0.38/common_utils/cloud/gcp/storage/gcs.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.37/common_utils/core/artifacts.py` & `gaohn-common-utils-0.0.38/common_utils/core/artifacts.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.37/common_utils/core/common.py` & `gaohn-common-utils-0.0.38/common_utils/core/common.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.37/common_utils/core/decorators.py` & `gaohn-common-utils-0.0.38/common_utils/core/decorators.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.37/common_utils/core/file_system_utils.py` & `gaohn-common-utils-0.0.38/common_utils/core/file_system_utils.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.37/common_utils/core/logger.py` & `gaohn-common-utils-0.0.38/common_utils/core/logger.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Logger class for logging to console and file."""
 import logging
 from dataclasses import dataclass, field
 from datetime import datetime
 from pathlib import Path
-from typing import Optional
+from typing import Optional, Union
 
 from rich.logging import RichHandler
 
 
 @dataclass
 class Logger:
     """Class for logger. Consider using singleton design to
@@ -15,18 +15,18 @@
 
     log_file: Optional[str] = "log.txt"
     module_name: Optional[str] = None
     level: int = logging.INFO
     propagate: bool = False
     log_dir: Optional[str] = "outputs"
 
-    log_output_dir: Optional[str] = field(default=None, init=False)
+    log_output_dir: Optional[Union[str, Path]] = field(default=None, init=False)
     logger: logging.Logger = field(init=False)
 
-    def __post_init__(self):
+    def __post_init__(self) -> None:
         self.logger = self._init_logger()
 
     def _create_log_output_dir(self) -> Path:
         current_time = datetime.now().strftime("%Y-%m-%dT%H:%M:%S")
         log_output_dir = Path(self.log_dir) / current_time
 
         Path(log_output_dir).mkdir(parents=True, exist_ok=True)
@@ -37,23 +37,19 @@
         if self.log_dir is not None:
             log_output_dir = self._create_log_output_dir()
             log_file_path = log_output_dir / self.log_file if self.log_file else None
             self.log_output_dir = log_output_dir
         else:
             log_file_path = None
 
-        if self.module_name is None:
-            logger = logging.getLogger(__name__)
-        else:
-            # get module name, useful for multi-module logging
-            logger = logging.getLogger(self.module_name)
-
+        # get module name, useful for multi-module logging
+        logger = logging.getLogger(self.module_name or __name__)
         logger.setLevel(self.level)
 
-        stream_handler = RichHandler(rich_tracebacks=True)
+        stream_handler = RichHandler(rich_tracebacks=True, level=self.level)
         logger.addHandler(stream_handler)
 
         if log_file_path:
             file_handler = logging.FileHandler(filename=str(log_file_path))
             file_handler.setFormatter(
                 logging.Formatter(
                     "%(asctime)s [%(levelname)s]: %(message)s",
```

### Comparing `gaohn-common-utils-0.0.37/common_utils/versioning/dvc/base.py` & `gaohn-common-utils-0.0.38/common_utils/versioning/dvc/base.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.37/gaohn_common_utils.egg-info/SOURCES.txt` & `gaohn-common-utils-0.0.38/gaohn_common_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.37/pyproject.toml` & `gaohn-common-utils-0.0.38/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gaohn-common-utils"
-version = "0.0.37"
+version = "0.0.38"
 authors = [
   { name="Gao Hongnan", email="hongnangao@gmail.com" },
 ]
 description = "A small utility package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -38,15 +38,17 @@
 dev = [
     "black==23.3.0",
     "pylint==2.17.4",
     "pytest==6.2.5",
     "mypy==1.3.0",
     "isort==5.12.0",
     "bandit==1.7.5",
+    "mypy==1.3.0",
     "toml==0.10.2",
+    "colorama==0.4.4",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/gao-hongnan/common-utils"
 "Bug Tracker" = "https://github.com/gao-hongnan/common-utils/issues"
 
 [tool.black]
@@ -142,12 +144,13 @@
     ".venv",
     "_build",
     "buck-out",
     "build",
     "dist",
 ]
 
-# https://mypy.readthedocs.io/en/stable/config_file.html
+# https://mypy.readthedocs.io/en/stable/config_file.html#using-a-pyproject-toml-file
 [tool.mypy]
 ignore_missing_imports = true
 disallow_untyped_defs = true
-disable_error_code = ['override', 'attr-defined']
+disable_error_code = ['override', 'attr-defined']
+disallow_any_generics = false
```

