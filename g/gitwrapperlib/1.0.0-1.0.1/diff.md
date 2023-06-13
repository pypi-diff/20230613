# Comparing `tmp/gitwrapperlib-1.0.0.tar.gz` & `tmp/gitwrapperlib-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gitwrapperlib-1.0.0.tar", last modified: Mon Mar 21 13:36:16 2022, max compression
+gzip compressed data, was "gitwrapperlib-1.0.1.tar", last modified: Tue Jun 13 11:06:09 2023, max compression
```

## Comparing `gitwrapperlib-1.0.0.tar` & `gitwrapperlib-1.0.1.tar`

### file list

```diff
@@ -1,49 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 13:36:16.000000 gitwrapperlib-1.0.0/
--rwxr-xr-x   0 runner    (1001) docker     (121)        5 2022-03-21 13:34:18.000000 gitwrapperlib-1.0.0/.VERSION
--rwxr-xr-x   0 runner    (1001) docker     (121)      171 2022-03-21 13:34:18.000000 gitwrapperlib-1.0.0/AUTHORS.rst
--rwxr-xr-x   0 runner    (1001) docker     (121)     1268 2022-03-21 13:34:18.000000 gitwrapperlib-1.0.0/CONTRIBUTING.rst
--rwxr-xr-x   0 runner    (1001) docker     (121)      741 2022-03-21 13:34:18.000000 gitwrapperlib-1.0.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1063 2022-03-21 13:34:18.000000 gitwrapperlib-1.0.0/LICENSE
--rwxr-xr-x   0 runner    (1001) docker     (121)      400 2022-03-21 13:34:18.000000 gitwrapperlib-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3641 2022-03-21 13:36:16.000000 gitwrapperlib-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      577 2022-03-21 13:34:18.000000 gitwrapperlib-1.0.0/Pipfile
--rw-r--r--   0 runner    (1001) docker     (121)    45616 2022-03-21 13:36:14.000000 gitwrapperlib-1.0.0/Pipfile.lock
--rwxr-xr-x   0 runner    (1001) docker     (121)     2323 2022-03-21 13:34:18.000000 gitwrapperlib-1.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      913 2022-03-21 13:34:18.000000 gitwrapperlib-1.0.0/USAGE.rst
--rw-r--r--   0 runner    (1001) docker     (121)      602 2022-03-21 13:36:14.000000 gitwrapperlib-1.0.0/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 13:36:16.000000 gitwrapperlib-1.0.0/docs/
--rwxr-xr-x   0 runner    (1001) docker     (121)     6790 2022-03-21 13:34:18.000000 gitwrapperlib-1.0.0/docs/Makefile
--rwxr-xr-x   0 runner    (1001) docker     (121)       28 2022-03-21 13:34:18.000000 gitwrapperlib-1.0.0/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (121)     8964 2022-03-21 13:34:18.000000 gitwrapperlib-1.0.0/docs/conf.py
--rwxr-xr-x   0 runner    (1001) docker     (121)       33 2022-03-21 13:34:18.000000 gitwrapperlib-1.0.0/docs/contributing.rst
--rwxr-xr-x   0 runner    (1001) docker     (121)       28 2022-03-21 13:34:18.000000 gitwrapperlib-1.0.0/docs/history.rst
--rwxr-xr-x   0 runner    (1001) docker     (121)      513 2022-03-21 13:34:18.000000 gitwrapperlib-1.0.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-03-21 13:34:18.000000 gitwrapperlib-1.0.0/docs/installation.rst
--rwxr-xr-x   0 runner    (1001) docker     (121)       27 2022-03-21 13:34:18.000000 gitwrapperlib-1.0.0/docs/readme.rst
--rwxr-xr-x   0 runner    (1001) docker     (121)       26 2022-03-21 13:34:18.000000 gitwrapperlib-1.0.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 13:36:16.000000 gitwrapperlib-1.0.0/gitwrapperlib/
--rwxr-xr-x   0 runner    (1001) docker     (121)        5 2022-03-21 13:36:14.000000 gitwrapperlib-1.0.0/gitwrapperlib/.VERSION
--rwxr-xr-x   0 runner    (1001) docker     (121)      171 2022-03-21 13:36:14.000000 gitwrapperlib-1.0.0/gitwrapperlib/AUTHORS.rst
--rwxr-xr-x   0 runner    (1001) docker     (121)     1268 2022-03-21 13:36:14.000000 gitwrapperlib-1.0.0/gitwrapperlib/CONTRIBUTING.rst
--rwxr-xr-x   0 runner    (1001) docker     (121)      741 2022-03-21 13:36:14.000000 gitwrapperlib-1.0.0/gitwrapperlib/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1063 2022-03-21 13:36:14.000000 gitwrapperlib-1.0.0/gitwrapperlib/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      577 2022-03-21 13:36:14.000000 gitwrapperlib-1.0.0/gitwrapperlib/Pipfile
--rw-r--r--   0 runner    (1001) docker     (121)    45616 2022-03-21 13:36:14.000000 gitwrapperlib-1.0.0/gitwrapperlib/Pipfile.lock
--rwxr-xr-x   0 runner    (1001) docker     (121)     2323 2022-03-21 13:36:14.000000 gitwrapperlib-1.0.0/gitwrapperlib/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      913 2022-03-21 13:36:14.000000 gitwrapperlib-1.0.0/gitwrapperlib/USAGE.rst
--rwxr-xr-x   0 runner    (1001) docker     (121)     1961 2022-03-21 13:34:18.000000 gitwrapperlib-1.0.0/gitwrapperlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2090 2022-03-21 13:34:18.000000 gitwrapperlib-1.0.0/gitwrapperlib/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)      602 2022-03-21 13:36:14.000000 gitwrapperlib-1.0.0/gitwrapperlib/dev-requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (121)     7076 2022-03-21 13:34:18.000000 gitwrapperlib-1.0.0/gitwrapperlib/gitwrapperlib.py
--rw-r--r--   0 runner    (1001) docker     (121)     1985 2022-03-21 13:34:18.000000 gitwrapperlib-1.0.0/gitwrapperlib/gitwrapperlibexceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)      408 2022-03-21 13:36:14.000000 gitwrapperlib-1.0.0/gitwrapperlib/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 13:36:16.000000 gitwrapperlib-1.0.0/gitwrapperlib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3641 2022-03-21 13:36:15.000000 gitwrapperlib-1.0.0/gitwrapperlib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      955 2022-03-21 13:36:16.000000 gitwrapperlib-1.0.0/gitwrapperlib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-21 13:36:15.000000 gitwrapperlib-1.0.0/gitwrapperlib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-21 13:36:15.000000 gitwrapperlib-1.0.0/gitwrapperlib.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-03-21 13:36:15.000000 gitwrapperlib-1.0.0/gitwrapperlib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-03-21 13:36:16.000000 gitwrapperlib-1.0.0/gitwrapperlib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      408 2022-03-21 13:36:14.000000 gitwrapperlib-1.0.0/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (121)      153 2022-03-21 13:36:16.000000 gitwrapperlib-1.0.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     1967 2022-03-21 13:34:18.000000 gitwrapperlib-1.0.0/setup.py
+drwxr-xr-x   0 ctyfoxylos   (502) staff       (20)        0 2023-06-13 11:06:09.755581 gitwrapperlib-1.0.1/
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)        5 2023-06-13 11:04:35.000000 gitwrapperlib-1.0.1/.VERSION
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)      171 2023-01-05 16:54:06.000000 gitwrapperlib-1.0.1/AUTHORS.rst
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)     1268 2023-01-05 16:54:03.000000 gitwrapperlib-1.0.1/CONTRIBUTING.rst
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)      837 2023-06-13 11:04:50.000000 gitwrapperlib-1.0.1/HISTORY.rst
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     1063 2023-01-05 16:54:09.000000 gitwrapperlib-1.0.1/LICENSE
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)      400 2023-01-05 16:54:11.000000 gitwrapperlib-1.0.1/MANIFEST.in
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     3717 2023-06-13 11:06:09.755755 gitwrapperlib-1.0.1/PKG-INFO
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)      600 2023-06-13 09:42:10.000000 gitwrapperlib-1.0.1/Pipfile
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)    59590 2023-06-13 09:41:25.000000 gitwrapperlib-1.0.1/Pipfile.lock
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)     2323 2023-01-05 16:54:07.000000 gitwrapperlib-1.0.1/README.rst
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)      913 2023-01-05 16:54:04.000000 gitwrapperlib-1.0.1/USAGE.rst
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)      588 2023-06-13 11:06:06.000000 gitwrapperlib-1.0.1/dev-requirements.txt
+drwxr-xr-x   0 ctyfoxylos   (502) staff       (20)        0 2023-06-13 11:06:09.649700 gitwrapperlib-1.0.1/docs/
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)     6790 2023-01-05 17:00:40.000000 gitwrapperlib-1.0.1/docs/Makefile
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)       28 2023-01-05 17:00:40.000000 gitwrapperlib-1.0.1/docs/authors.rst
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)     8964 2023-01-05 17:00:40.000000 gitwrapperlib-1.0.1/docs/conf.py
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)       33 2023-01-05 17:00:40.000000 gitwrapperlib-1.0.1/docs/contributing.rst
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)       28 2023-01-05 17:00:40.000000 gitwrapperlib-1.0.1/docs/history.rst
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)      513 2023-01-05 17:00:40.000000 gitwrapperlib-1.0.1/docs/index.rst
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)       33 2023-01-05 17:00:40.000000 gitwrapperlib-1.0.1/docs/installation.rst
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)       27 2023-01-05 17:00:40.000000 gitwrapperlib-1.0.1/docs/readme.rst
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)       26 2023-01-05 17:00:40.000000 gitwrapperlib-1.0.1/docs/usage.rst
+drwxr-xr-x   0 ctyfoxylos   (502) staff       (20)        0 2023-06-13 11:06:09.705129 gitwrapperlib-1.0.1/gitwrapperlib/
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)        5 2023-06-13 11:06:06.000000 gitwrapperlib-1.0.1/gitwrapperlib/.VERSION
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)      171 2023-06-13 11:06:06.000000 gitwrapperlib-1.0.1/gitwrapperlib/AUTHORS.rst
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)     1268 2023-06-13 11:06:06.000000 gitwrapperlib-1.0.1/gitwrapperlib/CONTRIBUTING.rst
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)      837 2023-06-13 11:06:06.000000 gitwrapperlib-1.0.1/gitwrapperlib/HISTORY.rst
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     1063 2023-06-13 11:06:06.000000 gitwrapperlib-1.0.1/gitwrapperlib/LICENSE
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)      600 2023-06-13 11:06:06.000000 gitwrapperlib-1.0.1/gitwrapperlib/Pipfile
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)    59590 2023-06-13 11:06:06.000000 gitwrapperlib-1.0.1/gitwrapperlib/Pipfile.lock
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)     2323 2023-06-13 11:06:06.000000 gitwrapperlib-1.0.1/gitwrapperlib/README.rst
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)      913 2023-06-13 11:06:06.000000 gitwrapperlib-1.0.1/gitwrapperlib/USAGE.rst
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)     1962 2023-06-13 08:39:21.000000 gitwrapperlib-1.0.1/gitwrapperlib/__init__.py
+drwxr-xr-x   0 ctyfoxylos   (502) staff       (20)        0 2023-06-13 11:06:09.747910 gitwrapperlib-1.0.1/gitwrapperlib/__pycache__/
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)      821 2021-06-02 07:43:10.000000 gitwrapperlib-1.0.1/gitwrapperlib/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)      810 2023-06-13 09:43:55.000000 gitwrapperlib-1.0.1/gitwrapperlib/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)      919 2021-06-02 07:43:10.000000 gitwrapperlib-1.0.1/gitwrapperlib/__pycache__/_version.cpython-37.pyc
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     1043 2023-06-13 09:43:55.000000 gitwrapperlib-1.0.1/gitwrapperlib/__pycache__/_version.cpython-39.pyc
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     6402 2021-12-02 08:06:31.000000 gitwrapperlib-1.0.1/gitwrapperlib/__pycache__/gitwrapperlib.cpython-37.pyc
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     7064 2023-06-13 10:52:37.000000 gitwrapperlib-1.0.1/gitwrapperlib/__pycache__/gitwrapperlib.cpython-39.pyc
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)      861 2021-06-02 07:43:10.000000 gitwrapperlib-1.0.1/gitwrapperlib/__pycache__/gitwrapperlibexceptions.cpython-37.pyc
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     1231 2023-06-13 09:43:55.000000 gitwrapperlib-1.0.1/gitwrapperlib/__pycache__/gitwrapperlibexceptions.cpython-39.pyc
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     2194 2023-06-13 08:36:02.000000 gitwrapperlib-1.0.1/gitwrapperlib/_version.py
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)      588 2023-06-13 11:06:06.000000 gitwrapperlib-1.0.1/gitwrapperlib/dev-requirements.txt
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)     6961 2023-06-13 10:52:27.000000 gitwrapperlib-1.0.1/gitwrapperlib/gitwrapperlib.py
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     1986 2023-06-13 08:36:02.000000 gitwrapperlib-1.0.1/gitwrapperlib/gitwrapperlibexceptions.py
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)      406 2023-06-13 11:06:06.000000 gitwrapperlib-1.0.1/gitwrapperlib/requirements.txt
+drwxr-xr-x   0 ctyfoxylos   (502) staff       (20)        0 2023-06-13 11:06:09.719221 gitwrapperlib-1.0.1/gitwrapperlib.egg-info/
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     3717 2023-06-13 11:06:09.000000 gitwrapperlib-1.0.1/gitwrapperlib.egg-info/PKG-INFO
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     1423 2023-06-13 11:06:09.000000 gitwrapperlib-1.0.1/gitwrapperlib.egg-info/SOURCES.txt
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)        1 2023-06-13 11:06:09.000000 gitwrapperlib-1.0.1/gitwrapperlib.egg-info/dependency_links.txt
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)        1 2023-06-13 09:42:02.000000 gitwrapperlib-1.0.1/gitwrapperlib.egg-info/not-zip-safe
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)       77 2023-06-13 11:06:09.000000 gitwrapperlib-1.0.1/gitwrapperlib.egg-info/requires.txt
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)       14 2023-06-13 11:06:09.000000 gitwrapperlib-1.0.1/gitwrapperlib.egg-info/top_level.txt
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)      406 2023-06-13 11:06:06.000000 gitwrapperlib-1.0.1/requirements.txt
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)      153 2023-06-13 11:06:09.757766 gitwrapperlib-1.0.1/setup.cfg
+-rwxr-xr-x   0 ctyfoxylos   (502) staff       (20)     1967 2023-01-05 16:54:03.000000 gitwrapperlib-1.0.1/setup.py
+drwxr-xr-x   0 ctyfoxylos   (502) staff       (20)        0 2023-06-13 11:06:09.754561 gitwrapperlib-1.0.1/tests/
+-rw-r--r--   0 ctyfoxylos   (502) staff       (20)     2218 2023-01-05 17:00:40.000000 gitwrapperlib-1.0.1/tests/test_gitwrapperlib.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `gitwrapperlib-1.0.0/CONTRIBUTING.rst` & `gitwrapperlib-1.0.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `gitwrapperlib-1.0.0/HISTORY.rst` & `gitwrapperlib-1.0.1/HISTORY.rst`

 * *Files 12% similar despite different names*

```diff
@@ -45,7 +45,13 @@
 * Self reference update for pipeline.
 
 
 1.0.0 (21-03-2022)
 ------------------
 
 * Removed references to master branch and implemented default remote retrieval, courtesy of Sten Spans <sspans@schubergphilis.com>
+
+
+1.0.1 (13-06-2023)
+------------------
+
+* Bump dependencies and update pipeline to python 3.9.
```

### Comparing `gitwrapperlib-1.0.0/LICENSE` & `gitwrapperlib-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gitwrapperlib-1.0.0/PKG-INFO` & `gitwrapperlib-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: gitwrapperlib
-Version: 1.0.0
+Version: 1.0.1
 Summary: A lightweight wrapper around the git command using sh module.
 Home-page: https://github.com/costastf/gitwrapperlib
 Author: Costas Tyfoxylos
 Author-email: costas.tyf@gmail.com
 License: MIT
 Keywords: gitwrapperlib git python sh
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 License-File: LICENSE
 License-File: AUTHORS.rst
@@ -135,7 +134,11 @@
 
 1.0.0 (21-03-2022)
 ------------------
 
 * Removed references to master branch and implemented default remote retrieval, courtesy of Sten Spans <sspans@schubergphilis.com>
 
 
+1.0.1 (13-06-2023)
+------------------
+
+* Bump dependencies and update pipeline to python 3.9.
```

### Comparing `gitwrapperlib-1.0.0/Pipfile` & `gitwrapperlib-1.0.1/Pipfile`

 * *Files 22% similar despite different names*

```diff
@@ -3,29 +3,28 @@
 url = "https://pypi.python.org/simple"
 verify_ssl = true
 name = "pypi"
 
 
 [dev-packages]
 
-flake8 = "==3.8.0"
-sphinx = "~=2.1.2"
-sphinx-rtd-theme = "~=0.4.3"
-prospector = "~=1.3.0"
-coverage = "~=4.5.4"
-nose = "~=1.3.7"
-nose-htmloutput = "~=0.6.0"
-tox = "~=3.13.2"
-betamax = "~=0.8.1"
-betamax-serializers = "~=0.2.1"
-semver = "~=2.8.1"
-gitwrapperlib = "~=0.10.2"
-twine = "~=1.13.0"
-coloredlogs = "~=10.0"
-emoji = "~=0.5.3"
-toml = "~=0.10.0"
+sphinx = ">=6.0,<7.0"
+sphinx-rtd-theme = ">=1.0,<2.0"
+prospector = ">=1.8,<2.0"
+coverage = ">=7,<8.0"
+nose = ">=1.3,<2.0"
+nose-htmloutput = ">=0.1,<1.0"
+tox = ">=4.0<5.0"
+betamax = ">=0.8,<1.0"
+betamax-serializers = "~=0.2,<1.0"
+semver = ">=3.0,<4.0"
+gitwrapperlib = ">=1.0,<2.0"
+twine = ">=4.0,<5.0"
+coloredlogs = ">=15.0,<16.0"
+emoji = ">=2.0,<3.0"
+toml = ">=0.1,<1.0"
 
 
 [packages]
 
-sh = {version = "~=1.12.14", sys_platform = "!='win32'"}
+sh = {version = ">=2.0,<3.0", sys_platform = "!='win32'"}
 pbs = {version = "~=0.110", sys_platform = "=='win32'"}
