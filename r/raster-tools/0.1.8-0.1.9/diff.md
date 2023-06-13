# Comparing `tmp/raster-tools-0.1.8.tar.gz` & `tmp/raster-tools-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raster-tools-0.1.8.tar", last modified: Tue May 23 22:06:23 2023, max compression
+gzip compressed data, was "raster-tools-0.1.9.tar", last modified: Fri Jun  2 20:21:51 2023, max compression
```

## Comparing `raster-tools-0.1.8.tar` & `raster-tools-0.1.9.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2023-05-23 22:06:23.165470 raster-tools-0.1.8/
--rw-------   0 fred      (1000) fred      (1000)    35149 2022-08-26 20:44:14.000000 raster-tools-0.1.8/LICENSE
--rw-r--r--   0 fred      (1000) fred      (1000)      316 2022-08-26 20:44:14.000000 raster-tools-0.1.8/MANIFEST.in
--rw-rw-r--   0 fred      (1000) fred      (1000)     1800 2023-05-23 22:06:23.165470 raster-tools-0.1.8/PKG-INFO
--rw-rw-r--   0 fred      (1000) fred      (1000)     1198 2023-04-11 21:45:35.000000 raster-tools-0.1.8/README.md
--rw-r--r--   0 fred      (1000) fred      (1000)      273 2022-08-26 20:44:14.000000 raster-tools-0.1.8/pyproject.toml
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2023-05-23 22:06:23.165470 raster-tools-0.1.8/raster_tools/
--rw-rw-r--   0 fred      (1000) fred      (1000)      934 2023-01-25 21:30:15.000000 raster-tools-0.1.8/raster_tools/__init__.py
--rw-r--r--   0 fred      (1000) fred      (1000)      383 2023-01-28 03:26:22.000000 raster-tools-0.1.8/raster_tools/_compat.py
--rw-rw-r--   0 fred      (1000) fred      (1000)       22 2023-05-23 22:06:02.000000 raster-tools-0.1.8/raster_tools/_version.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     7664 2023-01-04 22:54:45.000000 raster-tools-0.1.8/raster_tools/batch.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     6536 2023-02-01 01:11:45.000000 raster-tools-0.1.8/raster_tools/clipping.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    11725 2023-05-01 20:54:28.000000 raster-tools-0.1.8/raster_tools/creation.py
--rw-r--r--   0 fred      (1000) fred      (1000)     1286 2022-11-29 01:39:49.000000 raster-tools-0.1.8/raster_tools/dask_utils.py
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2023-05-23 22:06:23.165470 raster-tools-0.1.8/raster_tools/distance/
--rw-r--r--   0 fred      (1000) fred      (1000)      427 2022-08-26 20:44:16.000000 raster-tools-0.1.8/raster_tools/distance/__init__.py
--rw-r--r--   0 fred      (1000) fred      (1000)     6777 2022-10-21 23:01:50.000000 raster-tools-0.1.8/raster_tools/distance/_heap.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    26495 2023-05-23 21:55:22.000000 raster-tools-0.1.8/raster_tools/distance/cost_distance.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    34940 2023-04-13 22:25:41.000000 raster-tools-0.1.8/raster_tools/distance/proximity.py
--rw-r--r--   0 fred      (1000) fred      (1000)     3240 2022-12-09 03:28:15.000000 raster-tools-0.1.8/raster_tools/dtypes.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    21032 2023-04-21 22:57:28.000000 raster-tools-0.1.8/raster_tools/focal.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    43026 2023-05-01 20:58:01.000000 raster-tools-0.1.8/raster_tools/general.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     7149 2023-01-04 22:54:45.000000 raster-tools-0.1.8/raster_tools/io.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    12275 2023-02-15 02:21:21.000000 raster-tools-0.1.8/raster_tools/line_stats.py
--rw-r--r--   0 fred      (1000) fred      (1000)     2123 2022-10-22 00:44:28.000000 raster-tools-0.1.8/raster_tools/masking.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    48687 2023-05-23 21:55:18.000000 raster-tools-0.1.8/raster_tools/raster.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     4076 2023-05-18 19:19:17.000000 raster-tools-0.1.8/raster_tools/stat_common.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    18436 2023-05-23 22:00:46.000000 raster-tools-0.1.8/raster_tools/surface.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     3170 2023-05-11 18:56:03.000000 raster-tools-0.1.8/raster_tools/utils.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    28748 2023-05-23 21:55:18.000000 raster-tools-0.1.8/raster_tools/vector.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    20970 2023-05-01 20:58:01.000000 raster-tools-0.1.8/raster_tools/zonal.py
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2023-05-23 22:06:23.165470 raster-tools-0.1.8/raster_tools.egg-info/
--rw-rw-r--   0 fred      (1000) fred      (1000)     1800 2023-05-23 22:06:23.000000 raster-tools-0.1.8/raster_tools.egg-info/PKG-INFO
--rw-rw-r--   0 fred      (1000) fred      (1000)     1797 2023-05-23 22:06:23.000000 raster-tools-0.1.8/raster_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 fred      (1000) fred      (1000)        1 2023-05-23 22:06:23.000000 raster-tools-0.1.8/raster_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 fred      (1000) fred      (1000)      139 2023-05-23 22:06:23.000000 raster-tools-0.1.8/raster_tools.egg-info/requires.txt
--rw-rw-r--   0 fred      (1000) fred      (1000)       13 2023-05-23 22:06:23.000000 raster-tools-0.1.8/raster_tools.egg-info/top_level.txt
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2023-05-23 22:06:23.165470 raster-tools-0.1.8/requirements/
--rw-rw-r--   0 fred      (1000) fred      (1000)      139 2023-01-25 21:30:15.000000 raster-tools-0.1.8/requirements/default.txt
--rw-rw-r--   0 fred      (1000) fred      (1000)       38 2023-05-23 22:06:23.165470 raster-tools-0.1.8/setup.cfg
--rw-rw-r--   0 fred      (1000) fred      (1000)     1526 2023-01-31 00:50:40.000000 raster-tools-0.1.8/setup.py
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2023-05-23 22:06:23.165470 raster-tools-0.1.8/tests/
--rw-rw-r--   0 fred      (1000) fred      (1000)     4072 2023-01-04 22:54:46.000000 raster-tools-0.1.8/tests/test_clipping.py
--rw-r--r--   0 fred      (1000) fred      (1000)     4827 2023-05-01 20:54:28.000000 raster-tools-0.1.8/tests/test_creation.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     7404 2023-05-23 21:55:22.000000 raster-tools-0.1.8/tests/test_distance.py
--rw-r--r--   0 fred      (1000) fred      (1000)     1297 2022-08-26 20:44:16.000000 raster-tools-0.1.8/tests/test_distance__heap.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     8212 2023-04-14 00:09:55.000000 raster-tools-0.1.8/tests/test_distance_proximity.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    20233 2023-03-03 21:13:40.000000 raster-tools-0.1.8/tests/test_focal.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    29890 2023-04-29 01:59:10.000000 raster-tools-0.1.8/tests/test_general.py
--rw-r--r--   0 fred      (1000) fred      (1000)     7288 2023-01-28 03:48:27.000000 raster-tools-0.1.8/tests/test_line_stats.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    56760 2023-05-23 21:55:18.000000 raster-tools-0.1.8/tests/test_raster.py
--rw-r--r--   0 fred      (1000) fred      (1000)     4124 2022-08-26 20:44:16.000000 raster-tools-0.1.8/tests/test_stat_common.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     5157 2023-02-15 02:21:21.000000 raster-tools-0.1.8/tests/test_surface.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    10612 2023-05-11 21:16:13.000000 raster-tools-0.1.8/tests/test_vector.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     6903 2023-04-06 20:45:48.000000 raster-tools-0.1.8/tests/test_zonal.py
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2023-06-02 20:21:51.994378 raster-tools-0.1.9/
+-rw-------   0 fred      (1000) fred      (1000)    35149 2022-08-26 20:44:14.000000 raster-tools-0.1.9/LICENSE
+-rw-r--r--   0 fred      (1000) fred      (1000)      316 2022-08-26 20:44:14.000000 raster-tools-0.1.9/MANIFEST.in
+-rw-rw-r--   0 fred      (1000) fred      (1000)     1800 2023-06-02 20:21:51.994378 raster-tools-0.1.9/PKG-INFO
+-rw-rw-r--   0 fred      (1000) fred      (1000)     1198 2023-04-11 21:45:35.000000 raster-tools-0.1.9/README.md
+-rw-r--r--   0 fred      (1000) fred      (1000)      273 2022-08-26 20:44:14.000000 raster-tools-0.1.9/pyproject.toml
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2023-06-02 20:21:51.990378 raster-tools-0.1.9/raster_tools/
+-rw-rw-r--   0 fred      (1000) fred      (1000)      934 2023-01-25 21:30:15.000000 raster-tools-0.1.9/raster_tools/__init__.py
+-rw-r--r--   0 fred      (1000) fred      (1000)      383 2023-01-28 03:26:22.000000 raster-tools-0.1.9/raster_tools/_compat.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)       22 2023-06-02 20:15:33.000000 raster-tools-0.1.9/raster_tools/_version.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     7664 2023-01-04 22:54:45.000000 raster-tools-0.1.9/raster_tools/batch.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     6536 2023-02-01 01:11:45.000000 raster-tools-0.1.9/raster_tools/clipping.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    11725 2023-05-01 20:54:28.000000 raster-tools-0.1.9/raster_tools/creation.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     1286 2022-11-29 01:39:49.000000 raster-tools-0.1.9/raster_tools/dask_utils.py
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2023-06-02 20:21:51.990378 raster-tools-0.1.9/raster_tools/distance/
+-rw-r--r--   0 fred      (1000) fred      (1000)      427 2022-08-26 20:44:16.000000 raster-tools-0.1.9/raster_tools/distance/__init__.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     6777 2022-10-21 23:01:50.000000 raster-tools-0.1.9/raster_tools/distance/_heap.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    26495 2023-05-24 19:56:50.000000 raster-tools-0.1.9/raster_tools/distance/cost_distance.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    34940 2023-04-13 22:25:41.000000 raster-tools-0.1.9/raster_tools/distance/proximity.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     3240 2023-06-02 20:21:13.000000 raster-tools-0.1.9/raster_tools/dtypes.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    21032 2023-04-21 22:57:28.000000 raster-tools-0.1.9/raster_tools/focal.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    43021 2023-06-02 20:11:39.000000 raster-tools-0.1.9/raster_tools/general.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     7149 2023-01-04 22:54:45.000000 raster-tools-0.1.9/raster_tools/io.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    12275 2023-02-15 02:21:21.000000 raster-tools-0.1.9/raster_tools/line_stats.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     2123 2022-10-22 00:44:28.000000 raster-tools-0.1.9/raster_tools/masking.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    48687 2023-06-02 19:50:13.000000 raster-tools-0.1.9/raster_tools/raster.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     4076 2023-05-18 19:19:17.000000 raster-tools-0.1.9/raster_tools/stat_common.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    18436 2023-05-24 19:56:50.000000 raster-tools-0.1.9/raster_tools/surface.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     3170 2023-05-11 18:56:03.000000 raster-tools-0.1.9/raster_tools/utils.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    28748 2023-06-02 19:50:06.000000 raster-tools-0.1.9/raster_tools/vector.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    20970 2023-05-01 20:58:01.000000 raster-tools-0.1.9/raster_tools/zonal.py
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2023-06-02 20:21:51.990378 raster-tools-0.1.9/raster_tools.egg-info/
+-rw-rw-r--   0 fred      (1000) fred      (1000)     1800 2023-06-02 20:21:51.000000 raster-tools-0.1.9/raster_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 fred      (1000) fred      (1000)     1797 2023-06-02 20:21:51.000000 raster-tools-0.1.9/raster_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 fred      (1000) fred      (1000)        1 2023-06-02 20:21:51.000000 raster-tools-0.1.9/raster_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 fred      (1000) fred      (1000)      139 2023-06-02 20:21:51.000000 raster-tools-0.1.9/raster_tools.egg-info/requires.txt
+-rw-rw-r--   0 fred      (1000) fred      (1000)       13 2023-06-02 20:21:51.000000 raster-tools-0.1.9/raster_tools.egg-info/top_level.txt
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2023-06-02 20:21:51.990378 raster-tools-0.1.9/requirements/
+-rw-rw-r--   0 fred      (1000) fred      (1000)      139 2023-01-25 21:30:15.000000 raster-tools-0.1.9/requirements/default.txt
+-rw-rw-r--   0 fred      (1000) fred      (1000)       38 2023-06-02 20:21:51.994378 raster-tools-0.1.9/setup.cfg
+-rw-rw-r--   0 fred      (1000) fred      (1000)     1526 2023-01-31 00:50:40.000000 raster-tools-0.1.9/setup.py
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2023-06-02 20:21:51.994378 raster-tools-0.1.9/tests/
+-rw-rw-r--   0 fred      (1000) fred      (1000)     4072 2023-01-04 22:54:46.000000 raster-tools-0.1.9/tests/test_clipping.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     4827 2023-05-01 20:54:28.000000 raster-tools-0.1.9/tests/test_creation.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     7404 2023-05-24 19:56:50.000000 raster-tools-0.1.9/tests/test_distance.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     1297 2022-08-26 20:44:16.000000 raster-tools-0.1.9/tests/test_distance__heap.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     8212 2023-04-14 00:09:55.000000 raster-tools-0.1.9/tests/test_distance_proximity.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    20233 2023-03-03 21:13:40.000000 raster-tools-0.1.9/tests/test_focal.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    30382 2023-06-02 20:12:17.000000 raster-tools-0.1.9/tests/test_general.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     7288 2023-01-28 03:48:27.000000 raster-tools-0.1.9/tests/test_line_stats.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    56760 2023-06-02 19:51:08.000000 raster-tools-0.1.9/tests/test_raster.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     4124 2022-08-26 20:44:16.000000 raster-tools-0.1.9/tests/test_stat_common.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     5157 2023-02-15 02:21:21.000000 raster-tools-0.1.9/tests/test_surface.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    10612 2023-05-11 21:16:13.000000 raster-tools-0.1.9/tests/test_vector.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     6903 2023-04-06 20:45:48.000000 raster-tools-0.1.9/tests/test_zonal.py
```

### Comparing `raster-tools-0.1.8/LICENSE` & `raster-tools-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.8/PKG-INFO` & `raster-tools-0.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raster-tools
-Version: 0.1.8
+Version: 0.1.9
 Summary: Tools for processing geospatial data
 Home-page: https://github.com/UM-RMRS/raster_tools
 License: GPL-3.0
 Project-URL: Bug Tracker, https://github.com/UM-RMRS/raster_tools/issues
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `raster-tools-0.1.8/README.md` & `raster-tools-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.8/raster_tools/__init__.py` & `raster-tools-0.1.9/raster_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.8/raster_tools/batch.py` & `raster-tools-0.1.9/raster_tools/batch.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.8/raster_tools/clipping.py` & `raster-tools-0.1.9/raster_tools/clipping.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.8/raster_tools/creation.py` & `raster-tools-0.1.9/raster_tools/creation.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.8/raster_tools/dask_utils.py` & `raster-tools-0.1.9/raster_tools/dask_utils.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.8/raster_tools/distance/_heap.py` & `raster-tools-0.1.9/raster_tools/distance/_heap.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.8/raster_tools/distance/cost_distance.py` & `raster-tools-0.1.9/raster_tools/distance/cost_distance.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.8/raster_tools/distance/proximity.py` & `raster-tools-0.1.9/raster_tools/distance/proximity.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.8/raster_tools/dtypes.py` & `raster-tools-0.1.9/raster_tools/dtypes.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.8/raster_tools/focal.py` & `raster-tools-0.1.9/raster_tools/focal.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.8/raster_tools/general.py` & `raster-tools-0.1.9/raster_tools/general.py`

 * *Files 0% similar despite different names*

