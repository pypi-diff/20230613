# Comparing `tmp/bdpycmd-1.3.6.tar.gz` & `tmp/bdpycmd-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bdpycmd-1.3.6.tar", last modified: Tue Jun 13 16:08:25 2023, max compression
+gzip compressed data, was "bdpycmd-1.3.7.tar", last modified: Tue Jun 13 16:29:23 2023, max compression
```

## Comparing `bdpycmd-1.3.6.tar` & `bdpycmd-1.3.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 16:08:25.078485 bdpycmd-1.3.6/
--rw-r--r--   0 zhicheng   (501) staff       (20)     2618 2023-06-13 16:08:25.078549 bdpycmd-1.3.6/PKG-INFO
--rw-r--r--   0 zhicheng   (501) staff       (20)     1958 2023-06-13 16:06:43.000000 bdpycmd-1.3.6/README.md
--rw-r--r--   0 zhicheng   (501) staff       (20)       80 2022-09-04 10:23:26.000000 bdpycmd-1.3.6/pyproject.toml
--rw-r--r--   0 zhicheng   (501) staff       (20)      784 2023-06-13 16:08:25.078842 bdpycmd-1.3.6/setup.cfg
-drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 16:08:25.076470 bdpycmd-1.3.6/src/
-drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 16:08:25.077212 bdpycmd-1.3.6/src/bdpycmd/
--rw-r--r--   0 zhicheng   (501) staff       (20)        0 2023-06-13 08:19:55.000000 bdpycmd-1.3.6/src/bdpycmd/__init__.py
-drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 16:08:25.077795 bdpycmd-1.3.6/src/bdpycmd/cmd/
--rw-r--r--   0 zhicheng   (501) staff       (20)        0 2023-06-13 16:07:21.000000 bdpycmd-1.3.6/src/bdpycmd/cmd/__init__.py
-drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 16:08:25.077961 bdpycmd-1.3.6/src/bdpycmd/cmd/camp/
--rw-r--r--   0 zhicheng   (501) staff       (20)        0 2023-06-13 16:07:21.000000 bdpycmd-1.3.6/src/bdpycmd/cmd/camp/__init__.py
--rw-r--r--   0 zhicheng   (501) staff       (20)     2560 2023-06-13 16:07:21.000000 bdpycmd-1.3.6/src/bdpycmd/cmd/camp/assistant.py
-drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 16:08:25.078387 bdpycmd-1.3.6/src/bdpycmd/cmd/factory/
--rw-r--r--   0 zhicheng   (501) staff       (20)        0 2023-06-13 16:07:21.000000 bdpycmd-1.3.6/src/bdpycmd/cmd/factory/__init__.py
--rw-r--r--   0 zhicheng   (501) staff       (20)     5764 2023-06-13 16:07:21.000000 bdpycmd-1.3.6/src/bdpycmd/cmd/factory/base.py
--rw-r--r--   0 zhicheng   (501) staff       (20)      975 2023-06-13 16:07:21.000000 bdpycmd-1.3.6/src/bdpycmd/cmd/factory/docmd.py
--rw-r--r--   0 zhicheng   (501) staff       (20)      956 2023-06-13 16:07:21.000000 bdpycmd-1.3.6/src/bdpycmd/cmd/factory/dofunc.py
--rw-r--r--   0 zhicheng   (501) staff       (20)     8331 2023-06-13 16:07:21.000000 bdpycmd-1.3.6/src/bdpycmd/pycmd.py
-drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 16:08:25.077686 bdpycmd-1.3.6/src/bdpycmd.egg-info/
--rw-r--r--   0 zhicheng   (501) staff       (20)     2618 2023-06-13 16:08:25.000000 bdpycmd-1.3.6/src/bdpycmd.egg-info/PKG-INFO
--rw-r--r--   0 zhicheng   (501) staff       (20)      449 2023-06-13 16:08:25.000000 bdpycmd-1.3.6/src/bdpycmd.egg-info/SOURCES.txt
--rw-r--r--   0 zhicheng   (501) staff       (20)        1 2023-06-13 16:08:25.000000 bdpycmd-1.3.6/src/bdpycmd.egg-info/dependency_links.txt
--rw-r--r--   0 zhicheng   (501) staff       (20)        8 2023-06-13 16:08:25.000000 bdpycmd-1.3.6/src/bdpycmd.egg-info/top_level.txt
+drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 16:29:23.282037 bdpycmd-1.3.7/
+-rw-r--r--   0 zhicheng   (501) staff       (20)     2618 2023-06-13 16:29:23.282119 bdpycmd-1.3.7/PKG-INFO
+-rw-r--r--   0 zhicheng   (501) staff       (20)     1958 2023-06-13 16:06:43.000000 bdpycmd-1.3.7/README.md
+-rw-r--r--   0 zhicheng   (501) staff       (20)       80 2022-09-04 10:23:26.000000 bdpycmd-1.3.7/pyproject.toml
+-rw-r--r--   0 zhicheng   (501) staff       (20)      784 2023-06-13 16:29:23.282417 bdpycmd-1.3.7/setup.cfg
+drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 16:29:23.278875 bdpycmd-1.3.7/src/
+drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 16:29:23.279615 bdpycmd-1.3.7/src/bdpycmd/
+-rw-r--r--   0 zhicheng   (501) staff       (20)        0 2023-06-13 08:19:55.000000 bdpycmd-1.3.7/src/bdpycmd/__init__.py
+drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 16:29:23.280682 bdpycmd-1.3.7/src/bdpycmd/cmd/
+-rw-r--r--   0 zhicheng   (501) staff       (20)        0 2023-06-13 16:28:56.000000 bdpycmd-1.3.7/src/bdpycmd/cmd/__init__.py
+drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 16:29:23.280930 bdpycmd-1.3.7/src/bdpycmd/cmd/camp/
+-rw-r--r--   0 zhicheng   (501) staff       (20)        0 2023-06-13 16:28:56.000000 bdpycmd-1.3.7/src/bdpycmd/cmd/camp/__init__.py
+-rw-r--r--   0 zhicheng   (501) staff       (20)     2560 2023-06-13 16:28:56.000000 bdpycmd-1.3.7/src/bdpycmd/cmd/camp/assistant.py
+drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 16:29:23.281875 bdpycmd-1.3.7/src/bdpycmd/cmd/factory/
+-rw-r--r--   0 zhicheng   (501) staff       (20)        0 2023-06-13 16:28:56.000000 bdpycmd-1.3.7/src/bdpycmd/cmd/factory/__init__.py
+-rw-r--r--   0 zhicheng   (501) staff       (20)     5755 2023-06-13 16:28:56.000000 bdpycmd-1.3.7/src/bdpycmd/cmd/factory/base.py
+-rw-r--r--   0 zhicheng   (501) staff       (20)      975 2023-06-13 16:28:56.000000 bdpycmd-1.3.7/src/bdpycmd/cmd/factory/dacmd.py
+-rw-r--r--   0 zhicheng   (501) staff       (20)      956 2023-06-13 16:28:56.000000 bdpycmd-1.3.7/src/bdpycmd/cmd/factory/dafunc.py
+-rw-r--r--   0 zhicheng   (501) staff       (20)     8333 2023-06-13 16:28:56.000000 bdpycmd-1.3.7/src/bdpycmd/pycmd.py
+drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 16:29:23.280560 bdpycmd-1.3.7/src/bdpycmd.egg-info/
+-rw-r--r--   0 zhicheng   (501) staff       (20)     2618 2023-06-13 16:29:23.000000 bdpycmd-1.3.7/src/bdpycmd.egg-info/PKG-INFO
+-rw-r--r--   0 zhicheng   (501) staff       (20)      449 2023-06-13 16:29:23.000000 bdpycmd-1.3.7/src/bdpycmd.egg-info/SOURCES.txt
+-rw-r--r--   0 zhicheng   (501) staff       (20)        1 2023-06-13 16:29:23.000000 bdpycmd-1.3.7/src/bdpycmd.egg-info/dependency_links.txt
+-rw-r--r--   0 zhicheng   (501) staff       (20)        8 2023-06-13 16:29:23.000000 bdpycmd-1.3.7/src/bdpycmd.egg-info/top_level.txt
```

### Comparing `bdpycmd-1.3.6/PKG-INFO` & `bdpycmd-1.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bdpycmd
-Version: 1.3.6
+Version: 1.3.7
 Summary: Run Python`s file as command line
 Home-page: https://github.com/biandoucheng/bd-py-cmd
 Author: biandoucheng
 Author-email: biandoucheng@outlook.com
 Project-URL: Bug Tracker, https://github.com/biandoucheng/bd-py-cmd/issues
 Project-URL: Use Example, https://github.com/biandoucheng/open-example/tree/main/bdpycmd-example
 Classifier: Programming Language :: Python :: 3.5
```

