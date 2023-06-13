# Comparing `tmp/gitwrapperlib-1.0.1.tar.gz` & `tmp/gitwrapperlib-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitwrapperlib-1.0.1.tar", last modified: Tue Jun 13 11:06:09 2023, max compression
+gzip compressed data, was "gitwrapperlib-1.0.2.tar", last modified: Tue Jun 13 11:28:54 2023, max compression
```

## Comparing `gitwrapperlib-1.0.1.tar` & `gitwrapperlib-1.0.2.tar`

### file list

```diff
@@ -1,60 +1,51 @@
-drwxr-xr-x   0 ctyfoxylos   (502) staff       (20)        0 2023-06-13 11:06:09.755581 gitwrapperlib-1.0.1/
--rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)        5 2023-06-13 11:04:35.000000 gitwrapperlib-1.0.1/.VERSION
--rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)      171 2023-01-05 16:54:06.000000 gitwrapperlib-1.0.1/AUTHORS.rst
--rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)     1268 2023-01-05 16:54:03.000000 gitwrapperlib-1.0.1/CONTRIBUTING.rst
--rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)      837 2023-06-13 11:04:50.000000 gitwrapperlib-1.0.1/HISTORY.rst
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)     1063 2023-01-05 16:54:09.000000 gitwrapperlib-1.0.1/LICENSE
--rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)      400 2023-01-05 16:54:11.000000 gitwrapperlib-1.0.1/MANIFEST.in
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)     3717 2023-06-13 11:06:09.755755 gitwrapperlib-1.0.1/PKG-INFO
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)      600 2023-06-13 09:42:10.000000 gitwrapperlib-1.0.1/Pipfile
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)    59590 2023-06-13 09:41:25.000000 gitwrapperlib-1.0.1/Pipfile.lock
--rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)     2323 2023-01-05 16:54:07.000000 gitwrapperlib-1.0.1/README.rst
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)      913 2023-01-05 16:54:04.000000 gitwrapperlib-1.0.1/USAGE.rst
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)      588 2023-06-13 11:06:06.000000 gitwrapperlib-1.0.1/dev-requirements.txt
-drwxr-xr-x   0 ctyfoxylos   (502) staff       (20)        0 2023-06-13 11:06:09.649700 gitwrapperlib-1.0.1/docs/
--rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)     6790 2023-01-05 17:00:40.000000 gitwrapperlib-1.0.1/docs/Makefile
--rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)       28 2023-01-05 17:00:40.000000 gitwrapperlib-1.0.1/docs/authors.rst
--rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)     8964 2023-01-05 17:00:40.000000 gitwrapperlib-1.0.1/docs/conf.py
--rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)       33 2023-01-05 17:00:40.000000 gitwrapperlib-1.0.1/docs/contributing.rst
--rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)       28 2023-01-05 17:00:40.000000 gitwrapperlib-1.0.1/docs/history.rst
--rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)      513 2023-01-05 17:00:40.000000 gitwrapperlib-1.0.1/docs/index.rst
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)       33 2023-01-05 17:00:40.000000 gitwrapperlib-1.0.1/docs/installation.rst
--rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)       27 2023-01-05 17:00:40.000000 gitwrapperlib-1.0.1/docs/readme.rst
--rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)       26 2023-01-05 17:00:40.000000 gitwrapperlib-1.0.1/docs/usage.rst
-drwxr-xr-x   0 ctyfoxylos   (502) staff       (20)        0 2023-06-13 11:06:09.705129 gitwrapperlib-1.0.1/gitwrapperlib/
--rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)        5 2023-06-13 11:06:06.000000 gitwrapperlib-1.0.1/gitwrapperlib/.VERSION
--rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)      171 2023-06-13 11:06:06.000000 gitwrapperlib-1.0.1/gitwrapperlib/AUTHORS.rst
--rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)     1268 2023-06-13 11:06:06.000000 gitwrapperlib-1.0.1/gitwrapperlib/CONTRIBUTING.rst
--rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)      837 2023-06-13 11:06:06.000000 gitwrapperlib-1.0.1/gitwrapperlib/HISTORY.rst
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)     1063 2023-06-13 11:06:06.000000 gitwrapperlib-1.0.1/gitwrapperlib/LICENSE
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)      600 2023-06-13 11:06:06.000000 gitwrapperlib-1.0.1/gitwrapperlib/Pipfile
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)    59590 2023-06-13 11:06:06.000000 gitwrapperlib-1.0.1/gitwrapperlib/Pipfile.lock
--rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)     2323 2023-06-13 11:06:06.000000 gitwrapperlib-1.0.1/gitwrapperlib/README.rst
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)      913 2023-06-13 11:06:06.000000 gitwrapperlib-1.0.1/gitwrapperlib/USAGE.rst
--rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)     1962 2023-06-13 08:39:21.000000 gitwrapperlib-1.0.1/gitwrapperlib/__init__.py
-drwxr-xr-x   0 ctyfoxylos   (502) staff       (20)        0 2023-06-13 11:06:09.747910 gitwrapperlib-1.0.1/gitwrapperlib/__pycache__/
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)      821 2021-06-02 07:43:10.000000 gitwrapperlib-1.0.1/gitwrapperlib/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)      810 2023-06-13 09:43:55.000000 gitwrapperlib-1.0.1/gitwrapperlib/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)      919 2021-06-02 07:43:10.000000 gitwrapperlib-1.0.1/gitwrapperlib/__pycache__/_version.cpython-37.pyc
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)     1043 2023-06-13 09:43:55.000000 gitwrapperlib-1.0.1/gitwrapperlib/__pycache__/_version.cpython-39.pyc
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)     6402 2021-12-02 08:06:31.000000 gitwrapperlib-1.0.1/gitwrapperlib/__pycache__/gitwrapperlib.cpython-37.pyc
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)     7064 2023-06-13 10:52:37.000000 gitwrapperlib-1.0.1/gitwrapperlib/__pycache__/gitwrapperlib.cpython-39.pyc
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)      861 2021-06-02 07:43:10.000000 gitwrapperlib-1.0.1/gitwrapperlib/__pycache__/gitwrapperlibexceptions.cpython-37.pyc
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)     1231 2023-06-13 09:43:55.000000 gitwrapperlib-1.0.1/gitwrapperlib/__pycache__/gitwrapperlibexceptions.cpython-39.pyc
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)     2194 2023-06-13 08:36:02.000000 gitwrapperlib-1.0.1/gitwrapperlib/_version.py
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)      588 2023-06-13 11:06:06.000000 gitwrapperlib-1.0.1/gitwrapperlib/dev-requirements.txt
--rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)     6961 2023-06-13 10:52:27.000000 gitwrapperlib-1.0.1/gitwrapperlib/gitwrapperlib.py
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)     1986 2023-06-13 08:36:02.000000 gitwrapperlib-1.0.1/gitwrapperlib/gitwrapperlibexceptions.py
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)      406 2023-06-13 11:06:06.000000 gitwrapperlib-1.0.1/gitwrapperlib/requirements.txt
-drwxr-xr-x   0 ctyfoxylos   (502) staff       (20)        0 2023-06-13 11:06:09.719221 gitwrapperlib-1.0.1/gitwrapperlib.egg-info/
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)     3717 2023-06-13 11:06:09.000000 gitwrapperlib-1.0.1/gitwrapperlib.egg-info/PKG-INFO
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)     1423 2023-06-13 11:06:09.000000 gitwrapperlib-1.0.1/gitwrapperlib.egg-info/SOURCES.txt
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)        1 2023-06-13 11:06:09.000000 gitwrapperlib-1.0.1/gitwrapperlib.egg-info/dependency_links.txt
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)        1 2023-06-13 09:42:02.000000 gitwrapperlib-1.0.1/gitwrapperlib.egg-info/not-zip-safe
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)       77 2023-06-13 11:06:09.000000 gitwrapperlib-1.0.1/gitwrapperlib.egg-info/requires.txt
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)       14 2023-06-13 11:06:09.000000 gitwrapperlib-1.0.1/gitwrapperlib.egg-info/top_level.txt
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)      406 2023-06-13 11:06:06.000000 gitwrapperlib-1.0.1/requirements.txt
--rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)      153 2023-06-13 11:06:09.757766 gitwrapperlib-1.0.1/setup.cfg
--rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)     1967 2023-01-05 16:54:03.000000 gitwrapperlib-1.0.1/setup.py
-drwxr-xr-x   0 ctyfoxylos   (502) staff       (20)        0 2023-06-13 11:06:09.754561 gitwrapperlib-1.0.1/tests/
--rw-r--r--   0 ctyfoxylos   (502) staff       (20)     2218 2023-01-05 17:00:40.000000 gitwrapperlib-1.0.1/tests/test_gitwrapperlib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:28:54.343836 gitwrapperlib-1.0.2/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        5 2023-06-13 11:27:33.000000 gitwrapperlib-1.0.2/.VERSION
+-rwxr-xr-x   0 runner    (1001) docker     (123)      171 2023-06-13 11:27:33.000000 gitwrapperlib-1.0.2/AUTHORS.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1268 2023-06-13 11:27:33.000000 gitwrapperlib-1.0.2/CONTRIBUTING.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)      899 2023-06-13 11:27:33.000000 gitwrapperlib-1.0.2/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-13 11:27:33.000000 gitwrapperlib-1.0.2/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (123)      400 2023-06-13 11:27:33.000000 gitwrapperlib-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-06-13 11:28:54.343836 gitwrapperlib-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-13 11:27:33.000000 gitwrapperlib-1.0.2/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)    68815 2023-06-13 11:28:53.000000 gitwrapperlib-1.0.2/Pipfile.lock
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2323 2023-06-13 11:27:33.000000 gitwrapperlib-1.0.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-06-13 11:27:33.000000 gitwrapperlib-1.0.2/USAGE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-13 11:28:53.000000 gitwrapperlib-1.0.2/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:28:54.339836 gitwrapperlib-1.0.2/docs/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6790 2023-06-13 11:27:33.000000 gitwrapperlib-1.0.2/docs/Makefile
+-rwxr-xr-x   0 runner    (1001) docker     (123)       28 2023-06-13 11:27:33.000000 gitwrapperlib-1.0.2/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8964 2023-06-13 11:27:33.000000 gitwrapperlib-1.0.2/docs/conf.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       33 2023-06-13 11:27:33.000000 gitwrapperlib-1.0.2/docs/contributing.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)       28 2023-06-13 11:27:33.000000 gitwrapperlib-1.0.2/docs/history.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)      513 2023-06-13 11:27:33.000000 gitwrapperlib-1.0.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-13 11:27:33.000000 gitwrapperlib-1.0.2/docs/installation.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)       27 2023-06-13 11:27:33.000000 gitwrapperlib-1.0.2/docs/readme.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)       26 2023-06-13 11:27:33.000000 gitwrapperlib-1.0.2/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:28:54.339836 gitwrapperlib-1.0.2/gitwrapperlib/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        5 2023-06-13 11:28:53.000000 gitwrapperlib-1.0.2/gitwrapperlib/.VERSION
+-rwxr-xr-x   0 runner    (1001) docker     (123)      171 2023-06-13 11:28:53.000000 gitwrapperlib-1.0.2/gitwrapperlib/AUTHORS.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1268 2023-06-13 11:28:53.000000 gitwrapperlib-1.0.2/gitwrapperlib/CONTRIBUTING.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)      899 2023-06-13 11:28:53.000000 gitwrapperlib-1.0.2/gitwrapperlib/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-13 11:28:53.000000 gitwrapperlib-1.0.2/gitwrapperlib/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-13 11:28:53.000000 gitwrapperlib-1.0.2/gitwrapperlib/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)    68815 2023-06-13 11:28:53.000000 gitwrapperlib-1.0.2/gitwrapperlib/Pipfile.lock
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2323 2023-06-13 11:28:53.000000 gitwrapperlib-1.0.2/gitwrapperlib/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-06-13 11:28:53.000000 gitwrapperlib-1.0.2/gitwrapperlib/USAGE.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1962 2023-06-13 11:27:33.000000 gitwrapperlib-1.0.2/gitwrapperlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-06-13 11:27:33.000000 gitwrapperlib-1.0.2/gitwrapperlib/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-13 11:28:53.000000 gitwrapperlib-1.0.2/gitwrapperlib/dev-requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6961 2023-06-13 11:27:33.000000 gitwrapperlib-1.0.2/gitwrapperlib/gitwrapperlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-06-13 11:27:33.000000 gitwrapperlib-1.0.2/gitwrapperlib/gitwrapperlibexceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-13 11:28:53.000000 gitwrapperlib-1.0.2/gitwrapperlib/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:28:54.339836 gitwrapperlib-1.0.2/gitwrapperlib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-06-13 11:28:54.000000 gitwrapperlib-1.0.2/gitwrapperlib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-13 11:28:54.000000 gitwrapperlib-1.0.2/gitwrapperlib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 11:28:54.000000 gitwrapperlib-1.0.2/gitwrapperlib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 11:28:54.000000 gitwrapperlib-1.0.2/gitwrapperlib.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-13 11:28:54.000000 gitwrapperlib-1.0.2/gitwrapperlib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-13 11:28:54.000000 gitwrapperlib-1.0.2/gitwrapperlib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-13 11:28:53.000000 gitwrapperlib-1.0.2/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      153 2023-06-13 11:28:54.343836 gitwrapperlib-1.0.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1967 2023-06-13 11:27:33.000000 gitwrapperlib-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:28:54.343836 gitwrapperlib-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-06-13 11:27:33.000000 gitwrapperlib-1.0.2/tests/test_gitwrapperlib.py
```

### Comparing `gitwrapperlib-1.0.1/CONTRIBUTING.rst` & `gitwrapperlib-1.0.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `gitwrapperlib-1.0.1/HISTORY.rst` & `gitwrapperlib-1.0.2/HISTORY.rst`

 * *Files 12% similar despite different names*

