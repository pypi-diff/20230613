# Comparing `tmp/win32mica-1.8.tar.gz` & `tmp/win32mica-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "win32mica-1.8.tar", last modified: Thu Jan 26 13:18:12 2023, max compression
+gzip compressed data, was "win32mica-1.9.tar", last modified: Tue Jun 13 11:27:16 2023, max compression
```

## Comparing `win32mica-1.8.tar` & `win32mica-1.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 13:18:12.490834 win32mica-1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-01-26 13:18:02.000000 win32mica-1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-01-26 13:18:12.490834 win32mica-1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-01-26 13:18:02.000000 win32mica-1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-01-26 13:18:02.000000 win32mica-1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-26 13:18:12.490834 win32mica-1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-01-26 13:18:02.000000 win32mica-1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 13:18:12.490834 win32mica-1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 13:18:12.490834 win32mica-1.8/src/win32mica/
--rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-01-26 13:18:02.000000 win32mica-1.8/src/win32mica/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 13:18:12.490834 win32mica-1.8/src/win32mica.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-01-26 13:18:12.000000 win32mica-1.8/src/win32mica.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-01-26 13:18:12.000000 win32mica-1.8/src/win32mica.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-26 13:18:12.000000 win32mica-1.8/src/win32mica.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-01-26 13:18:12.000000 win32mica-1.8/src/win32mica.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:27:16.360606 win32mica-1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-13 11:27:04.000000 win32mica-1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-06-13 11:27:16.360606 win32mica-1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-06-13 11:27:04.000000 win32mica-1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-13 11:27:04.000000 win32mica-1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 11:27:16.360606 win32mica-1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-13 11:27:04.000000 win32mica-1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:27:16.360606 win32mica-1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:27:16.360606 win32mica-1.9/src/win32mica/
+-rw-r--r--   0 runner    (1001) docker     (123)     6200 2023-06-13 11:27:04.000000 win32mica-1.9/src/win32mica/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:27:16.360606 win32mica-1.9/src/win32mica.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-06-13 11:27:16.000000 win32mica-1.9/src/win32mica.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-13 11:27:16.000000 win32mica-1.9/src/win32mica.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 11:27:16.000000 win32mica-1.9/src/win32mica.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-13 11:27:16.000000 win32mica-1.9/src/win32mica.egg-info/top_level.txt
```

### Comparing `win32mica-1.8/LICENSE` & `win32mica-1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `win32mica-1.8/PKG-INFO` & `win32mica-1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: win32mica
-Version: 1.8
+Version: 1.9
 Summary: Apply mica background (if supported) and immersive dark mode to Windows 11 Win32 apps made with python, such as Tkinter or PyQt/PySide apps
 Home-page: https://github.com/marticliment/win32mica
 Author: Martí Climent
 Author-email: marticlilop@gmail.com
 Project-URL: Bug Tracker, https://github.com/marticliment/win32mica/issues
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `win32mica-1.8/README.md` & `win32mica-1.9/README.md`

 * *Files identical despite different names*

### Comparing `win32mica-1.8/setup.py` & `win32mica-1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="win32mica",
-    version="1.8",
+    version="1.9",
     author="Martí Climent",
     author_email="marticlilop@gmail.com",
     description="Apply mica background (if supported) and immersive dark mode to Windows 11 Win32 apps made with python, such as Tkinter or PyQt/PySide apps",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/marticliment/win32mica",
     project_urls={
```

### Comparing `win32mica-1.8/src/win32mica.egg-info/PKG-INFO` & `win32mica-1.9/src/win32mica.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: win32mica
-Version: 1.8
+Version: 1.9
 Summary: Apply mica background (if supported) and immersive dark mode to Windows 11 Win32 apps made with python, such as Tkinter or PyQt/PySide apps
 Home-page: https://github.com/marticliment/win32mica
 Author: Martí Climent
 Author-email: marticlilop@gmail.com
 Project-URL: Bug Tracker, https://github.com/marticliment/win32mica/issues
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

