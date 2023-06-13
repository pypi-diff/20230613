# Comparing `tmp/radvis-0.2.5.tar.gz` & `tmp/radvis-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radvis-0.2.5.tar", last modified: Mon Jun 12 06:27:57 2023, max compression
+gzip compressed data, was "radvis-0.3.0.tar", last modified: Tue Jun 13 14:24:36 2023, max compression
```

## Comparing `radvis-0.2.5.tar` & `radvis-0.3.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 06:27:57.253067 radvis-0.2.5/
--rw-rw-rw-   0        0        0     1089 2023-04-22 03:52:40.000000 radvis-0.2.5/LICENSE
--rw-rw-rw-   0        0        0     4135 2023-06-12 06:27:57.252067 radvis-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0     3834 2023-06-12 06:17:24.000000 radvis-0.2.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 06:27:57.197069 radvis-0.2.5/radvis/
--rw-rw-rw-   0        0        0      383 2023-06-12 06:26:15.000000 radvis-0.2.5/radvis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 06:27:57.226066 radvis-0.2.5/radvis/image/
--rw-rw-rw-   0        0        0      134 2023-06-12 06:10:13.000000 radvis-0.2.5/radvis/image/__init__.py
--rw-rw-rw-   0        0        0     1266 2023-06-12 06:17:42.000000 radvis-0.2.5/radvis/image/instantiate.py
--rw-rw-rw-   0        0        0     1345 2023-05-13 13:29:04.000000 radvis-0.2.5/radvis/image/rad_dicom_image.py
--rw-rw-rw-   0        0        0     4024 2023-06-12 06:12:48.000000 radvis-0.2.5/radvis/image/rad_image.py
--rw-rw-rw-   0        0        0     1408 2023-05-29 00:52:44.000000 radvis-0.2.5/radvis/image/rad_nifti_image.py
--rw-rw-rw-   0        0        0     1219 2023-06-12 06:17:56.000000 radvis-0.2.5/radvis/image/rad_numpy_image.py
-drwxrwxrwx   0        0        0        0 2023-06-12 06:27:57.232067 radvis-0.2.5/radvis/mesh/
--rw-rw-rw-   0        0        0      130 2023-05-29 03:00:11.000000 radvis-0.2.5/radvis/mesh/__init__.py
--rw-rw-rw-   0        0        0     1618 2023-05-29 03:00:19.000000 radvis-0.2.5/radvis/mesh/compute_mesh.py
--rw-rw-rw-   0        0        0     4074 2023-04-23 04:59:23.000000 radvis-0.2.5/radvis/mesh/rad_mesh.py
-drwxrwxrwx   0        0        0        0 2023-06-12 06:27:57.236068 radvis-0.2.5/radvis/processing/
--rw-rw-rw-   0        0        0      171 2023-05-29 03:20:54.000000 radvis-0.2.5/radvis/processing/__init__.py
--rw-rw-rw-   0        0        0     3165 2023-05-29 03:04:44.000000 radvis-0.2.5/radvis/processing/image.py
--rw-rw-rw-   0        0        0        0 2023-05-29 00:52:44.000000 radvis-0.2.5/radvis/processing/registration.py
-drwxrwxrwx   0        0        0        0 2023-06-12 06:27:57.239071 radvis-0.2.5/radvis/visualize/
--rw-rw-rw-   0        0        0      124 2023-05-29 00:52:44.000000 radvis-0.2.5/radvis/visualize/__init__.py
--rw-rw-rw-   0        0        0     9409 2023-06-05 03:35:02.000000 radvis-0.2.5/radvis/visualize/rad_slicer.py
--rw-rw-rw-   0        0        0     1857 2023-05-29 00:52:44.000000 radvis-0.2.5/radvis/visualize/rad_slicer_group.py
-drwxrwxrwx   0        0        0        0 2023-06-12 06:27:57.219068 radvis-0.2.5/radvis.egg-info/
--rw-rw-rw-   0        0        0     4135 2023-06-12 06:27:56.000000 radvis-0.2.5/radvis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      979 2023-06-12 06:27:57.000000 radvis-0.2.5/radvis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 06:27:56.000000 radvis-0.2.5/radvis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2023-06-12 06:27:56.000000 radvis-0.2.5/radvis.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-12 06:27:56.000000 radvis-0.2.5/radvis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-12 06:27:57.253067 radvis-0.2.5/setup.cfg
--rw-rw-rw-   0        0        0      669 2023-06-12 06:27:39.000000 radvis-0.2.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-12 06:27:57.240068 radvis-0.2.5/tests/
--rw-rw-rw-   0        0        0        0 2023-04-22 04:25:04.000000 radvis-0.2.5/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 06:27:57.242067 radvis-0.2.5/tests/mocks/
--rw-rw-rw-   0        0        0       40 2023-04-30 09:03:02.000000 radvis-0.2.5/tests/mocks/__init__.py
--rw-rw-rw-   0        0        0      455 2023-05-29 02:42:01.000000 radvis-0.2.5/tests/mocks/mock_rad_image.py
-drwxrwxrwx   0        0        0        0 2023-06-12 06:27:57.245067 radvis-0.2.5/tests/test_image/
--rw-rw-rw-   0        0        0        0 2023-06-12 06:14:11.000000 radvis-0.2.5/tests/test_image/__init__.py
--rw-rw-rw-   0        0        0      774 2023-06-12 06:18:24.000000 radvis-0.2.5/tests/test_image/test_instantiate.py
-drwxrwxrwx   0        0        0        0 2023-06-12 06:27:57.247067 radvis-0.2.5/tests/test_mesh/
--rw-rw-rw-   0        0        0        0 2023-04-23 02:35:32.000000 radvis-0.2.5/tests/test_mesh/__init__.py
--rw-rw-rw-   0        0        0     2248 2023-05-09 03:23:13.000000 radvis-0.2.5/tests/test_mesh/test_compute_mesh.py
-drwxrwxrwx   0        0        0        0 2023-06-12 06:27:57.249067 radvis-0.2.5/tests/test_processing/
--rw-rw-rw-   0        0        0        0 2023-05-29 02:40:16.000000 radvis-0.2.5/tests/test_processing/__init__.py
--rw-rw-rw-   0        0        0     1645 2023-05-29 02:59:47.000000 radvis-0.2.5/tests/test_processing/test_image.py
-drwxrwxrwx   0        0        0        0 2023-06-12 06:27:57.251067 radvis-0.2.5/tests/test_visualize/
--rw-rw-rw-   0        0        0        0 2023-04-30 08:55:21.000000 radvis-0.2.5/tests/test_visualize/__init__.py
--rw-rw-rw-   0        0        0      837 2023-05-29 02:59:35.000000 radvis-0.2.5/tests/test_visualize/test_rad_slicer.py
+drwxrwxrwx   0        0        0        0 2023-06-13 14:24:36.684312 radvis-0.3.0/
+-rw-rw-rw-   0        0        0     1089 2023-05-13 03:22:13.000000 radvis-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0     4739 2023-06-13 14:24:36.683316 radvis-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4438 2023-06-13 14:21:30.000000 radvis-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-13 14:24:36.625035 radvis-0.3.0/radvis/
+-rw-rw-rw-   0        0        0      383 2023-06-13 13:19:27.000000 radvis-0.3.0/radvis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 14:24:36.659380 radvis-0.3.0/radvis/image/
+-rw-rw-rw-   0        0        0      134 2023-06-13 13:19:27.000000 radvis-0.3.0/radvis/image/__init__.py
+-rw-rw-rw-   0        0        0     1266 2023-06-13 13:19:27.000000 radvis-0.3.0/radvis/image/instantiate.py
+-rw-rw-rw-   0        0        0     1345 2023-05-22 00:10:42.000000 radvis-0.3.0/radvis/image/rad_dicom_image.py
+-rw-rw-rw-   0        0        0     4024 2023-06-13 13:19:27.000000 radvis-0.3.0/radvis/image/rad_image.py
+-rw-rw-rw-   0        0        0     1408 2023-05-22 03:50:28.000000 radvis-0.3.0/radvis/image/rad_nifti_image.py
+-rw-rw-rw-   0        0        0     1219 2023-06-13 13:19:27.000000 radvis-0.3.0/radvis/image/rad_numpy_image.py
+drwxrwxrwx   0        0        0        0 2023-06-13 14:24:36.662370 radvis-0.3.0/radvis/mesh/
+-rw-rw-rw-   0        0        0      130 2023-06-13 13:19:27.000000 radvis-0.3.0/radvis/mesh/__init__.py
+-rw-rw-rw-   0        0        0     1618 2023-06-13 13:19:27.000000 radvis-0.3.0/radvis/mesh/compute_mesh.py
+-rw-rw-rw-   0        0        0     4074 2023-05-13 03:22:13.000000 radvis-0.3.0/radvis/mesh/rad_mesh.py
+drwxrwxrwx   0        0        0        0 2023-06-13 14:24:36.667386 radvis-0.3.0/radvis/processing/
+-rw-rw-rw-   0        0        0      171 2023-06-13 13:19:27.000000 radvis-0.3.0/radvis/processing/__init__.py
+-rw-rw-rw-   0        0        0     3165 2023-06-13 13:19:27.000000 radvis-0.3.0/radvis/processing/image.py
+-rw-rw-rw-   0        0        0        0 2023-06-13 13:19:27.000000 radvis-0.3.0/radvis/processing/registration.py
+drwxrwxrwx   0        0        0        0 2023-06-13 14:24:36.670350 radvis-0.3.0/radvis/visualize/
+-rw-rw-rw-   0        0        0      124 2023-05-22 02:27:22.000000 radvis-0.3.0/radvis/visualize/__init__.py
+-rw-rw-rw-   0        0        0    11339 2023-06-13 14:16:24.000000 radvis-0.3.0/radvis/visualize/rad_slicer.py
+-rw-rw-rw-   0        0        0     2351 2023-06-13 14:07:19.000000 radvis-0.3.0/radvis/visualize/rad_slicer_group.py
+drwxrwxrwx   0        0        0        0 2023-06-13 14:24:36.651399 radvis-0.3.0/radvis.egg-info/
+-rw-rw-rw-   0        0        0     4739 2023-06-13 14:24:36.000000 radvis-0.3.0/radvis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      979 2023-06-13 14:24:36.000000 radvis-0.3.0/radvis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 14:24:36.000000 radvis-0.3.0/radvis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2023-06-13 14:24:36.000000 radvis-0.3.0/radvis.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-13 14:24:36.000000 radvis-0.3.0/radvis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-13 14:24:36.684312 radvis-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      669 2023-06-13 14:22:51.000000 radvis-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 14:24:36.671346 radvis-0.3.0/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-13 03:22:13.000000 radvis-0.3.0/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 14:24:36.673341 radvis-0.3.0/tests/mocks/
+-rw-rw-rw-   0        0        0       40 2023-05-13 03:22:13.000000 radvis-0.3.0/tests/mocks/__init__.py
+-rw-rw-rw-   0        0        0      455 2023-06-13 13:19:27.000000 radvis-0.3.0/tests/mocks/mock_rad_image.py
+drwxrwxrwx   0        0        0        0 2023-06-13 14:24:36.675336 radvis-0.3.0/tests/test_image/
+-rw-rw-rw-   0        0        0        0 2023-06-13 13:19:27.000000 radvis-0.3.0/tests/test_image/__init__.py
+-rw-rw-rw-   0        0        0      774 2023-06-13 13:19:27.000000 radvis-0.3.0/tests/test_image/test_instantiate.py
+drwxrwxrwx   0        0        0        0 2023-06-13 14:24:36.678327 radvis-0.3.0/tests/test_mesh/
+-rw-rw-rw-   0        0        0        0 2023-05-13 03:22:13.000000 radvis-0.3.0/tests/test_mesh/__init__.py
+-rw-rw-rw-   0        0        0     2248 2023-05-13 03:22:13.000000 radvis-0.3.0/tests/test_mesh/test_compute_mesh.py
+drwxrwxrwx   0        0        0        0 2023-06-13 14:24:36.680322 radvis-0.3.0/tests/test_processing/
+-rw-rw-rw-   0        0        0        0 2023-06-13 13:19:27.000000 radvis-0.3.0/tests/test_processing/__init__.py
+-rw-rw-rw-   0        0        0     1645 2023-06-13 13:19:27.000000 radvis-0.3.0/tests/test_processing/test_image.py
+drwxrwxrwx   0        0        0        0 2023-06-13 14:24:36.682317 radvis-0.3.0/tests/test_visualize/
+-rw-rw-rw-   0        0        0        0 2023-05-13 03:22:13.000000 radvis-0.3.0/tests/test_visualize/__init__.py
+-rw-rw-rw-   0        0        0      837 2023-06-13 13:19:27.000000 radvis-0.3.0/tests/test_visualize/test_rad_slicer.py
```

### Comparing `radvis-0.2.5/LICENSE` & `radvis-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `radvis-0.2.5/PKG-INFO` & `radvis-0.3.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,9 @@
-Metadata-Version: 2.1
-Name: radvis
-Version: 0.2.5
-Summary: A visualization tool for medical images
-Home-page: https://github.com/medlee-code/RadVis
-Author: Matthew lee
-Author-email: matthewlee@medlee.io
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # RadVis
-RadVis (Radiology Visualization) is a visualization tool for medical images.
-
-Currently implemented features:
-- Load both DICOM and NIFTI images
-- Can display 2D slices of the 3D images
-- Ability to add a mask to the image
-- Works in both notebooks and scripts
+RadVis (Radiology Visualization) is a visualization tool for medical images. 
 
 ## Installation
 `pip install radvis`
 
 ## RadSlice Viewer
 
 Loading an image and displaying it with a slider
@@ -98,14 +81,39 @@
 ```
 
 <p float="left">
   <img src="https://raw.githubusercontent.com/medlee-code/RadVis/main/images/axis_1_brain_seg.gif?token=GHSAT0AAAAAACBJZC7PZ2WT3CJ26PONDN2YZC7T46Q" width="49%" /> 
   <img src="https://raw.githubusercontent.com/medlee-code/RadVis/main/images/axis_2_brain_seg.gif?token=GHSAT0AAAAAACBJZC7PDVRWL2CW2OCTUV3CZC7T5BQ" width="49%" />
 </p>
 
