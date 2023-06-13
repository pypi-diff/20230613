# Comparing `tmp/Apppath-1.0.1.tar.gz` & `tmp/Apppath-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Apppath-1.0.1.tar", last modified: Wed Apr 19 11:01:56 2023, max compression
+gzip compressed data, was "Apppath-1.0.2.tar", last modified: Tue Jun 13 10:24:32 2023, max compression
```

## Comparing `Apppath-1.0.1.tar` & `Apppath-1.0.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:01:56.182758 Apppath-1.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:01:56.182758 Apppath-1.0.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 11:01:51.000000 Apppath-1.0.1/.github/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:01:56.182758 Apppath-1.0.1/Apppath.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-04-19 11:01:56.000000 Apppath-1.0.1/Apppath.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-19 11:01:56.000000 Apppath-1.0.1/Apppath.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 11:01:56.000000 Apppath-1.0.1/Apppath.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-19 11:01:56.000000 Apppath-1.0.1/Apppath.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-19 11:01:56.000000 Apppath-1.0.1/Apppath.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-19 11:01:56.000000 Apppath-1.0.1/Apppath.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-19 11:01:51.000000 Apppath-1.0.1/KEYWORDS.md
--rw-r--r--   0 runner    (1001) docker     (123)    10644 2023-04-19 11:01:51.000000 Apppath-1.0.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-19 11:01:51.000000 Apppath-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-04-19 11:01:56.182758 Apppath-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-04-19 11:01:51.000000 Apppath-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-04-19 11:01:51.000000 Apppath-1.0.1/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:01:56.182758 Apppath-1.0.1/apppath/
--rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-04-19 11:01:51.000000 Apppath-1.0.1/apppath/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34204 2023-04-19 11:01:51.000000 Apppath-1.0.1/apppath/app_path.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:01:56.182758 Apppath-1.0.1/apppath/entry_points/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-19 11:01:51.000000 Apppath-1.0.1/apppath/entry_points/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-04-19 11:01:51.000000 Apppath-1.0.1/apppath/entry_points/clean_apppath.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-19 11:01:51.000000 Apppath-1.0.1/apppath/entry_points/open_apppath.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-04-19 11:01:51.000000 Apppath-1.0.1/apppath/system_open_path_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-04-19 11:01:51.000000 Apppath-1.0.1/apppath/windows_path_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:01:56.182758 Apppath-1.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-19 11:01:51.000000 Apppath-1.0.1/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-04-19 11:01:51.000000 Apppath-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-19 11:01:51.000000 Apppath-1.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-19 11:01:56.186758 Apppath-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-04-19 11:01:51.000000 Apppath-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:01:56.182758 Apppath-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-04-19 11:01:51.000000 Apppath-1.0.1/tests/test_app_path.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-19 11:01:51.000000 Apppath-1.0.1/tests/test_imports.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-19 11:01:51.000000 Apppath-1.0.1/tests/test_sanity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:24:32.457472 Apppath-1.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:24:32.453472 Apppath-1.0.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 10:24:24.000000 Apppath-1.0.2/.github/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:24:32.453472 Apppath-1.0.2/Apppath.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-06-13 10:24:32.000000 Apppath-1.0.2/Apppath.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-13 10:24:32.000000 Apppath-1.0.2/Apppath.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 10:24:32.000000 Apppath-1.0.2/Apppath.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-13 10:24:32.000000 Apppath-1.0.2/Apppath.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-13 10:24:32.000000 Apppath-1.0.2/Apppath.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-13 10:24:32.000000 Apppath-1.0.2/Apppath.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-13 10:24:24.000000 Apppath-1.0.2/KEYWORDS.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10644 2023-06-13 10:24:24.000000 Apppath-1.0.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-06-13 10:24:24.000000 Apppath-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-06-13 10:24:32.457472 Apppath-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-06-13 10:24:24.000000 Apppath-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-13 10:24:24.000000 Apppath-1.0.2/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:24:32.453472 Apppath-1.0.2/apppath/
+-rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-06-13 10:24:24.000000 Apppath-1.0.2/apppath/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34504 2023-06-13 10:24:24.000000 Apppath-1.0.2/apppath/app_path.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:24:32.453472 Apppath-1.0.2/apppath/entry_points/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-13 10:24:24.000000 Apppath-1.0.2/apppath/entry_points/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-13 10:24:24.000000 Apppath-1.0.2/apppath/entry_points/clean_apppath.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-13 10:24:24.000000 Apppath-1.0.2/apppath/entry_points/open_apppath.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-06-13 10:24:24.000000 Apppath-1.0.2/apppath/system_open_path_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-06-13 10:24:24.000000 Apppath-1.0.2/apppath/windows_path_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:24:32.453472 Apppath-1.0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-13 10:24:24.000000 Apppath-1.0.2/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-06-13 10:24:24.000000 Apppath-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-13 10:24:24.000000 Apppath-1.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-13 10:24:32.457472 Apppath-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-06-13 10:24:24.000000 Apppath-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:24:32.457472 Apppath-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-06-13 10:24:24.000000 Apppath-1.0.2/tests/test_app_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-13 10:24:24.000000 Apppath-1.0.2/tests/test_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-13 10:24:24.000000 Apppath-1.0.2/tests/test_sanity.py
```

### Comparing `Apppath-1.0.1/Apppath.egg-info/PKG-INFO` & `Apppath-1.0.2/Apppath.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Apppath
-Version: 1.0.1
+Version: 1.0.2
 Summary: A package for easing return of multiple values
 Home-page: https://github.com/pything/apppath
 Download-URL: https://github.com/pything/apppath/releases
 Author: Christian Heider Nielsen
 Author-email: christian.heider@alexandra.dk
 Maintainer: Christian Heider Nielsen
 Maintainer-email: christian.heider@alexandra.dk