```

### Comparing `gitwrapperlib-1.0.0/Pipfile.lock` & `gitwrapperlib-1.0.1/Pipfile.lock`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9104846792668958%*

 * *Differences: {"'_meta'": "{'hash': {'sha256': "*

 * *            "'4fa2d6a765b3b81f226c7b04ae11d34ed18d1ad2d3ff44959d98a7b1ceb4a025'}}",*

 * * "'default'": "{'sh': {'hashes': "*

 * *              "['sha256:14265a4cd1622429edcf300292ec98193530fb143fe642b3437024eca9bee8c5', "*

 * *              "'sha256:a18920f0839991bc9dfddb6dcc006c360b1064ba96257359f0ea356e9fa75a60'], "*

 * *              "'version': '==2.0.4'}}",*

 * * "'develop'": "{'alabaster': {'hashes': "*

 * *              "['sha256:1ee19aca801bbabb5ba3f5f258e4422dfa86f82f3e9cefb0859b283cdd7f62a3', […]*

```diff
@@ -1,11 +1,11 @@
 {
     "_meta": {
         "hash": {
-            "sha256": "adc6d97618b44175e9b1cf78a95b8b6d7233fb7fc0fd2706cf97911922256656"
+            "sha256": "4fa2d6a765b3b81f226c7b04ae11d34ed18d1ad2d3ff44959d98a7b1ceb4a025"
         },
         "pipfile-spec": 6,
         "requires": {},
         "sources": [
             {
                 "name": "pypi",
                 "url": "https://pypi.python.org/simple",
@@ -19,45 +19,46 @@
                 "sha256:05fafccbab7ce1cb2f25330267c8a622b569ad95b40c83220a36983f53757469"
             ],
             "markers": "sys_platform == 'win32'",
             "version": "==0.110"
         },
         "sh": {
             "hashes": [
-                "sha256:ae3258c5249493cebe73cb4e18253a41ed69262484bad36fdb3efcb8ad8870bb",
-                "sha256:b52bf5833ed01c7b5c5fb73a7f71b3d98d48e9b9b8764236237bdc7ecae850fc"
+                "sha256:14265a4cd1622429edcf300292ec98193530fb143fe642b3437024eca9bee8c5",
+                "sha256:a18920f0839991bc9dfddb6dcc006c360b1064ba96257359f0ea356e9fa75a60"
             ],
             "index": "pypi",
             "markers": "sys_platform != 'win32'",
-            "version": "==1.12.14"
+            "version": "==2.0.4"
         }
     },
     "develop": {
         "alabaster": {
             "hashes": [
-                "sha256:446438bdcca0e05bd45ea2de1668c1d9b032e1a9154c2c259092d77031ddd359",
-                "sha256:a661d72d58e6ea8a57f7a86e37d86716863ee5e92788398526d58b26a4e4dc02"
+                "sha256:1ee19aca801bbabb5ba3f5f258e4422dfa86f82f3e9cefb0859b283cdd7f62a3",
+                "sha256:a27a4a084d5e690e16e01e03ad2b2e552c61a65469419b907243193de1a84ae2"
             ],
-            "version": "==0.7.12"
+            "markers": "python_version >= '3.6'",
+            "version": "==0.7.13"
         },
         "astroid": {
             "hashes": [
-                "sha256:4c17cea3e592c21b6e222f673868961bad77e1f985cb1694ed077475a89229c1",
-                "sha256:d8506842a3faf734b81599c8b98dcc423de863adcc1999248480b18bd31a0f38"
+                "sha256:078e5212f9885fa85fbb0cf0101978a336190aadea6e13305409d099f71b2324",
+                "sha256:1039262575027b441137ab4a62a793a9b43defb42c32d5670f38686207cd780f"
             ],
-            "markers": "python_version >= '3.5'",
-            "version": "==2.4.1"
+            "markers": "python_full_version >= '3.7.2'",
+            "version": "==2.15.5"
         },
         "babel": {
             "hashes": [
-                "sha256:ab49e12b91d937cd11f0b67cb259a57ab4ad2b59ac7a3b41d6c06c0ac5b0def9",
-                "sha256:bc0c176f9f6a994582230df350aa6e05ba2ebe4b3ac317eab29d9be5d2768da0"
+                "sha256:b4246fb7677d3b98f501a39d43396d3cafdc8eadb045f4a31be01863f655c610",
+                "sha256:cc2d99999cd01d44420ae725a21c9e3711b3aadc7976d6147f622d8581963455"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
-            "version": "==2.9.1"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.12.1"
         },
         "betamax": {
             "hashes": [
                 "sha256:5bf004ceffccae881213fb722f34517166b84a34919b92ffc14d1dbd050b71c2",
                 "sha256:aa5ad34cc8d018b35814fb0557d15c78ced9ac56fdc43ccacdb882aa7a5217c1"
             ],
             "index": "pypi",
@@ -69,87 +70,221 @@
                 "sha256:345c419b1b73171f2951c62ac3c701775ac4b76e13e86464ebf0ff2a978e4949"
             ],
             "index": "pypi",
             "version": "==0.2.1"
         },
         "bleach": {
             "hashes": [
-                "sha256:0900d8b37eba61a802ee40ac0061f8c2b5dee29c1927dd1d233e075ebf5a71da",
-                "sha256:4d2651ab93271d1129ac9cbc679f524565cc8a1b791909c4a51eac4446a15994"
+                "sha256:1a1a85c1595e07d8db14c5f09f09e6433502c51c595970edc090551f0db99414",
+                "sha256:33c16e3353dbd13028ab4799a0f89a83f113405c766e9c122df8a06f5b85b3f4"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==4.1.0"
+            "markers": "python_version >= '3.7'",
+            "version": "==6.0.0"
+        },
+        "cachetools": {
+            "hashes": [
+                "sha256:95ef631eeaea14ba2e36f06437f36463aac3a096799e876ee55e5cdccb102590",
+                "sha256:dce83f2d9b4e1f732a8cd44af8e8fab2dbe46201467fc98b3ef8f269092bf62b"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==5.3.1"
         },
         "certifi": {
             "hashes": [
-                "sha256:78884e7c1d4b00ce3cea67b44566851c4343c120abd683433ce934a68ea58872",
-                "sha256:d62a0163eb4c2344ac042ab2bdf75399a71a2d8c7d47eac2e2ee91b9d6339569"
+                "sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7",
+                "sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716"
+            ],
+            "markers": "python_version >= '3.6'",
+            "version": "==2023.5.7"
+        },
+        "chardet": {
+            "hashes": [
+                "sha256:0d62712b956bc154f85fb0a266e2a3c5913c2967e00348701b32411d6def31e5",
+                "sha256:362777fb014af596ad31334fde1e8c327dfdb076e1960d1694662d46a6917ab9"
             ],
-            "version": "==2021.10.8"
+            "markers": "python_version >= '3.7'",
+            "version": "==5.1.0"
         },
         "charset-normalizer": {
             "hashes": [
-                "sha256:2857e29ff0d34db842cd7ca3230549d1a697f96ee6d3fb071cfa6c7393832597",
-                "sha256:6881edbebdb17b39b4eaaa821b438bf6eddffb4468cf344f09f89def34a8b1df"
+                "sha256:04afa6387e2b282cf78ff3dbce20f0cc071c12dc8f685bd40960cc68644cfea6",
+                "sha256:04eefcee095f58eaabe6dc3cc2262f3bcd776d2c67005880894f447b3f2cb9c1",
+                "sha256:0be65ccf618c1e7ac9b849c315cc2e8a8751d9cfdaa43027d4f6624bd587ab7e",
+                "sha256:0c95f12b74681e9ae127728f7e5409cbbef9cd914d5896ef238cc779b8152373",
+                "sha256:0ca564606d2caafb0abe6d1b5311c2649e8071eb241b2d64e75a0d0065107e62",
+                "sha256:10c93628d7497c81686e8e5e557aafa78f230cd9e77dd0c40032ef90c18f2230",
+                "sha256:11d117e6c63e8f495412d37e7dc2e2fff09c34b2d09dbe2bee3c6229577818be",
+                "sha256:11d3bcb7be35e7b1bba2c23beedac81ee893ac9871d0ba79effc7fc01167db6c",
+                "sha256:12a2b561af122e3d94cdb97fe6fb2bb2b82cef0cdca131646fdb940a1eda04f0",
+                "sha256:12d1a39aa6b8c6f6248bb54550efcc1c38ce0d8096a146638fd4738e42284448",
+                "sha256:1435ae15108b1cb6fffbcea2af3d468683b7afed0169ad718451f8db5d1aff6f",
+                "sha256:1c60b9c202d00052183c9be85e5eaf18a4ada0a47d188a83c8f5c5b23252f649",
+                "sha256:1e8fcdd8f672a1c4fc8d0bd3a2b576b152d2a349782d1eb0f6b8e52e9954731d",
+                "sha256:20064ead0717cf9a73a6d1e779b23d149b53daf971169289ed2ed43a71e8d3b0",
+                "sha256:21fa558996782fc226b529fdd2ed7866c2c6ec91cee82735c98a197fae39f706",
+                "sha256:22908891a380d50738e1f978667536f6c6b526a2064156203d418f4856d6e86a",
+                "sha256:3160a0fd9754aab7d47f95a6b63ab355388d890163eb03b2d2b87ab0a30cfa59",
+                "sha256:322102cdf1ab682ecc7d9b1c5eed4ec59657a65e1c146a0da342b78f4112db23",
+                "sha256:34e0a2f9c370eb95597aae63bf85eb5e96826d81e3dcf88b8886012906f509b5",
+                "sha256:3573d376454d956553c356df45bb824262c397c6e26ce43e8203c4c540ee0acb",
+                "sha256:3747443b6a904001473370d7810aa19c3a180ccd52a7157aacc264a5ac79265e",
+                "sha256:38e812a197bf8e71a59fe55b757a84c1f946d0ac114acafaafaf21667a7e169e",
+                "sha256:3a06f32c9634a8705f4ca9946d667609f52cf130d5548881401f1eb2c39b1e2c",
+                "sha256:3a5fc78f9e3f501a1614a98f7c54d3969f3ad9bba8ba3d9b438c3bc5d047dd28",
+                "sha256:3d9098b479e78c85080c98e1e35ff40b4a31d8953102bb0fd7d1b6f8a2111a3d",
+                "sha256:3dc5b6a8ecfdc5748a7e429782598e4f17ef378e3e272eeb1340ea57c9109f41",
+                "sha256:4155b51ae05ed47199dc5b2a4e62abccb274cee6b01da5b895099b61b1982974",
+                "sha256:49919f8400b5e49e961f320c735388ee686a62327e773fa5b3ce6721f7e785ce",
+                "sha256:53d0a3fa5f8af98a1e261de6a3943ca631c526635eb5817a87a59d9a57ebf48f",
+                "sha256:5f008525e02908b20e04707a4f704cd286d94718f48bb33edddc7d7b584dddc1",
+                "sha256:628c985afb2c7d27a4800bfb609e03985aaecb42f955049957814e0491d4006d",
+                "sha256:65ed923f84a6844de5fd29726b888e58c62820e0769b76565480e1fdc3d062f8",
+                "sha256:6734e606355834f13445b6adc38b53c0fd45f1a56a9ba06c2058f86893ae8017",
+                "sha256:6baf0baf0d5d265fa7944feb9f7451cc316bfe30e8df1a61b1bb08577c554f31",
+                "sha256:6f4f4668e1831850ebcc2fd0b1cd11721947b6dc7c00bf1c6bd3c929ae14f2c7",
+                "sha256:6f5c2e7bc8a4bf7c426599765b1bd33217ec84023033672c1e9a8b35eaeaaaf8",
+                "sha256:6f6c7a8a57e9405cad7485f4c9d3172ae486cfef1344b5ddd8e5239582d7355e",
+                "sha256:7381c66e0561c5757ffe616af869b916c8b4e42b367ab29fedc98481d1e74e14",
+                "sha256:73dc03a6a7e30b7edc5b01b601e53e7fc924b04e1835e8e407c12c037e81adbd",
+                "sha256:74db0052d985cf37fa111828d0dd230776ac99c740e1a758ad99094be4f1803d",
+                "sha256:75f2568b4189dda1c567339b48cba4ac7384accb9c2a7ed655cd86b04055c795",
+                "sha256:78cacd03e79d009d95635e7d6ff12c21eb89b894c354bd2b2ed0b4763373693b",
+                "sha256:80d1543d58bd3d6c271b66abf454d437a438dff01c3e62fdbcd68f2a11310d4b",
+                "sha256:830d2948a5ec37c386d3170c483063798d7879037492540f10a475e3fd6f244b",
+                "sha256:891cf9b48776b5c61c700b55a598621fdb7b1e301a550365571e9624f270c203",
+                "sha256:8f25e17ab3039b05f762b0a55ae0b3632b2e073d9c8fc88e89aca31a6198e88f",
+                "sha256:9a3267620866c9d17b959a84dd0bd2d45719b817245e49371ead79ed4f710d19",
+                "sha256:a04f86f41a8916fe45ac5024ec477f41f886b3c435da2d4e3d2709b22ab02af1",
+                "sha256:aaf53a6cebad0eae578f062c7d462155eada9c172bd8c4d250b8c1d8eb7f916a",
+                "sha256:abc1185d79f47c0a7aaf7e2412a0eb2c03b724581139193d2d82b3ad8cbb00ac",
+                "sha256:ac0aa6cd53ab9a31d397f8303f92c42f534693528fafbdb997c82bae6e477ad9",
+                "sha256:ac3775e3311661d4adace3697a52ac0bab17edd166087d493b52d4f4f553f9f0",
+                "sha256:b06f0d3bf045158d2fb8837c5785fe9ff9b8c93358be64461a1089f5da983137",
+                "sha256:b116502087ce8a6b7a5f1814568ccbd0e9f6cfd99948aa59b0e241dc57cf739f",
+                "sha256:b82fab78e0b1329e183a65260581de4375f619167478dddab510c6c6fb04d9b6",
+                "sha256:bd7163182133c0c7701b25e604cf1611c0d87712e56e88e7ee5d72deab3e76b5",
+                "sha256:c36bcbc0d5174a80d6cccf43a0ecaca44e81d25be4b7f90f0ed7bcfbb5a00909",
+                "sha256:c3af8e0f07399d3176b179f2e2634c3ce9c1301379a6b8c9c9aeecd481da494f",
+                "sha256:c84132a54c750fda57729d1e2599bb598f5fa0344085dbde5003ba429a4798c0",
+                "sha256:cb7b2ab0188829593b9de646545175547a70d9a6e2b63bf2cd87a0a391599324",
+                "sha256:cca4def576f47a09a943666b8f829606bcb17e2bc2d5911a46c8f8da45f56755",
+                "sha256:cf6511efa4801b9b38dc5546d7547d5b5c6ef4b081c60b23e4d941d0eba9cbeb",
+                "sha256:d16fd5252f883eb074ca55cb622bc0bee49b979ae4e8639fff6ca3ff44f9f854",
+                "sha256:d2686f91611f9e17f4548dbf050e75b079bbc2a82be565832bc8ea9047b61c8c",
+                "sha256:d7fc3fca01da18fbabe4625d64bb612b533533ed10045a2ac3dd194bfa656b60",
+                "sha256:dd5653e67b149503c68c4018bf07e42eeed6b4e956b24c00ccdf93ac79cdff84",
+                "sha256:de5695a6f1d8340b12a5d6d4484290ee74d61e467c39ff03b39e30df62cf83a0",
+                "sha256:e0ac8959c929593fee38da1c2b64ee9778733cdf03c482c9ff1d508b6b593b2b",
+                "sha256:e1b25e3ad6c909f398df8921780d6a3d120d8c09466720226fc621605b6f92b1",
+                "sha256:e633940f28c1e913615fd624fcdd72fdba807bf53ea6925d6a588e84e1151531",
+                "sha256:e89df2958e5159b811af9ff0f92614dabf4ff617c03a4c1c6ff53bf1c399e0e1",
+                "sha256:ea9f9c6034ea2d93d9147818f17c2a0860d41b71c38b9ce4d55f21b6f9165a11",
+                "sha256:f645caaf0008bacf349875a974220f1f1da349c5dbe7c4ec93048cdc785a3326",
+                "sha256:f8303414c7b03f794347ad062c0516cee0e15f7a612abd0ce1e25caf6ceb47df",
+                "sha256:fca62a8301b605b954ad2e9c3666f9d97f63872aa4efcae5492baca2056b74ab"
+            ],
+            "markers": "python_full_version >= '3.7.0'",
+            "version": "==3.1.0"
+        },
+        "colorama": {
+            "hashes": [
+                "sha256:08695f5cb7ed6e0531a20572697297273c47b8cae5a63ffc6d6ed5c201be6e44",
+                "sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6"
             ],
-            "markers": "python_version >= '3.0'",
-            "version": "==2.0.12"
+            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6'",
+            "version": "==0.4.6"
         },
         "coloredlogs": {
             "hashes": [
-                "sha256:34fad2e342d5a559c31b6c889e8d14f97cb62c47d9a2ae7b5ed14ea10a79eff8",
-                "sha256:b869a2dda3fa88154b9dd850e27828d8755bfab5a838a1c97fbc850c6e377c36"
+                "sha256:612ee75c546f53e92e70049c9dbfcc18c935a2b9a53b66085ce9ef6a6e5c0934",
+                "sha256:7c991aa71a4577af2f82600d8f8f3a89f936baeaf9b50a9c197da014e5bf16b0"
             ],
             "index": "pypi",
-            "version": "==10.0"
+            "version": "==15.0.1"
         },
         "coverage": {
             "hashes": [
-                "sha256:08907593569fe59baca0bf152c43f3863201efb6113ecb38ce7e97ce339805a6",
-                "sha256:0be0f1ed45fc0c185cfd4ecc19a1d6532d72f86a2bac9de7e24541febad72650",
-                "sha256:141f08ed3c4b1847015e2cd62ec06d35e67a3ac185c26f7635f4406b90afa9c5",
-                "sha256:19e4df788a0581238e9390c85a7a09af39c7b539b29f25c89209e6c3e371270d",
-                "sha256:23cc09ed395b03424d1ae30dcc292615c1372bfba7141eb85e11e50efaa6b351",
-                "sha256:245388cda02af78276b479f299bbf3783ef0a6a6273037d7c60dc73b8d8d7755",
-                "sha256:331cb5115673a20fb131dadd22f5bcaf7677ef758741312bee4937d71a14b2ef",
-                "sha256:386e2e4090f0bc5df274e720105c342263423e77ee8826002dcffe0c9533dbca",
-                "sha256:3a794ce50daee01c74a494919d5ebdc23d58873747fa0e288318728533a3e1ca",
-                "sha256:60851187677b24c6085248f0a0b9b98d49cba7ecc7ec60ba6b9d2e5574ac1ee9",
-                "sha256:63a9a5fc43b58735f65ed63d2cf43508f462dc49857da70b8980ad78d41d52fc",
-                "sha256:6b62544bb68106e3f00b21c8930e83e584fdca005d4fffd29bb39fb3ffa03cb5",
-                "sha256:6ba744056423ef8d450cf627289166da65903885272055fb4b5e113137cfa14f",
-                "sha256:7494b0b0274c5072bddbfd5b4a6c6f18fbbe1ab1d22a41e99cd2d00c8f96ecfe",
-                "sha256:826f32b9547c8091679ff292a82aca9c7b9650f9fda3e2ca6bf2ac905b7ce888",
-                "sha256:93715dffbcd0678057f947f496484e906bf9509f5c1c38fc9ba3922893cda5f5",
-                "sha256:9a334d6c83dfeadae576b4d633a71620d40d1c379129d587faa42ee3e2a85cce",
-                "sha256:af7ed8a8aa6957aac47b4268631fa1df984643f07ef00acd374e456364b373f5",
-                "sha256:bf0a7aed7f5521c7ca67febd57db473af4762b9622254291fbcbb8cd0ba5e33e",
-                "sha256:bf1ef9eb901113a9805287e090452c05547578eaab1b62e4ad456fcc049a9b7e",
-                "sha256:c0afd27bc0e307a1ffc04ca5ec010a290e49e3afbe841c5cafc5c5a80ecd81c9",
-                "sha256:dd579709a87092c6dbee09d1b7cfa81831040705ffa12a1b248935274aee0437",
-                "sha256:df6712284b2e44a065097846488f66840445eb987eb81b3cc6e4149e7b6982e1",
-                "sha256:e07d9f1a23e9e93ab5c62902833bf3e4b1f65502927379148b6622686223125c",
-                "sha256:e2ede7c1d45e65e209d6093b762e98e8318ddeff95317d07a27a2140b80cfd24",
-                "sha256:e4ef9c164eb55123c62411f5936b5c2e521b12356037b6e1c2617cef45523d47",
-                "sha256:eca2b7343524e7ba246cab8ff00cab47a2d6d54ada3b02772e908a45675722e2",
-                "sha256:eee64c616adeff7db37cc37da4180a3a5b6177f5c46b187894e633f088fb5b28",
-                "sha256:ef824cad1f980d27f26166f86856efe11eff9912c4fed97d3804820d43fa550c",
-                "sha256:efc89291bd5a08855829a3c522df16d856455297cf35ae827a37edac45f466a7",
-                "sha256:fa964bae817babece5aa2e8c1af841bebb6d0b9add8e637548809d040443fee0",
-                "sha256:ff37757e068ae606659c28c3bd0d923f9d29a85de79bf25b2b34b148473b5025"
+                "sha256:06a9a2be0b5b576c3f18f1a241f0473575c4a26021b52b2a85263a00f034d51f",
+                "sha256:06fb182e69f33f6cd1d39a6c597294cff3143554b64b9825d1dc69d18cc2fff2",
+                "sha256:0a5f9e1dbd7fbe30196578ca36f3fba75376fb99888c395c5880b355e2875f8a",
+                "sha256:0e1f928eaf5469c11e886fe0885ad2bf1ec606434e79842a879277895a50942a",
+                "sha256:171717c7cb6b453aebac9a2ef603699da237f341b38eebfee9be75d27dc38e01",
+                "sha256:1e9d683426464e4a252bf70c3498756055016f99ddaec3774bf368e76bbe02b6",
+                "sha256:201e7389591af40950a6480bd9edfa8ed04346ff80002cec1a66cac4549c1ad7",
+                "sha256:245167dd26180ab4c91d5e1496a30be4cd721a5cf2abf52974f965f10f11419f",
+                "sha256:2aee274c46590717f38ae5e4650988d1af340fe06167546cc32fe2f58ed05b02",
+                "sha256:2e07b54284e381531c87f785f613b833569c14ecacdcb85d56b25c4622c16c3c",
+                "sha256:31563e97dae5598556600466ad9beea39fb04e0229e61c12eaa206e0aa202063",
+                "sha256:33d6d3ea29d5b3a1a632b3c4e4f4ecae24ef170b0b9ee493883f2df10039959a",
+                "sha256:3d376df58cc111dc8e21e3b6e24606b5bb5dee6024f46a5abca99124b2229ef5",
+                "sha256:419bfd2caae268623dd469eff96d510a920c90928b60f2073d79f8fe2bbc5959",
+                "sha256:48c19d2159d433ccc99e729ceae7d5293fbffa0bdb94952d3579983d1c8c9d97",
+                "sha256:49969a9f7ffa086d973d91cec8d2e31080436ef0fb4a359cae927e742abfaaa6",
+                "sha256:52edc1a60c0d34afa421c9c37078817b2e67a392cab17d97283b64c5833f427f",
+                "sha256:537891ae8ce59ef63d0123f7ac9e2ae0fc8b72c7ccbe5296fec45fd68967b6c9",
+                "sha256:54b896376ab563bd38453cecb813c295cf347cf5906e8b41d340b0321a5433e5",
+                "sha256:58c2ccc2f00ecb51253cbe5d8d7122a34590fac9646a960d1430d5b15321d95f",
+                "sha256:5b7540161790b2f28143191f5f8ec02fb132660ff175b7747b95dcb77ac26562",
+                "sha256:5baa06420f837184130752b7c5ea0808762083bf3487b5038d68b012e5937dbe",
+                "sha256:5e330fc79bd7207e46c7d7fd2bb4af2963f5f635703925543a70b99574b0fea9",
+                "sha256:61b9a528fb348373c433e8966535074b802c7a5d7f23c4f421e6c6e2f1697a6f",
+                "sha256:63426706118b7f5cf6bb6c895dc215d8a418d5952544042c8a2d9fe87fcf09cb",
+                "sha256:6d040ef7c9859bb11dfeb056ff5b3872436e3b5e401817d87a31e1750b9ae2fb",
+                "sha256:6f48351d66575f535669306aa7d6d6f71bc43372473b54a832222803eb956fd1",
+                "sha256:7ee7d9d4822c8acc74a5e26c50604dff824710bc8de424904c0982e25c39c6cb",
+                "sha256:81c13a1fc7468c40f13420732805a4c38a105d89848b7c10af65a90beff25250",
+                "sha256:8d13c64ee2d33eccf7437961b6ea7ad8673e2be040b4f7fd4fd4d4d28d9ccb1e",
+                "sha256:8de8bb0e5ad103888d65abef8bca41ab93721647590a3f740100cd65c3b00511",
+                "sha256:8fa03bce9bfbeeef9f3b160a8bed39a221d82308b4152b27d82d8daa7041fee5",
+                "sha256:924d94291ca674905fe9481f12294eb11f2d3d3fd1adb20314ba89e94f44ed59",
+                "sha256:975d70ab7e3c80a3fe86001d8751f6778905ec723f5b110aed1e450da9d4b7f2",
+                "sha256:976b9c42fb2a43ebf304fa7d4a310e5f16cc99992f33eced91ef6f908bd8f33d",
+                "sha256:9e31cb64d7de6b6f09702bb27c02d1904b3aebfca610c12772452c4e6c21a0d3",
+                "sha256:a342242fe22407f3c17f4b499276a02b01e80f861f1682ad1d95b04018e0c0d4",
+                "sha256:a3d33a6b3eae87ceaefa91ffdc130b5e8536182cd6dfdbfc1aa56b46ff8c86de",
+                "sha256:a895fcc7b15c3fc72beb43cdcbdf0ddb7d2ebc959edac9cef390b0d14f39f8a9",
+                "sha256:afb17f84d56068a7c29f5fa37bfd38d5aba69e3304af08ee94da8ed5b0865833",
+                "sha256:b1c546aca0ca4d028901d825015dc8e4d56aac4b541877690eb76490f1dc8ed0",
+                "sha256:b29019c76039dc3c0fd815c41392a044ce555d9bcdd38b0fb60fb4cd8e475ba9",
+                "sha256:b46517c02ccd08092f4fa99f24c3b83d8f92f739b4657b0f146246a0ca6a831d",
+                "sha256:b7aa5f8a41217360e600da646004f878250a0d6738bcdc11a0a39928d7dc2050",
+                "sha256:b7b4c971f05e6ae490fef852c218b0e79d4e52f79ef0c8475566584a8fb3e01d",
+                "sha256:ba90a9563ba44a72fda2e85302c3abc71c5589cea608ca16c22b9804262aaeb6",
+                "sha256:cb017fd1b2603ef59e374ba2063f593abe0fc45f2ad9abdde5b4d83bd922a353",
+                "sha256:d22656368f0e6189e24722214ed8d66b8022db19d182927b9a248a2a8a2f67eb",
+                "sha256:d2c2db7fd82e9b72937969bceac4d6ca89660db0a0967614ce2481e81a0b771e",
+                "sha256:d39b5b4f2a66ccae8b7263ac3c8170994b65266797fb96cbbfd3fb5b23921db8",
+                "sha256:d62a5c7dad11015c66fbb9d881bc4caa5b12f16292f857842d9d1871595f4495",
+                "sha256:e7d9405291c6928619403db1d10bd07888888ec1abcbd9748fdaa971d7d661b2",
+                "sha256:e84606b74eb7de6ff581a7915e2dab7a28a0517fbe1c9239eb227e1354064dcd",
+                "sha256:eb393e5ebc85245347950143969b241d08b52b88a3dc39479822e073a1a8eb27",
+                "sha256:ebba1cd308ef115925421d3e6a586e655ca5a77b5bf41e02eb0e4562a111f2d1",
+                "sha256:ee57190f24fba796e36bb6d3aa8a8783c643d8fa9760c89f7a98ab5455fbf818",
+                "sha256:f2f67fe12b22cd130d34d0ef79206061bfb5eda52feb6ce0dba0644e20a03cf4",
+                "sha256:f6951407391b639504e3b3be51b7ba5f3528adbf1a8ac3302b687ecababf929e",
+                "sha256:f75f7168ab25dd93110c8a8117a22450c19976afbc44234cbf71481094c1b850",
+                "sha256:fdec9e8cbf13a5bf63290fc6013d216a4c7232efb51548594ca3631a7f13c3a3"
             ],
             "index": "pypi",
-            "version": "==4.5.4"
+            "version": "==7.2.7"
+        },
+        "dill": {
+            "hashes": [
+                "sha256:a07ffd2351b8c678dfc4a856a3005f8067aea51d6ba6c700796a4d9e280f39f0",
+                "sha256:e5db55f3687856d8fbdab002ed78544e1c4559a130302693d839dfe8f93f2373"
+            ],
+            "markers": "python_version < '3.11'",
+            "version": "==0.3.6"
         },
         "distlib": {
             "hashes": [
-                "sha256:6564fe0a8f51e734df6333d08b8b94d4ea8ee6b99b5ed50613f731fd4089f34b",
-                "sha256:e4b58818180336dc9c529bfb9a0b58728ffc09ad92027a3f30b7cd91e3458579"
+                "sha256:14bad2d9b04d3a36127ac97f30b12a19268f211063d8f8ee4f47108896e11b46",
+                "sha256:f35c4b692542ca110de7ef0bea44d73981caeb34ca0b9b6b2e6d7790dda8f80e"
             ],
-            "version": "==0.3.4"
+            "version": "==0.3.6"
         },
         "docutils": {
             "hashes": [
                 "sha256:23010f129180089fbcd3bc08cfefccb3b890b0050e1ca00c867036e9d161b98c",
                 "sha256:679987caf361a7539d76e584cbeddc311e3aee937877c87346f31debc63e9d06"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
@@ -160,177 +295,258 @@
                 "sha256:28323cbfc9352139fdd3d316fa17f325cc0e9ac74438cbba51d70f9b48f86c3a",
                 "sha256:51f54c0fd886fa3854387f354b19f429d38c04f984f38bc572558b703c0542a6"
             ],
             "version": "==0.2.1"
         },
         "emoji": {
             "hashes": [
-                "sha256:60652d3a2dcee5b8af8acb097c31776fb6d808027aeb7221830f72cdafefc174"
+                "sha256:0e048dd540a0644bd30790b540466492f1487a3788528422fe196a939a7a3ac0"
             ],
             "index": "pypi",
-            "version": "==0.5.4"
+            "version": "==2.5.0"
         },
         "filelock": {
             "hashes": [
-                "sha256:9cd540a9352e432c7246a48fe4e8712b10acb1df2ad1f30e8c070b82ae1fed85",
-                "sha256:f8314284bfffbdcfa0ff3d7992b023d4c628ced6feb957351d4c48d059f56bc0"
+                "sha256:002740518d8aa59a26b0c76e10fb8c6e15eae825d34b6fdf670333fd7b938d81",
+                "sha256:cbb791cdea2a72f23da6ac5b5269ab0a0d161e9ef0100e653b69049a7706d1ec"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.6.0"
+            "version": "==3.12.2"
         },
         "flake8": {
             "hashes": [
-                "sha256:bcf5163890bb01f11f04f0f444f01004d0f9ad5fab10c51104f770acf532008f",
-                "sha256:e2f33066fb92ac0a3a30ea509f61e325f2110b2e84644333a3ff8e9e98a2beab"
+                "sha256:6fbe320aad8d6b95cec8b8e47bc933004678dc63095be98528b7bdd2a9f510db",
+                "sha256:7a1cf6b73744f5806ab95e526f6f0d8c01c66d7bbe349562d22dfca20610b248"
             ],
-            "index": "pypi",
-            "version": "==3.8.0"
+            "markers": "python_full_version >= '3.6.1'",
+            "version": "==5.0.4"
         },
         "flake8-polyfill": {
             "hashes": [
                 "sha256:12be6a34ee3ab795b19ca73505e7b55826d5f6ad7230d31b18e106400169b9e9",
                 "sha256:e44b087597f6da52ec6393a709e7108b2905317d0c0b744cdca6208e670d8eda"
             ],
             "version": "==1.0.2"
         },
+        "gitdb": {
+            "hashes": [
+                "sha256:6eb990b69df4e15bad899ea868dc46572c3f75339735663b81de79b06f17eb9a",
+                "sha256:c286cf298426064079ed96a9e4a9d39e7f3e9bf15ba60701e95f5492f28415c7"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==4.0.10"
+        },
+        "gitpython": {
+            "hashes": [
+                "sha256:8ce3bcf69adfdf7c7d503e78fd3b1c492af782d58893b650adb2ac8912ddd573",
+                "sha256:f04893614f6aa713a60cbbe1e6a97403ef633103cdd0ef5eb6efe0deb98dbe8d"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==3.1.31"
+        },
         "gitwrapperlib": {
             "hashes": [
-                "sha256:e7ca1c670ec21e325f502997ba27dd479609460e420ae23c82d23bd6c21ebd19",
-                "sha256:e9476fd7e70f50060c249ce4608b77519c8a3891607475696d8a9e95b51943a5"
+                "sha256:3174bcc0de3fa70f78067cb2bc60a5c9820442d78594fb345bdd56740f64073a"
             ],
             "index": "pypi",
-            "version": "==0.10.3"
+            "version": "==1.0.0"
         },
         "humanfriendly": {
             "hashes": [
                 "sha256:1697e1a8a8f550fd43c2865cd84542fc175a61dcb779b6fee18cf6b6ccba1477",
                 "sha256:6b0b831ce8f15f7300721aa49829fc4e83921a9a301cc7f606be6686a2288ddc"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
             "version": "==10.0"
         },
         "idna": {
             "hashes": [
-                "sha256:84d9dd047ffa80596e0f246e2eab0b391788b0503584e8945f2368256d2735ff",
-                "sha256:9d643ff0a55b762d5cdb124b8eaa99c66322e2157b69160bc32796e824360e6d"
+                "sha256:814f528e8dead7d329833b91c5faa87d60bf71824cd12a7530b5526063d02cb4",
+                "sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2"
             ],
-            "markers": "python_version >= '3.0'",
-            "version": "==3.3"
+            "markers": "python_version >= '3.5'",
+            "version": "==3.4"
         },
         "imagesize": {
             "hashes": [
-                "sha256:1db2f82529e53c3e929e8926a1fa9235aa82d0bd0c580359c67ec31b2fddaa8c",
-                "sha256:cd1750d452385ca327479d45b64d9c7729ecf0b3969a58148298c77092261f9d"
+                "sha256:0d8d18d08f840c19d0ee7ca1fd82490fdc3729b7ac93f49870406ddde8ef8d8b",
+                "sha256:69150444affb9cb0d5cc5a92b3676f0b2fb7cd9ae39e947a5e11a36b4497cd4a"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
-            "version": "==1.3.0"
+            "version": "==1.4.1"
         },
         "importlib-metadata": {
             "hashes": [
-                "sha256:aa18d7378b00b40847790e7c27e11673d7fed219354109d0e7b9e5b25dc3ad26",
-                "sha256:d5f18a79777f3aa179c145737780282e27b508fc8fd688cb17c7a813e8bd39af"
+                "sha256:43dd286a2cd8995d5eaef7fee2066340423b818ed3fd70adf0bad5f1fac53fed",
+                "sha256:92501cdf9cc66ebd3e612f1b4f0c0765dfa42f0fa38ffb319b6bd84dd675d705"
             ],
-            "markers": "python_version < '3.8'",
-            "version": "==0.23"
+            "markers": "python_version < '3.10'",
+            "version": "==6.6.0"
         },
         "isort": {
             "hashes": [
-                "sha256:54da7e92468955c4fceacd0c86bd0ec997b0e1ee80d97f67c35a78b719dccab1",
-                "sha256:6e811fcb295968434526407adb8796944f1988c5b65e8139058f2014cbe100fd"
+                "sha256:8bef7dde241278824a6d83f44a544709b065191b95b6e50894bdc722fcba0504",
+                "sha256:f84c2818376e66cf843d497486ea8fed8700b340f308f076c6fb1229dff318b6"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
-            "version": "==4.3.21"
+            "markers": "python_full_version >= '3.8.0'",
+            "version": "==5.12.0"
+        },
+        "jaraco.classes": {
+            "hashes": [
+                "sha256:2353de3288bc6b82120752201c6b1c1a14b058267fa424ed5ce5984e3b922158",
+                "sha256:89559fa5c1d3c34eff6f631ad80bb21f378dbcbb35dd161fd2c6b93f5be2f98a"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==3.2.3"
         },
         "jinja2": {
             "hashes": [
-                "sha256:077ce6014f7b40d03b47d1f1ca4b0fc8328a692bd284016f806ed0eaca390ad8",
-                "sha256:611bb273cd68f3b993fabdc4064fc858c5b47a973cb5aa7999ec1ba405c87cd7"
+                "sha256:31351a702a408a9e7595a8fc6150fc3f43bb6bf7e319770cbc0db9df9437e852",
+                "sha256:6088930bfe239f0e6710546ab9c19c9ef35e29792895fed6e6e31a023a182a61"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==3.0.3"
+            "markers": "python_version >= '3.7'",
+            "version": "==3.1.2"
+        },
+        "keyring": {
+            "hashes": [
+                "sha256:771ed2a91909389ed6148631de678f82ddc73737d85a927f382a8a1b157898cd",
+                "sha256:ba2e15a9b35e21908d0aaf4e0a47acc52d6ae33444df0da2b49d41a46ef6d678"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==23.13.1"
         },
         "lazy-object-proxy": {
             "hashes": [
-                "sha256:0c4b206227a8097f05c4dbdd323c50edf81f15db3b8dc064d08c62d37e1a504d",
-                "sha256:194d092e6f246b906e8f70884e620e459fc54db3259e60cf69a4d66c3fda3449",
-                "sha256:1be7e4c9f96948003609aa6c974ae59830a6baecc5376c25c92d7d697e684c08",
-                "sha256:4677f594e474c91da97f489fea5b7daa17b5517190899cf213697e48d3902f5a",
-                "sha256:48dab84ebd4831077b150572aec802f303117c8cc5c871e182447281ebf3ac50",
-                "sha256:5541cada25cd173702dbd99f8e22434105456314462326f06dba3e180f203dfd",
-                "sha256:59f79fef100b09564bc2df42ea2d8d21a64fdcda64979c0fa3db7bdaabaf6239",
-                "sha256:8d859b89baf8ef7f8bc6b00aa20316483d67f0b1cbf422f5b4dc56701c8f2ffb",
-                "sha256:9254f4358b9b541e3441b007a0ea0764b9d056afdeafc1a5569eee1cc6c1b9ea",
-                "sha256:9651375199045a358eb6741df3e02a651e0330be090b3bc79f6d0de31a80ec3e",
-                "sha256:97bb5884f6f1cdce0099f86b907aa41c970c3c672ac8b9c8352789e103cf3156",
-                "sha256:9b15f3f4c0f35727d3a0fba4b770b3c4ebbb1fa907dbcc046a1d2799f3edd142",
-                "sha256:a2238e9d1bb71a56cd710611a1614d1194dc10a175c1e08d75e1a7bcc250d442",
-                "sha256:a6ae12d08c0bf9909ce12385803a543bfe99b95fe01e752536a60af2b7797c62",
-                "sha256:ca0a928a3ddbc5725be2dd1cf895ec0a254798915fb3a36af0964a0a4149e3db",
-                "sha256:cb2c7c57005a6804ab66f106ceb8482da55f5314b7fcb06551db1edae4ad1531",
-                "sha256:d74bb8693bf9cf75ac3b47a54d716bbb1a92648d5f781fc799347cfc95952383",
-                "sha256:d945239a5639b3ff35b70a88c5f2f491913eb94871780ebfabb2568bd58afc5a",
-                "sha256:eba7011090323c1dadf18b3b689845fd96a61ba0a1dfbd7f24b921398affc357",
-                "sha256:efa1909120ce98bbb3777e8b6f92237f5d5c8ea6758efea36a473e1d38f7d3e4",
-                "sha256:f3900e8a5de27447acbf900b4750b0ddfd7ec1ea7fbaf11dfa911141bc522af0"
+                "sha256:09763491ce220c0299688940f8dc2c5d05fd1f45af1e42e636b2e8b2303e4382",
+                "sha256:0a891e4e41b54fd5b8313b96399f8b0e173bbbfc03c7631f01efbe29bb0bcf82",
+                "sha256:189bbd5d41ae7a498397287c408617fe5c48633e7755287b21d741f7db2706a9",
+                "sha256:18b78ec83edbbeb69efdc0e9c1cb41a3b1b1ed11ddd8ded602464c3fc6020494",
+                "sha256:1aa3de4088c89a1b69f8ec0dcc169aa725b0ff017899ac568fe44ddc1396df46",
+                "sha256:212774e4dfa851e74d393a2370871e174d7ff0ebc980907723bb67d25c8a7c30",
+                "sha256:2d0daa332786cf3bb49e10dc6a17a52f6a8f9601b4cf5c295a4f85854d61de63",
+                "sha256:5f83ac4d83ef0ab017683d715ed356e30dd48a93746309c8f3517e1287523ef4",
+                "sha256:659fb5809fa4629b8a1ac5106f669cfc7bef26fbb389dda53b3e010d1ac4ebae",
+                "sha256:660c94ea760b3ce47d1855a30984c78327500493d396eac4dfd8bd82041b22be",
+                "sha256:66a3de4a3ec06cd8af3f61b8e1ec67614fbb7c995d02fa224813cb7afefee701",
+                "sha256:721532711daa7db0d8b779b0bb0318fa87af1c10d7fe5e52ef30f8eff254d0cd",
+                "sha256:7322c3d6f1766d4ef1e51a465f47955f1e8123caee67dd641e67d539a534d006",
+                "sha256:79a31b086e7e68b24b99b23d57723ef7e2c6d81ed21007b6281ebcd1688acb0a",
+                "sha256:81fc4d08b062b535d95c9ea70dbe8a335c45c04029878e62d744bdced5141586",
+                "sha256:8fa02eaab317b1e9e03f69aab1f91e120e7899b392c4fc19807a8278a07a97e8",
+                "sha256:9090d8e53235aa280fc9239a86ae3ea8ac58eff66a705fa6aa2ec4968b95c821",
+                "sha256:946d27deaff6cf8452ed0dba83ba38839a87f4f7a9732e8f9fd4107b21e6ff07",
+                "sha256:9990d8e71b9f6488e91ad25f322898c136b008d87bf852ff65391b004da5e17b",
+                "sha256:9cd077f3d04a58e83d04b20e334f678c2b0ff9879b9375ed107d5d07ff160171",
+                "sha256:9e7551208b2aded9c1447453ee366f1c4070602b3d932ace044715d89666899b",
+                "sha256:9f5fa4a61ce2438267163891961cfd5e32ec97a2c444e5b842d574251ade27d2",
+                "sha256:b40387277b0ed2d0602b8293b94d7257e17d1479e257b4de114ea11a8cb7f2d7",
+                "sha256:bfb38f9ffb53b942f2b5954e0f610f1e721ccebe9cce9025a38c8ccf4a5183a4",
+                "sha256:cbf9b082426036e19c6924a9ce90c740a9861e2bdc27a4834fd0a910742ac1e8",
+                "sha256:d9e25ef10a39e8afe59a5c348a4dbf29b4868ab76269f81ce1674494e2565a6e",
+                "sha256:db1c1722726f47e10e0b5fdbf15ac3b8adb58c091d12b3ab713965795036985f",
+                "sha256:e7c21c95cae3c05c14aafffe2865bbd5e377cfc1348c4f7751d9dc9a48ca4bda",
+                "sha256:e8c6cfb338b133fbdbc5cfaa10fe3c6aeea827db80c978dbd13bc9dd8526b7d4",
+                "sha256:ea806fd4c37bf7e7ad82537b0757999264d5f70c45468447bb2b91afdbe73a6e",
+                "sha256:edd20c5a55acb67c7ed471fa2b5fb66cb17f61430b7a6b9c3b4a1e40293b1671",
+                "sha256:f0117049dd1d5635bbff65444496c90e0baa48ea405125c088e93d9cf4525b11",
+                "sha256:f0705c376533ed2a9e5e97aacdbfe04cecd71e0aa84c7c0595d02ef93b6e4455",
+                "sha256:f12ad7126ae0c98d601a7ee504c1122bcef553d1d5e0c3bfa77b16b3968d2734",
+                "sha256:f2457189d8257dd41ae9b434ba33298aec198e30adf2dcdaaa3a28b9994f6adb",
+                "sha256:f699ac1c768270c9e384e4cbd268d6e67aebcfae6cd623b4d7c3bfde5a35db59"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
-            "version": "==1.4.3"
+            "markers": "python_version >= '3.7'",
+            "version": "==1.9.0"
+        },
+        "markdown-it-py": {
+            "hashes": [
+                "sha256:355216845c60bd96232cd8d8c40e8f9765cc86f46880e43a8fd22dc1a1a8cab1",
+                "sha256:e3f60a94fa066dc52ec76661e37c851cb232d92f9886b15cb560aaada2df8feb"
+            ],
+            "markers": "python_version >= '3.8'",
+            "version": "==3.0.0"
         },
         "markupsafe": {
             "hashes": [
-                "sha256:0212a68688482dc52b2d45013df70d169f542b7394fc744c02a57374a4207003",
-                "sha256:089cf3dbf0cd6c100f02945abeb18484bd1ee57a079aefd52cffd17fba910b88",
-                "sha256:10c1bfff05d95783da83491be968e8fe789263689c02724e0c691933c52994f5",
-                "sha256:33b74d289bd2f5e527beadcaa3f401e0df0a89927c1559c8566c066fa4248ab7",
-                "sha256:3799351e2336dc91ea70b034983ee71cf2f9533cdff7c14c90ea126bfd95d65a",
-                "sha256:3ce11ee3f23f79dbd06fb3d63e2f6af7b12db1d46932fe7bd8afa259a5996603",
-                "sha256:421be9fbf0ffe9ffd7a378aafebbf6f4602d564d34be190fc19a193232fd12b1",
-                "sha256:43093fb83d8343aac0b1baa75516da6092f58f41200907ef92448ecab8825135",
-                "sha256:46d00d6cfecdde84d40e572d63735ef81423ad31184100411e6e3388d405e247",
-                "sha256:4a33dea2b688b3190ee12bd7cfa29d39c9ed176bda40bfa11099a3ce5d3a7ac6",
-                "sha256:4b9fe39a2ccc108a4accc2676e77da025ce383c108593d65cc909add5c3bd601",
-                "sha256:56442863ed2b06d19c37f94d999035e15ee982988920e12a5b4ba29b62ad1f77",
-                "sha256:671cd1187ed5e62818414afe79ed29da836dde67166a9fac6d435873c44fdd02",
-                "sha256:694deca8d702d5db21ec83983ce0bb4b26a578e71fbdbd4fdcd387daa90e4d5e",
-                "sha256:6a074d34ee7a5ce3effbc526b7083ec9731bb3cbf921bbe1d3005d4d2bdb3a63",
-                "sha256:6d0072fea50feec76a4c418096652f2c3238eaa014b2f94aeb1d56a66b41403f",
-                "sha256:6fbf47b5d3728c6aea2abb0589b5d30459e369baa772e0f37a0320185e87c980",
-                "sha256:7f91197cc9e48f989d12e4e6fbc46495c446636dfc81b9ccf50bb0ec74b91d4b",
-                "sha256:86b1f75c4e7c2ac2ccdaec2b9022845dbb81880ca318bb7a0a01fbf7813e3812",
-                "sha256:8dc1c72a69aa7e082593c4a203dcf94ddb74bb5c8a731e4e1eb68d031e8498ff",
-                "sha256:8e3dcf21f367459434c18e71b2a9532d96547aef8a871872a5bd69a715c15f96",
-                "sha256:8e576a51ad59e4bfaac456023a78f6b5e6e7651dcd383bcc3e18d06f9b55d6d1",
-                "sha256:96e37a3dc86e80bf81758c152fe66dbf60ed5eca3d26305edf01892257049925",
-                "sha256:97a68e6ada378df82bc9f16b800ab77cbf4b2fada0081794318520138c088e4a",
-                "sha256:99a2a507ed3ac881b975a2976d59f38c19386d128e7a9a18b7df6fff1fd4c1d6",
-                "sha256:a49907dd8420c5685cfa064a1335b6754b74541bbb3706c259c02ed65b644b3e",
-                "sha256:b09bf97215625a311f669476f44b8b318b075847b49316d3e28c08e41a7a573f",
-                "sha256:b7bd98b796e2b6553da7225aeb61f447f80a1ca64f41d83612e6139ca5213aa4",
-                "sha256:b87db4360013327109564f0e591bd2a3b318547bcef31b468a92ee504d07ae4f",
-                "sha256:bcb3ed405ed3222f9904899563d6fc492ff75cce56cba05e32eff40e6acbeaa3",
-                "sha256:d4306c36ca495956b6d568d276ac11fdd9c30a36f1b6eb928070dc5360b22e1c",
-                "sha256:d5ee4f386140395a2c818d149221149c54849dfcfcb9f1debfe07a8b8bd63f9a",
-                "sha256:dda30ba7e87fbbb7eab1ec9f58678558fd9a6b8b853530e176eabd064da81417",
-                "sha256:e04e26803c9c3851c931eac40c695602c6295b8d432cbe78609649ad9bd2da8a",
-                "sha256:e1c0b87e09fa55a220f058d1d49d3fb8df88fbfab58558f1198e08c1e1de842a",
-                "sha256:e72591e9ecd94d7feb70c1cbd7be7b3ebea3f548870aa91e2732960fa4d57a37",
-                "sha256:e8c843bbcda3a2f1e3c2ab25913c80a3c5376cd00c6e8c4a86a89a28c8dc5452",
-                "sha256:efc1913fd2ca4f334418481c7e595c00aad186563bbc1ec76067848c7ca0a933",
-                "sha256:f121a1420d4e173a5d96e47e9a0c0dcff965afdf1626d28de1460815f7c4ee7a",
-                "sha256:fc7b548b17d238737688817ab67deebb30e8073c95749d55538ed473130ec0c7"
+                "sha256:05fb21170423db021895e1ea1e1f3ab3adb85d1c2333cbc2310f2a26bc77272e",
+                "sha256:0a4e4a1aff6c7ac4cd55792abf96c915634c2b97e3cc1c7129578aa68ebd754e",
+                "sha256:10bbfe99883db80bdbaff2dcf681dfc6533a614f700da1287707e8a5d78a8431",
+                "sha256:134da1eca9ec0ae528110ccc9e48041e0828d79f24121a1a146161103c76e686",
+                "sha256:1577735524cdad32f9f694208aa75e422adba74f1baee7551620e43a3141f559",
+                "sha256:1b40069d487e7edb2676d3fbdb2b0829ffa2cd63a2ec26c4938b2d34391b4ecc",
+                "sha256:282c2cb35b5b673bbcadb33a585408104df04f14b2d9b01d4c345a3b92861c2c",
+                "sha256:2c1b19b3aaacc6e57b7e25710ff571c24d6c3613a45e905b1fde04d691b98ee0",
+                "sha256:2ef12179d3a291be237280175b542c07a36e7f60718296278d8593d21ca937d4",
+                "sha256:338ae27d6b8745585f87218a3f23f1512dbf52c26c28e322dbe54bcede54ccb9",
+                "sha256:3c0fae6c3be832a0a0473ac912810b2877c8cb9d76ca48de1ed31e1c68386575",
+                "sha256:3fd4abcb888d15a94f32b75d8fd18ee162ca0c064f35b11134be77050296d6ba",
+                "sha256:42de32b22b6b804f42c5d98be4f7e5e977ecdd9ee9b660fda1a3edf03b11792d",
+                "sha256:504b320cd4b7eff6f968eddf81127112db685e81f7e36e75f9f84f0df46041c3",
+                "sha256:525808b8019e36eb524b8c68acdd63a37e75714eac50e988180b169d64480a00",
+                "sha256:56d9f2ecac662ca1611d183feb03a3fa4406469dafe241673d521dd5ae92a155",
+                "sha256:5bbe06f8eeafd38e5d0a4894ffec89378b6c6a625ff57e3028921f8ff59318ac",
+                "sha256:65c1a9bcdadc6c28eecee2c119465aebff8f7a584dd719facdd9e825ec61ab52",
+                "sha256:68e78619a61ecf91e76aa3e6e8e33fc4894a2bebe93410754bd28fce0a8a4f9f",
+                "sha256:69c0f17e9f5a7afdf2cc9fb2d1ce6aabdb3bafb7f38017c0b77862bcec2bbad8",
+                "sha256:6b2b56950d93e41f33b4223ead100ea0fe11f8e6ee5f641eb753ce4b77a7042b",
+                "sha256:787003c0ddb00500e49a10f2844fac87aa6ce977b90b0feaaf9de23c22508b24",
+                "sha256:7ef3cb2ebbf91e330e3bb937efada0edd9003683db6b57bb108c4001f37a02ea",
+                "sha256:8023faf4e01efadfa183e863fefde0046de576c6f14659e8782065bcece22198",
+                "sha256:8758846a7e80910096950b67071243da3e5a20ed2546e6392603c096778d48e0",
+                "sha256:8afafd99945ead6e075b973fefa56379c5b5c53fd8937dad92c662da5d8fd5ee",
+                "sha256:8c41976a29d078bb235fea9b2ecd3da465df42a562910f9022f1a03107bd02be",
+                "sha256:8e254ae696c88d98da6555f5ace2279cf7cd5b3f52be2b5cf97feafe883b58d2",
+                "sha256:9402b03f1a1b4dc4c19845e5c749e3ab82d5078d16a2a4c2cd2df62d57bb0707",
+                "sha256:962f82a3086483f5e5f64dbad880d31038b698494799b097bc59c2edf392fce6",
+                "sha256:9dcdfd0eaf283af041973bff14a2e143b8bd64e069f4c383416ecd79a81aab58",
+                "sha256:aa7bd130efab1c280bed0f45501b7c8795f9fdbeb02e965371bbef3523627779",
+                "sha256:ab4a0df41e7c16a1392727727e7998a467472d0ad65f3ad5e6e765015df08636",
+                "sha256:ad9e82fb8f09ade1c3e1b996a6337afac2b8b9e365f926f5a61aacc71adc5b3c",
+                "sha256:af598ed32d6ae86f1b747b82783958b1a4ab8f617b06fe68795c7f026abbdcad",
+                "sha256:b076b6226fb84157e3f7c971a47ff3a679d837cf338547532ab866c57930dbee",
+                "sha256:b7ff0f54cb4ff66dd38bebd335a38e2c22c41a8ee45aa608efc890ac3e3931bc",
+                "sha256:bfce63a9e7834b12b87c64d6b155fdd9b3b96191b6bd334bf37db7ff1fe457f2",
+                "sha256:c011a4149cfbcf9f03994ec2edffcb8b1dc2d2aede7ca243746df97a5d41ce48",
+                "sha256:c9c804664ebe8f83a211cace637506669e7890fec1b4195b505c214e50dd4eb7",
+                "sha256:ca379055a47383d02a5400cb0d110cef0a776fc644cda797db0c5696cfd7e18e",
+                "sha256:cb0932dc158471523c9637e807d9bfb93e06a95cbf010f1a38b98623b929ef2b",
+                "sha256:cd0f502fe016460680cd20aaa5a76d241d6f35a1c3350c474bac1273803893fa",
+                "sha256:ceb01949af7121f9fc39f7d27f91be8546f3fb112c608bc4029aef0bab86a2a5",
+                "sha256:d080e0a5eb2529460b30190fcfcc4199bd7f827663f858a226a81bc27beaa97e",
+                "sha256:dd15ff04ffd7e05ffcb7fe79f1b98041b8ea30ae9234aed2a9168b5797c3effb",
+                "sha256:df0be2b576a7abbf737b1575f048c23fb1d769f267ec4358296f31c2479db8f9",
+                "sha256:e09031c87a1e51556fdcb46e5bd4f59dfb743061cf93c4d6831bf894f125eb57",
+                "sha256:e4dd52d80b8c83fdce44e12478ad2e85c64ea965e75d66dbeafb0a3e77308fcc",
+                "sha256:fec21693218efe39aa7f8599346e90c705afa52c5b31ae019b2e57e8f6542bb2"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==2.1.1"
+            "version": "==2.1.3"
         },
         "mccabe": {
             "hashes": [
-                "sha256:ab8a6258860da4b6677da4bd2fe5dc2c659cff31b3ee4f7f5d64e79735b80d42",
-                "sha256:dd8d182285a0fe56bace7f45b5e7d1a6ebcbf524e8f3bd87eb0f125271b8831f"
+                "sha256:348e0240c33b60bbdf4e523192ef919f28cb2c3d7d5c7794f74009290f236325",
+                "sha256:6c2d30ab6be0e4a46919781807b4f0d834ebdd6c6e3dca0bda5a15f863427b6e"
             ],
-            "version": "==0.6.1"
+            "markers": "python_version >= '3.6'",
+            "version": "==0.7.0"
+        },
+        "mdurl": {
+            "hashes": [
+                "sha256:84008a41e51615a49fc9966191ff91509e3c40b939176e643fd50a5c2196b8f8",
+                "sha256:bb413d29f5eea38f31dd4754dd7377d4465116fb207585f97bf925588687c1ba"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==0.1.2"
+        },
+        "more-itertools": {
+            "hashes": [
+                "sha256:cabaa341ad0389ea83c17a94566a53ae4c9d07349861ecb14dc6d0345cf9ac5d",
+                "sha256:d2bc7f02446e86a68911e58ded76d6561eea00cddfb2a91e7019bbb586c799f3"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==9.1.0"
         },
         "nose": {
             "hashes": [
                 "sha256:9ff7c6cc443f8c51994b34a667bbcf45afd6d945be7477b52e97516fd17c53ac",
                 "sha256:dadcddc0aefbf99eea214e0f1232b94f2fa9bd98fa8353711dacb112bfcbbb2a",
                 "sha256:f1bffef9cbc82628f6e7d7b40d7e255aefaa1adb6a1b1d26c69a8b79e6208a98"
             ],
@@ -343,125 +559,111 @@
                 "sha256:ab2d0dca21aa5a7ae280c6fb869882260b825d9ced368b557b9124cf51ffb119"
             ],
             "index": "pypi",
             "version": "==0.6.0"
         },
         "packaging": {
             "hashes": [
-                "sha256:dd47c42927d89ab911e606518907cc2d3a1f38bbd026385970643f9c5b8ecfeb",
-                "sha256:ef103e05f519cdc783ae24ea4e2e0f508a9c99b2d4969652eed6a2e1ea5bd522"
+                "sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61",
+                "sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==21.3"
+            "markers": "python_version >= '3.7'",
+            "version": "==23.1"
         },
         "pep8-naming": {
             "hashes": [
                 "sha256:5d9f1056cb9427ce344e98d1a7f5665710e2f20f748438e308995852cfa24164",
                 "sha256:f3b4a5f9dd72b991bf7d8e2a341d2e1aa3a884a769b5aaac4f56825c1763bf3a"
             ],
             "version": "==0.10.0"
         },
         "pkginfo": {
             "hashes": [
-                "sha256:542e0d0b6750e2e21c20179803e40ab50598d8066d51097a0e382cba9eb02bff",
-                "sha256:c24c487c6a7f72c66e816ab1796b96ac6c3d14d49338293d2141664330b55ffc"
+                "sha256:4b7a555a6d5a22169fcc9cf7bfd78d296b0361adad412a346c1226849af5e546",
+                "sha256:8fd5896e8718a4372f0ea9cc9d96f6417c9b986e23a4d116dda26b62cc29d046"
             ],
-            "version": "==1.8.2"
+            "markers": "python_version >= '3.6'",
+            "version": "==1.9.6"
         },
         "platformdirs": {
             "hashes": [
-                "sha256:7535e70dfa32e84d4b34996ea99c5e432fa29a708d0f4e394bbcb2a8faa4f16d",
-                "sha256:bcae7cab893c2d310a711b70b24efb93334febe65f8de776ee320b517471e227"
+                "sha256:0ade98a4895e87dc51d47151f7d2ec290365a585151d97b4d8d6312ed6132fed",
+                "sha256:e48fabd87db8f3a7df7150a4a5ea22c546ee8bc39bc2473244730d4b56d2cc4e"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==2.5.1"
+            "version": "==3.5.3"
         },
         "pluggy": {
             "hashes": [
-                "sha256:15b2acde666561e1298d71b523007ed7364de07029219b604cf808bfa1c765b0",
-                "sha256:966c145cd83c96502c3c3868f50408687b38434af77734af1e9ca461a4081d2d"
+                "sha256:4224373bacce55f955a878bf9cfa763c1e360858e330072059e10bad68531159",
+                "sha256:74134bbf457f031a36d68416e1509f34bd5ccc019f0bcc952c7b909d06b37bd3"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
-            "version": "==0.13.1"
-        },
-        "poetry-semver": {
-            "hashes": [
-                "sha256:4e6349bd7231cc657f0e1930f7b204e87e33dfd63eef5cac869363969515083a",
-                "sha256:d809b612aa27b39bf2d0fc9d31b4f4809b0e972646c5f19cfa46c725b7638810"
-            ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
-            "version": "==0.1.0"
+            "markers": "python_version >= '3.6'",
+            "version": "==1.0.0"
         },
         "prospector": {
             "hashes": [
-                "sha256:700d7918d93d73035a2a58fb18c6be0b609a0481fc6e0908843fa856b89e52c6"
+                "sha256:3bfe103c28bb821cca84926ca31357fbfd32405e4bf8c34ca2e55885684557e4",
+                "sha256:cc8f09e79bdd32247edddf05b666940e88ad96338a84f5717b1e8c0678337821"
             ],
             "index": "pypi",
-            "version": "==1.3.1"
-        },
-        "py": {
-            "hashes": [
-                "sha256:51c75c4126074b472f746a24399ad32f6053d1b34b68d2fa41e558e6f4a98719",
-                "sha256:607c53218732647dff4acdfcd50cb62615cedf612e72d1724fb1a0cc6405b378"
-            ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
-            "version": "==1.11.0"
+            "version": "==1.10.2"
         },
         "pycodestyle": {
             "hashes": [
-                "sha256:2295e7b2f6b5bd100585ebcb1f616591b652db8a741695b3d8f5d28bdc934367",
-                "sha256:c58a7d2815e0e8d7972bf1803331fb0152f867bd89adf8a01dfd55085434192e"
+                "sha256:2c9607871d58c76354b697b42f5d57e1ada7d261c261efac224b664affdc5785",
+                "sha256:d1735fc58b418fd7c5f658d28d943854f8a849b01a5d0a1e6f3f3fdd0166804b"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
-            "version": "==2.6.0"
+            "markers": "python_version >= '3.6'",
+            "version": "==2.9.1"
         },
         "pydocstyle": {
             "hashes": [
-                "sha256:1d41b7c459ba0ee6c345f2eb9ae827cab14a7533a88c5c6f7e94923f72df92dc",
-                "sha256:6987826d6775056839940041beef5c08cc7e3d71d63149b48e36727f70144dc4"
+                "sha256:118762d452a49d6b05e194ef344a55822987a462831ade91ec5c06fd2169d019",
+                "sha256:7ce43f0c0ac87b07494eb9c0b462c0b73e6ff276807f204d6b53edc72b7e44e1"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==6.1.1"
+            "version": "==6.3.0"
         },
         "pyflakes": {
             "hashes": [
-                "sha256:0d94e0e05a19e57a99444b6ddcf9a6eb2e5c68d3ca1e98e90707af8152c90a92",
-                "sha256:35b2d75ee967ea93b55750aa9edbbf72813e06a66ba54438df2cfac9e3c27fc8"
+                "sha256:4579f67d887f804e67edb544428f264b7b24f435b263c4614f384135cea553d2",
+                "sha256:491feb020dca48ccc562a8c0cbe8df07ee13078df59813b83959cbdada312ea3"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
-            "version": "==2.2.0"
+            "markers": "python_version >= '3.6'",
+            "version": "==2.5.0"
         },
         "pygments": {
             "hashes": [
-                "sha256:44238f1b60a76d78fc8ca0528ee429702aae011c265fe6a8dd8b63049ae41c65",
-                "sha256:4e426f72023d88d03b2fa258de560726ce890ff3b630f88c21cbb8b2503b8c6a"
+                "sha256:8ace4d3c1dd481894b2005f560ead0f9f19ee64fe983366be1a21e171d12775c",
+                "sha256:db2db3deb4b4179f399a09054b023b6a586b76499d36965813c71aa8ed7b5fd1"
             ],
-            "markers": "python_version >= '3.5'",
-            "version": "==2.11.2"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.15.1"
         },
         "pylint": {
             "hashes": [
-                "sha256:7dd78437f2d8d019717dbf287772d0b2dbdfd13fc016aa7faa08d67bccc46adc",
-                "sha256:d0ece7d223fe422088b0e8f13fa0a1e8eb745ebffcb8ed53d3e95394b6101a1c"
+                "sha256:5dcf1d9e19f41f38e4e85d10f511e5b9c35e1aa74251bf95cdd8cb23584e2db1",
+                "sha256:7a1145fb08c251bdb5cca11739722ce64a63db479283d10ce718b2460e54123c"
             ],
-            "markers": "python_version >= '3.5'",
-            "version": "==2.5.3"
+            "markers": "python_full_version >= '3.7.2'",
+            "version": "==2.17.4"
         },
         "pylint-celery": {
             "hashes": [
                 "sha256:41e32094e7408d15c044178ea828dd524beedbdbe6f83f712c5e35bde1de4beb"
             ],
             "version": "==0.3"
         },
         "pylint-django": {
             "hashes": [
-                "sha256:b7756844dba0cecd3471056a1ef4154439defedaba38bf3ced9f848d2bf6297c",
-                "sha256:ca32277c77878dd3c2d9e75f3f3f7f0c0712f053f10ff1b946cdc27367a6c911"
+                "sha256:0ac090d106c62fe33782a1d01bda1610b761bb1c9bf5035ced9d5f23a13d8591",
+                "sha256:56b12b6adf56d548412445bd35483034394a1a94901c3f8571980a13882299d5"
             ],
-            "version": "==2.1.0"
+            "version": "==2.5.3"
         },
         "pylint-flask": {
             "hashes": [
                 "sha256:f4d97de2216bf7bfce07c9c08b166e978fe9f2725de2a50a9845a97de7e31517"
             ],
             "version": "==0.6"
         },
@@ -469,186 +671,201 @@
             "hashes": [
                 "sha256:b3d43e85ab74c4f48bb46ae4ce771e39c3a20f8b3d56982ab17aa73b4f98d535",
                 "sha256:ce48bc0516ae9415dd5c752c940dfe601b18fe0f48aa249f2386adfa95a004dd"
             ],
             "markers": "python_full_version >= '3.6.2'",
             "version": "==0.7"
         },
-        "pyparsing": {
-            "hashes": [
-                "sha256:18ee9022775d270c55187733956460083db60b37d0d0fb357445f3094eed3eea",
-                "sha256:a6c06a88f252e6c322f65faf8f418b16213b51bdfaece0524c1c1bc30c63c484"
-            ],
-            "markers": "python_version >= '3.6'",
-            "version": "==3.0.7"
-        },
-        "pytz": {
+        "pyproject-api": {
             "hashes": [
-                "sha256:1e760e2fe6a8163bc0b3d9a19c4f84342afa0a2affebfaa84b01b978a02ecaa7",
-                "sha256:e68985985296d9a66a881eb3193b0906246245294a881e7c8afe623866ac6a5c"
+                "sha256:435f46547a9ff22cf4208ee274fca3e2869aeb062a4834adfc99a4dd64af3cf9",
+                "sha256:4698a3777c2e0f6b624f8a4599131e2a25376d90fe8d146d7ac74c67c6f97c43"
             ],
-            "version": "==2022.1"
+            "markers": "python_version >= '3.7'",
+            "version": "==1.5.1"
         },
         "pyyaml": {
             "hashes": [
+                "sha256:01b45c0191e6d66c470b6cf1b9531a771a83c1c4208272ead47a3ae4f2f603bf",
                 "sha256:0283c35a6a9fbf047493e3a0ce8d79ef5030852c51e9d911a27badfde0605293",
                 "sha256:055d937d65826939cb044fc8c9b08889e8c743fdc6a32b33e2390f66013e449b",
                 "sha256:07751360502caac1c067a8132d150cf3d61339af5691fe9e87803040dbc5db57",
                 "sha256:0b4624f379dab24d3725ffde76559cff63d9ec94e1736b556dacdfebe5ab6d4b",
                 "sha256:0ce82d761c532fe4ec3f87fc45688bdd3a4c1dc5e0b4a19814b9009a29baefd4",
                 "sha256:1e4747bc279b4f613a09eb64bba2ba602d8a6664c6ce6396a4d0cd413a50ce07",
                 "sha256:213c60cd50106436cc818accf5baa1aba61c0189ff610f64f4a3e8c6726218ba",
                 "sha256:231710d57adfd809ef5d34183b8ed1eeae3f76459c18fb4a0b373ad56bedcdd9",
                 "sha256:277a0ef2981ca40581a47093e9e2d13b3f1fbbeffae064c1d21bfceba2030287",
                 "sha256:2cd5df3de48857ed0544b34e2d40e9fac445930039f3cfe4bcc592a1f836d513",
                 "sha256:40527857252b61eacd1d9af500c3337ba8deb8fc298940291486c465c8b46ec0",
+                "sha256:432557aa2c09802be39460360ddffd48156e30721f5e8d917f01d31694216782",
                 "sha256:473f9edb243cb1935ab5a084eb238d842fb8f404ed2193a915d1784b5a6b5fc0",
                 "sha256:48c346915c114f5fdb3ead70312bd042a953a8ce5c7106d5bfb1a5254e47da92",
                 "sha256:50602afada6d6cbfad699b0c7bb50d5ccffa7e46a3d738092afddc1f9758427f",
                 "sha256:68fb519c14306fec9720a2a5b45bc9f0c8d1b9c72adf45c37baedfcd949c35a2",
                 "sha256:77f396e6ef4c73fdc33a9157446466f1cff553d979bd00ecb64385760c6babdc",
+                "sha256:81957921f441d50af23654aa6c5e5eaf9b06aba7f0a19c18a538dc7ef291c5a1",
                 "sha256:819b3830a1543db06c4d4b865e70ded25be52a2e0631ccd2f6a47a2822f2fd7c",
                 "sha256:897b80890765f037df3403d22bab41627ca8811ae55e9a722fd0392850ec4d86",
                 "sha256:98c4d36e99714e55cfbaaee6dd5badbc9a1ec339ebfc3b1f52e293aee6bb71a4",
                 "sha256:9df7ed3b3d2e0ecfe09e14741b857df43adb5a3ddadc919a2d94fbdf78fea53c",
                 "sha256:9fa600030013c4de8165339db93d182b9431076eb98eb40ee068700c9c813e34",
                 "sha256:a80a78046a72361de73f8f395f1f1e49f956c6be882eed58505a15f3e430962b",
+                "sha256:afa17f5bc4d1b10afd4466fd3a44dc0e245382deca5b3c353d8b757f9e3ecb8d",
                 "sha256:b3d267842bf12586ba6c734f89d1f5b871df0273157918b0ccefa29deb05c21c",
                 "sha256:b5b9eccad747aabaaffbc6064800670f0c297e52c12754eb1d976c57e4f74dcb",
+                "sha256:bfaef573a63ba8923503d27530362590ff4f576c626d86a9fed95822a8255fd7",
                 "sha256:c5687b8d43cf58545ade1fe3e055f70eac7a5a1a0bf42824308d868289a95737",
                 "sha256:cba8c411ef271aa037d7357a2bc8f9ee8b58b9965831d9e51baf703280dc73d3",
                 "sha256:d15a181d1ecd0d4270dc32edb46f7cb7733c7c508857278d3d378d14d606db2d",
+                "sha256:d4b0ba9512519522b118090257be113b9468d804b19d63c71dbcf4a48fa32358",
                 "sha256:d4db7c7aef085872ef65a8fd7d6d09a14ae91f691dec3e87ee5ee0539d516f53",
                 "sha256:d4eccecf9adf6fbcc6861a38015c2a64f38b9d94838ac1810a9023a0609e1b78",
                 "sha256:d67d839ede4ed1b28a4e8909735fc992a923cdb84e618544973d7dfc71540803",
                 "sha256:daf496c58a8c52083df09b80c860005194014c3698698d1a57cbcfa182142a3a",
+                "sha256:dbad0e9d368bb989f4515da330b88a057617d16b6a8245084f1b05400f24609f",
                 "sha256:e61ceaab6f49fb8bdfaa0f92c4b57bcfbea54c09277b1b4f7ac376bfb7a7c174",
                 "sha256:f84fbc98b019fef2ee9a1cb3ce93e3187a6df0b2538a651bfb890254ba9f90b5"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==6.0"
         },
         "readme-renderer": {
             "hashes": [
-                "sha256:262510fe6aae81ed4e94d8b169077f325614c0b1a45916a80442c6576264a9c2",
-                "sha256:dfb4d17f21706d145f7473e0b61ca245ba58e810cf9b2209a48239677f82e5b0"
+                "sha256:cd653186dfc73055656f090f227f5cb22a046d7f71a841dfa305f55c9a513273",
+                "sha256:f67a16caedfa71eef48a31b39708637a6f4664c4394801a7b0d6432d13907343"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==34.0"
+            "markers": "python_version >= '3.7'",
+            "version": "==37.3"
         },
         "requests": {
             "hashes": [
-                "sha256:68d7c56fd5a8999887728ef304a6d12edc7be74f1cfa47714fc8b414525c9a61",
-                "sha256:f22fa1e554c9ddfd16e6e41ac79759e17be9e492b3587efa038054674760e72d"
+                "sha256:58cd2187c01e70e6e26505bca751777aa9f2ee0b7f4300988b709f44e013003f",
+                "sha256:942c5a758f98d790eaed1a29cb6eefc7ffb0d1cf7af05c3d2791656dbd6ad1e1"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'",
-            "version": "==2.27.1"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.31.0"
         },
         "requests-toolbelt": {
             "hashes": [
-                "sha256:380606e1d10dc85c3bd47bf5a6095f815ec007be7a8b69c878507068df059e6f",
-                "sha256:968089d4584ad4ad7c171454f0a5c6dac23971e9472521ea3b6d49d610aa6fc0"
+                "sha256:7681a0a3d047012b5bdc0ee37d7f8f07ebe76ab08caeccfc3921ce23c88d5bc6",
+                "sha256:cccfdd665f0a24fcf4726e690f65639d272bb0637b9b92dfd91a5568ccf6bd06"
             ],
-            "version": "==0.9.1"
+            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
+            "version": "==1.0.0"
         },
         "requirements-detector": {
             "hashes": [
-                "sha256:6c32d39a36612a20d4b0d29e9b6ffbf82a42ce7aa9f8a2f620ac467cccaf8bc2",
-                "sha256:98ef5113d991f2aa30b229fe6f63f2878c7e35326e9e21d71ef8113021e2eefa"
+                "sha256:3642cd7a5b261d79536c36bb7ecacf2adabd902d2e0e42bfb2ba82515da10501",
+                "sha256:d7c60493bf166da3dd59de0e6cb25765e0e32a1931aeae92614034e5786d0bd0"
             ],
-            "markers": "python_version < '4' and python_full_version >= '3.6.2'",
-            "version": "==1.0.2"
+            "markers": "python_version >= '3.7' and python_version < '4.0'",
+            "version": "==1.2.2"
         },
-        "semver": {
+        "rfc3986": {
             "hashes": [
-                "sha256:41c9aa26c67dc16c54be13074c352ab666bce1fa219c7110e8f03374cd4206b0",
-                "sha256:5b09010a66d9a3837211bb7ae5a20d10ba88f8cb49e92cb139a69ef90d5060d8"
+                "sha256:50b1502b60e289cb37883f3dfd34532b8873c7de9f49bb546641ce9cbd256ebd",
+                "sha256:97aacf9dbd4bfd829baad6e6309fa6573aaf1be3f6fa735c8ab05e46cecb261c"
             ],
-            "index": "pypi",
-            "version": "==2.8.1"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.0.0"
         },
-        "setoptconf": {
+        "rich": {
             "hashes": [
-                "sha256:1fa613dc4a6fbfbaab9a52319d1e369d030e8ed80455b151574ccf3390ec86c6",
-                "sha256:d2ecbd27c0c7d0d53990e2df98d9aad6490df8b75b71c621d8c441d6e91e3161"
+                "sha256:8f87bc7ee54675732fa66a05ebfe489e27264caeeff3728c945d25971b6485ec",
+                "sha256:d653d6bccede5844304c605d5aac802c7cf9621efd700b46c7ec2b51ea914898"
             ],
-            "markers": "python_version >= '3.0'",
-            "version": "==0.3.0"
+            "markers": "python_full_version >= '3.7.0'",
+            "version": "==13.4.2"
         },
-        "setuptools": {
+        "semver": {
             "hashes": [
-                "sha256:6599055eeb23bfef457d5605d33a4d68804266e6cb430b0fb12417c5efeae36c",
-                "sha256:782ef48d58982ddb49920c11a0c5c9c0b02e7d7d1c2ad0aa44e1a1e133051c96"
+                "sha256:94df43924c4521ec7d307fc86da1531db6c2c33d9d5cdc3e64cca0eb68569269",
+                "sha256:ab4f69fb1d1ecfb5d81f96411403d7a611fa788c45d252cf5b408025df3ab6ce"
             ],
-            "markers": "python_version >= '3.7'",
-            "version": "==60.10.0"
+            "index": "pypi",
+            "version": "==3.0.0"
         },
-        "sh": {
+        "setoptconf-tmp": {
             "hashes": [
-                "sha256:ae3258c5249493cebe73cb4e18253a41ed69262484bad36fdb3efcb8ad8870bb",
-                "sha256:b52bf5833ed01c7b5c5fb73a7f71b3d98d48e9b9b8764236237bdc7ecae850fc"
+                "sha256:76035d5cd1593d38b9056ae12d460eca3aaa34ad05c315b69145e138ba80a745",
+                "sha256:e0480addd11347ba52f762f3c4d8afa3e10ad0affbc53e3ffddc0ca5f27d5778"
             ],
-            "index": "pypi",
-            "markers": "sys_platform != 'win32'",
-            "version": "==1.12.14"
+            "version": "==0.3.1"
         },
         "six": {
             "hashes": [
                 "sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926",
                 "sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
             "version": "==1.16.0"
         },
+        "smmap": {
+            "hashes": [
+                "sha256:2aba19d6a040e78d8b09de5c57e96207b09ed71d8e55ce0959eeee6c8e190d94",
+                "sha256:c840e62059cd3be204b0c9c9f74be2c09d5648eddd4580d9314c3ecde0b30936"
+            ],
+            "markers": "python_version >= '3.6'",
+            "version": "==5.0.0"
+        },
         "snowballstemmer": {
             "hashes": [
                 "sha256:09b16deb8547d3412ad7b590689584cd0fe25ec8db3be37788be3810cbf19cb1",
                 "sha256:c8e1716e83cc398ae16824e5572ae04e0d9fc2c6b985fb0f900f5f0c96ecba1a"
             ],
             "version": "==2.2.0"
         },
         "sphinx": {
             "hashes": [
-                "sha256:22538e1bbe62b407cf5a8aabe1bb15848aa66bb79559f42f5202bbce6b757a69",
-                "sha256:f9a79e746b87921cabc3baa375199c6076d1270cee53915dbd24fdbeaaacc427"
+                "sha256:6d56a34697bb749ffa0152feafc4b19836c755d90a7c59b72bc7dfd371b9cc6b",
+                "sha256:97787ff1fa3256a3eef9eda523a63dbf299f7b47e053cfcf684a1c2a8380c912"
             ],
             "index": "pypi",
-            "version": "==2.1.2"
+            "version": "==6.2.1"
         },
         "sphinx-rtd-theme": {
             "hashes": [
-                "sha256:00cf895504a7895ee433807c62094cf1e95f065843bf3acd17037c3e9a2becd4",
-                "sha256:728607e34d60456d736cc7991fd236afb828b21b82f956c5ea75f94c8414040a"
+                "sha256:01c5c5a72e2d025bd23d1f06c59a4831b06e6ce6c01fdd5ebfe9986c0a880fc7",
+                "sha256:6a7e7d8af34eb8fc57d52a09c6b6b9c46ff44aea5951bc831eeb9245378f3689"
             ],
             "index": "pypi",
-            "version": "==0.4.3"
+            "version": "==1.2.2"
         },
         "sphinxcontrib-applehelp": {
             "hashes": [
-                "sha256:806111e5e962be97c29ec4c1e7fe277bfd19e9652fb1a4392105b43e01af885a",
-                "sha256:a072735ec80e7675e3f432fcae8610ecf509c5f1869d17e2eecff44389cdbc58"
+                "sha256:29d341f67fb0f6f586b23ad80e072c8e6ad0b48417db2bde114a4c9746feb228",
+                "sha256:828f867945bbe39817c210a1abfd1bc4895c8b73fcaade56d45357a348a07d7e"
             ],
-            "markers": "python_version >= '3.5'",
-            "version": "==1.0.2"
+            "markers": "python_version >= '3.8'",
+            "version": "==1.0.4"
         },
         "sphinxcontrib-devhelp": {
             "hashes": [
                 "sha256:8165223f9a335cc1af7ffe1ed31d2871f325254c0423bc0c4c7cd1c1e4734a2e",
                 "sha256:ff7f1afa7b9642e7060379360a67e9c41e8f3121f2ce9164266f61b9f4b338e4"
             ],
             "markers": "python_version >= '3.5'",
             "version": "==1.0.2"
         },
         "sphinxcontrib-htmlhelp": {
             "hashes": [
-                "sha256:d412243dfb797ae3ec2b59eca0e52dac12e75a241bf0e4eb861e450d06c6ed07",
-                "sha256:f5f8bb2d0d629f398bf47d0d69c07bc13b65f75a81ad9e2f71a63d4b7a2f6db2"
+                "sha256:0cbdd302815330058422b98a113195c9249825d681e18f11e8b1f78a2f11efff",
+                "sha256:c38cb46dccf316c79de6e5515e1770414b797162b23cd3d06e67020e1d2a6903"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==2.0.0"
+            "markers": "python_version >= '3.8'",
+            "version": "==2.0.1"
+        },
+        "sphinxcontrib-jquery": {
+            "hashes": [
+                "sha256:1620739f04e36a2c779f1a131a2dfd49b2fd07351bf1968ced074365933abc7a",
+                "sha256:f936030d7d0147dd026a4f2b5a57343d233f1fc7b363f68b3d4f1cb0993878ae"
+            ],
+            "markers": "python_version >= '2.7'",
+            "version": "==4.1"
         },
         "sphinxcontrib-jsmath": {
             "hashes": [
                 "sha256:2ec2eaebfb78f3f2078e73666b1415417a116cc848b72e5172e596c871103178",
                 "sha256:a9925e4a4587247ed2191a22df5f6970656cb8ca2bd6284309578f2153e0c4b8"
             ],
             "markers": "python_version >= '3.5'",
@@ -674,170 +891,161 @@
             "hashes": [
                 "sha256:806143ae5bfb6a3c6e736a764057db0e6a0e05e338b5630894a5f779cabb4f9b",
                 "sha256:b3bda1d108d5dd99f4a20d24d9c348e91c4db7ab1b749200bded2f839ccbe68f"
             ],
             "index": "pypi",
             "version": "==0.10.2"
         },
-        "tox": {
+        "tomli": {
             "hashes": [
-                "sha256:dab0b0160dd187b654fc33d690ee1d7bf328bd5b8dc6ef3bb3cc468969c659ba",
-                "sha256:ee35ffce74933a6c6ac10c9a0182e41763140a5a5070e21b114feca56eaccdcd"
+                "sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc",
+                "sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f"
             ],
-            "index": "pypi",
-            "version": "==3.13.2"
+            "markers": "python_version < '3.11'",
+            "version": "==2.0.1"
         },
-        "tqdm": {
+        "tomlkit": {
             "hashes": [
-                "sha256:1d9835ede8e394bb8c9dcbffbca02d717217113adc679236873eeaac5bc0b3cd",
-                "sha256:e643e071046f17139dea55b880dc9b33822ce21613b4a4f5ea57f202833dbc29"
+                "sha256:8c726c4c202bdb148667835f68d68780b9a003a9ec34167b6c673b38eff2a171",
+                "sha256:9330fc7faa1db67b541b28e62018c17d20be733177d290a13b24c62d1614e0c3"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
-            "version": "==4.63.0"
+            "markers": "python_version >= '3.7'",
+            "version": "==0.11.8"
+        },
+        "tox": {
+            "hashes": [
+                "sha256:4874000453e637a87ca892f9744a2ab9a7d24064dad1b0ecbf5a4c3c146cc732",
+                "sha256:954f1f647f67f481d239a193288983242a6152b67503c4a56b19a4aafaa29736"
+            ],
+            "index": "pypi",
+            "version": "==4.6.0"
         },
         "twine": {
             "hashes": [
-                "sha256:0fb0bfa3df4f62076cab5def36b1a71a2e4acb4d1fa5c97475b048117b1a6446",
-                "sha256:d6c29c933ecfc74e9b1d9fa13aa1f87c5d5770e119f5a4ce032092f0ff5b14dc"
+                "sha256:929bc3c280033347a00f847236564d1c52a3e61b1ac2516c97c48f3ceab756d8",
+                "sha256:9e102ef5fdd5a20661eb88fad46338806c3bd32cf1db729603fe3697b1bc83c8"
             ],
             "index": "pypi",
-            "version": "==1.13.0"
+            "version": "==4.0.2"
         },
-        "typed-ast": {
+        "typing-extensions": {
             "hashes": [
-                "sha256:01ae5f73431d21eead5015997ab41afa53aa1fbe252f9da060be5dad2c730ace",
-                "sha256:067a74454df670dcaa4e59349a2e5c81e567d8d65458d480a5b3dfecec08c5ff",
-                "sha256:0fb71b8c643187d7492c1f8352f2c15b4c4af3f6338f21681d3681b3dc31a266",
-                "sha256:1b3ead4a96c9101bef08f9f7d1217c096f31667617b58de957f690c92378b528",
-                "sha256:2068531575a125b87a41802130fa7e29f26c09a2833fea68d9a40cf33902eba6",
-                "sha256:209596a4ec71d990d71d5e0d312ac935d86930e6eecff6ccc7007fe54d703808",
-                "sha256:2c726c276d09fc5c414693a2de063f521052d9ea7c240ce553316f70656c84d4",
-                "sha256:398e44cd480f4d2b7ee8d98385ca104e35c81525dd98c519acff1b79bdaac363",
-                "sha256:52b1eb8c83f178ab787f3a4283f68258525f8d70f778a2f6dd54d3b5e5fb4341",
-                "sha256:5feca99c17af94057417d744607b82dd0a664fd5e4ca98061480fd8b14b18d04",
-                "sha256:7538e495704e2ccda9b234b82423a4038f324f3a10c43bc088a1636180f11a41",
-                "sha256:760ad187b1041a154f0e4d0f6aae3e40fdb51d6de16e5c99aedadd9246450e9e",
-                "sha256:777a26c84bea6cd934422ac2e3b78863a37017618b6e5c08f92ef69853e765d3",
-                "sha256:95431a26309a21874005845c21118c83991c63ea800dd44843e42a916aec5899",
-                "sha256:9ad2c92ec681e02baf81fdfa056fe0d818645efa9af1f1cd5fd6f1bd2bdfd805",
-                "sha256:9c6d1a54552b5330bc657b7ef0eae25d00ba7ffe85d9ea8ae6540d2197a3788c",
-                "sha256:aee0c1256be6c07bd3e1263ff920c325b59849dc95392a05f258bb9b259cf39c",
-                "sha256:af3d4a73793725138d6b334d9d247ce7e5f084d96284ed23f22ee626a7b88e39",
-                "sha256:b36b4f3920103a25e1d5d024d155c504080959582b928e91cb608a65c3a49e1a",
-                "sha256:b9574c6f03f685070d859e75c7f9eeca02d6933273b5e69572e5ff9d5e3931c3",
-                "sha256:bff6ad71c81b3bba8fa35f0f1921fb24ff4476235a6e94a26ada2e54370e6da7",
-                "sha256:c190f0899e9f9f8b6b7863debfb739abcb21a5c054f911ca3596d12b8a4c4c7f",
-                "sha256:c907f561b1e83e93fad565bac5ba9c22d96a54e7ea0267c708bffe863cbe4075",
-                "sha256:cae53c389825d3b46fb37538441f75d6aecc4174f615d048321b716df2757fb0",
-                "sha256:dd4a21253f42b8d2b48410cb31fe501d32f8b9fbeb1f55063ad102fe9c425e40",
-                "sha256:dde816ca9dac1d9c01dd504ea5967821606f02e510438120091b84e852367428",
-                "sha256:f2362f3cb0f3172c42938946dbc5b7843c2a28aec307c49100c8b38764eb6927",
-                "sha256:f328adcfebed9f11301eaedfa48e15bdece9b519fb27e6a8c01aa52a17ec31b3",
-                "sha256:f8afcf15cc511ada719a88e013cec87c11aff7b91f019295eb4530f96fe5ef2f",
-                "sha256:fb1bbeac803adea29cedd70781399c99138358c26d05fcbd23c13016b7f5ec65"
+                "sha256:88a4153d8505aabbb4e13aacb7c486c2b4a33ca3b3f807914a9b4c844c471c26",
+                "sha256:d91d5919357fe7f681a9f2b5b4cb2a5f1ef0a1e9f59c4d8ff0d3491e05c0ffd5"
             ],
-            "markers": "python_version < '3.8' and implementation_name == 'cpython'",
-            "version": "==1.4.3"
+            "markers": "python_version < '3.10'",
+            "version": "==4.6.3"
         },
         "urllib3": {
             "hashes": [
-                "sha256:44ece4d53fb1706f667c9bd1c648f5469a2ec925fcf3a776667042d645472c14",
-                "sha256:aabaf16477806a5e1dd19aa41f8c2b7950dd3c746362d7e3223dbe6de6ac448e"
+                "sha256:48e7fafa40319d358848e1bc6809b208340fafe2096f1725d05d67443d0483d1",
+                "sha256:bee28b5e56addb8226c96f7f13ac28cb4c301dd5ea8a6ca179c0b9835e032825"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4' and python_version < '4'",
-            "version": "==1.26.9"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.0.3"
         },
         "virtualenv": {
             "hashes": [
-                "sha256:c3e01300fb8495bc00ed70741f5271fc95fed067eb7106297be73d30879af60c",
-                "sha256:ce8901d3bbf3b90393498187f2d56797a8a452fb2d0d7efc6fd837554d6f679c"
+                "sha256:6abec7670e5802a528357fdc75b26b9f57d5d92f29c5462ba0fbe45feacc685e",
+                "sha256:a85caa554ced0c0afbd0d638e7e2d7b5f92d23478d05d17a76daeac8f279f924"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
-            "version": "==20.13.4"
+            "markers": "python_version >= '3.7'",
+            "version": "==20.23.0"
         },
         "webencodings": {
             "hashes": [
                 "sha256:a0af1213f3c2226497a97e2b3aa01a7e4bee4f403f95be16fc9acd2947514a78",
                 "sha256:b36a1c245f2d304965eb4e0a82848379241dc04b865afcc4aab16748587e1923"
             ],
             "version": "==0.5.1"
         },
         "wrapt": {
             "hashes": [
-                "sha256:00108411e0f34c52ce16f81f1d308a571df7784932cc7491d1e94be2ee93374b",
-                "sha256:01f799def9b96a8ec1ef6b9c1bbaf2bbc859b87545efbecc4a78faea13d0e3a0",
-                "sha256:09d16ae7a13cff43660155383a2372b4aa09109c7127aa3f24c3cf99b891c330",
-                "sha256:14e7e2c5f5fca67e9a6d5f753d21f138398cad2b1159913ec9e9a67745f09ba3",
-                "sha256:167e4793dc987f77fd476862d32fa404d42b71f6a85d3b38cbce711dba5e6b68",
-                "sha256:1807054aa7b61ad8d8103b3b30c9764de2e9d0c0978e9d3fc337e4e74bf25faa",
-                "sha256:1f83e9c21cd5275991076b2ba1cd35418af3504667affb4745b48937e214bafe",
-                "sha256:21b1106bff6ece8cb203ef45b4f5778d7226c941c83aaaa1e1f0f4f32cc148cd",
-                "sha256:22626dca56fd7f55a0733e604f1027277eb0f4f3d95ff28f15d27ac25a45f71b",
-                "sha256:23f96134a3aa24cc50614920cc087e22f87439053d886e474638c68c8d15dc80",
-                "sha256:2498762814dd7dd2a1d0248eda2afbc3dd9c11537bc8200a4b21789b6df6cd38",
-                "sha256:28c659878f684365d53cf59dc9a1929ea2eecd7ac65da762be8b1ba193f7e84f",
-                "sha256:2eca15d6b947cfff51ed76b2d60fd172c6ecd418ddab1c5126032d27f74bc350",
-                "sha256:354d9fc6b1e44750e2a67b4b108841f5f5ea08853453ecbf44c81fdc2e0d50bd",
-                "sha256:36a76a7527df8583112b24adc01748cd51a2d14e905b337a6fefa8b96fc708fb",
-                "sha256:3a0a4ca02752ced5f37498827e49c414d694ad7cf451ee850e3ff160f2bee9d3",
-                "sha256:3a71dbd792cc7a3d772ef8cd08d3048593f13d6f40a11f3427c000cf0a5b36a0",
-                "sha256:3a88254881e8a8c4784ecc9cb2249ff757fd94b911d5df9a5984961b96113fff",
-                "sha256:47045ed35481e857918ae78b54891fac0c1d197f22c95778e66302668309336c",
-                "sha256:4775a574e9d84e0212f5b18886cace049a42e13e12009bb0491562a48bb2b758",
-                "sha256:493da1f8b1bb8a623c16552fb4a1e164c0200447eb83d3f68b44315ead3f9036",
-                "sha256:4b847029e2d5e11fd536c9ac3136ddc3f54bc9488a75ef7d040a3900406a91eb",
-                "sha256:59d7d92cee84a547d91267f0fea381c363121d70fe90b12cd88241bd9b0e1763",
-                "sha256:5a0898a640559dec00f3614ffb11d97a2666ee9a2a6bad1259c9facd01a1d4d9",
-                "sha256:5a9a1889cc01ed2ed5f34574c90745fab1dd06ec2eee663e8ebeefe363e8efd7",
-                "sha256:5b835b86bd5a1bdbe257d610eecab07bf685b1af2a7563093e0e69180c1d4af1",
-                "sha256:5f24ca7953f2643d59a9c87d6e272d8adddd4a53bb62b9208f36db408d7aafc7",
-                "sha256:61e1a064906ccba038aa3c4a5a82f6199749efbbb3cef0804ae5c37f550eded0",
-                "sha256:65bf3eb34721bf18b5a021a1ad7aa05947a1767d1aa272b725728014475ea7d5",
-                "sha256:6807bcee549a8cb2f38f73f469703a1d8d5d990815c3004f21ddb68a567385ce",
-                "sha256:68aeefac31c1f73949662ba8affaf9950b9938b712fb9d428fa2a07e40ee57f8",
-                "sha256:6915682f9a9bc4cf2908e83caf5895a685da1fbd20b6d485dafb8e218a338279",
-                "sha256:6d9810d4f697d58fd66039ab959e6d37e63ab377008ef1d63904df25956c7db0",
-                "sha256:729d5e96566f44fccac6c4447ec2332636b4fe273f03da128fff8d5559782b06",
-                "sha256:748df39ed634851350efa87690c2237a678ed794fe9ede3f0d79f071ee042561",
-                "sha256:763a73ab377390e2af26042f685a26787c402390f682443727b847e9496e4a2a",
-                "sha256:8323a43bd9c91f62bb7d4be74cc9ff10090e7ef820e27bfe8815c57e68261311",
-                "sha256:8529b07b49b2d89d6917cfa157d3ea1dfb4d319d51e23030664a827fe5fd2131",
-                "sha256:87fa943e8bbe40c8c1ba4086971a6fefbf75e9991217c55ed1bcb2f1985bd3d4",
-                "sha256:88236b90dda77f0394f878324cfbae05ae6fde8a84d548cfe73a75278d760291",
-                "sha256:891c353e95bb11abb548ca95c8b98050f3620a7378332eb90d6acdef35b401d4",
-                "sha256:89ba3d548ee1e6291a20f3c7380c92f71e358ce8b9e48161401e087e0bc740f8",
-                "sha256:8c6be72eac3c14baa473620e04f74186c5d8f45d80f8f2b4eda6e1d18af808e8",
-                "sha256:9a242871b3d8eecc56d350e5e03ea1854de47b17f040446da0e47dc3e0b9ad4d",
-                "sha256:9a3ff5fb015f6feb78340143584d9f8a0b91b6293d6b5cf4295b3e95d179b88c",
-                "sha256:9a5a544861b21e0e7575b6023adebe7a8c6321127bb1d238eb40d99803a0e8bd",
-                "sha256:9d57677238a0c5411c76097b8b93bdebb02eb845814c90f0b01727527a179e4d",
-                "sha256:9d8c68c4145041b4eeae96239802cfdfd9ef927754a5be3f50505f09f309d8c6",
-                "sha256:9d9fcd06c952efa4b6b95f3d788a819b7f33d11bea377be6b8980c95e7d10775",
-                "sha256:a0057b5435a65b933cbf5d859cd4956624df37b8bf0917c71756e4b3d9958b9e",
-                "sha256:a65bffd24409454b889af33b6c49d0d9bcd1a219b972fba975ac935f17bdf627",
-                "sha256:b0ed6ad6c9640671689c2dbe6244680fe8b897c08fd1fab2228429b66c518e5e",
-                "sha256:b21650fa6907e523869e0396c5bd591cc326e5c1dd594dcdccac089561cacfb8",
-                "sha256:b3f7e671fb19734c872566e57ce7fc235fa953d7c181bb4ef138e17d607dc8a1",
-                "sha256:b77159d9862374da213f741af0c361720200ab7ad21b9f12556e0eb95912cd48",
-                "sha256:bb36fbb48b22985d13a6b496ea5fb9bb2a076fea943831643836c9f6febbcfdc",
-                "sha256:d066ffc5ed0be00cd0352c95800a519cf9e4b5dd34a028d301bdc7177c72daf3",
-                "sha256:d332eecf307fca852d02b63f35a7872de32d5ba8b4ec32da82f45df986b39ff6",
-                "sha256:d808a5a5411982a09fef6b49aac62986274ab050e9d3e9817ad65b2791ed1425",
-                "sha256:d9bdfa74d369256e4218000a629978590fd7cb6cf6893251dad13d051090436d",
-                "sha256:db6a0ddc1282ceb9032e41853e659c9b638789be38e5b8ad7498caac00231c23",
-                "sha256:debaf04f813ada978d7d16c7dfa16f3c9c2ec9adf4656efdc4defdf841fc2f0c",
-                "sha256:f0408e2dbad9e82b4c960274214af533f856a199c9274bd4aff55d4634dedc33",
-                "sha256:f2f3bc7cd9c9fcd39143f11342eb5963317bd54ecc98e3650ca22704b69d9653"
+                "sha256:02fce1852f755f44f95af51f69d22e45080102e9d00258053b79367d07af39c0",
+                "sha256:077ff0d1f9d9e4ce6476c1a924a3332452c1406e59d90a2cf24aeb29eeac9420",
+                "sha256:078e2a1a86544e644a68422f881c48b84fef6d18f8c7a957ffd3f2e0a74a0d4a",
+                "sha256:0970ddb69bba00670e58955f8019bec4a42d1785db3faa043c33d81de2bf843c",
+                "sha256:1286eb30261894e4c70d124d44b7fd07825340869945c79d05bda53a40caa079",
+                "sha256:21f6d9a0d5b3a207cdf7acf8e58d7d13d463e639f0c7e01d82cdb671e6cb7923",
+                "sha256:230ae493696a371f1dbffaad3dafbb742a4d27a0afd2b1aecebe52b740167e7f",
+                "sha256:26458da5653aa5b3d8dc8b24192f574a58984c749401f98fff994d41d3f08da1",
+                "sha256:2cf56d0e237280baed46f0b5316661da892565ff58309d4d2ed7dba763d984b8",
+                "sha256:2e51de54d4fb8fb50d6ee8327f9828306a959ae394d3e01a1ba8b2f937747d86",
+                "sha256:2fbfbca668dd15b744418265a9607baa970c347eefd0db6a518aaf0cfbd153c0",
+                "sha256:38adf7198f8f154502883242f9fe7333ab05a5b02de7d83aa2d88ea621f13364",
+                "sha256:3a8564f283394634a7a7054b7983e47dbf39c07712d7b177b37e03f2467a024e",
+                "sha256:3abbe948c3cbde2689370a262a8d04e32ec2dd4f27103669a45c6929bcdbfe7c",
+                "sha256:3bbe623731d03b186b3d6b0d6f51865bf598587c38d6f7b0be2e27414f7f214e",
+                "sha256:40737a081d7497efea35ab9304b829b857f21558acfc7b3272f908d33b0d9d4c",
+                "sha256:41d07d029dd4157ae27beab04d22b8e261eddfc6ecd64ff7000b10dc8b3a5727",
+                "sha256:46ed616d5fb42f98630ed70c3529541408166c22cdfd4540b88d5f21006b0eff",
+                "sha256:493d389a2b63c88ad56cdc35d0fa5752daac56ca755805b1b0c530f785767d5e",
+                "sha256:4ff0d20f2e670800d3ed2b220d40984162089a6e2c9646fdb09b85e6f9a8fc29",
+                "sha256:54accd4b8bc202966bafafd16e69da9d5640ff92389d33d28555c5fd4f25ccb7",
+                "sha256:56374914b132c702aa9aa9959c550004b8847148f95e1b824772d453ac204a72",
+                "sha256:578383d740457fa790fdf85e6d346fda1416a40549fe8db08e5e9bd281c6a475",
+                "sha256:58d7a75d731e8c63614222bcb21dd992b4ab01a399f1f09dd82af17bbfc2368a",
+                "sha256:5c5aa28df055697d7c37d2099a7bc09f559d5053c3349b1ad0c39000e611d317",
+                "sha256:5fc8e02f5984a55d2c653f5fea93531e9836abbd84342c1d1e17abc4a15084c2",
+                "sha256:63424c681923b9f3bfbc5e3205aafe790904053d42ddcc08542181a30a7a51bd",
+                "sha256:64b1df0f83706b4ef4cfb4fb0e4c2669100fd7ecacfb59e091fad300d4e04640",
+                "sha256:74934ebd71950e3db69960a7da29204f89624dde411afbfb3b4858c1409b1e98",
+                "sha256:75669d77bb2c071333417617a235324a1618dba66f82a750362eccbe5b61d248",
+                "sha256:75760a47c06b5974aa5e01949bf7e66d2af4d08cb8c1d6516af5e39595397f5e",
+                "sha256:76407ab327158c510f44ded207e2f76b657303e17cb7a572ffe2f5a8a48aa04d",
+                "sha256:76e9c727a874b4856d11a32fb0b389afc61ce8aaf281ada613713ddeadd1cfec",
+                "sha256:77d4c1b881076c3ba173484dfa53d3582c1c8ff1f914c6461ab70c8428b796c1",
+                "sha256:780c82a41dc493b62fc5884fb1d3a3b81106642c5c5c78d6a0d4cbe96d62ba7e",
+                "sha256:7dc0713bf81287a00516ef43137273b23ee414fe41a3c14be10dd95ed98a2df9",
+                "sha256:7eebcdbe3677e58dd4c0e03b4f2cfa346ed4049687d839adad68cc38bb559c92",
+                "sha256:896689fddba4f23ef7c718279e42f8834041a21342d95e56922e1c10c0cc7afb",
+                "sha256:96177eb5645b1c6985f5c11d03fc2dbda9ad24ec0f3a46dcce91445747e15094",
+                "sha256:96e25c8603a155559231c19c0349245eeb4ac0096fe3c1d0be5c47e075bd4f46",
+                "sha256:9d37ac69edc5614b90516807de32d08cb8e7b12260a285ee330955604ed9dd29",
+                "sha256:9ed6aa0726b9b60911f4aed8ec5b8dd7bf3491476015819f56473ffaef8959bd",
+                "sha256:a487f72a25904e2b4bbc0817ce7a8de94363bd7e79890510174da9d901c38705",
+                "sha256:a4cbb9ff5795cd66f0066bdf5947f170f5d63a9274f99bdbca02fd973adcf2a8",
+                "sha256:a74d56552ddbde46c246b5b89199cb3fd182f9c346c784e1a93e4dc3f5ec9975",
+                "sha256:a89ce3fd220ff144bd9d54da333ec0de0399b52c9ac3d2ce34b569cf1a5748fb",
+                "sha256:abd52a09d03adf9c763d706df707c343293d5d106aea53483e0ec8d9e310ad5e",
+                "sha256:abd8f36c99512755b8456047b7be10372fca271bf1467a1caa88db991e7c421b",
+                "sha256:af5bd9ccb188f6a5fdda9f1f09d9f4c86cc8a539bd48a0bfdc97723970348418",
+                "sha256:b02f21c1e2074943312d03d243ac4388319f2456576b2c6023041c4d57cd7019",
+                "sha256:b06fa97478a5f478fb05e1980980a7cdf2712015493b44d0c87606c1513ed5b1",
+                "sha256:b0724f05c396b0a4c36a3226c31648385deb6a65d8992644c12a4963c70326ba",
+                "sha256:b130fe77361d6771ecf5a219d8e0817d61b236b7d8b37cc045172e574ed219e6",
+                "sha256:b56d5519e470d3f2fe4aa7585f0632b060d532d0696c5bdfb5e8319e1d0f69a2",
+                "sha256:b67b819628e3b748fd3c2192c15fb951f549d0f47c0449af0764d7647302fda3",
+                "sha256:ba1711cda2d30634a7e452fc79eabcadaffedf241ff206db2ee93dd2c89a60e7",
+                "sha256:bbeccb1aa40ab88cd29e6c7d8585582c99548f55f9b2581dfc5ba68c59a85752",
+                "sha256:bd84395aab8e4d36263cd1b9308cd504f6cf713b7d6d3ce25ea55670baec5416",
+                "sha256:c99f4309f5145b93eca6e35ac1a988f0dc0a7ccf9ccdcd78d3c0adf57224e62f",
+                "sha256:ca1cccf838cd28d5a0883b342474c630ac48cac5df0ee6eacc9c7290f76b11c1",
+                "sha256:cd525e0e52a5ff16653a3fc9e3dd827981917d34996600bbc34c05d048ca35cc",
+                "sha256:cdb4f085756c96a3af04e6eca7f08b1345e94b53af8921b25c72f096e704e145",
+                "sha256:ce42618f67741d4697684e501ef02f29e758a123aa2d669e2d964ff734ee00ee",
+                "sha256:d06730c6aed78cee4126234cf2d071e01b44b915e725a6cb439a879ec9754a3a",
+                "sha256:d5fe3e099cf07d0fb5a1e23d399e5d4d1ca3e6dfcbe5c8570ccff3e9208274f7",
+                "sha256:d6bcbfc99f55655c3d93feb7ef3800bd5bbe963a755687cbf1f490a71fb7794b",
+                "sha256:d787272ed958a05b2c86311d3a4135d3c2aeea4fc655705f074130aa57d71653",
+                "sha256:e169e957c33576f47e21864cf3fc9ff47c223a4ebca8960079b8bd36cb014fd0",
+                "sha256:e20076a211cd6f9b44a6be58f7eeafa7ab5720eb796975d0c03f05b47d89eb90",
+                "sha256:e826aadda3cae59295b95343db8f3d965fb31059da7de01ee8d1c40a60398b29",
+                "sha256:eef4d64c650f33347c1f9266fa5ae001440b232ad9b98f1f43dfe7a79435c0a6",
+                "sha256:f2e69b3ed24544b0d3dbe2c5c0ba5153ce50dcebb576fdc4696d52aa22db6034",
+                "sha256:f87ec75864c37c4c6cb908d282e1969e79763e0d9becdfe9fe5473b7bb1e5f09",
+                "sha256:fbec11614dba0424ca72f4e8ba3c420dba07b4a7c206c8c8e4e73f2e98f4c559",
+                "sha256:fd69666217b62fa5d7c6aa88e507493a34dec4fa20c5bd925e4bc12fce586639"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
-            "version": "==1.14.0"
+            "markers": "python_version < '3.11'",
+            "version": "==1.15.0"
         },
         "zipp": {
             "hashes": [
-                "sha256:9f50f446828eb9d45b267433fd3e9da8d801f614129124863f9c51ebceafb87d",
-                "sha256:b47250dd24f92b7dd6a0a8fc5244da14608f3ca90a5efcd37a3b1642fac9a375"
+                "sha256:112929ad649da941c23de50f356a2b5570c954b65150642bccdd66bf194d224b",
+                "sha256:48904fc76a60e542af151aded95726c1a5c34ed43ab4134b597665c86d7ad556"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.7.0"
+            "version": "==3.15.0"
         }
     }
 }
```

### Comparing `gitwrapperlib-1.0.0/README.rst` & `gitwrapperlib-1.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `gitwrapperlib-1.0.0/USAGE.rst` & `gitwrapperlib-1.0.1/USAGE.rst`

 * *Files identical despite different names*

### Comparing `gitwrapperlib-1.0.0/docs/Makefile` & `gitwrapperlib-1.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `gitwrapperlib-1.0.0/docs/conf.py` & `gitwrapperlib-1.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `gitwrapperlib-1.0.0/docs/index.rst` & `gitwrapperlib-1.0.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `gitwrapperlib-1.0.0/gitwrapperlib/CONTRIBUTING.rst` & `gitwrapperlib-1.0.1/gitwrapperlib/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `gitwrapperlib-1.0.0/gitwrapperlib/HISTORY.rst` & `gitwrapperlib-1.0.1/gitwrapperlib/HISTORY.rst`

 * *Files 12% similar despite different names*

```diff
@@ -45,7 +45,13 @@
 * Self reference update for pipeline.
 
 
 1.0.0 (21-03-2022)
 ------------------
 
 * Removed references to master branch and implemented default remote retrieval, courtesy of Sten Spans <sspans@schubergphilis.com>
+
+
+1.0.1 (13-06-2023)
+------------------
+
+* Bump dependencies and update pipeline to python 3.9.
```

### Comparing `gitwrapperlib-1.0.0/gitwrapperlib/LICENSE` & `gitwrapperlib-1.0.1/gitwrapperlib/LICENSE`

 * *Files identical despite different names*

### Comparing `gitwrapperlib-1.0.0/gitwrapperlib/Pipfile` & `gitwrapperlib-1.0.1/gitwrapperlib/Pipfile`

 * *Files 22% similar despite different names*

```diff
@@ -3,29 +3,28 @@
 url = "https://pypi.python.org/simple"
 verify_ssl = true
 name = "pypi"
 
 
 [dev-packages]
 
-flake8 = "==3.8.0"
-sphinx = "~=2.1.2"
-sphinx-rtd-theme = "~=0.4.3"
-prospector = "~=1.3.0"
-coverage = "~=4.5.4"
-nose = "~=1.3.7"
-nose-htmloutput = "~=0.6.0"
-tox = "~=3.13.2"
-betamax = "~=0.8.1"
-betamax-serializers = "~=0.2.1"
-semver = "~=2.8.1"
-gitwrapperlib = "~=0.10.2"
-twine = "~=1.13.0"
-coloredlogs = "~=10.0"
-emoji = "~=0.5.3"
-toml = "~=0.10.0"
+sphinx = ">=6.0,<7.0"
+sphinx-rtd-theme = ">=1.0,<2.0"
+prospector = ">=1.8,<2.0"
+coverage = ">=7,<8.0"
+nose = ">=1.3,<2.0"
+nose-htmloutput = ">=0.1,<1.0"
+tox = ">=4.0<5.0"
+betamax = ">=0.8,<1.0"
+betamax-serializers = "~=0.2,<1.0"
+semver = ">=3.0,<4.0"
+gitwrapperlib = ">=1.0,<2.0"
+twine = ">=4.0,<5.0"
+coloredlogs = ">=15.0,<16.0"
+emoji = ">=2.0,<3.0"
+toml = ">=0.1,<1.0"
 
 
 [packages]
 
-sh = {version = "~=1.12.14", sys_platform = "!='win32'"}
+sh = {version = ">=2.0,<3.0", sys_platform = "!='win32'"}
 pbs = {version = "~=0.110", sys_platform = "=='win32'"}
```

### Comparing `gitwrapperlib-1.0.0/gitwrapperlib/Pipfile.lock` & `gitwrapperlib-1.0.1/gitwrapperlib/Pipfile.lock`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9104846792668958%*

 * *Differences: {"'_meta'": "{'hash': {'sha256': "*

 * *            "'4fa2d6a765b3b81f226c7b04ae11d34ed18d1ad2d3ff44959d98a7b1ceb4a025'}}",*

 * * "'default'": "{'sh': {'hashes': "*

 * *              "['sha256:14265a4cd1622429edcf300292ec98193530fb143fe642b3437024eca9bee8c5', "*

 * *              "'sha256:a18920f0839991bc9dfddb6dcc006c360b1064ba96257359f0ea356e9fa75a60'], "*

 * *              "'version': '==2.0.4'}}",*

 * * "'develop'": "{'alabaster': {'hashes': "*

 * *              "['sha256:1ee19aca801bbabb5ba3f5f258e4422dfa86f82f3e9cefb0859b283cdd7f62a3', […]*

```diff
@@ -1,11 +1,11 @@
 {
     "_meta": {
         "hash": {
-            "sha256": "adc6d97618b44175e9b1cf78a95b8b6d7233fb7fc0fd2706cf97911922256656"
+            "sha256": "4fa2d6a765b3b81f226c7b04ae11d34ed18d1ad2d3ff44959d98a7b1ceb4a025"
         },
         "pipfile-spec": 6,
         "requires": {},
         "sources": [
             {
                 "name": "pypi",
                 "url": "https://pypi.python.org/simple",
@@ -19,45 +19,46 @@
                 "sha256:05fafccbab7ce1cb2f25330267c8a622b569ad95b40c83220a36983f53757469"
             ],
             "markers": "sys_platform == 'win32'",
             "version": "==0.110"
         },
         "sh": {
             "hashes": [
-                "sha256:ae3258c5249493cebe73cb4e18253a41ed69262484bad36fdb3efcb8ad8870bb",
-                "sha256:b52bf5833ed01c7b5c5fb73a7f71b3d98d48e9b9b8764236237bdc7ecae850fc"
+                "sha256:14265a4cd1622429edcf300292ec98193530fb143fe642b3437024eca9bee8c5",
+                "sha256:a18920f0839991bc9dfddb6dcc006c360b1064ba96257359f0ea356e9fa75a60"
             ],
             "index": "pypi",
             "markers": "sys_platform != 'win32'",
-            "version": "==1.12.14"
+            "version": "==2.0.4"
         }
     },
     "develop": {
         "alabaster": {
             "hashes": [
-                "sha256:446438bdcca0e05bd45ea2de1668c1d9b032e1a9154c2c259092d77031ddd359",
-                "sha256:a661d72d58e6ea8a57f7a86e37d86716863ee5e92788398526d58b26a4e4dc02"
+                "sha256:1ee19aca801bbabb5ba3f5f258e4422dfa86f82f3e9cefb0859b283cdd7f62a3",
+                "sha256:a27a4a084d5e690e16e01e03ad2b2e552c61a65469419b907243193de1a84ae2"
             ],
-            "version": "==0.7.12"
+            "markers": "python_version >= '3.6'",
+            "version": "==0.7.13"
         },
         "astroid": {
             "hashes": [
-                "sha256:4c17cea3e592c21b6e222f673868961bad77e1f985cb1694ed077475a89229c1",
-                "sha256:d8506842a3faf734b81599c8b98dcc423de863adcc1999248480b18bd31a0f38"
+                "sha256:078e5212f9885fa85fbb0cf0101978a336190aadea6e13305409d099f71b2324",
+                "sha256:1039262575027b441137ab4a62a793a9b43defb42c32d5670f38686207cd780f"
             ],
-            "markers": "python_version >= '3.5'",
-            "version": "==2.4.1"
+            "markers": "python_full_version >= '3.7.2'",
+            "version": "==2.15.5"
         },
         "babel": {
             "hashes": [
-                "sha256:ab49e12b91d937cd11f0b67cb259a57ab4ad2b59ac7a3b41d6c06c0ac5b0def9",
-                "sha256:bc0c176f9f6a994582230df350aa6e05ba2ebe4b3ac317eab29d9be5d2768da0"
+                "sha256:b4246fb7677d3b98f501a39d43396d3cafdc8eadb045f4a31be01863f655c610",
+                "sha256:cc2d99999cd01d44420ae725a21c9e3711b3aadc7976d6147f622d8581963455"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
-            "version": "==2.9.1"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.12.1"
         },
         "betamax": {
             "hashes": [
                 "sha256:5bf004ceffccae881213fb722f34517166b84a34919b92ffc14d1dbd050b71c2",
                 "sha256:aa5ad34cc8d018b35814fb0557d15c78ced9ac56fdc43ccacdb882aa7a5217c1"
             ],
             "index": "pypi",
@@ -69,87 +70,221 @@
                 "sha256:345c419b1b73171f2951c62ac3c701775ac4b76e13e86464ebf0ff2a978e4949"
             ],
             "index": "pypi",
             "version": "==0.2.1"
         },
         "bleach": {
             "hashes": [
-                "sha256:0900d8b37eba61a802ee40ac0061f8c2b5dee29c1927dd1d233e075ebf5a71da",
-                "sha256:4d2651ab93271d1129ac9cbc679f524565cc8a1b791909c4a51eac4446a15994"
+                "sha256:1a1a85c1595e07d8db14c5f09f09e6433502c51c595970edc090551f0db99414",
+                "sha256:33c16e3353dbd13028ab4799a0f89a83f113405c766e9c122df8a06f5b85b3f4"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==4.1.0"
+            "markers": "python_version >= '3.7'",
+            "version": "==6.0.0"
+        },
+        "cachetools": {
+            "hashes": [
+                "sha256:95ef631eeaea14ba2e36f06437f36463aac3a096799e876ee55e5cdccb102590",
+                "sha256:dce83f2d9b4e1f732a8cd44af8e8fab2dbe46201467fc98b3ef8f269092bf62b"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==5.3.1"
         },
         "certifi": {
             "hashes": [
-                "sha256:78884e7c1d4b00ce3cea67b44566851c4343c120abd683433ce934a68ea58872",
-                "sha256:d62a0163eb4c2344ac042ab2bdf75399a71a2d8c7d47eac2e2ee91b9d6339569"
+                "sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7",
+                "sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716"
+            ],
+            "markers": "python_version >= '3.6'",
+            "version": "==2023.5.7"
+        },
+        "chardet": {
+            "hashes": [
+                "sha256:0d62712b956bc154f85fb0a266e2a3c5913c2967e00348701b32411d6def31e5",
+                "sha256:362777fb014af596ad31334fde1e8c327dfdb076e1960d1694662d46a6917ab9"
             ],
-            "version": "==2021.10.8"
+            "markers": "python_version >= '3.7'",
+            "version": "==5.1.0"
         },
         "charset-normalizer": {
             "hashes": [
-                "sha256:2857e29ff0d34db842cd7ca3230549d1a697f96ee6d3fb071cfa6c7393832597",
-                "sha256:6881edbebdb17b39b4eaaa821b438bf6eddffb4468cf344f09f89def34a8b1df"
+                "sha256:04afa6387e2b282cf78ff3dbce20f0cc071c12dc8f685bd40960cc68644cfea6",
+                "sha256:04eefcee095f58eaabe6dc3cc2262f3bcd776d2c67005880894f447b3f2cb9c1",
+                "sha256:0be65ccf618c1e7ac9b849c315cc2e8a8751d9cfdaa43027d4f6624bd587ab7e",
+                "sha256:0c95f12b74681e9ae127728f7e5409cbbef9cd914d5896ef238cc779b8152373",
+                "sha256:0ca564606d2caafb0abe6d1b5311c2649e8071eb241b2d64e75a0d0065107e62",
+                "sha256:10c93628d7497c81686e8e5e557aafa78f230cd9e77dd0c40032ef90c18f2230",
+                "sha256:11d117e6c63e8f495412d37e7dc2e2fff09c34b2d09dbe2bee3c6229577818be",
+                "sha256:11d3bcb7be35e7b1bba2c23beedac81ee893ac9871d0ba79effc7fc01167db6c",
+                "sha256:12a2b561af122e3d94cdb97fe6fb2bb2b82cef0cdca131646fdb940a1eda04f0",
+                "sha256:12d1a39aa6b8c6f6248bb54550efcc1c38ce0d8096a146638fd4738e42284448",
+                "sha256:1435ae15108b1cb6fffbcea2af3d468683b7afed0169ad718451f8db5d1aff6f",
+                "sha256:1c60b9c202d00052183c9be85e5eaf18a4ada0a47d188a83c8f5c5b23252f649",
+                "sha256:1e8fcdd8f672a1c4fc8d0bd3a2b576b152d2a349782d1eb0f6b8e52e9954731d",
+                "sha256:20064ead0717cf9a73a6d1e779b23d149b53daf971169289ed2ed43a71e8d3b0",
+                "sha256:21fa558996782fc226b529fdd2ed7866c2c6ec91cee82735c98a197fae39f706",
+                "sha256:22908891a380d50738e1f978667536f6c6b526a2064156203d418f4856d6e86a",
+                "sha256:3160a0fd9754aab7d47f95a6b63ab355388d890163eb03b2d2b87ab0a30cfa59",
+                "sha256:322102cdf1ab682ecc7d9b1c5eed4ec59657a65e1c146a0da342b78f4112db23",
+                "sha256:34e0a2f9c370eb95597aae63bf85eb5e96826d81e3dcf88b8886012906f509b5",
+                "sha256:3573d376454d956553c356df45bb824262c397c6e26ce43e8203c4c540ee0acb",
+                "sha256:3747443b6a904001473370d7810aa19c3a180ccd52a7157aacc264a5ac79265e",
+                "sha256:38e812a197bf8e71a59fe55b757a84c1f946d0ac114acafaafaf21667a7e169e",
+                "sha256:3a06f32c9634a8705f4ca9946d667609f52cf130d5548881401f1eb2c39b1e2c",
+                "sha256:3a5fc78f9e3f501a1614a98f7c54d3969f3ad9bba8ba3d9b438c3bc5d047dd28",
+                "sha256:3d9098b479e78c85080c98e1e35ff40b4a31d8953102bb0fd7d1b6f8a2111a3d",
+                "sha256:3dc5b6a8ecfdc5748a7e429782598e4f17ef378e3e272eeb1340ea57c9109f41",
+                "sha256:4155b51ae05ed47199dc5b2a4e62abccb274cee6b01da5b895099b61b1982974",
+                "sha256:49919f8400b5e49e961f320c735388ee686a62327e773fa5b3ce6721f7e785ce",
+                "sha256:53d0a3fa5f8af98a1e261de6a3943ca631c526635eb5817a87a59d9a57ebf48f",
+                "sha256:5f008525e02908b20e04707a4f704cd286d94718f48bb33edddc7d7b584dddc1",
+                "sha256:628c985afb2c7d27a4800bfb609e03985aaecb42f955049957814e0491d4006d",
+                "sha256:65ed923f84a6844de5fd29726b888e58c62820e0769b76565480e1fdc3d062f8",
+                "sha256:6734e606355834f13445b6adc38b53c0fd45f1a56a9ba06c2058f86893ae8017",
+                "sha256:6baf0baf0d5d265fa7944feb9f7451cc316bfe30e8df1a61b1bb08577c554f31",
+                "sha256:6f4f4668e1831850ebcc2fd0b1cd11721947b6dc7c00bf1c6bd3c929ae14f2c7",
+                "sha256:6f5c2e7bc8a4bf7c426599765b1bd33217ec84023033672c1e9a8b35eaeaaaf8",
+                "sha256:6f6c7a8a57e9405cad7485f4c9d3172ae486cfef1344b5ddd8e5239582d7355e",
+                "sha256:7381c66e0561c5757ffe616af869b916c8b4e42b367ab29fedc98481d1e74e14",
+                "sha256:73dc03a6a7e30b7edc5b01b601e53e7fc924b04e1835e8e407c12c037e81adbd",
+                "sha256:74db0052d985cf37fa111828d0dd230776ac99c740e1a758ad99094be4f1803d",
+                "sha256:75f2568b4189dda1c567339b48cba4ac7384accb9c2a7ed655cd86b04055c795",
+                "sha256:78cacd03e79d009d95635e7d6ff12c21eb89b894c354bd2b2ed0b4763373693b",
+                "sha256:80d1543d58bd3d6c271b66abf454d437a438dff01c3e62fdbcd68f2a11310d4b",
+                "sha256:830d2948a5ec37c386d3170c483063798d7879037492540f10a475e3fd6f244b",
+                "sha256:891cf9b48776b5c61c700b55a598621fdb7b1e301a550365571e9624f270c203",
+                "sha256:8f25e17ab3039b05f762b0a55ae0b3632b2e073d9c8fc88e89aca31a6198e88f",
+                "sha256:9a3267620866c9d17b959a84dd0bd2d45719b817245e49371ead79ed4f710d19",
+                "sha256:a04f86f41a8916fe45ac5024ec477f41f886b3c435da2d4e3d2709b22ab02af1",
+                "sha256:aaf53a6cebad0eae578f062c7d462155eada9c172bd8c4d250b8c1d8eb7f916a",
+                "sha256:abc1185d79f47c0a7aaf7e2412a0eb2c03b724581139193d2d82b3ad8cbb00ac",
+                "sha256:ac0aa6cd53ab9a31d397f8303f92c42f534693528fafbdb997c82bae6e477ad9",
+                "sha256:ac3775e3311661d4adace3697a52ac0bab17edd166087d493b52d4f4f553f9f0",
+                "sha256:b06f0d3bf045158d2fb8837c5785fe9ff9b8c93358be64461a1089f5da983137",
+                "sha256:b116502087ce8a6b7a5f1814568ccbd0e9f6cfd99948aa59b0e241dc57cf739f",
+                "sha256:b82fab78e0b1329e183a65260581de4375f619167478dddab510c6c6fb04d9b6",
+                "sha256:bd7163182133c0c7701b25e604cf1611c0d87712e56e88e7ee5d72deab3e76b5",
+                "sha256:c36bcbc0d5174a80d6cccf43a0ecaca44e81d25be4b7f90f0ed7bcfbb5a00909",
+                "sha256:c3af8e0f07399d3176b179f2e2634c3ce9c1301379a6b8c9c9aeecd481da494f",
+                "sha256:c84132a54c750fda57729d1e2599bb598f5fa0344085dbde5003ba429a4798c0",
+                "sha256:cb7b2ab0188829593b9de646545175547a70d9a6e2b63bf2cd87a0a391599324",
+                "sha256:cca4def576f47a09a943666b8f829606bcb17e2bc2d5911a46c8f8da45f56755",
+                "sha256:cf6511efa4801b9b38dc5546d7547d5b5c6ef4b081c60b23e4d941d0eba9cbeb",
+                "sha256:d16fd5252f883eb074ca55cb622bc0bee49b979ae4e8639fff6ca3ff44f9f854",
+                "sha256:d2686f91611f9e17f4548dbf050e75b079bbc2a82be565832bc8ea9047b61c8c",
+                "sha256:d7fc3fca01da18fbabe4625d64bb612b533533ed10045a2ac3dd194bfa656b60",
+                "sha256:dd5653e67b149503c68c4018bf07e42eeed6b4e956b24c00ccdf93ac79cdff84",
+                "sha256:de5695a6f1d8340b12a5d6d4484290ee74d61e467c39ff03b39e30df62cf83a0",
+                "sha256:e0ac8959c929593fee38da1c2b64ee9778733cdf03c482c9ff1d508b6b593b2b",
+                "sha256:e1b25e3ad6c909f398df8921780d6a3d120d8c09466720226fc621605b6f92b1",
+                "sha256:e633940f28c1e913615fd624fcdd72fdba807bf53ea6925d6a588e84e1151531",
+                "sha256:e89df2958e5159b811af9ff0f92614dabf4ff617c03a4c1c6ff53bf1c399e0e1",
+                "sha256:ea9f9c6034ea2d93d9147818f17c2a0860d41b71c38b9ce4d55f21b6f9165a11",
+                "sha256:f645caaf0008bacf349875a974220f1f1da349c5dbe7c4ec93048cdc785a3326",
+                "sha256:f8303414c7b03f794347ad062c0516cee0e15f7a612abd0ce1e25caf6ceb47df",
+                "sha256:fca62a8301b605b954ad2e9c3666f9d97f63872aa4efcae5492baca2056b74ab"
+            ],
+            "markers": "python_full_version >= '3.7.0'",
+            "version": "==3.1.0"
+        },
+        "colorama": {
+            "hashes": [
+                "sha256:08695f5cb7ed6e0531a20572697297273c47b8cae5a63ffc6d6ed5c201be6e44",
+                "sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6"
             ],
-            "markers": "python_version >= '3.0'",
-            "version": "==2.0.12"
+            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6'",
+            "version": "==0.4.6"
         },
         "coloredlogs": {
             "hashes": [
-                "sha256:34fad2e342d5a559c31b6c889e8d14f97cb62c47d9a2ae7b5ed14ea10a79eff8",
-                "sha256:b869a2dda3fa88154b9dd850e27828d8755bfab5a838a1c97fbc850c6e377c36"
+                "sha256:612ee75c546f53e92e70049c9dbfcc18c935a2b9a53b66085ce9ef6a6e5c0934",
+                "sha256:7c991aa71a4577af2f82600d8f8f3a89f936baeaf9b50a9c197da014e5bf16b0"
             ],
             "index": "pypi",
-            "version": "==10.0"
+            "version": "==15.0.1"
         },
         "coverage": {
             "hashes": [
-                "sha256:08907593569fe59baca0bf152c43f3863201efb6113ecb38ce7e97ce339805a6",
-                "sha256:0be0f1ed45fc0c185cfd4ecc19a1d6532d72f86a2bac9de7e24541febad72650",
-                "sha256:141f08ed3c4b1847015e2cd62ec06d35e67a3ac185c26f7635f4406b90afa9c5",
-                "sha256:19e4df788a0581238e9390c85a7a09af39c7b539b29f25c89209e6c3e371270d",
-                "sha256:23cc09ed395b03424d1ae30dcc292615c1372bfba7141eb85e11e50efaa6b351",
-                "sha256:245388cda02af78276b479f299bbf3783ef0a6a6273037d7c60dc73b8d8d7755",
-                "sha256:331cb5115673a20fb131dadd22f5bcaf7677ef758741312bee4937d71a14b2ef",
-                "sha256:386e2e4090f0bc5df274e720105c342263423e77ee8826002dcffe0c9533dbca",
-                "sha256:3a794ce50daee01c74a494919d5ebdc23d58873747fa0e288318728533a3e1ca",
-                "sha256:60851187677b24c6085248f0a0b9b98d49cba7ecc7ec60ba6b9d2e5574ac1ee9",
-                "sha256:63a9a5fc43b58735f65ed63d2cf43508f462dc49857da70b8980ad78d41d52fc",
-                "sha256:6b62544bb68106e3f00b21c8930e83e584fdca005d4fffd29bb39fb3ffa03cb5",
-                "sha256:6ba744056423ef8d450cf627289166da65903885272055fb4b5e113137cfa14f",
-                "sha256:7494b0b0274c5072bddbfd5b4a6c6f18fbbe1ab1d22a41e99cd2d00c8f96ecfe",
-                "sha256:826f32b9547c8091679ff292a82aca9c7b9650f9fda3e2ca6bf2ac905b7ce888",
-                "sha256:93715dffbcd0678057f947f496484e906bf9509f5c1c38fc9ba3922893cda5f5",
-                "sha256:9a334d6c83dfeadae576b4d633a71620d40d1c379129d587faa42ee3e2a85cce",
-                "sha256:af7ed8a8aa6957aac47b4268631fa1df984643f07ef00acd374e456364b373f5",
-                "sha256:bf0a7aed7f5521c7ca67febd57db473af4762b9622254291fbcbb8cd0ba5e33e",
-                "sha256:bf1ef9eb901113a9805287e090452c05547578eaab1b62e4ad456fcc049a9b7e",
-                "sha256:c0afd27bc0e307a1ffc04ca5ec010a290e49e3afbe841c5cafc5c5a80ecd81c9",
-                "sha256:dd579709a87092c6dbee09d1b7cfa81831040705ffa12a1b248935274aee0437",
-                "sha256:df6712284b2e44a065097846488f66840445eb987eb81b3cc6e4149e7b6982e1",
-                "sha256:e07d9f1a23e9e93ab5c62902833bf3e4b1f65502927379148b6622686223125c",
-                "sha256:e2ede7c1d45e65e209d6093b762e98e8318ddeff95317d07a27a2140b80cfd24",
-                "sha256:e4ef9c164eb55123c62411f5936b5c2e521b12356037b6e1c2617cef45523d47",
-                "sha256:eca2b7343524e7ba246cab8ff00cab47a2d6d54ada3b02772e908a45675722e2",
-                "sha256:eee64c616adeff7db37cc37da4180a3a5b6177f5c46b187894e633f088fb5b28",
-                "sha256:ef824cad1f980d27f26166f86856efe11eff9912c4fed97d3804820d43fa550c",
-                "sha256:efc89291bd5a08855829a3c522df16d856455297cf35ae827a37edac45f466a7",
-                "sha256:fa964bae817babece5aa2e8c1af841bebb6d0b9add8e637548809d040443fee0",
-                "sha256:ff37757e068ae606659c28c3bd0d923f9d29a85de79bf25b2b34b148473b5025"
+                "sha256:06a9a2be0b5b576c3f18f1a241f0473575c4a26021b52b2a85263a00f034d51f",
+                "sha256:06fb182e69f33f6cd1d39a6c597294cff3143554b64b9825d1dc69d18cc2fff2",
+                "sha256:0a5f9e1dbd7fbe30196578ca36f3fba75376fb99888c395c5880b355e2875f8a",
+                "sha256:0e1f928eaf5469c11e886fe0885ad2bf1ec606434e79842a879277895a50942a",
+                "sha256:171717c7cb6b453aebac9a2ef603699da237f341b38eebfee9be75d27dc38e01",
+                "sha256:1e9d683426464e4a252bf70c3498756055016f99ddaec3774bf368e76bbe02b6",
+                "sha256:201e7389591af40950a6480bd9edfa8ed04346ff80002cec1a66cac4549c1ad7",
+                "sha256:245167dd26180ab4c91d5e1496a30be4cd721a5cf2abf52974f965f10f11419f",
+                "sha256:2aee274c46590717f38ae5e4650988d1af340fe06167546cc32fe2f58ed05b02",
+                "sha256:2e07b54284e381531c87f785f613b833569c14ecacdcb85d56b25c4622c16c3c",
+                "sha256:31563e97dae5598556600466ad9beea39fb04e0229e61c12eaa206e0aa202063",
+                "sha256:33d6d3ea29d5b3a1a632b3c4e4f4ecae24ef170b0b9ee493883f2df10039959a",
+                "sha256:3d376df58cc111dc8e21e3b6e24606b5bb5dee6024f46a5abca99124b2229ef5",
+                "sha256:419bfd2caae268623dd469eff96d510a920c90928b60f2073d79f8fe2bbc5959",
+                "sha256:48c19d2159d433ccc99e729ceae7d5293fbffa0bdb94952d3579983d1c8c9d97",
+                "sha256:49969a9f7ffa086d973d91cec8d2e31080436ef0fb4a359cae927e742abfaaa6",
+                "sha256:52edc1a60c0d34afa421c9c37078817b2e67a392cab17d97283b64c5833f427f",
+                "sha256:537891ae8ce59ef63d0123f7ac9e2ae0fc8b72c7ccbe5296fec45fd68967b6c9",
+                "sha256:54b896376ab563bd38453cecb813c295cf347cf5906e8b41d340b0321a5433e5",
+                "sha256:58c2ccc2f00ecb51253cbe5d8d7122a34590fac9646a960d1430d5b15321d95f",
+                "sha256:5b7540161790b2f28143191f5f8ec02fb132660ff175b7747b95dcb77ac26562",
+                "sha256:5baa06420f837184130752b7c5ea0808762083bf3487b5038d68b012e5937dbe",
+                "sha256:5e330fc79bd7207e46c7d7fd2bb4af2963f5f635703925543a70b99574b0fea9",
+                "sha256:61b9a528fb348373c433e8966535074b802c7a5d7f23c4f421e6c6e2f1697a6f",
+                "sha256:63426706118b7f5cf6bb6c895dc215d8a418d5952544042c8a2d9fe87fcf09cb",
+                "sha256:6d040ef7c9859bb11dfeb056ff5b3872436e3b5e401817d87a31e1750b9ae2fb",
+                "sha256:6f48351d66575f535669306aa7d6d6f71bc43372473b54a832222803eb956fd1",
+                "sha256:7ee7d9d4822c8acc74a5e26c50604dff824710bc8de424904c0982e25c39c6cb",
+                "sha256:81c13a1fc7468c40f13420732805a4c38a105d89848b7c10af65a90beff25250",
+                "sha256:8d13c64ee2d33eccf7437961b6ea7ad8673e2be040b4f7fd4fd4d4d28d9ccb1e",
+                "sha256:8de8bb0e5ad103888d65abef8bca41ab93721647590a3f740100cd65c3b00511",
+                "sha256:8fa03bce9bfbeeef9f3b160a8bed39a221d82308b4152b27d82d8daa7041fee5",
+                "sha256:924d94291ca674905fe9481f12294eb11f2d3d3fd1adb20314ba89e94f44ed59",
+                "sha256:975d70ab7e3c80a3fe86001d8751f6778905ec723f5b110aed1e450da9d4b7f2",
+                "sha256:976b9c42fb2a43ebf304fa7d4a310e5f16cc99992f33eced91ef6f908bd8f33d",
+                "sha256:9e31cb64d7de6b6f09702bb27c02d1904b3aebfca610c12772452c4e6c21a0d3",
+                "sha256:a342242fe22407f3c17f4b499276a02b01e80f861f1682ad1d95b04018e0c0d4",
+                "sha256:a3d33a6b3eae87ceaefa91ffdc130b5e8536182cd6dfdbfc1aa56b46ff8c86de",
+                "sha256:a895fcc7b15c3fc72beb43cdcbdf0ddb7d2ebc959edac9cef390b0d14f39f8a9",
+                "sha256:afb17f84d56068a7c29f5fa37bfd38d5aba69e3304af08ee94da8ed5b0865833",
+                "sha256:b1c546aca0ca4d028901d825015dc8e4d56aac4b541877690eb76490f1dc8ed0",
+                "sha256:b29019c76039dc3c0fd815c41392a044ce555d9bcdd38b0fb60fb4cd8e475ba9",
+                "sha256:b46517c02ccd08092f4fa99f24c3b83d8f92f739b4657b0f146246a0ca6a831d",
+                "sha256:b7aa5f8a41217360e600da646004f878250a0d6738bcdc11a0a39928d7dc2050",
+                "sha256:b7b4c971f05e6ae490fef852c218b0e79d4e52f79ef0c8475566584a8fb3e01d",
+                "sha256:ba90a9563ba44a72fda2e85302c3abc71c5589cea608ca16c22b9804262aaeb6",
+                "sha256:cb017fd1b2603ef59e374ba2063f593abe0fc45f2ad9abdde5b4d83bd922a353",
+                "sha256:d22656368f0e6189e24722214ed8d66b8022db19d182927b9a248a2a8a2f67eb",
+                "sha256:d2c2db7fd82e9b72937969bceac4d6ca89660db0a0967614ce2481e81a0b771e",
+                "sha256:d39b5b4f2a66ccae8b7263ac3c8170994b65266797fb96cbbfd3fb5b23921db8",
+                "sha256:d62a5c7dad11015c66fbb9d881bc4caa5b12f16292f857842d9d1871595f4495",
+                "sha256:e7d9405291c6928619403db1d10bd07888888ec1abcbd9748fdaa971d7d661b2",
+                "sha256:e84606b74eb7de6ff581a7915e2dab7a28a0517fbe1c9239eb227e1354064dcd",
+                "sha256:eb393e5ebc85245347950143969b241d08b52b88a3dc39479822e073a1a8eb27",
+                "sha256:ebba1cd308ef115925421d3e6a586e655ca5a77b5bf41e02eb0e4562a111f2d1",
+                "sha256:ee57190f24fba796e36bb6d3aa8a8783c643d8fa9760c89f7a98ab5455fbf818",
+                "sha256:f2f67fe12b22cd130d34d0ef79206061bfb5eda52feb6ce0dba0644e20a03cf4",
+                "sha256:f6951407391b639504e3b3be51b7ba5f3528adbf1a8ac3302b687ecababf929e",
+                "sha256:f75f7168ab25dd93110c8a8117a22450c19976afbc44234cbf71481094c1b850",
+                "sha256:fdec9e8cbf13a5bf63290fc6013d216a4c7232efb51548594ca3631a7f13c3a3"
             ],
             "index": "pypi",
-            "version": "==4.5.4"
+            "version": "==7.2.7"
+        },
+        "dill": {
+            "hashes": [
+                "sha256:a07ffd2351b8c678dfc4a856a3005f8067aea51d6ba6c700796a4d9e280f39f0",
+                "sha256:e5db55f3687856d8fbdab002ed78544e1c4559a130302693d839dfe8f93f2373"
+            ],
+            "markers": "python_version < '3.11'",
+            "version": "==0.3.6"
         },
         "distlib": {
             "hashes": [
-                "sha256:6564fe0a8f51e734df6333d08b8b94d4ea8ee6b99b5ed50613f731fd4089f34b",
-                "sha256:e4b58818180336dc9c529bfb9a0b58728ffc09ad92027a3f30b7cd91e3458579"
+                "sha256:14bad2d9b04d3a36127ac97f30b12a19268f211063d8f8ee4f47108896e11b46",
+                "sha256:f35c4b692542ca110de7ef0bea44d73981caeb34ca0b9b6b2e6d7790dda8f80e"
             ],
-            "version": "==0.3.4"
+            "version": "==0.3.6"
         },
         "docutils": {
             "hashes": [
                 "sha256:23010f129180089fbcd3bc08cfefccb3b890b0050e1ca00c867036e9d161b98c",
                 "sha256:679987caf361a7539d76e584cbeddc311e3aee937877c87346f31debc63e9d06"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
@@ -160,177 +295,258 @@
                 "sha256:28323cbfc9352139fdd3d316fa17f325cc0e9ac74438cbba51d70f9b48f86c3a",
                 "sha256:51f54c0fd886fa3854387f354b19f429d38c04f984f38bc572558b703c0542a6"
             ],
             "version": "==0.2.1"
         },
         "emoji": {
             "hashes": [
-                "sha256:60652d3a2dcee5b8af8acb097c31776fb6d808027aeb7221830f72cdafefc174"
+                "sha256:0e048dd540a0644bd30790b540466492f1487a3788528422fe196a939a7a3ac0"
             ],
             "index": "pypi",
-            "version": "==0.5.4"
+            "version": "==2.5.0"
         },
         "filelock": {
             "hashes": [
-                "sha256:9cd540a9352e432c7246a48fe4e8712b10acb1df2ad1f30e8c070b82ae1fed85",
-                "sha256:f8314284bfffbdcfa0ff3d7992b023d4c628ced6feb957351d4c48d059f56bc0"
+                "sha256:002740518d8aa59a26b0c76e10fb8c6e15eae825d34b6fdf670333fd7b938d81",
+                "sha256:cbb791cdea2a72f23da6ac5b5269ab0a0d161e9ef0100e653b69049a7706d1ec"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.6.0"
+            "version": "==3.12.2"
         },
         "flake8": {
             "hashes": [
-                "sha256:bcf5163890bb01f11f04f0f444f01004d0f9ad5fab10c51104f770acf532008f",
-                "sha256:e2f33066fb92ac0a3a30ea509f61e325f2110b2e84644333a3ff8e9e98a2beab"
+                "sha256:6fbe320aad8d6b95cec8b8e47bc933004678dc63095be98528b7bdd2a9f510db",
+                "sha256:7a1cf6b73744f5806ab95e526f6f0d8c01c66d7bbe349562d22dfca20610b248"
             ],
-            "index": "pypi",
-            "version": "==3.8.0"
+            "markers": "python_full_version >= '3.6.1'",
+            "version": "==5.0.4"
         },
         "flake8-polyfill": {
             "hashes": [
                 "sha256:12be6a34ee3ab795b19ca73505e7b55826d5f6ad7230d31b18e106400169b9e9",
                 "sha256:e44b087597f6da52ec6393a709e7108b2905317d0c0b744cdca6208e670d8eda"
             ],
             "version": "==1.0.2"
         },
+        "gitdb": {
+            "hashes": [
+                "sha256:6eb990b69df4e15bad899ea868dc46572c3f75339735663b81de79b06f17eb9a",
+                "sha256:c286cf298426064079ed96a9e4a9d39e7f3e9bf15ba60701e95f5492f28415c7"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==4.0.10"
+        },
+        "gitpython": {
+            "hashes": [
+                "sha256:8ce3bcf69adfdf7c7d503e78fd3b1c492af782d58893b650adb2ac8912ddd573",
+                "sha256:f04893614f6aa713a60cbbe1e6a97403ef633103cdd0ef5eb6efe0deb98dbe8d"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==3.1.31"
+        },
         "gitwrapperlib": {
             "hashes": [
-                "sha256:e7ca1c670ec21e325f502997ba27dd479609460e420ae23c82d23bd6c21ebd19",
-                "sha256:e9476fd7e70f50060c249ce4608b77519c8a3891607475696d8a9e95b51943a5"
+                "sha256:3174bcc0de3fa70f78067cb2bc60a5c9820442d78594fb345bdd56740f64073a"
             ],
             "index": "pypi",
-            "version": "==0.10.3"
+            "version": "==1.0.0"
         },
         "humanfriendly": {
             "hashes": [
                 "sha256:1697e1a8a8f550fd43c2865cd84542fc175a61dcb779b6fee18cf6b6ccba1477",
                 "sha256:6b0b831ce8f15f7300721aa49829fc4e83921a9a301cc7f606be6686a2288ddc"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
             "version": "==10.0"
         },
         "idna": {
             "hashes": [
-                "sha256:84d9dd047ffa80596e0f246e2eab0b391788b0503584e8945f2368256d2735ff",
-                "sha256:9d643ff0a55b762d5cdb124b8eaa99c66322e2157b69160bc32796e824360e6d"
+                "sha256:814f528e8dead7d329833b91c5faa87d60bf71824cd12a7530b5526063d02cb4",
+                "sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2"
             ],
-            "markers": "python_version >= '3.0'",
-            "version": "==3.3"
+            "markers": "python_version >= '3.5'",
+            "version": "==3.4"
         },
         "imagesize": {
             "hashes": [
-                "sha256:1db2f82529e53c3e929e8926a1fa9235aa82d0bd0c580359c67ec31b2fddaa8c",
-                "sha256:cd1750d452385ca327479d45b64d9c7729ecf0b3969a58148298c77092261f9d"
+                "sha256:0d8d18d08f840c19d0ee7ca1fd82490fdc3729b7ac93f49870406ddde8ef8d8b",
+                "sha256:69150444affb9cb0d5cc5a92b3676f0b2fb7cd9ae39e947a5e11a36b4497cd4a"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
-            "version": "==1.3.0"
+            "version": "==1.4.1"
         },
         "importlib-metadata": {
             "hashes": [
-                "sha256:aa18d7378b00b40847790e7c27e11673d7fed219354109d0e7b9e5b25dc3ad26",
-                "sha256:d5f18a79777f3aa179c145737780282e27b508fc8fd688cb17c7a813e8bd39af"
+                "sha256:43dd286a2cd8995d5eaef7fee2066340423b818ed3fd70adf0bad5f1fac53fed",
+                "sha256:92501cdf9cc66ebd3e612f1b4f0c0765dfa42f0fa38ffb319b6bd84dd675d705"
             ],
-            "markers": "python_version < '3.8'",
-            "version": "==0.23"
+            "markers": "python_version < '3.10'",
+            "version": "==6.6.0"
         },
         "isort": {
             "hashes": [
-                "sha256:54da7e92468955c4fceacd0c86bd0ec997b0e1ee80d97f67c35a78b719dccab1",
-                "sha256:6e811fcb295968434526407adb8796944f1988c5b65e8139058f2014cbe100fd"
+                "sha256:8bef7dde241278824a6d83f44a544709b065191b95b6e50894bdc722fcba0504",
+                "sha256:f84c2818376e66cf843d497486ea8fed8700b340f308f076c6fb1229dff318b6"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
-            "version": "==4.3.21"
+            "markers": "python_full_version >= '3.8.0'",
+            "version": "==5.12.0"
+        },
+        "jaraco.classes": {
+            "hashes": [
+                "sha256:2353de3288bc6b82120752201c6b1c1a14b058267fa424ed5ce5984e3b922158",
+                "sha256:89559fa5c1d3c34eff6f631ad80bb21f378dbcbb35dd161fd2c6b93f5be2f98a"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==3.2.3"
         },
         "jinja2": {
             "hashes": [
-                "sha256:077ce6014f7b40d03b47d1f1ca4b0fc8328a692bd284016f806ed0eaca390ad8",
-                "sha256:611bb273cd68f3b993fabdc4064fc858c5b47a973cb5aa7999ec1ba405c87cd7"
+                "sha256:31351a702a408a9e7595a8fc6150fc3f43bb6bf7e319770cbc0db9df9437e852",
+                "sha256:6088930bfe239f0e6710546ab9c19c9ef35e29792895fed6e6e31a023a182a61"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==3.0.3"
+            "markers": "python_version >= '3.7'",
+            "version": "==3.1.2"
+        },
+        "keyring": {
+            "hashes": [
+                "sha256:771ed2a91909389ed6148631de678f82ddc73737d85a927f382a8a1b157898cd",
+                "sha256:ba2e15a9b35e21908d0aaf4e0a47acc52d6ae33444df0da2b49d41a46ef6d678"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==23.13.1"
         },
         "lazy-object-proxy": {
             "hashes": [
-                "sha256:0c4b206227a8097f05c4dbdd323c50edf81f15db3b8dc064d08c62d37e1a504d",
-                "sha256:194d092e6f246b906e8f70884e620e459fc54db3259e60cf69a4d66c3fda3449",
-                "sha256:1be7e4c9f96948003609aa6c974ae59830a6baecc5376c25c92d7d697e684c08",
-                "sha256:4677f594e474c91da97f489fea5b7daa17b5517190899cf213697e48d3902f5a",
-                "sha256:48dab84ebd4831077b150572aec802f303117c8cc5c871e182447281ebf3ac50",
-                "sha256:5541cada25cd173702dbd99f8e22434105456314462326f06dba3e180f203dfd",
-                "sha256:59f79fef100b09564bc2df42ea2d8d21a64fdcda64979c0fa3db7bdaabaf6239",
-                "sha256:8d859b89baf8ef7f8bc6b00aa20316483d67f0b1cbf422f5b4dc56701c8f2ffb",
-                "sha256:9254f4358b9b541e3441b007a0ea0764b9d056afdeafc1a5569eee1cc6c1b9ea",
-                "sha256:9651375199045a358eb6741df3e02a651e0330be090b3bc79f6d0de31a80ec3e",
-                "sha256:97bb5884f6f1cdce0099f86b907aa41c970c3c672ac8b9c8352789e103cf3156",
-                "sha256:9b15f3f4c0f35727d3a0fba4b770b3c4ebbb1fa907dbcc046a1d2799f3edd142",
-                "sha256:a2238e9d1bb71a56cd710611a1614d1194dc10a175c1e08d75e1a7bcc250d442",
-                "sha256:a6ae12d08c0bf9909ce12385803a543bfe99b95fe01e752536a60af2b7797c62",
-                "sha256:ca0a928a3ddbc5725be2dd1cf895ec0a254798915fb3a36af0964a0a4149e3db",
-                "sha256:cb2c7c57005a6804ab66f106ceb8482da55f5314b7fcb06551db1edae4ad1531",
-                "sha256:d74bb8693bf9cf75ac3b47a54d716bbb1a92648d5f781fc799347cfc95952383",
-                "sha256:d945239a5639b3ff35b70a88c5f2f491913eb94871780ebfabb2568bd58afc5a",
-                "sha256:eba7011090323c1dadf18b3b689845fd96a61ba0a1dfbd7f24b921398affc357",
-                "sha256:efa1909120ce98bbb3777e8b6f92237f5d5c8ea6758efea36a473e1d38f7d3e4",
-                "sha256:f3900e8a5de27447acbf900b4750b0ddfd7ec1ea7fbaf11dfa911141bc522af0"
+                "sha256:09763491ce220c0299688940f8dc2c5d05fd1f45af1e42e636b2e8b2303e4382",
+                "sha256:0a891e4e41b54fd5b8313b96399f8b0e173bbbfc03c7631f01efbe29bb0bcf82",
+                "sha256:189bbd5d41ae7a498397287c408617fe5c48633e7755287b21d741f7db2706a9",
+                "sha256:18b78ec83edbbeb69efdc0e9c1cb41a3b1b1ed11ddd8ded602464c3fc6020494",
+                "sha256:1aa3de4088c89a1b69f8ec0dcc169aa725b0ff017899ac568fe44ddc1396df46",
+                "sha256:212774e4dfa851e74d393a2370871e174d7ff0ebc980907723bb67d25c8a7c30",
+                "sha256:2d0daa332786cf3bb49e10dc6a17a52f6a8f9601b4cf5c295a4f85854d61de63",
+                "sha256:5f83ac4d83ef0ab017683d715ed356e30dd48a93746309c8f3517e1287523ef4",
+                "sha256:659fb5809fa4629b8a1ac5106f669cfc7bef26fbb389dda53b3e010d1ac4ebae",
+                "sha256:660c94ea760b3ce47d1855a30984c78327500493d396eac4dfd8bd82041b22be",
+                "sha256:66a3de4a3ec06cd8af3f61b8e1ec67614fbb7c995d02fa224813cb7afefee701",
+                "sha256:721532711daa7db0d8b779b0bb0318fa87af1c10d7fe5e52ef30f8eff254d0cd",
+                "sha256:7322c3d6f1766d4ef1e51a465f47955f1e8123caee67dd641e67d539a534d006",
+                "sha256:79a31b086e7e68b24b99b23d57723ef7e2c6d81ed21007b6281ebcd1688acb0a",
+                "sha256:81fc4d08b062b535d95c9ea70dbe8a335c45c04029878e62d744bdced5141586",
+                "sha256:8fa02eaab317b1e9e03f69aab1f91e120e7899b392c4fc19807a8278a07a97e8",
+                "sha256:9090d8e53235aa280fc9239a86ae3ea8ac58eff66a705fa6aa2ec4968b95c821",
+                "sha256:946d27deaff6cf8452ed0dba83ba38839a87f4f7a9732e8f9fd4107b21e6ff07",
+                "sha256:9990d8e71b9f6488e91ad25f322898c136b008d87bf852ff65391b004da5e17b",
+                "sha256:9cd077f3d04a58e83d04b20e334f678c2b0ff9879b9375ed107d5d07ff160171",
+                "sha256:9e7551208b2aded9c1447453ee366f1c4070602b3d932ace044715d89666899b",
+                "sha256:9f5fa4a61ce2438267163891961cfd5e32ec97a2c444e5b842d574251ade27d2",
+                "sha256:b40387277b0ed2d0602b8293b94d7257e17d1479e257b4de114ea11a8cb7f2d7",
+                "sha256:bfb38f9ffb53b942f2b5954e0f610f1e721ccebe9cce9025a38c8ccf4a5183a4",
+                "sha256:cbf9b082426036e19c6924a9ce90c740a9861e2bdc27a4834fd0a910742ac1e8",
+                "sha256:d9e25ef10a39e8afe59a5c348a4dbf29b4868ab76269f81ce1674494e2565a6e",
+                "sha256:db1c1722726f47e10e0b5fdbf15ac3b8adb58c091d12b3ab713965795036985f",
+                "sha256:e7c21c95cae3c05c14aafffe2865bbd5e377cfc1348c4f7751d9dc9a48ca4bda",
+                "sha256:e8c6cfb338b133fbdbc5cfaa10fe3c6aeea827db80c978dbd13bc9dd8526b7d4",
+                "sha256:ea806fd4c37bf7e7ad82537b0757999264d5f70c45468447bb2b91afdbe73a6e",
+                "sha256:edd20c5a55acb67c7ed471fa2b5fb66cb17f61430b7a6b9c3b4a1e40293b1671",
+                "sha256:f0117049dd1d5635bbff65444496c90e0baa48ea405125c088e93d9cf4525b11",
+                "sha256:f0705c376533ed2a9e5e97aacdbfe04cecd71e0aa84c7c0595d02ef93b6e4455",
+                "sha256:f12ad7126ae0c98d601a7ee504c1122bcef553d1d5e0c3bfa77b16b3968d2734",
+                "sha256:f2457189d8257dd41ae9b434ba33298aec198e30adf2dcdaaa3a28b9994f6adb",
+                "sha256:f699ac1c768270c9e384e4cbd268d6e67aebcfae6cd623b4d7c3bfde5a35db59"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
-            "version": "==1.4.3"
+            "markers": "python_version >= '3.7'",
+            "version": "==1.9.0"
+        },
+        "markdown-it-py": {
+            "hashes": [
+                "sha256:355216845c60bd96232cd8d8c40e8f9765cc86f46880e43a8fd22dc1a1a8cab1",
+                "sha256:e3f60a94fa066dc52ec76661e37c851cb232d92f9886b15cb560aaada2df8feb"
+            ],
+            "markers": "python_version >= '3.8'",
+            "version": "==3.0.0"
         },
         "markupsafe": {
             "hashes": [
-                "sha256:0212a68688482dc52b2d45013df70d169f542b7394fc744c02a57374a4207003",
-                "sha256:089cf3dbf0cd6c100f02945abeb18484bd1ee57a079aefd52cffd17fba910b88",
-                "sha256:10c1bfff05d95783da83491be968e8fe789263689c02724e0c691933c52994f5",
-                "sha256:33b74d289bd2f5e527beadcaa3f401e0df0a89927c1559c8566c066fa4248ab7",
-                "sha256:3799351e2336dc91ea70b034983ee71cf2f9533cdff7c14c90ea126bfd95d65a",
-                "sha256:3ce11ee3f23f79dbd06fb3d63e2f6af7b12db1d46932fe7bd8afa259a5996603",
-                "sha256:421be9fbf0ffe9ffd7a378aafebbf6f4602d564d34be190fc19a193232fd12b1",
-                "sha256:43093fb83d8343aac0b1baa75516da6092f58f41200907ef92448ecab8825135",
-                "sha256:46d00d6cfecdde84d40e572d63735ef81423ad31184100411e6e3388d405e247",
-                "sha256:4a33dea2b688b3190ee12bd7cfa29d39c9ed176bda40bfa11099a3ce5d3a7ac6",
-                "sha256:4b9fe39a2ccc108a4accc2676e77da025ce383c108593d65cc909add5c3bd601",
-                "sha256:56442863ed2b06d19c37f94d999035e15ee982988920e12a5b4ba29b62ad1f77",
-                "sha256:671cd1187ed5e62818414afe79ed29da836dde67166a9fac6d435873c44fdd02",
-                "sha256:694deca8d702d5db21ec83983ce0bb4b26a578e71fbdbd4fdcd387daa90e4d5e",
-                "sha256:6a074d34ee7a5ce3effbc526b7083ec9731bb3cbf921bbe1d3005d4d2bdb3a63",
-                "sha256:6d0072fea50feec76a4c418096652f2c3238eaa014b2f94aeb1d56a66b41403f",
-                "sha256:6fbf47b5d3728c6aea2abb0589b5d30459e369baa772e0f37a0320185e87c980",
-                "sha256:7f91197cc9e48f989d12e4e6fbc46495c446636dfc81b9ccf50bb0ec74b91d4b",
-                "sha256:86b1f75c4e7c2ac2ccdaec2b9022845dbb81880ca318bb7a0a01fbf7813e3812",
-                "sha256:8dc1c72a69aa7e082593c4a203dcf94ddb74bb5c8a731e4e1eb68d031e8498ff",
-                "sha256:8e3dcf21f367459434c18e71b2a9532d96547aef8a871872a5bd69a715c15f96",
-                "sha256:8e576a51ad59e4bfaac456023a78f6b5e6e7651dcd383bcc3e18d06f9b55d6d1",
-                "sha256:96e37a3dc86e80bf81758c152fe66dbf60ed5eca3d26305edf01892257049925",
-                "sha256:97a68e6ada378df82bc9f16b800ab77cbf4b2fada0081794318520138c088e4a",
-                "sha256:99a2a507ed3ac881b975a2976d59f38c19386d128e7a9a18b7df6fff1fd4c1d6",
-                "sha256:a49907dd8420c5685cfa064a1335b6754b74541bbb3706c259c02ed65b644b3e",
-                "sha256:b09bf97215625a311f669476f44b8b318b075847b49316d3e28c08e41a7a573f",
-                "sha256:b7bd98b796e2b6553da7225aeb61f447f80a1ca64f41d83612e6139ca5213aa4",
-                "sha256:b87db4360013327109564f0e591bd2a3b318547bcef31b468a92ee504d07ae4f",
-                "sha256:bcb3ed405ed3222f9904899563d6fc492ff75cce56cba05e32eff40e6acbeaa3",
-                "sha256:d4306c36ca495956b6d568d276ac11fdd9c30a36f1b6eb928070dc5360b22e1c",
-                "sha256:d5ee4f386140395a2c818d149221149c54849dfcfcb9f1debfe07a8b8bd63f9a",
-                "sha256:dda30ba7e87fbbb7eab1ec9f58678558fd9a6b8b853530e176eabd064da81417",
-                "sha256:e04e26803c9c3851c931eac40c695602c6295b8d432cbe78609649ad9bd2da8a",
-                "sha256:e1c0b87e09fa55a220f058d1d49d3fb8df88fbfab58558f1198e08c1e1de842a",
-                "sha256:e72591e9ecd94d7feb70c1cbd7be7b3ebea3f548870aa91e2732960fa4d57a37",
-                "sha256:e8c843bbcda3a2f1e3c2ab25913c80a3c5376cd00c6e8c4a86a89a28c8dc5452",
-                "sha256:efc1913fd2ca4f334418481c7e595c00aad186563bbc1ec76067848c7ca0a933",
-                "sha256:f121a1420d4e173a5d96e47e9a0c0dcff965afdf1626d28de1460815f7c4ee7a",
-                "sha256:fc7b548b17d238737688817ab67deebb30e8073c95749d55538ed473130ec0c7"
+                "sha256:05fb21170423db021895e1ea1e1f3ab3adb85d1c2333cbc2310f2a26bc77272e",
+                "sha256:0a4e4a1aff6c7ac4cd55792abf96c915634c2b97e3cc1c7129578aa68ebd754e",
+                "sha256:10bbfe99883db80bdbaff2dcf681dfc6533a614f700da1287707e8a5d78a8431",
+                "sha256:134da1eca9ec0ae528110ccc9e48041e0828d79f24121a1a146161103c76e686",
+                "sha256:1577735524cdad32f9f694208aa75e422adba74f1baee7551620e43a3141f559",
+                "sha256:1b40069d487e7edb2676d3fbdb2b0829ffa2cd63a2ec26c4938b2d34391b4ecc",
+                "sha256:282c2cb35b5b673bbcadb33a585408104df04f14b2d9b01d4c345a3b92861c2c",
+                "sha256:2c1b19b3aaacc6e57b7e25710ff571c24d6c3613a45e905b1fde04d691b98ee0",
+                "sha256:2ef12179d3a291be237280175b542c07a36e7f60718296278d8593d21ca937d4",
+                "sha256:338ae27d6b8745585f87218a3f23f1512dbf52c26c28e322dbe54bcede54ccb9",
+                "sha256:3c0fae6c3be832a0a0473ac912810b2877c8cb9d76ca48de1ed31e1c68386575",
+                "sha256:3fd4abcb888d15a94f32b75d8fd18ee162ca0c064f35b11134be77050296d6ba",
+                "sha256:42de32b22b6b804f42c5d98be4f7e5e977ecdd9ee9b660fda1a3edf03b11792d",
+                "sha256:504b320cd4b7eff6f968eddf81127112db685e81f7e36e75f9f84f0df46041c3",
+                "sha256:525808b8019e36eb524b8c68acdd63a37e75714eac50e988180b169d64480a00",
+                "sha256:56d9f2ecac662ca1611d183feb03a3fa4406469dafe241673d521dd5ae92a155",
+                "sha256:5bbe06f8eeafd38e5d0a4894ffec89378b6c6a625ff57e3028921f8ff59318ac",
+                "sha256:65c1a9bcdadc6c28eecee2c119465aebff8f7a584dd719facdd9e825ec61ab52",
+                "sha256:68e78619a61ecf91e76aa3e6e8e33fc4894a2bebe93410754bd28fce0a8a4f9f",
+                "sha256:69c0f17e9f5a7afdf2cc9fb2d1ce6aabdb3bafb7f38017c0b77862bcec2bbad8",
+                "sha256:6b2b56950d93e41f33b4223ead100ea0fe11f8e6ee5f641eb753ce4b77a7042b",
+                "sha256:787003c0ddb00500e49a10f2844fac87aa6ce977b90b0feaaf9de23c22508b24",
+                "sha256:7ef3cb2ebbf91e330e3bb937efada0edd9003683db6b57bb108c4001f37a02ea",
+                "sha256:8023faf4e01efadfa183e863fefde0046de576c6f14659e8782065bcece22198",
+                "sha256:8758846a7e80910096950b67071243da3e5a20ed2546e6392603c096778d48e0",
+                "sha256:8afafd99945ead6e075b973fefa56379c5b5c53fd8937dad92c662da5d8fd5ee",
+                "sha256:8c41976a29d078bb235fea9b2ecd3da465df42a562910f9022f1a03107bd02be",
+                "sha256:8e254ae696c88d98da6555f5ace2279cf7cd5b3f52be2b5cf97feafe883b58d2",
+                "sha256:9402b03f1a1b4dc4c19845e5c749e3ab82d5078d16a2a4c2cd2df62d57bb0707",
+                "sha256:962f82a3086483f5e5f64dbad880d31038b698494799b097bc59c2edf392fce6",
+                "sha256:9dcdfd0eaf283af041973bff14a2e143b8bd64e069f4c383416ecd79a81aab58",
+                "sha256:aa7bd130efab1c280bed0f45501b7c8795f9fdbeb02e965371bbef3523627779",
+                "sha256:ab4a0df41e7c16a1392727727e7998a467472d0ad65f3ad5e6e765015df08636",
+                "sha256:ad9e82fb8f09ade1c3e1b996a6337afac2b8b9e365f926f5a61aacc71adc5b3c",
+                "sha256:af598ed32d6ae86f1b747b82783958b1a4ab8f617b06fe68795c7f026abbdcad",
+                "sha256:b076b6226fb84157e3f7c971a47ff3a679d837cf338547532ab866c57930dbee",
+                "sha256:b7ff0f54cb4ff66dd38bebd335a38e2c22c41a8ee45aa608efc890ac3e3931bc",
+                "sha256:bfce63a9e7834b12b87c64d6b155fdd9b3b96191b6bd334bf37db7ff1fe457f2",
+                "sha256:c011a4149cfbcf9f03994ec2edffcb8b1dc2d2aede7ca243746df97a5d41ce48",
+                "sha256:c9c804664ebe8f83a211cace637506669e7890fec1b4195b505c214e50dd4eb7",
+                "sha256:ca379055a47383d02a5400cb0d110cef0a776fc644cda797db0c5696cfd7e18e",
+                "sha256:cb0932dc158471523c9637e807d9bfb93e06a95cbf010f1a38b98623b929ef2b",
+                "sha256:cd0f502fe016460680cd20aaa5a76d241d6f35a1c3350c474bac1273803893fa",
+                "sha256:ceb01949af7121f9fc39f7d27f91be8546f3fb112c608bc4029aef0bab86a2a5",
+                "sha256:d080e0a5eb2529460b30190fcfcc4199bd7f827663f858a226a81bc27beaa97e",
+                "sha256:dd15ff04ffd7e05ffcb7fe79f1b98041b8ea30ae9234aed2a9168b5797c3effb",
+                "sha256:df0be2b576a7abbf737b1575f048c23fb1d769f267ec4358296f31c2479db8f9",
+                "sha256:e09031c87a1e51556fdcb46e5bd4f59dfb743061cf93c4d6831bf894f125eb57",
+                "sha256:e4dd52d80b8c83fdce44e12478ad2e85c64ea965e75d66dbeafb0a3e77308fcc",
+                "sha256:fec21693218efe39aa7f8599346e90c705afa52c5b31ae019b2e57e8f6542bb2"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==2.1.1"
+            "version": "==2.1.3"
         },
         "mccabe": {
             "hashes": [
-                "sha256:ab8a6258860da4b6677da4bd2fe5dc2c659cff31b3ee4f7f5d64e79735b80d42",
-                "sha256:dd8d182285a0fe56bace7f45b5e7d1a6ebcbf524e8f3bd87eb0f125271b8831f"
+                "sha256:348e0240c33b60bbdf4e523192ef919f28cb2c3d7d5c7794f74009290f236325",
+                "sha256:6c2d30ab6be0e4a46919781807b4f0d834ebdd6c6e3dca0bda5a15f863427b6e"
             ],
-            "version": "==0.6.1"
+            "markers": "python_version >= '3.6'",
+            "version": "==0.7.0"
+        },
+        "mdurl": {
+            "hashes": [
+                "sha256:84008a41e51615a49fc9966191ff91509e3c40b939176e643fd50a5c2196b8f8",
+                "sha256:bb413d29f5eea38f31dd4754dd7377d4465116fb207585f97bf925588687c1ba"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==0.1.2"
+        },
+        "more-itertools": {
+            "hashes": [
+                "sha256:cabaa341ad0389ea83c17a94566a53ae4c9d07349861ecb14dc6d0345cf9ac5d",
+                "sha256:d2bc7f02446e86a68911e58ded76d6561eea00cddfb2a91e7019bbb586c799f3"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==9.1.0"
         },
         "nose": {
             "hashes": [
                 "sha256:9ff7c6cc443f8c51994b34a667bbcf45afd6d945be7477b52e97516fd17c53ac",
                 "sha256:dadcddc0aefbf99eea214e0f1232b94f2fa9bd98fa8353711dacb112bfcbbb2a",
                 "sha256:f1bffef9cbc82628f6e7d7b40d7e255aefaa1adb6a1b1d26c69a8b79e6208a98"
             ],
@@ -343,125 +559,111 @@
                 "sha256:ab2d0dca21aa5a7ae280c6fb869882260b825d9ced368b557b9124cf51ffb119"
             ],
             "index": "pypi",
             "version": "==0.6.0"
         },
         "packaging": {
             "hashes": [
-                "sha256:dd47c42927d89ab911e606518907cc2d3a1f38bbd026385970643f9c5b8ecfeb",
-                "sha256:ef103e05f519cdc783ae24ea4e2e0f508a9c99b2d4969652eed6a2e1ea5bd522"
+                "sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61",
+                "sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==21.3"
+            "markers": "python_version >= '3.7'",
+            "version": "==23.1"
         },
         "pep8-naming": {
             "hashes": [
                 "sha256:5d9f1056cb9427ce344e98d1a7f5665710e2f20f748438e308995852cfa24164",
                 "sha256:f3b4a5f9dd72b991bf7d8e2a341d2e1aa3a884a769b5aaac4f56825c1763bf3a"
             ],
             "version": "==0.10.0"
         },
         "pkginfo": {
             "hashes": [
-                "sha256:542e0d0b6750e2e21c20179803e40ab50598d8066d51097a0e382cba9eb02bff",
-                "sha256:c24c487c6a7f72c66e816ab1796b96ac6c3d14d49338293d2141664330b55ffc"
+                "sha256:4b7a555a6d5a22169fcc9cf7bfd78d296b0361adad412a346c1226849af5e546",
+                "sha256:8fd5896e8718a4372f0ea9cc9d96f6417c9b986e23a4d116dda26b62cc29d046"
             ],
-            "version": "==1.8.2"
+            "markers": "python_version >= '3.6'",
+            "version": "==1.9.6"
         },
         "platformdirs": {
             "hashes": [
-                "sha256:7535e70dfa32e84d4b34996ea99c5e432fa29a708d0f4e394bbcb2a8faa4f16d",
-                "sha256:bcae7cab893c2d310a711b70b24efb93334febe65f8de776ee320b517471e227"
+                "sha256:0ade98a4895e87dc51d47151f7d2ec290365a585151d97b4d8d6312ed6132fed",
+                "sha256:e48fabd87db8f3a7df7150a4a5ea22c546ee8bc39bc2473244730d4b56d2cc4e"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==2.5.1"
+            "version": "==3.5.3"
         },
         "pluggy": {
             "hashes": [
-                "sha256:15b2acde666561e1298d71b523007ed7364de07029219b604cf808bfa1c765b0",
-                "sha256:966c145cd83c96502c3c3868f50408687b38434af77734af1e9ca461a4081d2d"
+                "sha256:4224373bacce55f955a878bf9cfa763c1e360858e330072059e10bad68531159",
+                "sha256:74134bbf457f031a36d68416e1509f34bd5ccc019f0bcc952c7b909d06b37bd3"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
-            "version": "==0.13.1"
-        },
-        "poetry-semver": {
-            "hashes": [
-                "sha256:4e6349bd7231cc657f0e1930f7b204e87e33dfd63eef5cac869363969515083a",
-                "sha256:d809b612aa27b39bf2d0fc9d31b4f4809b0e972646c5f19cfa46c725b7638810"
-            ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
-            "version": "==0.1.0"
+            "markers": "python_version >= '3.6'",
+            "version": "==1.0.0"
         },
         "prospector": {
             "hashes": [
-                "sha256:700d7918d93d73035a2a58fb18c6be0b609a0481fc6e0908843fa856b89e52c6"
+                "sha256:3bfe103c28bb821cca84926ca31357fbfd32405e4bf8c34ca2e55885684557e4",
+                "sha256:cc8f09e79bdd32247edddf05b666940e88ad96338a84f5717b1e8c0678337821"
             ],
             "index": "pypi",
-            "version": "==1.3.1"
-        },
-        "py": {
-            "hashes": [
-                "sha256:51c75c4126074b472f746a24399ad32f6053d1b34b68d2fa41e558e6f4a98719",
-                "sha256:607c53218732647dff4acdfcd50cb62615cedf612e72d1724fb1a0cc6405b378"
-            ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
-            "version": "==1.11.0"
+            "version": "==1.10.2"
         },
         "pycodestyle": {
             "hashes": [
-                "sha256:2295e7b2f6b5bd100585ebcb1f616591b652db8a741695b3d8f5d28bdc934367",
-                "sha256:c58a7d2815e0e8d7972bf1803331fb0152f867bd89adf8a01dfd55085434192e"
+                "sha256:2c9607871d58c76354b697b42f5d57e1ada7d261c261efac224b664affdc5785",
+                "sha256:d1735fc58b418fd7c5f658d28d943854f8a849b01a5d0a1e6f3f3fdd0166804b"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
-            "version": "==2.6.0"
+            "markers": "python_version >= '3.6'",
+            "version": "==2.9.1"
         },
         "pydocstyle": {
             "hashes": [
-                "sha256:1d41b7c459ba0ee6c345f2eb9ae827cab14a7533a88c5c6f7e94923f72df92dc",
-                "sha256:6987826d6775056839940041beef5c08cc7e3d71d63149b48e36727f70144dc4"
+                "sha256:118762d452a49d6b05e194ef344a55822987a462831ade91ec5c06fd2169d019",
+                "sha256:7ce43f0c0ac87b07494eb9c0b462c0b73e6ff276807f204d6b53edc72b7e44e1"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==6.1.1"
+            "version": "==6.3.0"
         },
         "pyflakes": {
             "hashes": [
-                "sha256:0d94e0e05a19e57a99444b6ddcf9a6eb2e5c68d3ca1e98e90707af8152c90a92",
-                "sha256:35b2d75ee967ea93b55750aa9edbbf72813e06a66ba54438df2cfac9e3c27fc8"
+                "sha256:4579f67d887f804e67edb544428f264b7b24f435b263c4614f384135cea553d2",
+                "sha256:491feb020dca48ccc562a8c0cbe8df07ee13078df59813b83959cbdada312ea3"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
-            "version": "==2.2.0"
+            "markers": "python_version >= '3.6'",
+            "version": "==2.5.0"
         },
         "pygments": {
             "hashes": [
-                "sha256:44238f1b60a76d78fc8ca0528ee429702aae011c265fe6a8dd8b63049ae41c65",
-                "sha256:4e426f72023d88d03b2fa258de560726ce890ff3b630f88c21cbb8b2503b8c6a"
+                "sha256:8ace4d3c1dd481894b2005f560ead0f9f19ee64fe983366be1a21e171d12775c",
+                "sha256:db2db3deb4b4179f399a09054b023b6a586b76499d36965813c71aa8ed7b5fd1"
             ],
-            "markers": "python_version >= '3.5'",
-            "version": "==2.11.2"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.15.1"
         },
         "pylint": {
             "hashes": [
-                "sha256:7dd78437f2d8d019717dbf287772d0b2dbdfd13fc016aa7faa08d67bccc46adc",
-                "sha256:d0ece7d223fe422088b0e8f13fa0a1e8eb745ebffcb8ed53d3e95394b6101a1c"
+                "sha256:5dcf1d9e19f41f38e4e85d10f511e5b9c35e1aa74251bf95cdd8cb23584e2db1",
+                "sha256:7a1145fb08c251bdb5cca11739722ce64a63db479283d10ce718b2460e54123c"
             ],
-            "markers": "python_version >= '3.5'",
-            "version": "==2.5.3"
+            "markers": "python_full_version >= '3.7.2'",
+            "version": "==2.17.4"
         },
         "pylint-celery": {
             "hashes": [
                 "sha256:41e32094e7408d15c044178ea828dd524beedbdbe6f83f712c5e35bde1de4beb"
             ],
             "version": "==0.3"
         },
         "pylint-django": {
             "hashes": [
-                "sha256:b7756844dba0cecd3471056a1ef4154439defedaba38bf3ced9f848d2bf6297c",
-                "sha256:ca32277c77878dd3c2d9e75f3f3f7f0c0712f053f10ff1b946cdc27367a6c911"
+                "sha256:0ac090d106c62fe33782a1d01bda1610b761bb1c9bf5035ced9d5f23a13d8591",
+                "sha256:56b12b6adf56d548412445bd35483034394a1a94901c3f8571980a13882299d5"
             ],
-            "version": "==2.1.0"
+            "version": "==2.5.3"
         },
         "pylint-flask": {
             "hashes": [
                 "sha256:f4d97de2216bf7bfce07c9c08b166e978fe9f2725de2a50a9845a97de7e31517"
             ],
             "version": "==0.6"
         },
@@ -469,186 +671,201 @@
             "hashes": [
                 "sha256:b3d43e85ab74c4f48bb46ae4ce771e39c3a20f8b3d56982ab17aa73b4f98d535",
                 "sha256:ce48bc0516ae9415dd5c752c940dfe601b18fe0f48aa249f2386adfa95a004dd"
             ],
             "markers": "python_full_version >= '3.6.2'",
             "version": "==0.7"
         },
-        "pyparsing": {
-            "hashes": [
-                "sha256:18ee9022775d270c55187733956460083db60b37d0d0fb357445f3094eed3eea",
-                "sha256:a6c06a88f252e6c322f65faf8f418b16213b51bdfaece0524c1c1bc30c63c484"
-            ],
-            "markers": "python_version >= '3.6'",
-            "version": "==3.0.7"
-        },
-        "pytz": {
+        "pyproject-api": {
             "hashes": [
-                "sha256:1e760e2fe6a8163bc0b3d9a19c4f84342afa0a2affebfaa84b01b978a02ecaa7",
-                "sha256:e68985985296d9a66a881eb3193b0906246245294a881e7c8afe623866ac6a5c"
+                "sha256:435f46547a9ff22cf4208ee274fca3e2869aeb062a4834adfc99a4dd64af3cf9",
+                "sha256:4698a3777c2e0f6b624f8a4599131e2a25376d90fe8d146d7ac74c67c6f97c43"
             ],
-            "version": "==2022.1"
+            "markers": "python_version >= '3.7'",
+            "version": "==1.5.1"
         },
         "pyyaml": {
             "hashes": [
+                "sha256:01b45c0191e6d66c470b6cf1b9531a771a83c1c4208272ead47a3ae4f2f603bf",
                 "sha256:0283c35a6a9fbf047493e3a0ce8d79ef5030852c51e9d911a27badfde0605293",
                 "sha256:055d937d65826939cb044fc8c9b08889e8c743fdc6a32b33e2390f66013e449b",
                 "sha256:07751360502caac1c067a8132d150cf3d61339af5691fe9e87803040dbc5db57",
                 "sha256:0b4624f379dab24d3725ffde76559cff63d9ec94e1736b556dacdfebe5ab6d4b",
                 "sha256:0ce82d761c532fe4ec3f87fc45688bdd3a4c1dc5e0b4a19814b9009a29baefd4",
                 "sha256:1e4747bc279b4f613a09eb64bba2ba602d8a6664c6ce6396a4d0cd413a50ce07",
                 "sha256:213c60cd50106436cc818accf5baa1aba61c0189ff610f64f4a3e8c6726218ba",
                 "sha256:231710d57adfd809ef5d34183b8ed1eeae3f76459c18fb4a0b373ad56bedcdd9",
                 "sha256:277a0ef2981ca40581a47093e9e2d13b3f1fbbeffae064c1d21bfceba2030287",
                 "sha256:2cd5df3de48857ed0544b34e2d40e9fac445930039f3cfe4bcc592a1f836d513",
                 "sha256:40527857252b61eacd1d9af500c3337ba8deb8fc298940291486c465c8b46ec0",
+                "sha256:432557aa2c09802be39460360ddffd48156e30721f5e8d917f01d31694216782",
                 "sha256:473f9edb243cb1935ab5a084eb238d842fb8f404ed2193a915d1784b5a6b5fc0",
                 "sha256:48c346915c114f5fdb3ead70312bd042a953a8ce5c7106d5bfb1a5254e47da92",
                 "sha256:50602afada6d6cbfad699b0c7bb50d5ccffa7e46a3d738092afddc1f9758427f",
                 "sha256:68fb519c14306fec9720a2a5b45bc9f0c8d1b9c72adf45c37baedfcd949c35a2",
                 "sha256:77f396e6ef4c73fdc33a9157446466f1cff553d979bd00ecb64385760c6babdc",
+                "sha256:81957921f441d50af23654aa6c5e5eaf9b06aba7f0a19c18a538dc7ef291c5a1",
                 "sha256:819b3830a1543db06c4d4b865e70ded25be52a2e0631ccd2f6a47a2822f2fd7c",
                 "sha256:897b80890765f037df3403d22bab41627ca8811ae55e9a722fd0392850ec4d86",
                 "sha256:98c4d36e99714e55cfbaaee6dd5badbc9a1ec339ebfc3b1f52e293aee6bb71a4",
                 "sha256:9df7ed3b3d2e0ecfe09e14741b857df43adb5a3ddadc919a2d94fbdf78fea53c",
                 "sha256:9fa600030013c4de8165339db93d182b9431076eb98eb40ee068700c9c813e34",
                 "sha256:a80a78046a72361de73f8f395f1f1e49f956c6be882eed58505a15f3e430962b",
+                "sha256:afa17f5bc4d1b10afd4466fd3a44dc0e245382deca5b3c353d8b757f9e3ecb8d",
                 "sha256:b3d267842bf12586ba6c734f89d1f5b871df0273157918b0ccefa29deb05c21c",
                 "sha256:b5b9eccad747aabaaffbc6064800670f0c297e52c12754eb1d976c57e4f74dcb",
+                "sha256:bfaef573a63ba8923503d27530362590ff4f576c626d86a9fed95822a8255fd7",
                 "sha256:c5687b8d43cf58545ade1fe3e055f70eac7a5a1a0bf42824308d868289a95737",
                 "sha256:cba8c411ef271aa037d7357a2bc8f9ee8b58b9965831d9e51baf703280dc73d3",
                 "sha256:d15a181d1ecd0d4270dc32edb46f7cb7733c7c508857278d3d378d14d606db2d",
+                "sha256:d4b0ba9512519522b118090257be113b9468d804b19d63c71dbcf4a48fa32358",
                 "sha256:d4db7c7aef085872ef65a8fd7d6d09a14ae91f691dec3e87ee5ee0539d516f53",
                 "sha256:d4eccecf9adf6fbcc6861a38015c2a64f38b9d94838ac1810a9023a0609e1b78",
                 "sha256:d67d839ede4ed1b28a4e8909735fc992a923cdb84e618544973d7dfc71540803",
                 "sha256:daf496c58a8c52083df09b80c860005194014c3698698d1a57cbcfa182142a3a",
+                "sha256:dbad0e9d368bb989f4515da330b88a057617d16b6a8245084f1b05400f24609f",
                 "sha256:e61ceaab6f49fb8bdfaa0f92c4b57bcfbea54c09277b1b4f7ac376bfb7a7c174",
                 "sha256:f84fbc98b019fef2ee9a1cb3ce93e3187a6df0b2538a651bfb890254ba9f90b5"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==6.0"
         },
         "readme-renderer": {
             "hashes": [
-                "sha256:262510fe6aae81ed4e94d8b169077f325614c0b1a45916a80442c6576264a9c2",
-                "sha256:dfb4d17f21706d145f7473e0b61ca245ba58e810cf9b2209a48239677f82e5b0"
+                "sha256:cd653186dfc73055656f090f227f5cb22a046d7f71a841dfa305f55c9a513273",
+                "sha256:f67a16caedfa71eef48a31b39708637a6f4664c4394801a7b0d6432d13907343"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==34.0"
+            "markers": "python_version >= '3.7'",
+            "version": "==37.3"
         },
         "requests": {
             "hashes": [
-                "sha256:68d7c56fd5a8999887728ef304a6d12edc7be74f1cfa47714fc8b414525c9a61",
-                "sha256:f22fa1e554c9ddfd16e6e41ac79759e17be9e492b3587efa038054674760e72d"
+                "sha256:58cd2187c01e70e6e26505bca751777aa9f2ee0b7f4300988b709f44e013003f",
+                "sha256:942c5a758f98d790eaed1a29cb6eefc7ffb0d1cf7af05c3d2791656dbd6ad1e1"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'",
-            "version": "==2.27.1"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.31.0"
         },
         "requests-toolbelt": {
             "hashes": [
-                "sha256:380606e1d10dc85c3bd47bf5a6095f815ec007be7a8b69c878507068df059e6f",
-                "sha256:968089d4584ad4ad7c171454f0a5c6dac23971e9472521ea3b6d49d610aa6fc0"
+                "sha256:7681a0a3d047012b5bdc0ee37d7f8f07ebe76ab08caeccfc3921ce23c88d5bc6",
+                "sha256:cccfdd665f0a24fcf4726e690f65639d272bb0637b9b92dfd91a5568ccf6bd06"
             ],
-            "version": "==0.9.1"
+            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
+            "version": "==1.0.0"
         },
         "requirements-detector": {
             "hashes": [
-                "sha256:6c32d39a36612a20d4b0d29e9b6ffbf82a42ce7aa9f8a2f620ac467cccaf8bc2",
-                "sha256:98ef5113d991f2aa30b229fe6f63f2878c7e35326e9e21d71ef8113021e2eefa"
+                "sha256:3642cd7a5b261d79536c36bb7ecacf2adabd902d2e0e42bfb2ba82515da10501",
+                "sha256:d7c60493bf166da3dd59de0e6cb25765e0e32a1931aeae92614034e5786d0bd0"
             ],
-            "markers": "python_version < '4' and python_full_version >= '3.6.2'",
-            "version": "==1.0.2"
+            "markers": "python_version >= '3.7' and python_version < '4.0'",
+            "version": "==1.2.2"
         },
-        "semver": {
+        "rfc3986": {
             "hashes": [
-                "sha256:41c9aa26c67dc16c54be13074c352ab666bce1fa219c7110e8f03374cd4206b0",
-                "sha256:5b09010a66d9a3837211bb7ae5a20d10ba88f8cb49e92cb139a69ef90d5060d8"
+                "sha256:50b1502b60e289cb37883f3dfd34532b8873c7de9f49bb546641ce9cbd256ebd",
+                "sha256:97aacf9dbd4bfd829baad6e6309fa6573aaf1be3f6fa735c8ab05e46cecb261c"
             ],
-            "index": "pypi",
-            "version": "==2.8.1"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.0.0"
         },
-        "setoptconf": {
+        "rich": {
             "hashes": [
-                "sha256:1fa613dc4a6fbfbaab9a52319d1e369d030e8ed80455b151574ccf3390ec86c6",
-                "sha256:d2ecbd27c0c7d0d53990e2df98d9aad6490df8b75b71c621d8c441d6e91e3161"
+                "sha256:8f87bc7ee54675732fa66a05ebfe489e27264caeeff3728c945d25971b6485ec",
+                "sha256:d653d6bccede5844304c605d5aac802c7cf9621efd700b46c7ec2b51ea914898"
             ],
-            "markers": "python_version >= '3.0'",
-            "version": "==0.3.0"
+            "markers": "python_full_version >= '3.7.0'",
+            "version": "==13.4.2"
         },
-        "setuptools": {
+        "semver": {
             "hashes": [
-                "sha256:6599055eeb23bfef457d5605d33a4d68804266e6cb430b0fb12417c5efeae36c",
-                "sha256:782ef48d58982ddb49920c11a0c5c9c0b02e7d7d1c2ad0aa44e1a1e133051c96"
+                "sha256:94df43924c4521ec7d307fc86da1531db6c2c33d9d5cdc3e64cca0eb68569269",
+                "sha256:ab4f69fb1d1ecfb5d81f96411403d7a611fa788c45d252cf5b408025df3ab6ce"
             ],
-            "markers": "python_version >= '3.7'",
-            "version": "==60.10.0"
+            "index": "pypi",
+            "version": "==3.0.0"
         },
-        "sh": {
+        "setoptconf-tmp": {
             "hashes": [
-                "sha256:ae3258c5249493cebe73cb4e18253a41ed69262484bad36fdb3efcb8ad8870bb",
-                "sha256:b52bf5833ed01c7b5c5fb73a7f71b3d98d48e9b9b8764236237bdc7ecae850fc"
+                "sha256:76035d5cd1593d38b9056ae12d460eca3aaa34ad05c315b69145e138ba80a745",
+                "sha256:e0480addd11347ba52f762f3c4d8afa3e10ad0affbc53e3ffddc0ca5f27d5778"
             ],
-            "index": "pypi",
-            "markers": "sys_platform != 'win32'",
-            "version": "==1.12.14"
+            "version": "==0.3.1"
         },
         "six": {
             "hashes": [
                 "sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926",
                 "sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
             "version": "==1.16.0"
         },
+        "smmap": {
+            "hashes": [
+                "sha256:2aba19d6a040e78d8b09de5c57e96207b09ed71d8e55ce0959eeee6c8e190d94",
+                "sha256:c840e62059cd3be204b0c9c9f74be2c09d5648eddd4580d9314c3ecde0b30936"
+            ],
+            "markers": "python_version >= '3.6'",
+            "version": "==5.0.0"
+        },
         "snowballstemmer": {
             "hashes": [
                 "sha256:09b16deb8547d3412ad7b590689584cd0fe25ec8db3be37788be3810cbf19cb1",
                 "sha256:c8e1716e83cc398ae16824e5572ae04e0d9fc2c6b985fb0f900f5f0c96ecba1a"
             ],
             "version": "==2.2.0"
         },
         "sphinx": {
             "hashes": [
-                "sha256:22538e1bbe62b407cf5a8aabe1bb15848aa66bb79559f42f5202bbce6b757a69",
-                "sha256:f9a79e746b87921cabc3baa375199c6076d1270cee53915dbd24fdbeaaacc427"
+                "sha256:6d56a34697bb749ffa0152feafc4b19836c755d90a7c59b72bc7dfd371b9cc6b",
+                "sha256:97787ff1fa3256a3eef9eda523a63dbf299f7b47e053cfcf684a1c2a8380c912"
             ],
             "index": "pypi",
-            "version": "==2.1.2"
+            "version": "==6.2.1"
         },
         "sphinx-rtd-theme": {
             "hashes": [
-                "sha256:00cf895504a7895ee433807c62094cf1e95f065843bf3acd17037c3e9a2becd4",
-                "sha256:728607e34d60456d736cc7991fd236afb828b21b82f956c5ea75f94c8414040a"
+                "sha256:01c5c5a72e2d025bd23d1f06c59a4831b06e6ce6c01fdd5ebfe9986c0a880fc7",
+                "sha256:6a7e7d8af34eb8fc57d52a09c6b6b9c46ff44aea5951bc831eeb9245378f3689"
             ],
             "index": "pypi",
-            "version": "==0.4.3"
+            "version": "==1.2.2"
         },
         "sphinxcontrib-applehelp": {
             "hashes": [
-                "sha256:806111e5e962be97c29ec4c1e7fe277bfd19e9652fb1a4392105b43e01af885a",
-                "sha256:a072735ec80e7675e3f432fcae8610ecf509c5f1869d17e2eecff44389cdbc58"
+                "sha256:29d341f67fb0f6f586b23ad80e072c8e6ad0b48417db2bde114a4c9746feb228",
+                "sha256:828f867945bbe39817c210a1abfd1bc4895c8b73fcaade56d45357a348a07d7e"
             ],
-            "markers": "python_version >= '3.5'",
-            "version": "==1.0.2"
+            "markers": "python_version >= '3.8'",
+            "version": "==1.0.4"
         },
         "sphinxcontrib-devhelp": {
             "hashes": [
                 "sha256:8165223f9a335cc1af7ffe1ed31d2871f325254c0423bc0c4c7cd1c1e4734a2e",
                 "sha256:ff7f1afa7b9642e7060379360a67e9c41e8f3121f2ce9164266f61b9f4b338e4"
             ],
             "markers": "python_version >= '3.5'",
             "version": "==1.0.2"
         },
         "sphinxcontrib-htmlhelp": {
             "hashes": [
-                "sha256:d412243dfb797ae3ec2b59eca0e52dac12e75a241bf0e4eb861e450d06c6ed07",
-                "sha256:f5f8bb2d0d629f398bf47d0d69c07bc13b65f75a81ad9e2f71a63d4b7a2f6db2"
+                "sha256:0cbdd302815330058422b98a113195c9249825d681e18f11e8b1f78a2f11efff",
+                "sha256:c38cb46dccf316c79de6e5515e1770414b797162b23cd3d06e67020e1d2a6903"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==2.0.0"
+            "markers": "python_version >= '3.8'",
+            "version": "==2.0.1"
+        },
+        "sphinxcontrib-jquery": {
+            "hashes": [
+                "sha256:1620739f04e36a2c779f1a131a2dfd49b2fd07351bf1968ced074365933abc7a",
+                "sha256:f936030d7d0147dd026a4f2b5a57343d233f1fc7b363f68b3d4f1cb0993878ae"
+            ],
+            "markers": "python_version >= '2.7'",
+            "version": "==4.1"
         },
         "sphinxcontrib-jsmath": {
             "hashes": [
                 "sha256:2ec2eaebfb78f3f2078e73666b1415417a116cc848b72e5172e596c871103178",
                 "sha256:a9925e4a4587247ed2191a22df5f6970656cb8ca2bd6284309578f2153e0c4b8"
             ],
             "markers": "python_version >= '3.5'",
@@ -674,170 +891,161 @@
             "hashes": [
                 "sha256:806143ae5bfb6a3c6e736a764057db0e6a0e05e338b5630894a5f779cabb4f9b",
                 "sha256:b3bda1d108d5dd99f4a20d24d9c348e91c4db7ab1b749200bded2f839ccbe68f"
             ],
             "index": "pypi",
             "version": "==0.10.2"
         },
-        "tox": {
+        "tomli": {
             "hashes": [
-                "sha256:dab0b0160dd187b654fc33d690ee1d7bf328bd5b8dc6ef3bb3cc468969c659ba",
-                "sha256:ee35ffce74933a6c6ac10c9a0182e41763140a5a5070e21b114feca56eaccdcd"
+                "sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc",
+                "sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f"
             ],
-            "index": "pypi",
-            "version": "==3.13.2"
+            "markers": "python_version < '3.11'",
+            "version": "==2.0.1"
         },
-        "tqdm": {
+        "tomlkit": {
             "hashes": [
-                "sha256:1d9835ede8e394bb8c9dcbffbca02d717217113adc679236873eeaac5bc0b3cd",
-                "sha256:e643e071046f17139dea55b880dc9b33822ce21613b4a4f5ea57f202833dbc29"
+                "sha256:8c726c4c202bdb148667835f68d68780b9a003a9ec34167b6c673b38eff2a171",
+                "sha256:9330fc7faa1db67b541b28e62018c17d20be733177d290a13b24c62d1614e0c3"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
-            "version": "==4.63.0"
+            "markers": "python_version >= '3.7'",
+            "version": "==0.11.8"
+        },
+        "tox": {
+            "hashes": [
+                "sha256:4874000453e637a87ca892f9744a2ab9a7d24064dad1b0ecbf5a4c3c146cc732",
+                "sha256:954f1f647f67f481d239a193288983242a6152b67503c4a56b19a4aafaa29736"
+            ],
+            "index": "pypi",
+            "version": "==4.6.0"
         },
         "twine": {
             "hashes": [
-                "sha256:0fb0bfa3df4f62076cab5def36b1a71a2e4acb4d1fa5c97475b048117b1a6446",
-                "sha256:d6c29c933ecfc74e9b1d9fa13aa1f87c5d5770e119f5a4ce032092f0ff5b14dc"
+                "sha256:929bc3c280033347a00f847236564d1c52a3e61b1ac2516c97c48f3ceab756d8",
+                "sha256:9e102ef5fdd5a20661eb88fad46338806c3bd32cf1db729603fe3697b1bc83c8"
             ],
             "index": "pypi",
-            "version": "==1.13.0"
+            "version": "==4.0.2"
         },
-        "typed-ast": {
+        "typing-extensions": {
             "hashes": [
-                "sha256:01ae5f73431d21eead5015997ab41afa53aa1fbe252f9da060be5dad2c730ace",
-                "sha256:067a74454df670dcaa4e59349a2e5c81e567d8d65458d480a5b3dfecec08c5ff",
-                "sha256:0fb71b8c643187d7492c1f8352f2c15b4c4af3f6338f21681d3681b3dc31a266",
-                "sha256:1b3ead4a96c9101bef08f9f7d1217c096f31667617b58de957f690c92378b528",
-                "sha256:2068531575a125b87a41802130fa7e29f26c09a2833fea68d9a40cf33902eba6",
-                "sha256:209596a4ec71d990d71d5e0d312ac935d86930e6eecff6ccc7007fe54d703808",
-                "sha256:2c726c276d09fc5c414693a2de063f521052d9ea7c240ce553316f70656c84d4",
-                "sha256:398e44cd480f4d2b7ee8d98385ca104e35c81525dd98c519acff1b79bdaac363",
-                "sha256:52b1eb8c83f178ab787f3a4283f68258525f8d70f778a2f6dd54d3b5e5fb4341",
-                "sha256:5feca99c17af94057417d744607b82dd0a664fd5e4ca98061480fd8b14b18d04",
-                "sha256:7538e495704e2ccda9b234b82423a4038f324f3a10c43bc088a1636180f11a41",
-                "sha256:760ad187b1041a154f0e4d0f6aae3e40fdb51d6de16e5c99aedadd9246450e9e",
-                "sha256:777a26c84bea6cd934422ac2e3b78863a37017618b6e5c08f92ef69853e765d3",
-                "sha256:95431a26309a21874005845c21118c83991c63ea800dd44843e42a916aec5899",
-                "sha256:9ad2c92ec681e02baf81fdfa056fe0d818645efa9af1f1cd5fd6f1bd2bdfd805",
-                "sha256:9c6d1a54552b5330bc657b7ef0eae25d00ba7ffe85d9ea8ae6540d2197a3788c",
-                "sha256:aee0c1256be6c07bd3e1263ff920c325b59849dc95392a05f258bb9b259cf39c",
-                "sha256:af3d4a73793725138d6b334d9d247ce7e5f084d96284ed23f22ee626a7b88e39",
-                "sha256:b36b4f3920103a25e1d5d024d155c504080959582b928e91cb608a65c3a49e1a",
-                "sha256:b9574c6f03f685070d859e75c7f9eeca02d6933273b5e69572e5ff9d5e3931c3",
-                "sha256:bff6ad71c81b3bba8fa35f0f1921fb24ff4476235a6e94a26ada2e54370e6da7",
-                "sha256:c190f0899e9f9f8b6b7863debfb739abcb21a5c054f911ca3596d12b8a4c4c7f",
-                "sha256:c907f561b1e83e93fad565bac5ba9c22d96a54e7ea0267c708bffe863cbe4075",
-                "sha256:cae53c389825d3b46fb37538441f75d6aecc4174f615d048321b716df2757fb0",
-                "sha256:dd4a21253f42b8d2b48410cb31fe501d32f8b9fbeb1f55063ad102fe9c425e40",
-                "sha256:dde816ca9dac1d9c01dd504ea5967821606f02e510438120091b84e852367428",
-                "sha256:f2362f3cb0f3172c42938946dbc5b7843c2a28aec307c49100c8b38764eb6927",
-                "sha256:f328adcfebed9f11301eaedfa48e15bdece9b519fb27e6a8c01aa52a17ec31b3",
-                "sha256:f8afcf15cc511ada719a88e013cec87c11aff7b91f019295eb4530f96fe5ef2f",
-                "sha256:fb1bbeac803adea29cedd70781399c99138358c26d05fcbd23c13016b7f5ec65"
+                "sha256:88a4153d8505aabbb4e13aacb7c486c2b4a33ca3b3f807914a9b4c844c471c26",
+                "sha256:d91d5919357fe7f681a9f2b5b4cb2a5f1ef0a1e9f59c4d8ff0d3491e05c0ffd5"
             ],
-            "markers": "python_version < '3.8' and implementation_name == 'cpython'",
-            "version": "==1.4.3"
+            "markers": "python_version < '3.10'",
+            "version": "==4.6.3"
         },
         "urllib3": {
             "hashes": [
-                "sha256:44ece4d53fb1706f667c9bd1c648f5469a2ec925fcf3a776667042d645472c14",
-                "sha256:aabaf16477806a5e1dd19aa41f8c2b7950dd3c746362d7e3223dbe6de6ac448e"
+                "sha256:48e7fafa40319d358848e1bc6809b208340fafe2096f1725d05d67443d0483d1",
+                "sha256:bee28b5e56addb8226c96f7f13ac28cb4c301dd5ea8a6ca179c0b9835e032825"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4' and python_version < '4'",
-            "version": "==1.26.9"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.0.3"
         },
         "virtualenv": {
             "hashes": [
-                "sha256:c3e01300fb8495bc00ed70741f5271fc95fed067eb7106297be73d30879af60c",
-                "sha256:ce8901d3bbf3b90393498187f2d56797a8a452fb2d0d7efc6fd837554d6f679c"
+                "sha256:6abec7670e5802a528357fdc75b26b9f57d5d92f29c5462ba0fbe45feacc685e",
+                "sha256:a85caa554ced0c0afbd0d638e7e2d7b5f92d23478d05d17a76daeac8f279f924"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
-            "version": "==20.13.4"
+            "markers": "python_version >= '3.7'",
+            "version": "==20.23.0"
         },
         "webencodings": {
             "hashes": [
                 "sha256:a0af1213f3c2226497a97e2b3aa01a7e4bee4f403f95be16fc9acd2947514a78",
                 "sha256:b36a1c245f2d304965eb4e0a82848379241dc04b865afcc4aab16748587e1923"
             ],
             "version": "==0.5.1"
         },
         "wrapt": {
             "hashes": [
-                "sha256:00108411e0f34c52ce16f81f1d308a571df7784932cc7491d1e94be2ee93374b",
-                "sha256:01f799def9b96a8ec1ef6b9c1bbaf2bbc859b87545efbecc4a78faea13d0e3a0",
-                "sha256:09d16ae7a13cff43660155383a2372b4aa09109c7127aa3f24c3cf99b891c330",
-                "sha256:14e7e2c5f5fca67e9a6d5f753d21f138398cad2b1159913ec9e9a67745f09ba3",
-                "sha256:167e4793dc987f77fd476862d32fa404d42b71f6a85d3b38cbce711dba5e6b68",
-                "sha256:1807054aa7b61ad8d8103b3b30c9764de2e9d0c0978e9d3fc337e4e74bf25faa",
-                "sha256:1f83e9c21cd5275991076b2ba1cd35418af3504667affb4745b48937e214bafe",
-                "sha256:21b1106bff6ece8cb203ef45b4f5778d7226c941c83aaaa1e1f0f4f32cc148cd",
-                "sha256:22626dca56fd7f55a0733e604f1027277eb0f4f3d95ff28f15d27ac25a45f71b",
-                "sha256:23f96134a3aa24cc50614920cc087e22f87439053d886e474638c68c8d15dc80",
-                "sha256:2498762814dd7dd2a1d0248eda2afbc3dd9c11537bc8200a4b21789b6df6cd38",
-                "sha256:28c659878f684365d53cf59dc9a1929ea2eecd7ac65da762be8b1ba193f7e84f",
-                "sha256:2eca15d6b947cfff51ed76b2d60fd172c6ecd418ddab1c5126032d27f74bc350",
-                "sha256:354d9fc6b1e44750e2a67b4b108841f5f5ea08853453ecbf44c81fdc2e0d50bd",
-                "sha256:36a76a7527df8583112b24adc01748cd51a2d14e905b337a6fefa8b96fc708fb",
-                "sha256:3a0a4ca02752ced5f37498827e49c414d694ad7cf451ee850e3ff160f2bee9d3",
-                "sha256:3a71dbd792cc7a3d772ef8cd08d3048593f13d6f40a11f3427c000cf0a5b36a0",
-                "sha256:3a88254881e8a8c4784ecc9cb2249ff757fd94b911d5df9a5984961b96113fff",
-                "sha256:47045ed35481e857918ae78b54891fac0c1d197f22c95778e66302668309336c",
-                "sha256:4775a574e9d84e0212f5b18886cace049a42e13e12009bb0491562a48bb2b758",
-                "sha256:493da1f8b1bb8a623c16552fb4a1e164c0200447eb83d3f68b44315ead3f9036",
-                "sha256:4b847029e2d5e11fd536c9ac3136ddc3f54bc9488a75ef7d040a3900406a91eb",
-                "sha256:59d7d92cee84a547d91267f0fea381c363121d70fe90b12cd88241bd9b0e1763",
-                "sha256:5a0898a640559dec00f3614ffb11d97a2666ee9a2a6bad1259c9facd01a1d4d9",
-                "sha256:5a9a1889cc01ed2ed5f34574c90745fab1dd06ec2eee663e8ebeefe363e8efd7",
-                "sha256:5b835b86bd5a1bdbe257d610eecab07bf685b1af2a7563093e0e69180c1d4af1",
-                "sha256:5f24ca7953f2643d59a9c87d6e272d8adddd4a53bb62b9208f36db408d7aafc7",
-                "sha256:61e1a064906ccba038aa3c4a5a82f6199749efbbb3cef0804ae5c37f550eded0",
-                "sha256:65bf3eb34721bf18b5a021a1ad7aa05947a1767d1aa272b725728014475ea7d5",
-                "sha256:6807bcee549a8cb2f38f73f469703a1d8d5d990815c3004f21ddb68a567385ce",
-                "sha256:68aeefac31c1f73949662ba8affaf9950b9938b712fb9d428fa2a07e40ee57f8",
-                "sha256:6915682f9a9bc4cf2908e83caf5895a685da1fbd20b6d485dafb8e218a338279",
-                "sha256:6d9810d4f697d58fd66039ab959e6d37e63ab377008ef1d63904df25956c7db0",
-                "sha256:729d5e96566f44fccac6c4447ec2332636b4fe273f03da128fff8d5559782b06",
-                "sha256:748df39ed634851350efa87690c2237a678ed794fe9ede3f0d79f071ee042561",
-                "sha256:763a73ab377390e2af26042f685a26787c402390f682443727b847e9496e4a2a",
-                "sha256:8323a43bd9c91f62bb7d4be74cc9ff10090e7ef820e27bfe8815c57e68261311",
-                "sha256:8529b07b49b2d89d6917cfa157d3ea1dfb4d319d51e23030664a827fe5fd2131",
-                "sha256:87fa943e8bbe40c8c1ba4086971a6fefbf75e9991217c55ed1bcb2f1985bd3d4",
-                "sha256:88236b90dda77f0394f878324cfbae05ae6fde8a84d548cfe73a75278d760291",
-                "sha256:891c353e95bb11abb548ca95c8b98050f3620a7378332eb90d6acdef35b401d4",
-                "sha256:89ba3d548ee1e6291a20f3c7380c92f71e358ce8b9e48161401e087e0bc740f8",
-                "sha256:8c6be72eac3c14baa473620e04f74186c5d8f45d80f8f2b4eda6e1d18af808e8",
-                "sha256:9a242871b3d8eecc56d350e5e03ea1854de47b17f040446da0e47dc3e0b9ad4d",
-                "sha256:9a3ff5fb015f6feb78340143584d9f8a0b91b6293d6b5cf4295b3e95d179b88c",
-                "sha256:9a5a544861b21e0e7575b6023adebe7a8c6321127bb1d238eb40d99803a0e8bd",
-                "sha256:9d57677238a0c5411c76097b8b93bdebb02eb845814c90f0b01727527a179e4d",
-                "sha256:9d8c68c4145041b4eeae96239802cfdfd9ef927754a5be3f50505f09f309d8c6",
-                "sha256:9d9fcd06c952efa4b6b95f3d788a819b7f33d11bea377be6b8980c95e7d10775",
-                "sha256:a0057b5435a65b933cbf5d859cd4956624df37b8bf0917c71756e4b3d9958b9e",
-                "sha256:a65bffd24409454b889af33b6c49d0d9bcd1a219b972fba975ac935f17bdf627",
-                "sha256:b0ed6ad6c9640671689c2dbe6244680fe8b897c08fd1fab2228429b66c518e5e",
-                "sha256:b21650fa6907e523869e0396c5bd591cc326e5c1dd594dcdccac089561cacfb8",
-                "sha256:b3f7e671fb19734c872566e57ce7fc235fa953d7c181bb4ef138e17d607dc8a1",
-                "sha256:b77159d9862374da213f741af0c361720200ab7ad21b9f12556e0eb95912cd48",
-                "sha256:bb36fbb48b22985d13a6b496ea5fb9bb2a076fea943831643836c9f6febbcfdc",
-                "sha256:d066ffc5ed0be00cd0352c95800a519cf9e4b5dd34a028d301bdc7177c72daf3",
-                "sha256:d332eecf307fca852d02b63f35a7872de32d5ba8b4ec32da82f45df986b39ff6",
-                "sha256:d808a5a5411982a09fef6b49aac62986274ab050e9d3e9817ad65b2791ed1425",
-                "sha256:d9bdfa74d369256e4218000a629978590fd7cb6cf6893251dad13d051090436d",
-                "sha256:db6a0ddc1282ceb9032e41853e659c9b638789be38e5b8ad7498caac00231c23",
-                "sha256:debaf04f813ada978d7d16c7dfa16f3c9c2ec9adf4656efdc4defdf841fc2f0c",
-                "sha256:f0408e2dbad9e82b4c960274214af533f856a199c9274bd4aff55d4634dedc33",
-                "sha256:f2f3bc7cd9c9fcd39143f11342eb5963317bd54ecc98e3650ca22704b69d9653"
+                "sha256:02fce1852f755f44f95af51f69d22e45080102e9d00258053b79367d07af39c0",
+                "sha256:077ff0d1f9d9e4ce6476c1a924a3332452c1406e59d90a2cf24aeb29eeac9420",
+                "sha256:078e2a1a86544e644a68422f881c48b84fef6d18f8c7a957ffd3f2e0a74a0d4a",
+                "sha256:0970ddb69bba00670e58955f8019bec4a42d1785db3faa043c33d81de2bf843c",
+                "sha256:1286eb30261894e4c70d124d44b7fd07825340869945c79d05bda53a40caa079",
+                "sha256:21f6d9a0d5b3a207cdf7acf8e58d7d13d463e639f0c7e01d82cdb671e6cb7923",
+                "sha256:230ae493696a371f1dbffaad3dafbb742a4d27a0afd2b1aecebe52b740167e7f",
+                "sha256:26458da5653aa5b3d8dc8b24192f574a58984c749401f98fff994d41d3f08da1",
+                "sha256:2cf56d0e237280baed46f0b5316661da892565ff58309d4d2ed7dba763d984b8",
+                "sha256:2e51de54d4fb8fb50d6ee8327f9828306a959ae394d3e01a1ba8b2f937747d86",
+                "sha256:2fbfbca668dd15b744418265a9607baa970c347eefd0db6a518aaf0cfbd153c0",
+                "sha256:38adf7198f8f154502883242f9fe7333ab05a5b02de7d83aa2d88ea621f13364",
+                "sha256:3a8564f283394634a7a7054b7983e47dbf39c07712d7b177b37e03f2467a024e",
+                "sha256:3abbe948c3cbde2689370a262a8d04e32ec2dd4f27103669a45c6929bcdbfe7c",
+                "sha256:3bbe623731d03b186b3d6b0d6f51865bf598587c38d6f7b0be2e27414f7f214e",
+                "sha256:40737a081d7497efea35ab9304b829b857f21558acfc7b3272f908d33b0d9d4c",
+                "sha256:41d07d029dd4157ae27beab04d22b8e261eddfc6ecd64ff7000b10dc8b3a5727",
+                "sha256:46ed616d5fb42f98630ed70c3529541408166c22cdfd4540b88d5f21006b0eff",
+                "sha256:493d389a2b63c88ad56cdc35d0fa5752daac56ca755805b1b0c530f785767d5e",
+                "sha256:4ff0d20f2e670800d3ed2b220d40984162089a6e2c9646fdb09b85e6f9a8fc29",
+                "sha256:54accd4b8bc202966bafafd16e69da9d5640ff92389d33d28555c5fd4f25ccb7",
+                "sha256:56374914b132c702aa9aa9959c550004b8847148f95e1b824772d453ac204a72",
+                "sha256:578383d740457fa790fdf85e6d346fda1416a40549fe8db08e5e9bd281c6a475",
+                "sha256:58d7a75d731e8c63614222bcb21dd992b4ab01a399f1f09dd82af17bbfc2368a",
+                "sha256:5c5aa28df055697d7c37d2099a7bc09f559d5053c3349b1ad0c39000e611d317",
+                "sha256:5fc8e02f5984a55d2c653f5fea93531e9836abbd84342c1d1e17abc4a15084c2",
+                "sha256:63424c681923b9f3bfbc5e3205aafe790904053d42ddcc08542181a30a7a51bd",
+                "sha256:64b1df0f83706b4ef4cfb4fb0e4c2669100fd7ecacfb59e091fad300d4e04640",
+                "sha256:74934ebd71950e3db69960a7da29204f89624dde411afbfb3b4858c1409b1e98",
+                "sha256:75669d77bb2c071333417617a235324a1618dba66f82a750362eccbe5b61d248",
+                "sha256:75760a47c06b5974aa5e01949bf7e66d2af4d08cb8c1d6516af5e39595397f5e",
+                "sha256:76407ab327158c510f44ded207e2f76b657303e17cb7a572ffe2f5a8a48aa04d",
+                "sha256:76e9c727a874b4856d11a32fb0b389afc61ce8aaf281ada613713ddeadd1cfec",
+                "sha256:77d4c1b881076c3ba173484dfa53d3582c1c8ff1f914c6461ab70c8428b796c1",
+                "sha256:780c82a41dc493b62fc5884fb1d3a3b81106642c5c5c78d6a0d4cbe96d62ba7e",
+                "sha256:7dc0713bf81287a00516ef43137273b23ee414fe41a3c14be10dd95ed98a2df9",
+                "sha256:7eebcdbe3677e58dd4c0e03b4f2cfa346ed4049687d839adad68cc38bb559c92",
+                "sha256:896689fddba4f23ef7c718279e42f8834041a21342d95e56922e1c10c0cc7afb",
+                "sha256:96177eb5645b1c6985f5c11d03fc2dbda9ad24ec0f3a46dcce91445747e15094",
+                "sha256:96e25c8603a155559231c19c0349245eeb4ac0096fe3c1d0be5c47e075bd4f46",
+                "sha256:9d37ac69edc5614b90516807de32d08cb8e7b12260a285ee330955604ed9dd29",
+                "sha256:9ed6aa0726b9b60911f4aed8ec5b8dd7bf3491476015819f56473ffaef8959bd",
+                "sha256:a487f72a25904e2b4bbc0817ce7a8de94363bd7e79890510174da9d901c38705",
+                "sha256:a4cbb9ff5795cd66f0066bdf5947f170f5d63a9274f99bdbca02fd973adcf2a8",
+                "sha256:a74d56552ddbde46c246b5b89199cb3fd182f9c346c784e1a93e4dc3f5ec9975",
+                "sha256:a89ce3fd220ff144bd9d54da333ec0de0399b52c9ac3d2ce34b569cf1a5748fb",
+                "sha256:abd52a09d03adf9c763d706df707c343293d5d106aea53483e0ec8d9e310ad5e",
+                "sha256:abd8f36c99512755b8456047b7be10372fca271bf1467a1caa88db991e7c421b",
+                "sha256:af5bd9ccb188f6a5fdda9f1f09d9f4c86cc8a539bd48a0bfdc97723970348418",
+                "sha256:b02f21c1e2074943312d03d243ac4388319f2456576b2c6023041c4d57cd7019",
+                "sha256:b06fa97478a5f478fb05e1980980a7cdf2712015493b44d0c87606c1513ed5b1",
+                "sha256:b0724f05c396b0a4c36a3226c31648385deb6a65d8992644c12a4963c70326ba",
+                "sha256:b130fe77361d6771ecf5a219d8e0817d61b236b7d8b37cc045172e574ed219e6",
+                "sha256:b56d5519e470d3f2fe4aa7585f0632b060d532d0696c5bdfb5e8319e1d0f69a2",
+                "sha256:b67b819628e3b748fd3c2192c15fb951f549d0f47c0449af0764d7647302fda3",
+                "sha256:ba1711cda2d30634a7e452fc79eabcadaffedf241ff206db2ee93dd2c89a60e7",
+                "sha256:bbeccb1aa40ab88cd29e6c7d8585582c99548f55f9b2581dfc5ba68c59a85752",
+                "sha256:bd84395aab8e4d36263cd1b9308cd504f6cf713b7d6d3ce25ea55670baec5416",
+                "sha256:c99f4309f5145b93eca6e35ac1a988f0dc0a7ccf9ccdcd78d3c0adf57224e62f",
+                "sha256:ca1cccf838cd28d5a0883b342474c630ac48cac5df0ee6eacc9c7290f76b11c1",
+                "sha256:cd525e0e52a5ff16653a3fc9e3dd827981917d34996600bbc34c05d048ca35cc",
+                "sha256:cdb4f085756c96a3af04e6eca7f08b1345e94b53af8921b25c72f096e704e145",
+                "sha256:ce42618f67741d4697684e501ef02f29e758a123aa2d669e2d964ff734ee00ee",
+                "sha256:d06730c6aed78cee4126234cf2d071e01b44b915e725a6cb439a879ec9754a3a",
+                "sha256:d5fe3e099cf07d0fb5a1e23d399e5d4d1ca3e6dfcbe5c8570ccff3e9208274f7",
+                "sha256:d6bcbfc99f55655c3d93feb7ef3800bd5bbe963a755687cbf1f490a71fb7794b",
+                "sha256:d787272ed958a05b2c86311d3a4135d3c2aeea4fc655705f074130aa57d71653",
+                "sha256:e169e957c33576f47e21864cf3fc9ff47c223a4ebca8960079b8bd36cb014fd0",
+                "sha256:e20076a211cd6f9b44a6be58f7eeafa7ab5720eb796975d0c03f05b47d89eb90",
+                "sha256:e826aadda3cae59295b95343db8f3d965fb31059da7de01ee8d1c40a60398b29",
+                "sha256:eef4d64c650f33347c1f9266fa5ae001440b232ad9b98f1f43dfe7a79435c0a6",
+                "sha256:f2e69b3ed24544b0d3dbe2c5c0ba5153ce50dcebb576fdc4696d52aa22db6034",
+                "sha256:f87ec75864c37c4c6cb908d282e1969e79763e0d9becdfe9fe5473b7bb1e5f09",
+                "sha256:fbec11614dba0424ca72f4e8ba3c420dba07b4a7c206c8c8e4e73f2e98f4c559",
+                "sha256:fd69666217b62fa5d7c6aa88e507493a34dec4fa20c5bd925e4bc12fce586639"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
-            "version": "==1.14.0"
+            "markers": "python_version < '3.11'",
+            "version": "==1.15.0"
         },
         "zipp": {
             "hashes": [
-                "sha256:9f50f446828eb9d45b267433fd3e9da8d801f614129124863f9c51ebceafb87d",
-                "sha256:b47250dd24f92b7dd6a0a8fc5244da14608f3ca90a5efcd37a3b1642fac9a375"
+                "sha256:112929ad649da941c23de50f356a2b5570c954b65150642bccdd66bf194d224b",
+                "sha256:48904fc76a60e542af151aded95726c1a5c34ed43ab4134b597665c86d7ad556"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.7.0"
+            "version": "==3.15.0"
         }
     }
 }
```

### Comparing `gitwrapperlib-1.0.0/gitwrapperlib/README.rst` & `gitwrapperlib-1.0.1/gitwrapperlib/README.rst`

 * *Files identical despite different names*

### Comparing `gitwrapperlib-1.0.0/gitwrapperlib/USAGE.rst` & `gitwrapperlib-1.0.1/gitwrapperlib/USAGE.rst`

 * *Files identical despite different names*

### Comparing `gitwrapperlib-1.0.0/gitwrapperlib/__init__.py` & `gitwrapperlib-1.0.1/gitwrapperlib/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 """
 gitwrapperlib package.
 
 Import all parts from gitwrapperlib here
 
 .. _Google Python Style Guide:
-   http://google.github.io/styleguide/pyguide.html
+   https://google.github.io/styleguide/pyguide.html
 """
 from ._version import __version__
 from .gitwrapperlibexceptions import ExecutableNotFound
 from .gitwrapperlib import Git
 
 __author__ = '''Costas Tyfoxylos <costas.tyf@gmail.com>'''
 __docformat__ = '''google'''
```

### Comparing `gitwrapperlib-1.0.0/gitwrapperlib/_version.py` & `gitwrapperlib-1.0.1/gitwrapperlib/_version.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 #  DEALINGS IN THE SOFTWARE.
 #
 
 """
 Manages the version of the package.
 
 .. _Google Python Style Guide:
-   http://google.github.io/styleguide/pyguide.html
+   https://google.github.io/styleguide/pyguide.html
 
 """
 
 import os
 
 __author__ = '''Costas Tyfoxylos <costas.tyf@gmail.com>'''
 __docformat__ = '''google'''
@@ -54,12 +54,15 @@
     os.path.join(
         os.path.dirname(__file__),
         '.VERSION'
     )
 )
 
 try:
-    with open(VERSION_FILE_PATH) as f:
+    with open(VERSION_FILE_PATH, encoding='utf8') as f:
         __version__ = f.read()
 except IOError:
-    with open(LOCAL_VERSION_FILE_PATH) as f:
-        __version__ = f.read()
+    try:
+        with open(LOCAL_VERSION_FILE_PATH, encoding='utf8') as f:
+            __version__ = f.read()
+    except IOError:
+        __version__ = 'unknown'
```

### Comparing `gitwrapperlib-1.0.0/gitwrapperlib/gitwrapperlib.py` & `gitwrapperlib-1.0.1/gitwrapperlib/gitwrapperlib.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,28 +23,28 @@
 #  DEALINGS IN THE SOFTWARE.
 #
 
 """
 Main code for gitwrapperlib.
 
 .. _Google Python Style Guide:
-   http://google.github.io/styleguide/pyguide.html
+   https://google.github.io/styleguide/pyguide.html
 
 """
 
 import logging
 import sys
 import re
 try:
     import sh
 except ImportError:
     # fallback: emulate the sh API with pbs
     import pbs
 
-    class Sh:  # pylint: disable=too-few-public-methods
+    class Sh:
         """
         Overloading pbs to look like sh.
 
         https://stackoverflow.com/questions/28618906/porting-sh-1-11-based-code-to-windows
         """
 
         def __getattr__(self, attr):
@@ -74,35 +74,33 @@
 class Git:
     """Models the git command and constructs some extra helper methods."""
 
     passthrough_methods = ('init', 'pull')
     argument_methods = ('add', 'clone', 'push')
 
     def __init__(self, tty_out=True):
-        logger_name = u'{base}.{suffix}'.format(base=LOGGER_BASENAME,
-                                                suffix=self.__class__.__name__)
+        logger_name = f'{LOGGER_BASENAME}.{self.__class__.__name__}'
         self._logger = logging.getLogger(logger_name)
         self._git = self._get_command()
-        if not tty_out:
-            self._git = self._git.bake(_tty_out=False)
+        self._git = self._git.bake(_tty_out=tty_out)
 
     @staticmethod
     def _get_command():
         if sys.platform in ('win32', 'cygwin'):
             try:
                 sh.git()
             except WindowsError:  # pylint: disable=undefined-variable
-                raise ExecutableNotFound
+                raise ExecutableNotFound from None
             except pbs.ErrorReturnCode_1:
                 git = sh.git
         else:
             try:
                 git = sh.Command('git')
             except sh.CommandNotFound:
-                raise ExecutableNotFound
+                raise ExecutableNotFound from None
         return git
 
     def __getattr__(self, name):  # pylint: disable=inconsistent-return-statements
         if name in self.passthrough_methods:
             return getattr(self._git, name)
         if name in self.argument_methods:
             def wrapper(*args, **kwargs):  # noqa
@@ -166,15 +164,15 @@
     def get_default_branch(self):
         """Returns the remote default branch."""
         show_origin_text = str(self._git.remote('show', 'origin'))
         try:
             branch = re.search(r'HEAD branch: (\S+)', show_origin_text).group(1)
         except (IndexError, AttributeError):
             raise RemoteOriginError(f'git remote show origin command did not respond as expected, '
-                                    f'received :{show_origin_text}')
+                                    f'received :{show_origin_text}') from None
         if branch == '(unknown)':
             message = 'Failed to detect default remote branch, please check your remote settings.'
             self._logger.error(message)
             raise BranchNotFound(message)
         return branch
 
     def create_branch(self, name):
@@ -187,20 +185,20 @@
 
     def switch_branch(self, name):
         """Switches to a branch."""
         self._git.checkout(name)
 
     def list_tags(self):
         """Lists existing tags."""
-        return self._git.tag()
+        return self._git.tag().splitlines()
 
     def add_tag(self, value):
         """Tag with provided value."""
         self._git.tag(value)
 
     def delete_tag(self, value):
         """Delete the tag provided."""
         self._git.tag('-d', value)
 
     def create_patch(self, from_tag, to_tag):
         """Create a patch between tags."""
-        return str(self._git.diff('{}..{}'.format(from_tag, to_tag), _tty_out=False))
+        return str(self._git.diff(f'{from_tag}..{to_tag}', _tty_out=False))
```

### Comparing `gitwrapperlib-1.0.0/gitwrapperlib/gitwrapperlibexceptions.py` & `gitwrapperlib-1.0.1/gitwrapperlib/gitwrapperlibexceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 #  DEALINGS IN THE SOFTWARE.
 #
 
 """
 Custom exception code for gitwrapperlib.
 
 .. _Google Python Style Guide:
-   http://google.github.io/styleguide/pyguide.html
+   https://google.github.io/styleguide/pyguide.html
 
 """
 
 __author__ = '''Costas Tyfoxylos <costas.tyf@gmail.com>'''
 __docformat__ = '''google'''
 __date__ = '''02-01-2018'''
 __copyright__ = '''Copyright 2018, Costas Tyfoxylos'''
```

### Comparing `gitwrapperlib-1.0.0/gitwrapperlib.egg-info/PKG-INFO` & `gitwrapperlib-1.0.1/gitwrapperlib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: gitwrapperlib
-Version: 1.0.0
+Version: 1.0.1
 Summary: A lightweight wrapper around the git command using sh module.
 Home-page: https://github.com/costastf/gitwrapperlib
 Author: Costas Tyfoxylos
 Author-email: costas.tyf@gmail.com
 License: MIT
 Keywords: gitwrapperlib git python sh
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 License-File: LICENSE
 License-File: AUTHORS.rst
@@ -135,7 +134,11 @@
 
 1.0.0 (21-03-2022)
 ------------------
 
 * Removed references to master branch and implemented default remote retrieval, courtesy of Sten Spans <sspans@schubergphilis.com>
 
 
+1.0.1 (13-06-2023)
+------------------
+
+* Bump dependencies and update pipeline to python 3.9.
```

### Comparing `gitwrapperlib-1.0.0/setup.py` & `gitwrapperlib-1.0.1/setup.py`

 * *Files identical despite different names*