+You can also display multiple slicers at once
+```Python
+import radvis as rv
+import numpy as np
+
+img1 = rv.from_numpy(np.random.rand(50, 10, 10))
+img2 = rv.from_numpy(np.random.rand(10, 50, 10))
+img3 = rv.from_numpy(np.random.rand(10, 10, 50))
+img4 = rv.from_numpy(np.random.rand(50, 10, 10))
+img5 = rv.from_numpy(np.random.rand(10, 50, 10))
+img6 = rv.from_numpy(np.random.rand(10, 10, 50))
+
+rs1 = rv.RadSlicer(img1, title="Image 1")
+rs2 = rv.RadSlicer(img2, title="Image 2")
+rs3 = rv.RadSlicer(img3, title="Image 3")
+rs4 = rv.RadSlicer(img4, title="Image 4")
+rs5 = rv.RadSlicer(img5, title="Image 5")
+rs6 = rv.RadSlicer(img6, title="Image 6")
+
+rsg = rv.RadSlicerGroup([rs1, rs2, rs3, rs4, rs5, rs6], rows=2, cols=3)
+
+rsg.update_slider_heights(0.05)
+
+rsg.display()
+```
 ## Processing Module
 
 The processing module of RadVis offers a set of functions to perform preprocessing tasks
 
 ### Clipping
 The `percentile_clipping` function clips pixel intensities above and below percentile ranges