@@ -20,17 +20,17 @@
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Natural Language :: English
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: docs
+Provides-Extra: setup
 Provides-Extra: dev
 Provides-Extra: tests
-Provides-Extra: setup
 Provides-Extra: all
 License-File: LICENSE.md
 
 <!--![apppath](.github/images/apppath.svg)-->
 
 <p align="center">
   <img src=".github/images/apppath.svg" alt='AppPath' />
```

### Comparing `Apppath-1.0.1/Apppath.egg-info/SOURCES.txt` & `Apppath-1.0.2/Apppath.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Apppath-1.0.1/LICENSE.md` & `Apppath-1.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Apppath-1.0.1/PKG-INFO` & `Apppath-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Apppath
-Version: 1.0.1
+Version: 1.0.2
 Summary: A package for easing return of multiple values
 Home-page: https://github.com/pything/apppath
 Download-URL: https://github.com/pything/apppath/releases
 Author: Christian Heider Nielsen
 Author-email: christian.heider@alexandra.dk
 Maintainer: Christian Heider Nielsen
 Maintainer-email: christian.heider@alexandra.dk
@@ -20,17 +20,17 @@
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Natural Language :: English
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: docs
+Provides-Extra: setup
 Provides-Extra: dev
 Provides-Extra: tests
-Provides-Extra: setup
 Provides-Extra: all
 License-File: LICENSE.md
 
 <!--![apppath](.github/images/apppath.svg)-->
 
 <p align="center">
   <img src=".github/images/apppath.svg" alt='AppPath' />
```

### Comparing `Apppath-1.0.1/README.md` & `Apppath-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `Apppath-1.0.1/SECURITY.md` & `Apppath-1.0.2/SECURITY.md`

 * *Files identical despite different names*

### Comparing `Apppath-1.0.1/apppath/__init__.py` & `Apppath-1.0.2/apppath/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os
 from warnings import warn
 
 import pkg_resources
 
 __project__ = "Apppath"
 __author__ = "Christian Heider Nielsen"
-__version__ = "1.0.1"
+__version__ = "1.0.2"
 __doc__ = r"""
 Created on 27/04/2019
 
 A class and a set of functions for providing for system-consensual path for apps to store data, logs, cache...
 
 @author: cnheider
 """
```

### Comparing `Apppath-1.0.1/apppath/app_path.py` & `Apppath-1.0.2/apppath/app_path.py`

 * *Files 2% similar despite different names*

```diff
@@ -208,75 +208,75 @@
     @property
     def root_cache(self) -> Path:
         """description
 
         :return:
         """
         if get_system() != SystemEnum.linux:
-            raise SystemError("Invalid system")
+            raise SystemError(f"Invalid system: {get_system()}\n Expected {SystemEnum.linux}")
         return ensure_existence(Path("/var/cache") / self._app_name, enabled=self._ensure_existence)
 
     @property
     def root_config(self) -> Path:
         """description
 
         :return:
         """
         if get_system() != SystemEnum.linux:
