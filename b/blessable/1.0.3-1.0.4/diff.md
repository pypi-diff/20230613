# Comparing `tmp/blessable-1.0.3.tar.gz` & `tmp/blessable-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blessable-1.0.3.tar", last modified: Mon Jun 12 02:52:03 2023, max compression
+gzip compressed data, was "blessable-1.0.4.tar", last modified: Mon Jun 12 02:54:26 2023, max compression
```

## Comparing `blessable-1.0.3.tar` & `blessable-1.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 benjaminlee   (501) staff       (20)        0 2023-06-12 02:52:03.567955 blessable-1.0.3/
--rw-r--r--   0 benjaminlee   (501) staff       (20)     1802 2023-06-12 02:52:03.567814 blessable-1.0.3/PKG-INFO
--rw-r--r--   0 benjaminlee   (501) staff       (20)     1429 2023-06-12 01:37:31.000000 blessable-1.0.3/README.md
-drwxr-xr-x   0 benjaminlee   (501) staff       (20)        0 2023-06-12 02:52:03.566533 blessable-1.0.3/blessable/
--rw-r--r--   0 benjaminlee   (501) staff       (20)       33 2023-06-12 01:36:24.000000 blessable-1.0.3/blessable/__init__.py
--rw-r--r--   0 benjaminlee   (501) staff       (20)      624 2023-06-12 01:36:31.000000 blessable-1.0.3/blessable/blessable.py
--rw-r--r--   0 benjaminlee   (501) staff       (20)    15184 2023-06-12 00:48:54.000000 blessable-1.0.3/blessable/colormap.py
-drwxr-xr-x   0 benjaminlee   (501) staff       (20)        0 2023-06-12 02:52:03.567614 blessable-1.0.3/blessable.egg-info/
--rw-r--r--   0 benjaminlee   (501) staff       (20)     1802 2023-06-12 02:52:03.000000 blessable-1.0.3/blessable.egg-info/PKG-INFO
--rw-r--r--   0 benjaminlee   (501) staff       (20)      249 2023-06-12 02:52:03.000000 blessable-1.0.3/blessable.egg-info/SOURCES.txt
--rw-r--r--   0 benjaminlee   (501) staff       (20)        1 2023-06-12 02:52:03.000000 blessable-1.0.3/blessable.egg-info/dependency_links.txt
--rw-r--r--   0 benjaminlee   (501) staff       (20)        8 2023-06-12 02:52:03.000000 blessable-1.0.3/blessable.egg-info/requires.txt
--rw-r--r--   0 benjaminlee   (501) staff       (20)       10 2023-06-12 02:52:03.000000 blessable-1.0.3/blessable.egg-info/top_level.txt
--rw-r--r--   0 benjaminlee   (501) staff       (20)       38 2023-06-12 02:52:03.568009 blessable-1.0.3/setup.cfg
--rw-r--r--   0 benjaminlee   (501) staff       (20)      603 2023-06-12 02:50:12.000000 blessable-1.0.3/setup.py
+drwxr-xr-x   0 benjaminlee   (501) staff       (20)        0 2023-06-12 02:54:26.262496 blessable-1.0.4/
+-rw-r--r--   0 benjaminlee   (501) staff       (20)     1905 2023-06-12 02:54:26.262356 blessable-1.0.4/PKG-INFO
+-rw-r--r--   0 benjaminlee   (501) staff       (20)     1533 2023-06-12 02:54:11.000000 blessable-1.0.4/README.md
+drwxr-xr-x   0 benjaminlee   (501) staff       (20)        0 2023-06-12 02:54:26.261413 blessable-1.0.4/blessable/
+-rw-r--r--   0 benjaminlee   (501) staff       (20)       33 2023-06-12 01:36:24.000000 blessable-1.0.4/blessable/__init__.py
+-rw-r--r--   0 benjaminlee   (501) staff       (20)      624 2023-06-12 01:36:31.000000 blessable-1.0.4/blessable/blessable.py
+-rw-r--r--   0 benjaminlee   (501) staff       (20)    15184 2023-06-12 00:48:54.000000 blessable-1.0.4/blessable/colormap.py
+drwxr-xr-x   0 benjaminlee   (501) staff       (20)        0 2023-06-12 02:54:26.262158 blessable-1.0.4/blessable.egg-info/
+-rw-r--r--   0 benjaminlee   (501) staff       (20)     1905 2023-06-12 02:54:26.000000 blessable-1.0.4/blessable.egg-info/PKG-INFO
+-rw-r--r--   0 benjaminlee   (501) staff       (20)      249 2023-06-12 02:54:26.000000 blessable-1.0.4/blessable.egg-info/SOURCES.txt
+-rw-r--r--   0 benjaminlee   (501) staff       (20)        1 2023-06-12 02:54:26.000000 blessable-1.0.4/blessable.egg-info/dependency_links.txt
+-rw-r--r--   0 benjaminlee   (501) staff       (20)        8 2023-06-12 02:54:26.000000 blessable-1.0.4/blessable.egg-info/requires.txt
+-rw-r--r--   0 benjaminlee   (501) staff       (20)       10 2023-06-12 02:54:26.000000 blessable-1.0.4/blessable.egg-info/top_level.txt
+-rw-r--r--   0 benjaminlee   (501) staff       (20)       38 2023-06-12 02:54:26.262545 blessable-1.0.4/setup.cfg
+-rw-r--r--   0 benjaminlee   (501) staff       (20)      603 2023-06-12 02:54:23.000000 blessable-1.0.4/setup.py
```

### Comparing `blessable-1.0.3/PKG-INFO` & `blessable-1.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blessable
-Version: 1.0.3
+Version: 1.0.4
 Summary: "Blessable" - a simple markup language for Blessings.
 Home-page: https://github.com/fakerybakery/blessable
 Author: www.mrfake.name
 Project-URL: Bug Reports, https://github.com/fakerybakery/blessable/issues
 Project-URL: Source, https://github.com/fakerybakery/blessable
 Description-Content-Type: text/markdown
 
