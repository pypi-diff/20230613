# Comparing `tmp/memimport-0.13.0.0.post6.tar.gz` & `tmp/memimport-0.13.0.0.post7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "memimport-0.13.0.0.post6.tar", last modified: Sun Jun 11 01:30:55 2023, max compression
+gzip compressed data, was "memimport-0.13.0.0.post7.tar", last modified: Tue Jun 13 05:00:25 2023, max compression
```

## Comparing `memimport-0.13.0.0.post6.tar` & `memimport-0.13.0.0.post7.tar`

### file list

```diff
@@ -1,26 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 01:30:55.217791 memimport-0.13.0.0.post6/
--rw-rw-rw-   0        0        0    18174 2023-01-06 16:49:46.000000 memimport-0.13.0.0.post6/LICENSE.txt
--rw-rw-rw-   0        0        0      120 2023-01-06 14:20:55.000000 memimport-0.13.0.0.post6/MANIFEST.in
--rw-rw-rw-   0        0        0     1138 2023-01-06 16:55:29.000000 memimport-0.13.0.0.post6/MIT-License.txt
--rw-rw-rw-   0        0        0    16726 2023-01-01 12:50:56.000000 memimport-0.13.0.0.post6/MPL2-License.txt
--rw-rw-rw-   0        0        0     4472 2023-06-11 01:30:55.217791 memimport-0.13.0.0.post6/PKG-INFO
--rw-rw-rw-   0        0        0     2818 2023-01-08 13:33:36.000000 memimport-0.13.0.0.post6/README.md
--rw-rw-rw-   0        0        0      803 2023-01-08 15:53:45.000000 memimport-0.13.0.0.post6/fixupver.py
-drwxrwxrwx   0        0        0        0 2023-06-11 01:30:55.088791 memimport-0.13.0.0.post6/memimport.egg-info/
--rw-rw-rw-   0        0        0     4472 2023-06-11 01:30:54.000000 memimport-0.13.0.0.post6/memimport.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      402 2023-06-11 01:30:54.000000 memimport-0.13.0.0.post6/memimport.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 01:30:54.000000 memimport-0.13.0.0.post6/memimport.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-06-11 01:30:54.000000 memimport-0.13.0.0.post6/memimport.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5481 2023-06-11 01:13:58.000000 memimport-0.13.0.0.post6/memimport.py
--rw-rw-rw-   0        0        0       42 2023-06-11 01:30:55.218791 memimport-0.13.0.0.post6/setup.cfg
--rw-rw-rw-   0        0        0     3392 2023-01-06 13:17:39.000000 memimport-0.13.0.0.post6/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-11 01:30:55.202791 memimport-0.13.0.0.post6/source/
--rw-rw-rw-   0        0        0    39766 2022-12-22 12:56:19.000000 memimport-0.13.0.0.post6/source/MemoryModule.c
--rw-rw-rw-   0        0        0     4751 2023-01-01 12:53:09.000000 memimport-0.13.0.0.post6/source/MemoryModule.h
--rw-rw-rw-   0        0        0     6606 2023-01-01 12:53:14.000000 memimport-0.13.0.0.post6/source/MyLoadLibrary.c
--rw-rw-rw-   0        0        0      233 2023-01-01 12:53:19.000000 memimport-0.13.0.0.post6/source/MyLoadLibrary.h
--rw-rw-rw-   0        0        0     7499 2023-01-06 14:31:10.000000 memimport-0.13.0.0.post6/source/_memimporter.c
--rw-rw-rw-   0        0        0     1506 2023-01-01 12:52:54.000000 memimport-0.13.0.0.post6/source/actctx.c
--rw-rw-rw-   0        0        0     1579 2023-01-01 12:52:59.000000 memimport-0.13.0.0.post6/source/actctx.h
--rw-rw-rw-   0        0        0     2502 2023-01-09 14:52:22.000000 memimport-0.13.0.0.post6/test.py
--rw-rw-rw-   0        0        0    13052 2023-06-10 23:57:59.000000 memimport-0.13.0.0.post6/zipextimporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:00:25.669319 memimport-0.13.0.0.post7/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-13 05:00:22.000000 memimport-0.13.0.0.post7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-13 05:00:22.000000 memimport-0.13.0.0.post7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-13 05:00:22.000000 memimport-0.13.0.0.post7/MIT-License.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    16726 2023-06-13 05:00:22.000000 memimport-0.13.0.0.post7/MPL2-License.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-06-13 05:00:25.669319 memimport-0.13.0.0.post7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-06-13 05:00:22.000000 memimport-0.13.0.0.post7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-06-13 05:00:22.000000 memimport-0.13.0.0.post7/README_py2exe.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7162 2023-06-13 05:00:22.000000 memimport-0.13.0.0.post7/README_py2exe_ORIGINAL.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-06-13 05:00:22.000000 memimport-0.13.0.0.post7/README_py2exe_fork.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-06-13 05:00:22.000000 memimport-0.13.0.0.post7/TODO_py2exe.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-13 05:00:22.000000 memimport-0.13.0.0.post7/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-13 05:00:22.000000 memimport-0.13.0.0.post7/fixupver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:00:25.669319 memimport-0.13.0.0.post7/memimport.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-06-13 05:00:25.000000 memimport-0.13.0.0.post7/memimport.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-13 05:00:25.000000 memimport-0.13.0.0.post7/memimport.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 05:00:25.000000 memimport-0.13.0.0.post7/memimport.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 05:00:25.000000 memimport-0.13.0.0.post7/memimport.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-06-13 05:00:22.000000 memimport-0.13.0.0.post7/memimport.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 05:00:25.669319 memimport-0.13.0.0.post7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-06-13 05:00:22.000000 memimport-0.13.0.0.post7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:00:25.669319 memimport-0.13.0.0.post7/source/
+-rw-r--r--   0 runner    (1001) docker     (123)    39766 2023-06-13 05:00:22.000000 memimport-0.13.0.0.post7/source/MemoryModule.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-06-13 05:00:22.000000 memimport-0.13.0.0.post7/source/MemoryModule.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6606 2023-06-13 05:00:22.000000 memimport-0.13.0.0.post7/source/MyLoadLibrary.c
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-13 05:00:22.000000 memimport-0.13.0.0.post7/source/MyLoadLibrary.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-06-13 05:00:22.000000 memimport-0.13.0.0.post7/source/_memimporter.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-13 05:00:22.000000 memimport-0.13.0.0.post7/source/actctx.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-06-13 05:00:22.000000 memimport-0.13.0.0.post7/source/actctx.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-06-13 05:00:22.000000 memimport-0.13.0.0.post7/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13065 2023-06-13 05:00:22.000000 memimport-0.13.0.0.post7/zipextimporter.py
```

### Comparing `memimport-0.13.0.0.post6/LICENSE.txt` & `memimport-0.13.0.0.post7/MPL2-License.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,44 +1,7 @@
-The files source/MemoryModule.c and source/MemoryModule.h are licensed
-under the Mozilla Public License Version 2.0,
-see MPL2-License.txt.
-
-All other files are licensed under the MIT/X11 License,
-see MIT-License.txt.
-
-
-==========================================================================
-
-
-MIT/X11 License
-===============
-
-Copyright (c) 2000-2023 Thomas Heller, Mark Hammond, Jimmy Retzlaff,
-Alberto Sottile, SeaHOH
-
-Permission is hereby granted, free of charge, to any person obtaining
-a copy of this software and associated documentation files (the
-"Software"), to deal in the Software without restriction, including
-without limitation the rights to use, copy, modify, merge, publish,
-distribute, sublicense, and/or sell copies of the Software, and to
-permit persons to whom the Software is furnished to do so, subject to
-the following conditions:
-
-The above copyright notice and this permission notice shall be
-included in all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
-EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
-MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
-NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
-LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
-OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
-WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-
-
 Mozilla Public License Version 2.0
 ==================================
 
 1. Definitions
 --------------
 
 1.1. "Contributor"
