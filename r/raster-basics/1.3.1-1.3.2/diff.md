# Comparing `tmp/raster_basics-1.3.1.tar.gz` & `tmp/raster_basics-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raster_basics-1.3.1.tar", last modified: Tue Jun 13 17:49:56 2023, max compression
+gzip compressed data, was "raster_basics-1.3.2.tar", last modified: Tue Jun 13 18:15:07 2023, max compression
```

## Comparing `raster_basics-1.3.1.tar` & `raster_basics-1.3.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 albinwells   (501) staff       (20)        0 2023-06-13 17:49:56.882289 raster_basics-1.3.1/
--rw-r--r--   0 albinwells   (501) staff       (20)      184 2023-06-13 17:49:56.882366 raster_basics-1.3.1/PKG-INFO
-drwxr-xr-x   0 albinwells   (501) staff       (20)        0 2023-06-13 17:49:56.881309 raster_basics-1.3.1/raster_basics/
--rw-rw-r--   0 albinwells   (501) staff       (20)     8661 2023-02-27 17:09:17.000000 raster_basics-1.3.1/raster_basics/BaseFunctions.py
--rw-rw-r--   0 albinwells   (501) staff       (20)    42097 2023-06-01 21:15:30.000000 raster_basics-1.3.1/raster_basics/DataPlots.py
--rw-rw-r--   0 albinwells   (501) staff       (20)    18564 2023-06-13 17:47:25.000000 raster_basics-1.3.1/raster_basics/GlacierFunctions.py
--rw-rw-r--   0 albinwells   (501) staff       (20)    12235 2023-03-23 16:41:47.000000 raster_basics-1.3.1/raster_basics/RasterBasics.py
--rwxrwxrwx   0 albinwells   (501) staff       (20)    12008 2023-06-06 14:10:42.000000 raster_basics-1.3.1/raster_basics/SmoothingFunctions.py
--rw-rw-r--   0 albinwells   (501) staff       (20)      574 2023-02-03 15:09:59.000000 raster_basics-1.3.1/raster_basics/__init__.py
-drwxr-xr-x   0 albinwells   (501) staff       (20)        0 2023-06-13 17:49:56.882179 raster_basics-1.3.1/raster_basics.egg-info/
--rw-r--r--   0 albinwells   (501) staff       (20)      184 2023-06-13 17:49:56.000000 raster_basics-1.3.1/raster_basics.egg-info/PKG-INFO
--rw-r--r--   0 albinwells   (501) staff       (20)      386 2023-06-13 17:49:56.000000 raster_basics-1.3.1/raster_basics.egg-info/SOURCES.txt
--rw-r--r--   0 albinwells   (501) staff       (20)        1 2023-06-13 17:49:56.000000 raster_basics-1.3.1/raster_basics.egg-info/dependency_links.txt
--rw-r--r--   0 albinwells   (501) staff       (20)        1 2023-06-13 17:49:56.000000 raster_basics-1.3.1/raster_basics.egg-info/not-zip-safe
--rw-r--r--   0 albinwells   (501) staff       (20)       14 2023-06-13 17:49:56.000000 raster_basics-1.3.1/raster_basics.egg-info/top_level.txt
--rw-rw-r--   0 albinwells   (501) staff       (20)       38 2023-06-13 17:49:56.882677 raster_basics-1.3.1/setup.cfg
--rw-rw-r--   0 albinwells   (501) staff       (20)      421 2023-06-13 17:46:02.000000 raster_basics-1.3.1/setup.py
+drwxr-xr-x   0 albinwells   (501) staff       (20)        0 2023-06-13 18:15:07.720164 raster_basics-1.3.2/
+-rw-r--r--   0 albinwells   (501) staff       (20)      184 2023-06-13 18:15:07.720254 raster_basics-1.3.2/PKG-INFO
+drwxr-xr-x   0 albinwells   (501) staff       (20)        0 2023-06-13 18:15:07.719103 raster_basics-1.3.2/raster_basics/
+-rw-rw-r--   0 albinwells   (501) staff       (20)     8661 2023-02-27 17:09:17.000000 raster_basics-1.3.2/raster_basics/BaseFunctions.py
+-rw-rw-r--   0 albinwells   (501) staff       (20)    42097 2023-06-01 21:15:30.000000 raster_basics-1.3.2/raster_basics/DataPlots.py
+-rw-rw-r--   0 albinwells   (501) staff       (20)    18564 2023-06-13 17:47:25.000000 raster_basics-1.3.2/raster_basics/GlacierFunctions.py
+-rw-rw-r--   0 albinwells   (501) staff       (20)    12235 2023-03-23 16:41:47.000000 raster_basics-1.3.2/raster_basics/RasterBasics.py
+-rwxrwxrwx   0 albinwells   (501) staff       (20)    12126 2023-06-13 18:14:16.000000 raster_basics-1.3.2/raster_basics/SmoothingFunctions.py
+-rw-rw-r--   0 albinwells   (501) staff       (20)      574 2023-02-03 15:09:59.000000 raster_basics-1.3.2/raster_basics/__init__.py
+drwxr-xr-x   0 albinwells   (501) staff       (20)        0 2023-06-13 18:15:07.720017 raster_basics-1.3.2/raster_basics.egg-info/
+-rw-r--r--   0 albinwells   (501) staff       (20)      184 2023-06-13 18:15:07.000000 raster_basics-1.3.2/raster_basics.egg-info/PKG-INFO
+-rw-r--r--   0 albinwells   (501) staff       (20)      386 2023-06-13 18:15:07.000000 raster_basics-1.3.2/raster_basics.egg-info/SOURCES.txt
+-rw-r--r--   0 albinwells   (501) staff       (20)        1 2023-06-13 18:15:07.000000 raster_basics-1.3.2/raster_basics.egg-info/dependency_links.txt
+-rw-r--r--   0 albinwells   (501) staff       (20)        1 2023-06-13 18:15:07.000000 raster_basics-1.3.2/raster_basics.egg-info/not-zip-safe
+-rw-r--r--   0 albinwells   (501) staff       (20)       14 2023-06-13 18:15:07.000000 raster_basics-1.3.2/raster_basics.egg-info/top_level.txt
+-rw-rw-r--   0 albinwells   (501) staff       (20)       38 2023-06-13 18:15:07.720600 raster_basics-1.3.2/setup.cfg
+-rw-rw-r--   0 albinwells   (501) staff       (20)      421 2023-06-13 18:14:32.000000 raster_basics-1.3.2/setup.py
```

### Comparing `raster_basics-1.3.1/raster_basics/BaseFunctions.py` & `raster_basics-1.3.2/raster_basics/BaseFunctions.py`

 * *Files identical despite different names*

### Comparing `raster_basics-1.3.1/raster_basics/DataPlots.py` & `raster_basics-1.3.2/raster_basics/DataPlots.py`

 * *Files identical despite different names*

### Comparing `raster_basics-1.3.1/raster_basics/GlacierFunctions.py` & `raster_basics-1.3.2/raster_basics/GlacierFunctions.py`

 * *Files identical despite different names*

### Comparing `raster_basics-1.3.1/raster_basics/RasterBasics.py` & `raster_basics-1.3.2/raster_basics/RasterBasics.py`

 * *Files identical despite different names*

### Comparing `raster_basics-1.3.1/raster_basics/SmoothingFunctions.py` & `raster_basics-1.3.2/raster_basics/SmoothingFunctions.py`

 * *Files 1% similar despite different names*

```diff
@@ -200,30 +200,32 @@
     
     orig_vals_mean = np.mean(orig_vals) # find the mean of all centerline values
     smooth_vals_mean = np.mean(smooth_vals)
     scaling = orig_vals_mean/smooth_vals_mean # scaling factor between smooth and raw data based on centerline mean
     smooth_data_scaled = rasterio.open(smooth_data).read(1)*scaling
     return smooth_data_scaled, scaling
     
