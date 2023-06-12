# Comparing `tmp/torch-base-network-0.0.1.tar.gz` & `tmp/torch-base-network-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch-base-network-0.0.1.tar", last modified: Mon Jun 12 22:30:48 2023, max compression
+gzip compressed data, was "torch-base-network-0.0.2.tar", last modified: Mon Jun 12 23:19:05 2023, max compression
```

## Comparing `torch-base-network-0.0.1.tar` & `torch-base-network-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 andrejacobs   (501) staff       (20)        0 2023-06-12 22:30:48.664531 torch-base-network-0.0.1/
--rw-r--r--   0 andrejacobs   (501) staff       (20)      480 2023-06-12 22:30:48.664414 torch-base-network-0.0.1/PKG-INFO
--rw-r--r--   0 andrejacobs   (501) staff       (20)       38 2023-06-12 22:30:48.664582 torch-base-network-0.0.1/setup.cfg
--rw-r--r--   0 andrejacobs   (501) staff       (20)      737 2023-06-12 19:36:08.000000 torch-base-network-0.0.1/setup.py
-drwxr-xr-x   0 andrejacobs   (501) staff       (20)        0 2023-06-12 22:30:48.663601 torch-base-network-0.0.1/tbn/
--rw-r--r--   0 andrejacobs   (501) staff       (20)        0 2023-06-12 19:31:56.000000 torch-base-network-0.0.1/tbn/__init__.py
--rw-r--r--   0 andrejacobs   (501) staff       (20)     1241 2023-06-12 19:33:38.000000 torch-base-network-0.0.1/tbn/network.py
-drwxr-xr-x   0 andrejacobs   (501) staff       (20)        0 2023-06-12 22:30:48.664229 torch-base-network-0.0.1/torch_base_network.egg-info/
--rw-r--r--   0 andrejacobs   (501) staff       (20)      480 2023-06-12 22:30:48.000000 torch-base-network-0.0.1/torch_base_network.egg-info/PKG-INFO
--rw-r--r--   0 andrejacobs   (501) staff       (20)      207 2023-06-12 22:30:48.000000 torch-base-network-0.0.1/torch_base_network.egg-info/SOURCES.txt
--rw-r--r--   0 andrejacobs   (501) staff       (20)        1 2023-06-12 22:30:48.000000 torch-base-network-0.0.1/torch_base_network.egg-info/dependency_links.txt
--rw-r--r--   0 andrejacobs   (501) staff       (20)        4 2023-06-12 22:30:48.000000 torch-base-network-0.0.1/torch_base_network.egg-info/top_level.txt
+drwxr-xr-x   0 andrejacobs   (501) staff       (20)        0 2023-06-12 23:19:05.163478 torch-base-network-0.0.2/
+-rw-r--r--   0 andrejacobs   (501) staff       (20)      480 2023-06-12 23:19:05.163277 torch-base-network-0.0.2/PKG-INFO
+-rw-r--r--   0 andrejacobs   (501) staff       (20)       38 2023-06-12 23:19:05.163526 torch-base-network-0.0.2/setup.cfg
+-rw-r--r--   0 andrejacobs   (501) staff       (20)      737 2023-06-12 23:17:58.000000 torch-base-network-0.0.2/setup.py
+drwxr-xr-x   0 andrejacobs   (501) staff       (20)        0 2023-06-12 23:19:05.162339 torch-base-network-0.0.2/tbn/
+-rw-r--r--   0 andrejacobs   (501) staff       (20)        0 2023-06-12 19:31:56.000000 torch-base-network-0.0.2/tbn/__init__.py
+-rw-r--r--   0 andrejacobs   (501) staff       (20)     3649 2023-06-12 23:10:45.000000 torch-base-network-0.0.2/tbn/network.py
+drwxr-xr-x   0 andrejacobs   (501) staff       (20)        0 2023-06-12 23:19:05.163057 torch-base-network-0.0.2/torch_base_network.egg-info/
+-rw-r--r--   0 andrejacobs   (501) staff       (20)      480 2023-06-12 23:19:05.000000 torch-base-network-0.0.2/torch_base_network.egg-info/PKG-INFO
+-rw-r--r--   0 andrejacobs   (501) staff       (20)      207 2023-06-12 23:19:05.000000 torch-base-network-0.0.2/torch_base_network.egg-info/SOURCES.txt
+-rw-r--r--   0 andrejacobs   (501) staff       (20)        1 2023-06-12 23:19:05.000000 torch-base-network-0.0.2/torch_base_network.egg-info/dependency_links.txt
+-rw-r--r--   0 andrejacobs   (501) staff       (20)        4 2023-06-12 23:19:05.000000 torch-base-network-0.0.2/torch_base_network.egg-info/top_level.txt
```

### Comparing `torch-base-network-0.0.1/setup.py` & `torch-base-network-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'A base class for easier development of PyTorch models'
 LONG_DESCRIPTION = 'A package that makes it easy for developers to create PyTorch models easily'
 
 setup(
     name="torch-base-network",
     version=VERSION,
     description=DESCRIPTION,
```

