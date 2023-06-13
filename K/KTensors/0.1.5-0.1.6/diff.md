# Comparing `tmp/KTensors-0.1.5.tar.gz` & `tmp/KTensors-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KTensors-0.1.5.tar", last modified: Mon Jun 12 04:06:31 2023, max compression
+gzip compressed data, was "KTensors-0.1.6.tar", last modified: Tue Jun 13 00:47:44 2023, max compression
```

## Comparing `KTensors-0.1.5.tar` & `KTensors-0.1.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 hanchaozhang   (501) staff       (20)        0 2023-06-12 04:06:31.489947 KTensors-0.1.5/
-drwxr-xr-x   0 hanchaozhang   (501) staff       (20)        0 2023-06-12 04:06:31.489599 KTensors-0.1.5/KTensors.egg-info/
--rw-r--r--   0 hanchaozhang   (501) staff       (20)     2907 2023-06-12 04:06:31.000000 KTensors-0.1.5/KTensors.egg-info/PKG-INFO
--rw-r--r--   0 hanchaozhang   (501) staff       (20)      189 2023-06-12 04:06:31.000000 KTensors-0.1.5/KTensors.egg-info/SOURCES.txt
--rw-r--r--   0 hanchaozhang   (501) staff       (20)        1 2023-06-12 04:06:31.000000 KTensors-0.1.5/KTensors.egg-info/dependency_links.txt
--rw-r--r--   0 hanchaozhang   (501) staff       (20)        6 2023-06-12 04:06:31.000000 KTensors-0.1.5/KTensors.egg-info/requires.txt
--rw-r--r--   0 hanchaozhang   (501) staff       (20)        9 2023-06-12 04:06:31.000000 KTensors-0.1.5/KTensors.egg-info/top_level.txt
--rw-r--r--   0 hanchaozhang   (501) staff       (20)     2751 2023-06-12 00:12:19.000000 KTensors-0.1.5/KTensors.py
--rw-r--r--   0 hanchaozhang   (501) staff       (20)     2907 2023-06-12 04:06:31.489805 KTensors-0.1.5/PKG-INFO
--rw-r--r--   0 hanchaozhang   (501) staff       (20)     2598 2023-06-12 04:05:32.000000 KTensors-0.1.5/README.md
--rw-r--r--   0 hanchaozhang   (501) staff       (20)       38 2023-06-12 04:06:31.489991 KTensors-0.1.5/setup.cfg
--rw-r--r--   0 hanchaozhang   (501) staff       (20)     1225 2023-06-12 04:05:44.000000 KTensors-0.1.5/setup.py
+drwxr-xr-x   0 hanchaozhang   (501) staff       (20)        0 2023-06-13 00:47:44.412678 KTensors-0.1.6/
+drwxr-xr-x   0 hanchaozhang   (501) staff       (20)        0 2023-06-13 00:47:44.412337 KTensors-0.1.6/KTensors.egg-info/
+-rw-r--r--   0 hanchaozhang   (501) staff       (20)     2923 2023-06-13 00:47:44.000000 KTensors-0.1.6/KTensors.egg-info/PKG-INFO
+-rw-r--r--   0 hanchaozhang   (501) staff       (20)      189 2023-06-13 00:47:44.000000 KTensors-0.1.6/KTensors.egg-info/SOURCES.txt
+-rw-r--r--   0 hanchaozhang   (501) staff       (20)        1 2023-06-13 00:47:44.000000 KTensors-0.1.6/KTensors.egg-info/dependency_links.txt
+-rw-r--r--   0 hanchaozhang   (501) staff       (20)       12 2023-06-13 00:47:44.000000 KTensors-0.1.6/KTensors.egg-info/requires.txt
+-rw-r--r--   0 hanchaozhang   (501) staff       (20)        9 2023-06-13 00:47:44.000000 KTensors-0.1.6/KTensors.egg-info/top_level.txt
+-rw-r--r--   0 hanchaozhang   (501) staff       (20)     5584 2023-06-13 00:46:13.000000 KTensors-0.1.6/KTensors.py
+-rw-r--r--   0 hanchaozhang   (501) staff       (20)     2923 2023-06-13 00:47:44.412543 KTensors-0.1.6/PKG-INFO
+-rw-r--r--   0 hanchaozhang   (501) staff       (20)     2598 2023-06-13 00:46:50.000000 KTensors-0.1.6/README.md
+-rw-r--r--   0 hanchaozhang   (501) staff       (20)       38 2023-06-13 00:47:44.412721 KTensors-0.1.6/setup.cfg
+-rw-r--r--   0 hanchaozhang   (501) staff       (20)     1214 2023-06-13 00:46:48.000000 KTensors-0.1.6/setup.py
```

### Comparing `KTensors-0.1.5/KTensors.egg-info/PKG-INFO` & `KTensors-0.1.6/KTensors.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: KTensors
-Version: 0.1.5
+Version: 0.1.6
 Summary: K-Tensors
 Home-page: https://github.com/Hanchao-Zhang/KTensors
 Author: Hanchao Zhang
 Author-email: hz1641@nyu.edu
 License: MIT
 Keywords: KTensors: Clustering Positive Semi-Denfinite Matrices
 Requires: numpy
