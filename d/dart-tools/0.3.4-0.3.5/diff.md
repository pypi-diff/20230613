# Comparing `tmp/dart-tools-0.3.4.tar.gz` & `tmp/dart-tools-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dart-tools-0.3.4.tar", last modified: Sat Jun  3 17:38:16 2023, max compression
+gzip compressed data, was "dart-tools-0.3.5.tar", last modified: Mon Jun 12 01:37:30 2023, max compression
```

## Comparing `dart-tools-0.3.4.tar` & `dart-tools-0.3.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 zack       (501) staff       (20)        0 2023-06-03 17:38:16.996176 dart-tools-0.3.4/
--rw-r--r--   0 zack       (501) staff       (20)     1061 2023-02-28 02:56:19.000000 dart-tools-0.3.4/LICENSE
--rw-r--r--   0 zack       (501) staff       (20)     4358 2023-06-03 17:38:16.995762 dart-tools-0.3.4/PKG-INFO
--rw-r--r--   0 zack       (501) staff       (20)     1510 2023-04-03 00:03:57.000000 dart-tools-0.3.4/README.md
-drwxr-xr-x   0 zack       (501) staff       (20)        0 2023-06-03 17:38:16.989977 dart-tools-0.3.4/dart/
--rw-r--r--   0 zack       (501) staff       (20)       64 2023-02-28 04:01:58.000000 dart-tools-0.3.4/dart/__init__.py
--rwxr-xr-x   0 zack       (501) staff       (20)    12986 2023-06-03 17:35:56.000000 dart-tools-0.3.4/dart/dart.py
--rw-r--r--   0 zack       (501) staff       (20)     1709 2023-02-28 02:57:20.000000 dart-tools-0.3.4/dart/order_manager.py
-drwxr-xr-x   0 zack       (501) staff       (20)        0 2023-06-03 17:38:16.994329 dart-tools-0.3.4/dart_tools.egg-info/
--rw-r--r--   0 zack       (501) staff       (20)     4358 2023-06-03 17:38:16.000000 dart-tools-0.3.4/dart_tools.egg-info/PKG-INFO
--rw-r--r--   0 zack       (501) staff       (20)      339 2023-06-03 17:38:16.000000 dart-tools-0.3.4/dart_tools.egg-info/SOURCES.txt
--rw-r--r--   0 zack       (501) staff       (20)        1 2023-06-03 17:38:16.000000 dart-tools-0.3.4/dart_tools.egg-info/dependency_links.txt
-drwxr-xr-x   0 zack       (501) staff       (20)        0 2023-06-03 17:38:16.994825 dart-tools-0.3.4/dart_tools.egg-info/dist/
--rw-r--r--   0 zack       (501) staff       (20)     8788 2023-06-03 08:11:34.000000 dart-tools-0.3.4/dart_tools.egg-info/dist/dart-tools-0.3.3.tar.gz
--rw-r--r--   0 zack       (501) staff       (20)       34 2023-06-03 17:38:16.000000 dart-tools-0.3.4/dart_tools.egg-info/entry_points.txt
--rw-r--r--   0 zack       (501) staff       (20)       14 2023-06-03 17:38:16.000000 dart-tools-0.3.4/dart_tools.egg-info/requires.txt
--rw-r--r--   0 zack       (501) staff       (20)        5 2023-06-03 17:38:16.000000 dart-tools-0.3.4/dart_tools.egg-info/top_level.txt
--rw-r--r--   0 zack       (501) staff       (20)     1744 2023-06-03 17:36:01.000000 dart-tools-0.3.4/pyproject.toml
--rw-r--r--   0 zack       (501) staff       (20)       38 2023-06-03 17:38:16.996348 dart-tools-0.3.4/setup.cfg
+drwxr-xr-x   0 zack       (501) staff       (20)        0 2023-06-12 01:37:30.086641 dart-tools-0.3.5/
+-rw-r--r--   0 zack       (501) staff       (20)     1061 2023-02-28 02:56:19.000000 dart-tools-0.3.5/LICENSE
+-rw-r--r--   0 zack       (501) staff       (20)     4358 2023-06-12 01:37:30.086305 dart-tools-0.3.5/PKG-INFO
+-rw-r--r--   0 zack       (501) staff       (20)     1510 2023-04-03 00:03:57.000000 dart-tools-0.3.5/README.md
+drwxr-xr-x   0 zack       (501) staff       (20)        0 2023-06-12 01:37:30.081148 dart-tools-0.3.5/dart/
+-rw-r--r--   0 zack       (501) staff       (20)       64 2023-02-28 04:01:58.000000 dart-tools-0.3.5/dart/__init__.py
+-rwxr-xr-x   0 zack       (501) staff       (20)    13136 2023-06-12 01:35:43.000000 dart-tools-0.3.5/dart/dart.py
+-rw-r--r--   0 zack       (501) staff       (20)     1709 2023-02-28 02:57:20.000000 dart-tools-0.3.5/dart/order_manager.py
+drwxr-xr-x   0 zack       (501) staff       (20)        0 2023-06-12 01:37:30.084794 dart-tools-0.3.5/dart_tools.egg-info/
+-rw-r--r--   0 zack       (501) staff       (20)     4358 2023-06-12 01:37:29.000000 dart-tools-0.3.5/dart_tools.egg-info/PKG-INFO
+-rw-r--r--   0 zack       (501) staff       (20)      339 2023-06-12 01:37:29.000000 dart-tools-0.3.5/dart_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 zack       (501) staff       (20)        1 2023-06-12 01:37:29.000000 dart-tools-0.3.5/dart_tools.egg-info/dependency_links.txt
+drwxr-xr-x   0 zack       (501) staff       (20)        0 2023-06-12 01:37:30.085442 dart-tools-0.3.5/dart_tools.egg-info/dist/
+-rw-r--r--   0 zack       (501) staff       (20)     8788 2023-06-03 08:11:34.000000 dart-tools-0.3.5/dart_tools.egg-info/dist/dart-tools-0.3.3.tar.gz
+-rw-r--r--   0 zack       (501) staff       (20)       34 2023-06-12 01:37:29.000000 dart-tools-0.3.5/dart_tools.egg-info/entry_points.txt
+-rw-r--r--   0 zack       (501) staff       (20)       14 2023-06-12 01:37:29.000000 dart-tools-0.3.5/dart_tools.egg-info/requires.txt
+-rw-r--r--   0 zack       (501) staff       (20)        5 2023-06-12 01:37:29.000000 dart-tools-0.3.5/dart_tools.egg-info/top_level.txt
+-rw-r--r--   0 zack       (501) staff       (20)     1744 2023-06-12 01:05:15.000000 dart-tools-0.3.5/pyproject.toml
+-rw-r--r--   0 zack       (501) staff       (20)       38 2023-06-12 01:37:30.086758 dart-tools-0.3.5/setup.cfg
```

### Comparing `dart-tools-0.3.4/LICENSE` & `dart-tools-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dart-tools-0.3.4/PKG-INFO` & `dart-tools-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dart-tools
-Version: 0.3.4
+Version: 0.3.5
 Summary: The Dart CLI and Python Library
 Author-email: Dart Software Team <software@itsdart.com>
 License: MIT License
         
         Copyright (c) 2023 Dart
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dart-tools Version: 0.3.4 Summary: The Dart CLI and
+Metadata-Version: 2.1 Name: dart-tools Version: 0.3.5 Summary: The Dart CLI and
 Python Library Author-email: Dart Software Team
 itsdart.com> License: MIT License Copyright (c) 2023 Dart Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
