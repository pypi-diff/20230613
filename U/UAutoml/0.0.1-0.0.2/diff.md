# Comparing `tmp/UAutoml-0.0.1.tar.gz` & `tmp/UAutoml-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UAutoml-0.0.1.tar", last modified: Tue Jun 13 16:34:02 2023, max compression
+gzip compressed data, was "UAutoml-0.0.2.tar", last modified: Tue Jun 13 16:38:14 2023, max compression
```

## Comparing `UAutoml-0.0.1.tar` & `UAutoml-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 ujjwalreddyks   (501) staff       (20)        0 2023-06-13 16:34:02.460224 UAutoml-0.0.1/
--rw-r--r--   0 ujjwalreddyks   (501) staff       (20)     1073 2023-06-13 15:50:26.000000 UAutoml-0.0.1/LICENSE.txt
--rw-r--r--   0 ujjwalreddyks   (501) staff       (20)      556 2023-06-13 16:34:02.458955 UAutoml-0.0.1/PKG-INFO
--rw-r--r--   0 ujjwalreddyks   (501) staff       (20)     1582 2023-06-13 15:57:56.000000 UAutoml-0.0.1/README.md
--rw-r--r--   0 ujjwalreddyks   (501) staff       (20)       38 2023-06-13 16:34:02.460600 UAutoml-0.0.1/setup.cfg
--rw-r--r--   0 ujjwalreddyks   (501) staff       (20)      841 2023-06-13 16:30:23.000000 UAutoml-0.0.1/setup.py
-drwxr-xr-x   0 ujjwalreddyks   (501) staff       (20)        0 2023-06-13 16:34:02.454553 UAutoml-0.0.1/src/
-drwxr-xr-x   0 ujjwalreddyks   (501) staff       (20)        0 2023-06-13 16:34:02.457778 UAutoml-0.0.1/src/UAutoml.egg-info/
--rw-r--r--   0 ujjwalreddyks   (501) staff       (20)      556 2023-06-13 16:34:02.000000 UAutoml-0.0.1/src/UAutoml.egg-info/PKG-INFO
--rw-r--r--   0 ujjwalreddyks   (501) staff       (20)      219 2023-06-13 16:34:02.000000 UAutoml-0.0.1/src/UAutoml.egg-info/SOURCES.txt
--rw-r--r--   0 ujjwalreddyks   (501) staff       (20)        1 2023-06-13 16:34:02.000000 UAutoml-0.0.1/src/UAutoml.egg-info/dependency_links.txt
--rw-r--r--   0 ujjwalreddyks   (501) staff       (20)       19 2023-06-13 16:34:02.000000 UAutoml-0.0.1/src/UAutoml.egg-info/requires.txt
--rw-r--r--   0 ujjwalreddyks   (501) staff       (20)        8 2023-06-13 16:34:02.000000 UAutoml-0.0.1/src/UAutoml.egg-info/top_level.txt
--rw-r--r--   0 ujjwalreddyks   (501) staff       (20)    12183 2023-06-13 15:32:30.000000 UAutoml-0.0.1/src/UAutoml.py
+drwxr-xr-x   0 ujjwalreddyks   (501) staff       (20)        0 2023-06-13 16:38:14.633754 UAutoml-0.0.2/
+-rw-r--r--   0 ujjwalreddyks   (501) staff       (20)     1073 2023-06-13 15:50:26.000000 UAutoml-0.0.2/LICENSE.txt
+-rw-r--r--   0 ujjwalreddyks   (501) staff       (20)     2131 2023-06-13 16:38:14.632287 UAutoml-0.0.2/PKG-INFO
+-rw-r--r--   0 ujjwalreddyks   (501) staff       (20)     1582 2023-06-13 15:57:56.000000 UAutoml-0.0.2/README.md
+-rw-r--r--   0 ujjwalreddyks   (501) staff       (20)       38 2023-06-13 16:38:14.634193 UAutoml-0.0.2/setup.cfg
+-rw-r--r--   0 ujjwalreddyks   (501) staff       (20)      880 2023-06-13 16:37:15.000000 UAutoml-0.0.2/setup.py
+drwxr-xr-x   0 ujjwalreddyks   (501) staff       (20)        0 2023-06-13 16:38:14.627110 UAutoml-0.0.2/src/
+drwxr-xr-x   0 ujjwalreddyks   (501) staff       (20)        0 2023-06-13 16:38:14.630947 UAutoml-0.0.2/src/UAutoml.egg-info/
+-rw-r--r--   0 ujjwalreddyks   (501) staff       (20)     2131 2023-06-13 16:38:14.000000 UAutoml-0.0.2/src/UAutoml.egg-info/PKG-INFO
+-rw-r--r--   0 ujjwalreddyks   (501) staff       (20)      219 2023-06-13 16:38:14.000000 UAutoml-0.0.2/src/UAutoml.egg-info/SOURCES.txt
+-rw-r--r--   0 ujjwalreddyks   (501) staff       (20)        1 2023-06-13 16:38:14.000000 UAutoml-0.0.2/src/UAutoml.egg-info/dependency_links.txt
+-rw-r--r--   0 ujjwalreddyks   (501) staff       (20)       19 2023-06-13 16:38:14.000000 UAutoml-0.0.2/src/UAutoml.egg-info/requires.txt
+-rw-r--r--   0 ujjwalreddyks   (501) staff       (20)        8 2023-06-13 16:38:14.000000 UAutoml-0.0.2/src/UAutoml.egg-info/top_level.txt
+-rw-r--r--   0 ujjwalreddyks   (501) staff       (20)    12183 2023-06-13 15:32:30.000000 UAutoml-0.0.2/src/UAutoml.py
```

### Comparing `UAutoml-0.0.1/LICENSE.txt` & `UAutoml-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `UAutoml-0.0.1/README.md` & `UAutoml-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `UAutoml-0.0.1/setup.py` & `UAutoml-0.0.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,18 +2,19 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='UAutoml',
-    version='0.0.1',
+    version='0.0.2',
     description='Automated Machine Learning Framework for Data Analysisr',
     author= 'Ujjwal Reddy K S',
     url = 'https://github.com/ujjwalredd/Automated-Machine-Learning-Framework-for-Data-Analysis',
+    long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     keywords=['ML', 'Auto Data Analysis', 'models'],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

### Comparing `UAutoml-0.0.1/src/UAutoml.py` & `UAutoml-0.0.2/src/UAutoml.py`

 * *Files identical despite different names*

