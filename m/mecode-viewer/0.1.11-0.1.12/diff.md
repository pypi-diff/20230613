# Comparing `tmp/mecode_viewer-0.1.11.tar.gz` & `tmp/mecode_viewer-0.1.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mecode_viewer-0.1.11.tar", last modified: Tue Jun 13 00:32:48 2023, max compression
+gzip compressed data, was "mecode_viewer-0.1.12.tar", last modified: Tue Jun 13 00:33:26 2023, max compression
```

## Comparing `mecode_viewer-0.1.11.tar` & `mecode_viewer-0.1.12.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 rtelles    (502) staff       (20)        0 2023-06-13 00:32:48.599220 mecode_viewer-0.1.11/
--rw-r--r--   0 rtelles    (502) staff       (20)     3602 2022-11-21 22:26:04.000000 mecode_viewer-0.1.11/CONTRIBUTING.rst
--rw-r--r--   0 rtelles    (502) staff       (20)       89 2022-11-21 22:26:04.000000 mecode_viewer-0.1.11/HISTORY.rst
--rw-r--r--   0 rtelles    (502) staff       (20)     1073 2022-11-21 22:26:04.000000 mecode_viewer-0.1.11/LICENSE
--rw-r--r--   0 rtelles    (502) staff       (20)      242 2022-11-21 22:26:04.000000 mecode_viewer-0.1.11/MANIFEST.in
--rw-r--r--   0 rtelles    (502) staff       (20)     2062 2023-06-13 00:32:48.599354 mecode_viewer-0.1.11/PKG-INFO
--rw-r--r--   0 rtelles    (502) staff       (20)     1261 2023-06-13 00:32:44.000000 mecode_viewer-0.1.11/README.rst
-drwxr-xr-x   0 rtelles    (502) staff       (20)        0 2023-06-13 00:32:48.590963 mecode_viewer-0.1.11/docs/
--rw-r--r--   0 rtelles    (502) staff       (20)      614 2022-11-21 22:26:04.000000 mecode_viewer-0.1.11/docs/Makefile
--rwxr-xr-x   0 rtelles    (502) staff       (20)     4862 2022-11-21 22:26:04.000000 mecode_viewer-0.1.11/docs/conf.py
--rw-r--r--   0 rtelles    (502) staff       (20)       33 2022-11-21 22:26:04.000000 mecode_viewer-0.1.11/docs/contributing.rst
--rw-r--r--   0 rtelles    (502) staff       (20)       28 2022-11-21 22:26:04.000000 mecode_viewer-0.1.11/docs/history.rst
--rw-r--r--   0 rtelles    (502) staff       (20)      299 2022-11-21 22:26:04.000000 mecode_viewer-0.1.11/docs/index.rst
--rw-r--r--   0 rtelles    (502) staff       (20)     1170 2022-11-21 22:26:04.000000 mecode_viewer-0.1.11/docs/installation.rst
--rw-r--r--   0 rtelles    (502) staff       (20)      811 2022-11-21 22:26:04.000000 mecode_viewer-0.1.11/docs/make.bat
--rw-r--r--   0 rtelles    (502) staff       (20)       27 2022-11-21 22:26:04.000000 mecode_viewer-0.1.11/docs/readme.rst
--rw-r--r--   0 rtelles    (502) staff       (20)       81 2022-11-21 22:26:04.000000 mecode_viewer-0.1.11/docs/usage.rst
-drwxr-xr-x   0 rtelles    (502) staff       (20)        0 2023-06-13 00:32:48.592857 mecode_viewer-0.1.11/mecode_viewer/
--rw-r--r--   0 rtelles    (502) staff       (20)      165 2023-05-31 15:53:14.000000 mecode_viewer-0.1.11/mecode_viewer/__init__.py
--rw-r--r--   0 rtelles    (502) staff       (20)      454 2022-11-21 22:26:04.000000 mecode_viewer-0.1.11/mecode_viewer/cli.py
--rw-r--r--   0 rtelles    (502) staff       (20)    19757 2023-06-12 18:56:27.000000 mecode_viewer-0.1.11/mecode_viewer/mecode_viewer.py
-drwxr-xr-x   0 rtelles    (502) staff       (20)        0 2023-06-13 00:32:48.597794 mecode_viewer-0.1.11/mecode_viewer.egg-info/
--rw-r--r--   0 rtelles    (502) staff       (20)     2062 2023-06-13 00:32:48.000000 mecode_viewer-0.1.11/mecode_viewer.egg-info/PKG-INFO
--rw-r--r--   0 rtelles    (502) staff       (20)      610 2023-06-13 00:32:48.000000 mecode_viewer-0.1.11/mecode_viewer.egg-info/SOURCES.txt
--rw-r--r--   0 rtelles    (502) staff       (20)        1 2023-06-13 00:32:48.000000 mecode_viewer-0.1.11/mecode_viewer.egg-info/dependency_links.txt
--rw-r--r--   0 rtelles    (502) staff       (20)       57 2023-06-13 00:32:48.000000 mecode_viewer-0.1.11/mecode_viewer.egg-info/entry_points.txt
--rw-r--r--   0 rtelles    (502) staff       (20)        1 2023-06-12 21:06:47.000000 mecode_viewer-0.1.11/mecode_viewer.egg-info/not-zip-safe
--rw-r--r--   0 rtelles    (502) staff       (20)       39 2023-06-13 00:32:48.000000 mecode_viewer-0.1.11/mecode_viewer.egg-info/requires.txt
--rw-r--r--   0 rtelles    (502) staff       (20)       14 2023-06-13 00:32:48.000000 mecode_viewer-0.1.11/mecode_viewer.egg-info/top_level.txt
--rw-r--r--   0 rtelles    (502) staff       (20)      385 2023-06-13 00:32:48.600198 mecode_viewer-0.1.11/setup.cfg
--rw-r--r--   0 rtelles    (502) staff       (20)     1483 2023-06-13 00:25:49.000000 mecode_viewer-0.1.11/setup.py
-drwxr-xr-x   0 rtelles    (502) staff       (20)        0 2023-06-13 00:32:48.598862 mecode_viewer-0.1.11/tests/
--rw-r--r--   0 rtelles    (502) staff       (20)       43 2022-11-21 22:26:04.000000 mecode_viewer-0.1.11/tests/__init__.py
--rw-r--r--   0 rtelles    (502) staff       (20)      417 2022-11-21 22:26:04.000000 mecode_viewer-0.1.11/tests/test_mecode_viewer.py
+drwxr-xr-x   0 rtelles    (502) staff       (20)        0 2023-06-13 00:33:26.809385 mecode_viewer-0.1.12/
+-rw-r--r--   0 rtelles    (502) staff       (20)     3602 2022-11-21 22:26:04.000000 mecode_viewer-0.1.12/CONTRIBUTING.rst
+-rw-r--r--   0 rtelles    (502) staff       (20)       89 2022-11-21 22:26:04.000000 mecode_viewer-0.1.12/HISTORY.rst
+-rw-r--r--   0 rtelles    (502) staff       (20)     1073 2022-11-21 22:26:04.000000 mecode_viewer-0.1.12/LICENSE
+-rw-r--r--   0 rtelles    (502) staff       (20)      242 2022-11-21 22:26:04.000000 mecode_viewer-0.1.12/MANIFEST.in
+-rw-r--r--   0 rtelles    (502) staff       (20)     2062 2023-06-13 00:33:26.809498 mecode_viewer-0.1.12/PKG-INFO
+-rw-r--r--   0 rtelles    (502) staff       (20)     1261 2023-06-13 00:32:44.000000 mecode_viewer-0.1.12/README.rst
+drwxr-xr-x   0 rtelles    (502) staff       (20)        0 2023-06-13 00:33:26.801345 mecode_viewer-0.1.12/docs/
+-rw-r--r--   0 rtelles    (502) staff       (20)      614 2022-11-21 22:26:04.000000 mecode_viewer-0.1.12/docs/Makefile
+-rwxr-xr-x   0 rtelles    (502) staff       (20)     4862 2022-11-21 22:26:04.000000 mecode_viewer-0.1.12/docs/conf.py
+-rw-r--r--   0 rtelles    (502) staff       (20)       33 2022-11-21 22:26:04.000000 mecode_viewer-0.1.12/docs/contributing.rst
+-rw-r--r--   0 rtelles    (502) staff       (20)       28 2022-11-21 22:26:04.000000 mecode_viewer-0.1.12/docs/history.rst
+-rw-r--r--   0 rtelles    (502) staff       (20)      299 2022-11-21 22:26:04.000000 mecode_viewer-0.1.12/docs/index.rst
+-rw-r--r--   0 rtelles    (502) staff       (20)     1170 2022-11-21 22:26:04.000000 mecode_viewer-0.1.12/docs/installation.rst
+-rw-r--r--   0 rtelles    (502) staff       (20)      811 2022-11-21 22:26:04.000000 mecode_viewer-0.1.12/docs/make.bat
+-rw-r--r--   0 rtelles    (502) staff       (20)       27 2022-11-21 22:26:04.000000 mecode_viewer-0.1.12/docs/readme.rst
+-rw-r--r--   0 rtelles    (502) staff       (20)       81 2022-11-21 22:26:04.000000 mecode_viewer-0.1.12/docs/usage.rst
+drwxr-xr-x   0 rtelles    (502) staff       (20)        0 2023-06-13 00:33:26.803203 mecode_viewer-0.1.12/mecode_viewer/
+-rw-r--r--   0 rtelles    (502) staff       (20)      165 2023-05-31 15:53:14.000000 mecode_viewer-0.1.12/mecode_viewer/__init__.py
+-rw-r--r--   0 rtelles    (502) staff       (20)      454 2022-11-21 22:26:04.000000 mecode_viewer-0.1.12/mecode_viewer/cli.py
+-rw-r--r--   0 rtelles    (502) staff       (20)    19757 2023-06-12 18:56:27.000000 mecode_viewer-0.1.12/mecode_viewer/mecode_viewer.py
+drwxr-xr-x   0 rtelles    (502) staff       (20)        0 2023-06-13 00:33:26.808283 mecode_viewer-0.1.12/mecode_viewer.egg-info/
+-rw-r--r--   0 rtelles    (502) staff       (20)     2062 2023-06-13 00:33:26.000000 mecode_viewer-0.1.12/mecode_viewer.egg-info/PKG-INFO
+-rw-r--r--   0 rtelles    (502) staff       (20)      610 2023-06-13 00:33:26.000000 mecode_viewer-0.1.12/mecode_viewer.egg-info/SOURCES.txt
+-rw-r--r--   0 rtelles    (502) staff       (20)        1 2023-06-13 00:33:26.000000 mecode_viewer-0.1.12/mecode_viewer.egg-info/dependency_links.txt
+-rw-r--r--   0 rtelles    (502) staff       (20)       57 2023-06-13 00:33:26.000000 mecode_viewer-0.1.12/mecode_viewer.egg-info/entry_points.txt
+-rw-r--r--   0 rtelles    (502) staff       (20)        1 2023-06-12 21:06:47.000000 mecode_viewer-0.1.12/mecode_viewer.egg-info/not-zip-safe
+-rw-r--r--   0 rtelles    (502) staff       (20)       39 2023-06-13 00:33:26.000000 mecode_viewer-0.1.12/mecode_viewer.egg-info/requires.txt
+-rw-r--r--   0 rtelles    (502) staff       (20)       14 2023-06-13 00:33:26.000000 mecode_viewer-0.1.12/mecode_viewer.egg-info/top_level.txt
+-rw-r--r--   0 rtelles    (502) staff       (20)      385 2023-06-13 00:33:26.810095 mecode_viewer-0.1.12/setup.cfg
+-rw-r--r--   0 rtelles    (502) staff       (20)     1483 2023-06-13 00:33:08.000000 mecode_viewer-0.1.12/setup.py
+drwxr-xr-x   0 rtelles    (502) staff       (20)        0 2023-06-13 00:33:26.809033 mecode_viewer-0.1.12/tests/
+-rw-r--r--   0 rtelles    (502) staff       (20)       43 2022-11-21 22:26:04.000000 mecode_viewer-0.1.12/tests/__init__.py
+-rw-r--r--   0 rtelles    (502) staff       (20)      417 2022-11-21 22:26:04.000000 mecode_viewer-0.1.12/tests/test_mecode_viewer.py
```

### Comparing `mecode_viewer-0.1.11/CONTRIBUTING.rst` & `mecode_viewer-0.1.12/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `mecode_viewer-0.1.11/LICENSE` & `mecode_viewer-0.1.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mecode_viewer-0.1.11/PKG-INFO` & `mecode_viewer-0.1.12/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mecode_viewer
-Version: 0.1.11
+Version: 0.1.12
 Summary: Simple GCode Viewer
 Home-page: https://github.com/rtellez700/mecode_viewer
 Author: Rodrigo Telles
 Author-email: rtelles@g.harvard.edu
 License: MIT license
 Keywords: mecode_viewer
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `mecode_viewer-0.1.11/README.rst` & `mecode_viewer-0.1.12/README.rst`

 * *Files identical despite different names*

### Comparing `mecode_viewer-0.1.11/docs/Makefile` & `mecode_viewer-0.1.12/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mecode_viewer-0.1.11/docs/conf.py` & `mecode_viewer-0.1.12/docs/conf.py`

 * *Files identical despite different names*

### Comparing `mecode_viewer-0.1.11/docs/installation.rst` & `mecode_viewer-0.1.12/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `mecode_viewer-0.1.11/docs/make.bat` & `mecode_viewer-0.1.12/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mecode_viewer-0.1.11/mecode_viewer/mecode_viewer.py` & `mecode_viewer-0.1.12/mecode_viewer/mecode_viewer.py`

 * *Files identical despite different names*

### Comparing `mecode_viewer-0.1.11/mecode_viewer.egg-info/PKG-INFO` & `mecode_viewer-0.1.12/mecode_viewer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mecode-viewer
-Version: 0.1.11
+Version: 0.1.12
 Summary: Simple GCode Viewer
 Home-page: https://github.com/rtellez700/mecode_viewer
 Author: Rodrigo Telles
 Author-email: rtelles@g.harvard.edu
 License: MIT license
 Keywords: mecode_viewer
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `mecode_viewer-0.1.11/mecode_viewer.egg-info/SOURCES.txt` & `mecode_viewer-0.1.12/mecode_viewer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mecode_viewer-0.1.11/setup.py` & `mecode_viewer-0.1.12/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,10 +43,10 @@
     include_package_data=True,
     keywords='mecode_viewer',
     name='mecode_viewer',
     packages=find_packages(include=['mecode_viewer', 'mecode_viewer.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/rtellez700/mecode_viewer',
-    version='0.1.11',
+    version='0.1.12',
     zip_safe=False,
 )
```

