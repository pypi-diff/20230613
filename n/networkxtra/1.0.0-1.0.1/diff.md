# Comparing `tmp/networkxtra-1.0.0.tar.gz` & `tmp/networkxtra-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "networkxtra-1.0.0.tar", max compression
+gzip compressed data, was "networkxtra-1.0.1.tar", max compression
```

## Comparing `networkxtra-1.0.0.tar` & `networkxtra-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0     1071 2023-06-13 18:05:10.842650 networkxtra-1.0.0/LICENSE
--rw-r--r--   0        0        0      987 2023-06-13 18:05:10.842650 networkxtra-1.0.0/networkxtra/__init__.py
--rw-r--r--   0        0        0        0 2023-06-13 18:05:10.842650 networkxtra-1.0.0/networkxtra/algorithms/__init__.py
--rw-r--r--   0        0        0      267 2023-06-13 18:05:10.842650 networkxtra-1.0.0/networkxtra/algorithms/components.py
--rw-r--r--   0        0        0        0 2023-06-13 18:05:10.842650 networkxtra-1.0.0/networkxtra/convert/__init__.py
--rw-r--r--   0        0        0     1520 2023-06-13 18:05:10.842650 networkxtra-1.0.0/networkxtra/convert/geojsonl.py
--rw-r--r--   0        0        0        0 2023-06-13 18:05:10.842650 networkxtra-1.0.0/networkxtra/drawing/__init__.py
--rw-r--r--   0        0        0     1779 2023-06-13 18:05:10.842650 networkxtra-1.0.0/networkxtra/drawing/cairo.py
--rw-r--r--   0        0        0        0 2023-06-13 18:05:10.842650 networkxtra-1.0.0/networkxtra/functions/__init__.py
--rw-r--r--   0        0        0      115 2023-06-13 18:05:10.842650 networkxtra-1.0.0/networkxtra/functions/graph.py
--rw-r--r--   0        0        0      120 2023-06-13 18:05:10.842650 networkxtra-1.0.0/networkxtra/functions/leafs.py
--rw-r--r--   0        0        0        0 2023-06-13 18:05:10.842650 networkxtra-1.0.0/networkxtra/layout/__init__.py
--rw-r--r--   0        0        0     1434 2023-06-13 18:05:10.842650 networkxtra-1.0.0/networkxtra/layout/bfs.py
--rw-r--r--   0        0        0     3681 2023-06-13 18:05:10.842650 networkxtra-1.0.0/networkxtra/layout/lgl.py
--rw-r--r--   0        0        0        0 2023-06-13 18:05:10.842650 networkxtra-1.0.0/networkxtra/readwrite/__init__.py
--rw-r--r--   0        0        0      873 2023-06-13 18:05:10.842650 networkxtra-1.0.0/networkxtra/readwrite/geojsonl.py
--rw-r--r--   0        0        0     1108 2023-06-13 18:05:10.842650 networkxtra-1.0.0/networkxtra/readwrite/lgl.py
--rw-r--r--   0        0        0      600 2023-06-13 18:05:10.842650 networkxtra-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      690 1970-01-01 00:00:00.000000 networkxtra-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-13 18:09:36.741834 networkxtra-1.0.1/LICENSE
+-rw-r--r--   0        0        0      930 2023-06-13 18:09:36.741834 networkxtra-1.0.1/README.md
+-rw-r--r--   0        0        0      987 2023-06-13 18:09:36.741834 networkxtra-1.0.1/networkxtra/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-13 18:09:36.741834 networkxtra-1.0.1/networkxtra/algorithms/__init__.py
+-rw-r--r--   0        0        0      267 2023-06-13 18:09:36.741834 networkxtra-1.0.1/networkxtra/algorithms/components.py
+-rw-r--r--   0        0        0        0 2023-06-13 18:09:36.741834 networkxtra-1.0.1/networkxtra/convert/__init__.py
+-rw-r--r--   0        0        0     1520 2023-06-13 18:09:36.741834 networkxtra-1.0.1/networkxtra/convert/geojsonl.py
+-rw-r--r--   0        0        0        0 2023-06-13 18:09:36.741834 networkxtra-1.0.1/networkxtra/drawing/__init__.py
+-rw-r--r--   0        0        0     1779 2023-06-13 18:09:36.741834 networkxtra-1.0.1/networkxtra/drawing/cairo.py
+-rw-r--r--   0        0        0        0 2023-06-13 18:09:36.741834 networkxtra-1.0.1/networkxtra/functions/__init__.py
+-rw-r--r--   0        0        0      115 2023-06-13 18:09:36.741834 networkxtra-1.0.1/networkxtra/functions/graph.py
+-rw-r--r--   0        0        0      120 2023-06-13 18:09:36.741834 networkxtra-1.0.1/networkxtra/functions/leafs.py
+-rw-r--r--   0        0        0        0 2023-06-13 18:09:36.741834 networkxtra-1.0.1/networkxtra/layout/__init__.py
+-rw-r--r--   0        0        0     1434 2023-06-13 18:09:36.741834 networkxtra-1.0.1/networkxtra/layout/bfs.py
+-rw-r--r--   0        0        0     3681 2023-06-13 18:09:36.741834 networkxtra-1.0.1/networkxtra/layout/lgl.py
+-rw-r--r--   0        0        0        0 2023-06-13 18:09:36.741834 networkxtra-1.0.1/networkxtra/readwrite/__init__.py
+-rw-r--r--   0        0        0      873 2023-06-13 18:09:36.741834 networkxtra-1.0.1/networkxtra/readwrite/geojsonl.py
+-rw-r--r--   0        0        0     1108 2023-06-13 18:09:36.741834 networkxtra-1.0.1/networkxtra/readwrite/lgl.py
+-rw-r--r--   0        0        0      676 2023-06-13 18:09:36.741834 networkxtra-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1711 1970-01-01 00:00:00.000000 networkxtra-1.0.1/PKG-INFO
```

### Comparing `networkxtra-1.0.0/LICENSE` & `networkxtra-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `networkxtra-1.0.0/networkxtra/__init__.py` & `networkxtra-1.0.1/networkxtra/__init__.py`

 * *Files identical despite different names*