```

### Comparing `radvis-0.2.5/README.md` & `radvis-0.3.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,20 @@
-# RadVis
-RadVis (Radiology Visualization) is a visualization tool for medical images.
+Metadata-Version: 2.1
+Name: radvis
+Version: 0.3.0
+Summary: A visualization tool for medical images
+Home-page: https://github.com/medlee-code/RadVis
+Author: Matthew lee
+Author-email: matthewlee@medlee.io
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
 
-Currently implemented features:
-- Load both DICOM and NIFTI images
-- Can display 2D slices of the 3D images
-- Ability to add a mask to the image
-- Works in both notebooks and scripts
+# RadVis
+RadVis (Radiology Visualization) is a visualization tool for medical images. 
 
 ## Installation
 `pip install radvis`
 
 ## RadSlice Viewer
 
 Loading an image and displaying it with a slider
@@ -87,14 +92,39 @@
 ```
 
 <p float="left">
   <img src="https://raw.githubusercontent.com/medlee-code/RadVis/main/images/axis_1_brain_seg.gif?token=GHSAT0AAAAAACBJZC7PZ2WT3CJ26PONDN2YZC7T46Q" width="49%" /> 
   <img src="https://raw.githubusercontent.com/medlee-code/RadVis/main/images/axis_2_brain_seg.gif?token=GHSAT0AAAAAACBJZC7PDVRWL2CW2OCTUV3CZC7T5BQ" width="49%" />
 </p>
 
+You can also display multiple slicers at once
+```Python
+import radvis as rv
+import numpy as np
+
+img1 = rv.from_numpy(np.random.rand(50, 10, 10))
+img2 = rv.from_numpy(np.random.rand(10, 50, 10))
+img3 = rv.from_numpy(np.random.rand(10, 10, 50))
+img4 = rv.from_numpy(np.random.rand(50, 10, 10))
+img5 = rv.from_numpy(np.random.rand(10, 50, 10))
+img6 = rv.from_numpy(np.random.rand(10, 10, 50))
+
+rs1 = rv.RadSlicer(img1, title="Image 1")
+rs2 = rv.RadSlicer(img2, title="Image 2")
+rs3 = rv.RadSlicer(img3, title="Image 3")
+rs4 = rv.RadSlicer(img4, title="Image 4")
+rs5 = rv.RadSlicer(img5, title="Image 5")
+rs6 = rv.RadSlicer(img6, title="Image 6")
+
+rsg = rv.RadSlicerGroup([rs1, rs2, rs3, rs4, rs5, rs6], rows=2, cols=3)
+
+rsg.update_slider_heights(0.05)
+
+rsg.display()
+```
 ## Processing Module
 
 The processing module of RadVis offers a set of functions to perform preprocessing tasks
 
 ### Clipping
 The `percentile_clipping` function clips pixel intensities above and below percentile ranges
```