```

### Comparing `dart-tools-0.3.4/README.md` & `dart-tools-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `dart-tools-0.3.4/dart/dart.py` & `dart-tools-0.3.5/dart/dart.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from collections import defaultdict
 from getpass import getpass
 from importlib.metadata import version
 import json
 import os
 import random
 import re
+import signal
 import string
 import subprocess
 import sys
 
 from pick import pick
 import requests
 
@@ -81,14 +82,18 @@
     return subprocess.check_output(cmd, shell=True).decode()
 
 
 def _get_task_url(host, duid):
     return f"{host}/search?t={duid}"
 
 
+def _exit_gracefully(_signal_received, _frame) -> None:
+    sys.exit("Quitting.")
+
+
 class _Config:
     def __init__(self):
         self._content = {}
         if os.path.isfile(_CONFIG_FPATH):
             with open(_CONFIG_FPATH, "r", encoding="UTF-8") as fin:
                 self._content = json.load(fin)
         self._content = {
@@ -385,14 +390,16 @@
     if should_begin:
         _begin_task(config, session, user["email"], lambda: task)
 
     print("Done.")
 
 
 def cli():
+    signal.signal(signal.SIGINT, _exit_gracefully)
+
     if _VERSION_CMD in sys.argv:
         print_version()
         sys.exit(0)
 
     parser = argparse.ArgumentParser(
         prog="dart", description="A CLI to interact with Dart"
     )
```

### Comparing `dart-tools-0.3.4/dart/order_manager.py` & `dart-tools-0.3.5/dart/order_manager.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.3.4/dart_tools.egg-info/PKG-INFO` & `dart-tools-0.3.5/dart_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dart-tools
-Version: 0.3.4
+Version: 0.3.5
 Summary: The Dart CLI and Python Library
 Author-email: Dart Software Team <software@itsdart.com>
 License: MIT License
         
         Copyright (c) 2023 Dart
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dart-tools Version: 0.3.4 Summary: The Dart CLI and
+Metadata-Version: 2.1 Name: dart-tools Version: 0.3.5 Summary: The Dart CLI and
 Python Library Author-email: Dart Software Team
 itsdart.com> License: MIT License Copyright (c) 2023 Dart Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
```

### Comparing `dart-tools-0.3.4/dart_tools.egg-info/dist/dart-tools-0.3.3.tar.gz` & `dart-tools-0.3.5/dart_tools.egg-info/dist/dart-tools-0.3.3.tar.gz`

 * *Files identical despite different names*

### Comparing `dart-tools-0.3.4/pyproject.toml` & `dart-tools-0.3.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dart-tools"
-version = "0.3.4"
+version = "0.3.5"
 description = "The Dart CLI and Python Library"
 readme = "README.md"
 requires-python = ">=3.8"
 
 license = {file = "LICENSE"}
 keywords = ["dart", "cli", "projectmanagement", "taskmanagement"]
 authors = [
```

