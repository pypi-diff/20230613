# Comparing `tmp/ansys-mechanical-core-0.8.0.tar.gz` & `tmp/ansys_mechanical_core-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys-mechanical-core-0.8.0.tar", last modified: Fri May 12 13:26:39 2023, max compression
+gzip compressed data, was "ansys_mechanical_core-0.9.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ansys-mechanical-core-0.8.0.tar` & `ansys_mechanical_core-0.9.0.tar`

### file list

```diff
@@ -1,24 +1,28 @@
--rw-r--r--   0        0        0     1089 2023-05-12 13:26:24.233918 ansys-mechanical-core-0.8.0/LICENSE
--rw-r--r--   0        0        0     5456 2023-05-12 13:26:24.233918 ansys-mechanical-core-0.8.0/README.rst
--rw-r--r--   0        0        0     3943 2023-05-12 13:26:24.241918 ansys-mechanical-core-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     1242 2023-05-12 13:26:24.241918 ansys-mechanical-core-0.8.0/src/ansys/mechanical/core/__init__.py
--rw-r--r--   0        0        0      536 2023-05-12 13:26:24.241918 ansys-mechanical-core-0.8.0/src/ansys/mechanical/core/_version.py
--rw-r--r--   0        0        0      167 2023-05-12 13:26:24.241918 ansys-mechanical-core-0.8.0/src/ansys/mechanical/core/embedding/__init__.py
--rw-r--r--   0        0        0     5219 2023-05-12 13:26:24.241918 ansys-mechanical-core-0.8.0/src/ansys/mechanical/core/embedding/app.py
--rw-r--r--   0        0        0     1392 2023-05-12 13:26:24.241918 ansys-mechanical-core-0.8.0/src/ansys/mechanical/core/embedding/config.py
--rw-r--r--   0        0        0      819 2023-05-12 13:26:24.241918 ansys-mechanical-core-0.8.0/src/ansys/mechanical/core/embedding/imports.py
--rw-r--r--   0        0        0     1825 2023-05-12 13:26:24.241918 ansys-mechanical-core-0.8.0/src/ansys/mechanical/core/embedding/initializer.py
--rw-r--r--   0        0        0     1958 2023-05-12 13:26:24.241918 ansys-mechanical-core-0.8.0/src/ansys/mechanical/core/embedding/loader.py
--rw-r--r--   0        0        0     2022 2023-05-12 13:26:24.241918 ansys-mechanical-core-0.8.0/src/ansys/mechanical/core/embedding/logging.py
--rw-r--r--   0        0        0      852 2023-05-12 13:26:24.241918 ansys-mechanical-core-0.8.0/src/ansys/mechanical/core/embedding/resolver.py
--rw-r--r--   0        0        0     1287 2023-05-12 13:26:24.241918 ansys-mechanical-core-0.8.0/src/ansys/mechanical/core/embedding/runtime.py
--rw-r--r--   0        0        0      703 2023-05-12 13:26:24.245918 ansys-mechanical-core-0.8.0/src/ansys/mechanical/core/embedding/shims.py
--rw-r--r--   0        0        0     3312 2023-05-12 13:26:24.245918 ansys-mechanical-core-0.8.0/src/ansys/mechanical/core/errors.py
--rw-r--r--   0        0        0      113 2023-05-12 13:26:24.245918 ansys-mechanical-core-0.8.0/src/ansys/mechanical/core/examples/__init__.py
--rw-r--r--   0        0        0     2992 2023-05-12 13:26:24.245918 ansys-mechanical-core-0.8.0/src/ansys/mechanical/core/examples/downloads.py
--rw-r--r--   0        0        0     5505 2023-05-12 13:26:24.245918 ansys-mechanical-core-0.8.0/src/ansys/mechanical/core/launcher.py
--rw-r--r--   0        0        0    23658 2023-05-12 13:26:24.245918 ansys-mechanical-core-0.8.0/src/ansys/mechanical/core/logging.py
--rw-r--r--   0        0        0    87557 2023-05-12 13:26:24.245918 ansys-mechanical-core-0.8.0/src/ansys/mechanical/core/mechanical.py
--rw-r--r--   0        0        0     4215 2023-05-12 13:26:24.245918 ansys-mechanical-core-0.8.0/src/ansys/mechanical/core/misc.py
--rw-r--r--   0        0        0    25243 2023-05-12 13:26:24.245918 ansys-mechanical-core-0.8.0/src/ansys/mechanical/core/pool.py
--rw-r--r--   0        0        0     8130 1970-01-01 00:00:00.000000 ansys-mechanical-core-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-06-13 15:12:57.796721 ansys_mechanical_core-0.9.0/LICENSE
+-rw-r--r--   0        0        0     5448 2023-06-13 15:12:57.796721 ansys_mechanical_core-0.9.0/README.rst
+-rw-r--r--   0        0        0     4042 2023-06-13 15:12:57.804721 ansys_mechanical_core-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     1236 2023-06-13 15:12:57.804721 ansys_mechanical_core-0.9.0/src/ansys/mechanical/core/__init__.py
+-rw-r--r--   0        0        0      536 2023-06-13 15:12:57.804721 ansys_mechanical_core-0.9.0/src/ansys/mechanical/core/_version.py
+-rw-r--r--   0        0        0      138 2023-06-13 15:12:57.804721 ansys_mechanical_core-0.9.0/src/ansys/mechanical/core/embedding/__init__.py
+-rw-r--r--   0        0        0     4266 2023-06-13 15:12:57.804721 ansys_mechanical_core-0.9.0/src/ansys/mechanical/core/embedding/app.py
+-rw-r--r--   0        0        0     1392 2023-06-13 15:12:57.804721 ansys_mechanical_core-0.9.0/src/ansys/mechanical/core/embedding/config.py
+-rw-r--r--   0        0        0      819 2023-06-13 15:12:57.804721 ansys_mechanical_core-0.9.0/src/ansys/mechanical/core/embedding/imports.py
+-rw-r--r--   0        0        0     3697 2023-06-13 15:12:57.804721 ansys_mechanical_core-0.9.0/src/ansys/mechanical/core/embedding/initializer.py
+-rw-r--r--   0        0        0     1958 2023-06-13 15:12:57.804721 ansys_mechanical_core-0.9.0/src/ansys/mechanical/core/embedding/loader.py
+-rw-r--r--   0        0        0     6761 2023-06-13 15:12:57.804721 ansys_mechanical_core-0.9.0/src/ansys/mechanical/core/embedding/logger/__init__.py
+-rw-r--r--   0        0        0     4603 2023-06-13 15:12:57.804721 ansys_mechanical_core-0.9.0/src/ansys/mechanical/core/embedding/logger/environ.py
+-rw-r--r--   0        0        0     4834 2023-06-13 15:12:57.804721 ansys_mechanical_core-0.9.0/src/ansys/mechanical/core/embedding/logger/linux_api.py
+-rw-r--r--   0        0        0      238 2023-06-13 15:12:57.804721 ansys_mechanical_core-0.9.0/src/ansys/mechanical/core/embedding/logger/sinks.py
+-rw-r--r--   0        0        0     4094 2023-06-13 15:12:57.804721 ansys_mechanical_core-0.9.0/src/ansys/mechanical/core/embedding/logger/windows_api.py
+-rw-r--r--   0        0        0      852 2023-06-13 15:12:57.804721 ansys_mechanical_core-0.9.0/src/ansys/mechanical/core/embedding/resolver.py
+-rw-r--r--   0        0        0     1287 2023-06-13 15:12:57.804721 ansys_mechanical_core-0.9.0/src/ansys/mechanical/core/embedding/runtime.py
+-rw-r--r--   0        0        0      703 2023-06-13 15:12:57.804721 ansys_mechanical_core-0.9.0/src/ansys/mechanical/core/embedding/shims.py
+-rw-r--r--   0        0        0     3312 2023-06-13 15:12:57.804721 ansys_mechanical_core-0.9.0/src/ansys/mechanical/core/errors.py
+-rw-r--r--   0        0        0      113 2023-06-13 15:12:57.804721 ansys_mechanical_core-0.9.0/src/ansys/mechanical/core/examples/__init__.py
+-rw-r--r--   0        0        0     2990 2023-06-13 15:12:57.804721 ansys_mechanical_core-0.9.0/src/ansys/mechanical/core/examples/downloads.py
+-rw-r--r--   0        0        0     5505 2023-06-13 15:12:57.804721 ansys_mechanical_core-0.9.0/src/ansys/mechanical/core/launcher.py
+-rw-r--r--   0        0        0    23658 2023-06-13 15:12:57.808721 ansys_mechanical_core-0.9.0/src/ansys/mechanical/core/logging.py
+-rw-r--r--   0        0        0    78531 2023-06-13 15:12:57.808721 ansys_mechanical_core-0.9.0/src/ansys/mechanical/core/mechanical.py
+-rw-r--r--   0        0        0     4215 2023-06-13 15:12:57.808721 ansys_mechanical_core-0.9.0/src/ansys/mechanical/core/misc.py
+-rw-r--r--   0        0        0    25279 2023-06-13 15:12:57.808721 ansys_mechanical_core-0.9.0/src/ansys/mechanical/core/pool.py
+-rw-r--r--   0        0        0     8155 1970-01-01 00:00:00.000000 ansys_mechanical_core-0.9.0/PKG-INFO
```