### Comparing `radvis-0.2.5/radvis/image/instantiate.py` & `radvis-0.3.0/radvis/image/instantiate.py`

 * *Files identical despite different names*

### Comparing `radvis-0.2.5/radvis/image/rad_dicom_image.py` & `radvis-0.3.0/radvis/image/rad_dicom_image.py`

 * *Files identical despite different names*

### Comparing `radvis-0.2.5/radvis/image/rad_image.py` & `radvis-0.3.0/radvis/image/rad_image.py`

 * *Files identical despite different names*

### Comparing `radvis-0.2.5/radvis/image/rad_nifti_image.py` & `radvis-0.3.0/radvis/image/rad_nifti_image.py`

 * *Files identical despite different names*

### Comparing `radvis-0.2.5/radvis/image/rad_numpy_image.py` & `radvis-0.3.0/radvis/image/rad_numpy_image.py`

 * *Files identical despite different names*

### Comparing `radvis-0.2.5/radvis/mesh/compute_mesh.py` & `radvis-0.3.0/radvis/mesh/compute_mesh.py`

 * *Files identical despite different names*

### Comparing `radvis-0.2.5/radvis/mesh/rad_mesh.py` & `radvis-0.3.0/radvis/mesh/rad_mesh.py`

 * *Files identical despite different names*