```diff
@@ -51,7 +51,13 @@
 * Removed references to master branch and implemented default remote retrieval, courtesy of Sten Spans <sspans@schubergphilis.com>
 
 
 1.0.1 (13-06-2023)
 ------------------
 
 * Bump dependencies and update pipeline to python 3.9.
+
+
+1.0.2 (13-06-2023)
+------------------
+
+* Bump dependencies.
```

### Comparing `gitwrapperlib-1.0.1/LICENSE` & `gitwrapperlib-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gitwrapperlib-1.0.1/PKG-INFO` & `gitwrapperlib-1.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitwrapperlib
-Version: 1.0.1
+Version: 1.0.2
 Summary: A lightweight wrapper around the git command using sh module.
 Home-page: https://github.com/costastf/gitwrapperlib
 Author: Costas Tyfoxylos
 Author-email: costas.tyf@gmail.com
 License: MIT
 Keywords: gitwrapperlib git python sh
 Classifier: Development Status :: 4 - Beta
@@ -138,7 +138,13 @@
 * Removed references to master branch and implemented default remote retrieval, courtesy of Sten Spans <sspans@schubergphilis.com>
 
 
 1.0.1 (13-06-2023)
 ------------------
 
 * Bump dependencies and update pipeline to python 3.9.
+
+
+1.0.2 (13-06-2023)
+------------------
+
+* Bump dependencies.
```

### Comparing `gitwrapperlib-1.0.1/Pipfile` & `gitwrapperlib-1.0.2/Pipfile`

 * *Files 20% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 coverage = ">=7,<8.0"
 nose = ">=1.3,<2.0"
 nose-htmloutput = ">=0.1,<1.0"
 tox = ">=4.0<5.0"
 betamax = ">=0.8,<1.0"
 betamax-serializers = "~=0.2,<1.0"
 semver = ">=3.0,<4.0"
-gitwrapperlib = ">=1.0,<2.0"
+gitwrapperlib = ">=1.0.1,<2.0"
 twine = ">=4.0,<5.0"
 coloredlogs = ">=15.0,<16.0"
 emoji = ">=2.0,<3.0"
 toml = ">=0.1,<1.0"
 
 
 [packages]
```

