# Comparing `tmp/sparrow-mlpipes-0.4.4.dev1663691721.tar.gz` & `tmp/sparrow-mlpipes-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparrow-mlpipes-0.4.4.dev1663691721.tar", last modified: Tue Sep 20 16:35:34 2022, max compression
+gzip compressed data, was "sparrow-mlpipes-0.4.5.tar", last modified: Tue Jun 13 15:39:12 2023, max compression
```

## Comparing `sparrow-mlpipes-0.4.4.dev1663691721.tar` & `sparrow-mlpipes-0.4.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 16:35:34.530075 sparrow-mlpipes-0.4.4.dev1663691721/
--rwxr-xr-x   0 runner    (1001) docker     (121)     1074 2022-09-20 16:34:31.000000 sparrow-mlpipes-0.4.4.dev1663691721/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      221 2022-09-20 16:35:34.530075 sparrow-mlpipes-0.4.4.dev1663691721/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      844 2022-09-20 16:34:31.000000 sparrow-mlpipes-0.4.4.dev1663691721/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      546 2022-09-20 16:35:34.530075 sparrow-mlpipes-0.4.4.dev1663691721/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-20 16:34:31.000000 sparrow-mlpipes-0.4.4.dev1663691721/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 16:35:34.526075 sparrow-mlpipes-0.4.4.dev1663691721/sparrow_mlpipes/
--rwxr-xr-x   0 runner    (1001) docker     (121)      179 2022-09-20 16:34:31.000000 sparrow-mlpipes-0.4.4.dev1663691721/sparrow_mlpipes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 16:35:34.530075 sparrow-mlpipes-0.4.4.dev1663691721/sparrow_mlpipes/bins/
--rwxr-xr-x   0 runner    (1001) docker     (121)      281 2022-09-20 16:34:31.000000 sparrow-mlpipes-0.4.4.dev1663691721/sparrow_mlpipes/bins/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1611 2022-09-20 16:34:31.000000 sparrow-mlpipes-0.4.4.dev1663691721/sparrow_mlpipes/bins/nvinfer.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1660 2022-09-20 16:34:31.000000 sparrow-mlpipes-0.4.4.dev1663691721/sparrow_mlpipes/bins/nvinferserver.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      633 2022-09-20 16:34:31.000000 sparrow-mlpipes-0.4.4.dev1663691721/sparrow_mlpipes/bins/nvtracker.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1045 2022-09-20 16:34:31.000000 sparrow-mlpipes-0.4.4.dev1663691721/sparrow_mlpipes/bins/sink.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1539 2022-09-20 16:34:31.000000 sparrow-mlpipes-0.4.4.dev1663691721/sparrow_mlpipes/bins/source.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      893 2022-09-20 16:34:31.000000 sparrow-mlpipes-0.4.4.dev1663691721/sparrow_mlpipes/bins/visualization.py
--rwxr-xr-x   0 runner    (1001) docker     (121)       91 2022-09-20 16:34:31.000000 sparrow-mlpipes-0.4.4.dev1663691721/sparrow_mlpipes/constants.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      388 2022-09-20 16:34:31.000000 sparrow-mlpipes-0.4.4.dev1663691721/sparrow_mlpipes/element.py
--rwxr-xr-x   0 runner    (1001) docker     (121)       41 2022-09-20 16:34:31.000000 sparrow-mlpipes-0.4.4.dev1663691721/sparrow_mlpipes/exceptions.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      129 2022-09-20 16:34:31.000000 sparrow-mlpipes-0.4.4.dev1663691721/sparrow_mlpipes/initialize.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      846 2022-09-20 16:34:31.000000 sparrow-mlpipes-0.4.4.dev1663691721/sparrow_mlpipes/pipeline.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1656 2022-09-20 16:34:31.000000 sparrow-mlpipes-0.4.4.dev1663691721/sparrow_mlpipes/pyds.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 16:35:34.530075 sparrow-mlpipes-0.4.4.dev1663691721/sparrow_mlpipes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      221 2022-09-20 16:35:34.000000 sparrow-mlpipes-0.4.4.dev1663691721/sparrow_mlpipes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      661 2022-09-20 16:35:34.000000 sparrow-mlpipes-0.4.4.dev1663691721/sparrow_mlpipes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-20 16:35:34.000000 sparrow-mlpipes-0.4.4.dev1663691721/sparrow_mlpipes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       98 2022-09-20 16:35:34.000000 sparrow-mlpipes-0.4.4.dev1663691721/sparrow_mlpipes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-09-20 16:35:34.000000 sparrow-mlpipes-0.4.4.dev1663691721/sparrow_mlpipes.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:39:12.719612 sparrow-mlpipes-0.4.5/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1074 2023-06-13 15:37:08.000000 sparrow-mlpipes-0.4.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-13 15:39:12.719612 sparrow-mlpipes-0.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-13 15:37:08.000000 sparrow-mlpipes-0.4.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-13 15:39:12.719612 sparrow-mlpipes-0.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 15:37:08.000000 sparrow-mlpipes-0.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:39:12.715612 sparrow-mlpipes-0.4.5/sparrow_mlpipes/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      179 2023-06-13 15:37:08.000000 sparrow-mlpipes-0.4.5/sparrow_mlpipes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:39:12.719612 sparrow-mlpipes-0.4.5/sparrow_mlpipes/bins/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      281 2023-06-13 15:37:08.000000 sparrow-mlpipes-0.4.5/sparrow_mlpipes/bins/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1611 2023-06-13 15:37:08.000000 sparrow-mlpipes-0.4.5/sparrow_mlpipes/bins/nvinfer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1660 2023-06-13 15:37:08.000000 sparrow-mlpipes-0.4.5/sparrow_mlpipes/bins/nvinferserver.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      633 2023-06-13 15:37:08.000000 sparrow-mlpipes-0.4.5/sparrow_mlpipes/bins/nvtracker.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1045 2023-06-13 15:37:08.000000 sparrow-mlpipes-0.4.5/sparrow_mlpipes/bins/sink.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1539 2023-06-13 15:37:08.000000 sparrow-mlpipes-0.4.5/sparrow_mlpipes/bins/source.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      893 2023-06-13 15:37:08.000000 sparrow-mlpipes-0.4.5/sparrow_mlpipes/bins/visualization.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       91 2023-06-13 15:37:08.000000 sparrow-mlpipes-0.4.5/sparrow_mlpipes/constants.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      388 2023-06-13 15:37:08.000000 sparrow-mlpipes-0.4.5/sparrow_mlpipes/element.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       41 2023-06-13 15:37:08.000000 sparrow-mlpipes-0.4.5/sparrow_mlpipes/exceptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      129 2023-06-13 15:37:08.000000 sparrow-mlpipes-0.4.5/sparrow_mlpipes/initialize.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      846 2023-06-13 15:37:08.000000 sparrow-mlpipes-0.4.5/sparrow_mlpipes/pipeline.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1656 2023-06-13 15:37:08.000000 sparrow-mlpipes-0.4.5/sparrow_mlpipes/pyds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:39:12.715612 sparrow-mlpipes-0.4.5/sparrow_mlpipes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-13 15:39:12.000000 sparrow-mlpipes-0.4.5/sparrow_mlpipes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-13 15:39:12.000000 sparrow-mlpipes-0.4.5/sparrow_mlpipes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 15:39:12.000000 sparrow-mlpipes-0.4.5/sparrow_mlpipes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-13 15:39:12.000000 sparrow-mlpipes-0.4.5/sparrow_mlpipes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-13 15:39:12.000000 sparrow-mlpipes-0.4.5/sparrow_mlpipes.egg-info/top_level.txt
```

### Comparing `sparrow-mlpipes-0.4.4.dev1663691721/LICENSE` & `sparrow-mlpipes-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sparrow-mlpipes-0.4.4.dev1663691721/README.md` & `sparrow-mlpipes-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `sparrow-mlpipes-0.4.4.dev1663691721/sparrow_mlpipes/bins/nvinfer.py` & `sparrow-mlpipes-0.4.5/sparrow_mlpipes/bins/nvinfer.py`

 * *Files identical despite different names*

