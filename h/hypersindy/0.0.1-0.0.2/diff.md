# Comparing `tmp/hypersindy-0.0.1.tar.gz` & `tmp/hypersindy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypersindy-0.0.1.tar", last modified: Mon Jun 12 20:54:22 2023, max compression
+gzip compressed data, was "hypersindy-0.0.2.tar", last modified: Tue Jun 13 16:47:21 2023, max compression
```

## Comparing `hypersindy-0.0.1.tar` & `hypersindy-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 mozesj    (1010) mozesj    (1010)        0 2023-06-12 20:54:22.808141 hypersindy-0.0.1/
--rw-rw-r--   0 mozesj    (1010) mozesj    (1010)     1068 2023-06-12 20:53:55.000000 hypersindy-0.0.1/LICENSE.txt
--rw-rw-r--   0 mozesj    (1010) mozesj    (1010)        0 2023-06-09 18:26:29.000000 hypersindy-0.0.1/MANIFEST.in
--rw-rw-r--   0 mozesj    (1010) mozesj    (1010)     3534 2023-06-12 20:54:22.808141 hypersindy-0.0.1/PKG-INFO
--rw-rw-r--   0 mozesj    (1010) mozesj    (1010)     2993 2023-06-12 20:51:46.000000 hypersindy-0.0.1/README.md
--rw-rw-r--   0 mozesj    (1010) mozesj    (1010)      609 2023-06-12 20:05:04.000000 hypersindy-0.0.1/pyproject.toml
--rw-rw-r--   0 mozesj    (1010) mozesj    (1010)       38 2023-06-12 20:54:22.808141 hypersindy-0.0.1/setup.cfg
-drwxrwxr-x   0 mozesj    (1010) mozesj    (1010)        0 2023-06-12 20:54:22.808141 hypersindy-0.0.1/src/
-drwxrwxr-x   0 mozesj    (1010) mozesj    (1010)        0 2023-06-12 20:54:22.808141 hypersindy-0.0.1/src/hypersindy/
--rw-rw-r--   0 mozesj    (1010) mozesj    (1010)        0 2023-06-09 18:27:12.000000 hypersindy-0.0.1/src/hypersindy/__init__.py
--rw-rw-r--   0 mozesj    (1010) mozesj    (1010)     4292 2023-06-12 20:42:53.000000 hypersindy-0.0.1/src/hypersindy/dataset.py
--rw-rw-r--   0 mozesj    (1010) mozesj    (1010)     3368 2023-06-12 20:32:23.000000 hypersindy-0.0.1/src/hypersindy/equations.py
--rw-rw-r--   0 mozesj    (1010) mozesj    (1010)     3264 2023-06-12 19:00:33.000000 hypersindy-0.0.1/src/hypersindy/hypernet.py
--rw-rw-r--   0 mozesj    (1010) mozesj    (1010)     4861 2023-06-12 20:34:58.000000 hypersindy-0.0.1/src/hypersindy/l0.py
--rw-rw-r--   0 mozesj    (1010) mozesj    (1010)     7617 2023-06-12 20:46:16.000000 hypersindy-0.0.1/src/hypersindy/library.py
--rw-rw-r--   0 mozesj    (1010) mozesj    (1010)    13556 2023-06-12 20:42:52.000000 hypersindy-0.0.1/src/hypersindy/net.py
--rw-rw-r--   0 mozesj    (1010) mozesj    (1010)    16980 2023-06-12 20:34:55.000000 hypersindy-0.0.1/src/hypersindy/trainer.py
--rw-rw-r--   0 mozesj    (1010) mozesj    (1010)     5619 2023-06-12 19:00:37.000000 hypersindy-0.0.1/src/hypersindy/utils.py
-drwxrwxr-x   0 mozesj    (1010) mozesj    (1010)        0 2023-06-12 20:54:22.808141 hypersindy-0.0.1/src/hypersindy.egg-info/
--rw-rw-r--   0 mozesj    (1010) mozesj    (1010)     3534 2023-06-12 20:54:22.000000 hypersindy-0.0.1/src/hypersindy.egg-info/PKG-INFO
--rw-rw-r--   0 mozesj    (1010) mozesj    (1010)      427 2023-06-12 20:54:22.000000 hypersindy-0.0.1/src/hypersindy.egg-info/SOURCES.txt
--rw-rw-r--   0 mozesj    (1010) mozesj    (1010)        1 2023-06-12 20:54:22.000000 hypersindy-0.0.1/src/hypersindy.egg-info/dependency_links.txt
--rw-rw-r--   0 mozesj    (1010) mozesj    (1010)       11 2023-06-12 20:54:22.000000 hypersindy-0.0.1/src/hypersindy.egg-info/top_level.txt
+drwxrwxr-x   0 mozesj    (1010) mozesj    (1010)        0 2023-06-13 16:47:21.745823 hypersindy-0.0.2/
+-rw-rw-r--   0 mozesj    (1010) mozesj    (1010)     1068 2023-06-12 20:53:55.000000 hypersindy-0.0.2/LICENSE.txt
+-rw-rw-r--   0 mozesj    (1010) mozesj    (1010)        0 2023-06-09 18:26:29.000000 hypersindy-0.0.2/MANIFEST.in
+-rw-rw-r--   0 mozesj    (1010) mozesj    (1010)     1997 2023-06-13 16:47:21.745823 hypersindy-0.0.2/PKG-INFO
+-rw-rw-r--   0 mozesj    (1010) mozesj    (1010)     1456 2023-06-13 16:46:14.000000 hypersindy-0.0.2/README.md
+-rw-rw-r--   0 mozesj    (1010) mozesj    (1010)      609 2023-06-12 21:40:20.000000 hypersindy-0.0.2/pyproject.toml
+-rw-rw-r--   0 mozesj    (1010) mozesj    (1010)       38 2023-06-13 16:47:21.745823 hypersindy-0.0.2/setup.cfg
+drwxrwxr-x   0 mozesj    (1010) mozesj    (1010)        0 2023-06-13 16:47:21.745823 hypersindy-0.0.2/src/
+drwxrwxr-x   0 mozesj    (1010) mozesj    (1010)        0 2023-06-13 16:47:21.745823 hypersindy-0.0.2/src/hypersindy/
+-rw-rw-r--   0 mozesj    (1010) mozesj    (1010)        0 2023-06-09 18:27:12.000000 hypersindy-0.0.2/src/hypersindy/__init__.py
+-rw-rw-r--   0 mozesj    (1010) mozesj    (1010)     4290 2023-06-13 16:39:38.000000 hypersindy-0.0.2/src/hypersindy/dataset.py
+-rw-rw-r--   0 mozesj    (1010) mozesj    (1010)     3368 2023-06-12 20:32:23.000000 hypersindy-0.0.2/src/hypersindy/equations.py
+-rw-rw-r--   0 mozesj    (1010) mozesj    (1010)     3264 2023-06-12 19:00:33.000000 hypersindy-0.0.2/src/hypersindy/hypernet.py
+-rw-rw-r--   0 mozesj    (1010) mozesj    (1010)     4861 2023-06-12 20:34:58.000000 hypersindy-0.0.2/src/hypersindy/l0.py
+-rw-rw-r--   0 mozesj    (1010) mozesj    (1010)     7617 2023-06-12 20:46:16.000000 hypersindy-0.0.2/src/hypersindy/library.py
+-rw-rw-r--   0 mozesj    (1010) mozesj    (1010)    13556 2023-06-12 20:42:52.000000 hypersindy-0.0.2/src/hypersindy/net.py
+-rw-rw-r--   0 mozesj    (1010) mozesj    (1010)    16980 2023-06-12 20:34:55.000000 hypersindy-0.0.2/src/hypersindy/trainer.py
+-rw-rw-r--   0 mozesj    (1010) mozesj    (1010)     5619 2023-06-12 19:00:37.000000 hypersindy-0.0.2/src/hypersindy/utils.py
+drwxrwxr-x   0 mozesj    (1010) mozesj    (1010)        0 2023-06-13 16:47:21.745823 hypersindy-0.0.2/src/hypersindy.egg-info/
+-rw-rw-r--   0 mozesj    (1010) mozesj    (1010)     1997 2023-06-13 16:47:21.000000 hypersindy-0.0.2/src/hypersindy.egg-info/PKG-INFO
+-rw-rw-r--   0 mozesj    (1010) mozesj    (1010)      427 2023-06-13 16:47:21.000000 hypersindy-0.0.2/src/hypersindy.egg-info/SOURCES.txt
+-rw-rw-r--   0 mozesj    (1010) mozesj    (1010)        1 2023-06-13 16:47:21.000000 hypersindy-0.0.2/src/hypersindy.egg-info/dependency_links.txt
+-rw-rw-r--   0 mozesj    (1010) mozesj    (1010)       11 2023-06-13 16:47:21.000000 hypersindy-0.0.2/src/hypersindy.egg-info/top_level.txt
```

### Comparing `hypersindy-0.0.1/LICENSE.txt` & `hypersindy-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hypersindy-0.0.1/pyproject.toml` & `hypersindy-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hypersindy"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Mozes Jacobs", email="mozesjacobs15@gmail.com" },
 ]
 description = "HyperSINDy, a package to discover SDEs from time series data."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `hypersindy-0.0.1/src/hypersindy/dataset.py` & `hypersindy-0.0.2/src/hypersindy/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import torch
 from torch.utils.data import Dataset
 import numpy as np
 
-class SyntheticDataset(Dataset):
+class DynamicDataset(Dataset):
     """A dataset to run experiments with.
 
     Creates a dataset of torch tensors. Tensors must be loaded from numpy
     array files or passed in as numpy arrays.
 
 
     Attributes:
```

### Comparing `hypersindy-0.0.1/src/hypersindy/equations.py` & `hypersindy-0.0.2/src/hypersindy/equations.py`

 * *Files identical despite different names*

### Comparing `hypersindy-0.0.1/src/hypersindy/hypernet.py` & `hypersindy-0.0.2/src/hypersindy/hypernet.py`

 * *Files identical despite different names*

### Comparing `hypersindy-0.0.1/src/hypersindy/l0.py` & `hypersindy-0.0.2/src/hypersindy/l0.py`

 * *Files identical despite different names*

### Comparing `hypersindy-0.0.1/src/hypersindy/library.py` & `hypersindy-0.0.2/src/hypersindy/library.py`

 * *Files identical despite different names*

### Comparing `hypersindy-0.0.1/src/hypersindy/net.py` & `hypersindy-0.0.2/src/hypersindy/net.py`

 * *Files identical despite different names*

### Comparing `hypersindy-0.0.1/src/hypersindy/trainer.py` & `hypersindy-0.0.2/src/hypersindy/trainer.py`

 * *Files identical despite different names*

### Comparing `hypersindy-0.0.1/src/hypersindy/utils.py` & `hypersindy-0.0.2/src/hypersindy/utils.py`

 * *Files identical despite different names*

