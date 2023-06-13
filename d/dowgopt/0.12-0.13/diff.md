# Comparing `tmp/dowgopt-0.12.tar.gz` & `tmp/dowgopt-0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dowgopt-0.12.tar", last modified: Mon Jun 12 18:15:24 2023, max compression
+gzip compressed data, was "dowgopt-0.13.tar", last modified: Tue Jun 13 15:23:07 2023, max compression
```

## Comparing `dowgopt-0.12.tar` & `dowgopt-0.13.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 akhaled97 (1713700788) akhaled97 (1713700788)        0 2023-06-12 18:15:24.912774 dowgopt-0.12/
--rw-rw-r--   0 akhaled97 (1713700788) akhaled97 (1713700788)      768 2023-06-12 18:15:24.911120 dowgopt-0.12/PKG-INFO
--rw-rw-r--   0 akhaled97 (1713700788) akhaled97 (1713700788)      145 2023-06-12 18:10:14.000000 dowgopt-0.12/README.md
-drwxrwxr-x   0 akhaled97 (1713700788) akhaled97 (1713700788)        0 2023-06-12 18:15:24.886464 dowgopt-0.12/dowg/
--rw-rw-r--   0 akhaled97 (1713700788) akhaled97 (1713700788)       30 2023-06-12 18:10:14.000000 dowgopt-0.12/dowg/__init__.py
--rw-rw-r--   0 akhaled97 (1713700788) akhaled97 (1713700788)     3863 2023-06-12 18:10:14.000000 dowgopt-0.12/dowg/dowg.py
-drwxrwxr-x   0 akhaled97 (1713700788) akhaled97 (1713700788)        0 2023-06-12 18:15:24.905669 dowgopt-0.12/dowgopt.egg-info/
--rw-rw-r--   0 akhaled97 (1713700788) akhaled97 (1713700788)      768 2023-06-12 18:15:24.000000 dowgopt-0.12/dowgopt.egg-info/PKG-INFO
--rw-rw-r--   0 akhaled97 (1713700788) akhaled97 (1713700788)      202 2023-06-12 18:15:24.000000 dowgopt-0.12/dowgopt.egg-info/SOURCES.txt
--rw-rw-r--   0 akhaled97 (1713700788) akhaled97 (1713700788)        1 2023-06-12 18:15:24.000000 dowgopt-0.12/dowgopt.egg-info/dependency_links.txt
--rw-rw-r--   0 akhaled97 (1713700788) akhaled97 (1713700788)        6 2023-06-12 18:15:24.000000 dowgopt-0.12/dowgopt.egg-info/requires.txt
--rw-rw-r--   0 akhaled97 (1713700788) akhaled97 (1713700788)        5 2023-06-12 18:15:24.000000 dowgopt-0.12/dowgopt.egg-info/top_level.txt
--rw-rw-r--   0 akhaled97 (1713700788) akhaled97 (1713700788)       38 2023-06-12 18:15:24.913775 dowgopt-0.12/setup.cfg
--rw-rw-r--   0 akhaled97 (1713700788) akhaled97 (1713700788)      840 2023-06-12 18:15:05.000000 dowgopt-0.12/setup.py
+drwxrwxr-x   0 akhaled97 (1713700788) akhaled97 (1713700788)        0 2023-06-13 15:23:07.507180 dowgopt-0.13/
+-rw-rw-r--   0 akhaled97 (1713700788) akhaled97 (1713700788)      768 2023-06-13 15:23:07.505404 dowgopt-0.13/PKG-INFO
+-rw-rw-r--   0 akhaled97 (1713700788) akhaled97 (1713700788)      145 2023-06-12 18:10:14.000000 dowgopt-0.13/README.md
+drwxrwxr-x   0 akhaled97 (1713700788) akhaled97 (1713700788)        0 2023-06-13 15:23:07.481138 dowgopt-0.13/dowg/
+-rw-rw-r--   0 akhaled97 (1713700788) akhaled97 (1713700788)       30 2023-06-12 18:10:14.000000 dowgopt-0.13/dowg/__init__.py
+-rw-rw-r--   0 akhaled97 (1713700788) akhaled97 (1713700788)     3843 2023-06-13 15:22:31.000000 dowgopt-0.13/dowg/dowg.py
+drwxrwxr-x   0 akhaled97 (1713700788) akhaled97 (1713700788)        0 2023-06-13 15:23:07.500695 dowgopt-0.13/dowgopt.egg-info/
+-rw-rw-r--   0 akhaled97 (1713700788) akhaled97 (1713700788)      768 2023-06-13 15:23:07.000000 dowgopt-0.13/dowgopt.egg-info/PKG-INFO
+-rw-rw-r--   0 akhaled97 (1713700788) akhaled97 (1713700788)      202 2023-06-13 15:23:07.000000 dowgopt-0.13/dowgopt.egg-info/SOURCES.txt
+-rw-rw-r--   0 akhaled97 (1713700788) akhaled97 (1713700788)        1 2023-06-13 15:23:07.000000 dowgopt-0.13/dowgopt.egg-info/dependency_links.txt
+-rw-rw-r--   0 akhaled97 (1713700788) akhaled97 (1713700788)        6 2023-06-13 15:23:07.000000 dowgopt-0.13/dowgopt.egg-info/requires.txt
+-rw-rw-r--   0 akhaled97 (1713700788) akhaled97 (1713700788)        5 2023-06-13 15:23:07.000000 dowgopt-0.13/dowgopt.egg-info/top_level.txt
+-rw-rw-r--   0 akhaled97 (1713700788) akhaled97 (1713700788)       38 2023-06-13 15:23:07.508088 dowgopt-0.13/setup.cfg
+-rw-rw-r--   0 akhaled97 (1713700788) akhaled97 (1713700788)      840 2023-06-13 15:23:00.000000 dowgopt-0.13/setup.py
```

### Comparing `dowgopt-0.12/PKG-INFO` & `dowgopt-0.13/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dowgopt
-Version: 0.12
+Version: 0.13
 Summary: DoWG parameter-free optimizer for PyTorch
 Home-page: https://github.com/rka97/dowg
 Author: Ahmed Khaled
 Author-email: akregeb@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dowgopt-0.12/dowg/dowg.py` & `dowgopt-0.13/dowg/dowg.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         params (iterable): iterable of parameters to optimize or dicts defining
             parameter groups
         eps (float, optional): term added to the denominator to improve
             numerical stability (default: 1e-8)
     """
 
     def __init__(self, params, eps=1e-8):
-        defaults = dict(lr=lr, betas=betas, eps=eps)
+        defaults = dict(eps=eps)
         super(CDoWG, self).__init__(params, defaults)
 
     def step(self, closure=None):
         """Performs a single optimization step.
 
         Args:
             closure (callable, optional): A closure that reevaluates the model
```

### Comparing `dowgopt-0.12/dowgopt.egg-info/PKG-INFO` & `dowgopt-0.13/dowgopt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dowgopt
-Version: 0.12
+Version: 0.13
 Summary: DoWG parameter-free optimizer for PyTorch
 Home-page: https://github.com/rka97/dowg
 Author: Ahmed Khaled
 Author-email: akregeb@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dowgopt-0.12/setup.py` & `dowgopt-0.13/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="dowgopt",
-    version="0.12",
+    version="0.13",
     packages=find_packages(),
     install_requires=[
         "torch",
     ],
     author="Ahmed Khaled",
     author_email="akregeb@gmail.com",
     description="DoWG parameter-free optimizer for PyTorch",
```

