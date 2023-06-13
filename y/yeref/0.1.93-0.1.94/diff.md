# Comparing `tmp/yeref-0.1.93.tar.gz` & `tmp/yeref-0.1.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yeref-0.1.93.tar", last modified: Tue Jun 13 14:31:00 2023, max compression
+gzip compressed data, was "yeref-0.1.94.tar", last modified: Tue Jun 13 14:33:47 2023, max compression
```

## Comparing `yeref-0.1.93.tar` & `yeref-0.1.94.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-13 14:31:00.090739 yeref-0.1.93/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-06-13 14:31:00.090892 yeref-0.1.93/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)       38 2023-06-13 14:31:00.091555 yeref-0.1.93/setup.cfg
--rw-r--r--   0 mark       (501) staff       (20)     1391 2023-06-13 14:30:44.000000 yeref-0.1.93/setup.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-13 14:31:00.085403 yeref-0.1.93/yeref/
--rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.93/yeref/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)   551418 2023-06-13 11:23:32.000000 yeref-0.1.93/yeref/l_.py
--rw-r--r--   0 mark       (501) staff       (20)   210914 2023-06-13 13:35:20.000000 yeref-0.1.93/yeref/yeref.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-13 14:31:00.090309 yeref-0.1.93/yeref.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-06-13 14:31:00.000000 yeref-0.1.93/yeref.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      179 2023-06-13 14:31:00.000000 yeref-0.1.93/yeref.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-06-13 14:31:00.000000 yeref-0.1.93/yeref.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)        6 2023-06-13 14:31:00.000000 yeref-0.1.93/yeref.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-13 14:33:47.861246 yeref-0.1.94/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-06-13 14:33:47.861478 yeref-0.1.94/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)       38 2023-06-13 14:33:47.862107 yeref-0.1.94/setup.cfg
+-rw-r--r--   0 mark       (501) staff       (20)     1391 2023-06-13 14:33:33.000000 yeref-0.1.94/setup.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-13 14:33:47.853704 yeref-0.1.94/yeref/
+-rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.94/yeref/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)   551418 2023-06-13 11:23:32.000000 yeref-0.1.94/yeref/l_.py
+-rw-r--r--   0 mark       (501) staff       (20)   210914 2023-06-13 13:35:20.000000 yeref-0.1.94/yeref/yeref.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-13 14:33:47.860356 yeref-0.1.94/yeref.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-06-13 14:33:47.000000 yeref-0.1.94/yeref.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)      179 2023-06-13 14:33:47.000000 yeref-0.1.94/yeref.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-06-13 14:33:47.000000 yeref-0.1.94/yeref.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)        6 2023-06-13 14:33:47.000000 yeref-0.1.94/yeref.egg-info/top_level.txt
```

### Comparing `yeref-0.1.93/setup.py` & `yeref-0.1.94/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
       name='yeref',
-      version='0.1.93',
+      version='0.1.94',
       description='desc-f',
       author='john smith',
       packages=['yeref'],
       # install_requires=[
       #       "httplib2>=0.20.4",
       #       "moviepy>=1.0.3",
       #       "Pillow>=9.2.0",
```

### Comparing `yeref-0.1.93/yeref/l_.py` & `yeref-0.1.94/yeref/l_.py`

 * *Files identical despite different names*

### Comparing `yeref-0.1.93/yeref/yeref.py` & `yeref-0.1.94/yeref/yeref.py`

 * *Files identical despite different names*