### Comparing `ansys-mechanical-core-0.8.0/LICENSE` & `ansys_mechanical_core-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-core-0.8.0/README.rst` & `ansys_mechanical_core-0.9.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -10,20 +10,20 @@
    :target: https://pypi.org/project/ansys-mechanical-core
    :alt: Python
 
 .. |pypi| image:: https://img.shields.io/pypi/v/ansys-mechanical-core.svg?logo=python&logoColor=white
    :target: https://pypi.org/project/ansys-mechanical-core
    :alt: PyPI
 
-.. |codecov| image:: https://codecov.io/gh/pyansys/pymechanical/branch/main/graph/badge.svg
-   :target: https://codecov.io/gh/pyansys/ansys-mechanical-core
+.. |codecov| image:: https://codecov.io/gh/ansys/pymechanical/branch/main/graph/badge.svg
+   :target: https://codecov.io/gh/ansys/ansys-mechanical-core
    :alt: Codecov
 
-.. |GH-CI| image:: https://github.com/pyansys/pymechanical/actions/workflows/ci_cd.yml/badge.svg
-   :target: https://github.com/pyansys/pymechanical/actions/workflows/ci_cd.yml
+.. |GH-CI| image:: https://github.com/ansys/pymechanical/actions/workflows/ci_cd.yml/badge.svg
+   :target: https://github.com/ansys/pymechanical/actions/workflows/ci_cd.yml
    :alt: GH-CI
 
 .. |MIT| image:: https://img.shields.io/badge/License-MIT-yellow.svg
    :target: https://opensource.org/licenses/MIT
    :alt: MIT
 
 .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg?style=flat
```

### Comparing `ansys-mechanical-core-0.8.0/pyproject.toml` & `ansys_mechanical_core-0.9.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 # Check https://flit.readthedocs.io/en/latest/pyproject_toml.html for all available sections
 name = "ansys-mechanical-core"
-version = "0.8.0"
+version = "0.9.0"
 description = "A python wrapper for Ansys Mechanical"
 readme = "README.rst"
 requires-python = ">=3.7,<4.0"
 license = {file = "LICENSE"}
 authors = [
     {name = "ANSYS, Inc.", email = "pyansys.core@ansys.com"},
 ]