### Comparing `sparrow-mlpipes-0.4.4.dev1663691721/sparrow_mlpipes/bins/nvinferserver.py` & `sparrow-mlpipes-0.4.5/sparrow_mlpipes/bins/nvinferserver.py`

 * *Files identical despite different names*

### Comparing `sparrow-mlpipes-0.4.4.dev1663691721/sparrow_mlpipes/bins/nvtracker.py` & `sparrow-mlpipes-0.4.5/sparrow_mlpipes/bins/nvtracker.py`

 * *Files identical despite different names*

### Comparing `sparrow-mlpipes-0.4.4.dev1663691721/sparrow_mlpipes/bins/sink.py` & `sparrow-mlpipes-0.4.5/sparrow_mlpipes/bins/sink.py`

 * *Files identical despite different names*

### Comparing `sparrow-mlpipes-0.4.4.dev1663691721/sparrow_mlpipes/bins/source.py` & `sparrow-mlpipes-0.4.5/sparrow_mlpipes/bins/source.py`

 * *Files identical despite different names*

### Comparing `sparrow-mlpipes-0.4.4.dev1663691721/sparrow_mlpipes/bins/visualization.py` & `sparrow-mlpipes-0.4.5/sparrow_mlpipes/bins/visualization.py`

 * *Files identical despite different names*

### Comparing `sparrow-mlpipes-0.4.4.dev1663691721/sparrow_mlpipes/pipeline.py` & `sparrow-mlpipes-0.4.5/sparrow_mlpipes/pipeline.py`

 * *Files identical despite different names*

### Comparing `sparrow-mlpipes-0.4.4.dev1663691721/sparrow_mlpipes/pyds.py` & `sparrow-mlpipes-0.4.5/sparrow_mlpipes/pyds.py`

 * *Files identical despite different names*

### Comparing `sparrow-mlpipes-0.4.4.dev1663691721/sparrow_mlpipes.egg-info/SOURCES.txt` & `sparrow-mlpipes-0.4.5/sparrow_mlpipes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