-def distance_scaling_correction(data_vals1, data_vals2, distance, outline, polyfit_order=2, filter_std=None):
+def distance_scaling_correction(data_vals1, data_vals2, distance, outline=None, polyfit_order=2, filter_std=None):
     '''
     Correct smoothed data products based on a scaling from relative distance from centerline
     :param data_vals1: input array/data product 1, e.g. raw data (array-like)
     :param data_vals2: input data product 2--product to be corrected, e.g. smoothed data (array-like)
     :param distance: relative distance of every point from feature(s), e.g. centerlines (array-like)
-    :param outline: binary glacier outline array (array-like)
+    :param outline: Boolean glacier outline array (array-like)
     :param polyfit_order: order of the polynomial used to fit data, default 2 (int)
     :param filter_std: filtering outliers based on st.dev, default None (numeric)
     :return:
     '''
     x = distance.flatten()
     y_ratio = np.where(data_vals2 == 0, 1, data_vals1/data_vals2)
     # y_ratio = np.divide(data_vals1, data_vals2)
     y = y_ratio.flatten()
     
+    if outline is None:  # if no outline given, consider all array values
+    	outline = np.ones_like(distance)
     out = outline.flatten()
     y[out == 0] = -1
     x[out == 0] = -1
 
     # Filter outliers, if desired
     if filter_std != None:
         mean = np.nanmean(y)
```

### Comparing `raster_basics-1.3.1/raster_basics/__init__.py` & `raster_basics-1.3.2/raster_basics/__init__.py`

 * *Files identical despite different names*

