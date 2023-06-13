# Comparing `tmp/mypy-boto3-cloudtrail-1.26.61.tar.gz` & `tmp/mypy-boto3-cloudtrail-1.26.72.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-cloudtrail-1.26.61.tar", last modified: Tue Jan 31 20:49:53 2023, max compression
+gzip compressed data, was "mypy-boto3-cloudtrail-1.26.72.tar", last modified: Wed Feb 15 22:27:56 2023, max compression
```

## Comparing `mypy-boto3-cloudtrail-1.26.61.tar` & `mypy-boto3-cloudtrail-1.26.72.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 20:49:53.638128 mypy-boto3-cloudtrail-1.26.61/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-01-31 20:47:24.000000 mypy-boto3-cloudtrail-1.26.61/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17688 2023-01-31 20:49:53.638128 mypy-boto3-cloudtrail-1.26.61/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16189 2023-01-31 20:47:24.000000 mypy-boto3-cloudtrail-1.26.61/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 20:49:53.638128 mypy-boto3-cloudtrail-1.26.61/mypy_boto3_cloudtrail/
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-01-31 20:47:24.000000 mypy-boto3-cloudtrail-1.26.61/mypy_boto3_cloudtrail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-01-31 20:47:24.000000 mypy-boto3-cloudtrail-1.26.61/mypy_boto3_cloudtrail/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-01-31 20:47:24.000000 mypy-boto3-cloudtrail-1.26.61/mypy_boto3_cloudtrail/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37753 2023-01-31 20:47:25.000000 mypy-boto3-cloudtrail-1.26.61/mypy_boto3_cloudtrail/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    37696 2023-01-31 20:47:25.000000 mypy-boto3-cloudtrail-1.26.61/mypy_boto3_cloudtrail/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9782 2023-01-31 20:47:25.000000 mypy-boto3-cloudtrail-1.26.61/mypy_boto3_cloudtrail/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9780 2023-01-31 20:47:25.000000 mypy-boto3-cloudtrail-1.26.61/mypy_boto3_cloudtrail/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-01-31 20:47:25.000000 mypy-boto3-cloudtrail-1.26.61/mypy_boto3_cloudtrail/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7598 2023-01-31 20:47:25.000000 mypy-boto3-cloudtrail-1.26.61/mypy_boto3_cloudtrail/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 20:47:24.000000 mypy-boto3-cloudtrail-1.26.61/mypy_boto3_cloudtrail/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    39728 2023-01-31 20:47:26.000000 mypy-boto3-cloudtrail-1.26.61/mypy_boto3_cloudtrail/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    39689 2023-01-31 20:47:26.000000 mypy-boto3-cloudtrail-1.26.61/mypy_boto3_cloudtrail/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-31 20:47:24.000000 mypy-boto3-cloudtrail-1.26.61/mypy_boto3_cloudtrail/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 20:49:53.638128 mypy-boto3-cloudtrail-1.26.61/mypy_boto3_cloudtrail.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17688 2023-01-31 20:49:53.000000 mypy-boto3-cloudtrail-1.26.61/mypy_boto3_cloudtrail.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-01-31 20:49:53.000000 mypy-boto3-cloudtrail-1.26.61/mypy_boto3_cloudtrail.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 20:49:53.000000 mypy-boto3-cloudtrail-1.26.61/mypy_boto3_cloudtrail.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 20:49:53.000000 mypy-boto3-cloudtrail-1.26.61/mypy_boto3_cloudtrail.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-31 20:49:53.000000 mypy-boto3-cloudtrail-1.26.61/mypy_boto3_cloudtrail.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-31 20:49:53.000000 mypy-boto3-cloudtrail-1.26.61/mypy_boto3_cloudtrail.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-31 20:49:53.638128 mypy-boto3-cloudtrail-1.26.61/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-01-31 20:47:24.000000 mypy-boto3-cloudtrail-1.26.61/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 22:27:56.846127 mypy-boto3-cloudtrail-1.26.72/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-15 22:27:02.000000 mypy-boto3-cloudtrail-1.26.72/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17688 2023-02-15 22:27:56.842126 mypy-boto3-cloudtrail-1.26.72/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16189 2023-02-15 22:27:02.000000 mypy-boto3-cloudtrail-1.26.72/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 22:27:56.834126 mypy-boto3-cloudtrail-1.26.72/mypy_boto3_cloudtrail/
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-02-15 22:27:02.000000 mypy-boto3-cloudtrail-1.26.72/mypy_boto3_cloudtrail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-02-15 22:27:02.000000 mypy-boto3-cloudtrail-1.26.72/mypy_boto3_cloudtrail/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-02-15 22:27:02.000000 mypy-boto3-cloudtrail-1.26.72/mypy_boto3_cloudtrail/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37753 2023-02-15 22:27:03.000000 mypy-boto3-cloudtrail-1.26.72/mypy_boto3_cloudtrail/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37696 2023-02-15 22:27:03.000000 mypy-boto3-cloudtrail-1.26.72/mypy_boto3_cloudtrail/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9782 2023-02-15 22:27:03.000000 mypy-boto3-cloudtrail-1.26.72/mypy_boto3_cloudtrail/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9780 2023-02-15 22:27:03.000000 mypy-boto3-cloudtrail-1.26.72/mypy_boto3_cloudtrail/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-02-15 22:27:03.000000 mypy-boto3-cloudtrail-1.26.72/mypy_boto3_cloudtrail/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7598 2023-02-15 22:27:03.000000 mypy-boto3-cloudtrail-1.26.72/mypy_boto3_cloudtrail/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-15 22:27:02.000000 mypy-boto3-cloudtrail-1.26.72/mypy_boto3_cloudtrail/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    39728 2023-02-15 22:27:05.000000 mypy-boto3-cloudtrail-1.26.72/mypy_boto3_cloudtrail/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39689 2023-02-15 22:27:04.000000 mypy-boto3-cloudtrail-1.26.72/mypy_boto3_cloudtrail/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-15 22:27:02.000000 mypy-boto3-cloudtrail-1.26.72/mypy_boto3_cloudtrail/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 22:27:56.842126 mypy-boto3-cloudtrail-1.26.72/mypy_boto3_cloudtrail.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17688 2023-02-15 22:27:56.000000 mypy-boto3-cloudtrail-1.26.72/mypy_boto3_cloudtrail.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-02-15 22:27:56.000000 mypy-boto3-cloudtrail-1.26.72/mypy_boto3_cloudtrail.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-15 22:27:56.000000 mypy-boto3-cloudtrail-1.26.72/mypy_boto3_cloudtrail.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-15 22:27:56.000000 mypy-boto3-cloudtrail-1.26.72/mypy_boto3_cloudtrail.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-15 22:27:56.000000 mypy-boto3-cloudtrail-1.26.72/mypy_boto3_cloudtrail.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-15 22:27:56.000000 mypy-boto3-cloudtrail-1.26.72/mypy_boto3_cloudtrail.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-15 22:27:56.846127 mypy-boto3-cloudtrail-1.26.72/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-02-15 22:27:02.000000 mypy-boto3-cloudtrail-1.26.72/setup.py
```

### Comparing `mypy-boto3-cloudtrail-1.26.61/LICENSE` & `mypy-boto3-cloudtrail-1.26.72/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudtrail-1.26.61/PKG-INFO` & `mypy-boto3-cloudtrail-1.26.72/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cloudtrail
-Version: 1.26.61
-Summary: Type annotations for boto3.CloudTrail 1.26.61 service generated with mypy-boto3-builder 7.12.3
+Version: 1.26.72
+Summary: Type annotations for boto3.CloudTrail 1.26.72 service generated with mypy-boto3-builder 7.12.3
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudtrail.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudtrail)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cloudtrail?color=blue)](https://pypistats.org/packages/mypy-boto3-cloudtrail)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudTrail 1.26.61](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail)
+[boto3.CloudTrail 1.26.72](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-cloudtrail-1.26.61/README.md` & `mypy-boto3-cloudtrail-1.26.72/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudtrail.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudtrail)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cloudtrail?color=blue)](https://pypistats.org/packages/mypy-boto3-cloudtrail)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudTrail 1.26.61](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail)
+[boto3.CloudTrail 1.26.72](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-cloudtrail-1.26.61/mypy_boto3_cloudtrail/__init__.py` & `mypy-boto3-cloudtrail-1.26.72/mypy_boto3_cloudtrail/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudtrail-1.26.61/mypy_boto3_cloudtrail/__init__.pyi` & `mypy-boto3-cloudtrail-1.26.72/mypy_boto3_cloudtrail/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudtrail-1.26.61/mypy_boto3_cloudtrail/__main__.py` & `mypy-boto3-cloudtrail-1.26.72/mypy_boto3_cloudtrail/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CloudTrail 1.26.61\nVersion:         1.26.61\nBuilder version:"
+        "Type annotations for boto3.CloudTrail 1.26.72\nVersion:         1.26.72\nBuilder version:"
         " 7.12.3\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.61")
+    print("1.26.72")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-cloudtrail-1.26.61/mypy_boto3_cloudtrail/client.py` & `mypy-boto3-cloudtrail-1.26.72/mypy_boto3_cloudtrail/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudtrail-1.26.61/mypy_boto3_cloudtrail/client.pyi` & `mypy-boto3-cloudtrail-1.26.72/mypy_boto3_cloudtrail/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudtrail-1.26.61/mypy_boto3_cloudtrail/literals.py` & `mypy-boto3-cloudtrail-1.26.72/mypy_boto3_cloudtrail/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudtrail-1.26.61/mypy_boto3_cloudtrail/literals.pyi` & `mypy-boto3-cloudtrail-1.26.72/mypy_boto3_cloudtrail/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudtrail-1.26.61/mypy_boto3_cloudtrail/paginator.py` & `mypy-boto3-cloudtrail-1.26.72/mypy_boto3_cloudtrail/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudtrail-1.26.61/mypy_boto3_cloudtrail/paginator.pyi` & `mypy-boto3-cloudtrail-1.26.72/mypy_boto3_cloudtrail/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudtrail-1.26.61/mypy_boto3_cloudtrail/type_defs.py` & `mypy-boto3-cloudtrail-1.26.72/mypy_boto3_cloudtrail/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudtrail-1.26.61/mypy_boto3_cloudtrail/type_defs.pyi` & `mypy-boto3-cloudtrail-1.26.72/mypy_boto3_cloudtrail/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudtrail-1.26.61/mypy_boto3_cloudtrail.egg-info/PKG-INFO` & `mypy-boto3-cloudtrail-1.26.72/mypy_boto3_cloudtrail.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cloudtrail
-Version: 1.26.61
-Summary: Type annotations for boto3.CloudTrail 1.26.61 service generated with mypy-boto3-builder 7.12.3
+Version: 1.26.72
+Summary: Type annotations for boto3.CloudTrail 1.26.72 service generated with mypy-boto3-builder 7.12.3
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudtrail.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudtrail)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cloudtrail?color=blue)](https://pypistats.org/packages/mypy-boto3-cloudtrail)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudTrail 1.26.61](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail)
+[boto3.CloudTrail 1.26.72](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-cloudtrail-1.26.61/mypy_boto3_cloudtrail.egg-info/SOURCES.txt` & `mypy-boto3-cloudtrail-1.26.72/mypy_boto3_cloudtrail.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudtrail-1.26.61/setup.py` & `mypy-boto3-cloudtrail-1.26.72/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-cloudtrail",
-    version="1.26.61",
+    version="1.26.72",
     packages=["mypy_boto3_cloudtrail"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CloudTrail 1.26.61 service generated with mypy-boto3-builder"
+        "Type annotations for boto3.CloudTrail 1.26.72 service generated with mypy-boto3-builder"
         " 7.12.3"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