@@ -21,15 +21,21 @@
  - Linux
  - BSD
 
 Please refer to the Blessed documentation for more information.
 
 ## Usage
 
-First, import the `blessable` module:
+First, install the packages:
+
+```python
+pip install blessable # or python -m pip install blessable
+```
+
+Then, import the `blessable` module:
 
 ```python
 from blessable import Blessable
 ```
 
 Then, use `blessable` like this:
```

### Comparing `blessable-1.0.3/README.md` & `blessable-1.0.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,21 @@
  - Linux
  - BSD
 
 Please refer to the Blessed documentation for more information.
 
 ## Usage
 
-First, import the `blessable` module:
+First, install the packages:
+
+```python
+pip install blessable # or python -m pip install blessable
+```
+
+Then, import the `blessable` module:
 
 ```python
 from blessable import Blessable
 ```
 
 Then, use `blessable` like this:
 
@@ -69,8 +75,8 @@
 
  - `bold` (alias `b`)
  - `italic` (alias `i`)
  - `underline` (alias `u`)
 
 ## To Do
 
- - [ ] Support nested styling
+ - [ ] Support nested styling
```

### Comparing `blessable-1.0.3/blessable/blessable.py` & `blessable-1.0.4/blessable/blessable.py`

 * *Files identical despite different names*

### Comparing `blessable-1.0.3/blessable/colormap.py` & `blessable-1.0.4/blessable/colormap.py`

 * *Files identical despite different names*

### Comparing `blessable-1.0.3/blessable.egg-info/PKG-INFO` & `blessable-1.0.4/blessable.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blessable
-Version: 1.0.3
+Version: 1.0.4
 Summary: "Blessable" - a simple markup language for Blessings.
 Home-page: https://github.com/fakerybakery/blessable
 Author: www.mrfake.name
 Project-URL: Bug Reports, https://github.com/fakerybakery/blessable/issues
 Project-URL: Source, https://github.com/fakerybakery/blessable
 Description-Content-Type: text/markdown
 
@@ -21,15 +21,21 @@
  - Linux
  - BSD
 
 Please refer to the Blessed documentation for more information.
 
 ## Usage
 
-First, import the `blessable` module:
+First, install the packages:
+
+```python
+pip install blessable # or python -m pip install blessable
+```
+
+Then, import the `blessable` module:
 
 ```python
 from blessable import Blessable
 ```
 
 Then, use `blessable` like this:
```

### Comparing `blessable-1.0.3/setup.py` & `blessable-1.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 with open('README.md', 'r') as f:
     longdesc = f.read()
 setup(
     name='blessable',
-    version='1.0.3',
+    version='1.0.4',
     author='www.mrfake.name',
     description='"Blessable" - a simple markup language for Blessings.',
     long_description=longdesc,
     long_description_content_type='text/markdown',
     url='https://github.com/fakerybakery/blessable',
     packages=['blessable'],
     install_requires=['blessed'],
```

