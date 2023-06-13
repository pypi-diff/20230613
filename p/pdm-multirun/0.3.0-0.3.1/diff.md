# Comparing `tmp/pdm_multirun-0.3.0.tar.gz` & `tmp/pdm_multirun-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdm_multirun-0.3.0.tar", last modified: Thu Jun  8 14:08:15 2023, max compression
+gzip compressed data, was "pdm_multirun-0.3.1.tar", last modified: Tue Jun 13 13:14:06 2023, max compression
```

## Comparing `pdm_multirun-0.3.0.tar` & `pdm_multirun-0.3.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      754 2023-06-08 13:02:32.508182 pdm_multirun-0.3.0/LICENSE
--rw-r--r--   0        0        0     2353 2023-06-08 13:02:35.261493 pdm_multirun-0.3.0/README.md
--rw-r--r--   0        0        0     2535 2023-06-08 14:08:15.587166 pdm_multirun-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      150 2023-06-08 13:02:32.381516 pdm_multirun-0.3.0/src/pdm_multirun/__init__.py
--rw-r--r--   0        0        0     3208 2023-06-08 14:07:21.166026 pdm_multirun-0.3.0/src/pdm_multirun/plugin.py
--rw-r--r--   0        0        0        0 2023-06-08 13:02:32.378183 pdm_multirun-0.3.0/src/pdm_multirun/py.typed
--rw-r--r--   0        0        0      165 2023-06-08 13:02:32.371516 pdm_multirun-0.3.0/tests/__init__.py
--rw-r--r--   0        0        0       47 2023-06-08 13:02:32.368183 pdm_multirun-0.3.0/tests/conftest.py
--rw-r--r--   0        0        0      155 2023-06-08 13:53:36.229321 pdm_multirun-0.3.0/tests/test_plugin.py
--rw-r--r--   0        0        0     3784 1970-01-01 00:00:00.000000 pdm_multirun-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      754 2023-06-08 13:02:32.508182 pdm_multirun-0.3.1/LICENSE
+-rw-r--r--   0        0        0     2353 2023-06-08 13:02:35.261493 pdm_multirun-0.3.1/README.md
+-rw-r--r--   0        0        0     2595 2023-06-13 13:14:06.400693 pdm_multirun-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      150 2023-06-08 13:02:32.381516 pdm_multirun-0.3.1/src/pdm_multirun/__init__.py
+-rw-r--r--   0        0        0     3240 2023-06-13 10:35:41.322821 pdm_multirun-0.3.1/src/pdm_multirun/plugin.py
+-rw-r--r--   0        0        0        0 2023-06-08 13:02:32.378183 pdm_multirun-0.3.1/src/pdm_multirun/py.typed
+-rw-r--r--   0        0        0      165 2023-06-08 13:02:32.371516 pdm_multirun-0.3.1/tests/__init__.py
+-rw-r--r--   0        0        0       47 2023-06-08 13:02:32.368183 pdm_multirun-0.3.1/tests/conftest.py
+-rw-r--r--   0        0        0      155 2023-06-08 13:53:36.229321 pdm_multirun-0.3.1/tests/test_plugin.py
+-rw-r--r--   0        0        0     3784 1970-01-01 00:00:00.000000 pdm_multirun-0.3.1/PKG-INFO
```

### Comparing `pdm_multirun-0.3.0/LICENSE` & `pdm_multirun-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pdm_multirun-0.3.0/README.md` & `pdm_multirun-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `pdm_multirun-0.3.0/pyproject.toml` & `pdm_multirun-0.3.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     "Topic :: Software Development",
     "Topic :: Utilities",
     "Typing :: Typed",
 ]
 dependencies = [
     "pdm>=2",
 ]
-version = "0.3.0"
+version = "0.3.1"
 
 [project.license]
 text = "ISC"
 
 [project.urls]
 Homepage = "https://pawamoy.github.io/pdm-multirun"
 Documentation = "https://pawamoy.github.io/pdm-multirun"
@@ -47,14 +47,19 @@
 Discussions = "https://github.com/pawamoy/pdm-multirun/discussions"
 Gitter = "https://gitter.im/pdm-multirun/community"
 Funding = "https://github.com/sponsors/pawamoy"
 
 [project.entry-points.pdm]
 multirun = "pdm_multirun.plugin:multirun"
 
+[tool.pdm]
+plugins = [
+    "-e file:///${PROJECT_ROOT}",
+]
+
 [tool.pdm.version]
 source = "scm"
 
 [tool.pdm.build]
 package-dir = "src"
 editable-backend = "editables"
```

### Comparing `pdm_multirun-0.3.0/src/pdm_multirun/plugin.py` & `pdm_multirun-0.3.1/src/pdm_multirun/plugin.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 from __future__ import annotations
 
 import os
 from typing import TYPE_CHECKING
 
 from pdm import termui
-from pdm.cli import actions
 from pdm.cli.commands.run import Command as RunCommand
 from pdm.cli.commands.run import Project
+from pdm.cli.commands.use import Command as UseCommand
 from pdm.cli.hooks import HookManager
 
 if TYPE_CHECKING:
     import argparse
 
     from pdm.core import Core
 
@@ -69,15 +69,15 @@
     def _use(self, project: Project, options: argparse.Namespace, python: str) -> None:
         old_echo = project.core.ui.echo
         if not options.verbose:
             project.core.ui.echo = lambda *args, **kwargs: None  # type: ignore[method-assign]
         # unset cached environment
         project.environment = None  # type: ignore[assignment]
         try:
-            actions.do_use(
+            UseCommand().do_use(
                 project,
                 python=python,
                 first=True,
                 ignore_remembered=False,
                 hooks=HookManager(project, skip=options.skip),
             )
         finally:
```

### Comparing `pdm_multirun-0.3.0/PKG-INFO` & `pdm_multirun-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdm-multirun
-Version: 0.3.0
+Version: 0.3.1
 Summary: A PDM plugin to run a command on multiple Python versions.
 Author-Email: Timothée Mazzucotelli <pawamoy@pm.me>
 License: ISC
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