@@ -26,50 +26,51 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "ansys_api_mechanical==0.1.0",
-    "ansys-pythonnet==3.1.0rc1",
+    "ansys-pythonnet>=3.1.0rc1",
+    "ansys-tools-path>=0.2.3",
     "importlib-metadata>=4.0",
     "appdirs>=1.4.0",
     "grpcio>=1.30.0",
     "protobuf>=3.12.2,<3.21.0",
     "ansys-platform-instancemanagement>=1.0.1",
     "tqdm>=4.45.0",
 ]
 
 [project.urls]
 Documentation = "https://mechanical.docs.pyansys.com"
-Source = "https://github.com/pyansys/pymechanical"
-Homepage = "https://github.com/pyansys/pymechanical"
-Tracker = "https://github.com/pyansys/pymechanical/issues"
+Source = "https://github.com/ansys/pymechanical"
+Homepage = "https://github.com/ansys/pymechanical"
+Tracker = "https://github.com/ansys/pymechanical/issues"
 
 [project.optional-dependencies]
 tests = [
-    "pytest==7.3.1",
-    "pytest-cov==4.0.0",
+    "pytest==7.3.2",
+    "pytest-cov==4.1.0",
     "pytest-print==0.3.1",
 ]
 doc = [
-    "Sphinx==6.2.0", # BLOCKED BY sphinx-design - Cannot upgrade to Sphinx 7 for now
-    "ansys-sphinx-theme==0.9.8",
-    "grpcio==1.54.0",
+    "Sphinx==6.2.1", # BLOCKED BY sphinx-design - Cannot upgrade to Sphinx 7 for now
+    "ansys-sphinx-theme==0.9.9",
+    "grpcio==1.54.2",
     "imageio-ffmpeg==0.4.8",
-    "imageio==2.28.1",
+    "imageio==2.31.1",
     "jupyter_sphinx==0.4.0",
     "jupyterlab>=3.2.8",
     "matplotlib==3.7.1",
     "numpydoc==1.5.0",
-    "plotly==5.14.1",
+    "plotly==5.15.0",
     "pypandoc==1.11",
     "pytest-sphinx==0.5.0",
     "pythreejs==2.4.2",
-    "pyvista==0.39.0",
+    "pyvista==0.39.1",
     "sphinx-autobuild==2021.3.14",
     "sphinx-autodoc-typehints==1.23.0",
     "sphinx-copybutton==0.5.2",
     "sphinx_design==0.4.1",
     "sphinx-gallery==0.13.0",
     "sphinx-notfound-page==0.8.3",
     "sphinxcontrib-websupport==1.2.4",
@@ -114,11 +115,12 @@
 # --cov=ansys.mechanical --cov-report html:.cov/html --cov-report xml:.cov/xml --cov-report \
 # term -vv --print --print-relative-time"""
 testpaths = [
     "tests",
 ]
 markers = [
     "embedding: tests that embed Mechanical in the python process",
+    "python_env: tests that check for an appropriate python environment",
     "remote_session_launch: tests that launch Mechanical and work with gRPC server inside it",
     "remote_session_connect: tests that connect to Mechanical and work with gRPC server inside it",
 ]
 xfail_strict = true
```

### Comparing `ansys-mechanical-core-0.8.0/src/ansys/mechanical/core/__init__.py` & `ansys_mechanical_core-0.9.0/src/ansys/mechanical/core/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,33 @@
 """Initialize the package level imports."""
 import logging
 import os
 
+from ansys.tools.path import find_mechanical
 import appdirs
 
+# Setup data directory
+USER_DATA_PATH = appdirs.user_data_dir(appname="ansys_mechanical_core", appauthor="Ansys")
+if not os.path.exists(USER_DATA_PATH):
+    os.makedirs(USER_DATA_PATH)
+
+EXAMPLES_PATH = os.path.join(USER_DATA_PATH, "examples")
+if not os.path.exists(EXAMPLES_PATH):
+    os.makedirs(EXAMPLES_PATH)
+
 from ansys.mechanical.core.logging import Logger
 
 # Create logger for package level use
 LOG = Logger(level=logging.ERROR, to_file=False, to_stdout=True)
 LOG.debug("Loaded logging module as LOG")
 
 from ansys.mechanical.core._version import __version__
 from ansys.mechanical.core.mechanical import (
     change_default_mechanical_path,
     close_all_local_instances,
-    find_mechanical,
     get_mechanical_path,
     launch_mechanical,
 )
 
 # import few classes / functions
 from ansys.mechanical.core.mechanical import Mechanical as Mechanical
 
@@ -31,20 +40,7 @@
 
 # manage the package level ports
 LOCAL_PORTS = []
 
 from ansys.mechanical.core.pool import LocalMechanicalPool
 
 BUILDING_GALLERY = False
-
-# Setup data directory
-try:
-    USER_DATA_PATH = appdirs.user_data_dir("ansys_mechanical_core")
-    if not os.path.exists(USER_DATA_PATH):
-        os.makedirs(USER_DATA_PATH)
-
-    EXAMPLES_PATH = os.path.join(USER_DATA_PATH, "examples")
-    if not os.path.exists(EXAMPLES_PATH):
-        os.makedirs(EXAMPLES_PATH)
-
-except Exception:
-    pass
```

### Comparing `ansys-mechanical-core-0.8.0/src/ansys/mechanical/core/_version.py` & `ansys_mechanical_core-0.9.0/src/ansys/mechanical/core/_version.py`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-core-0.8.0/src/ansys/mechanical/core/embedding/app.py` & `ansys_mechanical_core-0.9.0/src/ansys/mechanical/core/embedding/app.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,15 @@
 """Main application class for embedded Mechanical."""
 import atexit
 import os
-import typing
 
 from ansys.mechanical.core.embedding import initializer, runtime
 from ansys.mechanical.core.embedding.config import Configuration, configure
 
 
-def _get_available_versions() -> typing.Dict[int, str]:
-    supported_versions = [222, 231, 232]
-    if os.name == "nt":  # pragma: no cover
-        supported_versions = [222, 231, 232]
-        awp_roots = {ver: os.environ.get(f"AWP_ROOT{ver}", "") for ver in supported_versions}
-        installed_versions = {
-            ver: path for ver, path in awp_roots.items() if path and os.path.isdir(path)
-        }
-        return installed_versions
-    else:
-        # TODO - this assumes the env var is set.
-        return {232: os.environ["AWP_ROOT232"]}
-
-
-def _get_default_version() -> int:
-    vers = _get_available_versions()
-    if not vers:  # pragma: no cover
-        raise Exception(
-            "Appropriate version of Ansys Mechanical is not installed. Must be at least v222"
-        )
-    return max(vers.keys())
-
-
 def _get_default_configuration() -> Configuration:
     configuration = Configuration()
     if os.name != "nt":
         configuration.no_act_addins = True
     return configuration
 
 
@@ -63,30 +39,27 @@
                 self._app = INSTANCES[0]
                 self._app.new()
                 self._version = self._app.version
                 self._disposed = True
                 return
         if len(INSTANCES) > 0:
             raise Exception("Cannot have more than one embedded mechanical instance")
-        self._version = kwargs.get("version")
-        if self._version == None:
-            self._version = _get_default_version()
-        initializer.initialize(self._version)
+        version = kwargs.get("version")
+        self._version = initializer.initialize(version)
         import clr
 
         clr.AddReference("Ansys.Mechanical.Embedding")
         import Ansys
 
         configuration = kwargs.get("config", _get_default_configuration())
         configure(configuration)
         self._app = Ansys.Mechanical.Embedding.Application(db_file)
         runtime.initialize(self._version)
         self._disposed = False
-        if len(INSTANCES) == 0:
-            atexit.register(_dispose_embedded_app, INSTANCES)
+        atexit.register(_dispose_embedded_app, INSTANCES)
         INSTANCES.append(self)
 
     def __repr__(self):
         """Get the product info."""
         if self._version < 232:  # pragma: no cover
             return "Ansys Mechanical"
         import clr
```

### Comparing `ansys-mechanical-core-0.8.0/src/ansys/mechanical/core/embedding/config.py` & `ansys_mechanical_core-0.9.0/src/ansys/mechanical/core/embedding/config.py`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-core-0.8.0/src/ansys/mechanical/core/embedding/imports.py` & `ansys_mechanical_core-0.9.0/src/ansys/mechanical/core/embedding/imports.py`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-core-0.8.0/src/ansys/mechanical/core/embedding/loader.py` & `ansys_mechanical_core-0.9.0/src/ansys/mechanical/core/embedding/loader.py`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-core-0.8.0/src/ansys/mechanical/core/embedding/resolver.py` & `ansys_mechanical_core-0.9.0/src/ansys/mechanical/core/embedding/resolver.py`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-core-0.8.0/src/ansys/mechanical/core/embedding/runtime.py` & `ansys_mechanical_core-0.9.0/src/ansys/mechanical/core/embedding/runtime.py`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-core-0.8.0/src/ansys/mechanical/core/embedding/shims.py` & `ansys_mechanical_core-0.9.0/src/ansys/mechanical/core/embedding/shims.py`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-core-0.8.0/src/ansys/mechanical/core/errors.py` & `ansys_mechanical_core-0.9.0/src/ansys/mechanical/core/errors.py`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-core-0.8.0/src/ansys/mechanical/core/examples/downloads.py` & `ansys_mechanical_core-0.9.0/src/ansys/mechanical/core/examples/downloads.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         if base[-1] != "/":
             base += "/"
         base = urljoin(base, path)
     return base
 
 
 def _get_default_server_and_joiner():
-    return "https://github.com/pyansys/example-data/raw/master", _joinurl
+    return "https://github.com/ansys/example-data/raw/master", _joinurl
 
 
 def _get_filepath_on_default_server(filename: str, *directory: str):
     server, joiner = _get_default_server_and_joiner()
     if directory:
         return joiner(server, *directory, filename)
     else:
```

### Comparing `ansys-mechanical-core-0.8.0/src/ansys/mechanical/core/launcher.py` & `ansys_mechanical_core-0.9.0/src/ansys/mechanical/core/launcher.py`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-core-0.8.0/src/ansys/mechanical/core/logging.py` & `ansys_mechanical_core-0.9.0/src/ansys/mechanical/core/logging.py`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-core-0.8.0/src/ansys/mechanical/core/mechanical.py` & `ansys_mechanical_core-0.9.0/src/ansys/mechanical/core/mechanical.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,26 +3,24 @@
 from contextlib import closing
 import datetime
 import fnmatch
 from functools import wraps
 import glob
 import os
 import pathlib
-import re
 import socket
 import threading
 import time
-import warnings
 import weakref
 
 import ansys.api.mechanical.v0.mechanical_pb2 as mechanical_pb2
 import ansys.api.mechanical.v0.mechanical_pb2_grpc as mechanical_pb2_grpc
 import ansys.platform.instancemanagement as pypim
 from ansys.platform.instancemanagement import Instance
-import appdirs
+import ansys.tools.path as atp
 import grpc
 
 import ansys.mechanical.core as pymechanical
 from ansys.mechanical.core import LOG
 from ansys.mechanical.core.errors import (
     MechanicalExitedError,
     MechanicalRuntimeError,
@@ -30,16 +28,14 @@
     protect_grpc,
 )
 from ansys.mechanical.core.launcher import MechanicalLauncher
 from ansys.mechanical.core.misc import (
     check_valid_ip,
     check_valid_port,
     check_valid_start_instance,
-    is_float,
-    is_windows,
     threaded,
 )
 
 # Checking if tqdm is installed.
 # If it is, the default value for progress_bar is true.
 try:
     from tqdm import tqdm
@@ -89,27 +85,14 @@
             mechanical.set_log_level(prior_log_level)
 
         return out
 
     return wrapper
 
 
-SETTINGS_DIR = appdirs.user_data_dir("ansys_mechanical_core")
-LOG.info(f"ansys_mechanical_core settings directory: {SETTINGS_DIR}")
-
-if not os.path.isdir(SETTINGS_DIR):
-    try:
-        os.makedirs(SETTINGS_DIR)
-    except OSError:  # pragma: no cover
-        warnings.warn(
-            "Unable to create settings directory.\n"
-            "Will be unable to cache Mechanical executable location."
-        )
-
-CONFIG_FILE = os.path.join(SETTINGS_DIR, "config.txt")
 LOCALHOST = "127.0.0.1"
 MECHANICAL_DEFAULT_PORT = 10000
 
 GALLERY_INSTANCE = [None]
 
 
 def _cleanup_gallery_instance():  # pragma: no cover
@@ -121,41 +104,14 @@
         )
         mechanical.exit(force=True)
 
 
 atexit.register(_cleanup_gallery_instance)
 
 