+Requires: scipy
 Description-Content-Type: text/markdown
 
 K-Tensors: Clustering Positive Semi-Definite Matrices<img src="./ktensorlogo.png" align="right" width="150" />
 ========================================================================================================================
 
 
 [![Project Status:
```

### Comparing `KTensors-0.1.5/PKG-INFO` & `KTensors-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: KTensors
-Version: 0.1.5
+Version: 0.1.6
 Summary: K-Tensors
 Home-page: https://github.com/Hanchao-Zhang/KTensors
 Author: Hanchao Zhang
 Author-email: hz1641@nyu.edu
 License: MIT
 Keywords: KTensors: Clustering Positive Semi-Denfinite Matrices
 Requires: numpy
+Requires: scipy
 Description-Content-Type: text/markdown
 
 K-Tensors: Clustering Positive Semi-Definite Matrices<img src="./ktensorlogo.png" align="right" width="150" />
 ========================================================================================================================
 
 
 [![Project Status:
```

### Comparing `KTensors-0.1.5/README.md` & `KTensors-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `KTensors-0.1.5/setup.py` & `KTensors-0.1.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 import os
 from setuptools import find_packages, setup
 
 # read the contents of your README file
 from pathlib import Path
+
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
+
 # Utility function to read the README file.
 # Used for the long_description.  It's nice, because now 1) we have a top level
 # README file and 2) it's easier to type in the README file than to put a raw
 # string in below ...
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
+
 setup(
-    name = "KTensors",
+    name="KTensors",
     description="K-Tensors",
     long_description=long_description,
-    long_description_content_type='text/markdown',
-    version = "0.1.5",
-    author = "Hanchao Zhang",
-    author_email = "hz1641@nyu.edu",
-    license = "MIT",
-    keywords = "KTensors: Clustering Positive Semi-Denfinite Matrices",
-    url = "https://github.com/Hanchao-Zhang/KTensors",
+    long_description_content_type="text/markdown",
+    version="0.1.6",
+    author="Hanchao Zhang",
+    author_email="hz1641@nyu.edu",
+    license="MIT",
+    keywords="KTensors: Clustering Positive Semi-Denfinite Matrices",
+    url="https://github.com/Hanchao-Zhang/KTensors",
     packages=find_packages("KTensors"),
     py_modules=["KTensors"],
-    requires=['numpy'],
-    install_requires=[
-        'numpy',
-    ],
+    requires=["numpy", "scipy"],
+    install_requires=["numpy", "scipy"],
     # classifiers=[
     #     "Development Status :: 3 - Alpha",
     #     "Topic :: Utilities",
     #     "License :: OSI Approved :: BSD License",
-    # ],    
-)
+    # ],
+)
```