### Comparing `radvis-0.2.5/radvis/processing/image.py` & `radvis-0.3.0/radvis/processing/image.py`

 * *Files identical despite different names*

### Comparing `radvis-0.2.5/radvis/visualize/rad_slicer.py` & `radvis-0.3.0/radvis/visualize/rad_slicer.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,35 +12,45 @@
     from ipywidgets import interact, IntSlider
 except ImportError:
     print("Warning: ipywidgets not installed. RadSlicer will not work in Jupyter Notebook.")
 
 
 class RadSlicer:
     def __init__(self, radimage: RadImage, axis: int = 0, title=None, cmap: str = "gray",
-                 width:int=4, height:int=4, show_slider:bool = True) -> None:
+                 width:int=4, height:int=4, show_slider:bool = True, slider_height:float=0.05,
+                 slider_color:str='green', show_axis=True) -> None:
         """
         Initialize the RadSlicer class.
 
         :param radimage: A RadImage object containing the image data
         :param axis: The image axis to slice along, defaults to 0
         :param cmap: The colormap to use for displaying the image, defaults to "gray"
+        :param width: The width of the figure, defaults to 4
+        :param height: The height of the figure, defaults to 4
+        :param show_slider: Whether or not to show the slider, defaults to True
+        :param slider_height: The height of the slider, defaults to 0.03
+        :param slider_color: The color of the slider, defaults to 'blue'
+        :param show_axis: Whether or not to show the axis, defaults to True
         """
         self.radimage = radimage
         self.axis = axis
         self._title = title
         self._slider = None
         self._show_slider = show_slider
         self._image_plot = None
         self._mask_plots = []
         self._masks = []
         self._ax = None
         self._cmap = cmap
         self._figsize = (width, height)
         self._notebook_environment = IPython.get_ipython().__class__.__name__ == 'ZMQInteractiveShell'
         self._slider_coords = None