-def _version_from_path(path):
-    """Extract the Mechanical version from a path.
-
-    Generally, the version of Mechanical is contained in the path:
-
-    - On Windows, for example: ``C:/Program Files/ANSYS Inc/v231/aisol/bin/winx64/AnsysWBU.exe``
-    - On Linux, for example: ``/usr/ansys_inc/v231/aisol/.workbench``
-
-    Parameters
-    ----------
-    path : str
-        Path to the Mechanical executable file.
-
-    Returns
-    -------
-    int
-        Integer version number (for example, 231).
-
-    """
-    # expect v<ver>/ansys
-    # replace \\ with / to account for possible windows path
-    matches = re.findall(r"v(\d\d\d)", path.replace("\\", "/"), re.IGNORECASE)
-    if not matches:
-        raise RuntimeError(f"Unable to extract Mechanical version from {path}.")
-    return int(matches[-1])
-
-
 def port_in_use(port, host=LOCALHOST):
     """Check whether a port is in use at the given host.
 
     You must actually *bind* the address. Just checking if you can create
     a socket is insufficient because it is possible to run into permission
     errors like::
 
@@ -229,299 +185,58 @@
 def create_ip_file(ip, path):
     """Create the ``mylocal.ip`` file needed to change the IP address of the gRPC server."""
     file_name = os.path.join(path, "mylocal.ip")
     with open(file_name, "w", encoding="utf-8") as f:
         f.write(ip)
 
 
-def _get_available_base_mechanical():
-    r"""Get a dictionary of available Mechanical versions with their base paths.
-
-    Returns
-    -------
-        Paths for Mechanical versions installed on Windows.
-
-    Examples
-    --------
-    On Windows:
-
-    >>> _get_available_base_mechanical()
-    >>> {231: 'C:\\Program Files\\ANSYS Inc\\v231'}
-
-    On Linux:
-
-    >>> _get_available_base_mechanical()
-    >>> {231: '/usr/ansys_inc/v231'}
-    """
-    base_path = None
-    if is_windows():
-        supported_versions = [232, 231]
-        awp_roots = {ver: os.environ.get(f"AWP_ROOT{ver}", "") for ver in supported_versions}
-        installed_versions = {
-            ver: path for ver, path in awp_roots.items() if path and os.path.isdir(path)
-        }
-        if installed_versions:
-            return installed_versions
-        else:
-            base_path = os.path.join(os.environ["PROGRAMFILES"], "ANSYS Inc")
-    else:
-        for path in ["/usr/ansys_inc", "/ansys_inc", "/install/ansys_inc"]:
-            if os.path.isdir(path):
-                base_path = path
-
-    if base_path is None:
-        return {}
-
-    paths = glob.glob(os.path.join(base_path, "v*"))
-
-    if not paths:
-        return {}
-
-    ansys_paths = {}
-    for path in paths:
-        ver_str = path[-3:]
-        if is_float(ver_str):
-            ansys_paths[int(ver_str)] = path
-
-    return ansys_paths
-
-
-def find_mechanical():
-    """
-    Search for the Mechanical path in the standard installation location.
-
-    Returns
-    -------
-    mechanical_path : str
-        Full path to the executable file for the latest Mechanical version.
-    version : float
-        Version in the float format. For example, ``23.1`` for 2023 R1.
-
-    Examples
-    --------
-    On Windows:
-
-    >>> from ansys.mechanical.core.mechanical import find_mechanical
-    >>> find_mechanical()
-    'C:/Program Files/ANSYS Inc/v231/aisol/bin/winx64/AnsysWBU.exe', 23.1
-
-    On Linux:
-
-    >>> find_mechanical()
-    (/usr/ansys_inc/v231/aisol/.workbench, 23.1)
-    """
-    versions = _get_available_base_mechanical()
-    if not versions:
-        return "", ""
-    version = max(versions.keys())
-    ans_path = versions[version]
-    if is_windows():
-        mechanical_bin = os.path.join(ans_path, "aisol", "bin", "winx64", f"AnsysWBU.exe")
-    else:
-        mechanical_bin = os.path.join(ans_path, "aisol", ".workbench")
-    return mechanical_bin, version / 10
-
-
 def get_mechanical_path(allow_input=True):
-    """Get the Mechanical path from a cached file or from user input."""
-    exe_loc = None
-    if os.path.isfile(CONFIG_FILE):
-        with open(CONFIG_FILE, "r", encoding="utf-8") as f:
-            exe_loc = f.read()
-        # verify
-        if not os.path.isfile(exe_loc) and allow_input:
-            exe_loc = save_mechanical_path()
-    elif allow_input:  # create configuration file
-        exe_loc = save_mechanical_path()
-    if exe_loc is None:
-        exe_loc = find_mechanical()[0]
-        if not exe_loc:
-            exe_loc = None
+    """Get path.
 