### Comparing `networkxtra-1.0.0/networkxtra/convert/geojsonl.py` & `networkxtra-1.0.1/networkxtra/convert/geojsonl.py`

 * *Files identical despite different names*

### Comparing `networkxtra-1.0.0/networkxtra/drawing/cairo.py` & `networkxtra-1.0.1/networkxtra/drawing/cairo.py`

 * *Files identical despite different names*

### Comparing `networkxtra-1.0.0/networkxtra/layout/bfs.py` & `networkxtra-1.0.1/networkxtra/layout/bfs.py`

 * *Files identical despite different names*

### Comparing `networkxtra-1.0.0/networkxtra/layout/lgl.py` & `networkxtra-1.0.1/networkxtra/layout/lgl.py`

 * *Files identical despite different names*

### Comparing `networkxtra-1.0.0/networkxtra/readwrite/geojsonl.py` & `networkxtra-1.0.1/networkxtra/readwrite/geojsonl.py`

 * *Files identical despite different names*

### Comparing `networkxtra-1.0.0/networkxtra/readwrite/lgl.py` & `networkxtra-1.0.1/networkxtra/readwrite/lgl.py`

 * *Files identical despite different names*

### Comparing `networkxtra-1.0.0/pyproject.toml` & `networkxtra-1.0.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 [tool.poetry]
 name = "networkxtra"
-version = "1.0.0"
+version = "1.0.1"
 description = "Extra functions for networkx."
 authors = [
-    "Matthieu Gouel <matthieu.gouel@lip6.fr>",
-    "Maxime Mouchet <max@maxmouchet.com>"
+    "Maxime Mouchet <max@maxmouchet.com>",
+    "Matthieu Gouel <matthieu.gouel@lip6.fr>"
 ]
+homepage = "https://github.com/maxmouchet/networkxtra"
+readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 networkx = "^3.1"
 numpy = "^1.24.3"
 pycairo = "^1.23.0"
```