+        self._slider_height = slider_height
+        self._slider_color = slider_color
+        self._show_axis = show_axis
         
     @property
     def title(self):
         """
         Returns the title. If title is 'None' then returns the title 'Axis: {axis}'
         """
         if self._title is None:
@@ -64,14 +74,32 @@
     @property
     def figsize(self):
         """
         Returns the figure size.
         """
         return self._figsize
 
+    @property
+    def slider_height(self):
+        """
+        Returns the height of the slider.
+        """
+        return self._slider_height
+    
+    @slider_height.setter
+    def slider_height(self, value:float):
+        """
+        Sets the height of the slider.
+
+        :param value: The height of the slider
+        """
+        self._slider_height = value
+        if self._show_slider and self._slider is not None:
+            self._update_slider()
+    
     def remove_slider(self) -> None:
         """
         Remove the slider from the plot.
         """
         self._show_slider = False
         del self._slider
         self._slider = None
@@ -96,14 +124,26 @@
         image_slice = int(val)
         self._image_plot.set_data(self.radimage.get_slice(image_slice, self.axis))
         for plot, (mask, _, _) in zip(self._mask_plots, self._masks):
             plot.set_data(mask[image_slice, :, :] if self.axis == 0 else
                           mask[:, image_slice, :] if self.axis == 1 else
                           mask[:, :, image_slice])
         self.fig.canvas.draw_idle()
+    
+    def _calculate_slider_position(self, ax: plt.Axes) -> tuple[float, float, float, float]:
+        # Get the bounding box of the original axis
+        bbox = ax.get_position()
+
+        # Calculate the width, height, left, and bottom parameters for the slider
+        width = bbox.width
+        height = 0.02  # You can adjust this as needed
+        left = bbox.x0
+        bottom = bbox.y0 - self._slider_height  # Place slider below axis, with a small gap
+
+        return left, bottom, width, height
 
     def _create_slider(self, ax: plt.Axes, initial_index: int = 0) -> Slider|None:
         """
         Create a slider for the given plt.Axes object.
 
         :param ax: The plt.Axes object to add the slider to
         :param initial_index: The initial slice index, defaults to 0
@@ -113,28 +153,33 @@
             return None
         
         if self._notebook_environment:
             slider = interact(lambda val: self._update_image(val), 
                               val=IntSlider(min=0, max=self.radimage.shape[self.axis]-1, step=1, value=initial_index, 
                                             description=f"{self.title}: Slice"))
         else:
-            ax_position = ax.get_position()
-            slider_width = ax_position.width - 0.2
-            slider_height = 0.03
-            slider_x = ax_position.x0 + 0.1
-            slider_y = ax_position.y0 - 0.15
-            
-            if self._slider_coords is not None:
-                slider_x, slider_y, slider_width, slider_height = self._slider_coords
-                
+            slider_x, slider_y, slider_width, slider_height = self._calculate_slider_position(ax)
             ax_slider = plt.axes([slider_x, slider_y, slider_width, slider_height])
             slider = Slider(ax_slider, f"Slice", 0, self.radimage.shape[self.axis] - 1, valstep=1, valfmt="%d",
-                                valinit=initial_index)
+                                valinit=initial_index, color=self._slider_color)
             slider.on_changed(self._update_image)
         return slider
+
+    def _update_slider(self, initial_index: int = 0) -> None:
+        """
+        Removes the old slider and updates with a new slider
+
+        :param initial_index: The initial slice index, defaults to 0
+        """
+        if self._slider is not None:
+            self._slider.ax.remove()
+            self._slider = None
+        self._slider = self._create_slider(self._ax, initial_index)
+        if self._slider is not None:
+            self.fig.canvas.draw()
     
     def _plot_image(self, ax: plt.Axes, initial_index: int = 0) -> None:
         """
         Plot the image on the given plt.Axes object and create a slider for it.
 
         :param ax: The plt.Axes object to plot the image on
         :param initial_index: The initial slice index, defaults to 0