-    return exe_loc
+    Deprecated - use `ansys.tools.path.get_mechanical_path` instead
+    """
+    return atp.get_mechanical_path(allow_input)
 
 
 def check_valid_mechanical():
-    """Check if a valid version of Mechanical is installed and preconfigured."""
-    mechanical_bin = get_mechanical_path(allow_input=False)
-    if mechanical_bin is not None:
-        version = _version_from_path(mechanical_bin)
-        return not (version < 231 and os.name != "posix")
-    return False
-
-
-def change_default_mechanical_path(exe_loc):
-    """Change your default Mechanical path.
-
-    Parameters
-    ----------
-    exe_loc : str
-        Full path for the Mechanical executable file to use.
+    """Change to see if the default Mechanical path is valid.
 
-    Examples
-    --------
-    On Windows:
+    Example (windows)
+    -----------------
 
-    >>> mechanical_pth = 'C:/Program Files/ANSYS Inc/v231/aisol/bin/win64/AnsysWBU.exe'
-    >>> mechanical.change_default_mechanical_path(mechanical_pth)
+    >>> from ansys.mechanical.core import mechanical
+    >>> from ansys.tools.path import change_default_mechanical_path
+    >>> mechanical_path = 'C:/Program Files/ANSYS Inc/v231/aisol/bin/win64/AnsysWBU.exe'
+    >>> change_default_mechanical_path(mechanical_pth)
     >>> mechanical.check_valid_mechanical()
     True
 
-    On Linux:
-
-    >>> from ansys.mechanical.core import mechanical
-    >>> mechanical.change_default_mechanical_path('/ansys_inc/v231/aisol/.workbench')
-    >>> mechanical.get_mechanical_path()
-    '/ansys_inc/v231/aisol/.workbench'
 
     """