### Comparing `gitwrapperlib-1.0.1/Pipfile.lock` & `gitwrapperlib-1.0.2/Pipfile.lock`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9786495271867612%*

 * *Differences: {"'_meta'": "{'hash': {'sha256': "*

 * *            "'4493901418e6af86722b8f9481acb9aa89b31adeecb88e23fd4a877a6d045f51'}}",*

 * * "'develop'": "{'gitwrapperlib': {'hashes': "*

 * *              "['sha256:20a8f0214bfcbcb56daf0e3ad4d8ab52e76c1d7b04989509416099776f05de35', "*

 * *              "'sha256:4bcb052f25298eb74e3f32e76ba402e699c7c3b61e2c2782ee820202f46c1b9e'], "*

 * *              "'version': '==1.0.1'}, 'cffi': OrderedDict([('hashes', "*

 * *              "['sha256:00a9ed42e88df81ffae7a8ab6d9356b371399b91dbdf0c3cb1e84c03a13aceb5' […]*

```diff
@@ -1,11 +1,11 @@
 {
     "_meta": {
         "hash": {
-            "sha256": "4fa2d6a765b3b81f226c7b04ae11d34ed18d1ad2d3ff44959d98a7b1ceb4a025"
+            "sha256": "4493901418e6af86722b8f9481acb9aa89b31adeecb88e23fd4a877a6d045f51"
         },
         "pipfile-spec": 6,
         "requires": {},
         "sources": [
             {
                 "name": "pypi",
                 "url": "https://pypi.python.org/simple",
@@ -92,14 +92,83 @@
             "hashes": [
                 "sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7",
                 "sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==2023.5.7"
         },
+        "cffi": {
+            "hashes": [
+                "sha256:00a9ed42e88df81ffae7a8ab6d9356b371399b91dbdf0c3cb1e84c03a13aceb5",
+                "sha256:03425bdae262c76aad70202debd780501fabeaca237cdfddc008987c0e0f59ef",
+                "sha256:04ed324bda3cda42b9b695d51bb7d54b680b9719cfab04227cdd1e04e5de3104",
+                "sha256:0e2642fe3142e4cc4af0799748233ad6da94c62a8bec3a6648bf8ee68b1c7426",
+                "sha256:173379135477dc8cac4bc58f45db08ab45d228b3363adb7af79436135d028405",
+                "sha256:198caafb44239b60e252492445da556afafc7d1e3ab7a1fb3f0584ef6d742375",
+                "sha256:1e74c6b51a9ed6589199c787bf5f9875612ca4a8a0785fb2d4a84429badaf22a",
+                "sha256:2012c72d854c2d03e45d06ae57f40d78e5770d252f195b93f581acf3ba44496e",
+                "sha256:21157295583fe8943475029ed5abdcf71eb3911894724e360acff1d61c1d54bc",
+                "sha256:2470043b93ff09bf8fb1d46d1cb756ce6132c54826661a32d4e4d132e1977adf",
+                "sha256:285d29981935eb726a4399badae8f0ffdff4f5050eaa6d0cfc3f64b857b77185",
+                "sha256:30d78fbc8ebf9c92c9b7823ee18eb92f2e6ef79b45ac84db507f52fbe3ec4497",
+                "sha256:320dab6e7cb2eacdf0e658569d2575c4dad258c0fcc794f46215e1e39f90f2c3",
+                "sha256:33ab79603146aace82c2427da5ca6e58f2b3f2fb5da893ceac0c42218a40be35",
+                "sha256:3548db281cd7d2561c9ad9984681c95f7b0e38881201e157833a2342c30d5e8c",
+                "sha256:3799aecf2e17cf585d977b780ce79ff0dc9b78d799fc694221ce814c2c19db83",
+                "sha256:39d39875251ca8f612b6f33e6b1195af86d1b3e60086068be9cc053aa4376e21",
+                "sha256:3b926aa83d1edb5aa5b427b4053dc420ec295a08e40911296b9eb1b6170f6cca",
+                "sha256:3bcde07039e586f91b45c88f8583ea7cf7a0770df3a1649627bf598332cb6984",
+                "sha256:3d08afd128ddaa624a48cf2b859afef385b720bb4b43df214f85616922e6a5ac",
+                "sha256:3eb6971dcff08619f8d91607cfc726518b6fa2a9eba42856be181c6d0d9515fd",
+                "sha256:40f4774f5a9d4f5e344f31a32b5096977b5d48560c5592e2f3d2c4374bd543ee",
+                "sha256:4289fc34b2f5316fbb762d75362931e351941fa95fa18789191b33fc4cf9504a",
+                "sha256:470c103ae716238bbe698d67ad020e1db9d9dba34fa5a899b5e21577e6d52ed2",
+                "sha256:4f2c9f67e9821cad2e5f480bc8d83b8742896f1242dba247911072d4fa94c192",
+                "sha256:50a74364d85fd319352182ef59c5c790484a336f6db772c1a9231f1c3ed0cbd7",
+                "sha256:54a2db7b78338edd780e7ef7f9f6c442500fb0d41a5a4ea24fff1c929d5af585",
+                "sha256:5635bd9cb9731e6d4a1132a498dd34f764034a8ce60cef4f5319c0541159392f",
+                "sha256:59c0b02d0a6c384d453fece7566d1c7e6b7bae4fc5874ef2ef46d56776d61c9e",
+                "sha256:5d598b938678ebf3c67377cdd45e09d431369c3b1a5b331058c338e201f12b27",
+                "sha256:5df2768244d19ab7f60546d0c7c63ce1581f7af8b5de3eb3004b9b6fc8a9f84b",
+                "sha256:5ef34d190326c3b1f822a5b7a45f6c4535e2f47ed06fec77d3d799c450b2651e",
+                "sha256:6975a3fac6bc83c4a65c9f9fcab9e47019a11d3d2cf7f3c0d03431bf145a941e",
+                "sha256:6c9a799e985904922a4d207a94eae35c78ebae90e128f0c4e521ce339396be9d",
+                "sha256:70df4e3b545a17496c9b3f41f5115e69a4f2e77e94e1d2a8e1070bc0c38c8a3c",
+                "sha256:7473e861101c9e72452f9bf8acb984947aa1661a7704553a9f6e4baa5ba64415",
+                "sha256:8102eaf27e1e448db915d08afa8b41d6c7ca7a04b7d73af6514df10a3e74bd82",
+                "sha256:87c450779d0914f2861b8526e035c5e6da0a3199d8f1add1a665e1cbc6fc6d02",
+                "sha256:8b7ee99e510d7b66cdb6c593f21c043c248537a32e0bedf02e01e9553a172314",
+                "sha256:91fc98adde3d7881af9b59ed0294046f3806221863722ba7d8d120c575314325",
+                "sha256:94411f22c3985acaec6f83c6df553f2dbe17b698cc7f8ae751ff2237d96b9e3c",
+                "sha256:98d85c6a2bef81588d9227dde12db8a7f47f639f4a17c9ae08e773aa9c697bf3",
+                "sha256:9ad5db27f9cabae298d151c85cf2bad1d359a1b9c686a275df03385758e2f914",
+                "sha256:a0b71b1b8fbf2b96e41c4d990244165e2c9be83d54962a9a1d118fd8657d2045",
+                "sha256:a0f100c8912c114ff53e1202d0078b425bee3649ae34d7b070e9697f93c5d52d",
+                "sha256:a591fe9e525846e4d154205572a029f653ada1a78b93697f3b5a8f1f2bc055b9",
+                "sha256:a5c84c68147988265e60416b57fc83425a78058853509c1b0629c180094904a5",
+                "sha256:a66d3508133af6e8548451b25058d5812812ec3798c886bf38ed24a98216fab2",
+                "sha256:a8c4917bd7ad33e8eb21e9a5bbba979b49d9a97acb3a803092cbc1133e20343c",
+                "sha256:b3bbeb01c2b273cca1e1e0c5df57f12dce9a4dd331b4fa1635b8bec26350bde3",
+                "sha256:cba9d6b9a7d64d4bd46167096fc9d2f835e25d7e4c121fb2ddfc6528fb0413b2",
+                "sha256:cc4d65aeeaa04136a12677d3dd0b1c0c94dc43abac5860ab33cceb42b801c1e8",
+                "sha256:ce4bcc037df4fc5e3d184794f27bdaab018943698f4ca31630bc7f84a7b69c6d",
+                "sha256:cec7d9412a9102bdc577382c3929b337320c4c4c4849f2c5cdd14d7368c5562d",
+                "sha256:d400bfb9a37b1351253cb402671cea7e89bdecc294e8016a707f6d1d8ac934f9",
+                "sha256:d61f4695e6c866a23a21acab0509af1cdfd2c013cf256bbf5b6b5e2695827162",
+                "sha256:db0fbb9c62743ce59a9ff687eb5f4afbe77e5e8403d6697f7446e5f609976f76",
+                "sha256:dd86c085fae2efd48ac91dd7ccffcfc0571387fe1193d33b6394db7ef31fe2a4",
+                "sha256:e00b098126fd45523dd056d2efba6c5a63b71ffe9f2bbe1a4fe1716e1d0c331e",
+                "sha256:e229a521186c75c8ad9490854fd8bbdd9a0c9aa3a524326b55be83b54d4e0ad9",
+                "sha256:e263d77ee3dd201c3a142934a086a4450861778baaeeb45db4591ef65550b0a6",
+                "sha256:ed9cb427ba5504c1dc15ede7d516b84757c3e3d7868ccc85121d9310d27eed0b",
+                "sha256:fa6693661a4c91757f4412306191b6dc88c1703f780c8234035eac011922bc01",
+                "sha256:fcd131dd944808b5bdb38e6f5b53013c5aa4f334c5cad0c72742f6eba4b73db0"
+            ],
+            "version": "==1.15.1"
+        },
         "chardet": {
             "hashes": [
                 "sha256:0d62712b956bc154f85fb0a266e2a3c5913c2967e00348701b32411d6def31e5",
                 "sha256:362777fb014af596ad31334fde1e8c327dfdb076e1960d1694662d46a6917ab9"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==5.1.0"
@@ -263,14 +332,39 @@
                 "sha256:f6951407391b639504e3b3be51b7ba5f3528adbf1a8ac3302b687ecababf929e",
                 "sha256:f75f7168ab25dd93110c8a8117a22450c19976afbc44234cbf71481094c1b850",
                 "sha256:fdec9e8cbf13a5bf63290fc6013d216a4c7232efb51548594ca3631a7f13c3a3"
             ],
             "index": "pypi",
             "version": "==7.2.7"
         },
+        "cryptography": {
+            "hashes": [
+                "sha256:059e348f9a3c1950937e1b5d7ba1f8e968508ab181e75fc32b879452f08356db",
+                "sha256:1a5472d40c8f8e91ff7a3d8ac6dfa363d8e3138b961529c996f3e2df0c7a411a",
+                "sha256:1a8e6c2de6fbbcc5e14fd27fb24414507cb3333198ea9ab1258d916f00bc3039",
+                "sha256:1fee5aacc7367487b4e22484d3c7e547992ed726d14864ee33c0176ae43b0d7c",
+                "sha256:5d092fdfedaec4cbbffbf98cddc915ba145313a6fdaab83c6e67f4e6c218e6f3",
+                "sha256:5f0ff6e18d13a3de56f609dd1fd11470918f770c6bd5d00d632076c727d35485",
+                "sha256:7bfc55a5eae8b86a287747053140ba221afc65eb06207bedf6e019b8934b477c",
+                "sha256:7fa01527046ca5facdf973eef2535a27fec4cb651e4daec4d043ef63f6ecd4ca",
+                "sha256:8dde71c4169ec5ccc1087bb7521d54251c016f126f922ab2dfe6649170a3b8c5",
+                "sha256:8f4ab7021127a9b4323537300a2acfb450124b2def3756f64dc3a3d2160ee4b5",
+                "sha256:948224d76c4b6457349d47c0c98657557f429b4e93057cf5a2f71d603e2fc3a3",
+                "sha256:9a6c7a3c87d595608a39980ebaa04d5a37f94024c9f24eb7d10262b92f739ddb",
+                "sha256:b46e37db3cc267b4dea1f56da7346c9727e1209aa98487179ee8ebed09d21e43",
+                "sha256:b4ceb5324b998ce2003bc17d519080b4ec8d5b7b70794cbd2836101406a9be31",
+                "sha256:cb33ccf15e89f7ed89b235cff9d49e2e62c6c981a6061c9c8bb47ed7951190bc",
+                "sha256:d198820aba55660b4d74f7b5fd1f17db3aa5eb3e6893b0a41b75e84e4f9e0e4b",
+                "sha256:d34579085401d3f49762d2f7d6634d6b6c2ae1242202e860f4d26b046e3a1006",
+                "sha256:eb8163f5e549a22888c18b0d53d6bb62a20510060a22fd5a995ec8a05268df8a",
+                "sha256:f73bff05db2a3e5974a6fd248af2566134d8981fd7ab012e5dd4ddb1d9a70699"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==41.0.1"
+        },
         "dill": {
             "hashes": [
                 "sha256:a07ffd2351b8c678dfc4a856a3005f8067aea51d6ba6c700796a4d9e280f39f0",
                 "sha256:e5db55f3687856d8fbdab002ed78544e1c4559a130302693d839dfe8f93f2373"
             ],
             "markers": "python_version < '3.11'",
             "version": "==0.3.6"
@@ -341,18 +435,19 @@
                 "sha256:f04893614f6aa713a60cbbe1e6a97403ef633103cdd0ef5eb6efe0deb98dbe8d"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==3.1.31"
         },
         "gitwrapperlib": {
             "hashes": [
-                "sha256:3174bcc0de3fa70f78067cb2bc60a5c9820442d78594fb345bdd56740f64073a"
+                "sha256:20a8f0214bfcbcb56daf0e3ad4d8ab52e76c1d7b04989509416099776f05de35",
+                "sha256:4bcb052f25298eb74e3f32e76ba402e699c7c3b61e2c2782ee820202f46c1b9e"
             ],
             "index": "pypi",
-            "version": "==1.0.0"
+            "version": "==1.0.1"
         },
         "humanfriendly": {
             "hashes": [
                 "sha256:1697e1a8a8f550fd43c2865cd84542fc175a61dcb779b6fee18cf6b6ccba1477",
                 "sha256:6b0b831ce8f15f7300721aa49829fc4e83921a9a301cc7f606be6686a2288ddc"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
@@ -394,14 +489,22 @@
             "hashes": [
                 "sha256:2353de3288bc6b82120752201c6b1c1a14b058267fa424ed5ce5984e3b922158",
                 "sha256:89559fa5c1d3c34eff6f631ad80bb21f378dbcbb35dd161fd2c6b93f5be2f98a"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==3.2.3"
         },
+        "jeepney": {
+            "hashes": [
+                "sha256:5efe48d255973902f6badc3ce55e2aa6c5c3b3bc642059ef3a91247bcfcc5806",
+                "sha256:c0a454ad016ca575060802ee4d590dd912e35c122fa04e70306de3d076cce755"
+            ],
+            "markers": "sys_platform == 'linux'",
+            "version": "==0.8.0"
+        },
         "jinja2": {
             "hashes": [
                 "sha256:31351a702a408a9e7595a8fc6150fc3f43bb6bf7e319770cbc0db9df9437e852",
                 "sha256:6088930bfe239f0e6710546ab9c19c9ef35e29792895fed6e6e31a023a182a61"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==3.1.2"
@@ -612,14 +715,21 @@
             "hashes": [
                 "sha256:2c9607871d58c76354b697b42f5d57e1ada7d261c261efac224b664affdc5785",
                 "sha256:d1735fc58b418fd7c5f658d28d943854f8a849b01a5d0a1e6f3f3fdd0166804b"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==2.9.1"
         },
+        "pycparser": {
+            "hashes": [
+                "sha256:8ee45429555515e1f6b185e78100aea234072576aa43ab53aefcae078162fca9",
+                "sha256:e644fdec12f7872f86c58ff790da456218b10f863970249516d60a5eaca77206"
+            ],
+            "version": "==2.21"
+        },
         "pydocstyle": {
             "hashes": [
                 "sha256:118762d452a49d6b05e194ef344a55822987a462831ade91ec5c06fd2169d019",
                 "sha256:7ce43f0c0ac87b07494eb9c0b462c0b73e6ff276807f204d6b53edc72b7e44e1"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==6.3.0"
@@ -773,14 +883,22 @@
             "hashes": [
                 "sha256:8f87bc7ee54675732fa66a05ebfe489e27264caeeff3728c945d25971b6485ec",
                 "sha256:d653d6bccede5844304c605d5aac802c7cf9621efd700b46c7ec2b51ea914898"
             ],
             "markers": "python_full_version >= '3.7.0'",
             "version": "==13.4.2"
         },
+        "secretstorage": {
+            "hashes": [
+                "sha256:2403533ef369eca6d2ba81718576c5e0f564d5cca1b58f73a8b23e7d4eeebd77",
+                "sha256:f356e6628222568e3af06f2eba8df495efa13b3b63081dafd4f7d9a7b7bc9f99"
+            ],
+            "markers": "sys_platform == 'linux'",
+            "version": "==3.3.3"
+        },
         "semver": {
             "hashes": [
                 "sha256:94df43924c4521ec7d307fc86da1531db6c2c33d9d5cdc3e64cca0eb68569269",
                 "sha256:ab4f69fb1d1ecfb5d81f96411403d7a611fa788c45d252cf5b408025df3ab6ce"
             ],
             "index": "pypi",
             "version": "==3.0.0"
@@ -788,14 +906,23 @@
         "setoptconf-tmp": {
             "hashes": [
                 "sha256:76035d5cd1593d38b9056ae12d460eca3aaa34ad05c315b69145e138ba80a745",
                 "sha256:e0480addd11347ba52f762f3c4d8afa3e10ad0affbc53e3ffddc0ca5f27d5778"
             ],
             "version": "==0.3.1"
         },
+        "sh": {
+            "hashes": [
+                "sha256:14265a4cd1622429edcf300292ec98193530fb143fe642b3437024eca9bee8c5",
+                "sha256:a18920f0839991bc9dfddb6dcc006c360b1064ba96257359f0ea356e9fa75a60"
+            ],
+            "index": "pypi",
+            "markers": "sys_platform != 'win32'",
+            "version": "==2.0.4"
+        },
         "six": {
             "hashes": [
                 "sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926",
                 "sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
             "version": "==1.16.0"
```

### Comparing `gitwrapperlib-1.0.1/README.rst` & `gitwrapperlib-1.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `gitwrapperlib-1.0.1/USAGE.rst` & `gitwrapperlib-1.0.2/USAGE.rst`

 * *Files identical despite different names*

### Comparing `gitwrapperlib-1.0.1/dev-requirements.txt` & `gitwrapperlib-1.0.2/dev-requirements.txt`

 * *Files 2% similar despite different names*

```diff
@@ -13,12 +13,12 @@
 coverage>=7.2.7
 nose>=1.3.7
 nose-htmloutput>=0.6.0
 tox>=4.6.0
 betamax>=0.8.1
 betamax-serializers~=0.2.1
 semver>=3.0.0
-gitwrapperlib>=1.0.0
+gitwrapperlib>=1.0.1
 twine>=4.0.2
 coloredlogs>=15.0.1
 emoji>=2.5.0
 toml>=0.10.2
```

### Comparing `gitwrapperlib-1.0.1/docs/Makefile` & `gitwrapperlib-1.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `gitwrapperlib-1.0.1/docs/conf.py` & `gitwrapperlib-1.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `gitwrapperlib-1.0.1/docs/index.rst` & `gitwrapperlib-1.0.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `gitwrapperlib-1.0.1/gitwrapperlib/CONTRIBUTING.rst` & `gitwrapperlib-1.0.2/gitwrapperlib/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `gitwrapperlib-1.0.1/gitwrapperlib/HISTORY.rst` & `gitwrapperlib-1.0.2/gitwrapperlib/HISTORY.rst`

 * *Files 12% similar despite different names*

```diff
@@ -51,7 +51,13 @@
 * Removed references to master branch and implemented default remote retrieval, courtesy of Sten Spans <sspans@schubergphilis.com>
 
 
 1.0.1 (13-06-2023)
 ------------------
 
 * Bump dependencies and update pipeline to python 3.9.
+
+
+1.0.2 (13-06-2023)
+------------------
+
+* Bump dependencies.
```

### Comparing `gitwrapperlib-1.0.1/gitwrapperlib/LICENSE` & `gitwrapperlib-1.0.2/gitwrapperlib/LICENSE`

 * *Files identical despite different names*

### Comparing `gitwrapperlib-1.0.1/gitwrapperlib/Pipfile` & `gitwrapperlib-1.0.2/gitwrapperlib/Pipfile`

 * *Files 20% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 coverage = ">=7,<8.0"
 nose = ">=1.3,<2.0"
 nose-htmloutput = ">=0.1,<1.0"
 tox = ">=4.0<5.0"
 betamax = ">=0.8,<1.0"
 betamax-serializers = "~=0.2,<1.0"
 semver = ">=3.0,<4.0"
-gitwrapperlib = ">=1.0,<2.0"
+gitwrapperlib = ">=1.0.1,<2.0"
 twine = ">=4.0,<5.0"
 coloredlogs = ">=15.0,<16.0"
 emoji = ">=2.0,<3.0"
 toml = ">=0.1,<1.0"
 
 
 [packages]
```

### Comparing `gitwrapperlib-1.0.1/gitwrapperlib/Pipfile.lock` & `gitwrapperlib-1.0.2/gitwrapperlib/Pipfile.lock`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9786495271867612%*

 * *Differences: {"'_meta'": "{'hash': {'sha256': "*

 * *            "'4493901418e6af86722b8f9481acb9aa89b31adeecb88e23fd4a877a6d045f51'}}",*

 * * "'develop'": "{'gitwrapperlib': {'hashes': "*

 * *              "['sha256:20a8f0214bfcbcb56daf0e3ad4d8ab52e76c1d7b04989509416099776f05de35', "*

 * *              "'sha256:4bcb052f25298eb74e3f32e76ba402e699c7c3b61e2c2782ee820202f46c1b9e'], "*

 * *              "'version': '==1.0.1'}, 'cffi': OrderedDict([('hashes', "*

 * *              "['sha256:00a9ed42e88df81ffae7a8ab6d9356b371399b91dbdf0c3cb1e84c03a13aceb5' […]*

```diff
@@ -1,11 +1,11 @@
 {
     "_meta": {
         "hash": {
-            "sha256": "4fa2d6a765b3b81f226c7b04ae11d34ed18d1ad2d3ff44959d98a7b1ceb4a025"
+            "sha256": "4493901418e6af86722b8f9481acb9aa89b31adeecb88e23fd4a877a6d045f51"
         },
         "pipfile-spec": 6,
         "requires": {},
         "sources": [
             {
                 "name": "pypi",
                 "url": "https://pypi.python.org/simple",
@@ -92,14 +92,83 @@
             "hashes": [
                 "sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7",
                 "sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==2023.5.7"
         },
+        "cffi": {
+            "hashes": [
+                "sha256:00a9ed42e88df81ffae7a8ab6d9356b371399b91dbdf0c3cb1e84c03a13aceb5",
+                "sha256:03425bdae262c76aad70202debd780501fabeaca237cdfddc008987c0e0f59ef",
+                "sha256:04ed324bda3cda42b9b695d51bb7d54b680b9719cfab04227cdd1e04e5de3104",
+                "sha256:0e2642fe3142e4cc4af0799748233ad6da94c62a8bec3a6648bf8ee68b1c7426",
+                "sha256:173379135477dc8cac4bc58f45db08ab45d228b3363adb7af79436135d028405",
+                "sha256:198caafb44239b60e252492445da556afafc7d1e3ab7a1fb3f0584ef6d742375",
+                "sha256:1e74c6b51a9ed6589199c787bf5f9875612ca4a8a0785fb2d4a84429badaf22a",
+                "sha256:2012c72d854c2d03e45d06ae57f40d78e5770d252f195b93f581acf3ba44496e",
+                "sha256:21157295583fe8943475029ed5abdcf71eb3911894724e360acff1d61c1d54bc",
+                "sha256:2470043b93ff09bf8fb1d46d1cb756ce6132c54826661a32d4e4d132e1977adf",
+                "sha256:285d29981935eb726a4399badae8f0ffdff4f5050eaa6d0cfc3f64b857b77185",
+                "sha256:30d78fbc8ebf9c92c9b7823ee18eb92f2e6ef79b45ac84db507f52fbe3ec4497",
+                "sha256:320dab6e7cb2eacdf0e658569d2575c4dad258c0fcc794f46215e1e39f90f2c3",
+                "sha256:33ab79603146aace82c2427da5ca6e58f2b3f2fb5da893ceac0c42218a40be35",
+                "sha256:3548db281cd7d2561c9ad9984681c95f7b0e38881201e157833a2342c30d5e8c",
+                "sha256:3799aecf2e17cf585d977b780ce79ff0dc9b78d799fc694221ce814c2c19db83",
+                "sha256:39d39875251ca8f612b6f33e6b1195af86d1b3e60086068be9cc053aa4376e21",
+                "sha256:3b926aa83d1edb5aa5b427b4053dc420ec295a08e40911296b9eb1b6170f6cca",
+                "sha256:3bcde07039e586f91b45c88f8583ea7cf7a0770df3a1649627bf598332cb6984",
+                "sha256:3d08afd128ddaa624a48cf2b859afef385b720bb4b43df214f85616922e6a5ac",
+                "sha256:3eb6971dcff08619f8d91607cfc726518b6fa2a9eba42856be181c6d0d9515fd",
+                "sha256:40f4774f5a9d4f5e344f31a32b5096977b5d48560c5592e2f3d2c4374bd543ee",
+                "sha256:4289fc34b2f5316fbb762d75362931e351941fa95fa18789191b33fc4cf9504a",
+                "sha256:470c103ae716238bbe698d67ad020e1db9d9dba34fa5a899b5e21577e6d52ed2",
+                "sha256:4f2c9f67e9821cad2e5f480bc8d83b8742896f1242dba247911072d4fa94c192",
+                "sha256:50a74364d85fd319352182ef59c5c790484a336f6db772c1a9231f1c3ed0cbd7",
+                "sha256:54a2db7b78338edd780e7ef7f9f6c442500fb0d41a5a4ea24fff1c929d5af585",
+                "sha256:5635bd9cb9731e6d4a1132a498dd34f764034a8ce60cef4f5319c0541159392f",
+                "sha256:59c0b02d0a6c384d453fece7566d1c7e6b7bae4fc5874ef2ef46d56776d61c9e",
+                "sha256:5d598b938678ebf3c67377cdd45e09d431369c3b1a5b331058c338e201f12b27",
+                "sha256:5df2768244d19ab7f60546d0c7c63ce1581f7af8b5de3eb3004b9b6fc8a9f84b",
+                "sha256:5ef34d190326c3b1f822a5b7a45f6c4535e2f47ed06fec77d3d799c450b2651e",
+                "sha256:6975a3fac6bc83c4a65c9f9fcab9e47019a11d3d2cf7f3c0d03431bf145a941e",
+                "sha256:6c9a799e985904922a4d207a94eae35c78ebae90e128f0c4e521ce339396be9d",
+                "sha256:70df4e3b545a17496c9b3f41f5115e69a4f2e77e94e1d2a8e1070bc0c38c8a3c",
+                "sha256:7473e861101c9e72452f9bf8acb984947aa1661a7704553a9f6e4baa5ba64415",
+                "sha256:8102eaf27e1e448db915d08afa8b41d6c7ca7a04b7d73af6514df10a3e74bd82",
+                "sha256:87c450779d0914f2861b8526e035c5e6da0a3199d8f1add1a665e1cbc6fc6d02",
+                "sha256:8b7ee99e510d7b66cdb6c593f21c043c248537a32e0bedf02e01e9553a172314",
+                "sha256:91fc98adde3d7881af9b59ed0294046f3806221863722ba7d8d120c575314325",
+                "sha256:94411f22c3985acaec6f83c6df553f2dbe17b698cc7f8ae751ff2237d96b9e3c",
+                "sha256:98d85c6a2bef81588d9227dde12db8a7f47f639f4a17c9ae08e773aa9c697bf3",
+                "sha256:9ad5db27f9cabae298d151c85cf2bad1d359a1b9c686a275df03385758e2f914",
+                "sha256:a0b71b1b8fbf2b96e41c4d990244165e2c9be83d54962a9a1d118fd8657d2045",
+                "sha256:a0f100c8912c114ff53e1202d0078b425bee3649ae34d7b070e9697f93c5d52d",
+                "sha256:a591fe9e525846e4d154205572a029f653ada1a78b93697f3b5a8f1f2bc055b9",
+                "sha256:a5c84c68147988265e60416b57fc83425a78058853509c1b0629c180094904a5",
+                "sha256:a66d3508133af6e8548451b25058d5812812ec3798c886bf38ed24a98216fab2",
+                "sha256:a8c4917bd7ad33e8eb21e9a5bbba979b49d9a97acb3a803092cbc1133e20343c",
+                "sha256:b3bbeb01c2b273cca1e1e0c5df57f12dce9a4dd331b4fa1635b8bec26350bde3",
+                "sha256:cba9d6b9a7d64d4bd46167096fc9d2f835e25d7e4c121fb2ddfc6528fb0413b2",
+                "sha256:cc4d65aeeaa04136a12677d3dd0b1c0c94dc43abac5860ab33cceb42b801c1e8",
+                "sha256:ce4bcc037df4fc5e3d184794f27bdaab018943698f4ca31630bc7f84a7b69c6d",
+                "sha256:cec7d9412a9102bdc577382c3929b337320c4c4c4849f2c5cdd14d7368c5562d",
+                "sha256:d400bfb9a37b1351253cb402671cea7e89bdecc294e8016a707f6d1d8ac934f9",
+                "sha256:d61f4695e6c866a23a21acab0509af1cdfd2c013cf256bbf5b6b5e2695827162",
+                "sha256:db0fbb9c62743ce59a9ff687eb5f4afbe77e5e8403d6697f7446e5f609976f76",
+                "sha256:dd86c085fae2efd48ac91dd7ccffcfc0571387fe1193d33b6394db7ef31fe2a4",
+                "sha256:e00b098126fd45523dd056d2efba6c5a63b71ffe9f2bbe1a4fe1716e1d0c331e",
+                "sha256:e229a521186c75c8ad9490854fd8bbdd9a0c9aa3a524326b55be83b54d4e0ad9",
+                "sha256:e263d77ee3dd201c3a142934a086a4450861778baaeeb45db4591ef65550b0a6",
+                "sha256:ed9cb427ba5504c1dc15ede7d516b84757c3e3d7868ccc85121d9310d27eed0b",
+                "sha256:fa6693661a4c91757f4412306191b6dc88c1703f780c8234035eac011922bc01",
+                "sha256:fcd131dd944808b5bdb38e6f5b53013c5aa4f334c5cad0c72742f6eba4b73db0"
+            ],
+            "version": "==1.15.1"
+        },
         "chardet": {
             "hashes": [
                 "sha256:0d62712b956bc154f85fb0a266e2a3c5913c2967e00348701b32411d6def31e5",
                 "sha256:362777fb014af596ad31334fde1e8c327dfdb076e1960d1694662d46a6917ab9"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==5.1.0"
@@ -263,14 +332,39 @@
                 "sha256:f6951407391b639504e3b3be51b7ba5f3528adbf1a8ac3302b687ecababf929e",
                 "sha256:f75f7168ab25dd93110c8a8117a22450c19976afbc44234cbf71481094c1b850",
                 "sha256:fdec9e8cbf13a5bf63290fc6013d216a4c7232efb51548594ca3631a7f13c3a3"
             ],
             "index": "pypi",
             "version": "==7.2.7"
         },
+        "cryptography": {
+            "hashes": [
+                "sha256:059e348f9a3c1950937e1b5d7ba1f8e968508ab181e75fc32b879452f08356db",
+                "sha256:1a5472d40c8f8e91ff7a3d8ac6dfa363d8e3138b961529c996f3e2df0c7a411a",
+                "sha256:1a8e6c2de6fbbcc5e14fd27fb24414507cb3333198ea9ab1258d916f00bc3039",
+                "sha256:1fee5aacc7367487b4e22484d3c7e547992ed726d14864ee33c0176ae43b0d7c",
+                "sha256:5d092fdfedaec4cbbffbf98cddc915ba145313a6fdaab83c6e67f4e6c218e6f3",
+                "sha256:5f0ff6e18d13a3de56f609dd1fd11470918f770c6bd5d00d632076c727d35485",
+                "sha256:7bfc55a5eae8b86a287747053140ba221afc65eb06207bedf6e019b8934b477c",
+                "sha256:7fa01527046ca5facdf973eef2535a27fec4cb651e4daec4d043ef63f6ecd4ca",
+                "sha256:8dde71c4169ec5ccc1087bb7521d54251c016f126f922ab2dfe6649170a3b8c5",
+                "sha256:8f4ab7021127a9b4323537300a2acfb450124b2def3756f64dc3a3d2160ee4b5",
+                "sha256:948224d76c4b6457349d47c0c98657557f429b4e93057cf5a2f71d603e2fc3a3",
+                "sha256:9a6c7a3c87d595608a39980ebaa04d5a37f94024c9f24eb7d10262b92f739ddb",
+                "sha256:b46e37db3cc267b4dea1f56da7346c9727e1209aa98487179ee8ebed09d21e43",
+                "sha256:b4ceb5324b998ce2003bc17d519080b4ec8d5b7b70794cbd2836101406a9be31",
+                "sha256:cb33ccf15e89f7ed89b235cff9d49e2e62c6c981a6061c9c8bb47ed7951190bc",
+                "sha256:d198820aba55660b4d74f7b5fd1f17db3aa5eb3e6893b0a41b75e84e4f9e0e4b",
+                "sha256:d34579085401d3f49762d2f7d6634d6b6c2ae1242202e860f4d26b046e3a1006",
+                "sha256:eb8163f5e549a22888c18b0d53d6bb62a20510060a22fd5a995ec8a05268df8a",
+                "sha256:f73bff05db2a3e5974a6fd248af2566134d8981fd7ab012e5dd4ddb1d9a70699"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==41.0.1"
+        },
         "dill": {
             "hashes": [
                 "sha256:a07ffd2351b8c678dfc4a856a3005f8067aea51d6ba6c700796a4d9e280f39f0",
                 "sha256:e5db55f3687856d8fbdab002ed78544e1c4559a130302693d839dfe8f93f2373"
             ],
             "markers": "python_version < '3.11'",
             "version": "==0.3.6"
@@ -341,18 +435,19 @@
                 "sha256:f04893614f6aa713a60cbbe1e6a97403ef633103cdd0ef5eb6efe0deb98dbe8d"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==3.1.31"
         },
         "gitwrapperlib": {
             "hashes": [
-                "sha256:3174bcc0de3fa70f78067cb2bc60a5c9820442d78594fb345bdd56740f64073a"
+                "sha256:20a8f0214bfcbcb56daf0e3ad4d8ab52e76c1d7b04989509416099776f05de35",
+                "sha256:4bcb052f25298eb74e3f32e76ba402e699c7c3b61e2c2782ee820202f46c1b9e"
             ],
             "index": "pypi",
-            "version": "==1.0.0"
+            "version": "==1.0.1"
         },
         "humanfriendly": {
             "hashes": [
                 "sha256:1697e1a8a8f550fd43c2865cd84542fc175a61dcb779b6fee18cf6b6ccba1477",
                 "sha256:6b0b831ce8f15f7300721aa49829fc4e83921a9a301cc7f606be6686a2288ddc"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
@@ -394,14 +489,22 @@
             "hashes": [
                 "sha256:2353de3288bc6b82120752201c6b1c1a14b058267fa424ed5ce5984e3b922158",
                 "sha256:89559fa5c1d3c34eff6f631ad80bb21f378dbcbb35dd161fd2c6b93f5be2f98a"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==3.2.3"
         },
+        "jeepney": {
+            "hashes": [
+                "sha256:5efe48d255973902f6badc3ce55e2aa6c5c3b3bc642059ef3a91247bcfcc5806",
+                "sha256:c0a454ad016ca575060802ee4d590dd912e35c122fa04e70306de3d076cce755"
+            ],
+            "markers": "sys_platform == 'linux'",
+            "version": "==0.8.0"
+        },
         "jinja2": {
             "hashes": [
                 "sha256:31351a702a408a9e7595a8fc6150fc3f43bb6bf7e319770cbc0db9df9437e852",
                 "sha256:6088930bfe239f0e6710546ab9c19c9ef35e29792895fed6e6e31a023a182a61"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==3.1.2"
@@ -612,14 +715,21 @@
             "hashes": [
                 "sha256:2c9607871d58c76354b697b42f5d57e1ada7d261c261efac224b664affdc5785",
                 "sha256:d1735fc58b418fd7c5f658d28d943854f8a849b01a5d0a1e6f3f3fdd0166804b"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==2.9.1"
         },
+        "pycparser": {
+            "hashes": [
+                "sha256:8ee45429555515e1f6b185e78100aea234072576aa43ab53aefcae078162fca9",
+                "sha256:e644fdec12f7872f86c58ff790da456218b10f863970249516d60a5eaca77206"
+            ],
+            "version": "==2.21"
+        },
         "pydocstyle": {
             "hashes": [
                 "sha256:118762d452a49d6b05e194ef344a55822987a462831ade91ec5c06fd2169d019",
                 "sha256:7ce43f0c0ac87b07494eb9c0b462c0b73e6ff276807f204d6b53edc72b7e44e1"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==6.3.0"
@@ -773,14 +883,22 @@
             "hashes": [
                 "sha256:8f87bc7ee54675732fa66a05ebfe489e27264caeeff3728c945d25971b6485ec",
                 "sha256:d653d6bccede5844304c605d5aac802c7cf9621efd700b46c7ec2b51ea914898"
             ],
             "markers": "python_full_version >= '3.7.0'",
             "version": "==13.4.2"
         },
+        "secretstorage": {
+            "hashes": [
+                "sha256:2403533ef369eca6d2ba81718576c5e0f564d5cca1b58f73a8b23e7d4eeebd77",
+                "sha256:f356e6628222568e3af06f2eba8df495efa13b3b63081dafd4f7d9a7b7bc9f99"
+            ],
+            "markers": "sys_platform == 'linux'",
+            "version": "==3.3.3"
+        },
         "semver": {
             "hashes": [
                 "sha256:94df43924c4521ec7d307fc86da1531db6c2c33d9d5cdc3e64cca0eb68569269",
                 "sha256:ab4f69fb1d1ecfb5d81f96411403d7a611fa788c45d252cf5b408025df3ab6ce"
             ],
             "index": "pypi",
             "version": "==3.0.0"
@@ -788,14 +906,23 @@
         "setoptconf-tmp": {
             "hashes": [
                 "sha256:76035d5cd1593d38b9056ae12d460eca3aaa34ad05c315b69145e138ba80a745",
                 "sha256:e0480addd11347ba52f762f3c4d8afa3e10ad0affbc53e3ffddc0ca5f27d5778"
             ],
             "version": "==0.3.1"
         },
+        "sh": {
+            "hashes": [
+                "sha256:14265a4cd1622429edcf300292ec98193530fb143fe642b3437024eca9bee8c5",
+                "sha256:a18920f0839991bc9dfddb6dcc006c360b1064ba96257359f0ea356e9fa75a60"
+            ],
+            "index": "pypi",
+            "markers": "sys_platform != 'win32'",
+            "version": "==2.0.4"
+        },
         "six": {
             "hashes": [
                 "sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926",
                 "sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
             "version": "==1.16.0"
```

### Comparing `gitwrapperlib-1.0.1/gitwrapperlib/README.rst` & `gitwrapperlib-1.0.2/gitwrapperlib/README.rst`

 * *Files identical despite different names*

### Comparing `gitwrapperlib-1.0.1/gitwrapperlib/USAGE.rst` & `gitwrapperlib-1.0.2/gitwrapperlib/USAGE.rst`

 * *Files identical despite different names*

### Comparing `gitwrapperlib-1.0.1/gitwrapperlib/__init__.py` & `gitwrapperlib-1.0.2/gitwrapperlib/__init__.py`

 * *Files identical despite different names*

### Comparing `gitwrapperlib-1.0.1/gitwrapperlib/_version.py` & `gitwrapperlib-1.0.2/gitwrapperlib/_version.py`

 * *Files identical despite different names*

### Comparing `gitwrapperlib-1.0.1/gitwrapperlib/dev-requirements.txt` & `gitwrapperlib-1.0.2/gitwrapperlib/dev-requirements.txt`

 * *Files 2% similar despite different names*

```diff
@@ -13,12 +13,12 @@
 coverage>=7.2.7
 nose>=1.3.7
 nose-htmloutput>=0.6.0
 tox>=4.6.0
 betamax>=0.8.1
 betamax-serializers~=0.2.1
 semver>=3.0.0
-gitwrapperlib>=1.0.0
+gitwrapperlib>=1.0.1
 twine>=4.0.2
 coloredlogs>=15.0.1
 emoji>=2.5.0
 toml>=0.10.2
```

### Comparing `gitwrapperlib-1.0.1/gitwrapperlib/gitwrapperlib.py` & `gitwrapperlib-1.0.2/gitwrapperlib/gitwrapperlib.py`

 * *Files identical despite different names*

### Comparing `gitwrapperlib-1.0.1/gitwrapperlib/gitwrapperlibexceptions.py` & `gitwrapperlib-1.0.2/gitwrapperlib/gitwrapperlibexceptions.py`

 * *Files identical despite different names*

### Comparing `gitwrapperlib-1.0.1/gitwrapperlib.egg-info/PKG-INFO` & `gitwrapperlib-1.0.2/gitwrapperlib.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitwrapperlib
-Version: 1.0.1
+Version: 1.0.2
 Summary: A lightweight wrapper around the git command using sh module.
 Home-page: https://github.com/costastf/gitwrapperlib
 Author: Costas Tyfoxylos
 Author-email: costas.tyf@gmail.com
 License: MIT
 Keywords: gitwrapperlib git python sh
 Classifier: Development Status :: 4 - Beta
@@ -138,7 +138,13 @@
 * Removed references to master branch and implemented default remote retrieval, courtesy of Sten Spans <sspans@schubergphilis.com>
 
 
 1.0.1 (13-06-2023)
 ------------------
 
 * Bump dependencies and update pipeline to python 3.9.
+
+
+1.0.2 (13-06-2023)
+------------------
+
+* Bump dependencies.
```

### Comparing `gitwrapperlib-1.0.1/setup.py` & `gitwrapperlib-1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `gitwrapperlib-1.0.1/tests/test_gitwrapperlib.py` & `gitwrapperlib-1.0.2/tests/test_gitwrapperlib.py`

 * *Files identical despite different names*