-            raise SystemError("Invalid system")
+            raise SystemError(f"Invalid system: {get_system()}\n Expected {SystemEnum.linux}")
         return ensure_existence(Path("/etc") / self._app_name, enabled=self._ensure_existence)
 
     @property
     def root_log(self) -> Path:
         """description
 
         :return:
         """
         if get_system() != SystemEnum.linux:
-            raise SystemError("Invalid system")
+            raise SystemError(f"Invalid system: {get_system()}\n Expected {SystemEnum.linux}")
         return ensure_existence(Path("/var/log") / self._app_name, enabled=self._ensure_existence)
 
     @property
     def root_state(self) -> Path:
         """description
 
         :return:
         """
         if get_system() != SystemEnum.linux:
-            raise SystemError("Invalid system")
+            raise SystemError(f"Invalid system: {get_system()}\n Expected {SystemEnum.linux}")
         return ensure_existence(Path("/var/lib") / self._app_name, enabled=self._ensure_existence)
 
     @property
     def root_run(self) -> Path:
         """description
 
         :return:
         """
         if get_system() != SystemEnum.linux:
-            raise SystemError("Invalid system")
+            raise SystemError(f"Invalid system: {get_system()}\n Expected {SystemEnum.linux}")
         return ensure_existence(Path("/run") / self._app_name, enabled=self._ensure_existence)
 
     @property
     def root_tmp(self) -> Path:
         """description
 
         :return:
         """
         if get_system() != SystemEnum.linux:
-            raise SystemError("Invalid system")
+            raise SystemError(f"Invalid system: {get_system()}\n Expected {SystemEnum.linux}")
         return ensure_existence(Path("/tmp") / self._app_name, enabled=self._ensure_existence)
 
     @property
     def root_long_tmp(self) -> Path:
         """description
 
         :return:
         """
         if get_system() != SystemEnum.linux:
-            raise SystemError("Invalid system")
+            raise SystemError(f"Invalid system: {get_system()}\n Expected {SystemEnum.linux}")
         return ensure_existence(Path("/var/tmp") / self._app_name, enabled=self._ensure_existence)
 
     @property
     def site_cache(self) -> Path:
         """
         TODO: Nonsense, is same as user_cache
         Returns:
@@ -388,16 +388,14 @@
             path_ = Path.home() / "Library" / "Application Support"
 
         elif get_system() == SystemEnum.linux:
             path_ = Path(os.getenv("XDG_DATA_HOME", Path.home() / ".local" / "share"))
         else:
             raise SystemError(f"Invalid system {get_system()}")
 
-        print(get_system())
-
         if app_author:
             path_ = path_ / app_author
         if app_name:
             path_ /= app_name
         if app_name and version:
             path_ /= version
         return path_
```

### Comparing `Apppath-1.0.1/apppath/entry_points/clean_apppath.py` & `Apppath-1.0.2/apppath/entry_points/clean_apppath.py`

 * *Files identical despite different names*

### Comparing `Apppath-1.0.1/apppath/entry_points/open_apppath.py` & `Apppath-1.0.2/apppath/entry_points/open_apppath.py`

 * *Files identical despite different names*

### Comparing `Apppath-1.0.1/apppath/system_open_path_utilities.py` & `Apppath-1.0.2/apppath/system_open_path_utilities.py`

 * *Files identical despite different names*

### Comparing `Apppath-1.0.1/apppath/windows_path_utilities.py` & `Apppath-1.0.2/apppath/windows_path_utilities.py`

 * *Files 0% similar despite different names*

```diff
@@ -124,15 +124,14 @@
             ddir = jna.Native.toString(buf.tostring()).rstrip("\0")
 
     return ddir
 
 
 get_win_folder = None
 
-
 if SYSTEM_ == "win32":  # IMPORT TESTS
     try:
         from win32com import shell
 
         get_win_folder = _get_win_folder_with_pywin32
     except ImportError:
         try:
```

### Comparing `Apppath-1.0.1/pyproject.toml` & `Apppath-1.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `Apppath-1.0.1/setup.py` & `Apppath-1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `Apppath-1.0.1/tests/test_app_path.py` & `Apppath-1.0.2/tests/test_app_path.py`

 * *Files identical despite different names*

