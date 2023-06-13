# Comparing `tmp/raster_basics-1.3.0.tar.gz` & `tmp/raster_basics-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raster_basics-1.3.0.tar", last modified: Tue Jun  6 14:11:21 2023, max compression
+gzip compressed data, was "raster_basics-1.3.1.tar", last modified: Tue Jun 13 17:49:56 2023, max compression
```

## Comparing `raster_basics-1.3.0.tar` & `raster_basics-1.3.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 albinwells   (501) staff       (20)        0 2023-06-06 14:11:21.015007 raster_basics-1.3.0/
--rw-r--r--   0 albinwells   (501) staff       (20)      184 2023-06-06 14:11:21.015071 raster_basics-1.3.0/PKG-INFO
-drwxr-xr-x   0 albinwells   (501) staff       (20)        0 2023-06-06 14:11:21.014164 raster_basics-1.3.0/raster_basics/
--rw-rw-r--   0 albinwells   (501) staff       (20)     8661 2023-02-27 17:09:17.000000 raster_basics-1.3.0/raster_basics/BaseFunctions.py
--rw-rw-r--   0 albinwells   (501) staff       (20)    42097 2023-06-01 21:15:30.000000 raster_basics-1.3.0/raster_basics/DataPlots.py
--rw-rw-r--   0 albinwells   (501) staff       (20)    17690 2023-06-02 17:27:11.000000 raster_basics-1.3.0/raster_basics/GlacierFunctions.py
--rw-rw-r--   0 albinwells   (501) staff       (20)    12235 2023-03-23 16:41:47.000000 raster_basics-1.3.0/raster_basics/RasterBasics.py
--rwxrwxrwx   0 albinwells   (501) staff       (20)    12008 2023-06-06 14:10:42.000000 raster_basics-1.3.0/raster_basics/SmoothingFunctions.py
--rw-rw-r--   0 albinwells   (501) staff       (20)      574 2023-02-03 15:09:59.000000 raster_basics-1.3.0/raster_basics/__init__.py
-drwxr-xr-x   0 albinwells   (501) staff       (20)        0 2023-06-06 14:11:21.014876 raster_basics-1.3.0/raster_basics.egg-info/
--rw-r--r--   0 albinwells   (501) staff       (20)      184 2023-06-06 14:11:20.000000 raster_basics-1.3.0/raster_basics.egg-info/PKG-INFO
--rw-r--r--   0 albinwells   (501) staff       (20)      386 2023-06-06 14:11:20.000000 raster_basics-1.3.0/raster_basics.egg-info/SOURCES.txt
--rw-r--r--   0 albinwells   (501) staff       (20)        1 2023-06-06 14:11:20.000000 raster_basics-1.3.0/raster_basics.egg-info/dependency_links.txt
--rw-r--r--   0 albinwells   (501) staff       (20)        1 2023-06-06 14:11:20.000000 raster_basics-1.3.0/raster_basics.egg-info/not-zip-safe
--rw-r--r--   0 albinwells   (501) staff       (20)       14 2023-06-06 14:11:20.000000 raster_basics-1.3.0/raster_basics.egg-info/top_level.txt
--rw-rw-r--   0 albinwells   (501) staff       (20)       38 2023-06-06 14:11:21.015323 raster_basics-1.3.0/setup.cfg
--rw-rw-r--   0 albinwells   (501) staff       (20)      421 2023-06-06 14:11:01.000000 raster_basics-1.3.0/setup.py
+drwxr-xr-x   0 albinwells   (501) staff       (20)        0 2023-06-13 17:49:56.882289 raster_basics-1.3.1/
+-rw-r--r--   0 albinwells   (501) staff       (20)      184 2023-06-13 17:49:56.882366 raster_basics-1.3.1/PKG-INFO
+drwxr-xr-x   0 albinwells   (501) staff       (20)        0 2023-06-13 17:49:56.881309 raster_basics-1.3.1/raster_basics/
+-rw-rw-r--   0 albinwells   (501) staff       (20)     8661 2023-02-27 17:09:17.000000 raster_basics-1.3.1/raster_basics/BaseFunctions.py
+-rw-rw-r--   0 albinwells   (501) staff       (20)    42097 2023-06-01 21:15:30.000000 raster_basics-1.3.1/raster_basics/DataPlots.py
+-rw-rw-r--   0 albinwells   (501) staff       (20)    18564 2023-06-13 17:47:25.000000 raster_basics-1.3.1/raster_basics/GlacierFunctions.py
+-rw-rw-r--   0 albinwells   (501) staff       (20)    12235 2023-03-23 16:41:47.000000 raster_basics-1.3.1/raster_basics/RasterBasics.py
+-rwxrwxrwx   0 albinwells   (501) staff       (20)    12008 2023-06-06 14:10:42.000000 raster_basics-1.3.1/raster_basics/SmoothingFunctions.py
+-rw-rw-r--   0 albinwells   (501) staff       (20)      574 2023-02-03 15:09:59.000000 raster_basics-1.3.1/raster_basics/__init__.py
+drwxr-xr-x   0 albinwells   (501) staff       (20)        0 2023-06-13 17:49:56.882179 raster_basics-1.3.1/raster_basics.egg-info/
+-rw-r--r--   0 albinwells   (501) staff       (20)      184 2023-06-13 17:49:56.000000 raster_basics-1.3.1/raster_basics.egg-info/PKG-INFO
+-rw-r--r--   0 albinwells   (501) staff       (20)      386 2023-06-13 17:49:56.000000 raster_basics-1.3.1/raster_basics.egg-info/SOURCES.txt
+-rw-r--r--   0 albinwells   (501) staff       (20)        1 2023-06-13 17:49:56.000000 raster_basics-1.3.1/raster_basics.egg-info/dependency_links.txt
+-rw-r--r--   0 albinwells   (501) staff       (20)        1 2023-06-13 17:49:56.000000 raster_basics-1.3.1/raster_basics.egg-info/not-zip-safe
+-rw-r--r--   0 albinwells   (501) staff       (20)       14 2023-06-13 17:49:56.000000 raster_basics-1.3.1/raster_basics.egg-info/top_level.txt
+-rw-rw-r--   0 albinwells   (501) staff       (20)       38 2023-06-13 17:49:56.882677 raster_basics-1.3.1/setup.cfg
+-rw-rw-r--   0 albinwells   (501) staff       (20)      421 2023-06-13 17:46:02.000000 raster_basics-1.3.1/setup.py
```

### Comparing `raster_basics-1.3.0/raster_basics/BaseFunctions.py` & `raster_basics-1.3.1/raster_basics/BaseFunctions.py`

 * *Files identical despite different names*

### Comparing `raster_basics-1.3.0/raster_basics/DataPlots.py` & `raster_basics-1.3.1/raster_basics/DataPlots.py`

 * *Files identical despite different names*

### Comparing `raster_basics-1.3.0/raster_basics/GlacierFunctions.py` & `raster_basics-1.3.1/raster_basics/GlacierFunctions.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import rasterio.mask
 import earthpy.spatial as es
 import richdem as rd
 import numpy as np
 import math
 import matplotlib.pyplot as plt
 from scipy import stats
