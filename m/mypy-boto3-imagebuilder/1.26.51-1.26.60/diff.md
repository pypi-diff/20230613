# Comparing `tmp/mypy-boto3-imagebuilder-1.26.51.tar.gz` & `tmp/mypy-boto3-imagebuilder-1.26.60.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-imagebuilder-1.26.51.tar", last modified: Tue Jan 17 20:24:22 2023, max compression
+gzip compressed data, was "mypy-boto3-imagebuilder-1.26.60.tar", last modified: Mon Jan 30 21:06:23 2023, max compression
```

## Comparing `mypy-boto3-imagebuilder-1.26.51.tar` & `mypy-boto3-imagebuilder-1.26.60.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 20:24:22.375515 mypy-boto3-imagebuilder-1.26.51/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-01-17 20:24:09.000000 mypy-boto3-imagebuilder-1.26.51/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18227 2023-01-17 20:24:22.375515 mypy-boto3-imagebuilder-1.26.51/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16720 2023-01-17 20:24:09.000000 mypy-boto3-imagebuilder-1.26.51/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 20:24:22.371515 mypy-boto3-imagebuilder-1.26.51/mypy_boto3_imagebuilder/
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-01-17 20:24:09.000000 mypy-boto3-imagebuilder-1.26.51/mypy_boto3_imagebuilder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-01-17 20:24:09.000000 mypy-boto3-imagebuilder-1.26.51/mypy_boto3_imagebuilder/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-01-17 20:24:09.000000 mypy-boto3-imagebuilder-1.26.51/mypy_boto3_imagebuilder/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37598 2023-01-17 20:24:09.000000 mypy-boto3-imagebuilder-1.26.51/mypy_boto3_imagebuilder/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    37541 2023-01-17 20:24:09.000000 mypy-boto3-imagebuilder-1.26.51/mypy_boto3_imagebuilder/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8709 2023-01-17 20:24:09.000000 mypy-boto3-imagebuilder-1.26.51/mypy_boto3_imagebuilder/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8707 2023-01-17 20:24:09.000000 mypy-boto3-imagebuilder-1.26.51/mypy_boto3_imagebuilder/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-17 20:24:09.000000 mypy-boto3-imagebuilder-1.26.51/mypy_boto3_imagebuilder/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    54196 2023-01-17 20:24:11.000000 mypy-boto3-imagebuilder-1.26.51/mypy_boto3_imagebuilder/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    54147 2023-01-17 20:24:10.000000 mypy-boto3-imagebuilder-1.26.51/mypy_boto3_imagebuilder/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-17 20:24:09.000000 mypy-boto3-imagebuilder-1.26.51/mypy_boto3_imagebuilder/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 20:24:22.375515 mypy-boto3-imagebuilder-1.26.51/mypy_boto3_imagebuilder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18227 2023-01-17 20:24:22.000000 mypy-boto3-imagebuilder-1.26.51/mypy_boto3_imagebuilder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-01-17 20:24:22.000000 mypy-boto3-imagebuilder-1.26.51/mypy_boto3_imagebuilder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-17 20:24:22.000000 mypy-boto3-imagebuilder-1.26.51/mypy_boto3_imagebuilder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-17 20:24:22.000000 mypy-boto3-imagebuilder-1.26.51/mypy_boto3_imagebuilder.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-17 20:24:22.000000 mypy-boto3-imagebuilder-1.26.51/mypy_boto3_imagebuilder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-01-17 20:24:22.000000 mypy-boto3-imagebuilder-1.26.51/mypy_boto3_imagebuilder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-17 20:24:22.375515 mypy-boto3-imagebuilder-1.26.51/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-01-17 20:24:09.000000 mypy-boto3-imagebuilder-1.26.51/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 21:06:23.446471 mypy-boto3-imagebuilder-1.26.60/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-01-30 21:05:58.000000 mypy-boto3-imagebuilder-1.26.60/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18227 2023-01-30 21:06:23.446471 mypy-boto3-imagebuilder-1.26.60/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16720 2023-01-30 21:05:58.000000 mypy-boto3-imagebuilder-1.26.60/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 21:06:23.446471 mypy-boto3-imagebuilder-1.26.60/mypy_boto3_imagebuilder/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-01-30 21:05:58.000000 mypy-boto3-imagebuilder-1.26.60/mypy_boto3_imagebuilder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-01-30 21:05:58.000000 mypy-boto3-imagebuilder-1.26.60/mypy_boto3_imagebuilder/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-01-30 21:05:58.000000 mypy-boto3-imagebuilder-1.26.60/mypy_boto3_imagebuilder/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37598 2023-01-30 21:05:58.000000 mypy-boto3-imagebuilder-1.26.60/mypy_boto3_imagebuilder/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37541 2023-01-30 21:05:58.000000 mypy-boto3-imagebuilder-1.26.60/mypy_boto3_imagebuilder/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8709 2023-01-30 21:05:58.000000 mypy-boto3-imagebuilder-1.26.60/mypy_boto3_imagebuilder/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8707 2023-01-30 21:05:58.000000 mypy-boto3-imagebuilder-1.26.60/mypy_boto3_imagebuilder/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-30 21:05:58.000000 mypy-boto3-imagebuilder-1.26.60/mypy_boto3_imagebuilder/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    54196 2023-01-30 21:06:00.000000 mypy-boto3-imagebuilder-1.26.60/mypy_boto3_imagebuilder/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54147 2023-01-30 21:06:00.000000 mypy-boto3-imagebuilder-1.26.60/mypy_boto3_imagebuilder/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-30 21:05:58.000000 mypy-boto3-imagebuilder-1.26.60/mypy_boto3_imagebuilder/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 21:06:23.446471 mypy-boto3-imagebuilder-1.26.60/mypy_boto3_imagebuilder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18227 2023-01-30 21:06:23.000000 mypy-boto3-imagebuilder-1.26.60/mypy_boto3_imagebuilder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-01-30 21:06:23.000000 mypy-boto3-imagebuilder-1.26.60/mypy_boto3_imagebuilder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-30 21:06:23.000000 mypy-boto3-imagebuilder-1.26.60/mypy_boto3_imagebuilder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-30 21:06:23.000000 mypy-boto3-imagebuilder-1.26.60/mypy_boto3_imagebuilder.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-30 21:06:23.000000 mypy-boto3-imagebuilder-1.26.60/mypy_boto3_imagebuilder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-01-30 21:06:23.000000 mypy-boto3-imagebuilder-1.26.60/mypy_boto3_imagebuilder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-30 21:06:23.446471 mypy-boto3-imagebuilder-1.26.60/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-01-30 21:05:58.000000 mypy-boto3-imagebuilder-1.26.60/setup.py
```

### Comparing `mypy-boto3-imagebuilder-1.26.51/LICENSE` & `mypy-boto3-imagebuilder-1.26.60/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-imagebuilder-1.26.51/PKG-INFO` & `mypy-boto3-imagebuilder-1.26.60/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-imagebuilder
-Version: 1.26.51
-Summary: Type annotations for boto3.imagebuilder 1.26.51 service generated with mypy-boto3-builder 7.12.3
+Version: 1.26.60
+Summary: Type annotations for boto3.imagebuilder 1.26.60 service generated with mypy-boto3-builder 7.12.3
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_imagebuilder/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-imagebuilder.svg?color=blue)](https://pypi.org/project/mypy-boto3-imagebuilder)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-imagebuilder?color=blue)](https://pypistats.org/packages/mypy-boto3-imagebuilder)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.imagebuilder 1.26.51](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder)
+[boto3.imagebuilder 1.26.60](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-imagebuilder-1.26.51/README.md` & `mypy-boto3-imagebuilder-1.26.60/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-imagebuilder.svg?color=blue)](https://pypi.org/project/mypy-boto3-imagebuilder)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-imagebuilder?color=blue)](https://pypistats.org/packages/mypy-boto3-imagebuilder)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.imagebuilder 1.26.51](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder)
+[boto3.imagebuilder 1.26.60](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-imagebuilder-1.26.51/mypy_boto3_imagebuilder/__main__.py` & `mypy-boto3-imagebuilder-1.26.60/mypy_boto3_imagebuilder/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.imagebuilder 1.26.51\nVersion:         1.26.51\nBuilder"
+        "Type annotations for boto3.imagebuilder 1.26.60\nVersion:         1.26.60\nBuilder"
         " version: 7.12.3\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_imagebuilder//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.51")
+    print("1.26.60")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-imagebuilder-1.26.51/mypy_boto3_imagebuilder/client.py` & `mypy-boto3-imagebuilder-1.26.60/mypy_boto3_imagebuilder/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-imagebuilder-1.26.51/mypy_boto3_imagebuilder/client.pyi` & `mypy-boto3-imagebuilder-1.26.60/mypy_boto3_imagebuilder/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-imagebuilder-1.26.51/mypy_boto3_imagebuilder/literals.py` & `mypy-boto3-imagebuilder-1.26.60/mypy_boto3_imagebuilder/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-imagebuilder-1.26.51/mypy_boto3_imagebuilder/literals.pyi` & `mypy-boto3-imagebuilder-1.26.60/mypy_boto3_imagebuilder/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-imagebuilder-1.26.51/mypy_boto3_imagebuilder/type_defs.py` & `mypy-boto3-imagebuilder-1.26.60/mypy_boto3_imagebuilder/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-imagebuilder-1.26.51/mypy_boto3_imagebuilder/type_defs.pyi` & `mypy-boto3-imagebuilder-1.26.60/mypy_boto3_imagebuilder/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-imagebuilder-1.26.51/mypy_boto3_imagebuilder.egg-info/PKG-INFO` & `mypy-boto3-imagebuilder-1.26.60/mypy_boto3_imagebuilder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-imagebuilder
-Version: 1.26.51
-Summary: Type annotations for boto3.imagebuilder 1.26.51 service generated with mypy-boto3-builder 7.12.3
+Version: 1.26.60
+Summary: Type annotations for boto3.imagebuilder 1.26.60 service generated with mypy-boto3-builder 7.12.3
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_imagebuilder/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-imagebuilder.svg?color=blue)](https://pypi.org/project/mypy-boto3-imagebuilder)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-imagebuilder?color=blue)](https://pypistats.org/packages/mypy-boto3-imagebuilder)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.imagebuilder 1.26.51](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder)
+[boto3.imagebuilder 1.26.60](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-imagebuilder-1.26.51/mypy_boto3_imagebuilder.egg-info/SOURCES.txt` & `mypy-boto3-imagebuilder-1.26.60/mypy_boto3_imagebuilder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-imagebuilder-1.26.51/setup.py` & `mypy-boto3-imagebuilder-1.26.60/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-imagebuilder",
-    version="1.26.51",
+    version="1.26.60",
     packages=["mypy_boto3_imagebuilder"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.imagebuilder 1.26.51 service generated with mypy-boto3-builder"
+        "Type annotations for boto3.imagebuilder 1.26.60 service generated with mypy-boto3-builder"
         " 7.12.3"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

