# Comparing `tmp/MALDIpy-0.1.1.tar.gz` & `tmp/MALDIpy-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MALDIpy-0.1.1.tar", last modified: Sat Jun 10 02:39:37 2023, max compression
+gzip compressed data, was "MALDIpy-0.1.2.tar", last modified: Mon Jun 12 22:12:05 2023, max compression
```

## Comparing `MALDIpy-0.1.1.tar` & `MALDIpy-0.1.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 hli       (1002) labmem    (1001)        0 2023-06-10 02:39:37.543417 MALDIpy-0.1.1/
--rw-r--r--   0 hli       (1002) labmem    (1001)     1062 2023-04-04 21:12:06.000000 MALDIpy-0.1.1/LICENSE
-drwxr-xr-x   0 hli       (1002) labmem    (1001)        0 2023-06-10 02:39:37.539417 MALDIpy-0.1.1/MALDIpy/
--rw-r--r--   0 hli       (1002) labmem    (1001)      187 2023-06-10 02:39:24.000000 MALDIpy-0.1.1/MALDIpy/__init__.py
--rw-r--r--   0 hli       (1002) labmem    (1001)     5008 2023-06-10 02:39:17.000000 MALDIpy-0.1.1/MALDIpy/featureplot.py
--rw-r--r--   0 hli       (1002) labmem    (1001)     6599 2023-04-06 16:02:36.000000 MALDIpy-0.1.1/MALDIpy/msi_data.py
--rw-r--r--   0 hli       (1002) labmem    (1001)     3084 2023-04-06 18:34:41.000000 MALDIpy-0.1.1/MALDIpy/multi_sample.py
--rw-r--r--   0 hli       (1002) labmem    (1001)     6619 2023-06-10 01:50:57.000000 MALDIpy-0.1.1/MALDIpy/projection.py
-drwxr-xr-x   0 hli       (1002) labmem    (1001)        0 2023-06-10 02:39:37.543417 MALDIpy-0.1.1/MALDIpy/shell/
--rw-r--r--   0 hli       (1002) labmem    (1001)       61 2023-04-04 21:15:37.000000 MALDIpy-0.1.1/MALDIpy/shell/__init__.py
--rw-r--r--   0 hli       (1002) labmem    (1001)      196 2023-04-04 21:15:37.000000 MALDIpy-0.1.1/MALDIpy/shell/usage.py
--rw-r--r--   0 hli       (1002) labmem    (1001)     1690 2023-04-06 13:55:22.000000 MALDIpy-0.1.1/MALDIpy/single_cell.py
-drwxr-xr-x   0 hli       (1002) labmem    (1001)        0 2023-06-10 02:39:37.543417 MALDIpy-0.1.1/MALDIpy/src/
--rw-r--r--   0 hli       (1002) labmem    (1001)        0 2023-04-04 21:12:06.000000 MALDIpy-0.1.1/MALDIpy/src/temp.txt
-drwxr-xr-x   0 hli       (1002) labmem    (1001)        0 2023-06-10 02:39:37.543417 MALDIpy-0.1.1/MALDIpy.egg-info/
--rw-r--r--   0 hli       (1002) labmem    (1001)      696 2023-06-10 02:39:37.000000 MALDIpy-0.1.1/MALDIpy.egg-info/PKG-INFO
--rw-r--r--   0 hli       (1002) labmem    (1001)      441 2023-06-10 02:39:37.000000 MALDIpy-0.1.1/MALDIpy.egg-info/SOURCES.txt
--rw-r--r--   0 hli       (1002) labmem    (1001)        1 2023-06-10 02:39:37.000000 MALDIpy-0.1.1/MALDIpy.egg-info/dependency_links.txt
--rw-r--r--   0 hli       (1002) labmem    (1001)       47 2023-06-10 02:39:37.000000 MALDIpy-0.1.1/MALDIpy.egg-info/entry_points.txt
--rw-r--r--   0 hli       (1002) labmem    (1001)        8 2023-06-10 02:39:37.000000 MALDIpy-0.1.1/MALDIpy.egg-info/top_level.txt
--rw-r--r--   0 hli       (1002) labmem    (1001)        1 2023-04-04 21:25:43.000000 MALDIpy-0.1.1/MALDIpy.egg-info/zip-safe
--rw-r--r--   0 hli       (1002) labmem    (1001)      176 2023-04-04 21:15:37.000000 MALDIpy-0.1.1/MANIFEST.in
--rw-r--r--   0 hli       (1002) labmem    (1001)      696 2023-06-10 02:39:37.543417 MALDIpy-0.1.1/PKG-INFO
--rw-r--r--   0 hli       (1002) labmem    (1001)      252 2023-06-10 02:39:29.000000 MALDIpy-0.1.1/README.md
--rw-r--r--   0 hli       (1002) labmem    (1001)        0 2023-04-04 21:12:06.000000 MALDIpy-0.1.1/requirements.txt
--rw-r--r--   0 hli       (1002) labmem    (1001)       38 2023-06-10 02:39:37.543417 MALDIpy-0.1.1/setup.cfg
--rw-r--r--   0 hli       (1002) labmem    (1001)     1922 2023-06-10 02:02:43.000000 MALDIpy-0.1.1/setup.py
+drwxr-xr-x   0 hli       (1002) labmem    (1001)        0 2023-06-12 22:12:04.997632 MALDIpy-0.1.2/
+-rw-r--r--   0 hli       (1002) labmem    (1001)     1062 2023-04-04 21:12:06.000000 MALDIpy-0.1.2/LICENSE
+drwxr-xr-x   0 hli       (1002) labmem    (1001)        0 2023-06-12 22:12:04.965632 MALDIpy-0.1.2/MALDIpy/
+-rw-r--r--   0 hli       (1002) labmem    (1001)      187 2023-06-12 22:10:24.000000 MALDIpy-0.1.2/MALDIpy/__init__.py
+-rw-r--r--   0 hli       (1002) labmem    (1001)     7689 2023-06-12 22:10:09.000000 MALDIpy-0.1.2/MALDIpy/featureplot.py
+-rw-r--r--   0 hli       (1002) labmem    (1001)     6599 2023-04-06 16:02:36.000000 MALDIpy-0.1.2/MALDIpy/msi_data.py
+-rw-r--r--   0 hli       (1002) labmem    (1001)     3084 2023-04-06 18:34:41.000000 MALDIpy-0.1.2/MALDIpy/multi_sample.py
+-rw-r--r--   0 hli       (1002) labmem    (1001)     6619 2023-06-10 01:50:57.000000 MALDIpy-0.1.2/MALDIpy/projection.py
+drwxr-xr-x   0 hli       (1002) labmem    (1001)        0 2023-06-12 22:12:04.993632 MALDIpy-0.1.2/MALDIpy/shell/
+-rw-r--r--   0 hli       (1002) labmem    (1001)       61 2023-04-04 21:15:37.000000 MALDIpy-0.1.2/MALDIpy/shell/__init__.py
+-rw-r--r--   0 hli       (1002) labmem    (1001)      196 2023-04-04 21:15:37.000000 MALDIpy-0.1.2/MALDIpy/shell/usage.py
+-rw-r--r--   0 hli       (1002) labmem    (1001)     1690 2023-04-06 13:55:22.000000 MALDIpy-0.1.2/MALDIpy/single_cell.py
+drwxr-xr-x   0 hli       (1002) labmem    (1001)        0 2023-06-12 22:12:04.997632 MALDIpy-0.1.2/MALDIpy/src/
+-rw-r--r--   0 hli       (1002) labmem    (1001)        0 2023-04-04 21:12:06.000000 MALDIpy-0.1.2/MALDIpy/src/temp.txt
+drwxr-xr-x   0 hli       (1002) labmem    (1001)        0 2023-06-12 22:12:04.985632 MALDIpy-0.1.2/MALDIpy.egg-info/
+-rw-r--r--   0 hli       (1002) labmem    (1001)      575 2023-06-12 22:12:04.000000 MALDIpy-0.1.2/MALDIpy.egg-info/PKG-INFO
+-rw-r--r--   0 hli       (1002) labmem    (1001)      441 2023-06-12 22:12:04.000000 MALDIpy-0.1.2/MALDIpy.egg-info/SOURCES.txt
+-rw-r--r--   0 hli       (1002) labmem    (1001)        1 2023-06-12 22:12:04.000000 MALDIpy-0.1.2/MALDIpy.egg-info/dependency_links.txt
+-rw-r--r--   0 hli       (1002) labmem    (1001)       47 2023-06-12 22:12:04.000000 MALDIpy-0.1.2/MALDIpy.egg-info/entry_points.txt
+-rw-r--r--   0 hli       (1002) labmem    (1001)        8 2023-06-12 22:12:04.000000 MALDIpy-0.1.2/MALDIpy.egg-info/top_level.txt
+-rw-r--r--   0 hli       (1002) labmem    (1001)        1 2023-04-04 21:25:43.000000 MALDIpy-0.1.2/MALDIpy.egg-info/zip-safe
+-rw-r--r--   0 hli       (1002) labmem    (1001)      176 2023-04-04 21:15:37.000000 MALDIpy-0.1.2/MANIFEST.in
+-rw-r--r--   0 hli       (1002) labmem    (1001)      575 2023-06-12 22:12:04.997632 MALDIpy-0.1.2/PKG-INFO
+-rw-r--r--   0 hli       (1002) labmem    (1001)      139 2023-06-12 22:11:17.000000 MALDIpy-0.1.2/README.md
+-rw-r--r--   0 hli       (1002) labmem    (1001)        0 2023-04-04 21:12:06.000000 MALDIpy-0.1.2/requirements.txt
+-rw-r--r--   0 hli       (1002) labmem    (1001)       38 2023-06-12 22:12:04.997632 MALDIpy-0.1.2/setup.cfg
+-rw-r--r--   0 hli       (1002) labmem    (1001)     1922 2023-06-10 02:02:43.000000 MALDIpy-0.1.2/setup.py
```

### Comparing `MALDIpy-0.1.1/LICENSE` & `MALDIpy-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `MALDIpy-0.1.1/MALDIpy/msi_data.py` & `MALDIpy-0.1.2/MALDIpy/msi_data.py`

 * *Files identical despite different names*

### Comparing `MALDIpy-0.1.1/MALDIpy/multi_sample.py` & `MALDIpy-0.1.2/MALDIpy/multi_sample.py`

 * *Files identical despite different names*

### Comparing `MALDIpy-0.1.1/MALDIpy/projection.py` & `MALDIpy-0.1.2/MALDIpy/projection.py`

 * *Files identical despite different names*

### Comparing `MALDIpy-0.1.1/MALDIpy/single_cell.py` & `MALDIpy-0.1.2/MALDIpy/single_cell.py`

 * *Files identical despite different names*

### Comparing `MALDIpy-0.1.1/setup.py` & `MALDIpy-0.1.2/setup.py`

 * *Files identical despite different names*