### Comparing `bdpycmd-1.3.6/README.md` & `bdpycmd-1.3.7/README.md`

 * *Files identical despite different names*

### Comparing `bdpycmd-1.3.6/setup.cfg` & `bdpycmd-1.3.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = bdpycmd
-version = 1.3.6
+version = 1.3.7
 author = biandoucheng
 author_email = biandoucheng@outlook.com
 description = Run Python`s file as command line
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/biandoucheng/bd-py-cmd
 project_urls =
```

### Comparing `bdpycmd-1.3.6/src/bdpycmd/cmd/camp/assistant.py` & `bdpycmd-1.3.7/src/bdpycmd/cmd/camp/assistant.py`

 * *Files identical despite different names*

### Comparing `bdpycmd-1.3.6/src/bdpycmd/cmd/factory/base.py` & `bdpycmd-1.3.7/src/bdpycmd/cmd/factory/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import re
 from functools import wraps
 from types import FunctionType
-from .docmd import CmdMeta
-from ..factory.dofunc import MethodMeta
+from .dacmd import CmdMeta
+from .dafunc import MethodMeta
 
 # Command Description Information
 _BDCMD_DESC_ = {
     "name":"base",
     "alias":"command base class",
     "desc":"All commands need to inherit from this base class"
 }
```

### Comparing `bdpycmd-1.3.6/src/bdpycmd/cmd/factory/docmd.py` & `bdpycmd-1.3.7/src/bdpycmd/cmd/factory/dacmd.py`

 * *Files identical despite different names*

### Comparing `bdpycmd-1.3.6/src/bdpycmd/cmd/factory/dofunc.py` & `bdpycmd-1.3.7/src/bdpycmd/cmd/factory/dafunc.py`

 * *Files identical despite different names*

### Comparing `bdpycmd-1.3.6/src/bdpycmd/pycmd.py` & `bdpycmd-1.3.7/src/bdpycmd/pycmd.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import sys,traceback,os
 from types import FunctionType
 from importlib import import_module
-from .cmd.factory.cmd import CmdMeta
+from .cmd.factory.dacmd import CmdMeta
 
 class CmdBaseConf:
     # project root directory
     __PROJECT_ROOT_DIR = os.path.abspath('.')
     # command script saver relative path
     __CMD_DIR = "cmd"
     # command folder, which can only be a child of the root directory
```

### Comparing `bdpycmd-1.3.6/src/bdpycmd.egg-info/PKG-INFO` & `bdpycmd-1.3.7/src/bdpycmd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bdpycmd
-Version: 1.3.6
+Version: 1.3.7
 Summary: Run Python`s file as command line
 Home-page: https://github.com/biandoucheng/bd-py-cmd
 Author: biandoucheng
 Author-email: biandoucheng@outlook.com
 Project-URL: Bug Tracker, https://github.com/biandoucheng/bd-py-cmd/issues
 Project-URL: Use Example, https://github.com/biandoucheng/open-example/tree/main/bdpycmd-example
 Classifier: Programming Language :: Python :: 3.5
```