```diff
@@ -965,15 +965,15 @@
     bands, rows, columns = x.shape
     rngs = mappings.shape[0]
     for bnd in range(bands):
         for rw in range(rows):
             for cl in range(columns):
                 if mask[bnd, rw, cl]:
                     continue
-                vl = int(x[bnd, rw, cl])
+                vl = x[bnd, rw, cl]
                 remap = False
                 for imap in range(rngs):
                     left, right, new = mappings[imap]
                     if inclusivity == 0:
                         remap = left <= vl < right
                     elif inclusivity == 1:
                         remap = left < vl <= right
```

### Comparing `raster-tools-0.1.8/raster_tools/io.py` & `raster-tools-0.1.9/raster_tools/io.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.8/raster_tools/line_stats.py` & `raster-tools-0.1.9/raster_tools/line_stats.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.8/raster_tools/masking.py` & `raster-tools-0.1.9/raster_tools/masking.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.8/raster_tools/raster.py` & `raster-tools-0.1.9/raster_tools/raster.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.8/raster_tools/stat_common.py` & `raster-tools-0.1.9/raster_tools/stat_common.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.8/raster_tools/surface.py` & `raster-tools-0.1.9/raster_tools/surface.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.8/raster_tools/utils.py` & `raster-tools-0.1.9/raster_tools/utils.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.8/raster_tools/vector.py` & `raster-tools-0.1.9/raster_tools/vector.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.8/raster_tools/zonal.py` & `raster-tools-0.1.9/raster_tools/zonal.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.8/raster_tools.egg-info/PKG-INFO` & `raster-tools-0.1.9/raster_tools.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raster-tools
-Version: 0.1.8
+Version: 0.1.9
 Summary: Tools for processing geospatial data
 Home-page: https://github.com/UM-RMRS/raster_tools
 License: GPL-3.0
 Project-URL: Bug Tracker, https://github.com/UM-RMRS/raster_tools/issues
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `raster-tools-0.1.8/raster_tools.egg-info/SOURCES.txt` & `raster-tools-0.1.9/raster_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.8/setup.py` & `raster-tools-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.8/tests/test_clipping.py` & `raster-tools-0.1.9/tests/test_clipping.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.8/tests/test_creation.py` & `raster-tools-0.1.9/tests/test_creation.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.8/tests/test_distance.py` & `raster-tools-0.1.9/tests/test_distance.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.8/tests/test_distance__heap.py` & `raster-tools-0.1.9/tests/test_distance__heap.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.8/tests/test_distance_proximity.py` & `raster-tools-0.1.9/tests/test_distance_proximity.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.8/tests/test_focal.py` & `raster-tools-0.1.9/tests/test_focal.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.8/tests/test_general.py` & `raster-tools-0.1.9/tests/test_general.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,25 @@
     binary_dilation,
     binary_erosion,
     grey_dilation,
     grey_erosion,
 )
 
 from raster_tools import creation, general
-from raster_tools.dtypes import F32, F64, I16, I32, I64, U8, U16, is_scalar
+from raster_tools.dtypes import (
+    F32,
+    F64,
+    I16,
+    I32,
+    I64,
+    U8,
+    U16,
+    get_common_dtype,
+    is_scalar,
+)
 from raster_tools.masking import get_default_null_value
 from raster_tools.raster import Raster, get_raster
 from raster_tools.stat_common import (
     nan_unique_count_jit,
     nanargmax_jit,
     nanargmin_jit,
     nanasm_jit,
@@ -599,48 +609,59 @@
 
 
 def test_band_concat_errors():
     with pytest.raises(ValueError):
         general.band_concat([])
 
 
-def test_remap_range():
-    rs = Raster(np.arange(25).reshape((5, 5)))
-    rsnp = rs.values
-
-    mapping = (0, 5, 1)
-    result = general.remap_range(rs, mapping)
-    truth = rsnp.copy()
-    truth[(rsnp >= mapping[0]) & (rsnp < mapping[1])] = mapping[2]
-    assert np.allclose(result, truth)
-    assert np.allclose(rs.remap_range(mapping), truth)
-
-    mappings = [mapping, (5, 15, -1)]
-    result = general.remap_range(rs, mappings)
-    truth[(rsnp >= mappings[1][0]) & (rsnp < mappings[1][1])] = mappings[1][2]
-    assert np.allclose(result, truth)
-    assert np.allclose(rs.remap_range(mappings), truth)
-
-    # Test multiple with potential conflict in last 2
-    mappings = [(0, 1, 0), (1, 2, 1), (2, 3, 8), (8, 9, 2)]
-    result = general.remap_range(rs, mappings)
-    truth = rsnp.copy()
-    for m in mappings:
-        truth[(rsnp >= m[0]) & (rsnp < m[1])] = m[2]
-    assert np.allclose(result.values, truth)
-    assert np.allclose(rs.remap_range(mappings), truth)
-
-    # Test precedence
-    mappings = [(0, 2, 0), (1, 2, 1)]
-    result = general.remap_range(rs, mappings)
-    truth = rsnp.copy()
-    m = mappings[0]
-    truth[(rsnp >= m[0]) & (rsnp < m[1])] = m[2]
-    assert np.allclose(result.values, truth)
-    assert np.allclose(rs.remap_range(mappings), truth)
+@pytest.mark.parametrize("inc", ["left", "right", "both", "none"])
+@pytest.mark.parametrize(
+    "raster,mapping",
+    [
+        (arange_raster((1, 5, 5)), (0, 5, 1)),
+        (arange_raster((1, 5, 5)), [(0, 5, 1), (5, 15, -1)]),
+        (
+            arange_raster((1, 5, 5)),
+            # Test multiple with potential conflict in last 2
+            [(0, 1, 0), (1, 2, 1), (2, 3, 8), (8, 9, 2)],
+        ),
+        # Test precedence
+        (arange_raster((1, 5, 5)), [(0, 2, 0), (1, 2, 1)]),
+        (arange_raster((1, 5, 5)) + 0.1, [(0, 2, 0), (1, 2, 1)]),
+    ],
+)
+def test_remap_range(raster, mapping, inc):
+    truth = raster.values
+    if np.asarray(mapping).shape == (3,):
+        mapping = [mapping]
+    out_dtype = get_common_dtype([m[-1] for m in mapping])
+    out_dtype = np.promote_types(raster.dtype, out_dtype)
+    truth = truth.astype(out_dtype)
+    remapped_mask = np.zeros_like(truth, dtype=bool)
+    for m in mapping:
+        if inc == "left":
+            match = (truth >= m[0]) & (truth < m[1])
+        elif inc == "right":
+            match = (truth > m[0]) & (truth <= m[1])
+        elif inc == "both":
+            match = (truth >= m[0]) & (truth <= m[1])
+        elif inc == "none":
+            match = (truth > m[0]) & (truth < m[1])
+        truth[(~remapped_mask) & match] = m[2]
+        remapped_mask |= match
+
+    result1 = general.remap_range(raster, mapping, inc)
+    result2 = raster.remap_range(mapping, inc)
+    assert_valid_raster(result1)
+    assert_valid_raster(result2)
+    assert result1.dtype == out_dtype
+    assert result2.dtype == out_dtype
+    assert np.allclose(result1, result2)
+    assert np.allclose(result1, truth)
+    assert np.allclose(result2, truth)
 
 
 @pytest.mark.parametrize(
     "rast,mapping",
     [
         (Raster(np.arange(16).reshape((4, 4))), [(0, 4, -1), (8, 12, 0)]),
         (
```

### Comparing `raster-tools-0.1.8/tests/test_line_stats.py` & `raster-tools-0.1.9/tests/test_line_stats.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.8/tests/test_raster.py` & `raster-tools-0.1.9/tests/test_raster.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.8/tests/test_stat_common.py` & `raster-tools-0.1.9/tests/test_stat_common.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.8/tests/test_surface.py` & `raster-tools-0.1.9/tests/test_surface.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.8/tests/test_vector.py` & `raster-tools-0.1.9/tests/test_vector.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.8/tests/test_zonal.py` & `raster-tools-0.1.9/tests/test_zonal.py`

 * *Files identical despite different names*

