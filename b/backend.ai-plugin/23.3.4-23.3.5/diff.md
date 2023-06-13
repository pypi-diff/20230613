# Comparing `tmp/backend.ai-plugin-23.3.4.tar.gz` & `tmp/backend.ai-plugin-23.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backend.ai-plugin-23.3.4.tar", last modified: Mon May 29 10:42:36 2023, max compression
+gzip compressed data, was "backend.ai-plugin-23.3.5.tar", last modified: Tue Jun 13 03:42:17 2023, max compression
```

## Comparing `backend.ai-plugin-23.3.4.tar` & `backend.ai-plugin-23.3.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:36.286992 backend.ai-plugin-23.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-29 10:42:36.000000 backend.ai-plugin-23.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-29 10:42:36.286992 backend.ai-plugin-23.3.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:36.282992 backend.ai-plugin-23.3.4/ai/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:36.282992 backend.ai-plugin-23.3.4/ai/backend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:36.286992 backend.ai-plugin-23.3.4/ai/backend/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-29 10:42:36.000000 backend.ai-plugin-23.3.4/ai/backend/plugin/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-29 10:42:36.000000 backend.ai-plugin-23.3.4/ai/backend/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8139 2023-05-29 10:42:36.000000 backend.ai-plugin-23.3.4/ai/backend/plugin/entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-29 10:42:36.000000 backend.ai-plugin-23.3.4/ai/backend/plugin/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:36.286992 backend.ai-plugin-23.3.4/backend.ai_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-29 10:42:36.000000 backend.ai-plugin-23.3.4/backend.ai_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-29 10:42:36.000000 backend.ai-plugin-23.3.4/backend.ai_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 10:42:36.000000 backend.ai-plugin-23.3.4/backend.ai_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 10:42:36.000000 backend.ai-plugin-23.3.4/backend.ai_plugin.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 10:42:36.000000 backend.ai-plugin-23.3.4/backend.ai_plugin.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-29 10:42:36.000000 backend.ai-plugin-23.3.4/backend.ai_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-29 10:42:36.000000 backend.ai-plugin-23.3.4/backend_shim.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 10:42:36.286992 backend.ai-plugin-23.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-05-29 10:42:36.000000 backend.ai-plugin-23.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:17.528261 backend.ai-plugin-23.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-13 03:42:17.000000 backend.ai-plugin-23.3.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-13 03:42:17.528261 backend.ai-plugin-23.3.5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:17.524261 backend.ai-plugin-23.3.5/ai/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:17.524261 backend.ai-plugin-23.3.5/ai/backend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:17.528261 backend.ai-plugin-23.3.5/ai/backend/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-13 03:42:17.000000 backend.ai-plugin-23.3.5/ai/backend/plugin/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-13 03:42:17.000000 backend.ai-plugin-23.3.5/ai/backend/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8254 2023-06-13 03:42:17.000000 backend.ai-plugin-23.3.5/ai/backend/plugin/entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-13 03:42:17.000000 backend.ai-plugin-23.3.5/ai/backend/plugin/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:42:17.528261 backend.ai-plugin-23.3.5/backend.ai_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-13 03:42:17.000000 backend.ai-plugin-23.3.5/backend.ai_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-13 03:42:17.000000 backend.ai-plugin-23.3.5/backend.ai_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 03:42:17.000000 backend.ai-plugin-23.3.5/backend.ai_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 03:42:17.000000 backend.ai-plugin-23.3.5/backend.ai_plugin.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 03:42:17.000000 backend.ai-plugin-23.3.5/backend.ai_plugin.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-13 03:42:17.000000 backend.ai-plugin-23.3.5/backend.ai_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-13 03:42:17.000000 backend.ai-plugin-23.3.5/backend_shim.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 03:42:17.528261 backend.ai-plugin-23.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-06-13 03:42:17.000000 backend.ai-plugin-23.3.5/setup.py
```

### Comparing `backend.ai-plugin-23.3.4/PKG-INFO` & `backend.ai-plugin-23.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-plugin
-Version: 23.3.4
+Version: 23.3.5
 Summary: Backend.AI Plugin Subsystem
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: MIT
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
```

### Comparing `backend.ai-plugin-23.3.4/ai/backend/plugin/entrypoint.py` & `backend.ai-plugin-23.3.5/ai/backend/plugin/entrypoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import ast
 import collections
 import configparser
 import itertools
 import logging
+import os
 from importlib.metadata import EntryPoint, entry_points
 from pathlib import Path
 from typing import Iterable, Iterator, Optional
 
 log = logging.getLogger(__spec__.name)  # type: ignore[name-defined]
 
 
@@ -141,14 +142,16 @@
                 if entrypoint.name not in entrypoints:
                     entrypoints[entrypoint.name] = entrypoint
         # TODO: implement pyproject.toml scanner
     yield from entrypoints.values()
 
 
 def find_build_root(path: Optional[Path] = None) -> Path:
+    if env_build_root := os.environ.get("BACKEND_BUILD_ROOT", None):
+        return Path(env_build_root)
     cwd = Path.cwd() if path is None else path
     while True:
         if (cwd / "BUILD_ROOT").exists():
             return cwd
         cwd = cwd.parent
         if cwd.parent == cwd:
             # reached the root directory
```

### Comparing `backend.ai-plugin-23.3.4/backend.ai_plugin.egg-info/PKG-INFO` & `backend.ai-plugin-23.3.5/backend.ai_plugin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-plugin
-Version: 23.3.4
+Version: 23.3.5
 Summary: Backend.AI Plugin Subsystem
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: MIT
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
```

### Comparing `backend.ai-plugin-23.3.4/backend_shim.py` & `backend.ai-plugin-23.3.5/backend_shim.py`

 * *Files identical despite different names*

### Comparing `backend.ai-plugin-23.3.4/setup.py` & `backend.ai-plugin-23.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,11 +46,11 @@
     ),
     'project_urls': {
         'Documentation': 'https://docs.backend.ai/',
         'Source': 'https://github.com/lablup/backend.ai',
     },
     'python_requires': '>=3.11,<3.12',
     'url': 'https://github.com/lablup/backend.ai',
-    'version': """23.03.4
+    'version': """23.03.5
 """,
     'zip_safe': False,
 })
```