@@ -142,22 +187,27 @@
         self._image_plot = ax.imshow(
             self.radimage.get_slice(initial_index, self.axis), 
             cmap=self._cmap,
             vmin=self.radimage.image_data.min(),
             vmax=self.radimage.image_data.max(),
             interpolation='none'
         )
+
+        if self._show_axis:
+            ax.axis('on')
+        else:
+            ax.axis('off')
+
         for mask, cmap, alpha in self._masks:
             mask_plot = ax.imshow(mask[initial_index, :, :] if self.axis == 0 else
                       mask[:, initial_index, :] if self.axis == 1 else
                       mask[:, :, initial_index],
                       cmap=cmap, interpolation='none', alpha=alpha,
                       vmin=0, vmax=mask.max())
             self._mask_plots.append(mask_plot)
-        self._slider = self._create_slider(ax, initial_index)
 
 
     def display(self, ax: plt.Axes = None, initial_index: int = 0, show_plot=True) -> None:
         """
         Display the RadSlicer plot with a slider to control the displayed slice.
         """
         if len(self.radimage.shape) != 3:
@@ -168,16 +218,17 @@
             plt.subplots_adjust(bottom=0.2)
         else:
             self._ax = ax
             self.fig = ax.get_figure()
                
         self._ax.set_title(self.title, y=1)
         self.fig.set_size_inches(self._figsize[0], self._figsize[1], forward=False)
-        
+        self._update_slider(initial_index)
         self._plot_image(self._ax, initial_index)