-    if os.path.isfile(exe_loc):
-        with open(CONFIG_FILE, "w", encoding="utf-8") as f:
-            f.write(exe_loc)
-    else:
-        raise FileNotFoundError("File %s is invalid or does not exist" % exe_loc)
-
-
-def save_mechanical_path(exe_loc=None):  # pragma: no cover
-    """Find the Mechanical path or query user.
-
-    Parameters
-    ----------
-    exe_loc : string, optional
-        Path for the Mechanical executable file (``AnsysWBU.exe``).
-        The default is ``None``, in which case an attempt is made to
-        obtain the path from the following sources in this order:
-
-        - The default Mechanical paths (for example,
-          ``C:/Program Files/Ansys Inc/vXXX/aiso/bin/AnsysWBU.exe``)
-        - The configuration file
-        - User input
-
-        If a path is supplied, this method performs some checks. If the
-        checks are aresuccessful, it writes this path to the configuration
-        file.
+    mechanical_path = atp.get_mechanical_path(False)
+    if mechanical_path == None:
+        return False
+    mechanical_version = atp.version_from_path("mechanical", mechanical_path)
+    return not (mechanical_version < 231 and os.name != "posix")
 
-    Returns
-    -------
-    str
-        Path for the Mechanical executable file.
 
-    Notes
-    -----
-    The location of the configuration file (``config.txt``) can be found in
-    ``appdirs.user_data_dir("ansys_mechanical_core")``. For example:
-
-    .. code:: pycon
-
-        >>> import appdirs
-        >>> import os
-        >>> print(os.path.join(appdirs.user_data_dir("ansys_mechanical_core"), "config.txt"))
-        C:/Users/[username]]/AppData/Local/ansys_mechanical_core/ansys_mechanical_core/config.txt
-
-    You can change the default for the ``exe_loc`` parameter either by modifying the
-    ``config.txt`` file or by running this code:
-
-    .. code:: pycon
-
-       >>> from ansys.mechanical.core.mechanical import save_mechanical_path
-       >>> save_mechanical_path("/new/path/to/executable")
+def change_default_mechanical_path(exe_loc):
+    """Change default path.
 
+    Deprecated - use `ansys.tools.path.change_default_mechanical_path` instead.
     """
-    if exe_loc is None:
-        exe_loc, _ = find_mechanical()
+    return atp.change_default_mechanical_path(exe_loc)
 
-    if is_valid_executable_path(exe_loc):  # pragma: not cover
-        if not is_common_executable_path(exe_loc):
-            warn_uncommon_executable_path(exe_loc)
-
-        change_default_mechanical_path(exe_loc)
-        return exe_loc
-
-    if exe_loc is not None:
-        if is_valid_executable_path(exe_loc):
-            return exe_loc  # pragma: no cover
-
-    # otherwise, query user for the location
-    print("Cached Mechanical executable file is not found.")
-    print(
-        "You are about to enter manually the path of the Mechanical executable file "
-        "(.workbench). This file is very likely contained in the path ending in "
-        "'vXXX/aisol/.workbench', but it is not required.\n \nIf you experience problems "
-        "with the input path, you can overwrite the configuration file with this code:\n"
-        ">>> from ansys.mechanical.core.mechanical import save_mechanical_path\n"
-        ">>> save_mechanical_path('/new/path/to/executable/')\n"
-    )
-    need_path = True
-    while need_path:  # pragma: no cover
-        exe_loc = input("Enter the location of an Mechanical executable file (.workbench):")
-
-        if is_valid_executable_path(exe_loc):
-            if not is_common_executable_path(exe_loc):
-                warn_uncommon_executable_path(exe_loc)
-            with open(CONFIG_FILE, "w", encoding="utf-8") as f:
-                f.write(exe_loc)
-            need_path = False
-        else:
-            print("The supplied path is either invalid or does not " "match the '.workbench' name.")
-
-    return exe_loc
-
-
-def is_valid_executable_path(exe_loc):  # pragma: no cover
-    """Check whether the given location for the Mechanical executable file is valid."""
-    if is_windows():
-        return (
-            os.path.isfile(exe_loc)
-            and re.search("AnsysWBU.exe", os.path.basename(os.path.normpath(exe_loc))) is not None
-        )
-    return (
-        os.path.isfile(exe_loc)
-        and re.search(".workbench", os.path.basename(os.path.normpath(exe_loc))) is not None
-    )
-
-
-def is_common_executable_path(exe_loc):  # pragma: no cover
-    """Check whether the give location for the Mechanical executable file is valid."""
-    path = os.path.normpath(exe_loc)
-    path = path.split(os.sep)
-
-    is_valid_path = is_valid_executable_path(exe_loc)
-
-    if is_windows():
-        return (
-            is_valid_path
-            and re.search(r"v\d\d\d", exe_loc)
-            and "aisol" in path
-            and "bin" in path
-            and "winx64" in path
-            and "AnsysWBU.exe" in path
-        )
-
-    return (
-        is_valid_path
-        and re.search(r"v\d\d\d", exe_loc)
-        and "aisol" in path
-        and ".workbench" in path
-    )
 
+def save_mechanical_path(exe_loc=None):  # pragma: no cover
+    """Save path.
 