+from scipy.ndimage import distance_transform_edt
 from shapely.geometry import Point
 from raster_basics.SmoothingFunctions import dynamicSmoothing, dynamicSmoothingExponential
 
 
 def glacierArea(outline, res):
     """
 	Area of a glacier
@@ -355,7 +356,24 @@
     ax.set_ylabel('Velocity Magnitude (In-Plane) (m/a)')
     ax.set_title(title, weight='bold')
     ax.set_xlim(left=0, right=driving_stress.max())
     ax.set_ylim(bottom=0, top=new_vel.max())
     plt.grid()
     plt.show(block=showPlot)
 
+
+def distance_from_line(line_array, res, mask=None):
+    '''
+    Calculate the Euclidean distance from centerline array
+    :param line_array: Boolean array input to calculate distance from. Distance is calculate from true values
+    :param res: Array Euclidean spacing (resoluion) -- numerical
+    :param mask: Boolean array mask for on/off glacier terrain (default None takes entire array as on-glacier)
+    :return: Array of distance values from line array  
+    '''
+    
+    if mask is None: # if not mask is input, we create a mask that includes all values in array
+        mask = np.ones_like(line_array) 
+        
+    distance_array = distance_transform_edt(np.logical_not(line_array), sampling=[res, res]) # calculate distance
+    distance_array[mask == 0] = 0 # remove off-glacier terrain
+    return distance_array
+
```

### Comparing `raster_basics-1.3.0/raster_basics/RasterBasics.py` & `raster_basics-1.3.1/raster_basics/RasterBasics.py`

 * *Files identical despite different names*

### Comparing `raster_basics-1.3.0/raster_basics/SmoothingFunctions.py` & `raster_basics-1.3.1/raster_basics/SmoothingFunctions.py`

 * *Files identical despite different names*

### Comparing `raster_basics-1.3.0/raster_basics/__init__.py` & `raster_basics-1.3.1/raster_basics/__init__.py`

 * *Files identical despite different names*

