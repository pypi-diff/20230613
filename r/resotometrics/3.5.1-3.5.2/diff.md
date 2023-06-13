# Comparing `tmp/resotometrics-3.5.1.tar.gz` & `tmp/resotometrics-3.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resotometrics-3.5.1.tar", last modified: Fri Jun  2 14:55:57 2023, max compression
+gzip compressed data, was "resotometrics-3.5.2.tar", last modified: Tue Jun 13 13:11:14 2023, max compression
```

## Comparing `resotometrics-3.5.1.tar` & `resotometrics-3.5.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:55:57.862066 resotometrics-3.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-02 14:53:16.000000 resotometrics-3.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-06-02 14:55:57.862066 resotometrics-3.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8536 2023-06-02 14:53:16.000000 resotometrics-3.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-02 14:53:16.000000 resotometrics-3.5.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:55:57.858066 resotometrics-3.5.1/resotometrics/
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-02 14:53:16.000000 resotometrics-3.5.1/resotometrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7707 2023-06-02 14:53:16.000000 resotometrics-3.5.1/resotometrics/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-06-02 14:53:16.000000 resotometrics-3.5.1/resotometrics/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    12823 2023-06-02 14:53:16.000000 resotometrics-3.5.1/resotometrics/default_metrics.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-02 14:53:16.000000 resotometrics-3.5.1/resotometrics/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-02 14:53:16.000000 resotometrics-3.5.1/resotometrics/search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:55:57.862066 resotometrics-3.5.1/resotometrics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-06-02 14:55:57.000000 resotometrics-3.5.1/resotometrics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-02 14:55:57.000000 resotometrics-3.5.1/resotometrics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:55:57.000000 resotometrics-3.5.1/resotometrics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-02 14:55:57.000000 resotometrics-3.5.1/resotometrics.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:54:22.000000 resotometrics-3.5.1/resotometrics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-02 14:55:57.000000 resotometrics-3.5.1/resotometrics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-02 14:55:57.000000 resotometrics-3.5.1/resotometrics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-02 14:55:57.862066 resotometrics-3.5.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:55:57.862066 resotometrics-3.5.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-02 14:53:16.000000 resotometrics-3.5.1/test/test_args.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:11:14.874974 resotometrics-3.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-13 13:07:55.000000 resotometrics-3.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-06-13 13:11:14.874974 resotometrics-3.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8536 2023-06-13 13:07:55.000000 resotometrics-3.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-13 13:07:55.000000 resotometrics-3.5.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:11:14.874974 resotometrics-3.5.2/resotometrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-13 13:07:55.000000 resotometrics-3.5.2/resotometrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7707 2023-06-13 13:07:55.000000 resotometrics-3.5.2/resotometrics/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-06-13 13:07:55.000000 resotometrics-3.5.2/resotometrics/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12823 2023-06-13 13:07:55.000000 resotometrics-3.5.2/resotometrics/default_metrics.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-13 13:07:55.000000 resotometrics-3.5.2/resotometrics/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-13 13:07:55.000000 resotometrics-3.5.2/resotometrics/search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:11:14.874974 resotometrics-3.5.2/resotometrics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-06-13 13:11:14.000000 resotometrics-3.5.2/resotometrics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-13 13:11:14.000000 resotometrics-3.5.2/resotometrics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 13:11:14.000000 resotometrics-3.5.2/resotometrics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-13 13:11:14.000000 resotometrics-3.5.2/resotometrics.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 13:09:18.000000 resotometrics-3.5.2/resotometrics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-13 13:11:14.000000 resotometrics-3.5.2/resotometrics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-13 13:11:14.000000 resotometrics-3.5.2/resotometrics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-13 13:11:14.874974 resotometrics-3.5.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:11:14.874974 resotometrics-3.5.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-13 13:07:55.000000 resotometrics-3.5.2/test/test_args.py
```

### Comparing `resotometrics-3.5.1/PKG-INFO` & `resotometrics-3.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotometrics
-Version: 3.5.1
+Version: 3.5.2
 Summary: Exports Resoto metrics in Prometheus format.
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/resotometrics
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resotometrics-3.5.1/README.md` & `resotometrics-3.5.2/README.md`

 * *Files identical despite different names*

### Comparing `resotometrics-3.5.1/pyproject.toml` & `resotometrics-3.5.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "resotometrics"
-version = "3.5.1"
+version = "3.5.2"
 authors = [{name="Some Engineering Inc."}]
 description = "Exports Resoto metrics in Prometheus format."
 license = {file="LICENSE"}
 requires-python = ">=3.9"
 classifiers = [
     # Current project status
     "Development Status :: 4 - Beta",
@@ -23,15 +23,15 @@
     "Natural Language :: English",
     "Topic :: Security",
     "Topic :: Utilities",
 ]
 readme = {file="README.md", content-type="text/markdown"}
 
 dependencies = [
-    "resotolib==3.5.1"
+    "resotolib==3.5.2"
 ]
 
 [pyproject.optional-dependencies]
 test = ["pytest"]
 
 [project.scripts]
 resotometrics = "resotometrics.__main__:main"
```

### Comparing `resotometrics-3.5.1/resotometrics/__main__.py` & `resotometrics-3.5.2/resotometrics/__main__.py`

 * *Files identical despite different names*

### Comparing `resotometrics-3.5.1/resotometrics/config.py` & `resotometrics-3.5.2/resotometrics/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 from attrs import define, field
 from typing import Dict, ClassVar
 
-import jsons
 from yaml import load
 from enum import Enum
 
+from resotolib.json import from_json
 
 try:
     from yaml import CLoader as Loader
 except ImportError:
     from yaml import Loader
 
 
@@ -29,15 +29,15 @@
 def _load_default_metrics() -> Dict[str, Metric]:
     local_path = os.path.abspath(os.path.dirname(__file__))
     default_metrics_file = f"{local_path}/default_metrics.yaml"
     if not os.path.isfile(default_metrics_file):
         raise RuntimeError(f"Could not find default metrics file {default_metrics_file}")
     with open(default_metrics_file, "r") as f:
         default_metrics = load(f, Loader=Loader)
-    return {metric_name: jsons.load(metric_data, Metric) for metric_name, metric_data in default_metrics.items()}
+    return {metric_name: from_json(metric_data, Metric) for metric_name, metric_data in default_metrics.items()}
 
 
 @define
 class ResotoMetricsConfig:
     kind: ClassVar[str] = "resotometrics"
     graph: str = field(
         default="resoto",
```

### Comparing `resotometrics-3.5.1/resotometrics/default_metrics.yaml` & `resotometrics-3.5.2/resotometrics/default_metrics.yaml`

 * *Files identical despite different names*

### Comparing `resotometrics-3.5.1/resotometrics/metrics.py` & `resotometrics-3.5.2/resotometrics/metrics.py`

 * *Files identical despite different names*

### Comparing `resotometrics-3.5.1/resotometrics/search.py` & `resotometrics-3.5.2/resotometrics/search.py`

 * *Files identical despite different names*

### Comparing `resotometrics-3.5.1/resotometrics.egg-info/PKG-INFO` & `resotometrics-3.5.2/resotometrics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotometrics
-Version: 3.5.1
+Version: 3.5.2
 Summary: Exports Resoto metrics in Prometheus format.
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/resotometrics
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resotometrics-3.5.1/test/test_args.py` & `resotometrics-3.5.2/test/test_args.py`

 * *Files identical despite different names*