-def warn_uncommon_executable_path(exe_loc):  # pragma: no cover
-    """Display warning if the location is wrong for the Mechanical executable file."""
-    if is_windows():
-        warnings.warn(
-            f"The supplied path ('{exe_loc}') does not match the usual Mechanical "
-            f"executable path style ('directory/vXXX/aisol/bin/winx64/AnsysWBU.exe'). "
-            "You might have problems at later use."
-        )
-    else:
-        warnings.warn(
-            f"The supplied path ('{exe_loc}') does not match the usual Mechanical "
-            f"executable path style ('directory/vXXX/aisol/.workbench'). "
-            "You might have problems at later use."
-        )
+    Deprecated - use `ansys.tools.path.save_mechanical_path` instead.
+    """
+    return atp.save_mechanical_path(exe_loc)
 
 
 client_to_server_loglevel = {
     "DEBUG": 1,
     "INFO": 2,
     "WARN": 3,
     "WARNING": 3,
@@ -2164,15 +1879,15 @@
     Launch Mechanical using a specified executable file.
 
     >>> exec_file_path = 'C:/Program Files/ANSYS Inc/v231/aisol/bin/win64/AnsysWBU.exe'
     >>> mechanical = launch_mechanical(exec_file_path)
 
     """
     # verify version
-    if _version_from_path(exec_file) < 231:
+    if atp.version_from_path("mechanical", exec_file) < 231:
         raise VersionError("The Mechanical gRPC interface requires Mechanical 2023 R1 or later.")
 
     # get the next available port
     local_ports = pymechanical.LOCAL_PORTS
     if port is None:
         if not local_ports:
             port = MECHANICAL_DEFAULT_PORT
