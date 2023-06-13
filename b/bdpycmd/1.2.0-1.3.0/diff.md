# Comparing `tmp/bdpycmd-1.2.0.tar.gz` & `tmp/bdpycmd-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bdpycmd-1.2.0.tar", last modified: Wed May 11 06:44:04 2022, max compression
+gzip compressed data, was "bdpycmd-1.3.0.tar", last modified: Tue Jun 13 08:38:16 2023, max compression
```

## Comparing `bdpycmd-1.2.0.tar` & `bdpycmd-1.3.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxrwx   0        0        0        0 2022-05-11 06:44:04.678239 bdpycmd-1.2.0/
--rw-rw-rw-   0        0        0     1817 2022-05-11 06:44:04.678239 bdpycmd-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     1140 2022-05-11 05:34:01.000000 bdpycmd-1.2.0/README.md
--rw-rw-rw-   0        0        0       82 2022-05-11 02:54:27.000000 bdpycmd-1.2.0/pyproject.toml
--rw-rw-rw-   0        0        0      815 2022-05-11 06:44:04.680314 bdpycmd-1.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-05-11 06:44:04.647045 bdpycmd-1.2.0/src/
-drwxrwxrwx   0        0        0        0 2022-05-11 06:44:04.654791 bdpycmd-1.2.0/src/bdpycmd/
--rw-rw-rw-   0        0        0        0 2022-05-11 05:55:37.000000 bdpycmd-1.2.0/src/bdpycmd/__init__.py
-drwxrwxrwx   0        0        0        0 2022-05-11 06:44:04.673762 bdpycmd-1.2.0/src/bdpycmd/cmd/
--rw-rw-rw-   0        0        0        0 2021-12-11 16:02:29.000000 bdpycmd-1.2.0/src/bdpycmd/cmd/__init__.py
-drwxrwxrwx   0        0        0        0 2022-05-11 06:44:04.674992 bdpycmd-1.2.0/src/bdpycmd/cmd/camp/
--rw-rw-rw-   0        0        0        0 2022-05-11 03:19:15.000000 bdpycmd-1.2.0/src/bdpycmd/cmd/camp/__init__.py
--rw-rw-rw-   0        0        0     2122 2022-05-11 05:31:50.000000 bdpycmd-1.2.0/src/bdpycmd/cmd/camp/assistant.py
-drwxrwxrwx   0        0        0        0 2022-05-11 06:44:04.677228 bdpycmd-1.2.0/src/bdpycmd/cmd/factory/
--rw-rw-rw-   0        0        0        0 2021-12-11 16:02:29.000000 bdpycmd-1.2.0/src/bdpycmd/cmd/factory/__init__.py
--rw-rw-rw-   0        0        0     3831 2022-05-11 05:26:55.000000 bdpycmd-1.2.0/src/bdpycmd/cmd/factory/base.py
--rw-rw-rw-   0        0        0     6139 2022-05-11 06:01:34.000000 bdpycmd-1.2.0/src/bdpycmd/pycmd.py
-drwxrwxrwx   0        0        0        0 2022-05-11 06:44:04.671070 bdpycmd-1.2.0/src/bdpycmd.egg-info/
--rw-rw-rw-   0        0        0     1817 2022-05-11 06:44:04.000000 bdpycmd-1.2.0/src/bdpycmd.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      382 2022-05-11 06:44:04.000000 bdpycmd-1.2.0/src/bdpycmd.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-05-11 06:44:04.000000 bdpycmd-1.2.0/src/bdpycmd.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2022-05-11 06:44:04.000000 bdpycmd-1.2.0/src/bdpycmd.egg-info/top_level.txt
+drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 08:38:16.854078 bdpycmd-1.3.0/
+-rw-r--r--   0 zhicheng   (501) staff       (20)     2066 2023-06-13 08:38:16.854158 bdpycmd-1.3.0/PKG-INFO
+-rw-r--r--   0 zhicheng   (501) staff       (20)     1406 2023-06-13 08:32:29.000000 bdpycmd-1.3.0/README.md
+-rw-r--r--   0 zhicheng   (501) staff       (20)       80 2022-09-04 10:23:26.000000 bdpycmd-1.3.0/pyproject.toml
+-rw-r--r--   0 zhicheng   (501) staff       (20)      784 2023-06-13 08:38:16.854419 bdpycmd-1.3.0/setup.cfg
+drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 08:38:16.851808 bdpycmd-1.3.0/src/
+drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 08:38:16.852837 bdpycmd-1.3.0/src/bdpycmd/
+-rw-r--r--   0 zhicheng   (501) staff       (20)        0 2023-06-13 08:19:55.000000 bdpycmd-1.3.0/src/bdpycmd/__init__.py
+drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 08:38:16.853445 bdpycmd-1.3.0/src/bdpycmd/cmd/
+-rw-r--r--   0 zhicheng   (501) staff       (20)        0 2023-06-13 08:12:26.000000 bdpycmd-1.3.0/src/bdpycmd/cmd/__init__.py
+drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 08:38:16.853637 bdpycmd-1.3.0/src/bdpycmd/cmd/camp/
+-rw-r--r--   0 zhicheng   (501) staff       (20)        0 2023-06-13 08:12:26.000000 bdpycmd-1.3.0/src/bdpycmd/cmd/camp/__init__.py
+-rw-r--r--   0 zhicheng   (501) staff       (20)     2560 2023-06-13 08:12:26.000000 bdpycmd-1.3.0/src/bdpycmd/cmd/camp/assistant.py
+drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 08:38:16.853980 bdpycmd-1.3.0/src/bdpycmd/cmd/factory/
+-rw-r--r--   0 zhicheng   (501) staff       (20)        0 2023-06-13 08:12:26.000000 bdpycmd-1.3.0/src/bdpycmd/cmd/factory/__init__.py
+-rw-r--r--   0 zhicheng   (501) staff       (20)     3918 2023-06-13 08:12:26.000000 bdpycmd-1.3.0/src/bdpycmd/cmd/factory/base.py
+-rw-r--r--   0 zhicheng   (501) staff       (20)      716 2023-06-13 08:12:26.000000 bdpycmd-1.3.0/src/bdpycmd/cmd/factory/cmd.py
+-rw-r--r--   0 zhicheng   (501) staff       (20)     7388 2023-06-13 08:12:26.000000 bdpycmd-1.3.0/src/bdpycmd/pycmd.py
+drwxr-xr-x   0 zhicheng   (501) staff       (20)        0 2023-06-13 08:38:16.853321 bdpycmd-1.3.0/src/bdpycmd.egg-info/
+-rw-r--r--   0 zhicheng   (501) staff       (20)     2066 2023-06-13 08:38:16.000000 bdpycmd-1.3.0/src/bdpycmd.egg-info/PKG-INFO
+-rw-r--r--   0 zhicheng   (501) staff       (20)      413 2023-06-13 08:38:16.000000 bdpycmd-1.3.0/src/bdpycmd.egg-info/SOURCES.txt
+-rw-r--r--   0 zhicheng   (501) staff       (20)        1 2023-06-13 08:38:16.000000 bdpycmd-1.3.0/src/bdpycmd.egg-info/dependency_links.txt
+-rw-r--r--   0 zhicheng   (501) staff       (20)        8 2023-06-13 08:38:16.000000 bdpycmd-1.3.0/src/bdpycmd.egg-info/top_level.txt
```

### Comparing `bdpycmd-1.2.0/PKG-INFO` & `bdpycmd-1.3.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,51 +1,43 @@
-Metadata-Version: 2.1
-Name: bdpycmd
-Version: 1.2.0
-Summary: Run Python`s file as command line
-Home-page: https://github.com/biandoucheng/bd-py-cmd
-Author: biandoucheng
-Author-email: biandoucheng@outlook.com
-Project-URL: Bug Tracker, https://github.com/biandoucheng/bd-py-cmd/issues
-Project-URL: Use Example, https://github.com/biandoucheng/open-example/tree/main/bdpycmd-example
-Classifier: Programming Language :: Python :: 3.5
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 5 - Production/Stable
-Requires-Python: >=3.5
-Description-Content-Type: text/markdown
-
-# Python command tool
-
-## Require
-+ python3.5 +
-
-## Description
-`
-It is used to run your Python code as a command line .
-It only works on class methods .
-Add as_cmder decorator on your class method and create command class in command file directory .
-In your project root directory, create a pycmd.py file and import everything under the bdpycmd.pycmd module .
-Add initialization code and execution entry to your pycmd.py .
-Open the command line interface, go to your project root directory (the same level as your pycmd.py file), and run python pycmd.py .
-`
-## Use the example project url
-<https://github.com/biandoucheng/open-example/tree/main/bdpycmd-example>
-
-## Source Codd url
-<https://github.com/biandoucheng/bd-py-cmd>
-
-## Annotation Specification
-`
-When adding comments to the command method, the following rules must be followed, otherwise the command parameters will not be parsed correctly
-
-@base.BaseCommand.as_cmder
-def your_func(p1,p2):
-    """
-    your function`s description
-
-    :param p1: type #describe
-    :param p2: type #describe
-    :return: type
-    """
-    your_func_content ...
-`
+# Python command tool
+
+## Require
++ python3.5 +
+
+## Description
+`
+It is used to run your Python code as a command line .
+It only works on class methods .
+Add as_cmder decorator on your class method and create command class in command file directory .
+In your project root directory, create a pycmd.py file and import everything under the bdpycmd.pycmd module .
+Add initialization code and execution entry to your pycmd.py .
+Open the command line interface, go to your project root directory (the same level as your pycmd.py file), and run python pycmd.py .
+`
+## Use the example project url
+<https://github.com/biandoucheng/open-example/tree/main/bdpycmd-example>
+
+## Source Codd url
+<https://github.com/biandoucheng/bd-py-cmd>
+
+## Annotation Specification
+`
+When adding comments to the command method, the following rules must be followed, otherwise the command parameters will not be parsed correctly
+
+@base.BaseCommand.as_cmder
+def your_func(p1,p2):
+    """
+    your function`s description
+
+    :param p1: type #describe
+    :param p2: type #describe
+    :return: type
+    """
+    your_func_content ...
+`
+## New features
+`
+2023.06.13
+1. Support command keyword retrieval:
+    No content input, press Enter directly to reality the next command
+    Enter the command number or any range, and relevant commands will be queried based on the provided content
+    Enter the '/' symbol to exit the help prompt
+`
```