```

### Comparing `memimport-0.13.0.0.post6/MIT-License.txt` & `memimport-0.13.0.0.post7/MIT-License.txt`

 * *Files identical despite different names*

### Comparing `memimport-0.13.0.0.post6/PKG-INFO` & `memimport-0.13.0.0.post7/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,113 +1,115 @@
-Metadata-Version: 2.1
-Name: memimport
-Version: 0.13.0.0.post6
-Summary: Helps import Python extensions from memory, e.g. extensions from Zip files or Web.
-Home-page: http://github.com/SeaHOH/memimport
-Author: Thomas Heller <theller@ctypes.org>, Alberto Sottile <alby128@gmail.com>
-Maintainer: SeaHOH
-Maintainer-email: seahoh@gmail.com
-License: MIT/X11
-Project-URL: Tracker, http://github.com/SeaHOH/memimport/issues
-Keywords: memory importer zip loader
-Platform: Windows
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
-Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Programming Language :: C
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Topic :: Software Development
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: System :: Software Distribution
-Classifier: Topic :: Utilities
-Requires-Python: >=3.6, <3.12
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-memimport for Python 3
-========================
-
-![operating system](https://img.shields.io/badge/OS-Windows-success)
-[![Python implementation](https://img.shields.io/badge/implementation-CPython-success)](https://www.python.org/downloads/)
-[![Python versions](https://img.shields.io/pypi/pyversions/memimport)](https://www.python.org/downloads/)
-[![licenses](https://img.shields.io/badge/license-MIT_|_MPL2-blue)](https://github.com/SeaHOH/memimport/blob/master/LICENSE.txt)
-![development status](https://img.shields.io/pypi/status/memimport)  
-[![latest tag](https://img.shields.io/github/v/tag/SeaHOH/memimport)](https://github.com/SeaHOH/memimport/tags)
-[![build status](https://img.shields.io/github/actions/workflow/status/SeaHOH/memimport/CI.yml)](https://github.com/SeaHOH/memimport/actions/workflows/CI.yml)
-[![latest version](https://img.shields.io/pypi/v/memimport)](https://pypi.org/project/memimport/)
-[![package format](https://img.shields.io/pypi/format/memimport)](https://pypi.org/project/memimport/#files)
-[![monthly downloads](https://img.shields.io/pypi/dm/memimport)](https://pypi.org/project/memimport/#files)
-
-`memimport` is a part of `py2exe`, which helps import Python extensions from
-memory, e.g. extensions from Zip files or Web.
-
-This repo via CI to build it as Python extensions, beacause the original has
-been built into the py2exe runstubs, only run with script, no REPL.
-
-Development of `memimport` is hosted here: https://github.com/SeaHOH/memimport.  
-Development of `py2exe` is hosted here: https://github.com/py2exe/py2exe.
-
-
-Installation
-------------
-
-    pip install memimport
-
-
-Usage
------
-
-```python
-import zipextimporter
-import sys
-
-sys.path.insert(0, 'path/to/libs.zip')
-```
-
-then
-
-```python
-zipextimporter.install()            # default, prefer `hook=False`, `hook=True` as fallback
-```
-
-or
-
-```python
-zipextimporter.install(hook=False)  # better compatibility, monkey patch `zipimport.zipimporter`
-                                    # equal to empty argument, `hook=True` as fallback
-```
-
-or
-
-```python
-zipextimporter.install(hook=True)   # not recommend, install to `sys.path_hooks`
-```
-
-then
-
-```python
-import ext_mod_in_zip      # now, support __init__.pyd in packages
-
-ext_mod_in_zip             # <module 'ext_mod_in_zip' from 'path\\to\\libs.zip\\ext_mod_in_zip\\__init__.pyd'>
-ext_mod_in_zip.__file__    # 'path\\to\\libs.zip\\ext_mod_in_zip\\__init__.pyd'>
-ext_mod_in_zip.__loader__  # <ZipExtensionImporter object 'path\to\libs.zip\'>
-
-import py_mod_in_zip
-
-py_mod_in_zip              # <module 'py_mod_in_zip' from 'path\\to\\libs.zip\\py_mod_in_zip\\__init__.py'>
-py_mod_in_zip.__file__     # 'path\\to\\libs.zip\\py_mod_in_zip\\__init__.py'>
-py_mod_in_zip.__loader__   # <zipimporter object 'path\to\libs.zip\'>
-```
-
-More usage see source or use help function.
-
-
+Metadata-Version: 2.1
+Name: memimport
+Version: 0.13.0.0.post7
+Summary: Helps import Python extensions from memory, e.g. extensions from Zip files or Web.
+Home-page: http://github.com/SeaHOH/memimport
+Author: Thomas Heller <theller@ctypes.org>, Alberto Sottile <alby128@gmail.com>
+Maintainer: SeaHOH
+Maintainer-email: seahoh@gmail.com
+License: MIT/X11 OR (MPL 2.0)
+Project-URL: Tracker, http://github.com/SeaHOH/memimport/issues
+Keywords: memory importer zip loader
+Platform: Windows
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Programming Language :: C
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: System :: Software Distribution
+Classifier: Topic :: Utilities
+Requires-Python: >=3.6, <3.12
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+License-File: MIT-License.txt
+License-File: MPL2-License.txt
+
+memimport for Python 3
+========================
+
+![operating system](https://img.shields.io/badge/OS-Windows-success)
+[![Python implementation](https://img.shields.io/badge/implementation-CPython-success)](https://www.python.org/downloads/)
+[![Python versions](https://img.shields.io/pypi/pyversions/memimport)](https://www.python.org/downloads/)
+[![licenses](https://img.shields.io/badge/license-MIT_|_MPL2-blue)](https://github.com/SeaHOH/memimport/blob/master/LICENSE.txt)
+![development status](https://img.shields.io/pypi/status/memimport)  
+[![latest tag](https://img.shields.io/github/v/tag/SeaHOH/memimport)](https://github.com/SeaHOH/memimport/tags)
+[![build status](https://img.shields.io/github/actions/workflow/status/SeaHOH/memimport/CI.yml)](https://github.com/SeaHOH/memimport/actions/workflows/CI.yml)
+[![latest version](https://img.shields.io/pypi/v/memimport)](https://pypi.org/project/memimport/)
+[![package format](https://img.shields.io/pypi/format/memimport)](https://pypi.org/project/memimport/#files)
+[![monthly downloads](https://img.shields.io/pypi/dm/memimport)](https://pypi.org/project/memimport/#files)
+
+`memimport` is a part of `py2exe`, which helps import Python extensions from
+memory, e.g. extensions from Zip files or Web.
+
+This repo via CI to build it as Python extensions, beacause the original has
+been built into the py2exe runstubs, only run with script, no REPL.
+
+Development of `memimport` is hosted here: https://github.com/SeaHOH/memimport.  
+Development of `py2exe` is hosted here: https://github.com/py2exe/py2exe.
+
+
+Installation
+------------
+
+    pip install memimport
+
+
+Usage
+-----
+
+```python
+import zipextimporter
+import sys
+
+sys.path.insert(0, 'path/to/libs.zip')
+```
+
+then
+
+```python
+zipextimporter.install()            # default, prefer `hook=False`, `hook=True` as fallback
+```
+
+or
+
+```python
+zipextimporter.install(hook=False)  # better compatibility, monkey patch `zipimport.zipimporter`
+                                    # equal to empty argument, `hook=True` as fallback
+```
+
+or
+
+```python
+zipextimporter.install(hook=True)   # not recommend, install to `sys.path_hooks`
+```
+
+then
+
+```python
+import ext_mod_in_zip      # now, support __init__.pyd in packages
+
+ext_mod_in_zip             # <module 'ext_mod_in_zip' from 'path\\to\\libs.zip\\ext_mod_in_zip\\__init__.pyd'>
+ext_mod_in_zip.__file__    # 'path\\to\\libs.zip\\ext_mod_in_zip\\__init__.pyd'>
+ext_mod_in_zip.__loader__  # <ZipExtensionImporter object 'path\to\libs.zip\'>
+
+import py_mod_in_zip
+
+py_mod_in_zip              # <module 'py_mod_in_zip' from 'path\\to\\libs.zip\\py_mod_in_zip\\__init__.py'>
+py_mod_in_zip.__file__     # 'path\\to\\libs.zip\\py_mod_in_zip\\__init__.py'>
+py_mod_in_zip.__loader__   # <zipimporter object 'path\to\libs.zip\'>
+```
+
+More usage see source or use help function.
+
+
```

### Comparing `memimport-0.13.0.0.post6/README.md` & `memimport-0.13.0.0.post7/README.md`

 * *Files identical despite different names*

### Comparing `memimport-0.13.0.0.post6/fixupver.py` & `memimport-0.13.0.0.post7/fixupver.py`

 * *Files identical despite different names*

### Comparing `memimport-0.13.0.0.post6/memimport.egg-info/PKG-INFO` & `memimport-0.13.0.0.post7/memimport.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,113 +1,115 @@
-Metadata-Version: 2.1
-Name: memimport
-Version: 0.13.0.0.post6
-Summary: Helps import Python extensions from memory, e.g. extensions from Zip files or Web.
-Home-page: http://github.com/SeaHOH/memimport
-Author: Thomas Heller <theller@ctypes.org>, Alberto Sottile <alby128@gmail.com>
-Maintainer: SeaHOH
-Maintainer-email: seahoh@gmail.com
-License: MIT/X11
-Project-URL: Tracker, http://github.com/SeaHOH/memimport/issues
-Keywords: memory importer zip loader
-Platform: Windows
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
-Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Programming Language :: C
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Topic :: Software Development
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: System :: Software Distribution
-Classifier: Topic :: Utilities
-Requires-Python: >=3.6, <3.12
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-memimport for Python 3
-========================
-
-![operating system](https://img.shields.io/badge/OS-Windows-success)
-[![Python implementation](https://img.shields.io/badge/implementation-CPython-success)](https://www.python.org/downloads/)
-[![Python versions](https://img.shields.io/pypi/pyversions/memimport)](https://www.python.org/downloads/)
-[![licenses](https://img.shields.io/badge/license-MIT_|_MPL2-blue)](https://github.com/SeaHOH/memimport/blob/master/LICENSE.txt)
-![development status](https://img.shields.io/pypi/status/memimport)  
-[![latest tag](https://img.shields.io/github/v/tag/SeaHOH/memimport)](https://github.com/SeaHOH/memimport/tags)
-[![build status](https://img.shields.io/github/actions/workflow/status/SeaHOH/memimport/CI.yml)](https://github.com/SeaHOH/memimport/actions/workflows/CI.yml)
-[![latest version](https://img.shields.io/pypi/v/memimport)](https://pypi.org/project/memimport/)
-[![package format](https://img.shields.io/pypi/format/memimport)](https://pypi.org/project/memimport/#files)
-[![monthly downloads](https://img.shields.io/pypi/dm/memimport)](https://pypi.org/project/memimport/#files)
-
-`memimport` is a part of `py2exe`, which helps import Python extensions from
-memory, e.g. extensions from Zip files or Web.
-
-This repo via CI to build it as Python extensions, beacause the original has
-been built into the py2exe runstubs, only run with script, no REPL.
-
-Development of `memimport` is hosted here: https://github.com/SeaHOH/memimport.  
-Development of `py2exe` is hosted here: https://github.com/py2exe/py2exe.
-
-
-Installation
-------------
-
-    pip install memimport
-
-
-Usage
------
-
-```python
-import zipextimporter
-import sys
-
-sys.path.insert(0, 'path/to/libs.zip')
-```
-
-then
-
-```python
-zipextimporter.install()            # default, prefer `hook=False`, `hook=True` as fallback
-```
-
-or
-
-```python
-zipextimporter.install(hook=False)  # better compatibility, monkey patch `zipimport.zipimporter`
-                                    # equal to empty argument, `hook=True` as fallback
-```
-
-or
-
-```python
-zipextimporter.install(hook=True)   # not recommend, install to `sys.path_hooks`
-```
-
-then
-
-```python
-import ext_mod_in_zip      # now, support __init__.pyd in packages
-
-ext_mod_in_zip             # <module 'ext_mod_in_zip' from 'path\\to\\libs.zip\\ext_mod_in_zip\\__init__.pyd'>
-ext_mod_in_zip.__file__    # 'path\\to\\libs.zip\\ext_mod_in_zip\\__init__.pyd'>
-ext_mod_in_zip.__loader__  # <ZipExtensionImporter object 'path\to\libs.zip\'>
-
-import py_mod_in_zip
-
-py_mod_in_zip              # <module 'py_mod_in_zip' from 'path\\to\\libs.zip\\py_mod_in_zip\\__init__.py'>
-py_mod_in_zip.__file__     # 'path\\to\\libs.zip\\py_mod_in_zip\\__init__.py'>
-py_mod_in_zip.__loader__   # <zipimporter object 'path\to\libs.zip\'>
-```
-
-More usage see source or use help function.
-
-
+Metadata-Version: 2.1
+Name: memimport
+Version: 0.13.0.0.post7
+Summary: Helps import Python extensions from memory, e.g. extensions from Zip files or Web.
+Home-page: http://github.com/SeaHOH/memimport
+Author: Thomas Heller <theller@ctypes.org>, Alberto Sottile <alby128@gmail.com>
+Maintainer: SeaHOH
+Maintainer-email: seahoh@gmail.com
+License: MIT/X11 OR (MPL 2.0)
+Project-URL: Tracker, http://github.com/SeaHOH/memimport/issues
+Keywords: memory importer zip loader
+Platform: Windows
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Programming Language :: C
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: System :: Software Distribution
+Classifier: Topic :: Utilities
+Requires-Python: >=3.6, <3.12
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+License-File: MIT-License.txt
+License-File: MPL2-License.txt
+
+memimport for Python 3
+========================
+
+![operating system](https://img.shields.io/badge/OS-Windows-success)
+[![Python implementation](https://img.shields.io/badge/implementation-CPython-success)](https://www.python.org/downloads/)
+[![Python versions](https://img.shields.io/pypi/pyversions/memimport)](https://www.python.org/downloads/)
+[![licenses](https://img.shields.io/badge/license-MIT_|_MPL2-blue)](https://github.com/SeaHOH/memimport/blob/master/LICENSE.txt)
+![development status](https://img.shields.io/pypi/status/memimport)  
+[![latest tag](https://img.shields.io/github/v/tag/SeaHOH/memimport)](https://github.com/SeaHOH/memimport/tags)
+[![build status](https://img.shields.io/github/actions/workflow/status/SeaHOH/memimport/CI.yml)](https://github.com/SeaHOH/memimport/actions/workflows/CI.yml)
+[![latest version](https://img.shields.io/pypi/v/memimport)](https://pypi.org/project/memimport/)
+[![package format](https://img.shields.io/pypi/format/memimport)](https://pypi.org/project/memimport/#files)
+[![monthly downloads](https://img.shields.io/pypi/dm/memimport)](https://pypi.org/project/memimport/#files)
+
+`memimport` is a part of `py2exe`, which helps import Python extensions from
+memory, e.g. extensions from Zip files or Web.
+
+This repo via CI to build it as Python extensions, beacause the original has
+been built into the py2exe runstubs, only run with script, no REPL.
+
+Development of `memimport` is hosted here: https://github.com/SeaHOH/memimport.  
+Development of `py2exe` is hosted here: https://github.com/py2exe/py2exe.
+
+
+Installation
+------------
+
+    pip install memimport
+
+
+Usage
+-----
+
+```python
+import zipextimporter
+import sys
+
+sys.path.insert(0, 'path/to/libs.zip')
+```
+
+then
+
+```python
+zipextimporter.install()            # default, prefer `hook=False`, `hook=True` as fallback
+```
+
+or
+
+```python
+zipextimporter.install(hook=False)  # better compatibility, monkey patch `zipimport.zipimporter`
+                                    # equal to empty argument, `hook=True` as fallback
+```
+
+or
+
+```python
+zipextimporter.install(hook=True)   # not recommend, install to `sys.path_hooks`
+```
+
+then
+
+```python
+import ext_mod_in_zip      # now, support __init__.pyd in packages
+
+ext_mod_in_zip             # <module 'ext_mod_in_zip' from 'path\\to\\libs.zip\\ext_mod_in_zip\\__init__.pyd'>
+ext_mod_in_zip.__file__    # 'path\\to\\libs.zip\\ext_mod_in_zip\\__init__.pyd'>
+ext_mod_in_zip.__loader__  # <ZipExtensionImporter object 'path\to\libs.zip\'>
+
+import py_mod_in_zip
+
+py_mod_in_zip              # <module 'py_mod_in_zip' from 'path\\to\\libs.zip\\py_mod_in_zip\\__init__.py'>
+py_mod_in_zip.__file__     # 'path\\to\\libs.zip\\py_mod_in_zip\\__init__.py'>
+py_mod_in_zip.__loader__   # <zipimporter object 'path\to\libs.zip\'>
+```
+
+More usage see source or use help function.
+
+
```

### Comparing `memimport-0.13.0.0.post6/memimport.py` & `memimport-0.13.0.0.post7/memimport.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,26 +32,23 @@
 'Some error message'
 >>>
 
 '''
 
 import os
 import sys
-try:
-    from _frozen_importlib import ModuleSpec
-    from _frozen_importlib_external import ExtensionFileLoader
-except ImportError:
-    from importlib.machinery import ModuleSpec, ExtensionFileLoader
+from _frozen_importlib import ModuleSpec
+from _frozen_importlib_external import ExtensionFileLoader
 
 # _memimporter is a module built into the py2exe runstubs,
 # or a standalone module of memimport.
 from _memimporter import import_module
 
 
-__version__ = '0.13.0.0.post6'
+__version__ = '0.13.0.0.post7'
 
 __all__ = [
     'memimport_from_data', 'memimport_from_loader', 'memimport_from_spec',
     'memimport', 'set_verbose'
 ]
 
 
@@ -163,11 +160,11 @@
 
 verbose = sys.flags.verbose
 
 def _verbose_msg(msg, verbosity=1):
     if max(verbose, sys.flags.verbose) >= verbosity:
         print(msg, file=sys.stderr)
 
-def set_verbose(i):
+def set_verbose(i=1):
     '''Set verbose, the argument as same as built-in function int's.'''
     global verbose
     verbose = int(i)
```

### Comparing `memimport-0.13.0.0.post6/setup.py` & `memimport-0.13.0.0.post7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,19 +6,21 @@
 import os
 import sys
 import glob
 import platform
 
 from importlib import machinery
 
-if platform.system() != "Windows":
-    raise RuntimeError("This package requires Windows")
+if sys.argv != ['setup.py', 'sdist']:
 
-if sys.version_info < (3, 6):
-    raise RuntimeError("This package requires Python 3.6 or later")
+    if platform.system() != "Windows":
+        raise RuntimeError("This package requires Windows")
+
+    if sys.version_info < (3, 6):
+        raise RuntimeError("This package requires Python 3.6 or later")
 
 ############################################################################
 
 from setuptools import setup
 
 from setuptools.extension import Extension
 
@@ -68,15 +70,20 @@
         author="Thomas Heller <theller@ctypes.org>, Alberto Sottile <alby128@gmail.com>",
         maintainer="SeaHOH",
         maintainer_email="seahoh@gmail.com",
         url="http://github.com/SeaHOH/memimport",
         project_urls={
             "Tracker": "http://github.com/SeaHOH/memimport/issues"
         },
-        license="MIT/X11",
+        license="MIT/X11 OR (MPL 2.0)",
+        license_files=[
+            "LICENSE.txt",
+            "MIT-License.txt",
+            "MPL2-License.txt",
+        ],
         setup_requires=["wheel"],
         platforms="Windows",
         python_requires=">=3.6, <3.12",
 
         classifiers=[
             "Development Status :: 4 - Beta",
             "Environment :: Console",
```

### Comparing `memimport-0.13.0.0.post6/source/MemoryModule.c` & `memimport-0.13.0.0.post7/source/MemoryModule.c`

 * *Files identical despite different names*

### Comparing `memimport-0.13.0.0.post6/source/MemoryModule.h` & `memimport-0.13.0.0.post7/source/MemoryModule.h`

 * *Files identical despite different names*

### Comparing `memimport-0.13.0.0.post6/source/MyLoadLibrary.c` & `memimport-0.13.0.0.post7/source/MyLoadLibrary.c`

 * *Files identical despite different names*

### Comparing `memimport-0.13.0.0.post6/source/_memimporter.c` & `memimport-0.13.0.0.post7/source/_memimporter.c`

 * *Files identical despite different names*

### Comparing `memimport-0.13.0.0.post6/source/actctx.c` & `memimport-0.13.0.0.post7/source/actctx.c`

 * *Files identical despite different names*

### Comparing `memimport-0.13.0.0.post6/source/actctx.h` & `memimport-0.13.0.0.post7/source/actctx.h`

 * *Files identical despite different names*

### Comparing `memimport-0.13.0.0.post6/test.py` & `memimport-0.13.0.0.post7/test.py`

 * *Files identical despite different names*

### Comparing `memimport-0.13.0.0.post6/zipextimporter.py` & `memimport-0.13.0.0.post7/zipextimporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
 import os
 import sys
 from zipimport import *
 from _frozen_importlib import ModuleSpec, spec_from_loader
 from _frozen_importlib_external import ExtensionFileLoader, spec_from_file_location
 
-from memimport import memimport, export_hook_name
+from memimport import memimport, export_hook_name, __version__
 
 
 __all__ = [
     'install', 'set_verbose',
     'set_exclude_modules', 'set_ver_binding_modules',
     'list_exclude_modules', 'list_ver_binding_modules'
 ]
@@ -353,22 +353,22 @@
     _set_importer(modules, _names_pyver.add, f)
 
 
 def _set_importer(modules, attrfunc, argsfunc=None):
     if not isinstance(modules, (list, tuple)):
         modules = [modules]
     for module in modules:
-        if not isinstance((module, str)):
+        if not isinstance(module, str):
             raise ValueError(f'the module name MUST be a str, not {type(module)}')
         attrfunc(argsfunc and argsfunc(module) or module)
 
 
 verbose = sys.flags.verbose
 
 def _verbose_msg(msg, verbosity=1):
     if max(verbose, sys.flags.verbose) >= verbosity:
         print(msg, file=sys.stderr)
 
-def set_verbose(i):
+def set_verbose(i=1):
     '''Set verbose, the argument as same as built-in function int's.'''
     global verbose
     verbose = int(i)
```