@@ -2223,14 +1938,15 @@
         ]
     )
 
     return channel, instance
 
 
 def launch_mechanical(
+    allow_input=True,
     exec_file=None,
     batch=True,
     loglevel="ERROR",
     log_file=False,
     log_mechanical=None,
     additional_switches=None,
     additional_envs=None,
@@ -2244,14 +1960,17 @@
     version=None,
     keep_connection_alive=True,
 ) -> Mechanical:
     """Start Mechanical locally.
 
     Parameters
     ----------
+    allow_input: bool, optional
+        Whether to allow user input when discovering the path to the Mechanical
+        executable file.
     exec_file : str, optional
         Path for the Mechanical executable file. The default is ``None``,
         in which case the cached location is used. If PyPIM is configured
         and this parameter is set to ``None``, PyPIM launches Mechanical
         using its ``version`` parameter.
     batch : bool, optional
         Whether to launch Mechanical in batch mode. The default is ``True``.
@@ -2449,15 +2168,15 @@
         if ip != LOCALHOST:  # Default local ip is 127.0.0.1
             create_ip_file(ip, os.getcwd())
 
         return mechanical
 
     # verify executable
     if exec_file is None:
-        exec_file = get_mechanical_path()
+        exec_file = get_mechanical_path(allow_input)
         if exec_file is None:  # pragma: no cover
             raise FileNotFoundError(
                 "Path to the Mechanical executable file is invalid or cache cannot be loaded. "
                 "Enter a path manually by specifying a value for the "
                 "'exec_file' parameter."
             )
     else:  # verify ansys exists at this location
```

### Comparing `ansys-mechanical-core-0.8.0/src/ansys/mechanical/core/misc.py` & `ansys_mechanical_core-0.9.0/src/ansys/mechanical/core/misc.py`

 * *Files identical despite different names*

### Comparing `ansys-mechanical-core-0.8.0/src/ansys/mechanical/core/pool.py` & `ansys_mechanical_core-0.9.0/src/ansys/mechanical/core/pool.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """This module is for threaded implementations of the Mechanical interface."""
 
 import os
 import time
 import warnings
 
 import ansys.platform.instancemanagement as pypim
+from ansys.tools.path import version_from_path
 
 from ansys.mechanical.core.errors import VersionError
 from ansys.mechanical.core.mechanical import (
     _HAS_TQDM,
     LOG,
     MECHANICAL_DEFAULT_PORT,
-    _version_from_path,
     get_mechanical_path,
     launch_mechanical,
     port_in_use,
 )
 from ansys.mechanical.core.misc import threaded, threaded_daemon
 
 if _HAS_TQDM:
@@ -165,15 +165,15 @@
                     raise FileNotFoundError(
                         "Path to Mechanical executable file is invalid or cache cannot be loaded. "
                         "Enter a path manually by specifying a value for the "
                         "'exec_file' parameter."
                     )
 
         if not self._remote:  # pragma: no cover
-            if _version_from_path(exec_file) < 231:
+            if version_from_path("mechanical", exec_file) < 231:
                 raise VersionError("A local Mechanical pool requires Mechanical 2023 R1 or later.")
 
         ports = None
 
         if not self._remote:
             # grab available ports
             ports = available_ports(n_instances, port)
```

### Comparing `ansys-mechanical-core-0.8.0/PKG-INFO` & `ansys_mechanical_core-0.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansys-mechanical-core
-Version: 0.8.0
+Version: 0.9.0
 Summary: A python wrapper for Ansys Mechanical
 Author-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Maintainer-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Requires-Python: >=3.7,<4.0
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -12,50 +12,51 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Dist: ansys_api_mechanical==0.1.0
-Requires-Dist: ansys-pythonnet==3.1.0rc1
+Requires-Dist: ansys-pythonnet>=3.1.0rc1
+Requires-Dist: ansys-tools-path>=0.2.3
 Requires-Dist: importlib-metadata>=4.0
 Requires-Dist: appdirs>=1.4.0
 Requires-Dist: grpcio>=1.30.0
 Requires-Dist: protobuf>=3.12.2,<3.21.0
 Requires-Dist: ansys-platform-instancemanagement>=1.0.1
 Requires-Dist: tqdm>=4.45.0
-Requires-Dist: Sphinx==6.2.0 ; extra == "doc"
-Requires-Dist: ansys-sphinx-theme==0.9.8 ; extra == "doc"
-Requires-Dist: grpcio==1.54.0 ; extra == "doc"
+Requires-Dist: Sphinx==6.2.1 ; extra == "doc"
+Requires-Dist: ansys-sphinx-theme==0.9.9 ; extra == "doc"
+Requires-Dist: grpcio==1.54.2 ; extra == "doc"
 Requires-Dist: imageio-ffmpeg==0.4.8 ; extra == "doc"
-Requires-Dist: imageio==2.28.1 ; extra == "doc"
+Requires-Dist: imageio==2.31.1 ; extra == "doc"
 Requires-Dist: jupyter_sphinx==0.4.0 ; extra == "doc"
 Requires-Dist: jupyterlab>=3.2.8 ; extra == "doc"
 Requires-Dist: matplotlib==3.7.1 ; extra == "doc"
 Requires-Dist: numpydoc==1.5.0 ; extra == "doc"
-Requires-Dist: plotly==5.14.1 ; extra == "doc"
+Requires-Dist: plotly==5.15.0 ; extra == "doc"
 Requires-Dist: pypandoc==1.11 ; extra == "doc"
 Requires-Dist: pytest-sphinx==0.5.0 ; extra == "doc"
 Requires-Dist: pythreejs==2.4.2 ; extra == "doc"
-Requires-Dist: pyvista==0.39.0 ; extra == "doc"
+Requires-Dist: pyvista==0.39.1 ; extra == "doc"
 Requires-Dist: sphinx-autobuild==2021.3.14 ; extra == "doc"
 Requires-Dist: sphinx-autodoc-typehints==1.23.0 ; extra == "doc"
 Requires-Dist: sphinx-copybutton==0.5.2 ; extra == "doc"
 Requires-Dist: sphinx_design==0.4.1 ; extra == "doc"
 Requires-Dist: sphinx-gallery==0.13.0 ; extra == "doc"
 Requires-Dist: sphinx-notfound-page==0.8.3 ; extra == "doc"
 Requires-Dist: sphinxcontrib-websupport==1.2.4 ; extra == "doc"
 Requires-Dist: sphinxemoji==0.2.0 ; extra == "doc"
-Requires-Dist: pytest==7.3.1 ; extra == "tests"
-Requires-Dist: pytest-cov==4.0.0 ; extra == "tests"
+Requires-Dist: pytest==7.3.2 ; extra == "tests"
+Requires-Dist: pytest-cov==4.1.0 ; extra == "tests"
 Requires-Dist: pytest-print==0.3.1 ; extra == "tests"
 Project-URL: Documentation, https://mechanical.docs.pyansys.com
-Project-URL: Homepage, https://github.com/pyansys/pymechanical
-Project-URL: Source, https://github.com/pyansys/pymechanical
-Project-URL: Tracker, https://github.com/pyansys/pymechanical/issues
+Project-URL: Homepage, https://github.com/ansys/pymechanical
+Project-URL: Source, https://github.com/ansys/pymechanical
+Project-URL: Tracker, https://github.com/ansys/pymechanical/issues
 Provides-Extra: doc
 Provides-Extra: tests
 
 PyMechanical
 ============
 |pyansys| |python| |pypi| |GH-CI| |codecov| |MIT| |black|
 
@@ -67,20 +68,20 @@
    :target: https://pypi.org/project/ansys-mechanical-core
    :alt: Python
 
 .. |pypi| image:: https://img.shields.io/pypi/v/ansys-mechanical-core.svg?logo=python&logoColor=white
    :target: https://pypi.org/project/ansys-mechanical-core
    :alt: PyPI
 
-.. |codecov| image:: https://codecov.io/gh/pyansys/pymechanical/branch/main/graph/badge.svg
-   :target: https://codecov.io/gh/pyansys/ansys-mechanical-core
+.. |codecov| image:: https://codecov.io/gh/ansys/pymechanical/branch/main/graph/badge.svg
+   :target: https://codecov.io/gh/ansys/ansys-mechanical-core
    :alt: Codecov
 
-.. |GH-CI| image:: https://github.com/pyansys/pymechanical/actions/workflows/ci_cd.yml/badge.svg
-   :target: https://github.com/pyansys/pymechanical/actions/workflows/ci_cd.yml
+.. |GH-CI| image:: https://github.com/ansys/pymechanical/actions/workflows/ci_cd.yml/badge.svg
+   :target: https://github.com/ansys/pymechanical/actions/workflows/ci_cd.yml
    :alt: GH-CI
 
 .. |MIT| image:: https://img.shields.io/badge/License-MIT-yellow.svg
    :target: https://opensource.org/licenses/MIT
    :alt: MIT
 
 .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg?style=flat
```