+
         
         if show_plot:
             plt.show()
 
     def add_mask(self, mask: np.ndarray | RadImage, color: str | Colormap = 'red', alpha: float = 0.5):
         """
         Adds a mask to the RadSlicer.
```

### Comparing `radvis-0.2.5/radvis/visualize/rad_slicer_group.py` & `radvis-0.3.0/radvis/visualize/rad_slicer_group.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from radvis.visualize.rad_slicer import RadSlicer
 import matplotlib.pyplot as plt
 from matplotlib.widgets import Slider
 
 
 class RadSlicerGroup:
-    def __init__(self, radslicers: list[RadSlicer], rows: int, cols: int) -> None:
+    def __init__(self, radslicers: list[RadSlicer], rows: int, cols: int = 1) -> None:
         """
         Initialize the RadSlicerGroup class.
 
         :param radslicers: A list of RadSlicer objects
         :param rows: The number of rows to display the RadSlicers in
         :param cols: The number of columns to display the RadSlicers in
         """
         self.radslicers = radslicers
         self.rows = rows
         self.cols = cols
         self._verify_dimensions()
+        self.fig, self.axes = plt.subplots(self.rows, self.cols, figsize=(self._get_figure_width(), self._get_figure_height()))
 
     def _verify_dimensions(self) -> None:
         """
         Verifies the provided rows and columns are valid for the number of RadSlicers.
         """
         if self.rows * self.cols != len(self.radslicers):
             raise ValueError(f"Number of RadSlicers ({len(self.radslicers)}) does not match provided grid dimensions ({self.rows}x{self.cols}).")
@@ -32,19 +33,33 @@
     
     def _get_figure_height(self) -> int:
         """
         Returns the height of the figure.
         """
         return self.rows * sum([rs.height for rs in self.radslicers])
     
+    def _update_image(self, val:int):
+        """
+        Updates each RadSlider for the provided image
+        """ 
+        for radslicer in self.radslicers:
+            radslicer._update_image(val)
+    
+    def update_slider_heights(self, height: float) -> None:
+        """
+        Updates the height of the slider for each RadSlicer.
+
+        :param height: The height of the slider
+        """
+        for radslicer in self.radslicers:
+            radslicer.slider_height = height
+
     def display(self, initial_index: int = 0) -> None:
         """
         Display the RadSlicers in a grid.
         """
-        fig, axes = plt.subplots(self.rows, self.cols, figsize=(self._get_figure_width(), self._get_figure_height()))
-        axes = axes.flatten()
+        axes = self.axes.flatten()
 
-        for i, (radslicer, ax) in enumerate(zip(self.radslicers, axes)):
+        for _, (radslicer, ax) in enumerate(zip(self.radslicers, axes)):
             radslicer.display(ax=ax, initial_index=initial_index, show_plot=False)
 
-        plt.tight_layout()
         plt.show()
```

### Comparing `radvis-0.2.5/radvis.egg-info/PKG-INFO` & `radvis-0.3.0/radvis.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,20 @@
 Metadata-Version: 2.1
 Name: radvis
-Version: 0.2.5
+Version: 0.3.0
 Summary: A visualization tool for medical images
 Home-page: https://github.com/medlee-code/RadVis
 Author: Matthew lee
 Author-email: matthewlee@medlee.io
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # RadVis
-RadVis (Radiology Visualization) is a visualization tool for medical images.
-
-Currently implemented features:
-- Load both DICOM and NIFTI images
-- Can display 2D slices of the 3D images
-- Ability to add a mask to the image
-- Works in both notebooks and scripts
+RadVis (Radiology Visualization) is a visualization tool for medical images. 
 
 ## Installation
 `pip install radvis`
 
 ## RadSlice Viewer
 
 Loading an image and displaying it with a slider
@@ -98,14 +92,39 @@
 ```
 
 <p float="left">
   <img src="https://raw.githubusercontent.com/medlee-code/RadVis/main/images/axis_1_brain_seg.gif?token=GHSAT0AAAAAACBJZC7PZ2WT3CJ26PONDN2YZC7T46Q" width="49%" /> 
   <img src="https://raw.githubusercontent.com/medlee-code/RadVis/main/images/axis_2_brain_seg.gif?token=GHSAT0AAAAAACBJZC7PDVRWL2CW2OCTUV3CZC7T5BQ" width="49%" />
 </p>
 
+You can also display multiple slicers at once
+```Python
+import radvis as rv
+import numpy as np
+
+img1 = rv.from_numpy(np.random.rand(50, 10, 10))
+img2 = rv.from_numpy(np.random.rand(10, 50, 10))
+img3 = rv.from_numpy(np.random.rand(10, 10, 50))
+img4 = rv.from_numpy(np.random.rand(50, 10, 10))
+img5 = rv.from_numpy(np.random.rand(10, 50, 10))
+img6 = rv.from_numpy(np.random.rand(10, 10, 50))
+
+rs1 = rv.RadSlicer(img1, title="Image 1")
+rs2 = rv.RadSlicer(img2, title="Image 2")
+rs3 = rv.RadSlicer(img3, title="Image 3")
+rs4 = rv.RadSlicer(img4, title="Image 4")
+rs5 = rv.RadSlicer(img5, title="Image 5")
+rs6 = rv.RadSlicer(img6, title="Image 6")
+
+rsg = rv.RadSlicerGroup([rs1, rs2, rs3, rs4, rs5, rs6], rows=2, cols=3)
+
+rsg.update_slider_heights(0.05)
+
+rsg.display()
+```
 ## Processing Module
 
 The processing module of RadVis offers a set of functions to perform preprocessing tasks
 
 ### Clipping
 The `percentile_clipping` function clips pixel intensities above and below percentile ranges
```

### Comparing `radvis-0.2.5/radvis.egg-info/SOURCES.txt` & `radvis-0.3.0/radvis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `radvis-0.2.5/setup.py` & `radvis-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='radvis',
-    version='0.2.5',
+    version='0.3.0',
     url='https://github.com/medlee-code/RadVis',
     author='Matthew lee',
     author_email='matthewlee@medlee.io',
     description='A visualization tool for medical images',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
```

### Comparing `radvis-0.2.5/tests/test_image/test_instantiate.py` & `radvis-0.3.0/tests/test_image/test_instantiate.py`

 * *Files identical despite different names*

### Comparing `radvis-0.2.5/tests/test_mesh/test_compute_mesh.py` & `radvis-0.3.0/tests/test_mesh/test_compute_mesh.py`

 * *Files identical despite different names*

### Comparing `radvis-0.2.5/tests/test_processing/test_image.py` & `radvis-0.3.0/tests/test_processing/test_image.py`

 * *Files identical despite different names*

### Comparing `radvis-0.2.5/tests/test_visualize/test_rad_slicer.py` & `radvis-0.3.0/tests/test_visualize/test_rad_slicer.py`

 * *Files identical despite different names*

