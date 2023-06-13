# Comparing `tmp/orange-earth-observation-1.0.2.tar.gz` & `tmp/orange-earth-observation-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orange-earth-observation-1.0.2.tar", last modified: Wed Jun  7 11:56:38 2023, max compression
+gzip compressed data, was "orange-earth-observation-1.1.0.tar", last modified: Tue Jun 13 07:41:27 2023, max compression
```

## Comparing `orange-earth-observation-1.0.2.tar` & `orange-earth-observation-1.1.0.tar`

### file list

```diff
@@ -1,45 +1,52 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 11:56:38.562532 orange-earth-observation-1.0.2/
--rw-rw-rw-   0 root         (0) root         (0)       56 2023-05-10 16:10:17.000000 orange-earth-observation-1.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6147 2023-06-07 11:56:38.562532 orange-earth-observation-1.0.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5640 2023-06-07 11:53:04.000000 orange-earth-observation-1.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 11:56:38.558532 orange-earth-observation-1.0.2/orange_earth_observation.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6147 2023-06-07 11:56:38.000000 orange-earth-observation-1.0.2/orange_earth_observation.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1729 2023-06-07 11:56:38.000000 orange-earth-observation-1.0.2/orange_earth_observation.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 11:56:38.000000 orange-earth-observation-1.0.2/orange_earth_observation.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      146 2023-06-07 11:56:38.000000 orange-earth-observation-1.0.2/orange_earth_observation.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-06-07 11:56:38.000000 orange-earth-observation-1.0.2/orange_earth_observation.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 11:56:38.000000 orange-earth-observation-1.0.2/orange_earth_observation.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      227 2023-06-07 11:56:38.000000 orange-earth-observation-1.0.2/orange_earth_observation.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-06-07 11:56:38.000000 orange-earth-observation-1.0.2/orange_earth_observation.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 11:56:38.554531 orange-earth-observation-1.0.2/orangecontrib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 11:56:38.566532 orange-earth-observation-1.0.2/orangecontrib/earth_observation/
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-05-10 16:10:17.000000 orange-earth-observation-1.0.2/orangecontrib/earth_observation/__init__.py
--rw-r--r--   0 root         (0) root         (0)      497 2023-06-07 11:56:38.566532 orange-earth-observation-1.0.2/orangecontrib/earth_observation/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 11:56:38.558532 orange-earth-observation-1.0.2/orangecontrib/earth_observation/widgets/
--rw-rw-rw-   0 root         (0) root         (0)      200 2023-05-10 16:10:17.000000 orange-earth-observation-1.0.2/orangecontrib/earth_observation/widgets/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    19663 2023-06-07 11:53:04.000000 orange-earth-observation-1.0.2/orangecontrib/earth_observation/widgets/catalog.py
--rw-rw-rw-   0 root         (0) root         (0)     5211 2023-05-10 16:10:17.000000 orange-earth-observation-1.0.2/orangecontrib/earth_observation/widgets/cloud_mask.py
--rw-rw-rw-   0 root         (0) root         (0)     8284 2023-05-10 16:10:17.000000 orange-earth-observation-1.0.2/orangecontrib/earth_observation/widgets/crop_image.py
--rw-rw-rw-   0 root         (0) root         (0)    10887 2023-05-10 16:10:17.000000 orange-earth-observation-1.0.2/orangecontrib/earth_observation/widgets/histogram.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 11:56:38.562532 orange-earth-observation-1.0.2/orangecontrib/earth_observation/widgets/icons/
--rw-rw-rw-   0 root         (0) root         (0)     1003 2023-05-10 16:10:17.000000 orange-earth-observation-1.0.2/orangecontrib/earth_observation/widgets/icons/catalog.svg
--rw-rw-rw-   0 root         (0) root         (0)     6968 2023-05-10 16:10:17.000000 orange-earth-observation-1.0.2/orangecontrib/earth_observation/widgets/icons/category.svg
--rw-rw-rw-   0 root         (0) root         (0)     1239 2023-05-10 16:10:17.000000 orange-earth-observation-1.0.2/orangecontrib/earth_observation/widgets/icons/cloud.svg
--rw-rw-rw-   0 root         (0) root         (0)     1368 2023-05-10 16:10:17.000000 orange-earth-observation-1.0.2/orangecontrib/earth_observation/widgets/icons/crop.svg
--rw-rw-rw-   0 root         (0) root         (0)      258 2023-05-10 16:10:17.000000 orange-earth-observation-1.0.2/orangecontrib/earth_observation/widgets/icons/histogram.svg
--rw-rw-rw-   0 root         (0) root         (0)      924 2023-05-10 16:10:17.000000 orange-earth-observation-1.0.2/orangecontrib/earth_observation/widgets/icons/load.svg
--rw-rw-rw-   0 root         (0) root         (0)     1192 2023-05-10 16:10:17.000000 orange-earth-observation-1.0.2/orangecontrib/earth_observation/widgets/icons/mosaic.svg
--rw-rw-rw-   0 root         (0) root         (0)      323 2023-05-10 16:10:17.000000 orange-earth-observation-1.0.2/orangecontrib/earth_observation/widgets/icons/nuts.svg
--rw-rw-rw-   0 root         (0) root         (0)     2467 2023-05-10 16:10:17.000000 orange-earth-observation-1.0.2/orangecontrib/earth_observation/widgets/icons/projection.svg
--rw-rw-rw-   0 root         (0) root         (0)     2492 2023-05-10 16:10:17.000000 orange-earth-observation-1.0.2/orangecontrib/earth_observation/widgets/icons/view.svg
--rw-rw-rw-   0 root         (0) root         (0)     4100 2023-05-26 08:49:08.000000 orange-earth-observation-1.0.2/orangecontrib/earth_observation/widgets/load_image.py
--rw-rw-rw-   0 root         (0) root         (0)     4427 2023-05-10 16:10:17.000000 orange-earth-observation-1.0.2/orangecontrib/earth_observation/widgets/mosaic_image.py
--rw-rw-rw-   0 root         (0) root         (0)     7523 2023-05-10 16:10:17.000000 orange-earth-observation-1.0.2/orangecontrib/earth_observation/widgets/nuts_shape.py
--rw-rw-rw-   0 root         (0) root         (0)     4092 2023-05-10 16:10:17.000000 orange-earth-observation-1.0.2/orangecontrib/earth_observation/widgets/reproject_image.py
--rw-rw-rw-   0 root         (0) root         (0)      252 2023-05-10 16:10:17.000000 orange-earth-observation-1.0.2/orangecontrib/earth_observation/widgets/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     4255 2023-06-07 11:53:04.000000 orange-earth-observation-1.0.2/orangecontrib/earth_observation/widgets/view_image.py
--rw-rw-rw-   0 root         (0) root         (0)      101 2023-05-10 16:10:17.000000 orange-earth-observation-1.0.2/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      229 2023-06-07 11:53:04.000000 orange-earth-observation-1.0.2/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)     1212 2023-06-07 11:56:38.562532 orange-earth-observation-1.0.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      124 2023-05-10 16:10:17.000000 orange-earth-observation-1.0.2/setup.py
--rw-rw-rw-   0 root         (0) root         (0)    83021 2023-05-10 16:10:17.000000 orange-earth-observation-1.0.2/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 07:41:27.677033 orange-earth-observation-1.1.0/
+-rw-rw-rw-   0 root         (0) root         (0)       56 2023-05-10 16:10:17.000000 orange-earth-observation-1.1.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6147 2023-06-13 07:41:27.677033 orange-earth-observation-1.1.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5640 2023-06-12 15:57:10.000000 orange-earth-observation-1.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 07:41:27.669032 orange-earth-observation-1.1.0/orange_earth_observation.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6147 2023-06-13 07:41:27.000000 orange-earth-observation-1.1.0/orange_earth_observation.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2133 2023-06-13 07:41:27.000000 orange-earth-observation-1.1.0/orange_earth_observation.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 07:41:27.000000 orange-earth-observation-1.1.0/orange_earth_observation.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      146 2023-06-13 07:41:27.000000 orange-earth-observation-1.1.0/orange_earth_observation.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-06-13 07:41:27.000000 orange-earth-observation-1.1.0/orange_earth_observation.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 07:41:27.000000 orange-earth-observation-1.1.0/orange_earth_observation.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      249 2023-06-13 07:41:27.000000 orange-earth-observation-1.1.0/orange_earth_observation.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-06-13 07:41:27.000000 orange-earth-observation-1.1.0/orange_earth_observation.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 07:41:27.661032 orange-earth-observation-1.1.0/orangecontrib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 07:41:27.681033 orange-earth-observation-1.1.0/orangecontrib/earth_observation/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-05-10 16:10:17.000000 orange-earth-observation-1.1.0/orangecontrib/earth_observation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      497 2023-06-13 07:41:27.681033 orange-earth-observation-1.1.0/orangecontrib/earth_observation/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 07:41:27.673032 orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/
+-rw-rw-rw-   0 root         (0) root         (0)      200 2023-05-10 16:10:17.000000 orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    21262 2023-06-12 15:57:10.000000 orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/catalog.py
+-rw-rw-rw-   0 root         (0) root         (0)     5211 2023-05-10 16:10:17.000000 orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/cloud_mask.py
+-rw-rw-rw-   0 root         (0) root         (0)     8284 2023-05-10 16:10:17.000000 orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/crop_image.py
+-rw-rw-rw-   0 root         (0) root         (0)     7648 2023-06-12 15:57:10.000000 orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/geoserver.py
+-rw-rw-rw-   0 root         (0) root         (0)    10887 2023-05-10 16:10:17.000000 orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/histogram.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 07:41:27.677033 orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/icons/
+-rw-rw-rw-   0 root         (0) root         (0)     6582 2023-06-12 15:57:10.000000 orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/icons/calculate.svg
+-rw-rw-rw-   0 root         (0) root         (0)     1003 2023-05-10 16:10:17.000000 orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/icons/catalog.svg
+-rw-rw-rw-   0 root         (0) root         (0)     6968 2023-05-10 16:10:17.000000 orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/icons/category.svg
+-rw-rw-rw-   0 root         (0) root         (0)     1239 2023-05-10 16:10:17.000000 orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/icons/cloud.svg
+-rw-rw-rw-   0 root         (0) root         (0)     1368 2023-05-10 16:10:17.000000 orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/icons/crop.svg
+-rw-rw-rw-   0 root         (0) root         (0)      872 2023-06-12 15:57:10.000000 orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/icons/geoserver.svg
+-rw-rw-rw-   0 root         (0) root         (0)      258 2023-05-10 16:10:17.000000 orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/icons/histogram.svg
+-rw-rw-rw-   0 root         (0) root         (0)      924 2023-05-10 16:10:17.000000 orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/icons/load.svg
+-rw-rw-rw-   0 root         (0) root         (0)     2115 2023-06-12 15:57:10.000000 orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/icons/manifest.svg
+-rw-rw-rw-   0 root         (0) root         (0)     1192 2023-05-10 16:10:17.000000 orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/icons/mosaic.svg
+-rw-rw-rw-   0 root         (0) root         (0)      323 2023-05-10 16:10:17.000000 orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/icons/nuts.svg
+-rw-rw-rw-   0 root         (0) root         (0)     2467 2023-05-10 16:10:17.000000 orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/icons/projection.svg
+-rw-rw-rw-   0 root         (0) root         (0)     2492 2023-05-10 16:10:17.000000 orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/icons/view.svg
+-rw-rw-rw-   0 root         (0) root         (0)     6294 2023-06-12 15:57:10.000000 orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/index_calculation.py
+-rw-rw-rw-   0 root         (0) root         (0)     4100 2023-05-26 08:49:08.000000 orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/load_image.py
+-rw-rw-rw-   0 root         (0) root         (0)     3587 2023-06-12 15:57:10.000000 orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/manifest.py
+-rw-rw-rw-   0 root         (0) root         (0)     4427 2023-05-10 16:10:17.000000 orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/mosaic_image.py
+-rw-rw-rw-   0 root         (0) root         (0)     7523 2023-05-10 16:10:17.000000 orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/nuts_shape.py
+-rw-rw-rw-   0 root         (0) root         (0)     4092 2023-05-10 16:10:17.000000 orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/reproject_image.py
+-rw-rw-rw-   0 root         (0) root         (0)     7269 2023-06-12 15:57:10.000000 orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/rgb_calculation.py
+-rw-rw-rw-   0 root         (0) root         (0)      252 2023-05-10 16:10:17.000000 orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     4938 2023-06-12 15:57:10.000000 orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/view_image.py
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-05-10 16:10:17.000000 orange-earth-observation-1.1.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      249 2023-06-12 15:57:10.000000 orange-earth-observation-1.1.0/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1212 2023-06-13 07:41:27.681033 orange-earth-observation-1.1.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      124 2023-05-10 16:10:17.000000 orange-earth-observation-1.1.0/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)    83021 2023-05-10 16:10:17.000000 orange-earth-observation-1.1.0/versioneer.py
```

### Comparing `orange-earth-observation-1.0.2/PKG-INFO` & `orange-earth-observation-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orange-earth-observation
-Version: 1.0.2
+Version: 1.1.0
 Summary: Add-on containing widgets for earth observation data operations
 Home-page: https://gitlab.com/drb-python/samples/odm/eo_addon
 Author: GAEL Systems
 Author-email: drb-python@gael.fr
 License: LGPLv3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Environment :: Plugins
```

### Comparing `orange-earth-observation-1.0.2/README.md` & `orange-earth-observation-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `orange-earth-observation-1.0.2/orange_earth_observation.egg-info/PKG-INFO` & `orange-earth-observation-1.1.0/orange_earth_observation.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orange-earth-observation
-Version: 1.0.2
+Version: 1.1.0
 Summary: Add-on containing widgets for earth observation data operations
 Home-page: https://gitlab.com/drb-python/samples/odm/eo_addon
 Author: GAEL Systems
 Author-email: drb-python@gael.fr
 License: LGPLv3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Environment :: Plugins
```

### Comparing `orange-earth-observation-1.0.2/orange_earth_observation.egg-info/SOURCES.txt` & `orange-earth-observation-1.1.0/orange_earth_observation.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -15,24 +15,31 @@
 orange_earth_observation.egg-info/top_level.txt
 orangecontrib/earth_observation/__init__.py
 orangecontrib/earth_observation/_version.py
 orangecontrib/earth_observation/widgets/__init__.py
 orangecontrib/earth_observation/widgets/catalog.py
 orangecontrib/earth_observation/widgets/cloud_mask.py
 orangecontrib/earth_observation/widgets/crop_image.py
+orangecontrib/earth_observation/widgets/geoserver.py
 orangecontrib/earth_observation/widgets/histogram.py
+orangecontrib/earth_observation/widgets/index_calculation.py
 orangecontrib/earth_observation/widgets/load_image.py
+orangecontrib/earth_observation/widgets/manifest.py
 orangecontrib/earth_observation/widgets/mosaic_image.py
 orangecontrib/earth_observation/widgets/nuts_shape.py
 orangecontrib/earth_observation/widgets/reproject_image.py
+orangecontrib/earth_observation/widgets/rgb_calculation.py
 orangecontrib/earth_observation/widgets/utils.py
 orangecontrib/earth_observation/widgets/view_image.py
+orangecontrib/earth_observation/widgets/icons/calculate.svg
 orangecontrib/earth_observation/widgets/icons/catalog.svg
 orangecontrib/earth_observation/widgets/icons/category.svg
 orangecontrib/earth_observation/widgets/icons/cloud.svg
 orangecontrib/earth_observation/widgets/icons/crop.svg
+orangecontrib/earth_observation/widgets/icons/geoserver.svg
 orangecontrib/earth_observation/widgets/icons/histogram.svg
 orangecontrib/earth_observation/widgets/icons/load.svg
+orangecontrib/earth_observation/widgets/icons/manifest.svg
 orangecontrib/earth_observation/widgets/icons/mosaic.svg
 orangecontrib/earth_observation/widgets/icons/nuts.svg
 orangecontrib/earth_observation/widgets/icons/projection.svg
 orangecontrib/earth_observation/widgets/icons/view.svg
```

### Comparing `orange-earth-observation-1.0.2/orangecontrib/earth_observation/widgets/catalog.py` & `orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/catalog.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 import io
 from Orange.widgets import widget, gui, settings
 from Orange.widgets.utils.signals import Output
 from PyQt5.QtCore import Qt, QDate
 from PyQt5.QtGui import QPalette, QColor, QTextCharFormat
 from PyQt5.QtWidgets import QAction, QPushButton, \
     QFileDialog, QCalendarWidget, QHBoxLayout
@@ -75,37 +76,40 @@
 class OWDataCatalog(widget.OWWidget):
     name = "EO Data Catalog"
     description = "Access and retrieve data from " \
                   "different services using Odata protocol"
     icon = "icons/catalog.svg"
     priority = 10
 
-    services = ["CSC Service", "DHuS Service", "Dias Service"]
+    services = ["CSC Service", "DHuS Service", "Dias Service", "Drive"]
     missions = ["S1", "S2", "S3",
                 "S5p", "EN1", "LC08"]
     platforms = []
     product_types = []
     sensors = []
     nodes = []
     output_nodes = []
 
     cloud_cover_value = 20
-    latitude = 48.8
-    longitude = 2.4
+    latitude_min = 41.5
+    longitude_min = -4.6
+    latitude_max = 51.34
+    longitude_max = 8.8
 
     modality = Qt.ApplicationModal
-    current_path = os.getcwd()
+    dir = os.getcwd()
     recent_paths = settings.Setting([])
 
     want_main_area = False
     graph_name = "thumbnailView"
     auto_commit = settings.Setting(True)
 
     class Outputs:
-        output = Output("Data", DrbNode, auto_summary=False)
+        output = Output("DrbNode", DrbNode, auto_summary=False)
+        dir = Output("Dir", str, auto_summary=False)
 
     def __init__(self):
         super().__init__()
         self.data = None
         self.username = None
         self.password = None
         self.service = None
@@ -115,14 +119,15 @@
         # GUI Commands
         self.combobox_service = gui.comboBox(
             self.controlArea, self, "", items=self.services,
             label="Choose Service: ",
             orientation=Qt.Horizontal,
             contentsLength=8,
         )
+        self.combobox_service.activated.connect(self.choose_datasource)
 
         gui.rubber(self.controlArea)
 
         self.authentication_box = gui.widgetBox(
             self.controlArea, "Authentication: ")
         gui.rubber(self.controlArea)
 
@@ -185,23 +190,36 @@
         self.slider_cc_value = gui.hSlider(
             self.predicate_box, self, "cloud_cover_value",
             label="Cloud Cover Value %:", minValue=0, maxValue=100, step=1,
             width=400,
             createLabel=True
         )
 
-        self.lat_spinbox = gui.doubleSpin(
-            self.predicate_box, self, "latitude", -90, 90,
-            label="Latitude:",
+        self.lat_min_spinbox = gui.doubleSpin(
+            self.predicate_box, self, "latitude_min", -90, 90,
+            label="Min. Latitude:",
             orientation=Qt.Horizontal,
             decimals=2
         )
-        self.lon_spinbox = gui.doubleSpin(
-            self.predicate_box, self, "longitude", -180, 180,
-            label="Longitude:",
+        self.lon_min_spinbox = gui.doubleSpin(
+            self.predicate_box, self, "longitude_min", -180, 180,
+            label="Min. Longitude:",
+            orientation=Qt.Horizontal,
+            decimals=2
+        )
+
+        self.lat_max_spinbox = gui.doubleSpin(
+            self.predicate_box, self, "latitude_max", -90, 90,
+            label="Max. Latitude:",
+            orientation=Qt.Horizontal,
+            decimals=2
+        )
+        self.lon_max_spinbox = gui.doubleSpin(
+            self.predicate_box, self, "longitude_max", -180, 180,
+            label="Max. Longitude:",
             orientation=Qt.Horizontal,
             decimals=2
         )
 
         self.filter_button = gui.button(
             self.predicate_box, self, "Apply Predicate",
             callback=self.apply_filter
@@ -232,25 +250,41 @@
         browse_button = QPushButton(
             browse_action.iconText(),
             clicked=browse_action.trigger
         )
 
         vbox = gui.vBox(self.controlArea, box="Select Directory to:")
         hbox = gui.hBox(vbox)
+        self.output_dir = gui.lineEdit(
+            hbox, self, value="", label="Output Dir:"
+        )
+
+        hbox.layout().addWidget(self.output_dir)
         hbox.layout().addWidget(browse_button)
 
         self.download_button = gui.button(
             vbox, self, "Download Selection",
             callback=self.download
         )
 
         gui.rubber(self.controlArea)
         gui.auto_commit(self.buttonsArea, self,
                         "auto_commit", "Send", box=False)
 
+    def _EnableGUI(self, bActivate):
+        self.username_line.setEnabled(bActivate)
+        self.password_line.setEnabled(bActivate)
+        self.query_button.setEnabled(bActivate)
+
+        self.calendar.setEnabled(bActivate)
+        self.predicate_box.setEnabled(bActivate)
+
+        self.selection_box.setEnabled(bActivate)
+        self.download_button.setEnabled(bActivate)
+
     def query_service(self):
 
         self.choose_service()
 
         self.username = self.username_line.text()
         self.username_line.clear()
         self.password = self.password_line.text()
@@ -261,29 +295,43 @@
                password=self.password)
 
         self.service_node = OdataFactory().create(self.service)
         gui.label(
             self.authentication_box, self,
             f'{len(self.service_node.children)} results found')
 
-    def choose_service(self):
+    def choose_datasource(self):
         idx = self.combobox_service.currentIndex()
 
+        if idx == 3:
+            self.__open_dialog()
+            self.service = ''
+            self._EnableGUI(False)
+        else:
+            self._EnableGUI(True)
+
+    def choose_service(self):
+        idx = self.combobox_service.currentIndex()
         # CSC
         if idx == 0:
             self.service = 'https://demo1.databridge.gael.fr/gss-catalogue'
 
         # DHuS
         elif idx == 1:
             self.service = 'https://apihub.copernicus.eu/apihub/odata/v2'
 
             # DIAS
         elif idx == 2:
             self.service = 'https://catalogue.onda-dias.eu/dias-catalogue'
 
+            # drive path
+        elif idx == 3:
+            self.__open_dialog()
+            self.service = ''
+
     def choose_mission(self):
         idx = self.combobox_mission.currentIndex()
 
         # Sentinel1
         if idx == 0:
 
             self.platforms = ["", "A", "B"]
@@ -407,22 +455,22 @@
         if idx_mission == 1 or idx_mission == 5:
             cc = self.cloud_cover_value
             predicate = predicate + \
                 f" and Attributes/OData.CSC.DoubleAttribute/any(" \
                 f"att:att/Name eq 'cloudCover' and " \
                 f"att/OData.CSC.DoubleAttribute/Value lt {cc})"
 
-        long_min = self.longitude - 0.5
-        long_max = self.longitude + 0.5
-        lat_min = self.latitude - 0.5
-        lat_max = self.latitude + 0.5
-
-        WTK_area = f"Polygon(({long_min} {lat_max}," \
-                   f"{long_max} {lat_max},{long_max} {lat_min}," \
-                   f"{long_min} {lat_min},{long_min} {lat_max}))"
+        lat_min = self.latitude_min
+        lon_min = self.longitude_min
+        lat_max = self.latitude_max
+        lon_max = self.longitude_max
+
+        WTK_area = f"Polygon(({lon_min} {lat_max}," \
+                   f"{lon_max} {lat_max},{lon_max} {lat_min}," \
+                   f"{lon_min} {lat_min},{lon_min} {lat_max}))"
         predicate = predicate + f" and OData.CSC.Intersects(" \
                                 f"location=Footprint," \
                                 f"area=geography'SRID=4326;" \
                                 f"{WTK_area}')"
 
         start_date = self.statemachine.first_date
         end_date = self.statemachine.second_date
@@ -486,23 +534,24 @@
 
         idx = self.combobox_node_selection.currentIndex()
         product_name = self.nodes[idx]
         product_node = self.service_node[product_name]
 
         with product_node.get_impl(io.BytesIO) as stream:
             with open(os.path.join(
-                    self.current_path + f'/{product_name}'), 'wb') as f:
+                    self.dir + f'/{product_name}'), 'wb') as f:
                 f.write(stream.read())
             f.close()
 
     @gui.deferred
     def commit(self):
         """
         Commits the result the next widget in the line.
         """
+        self.Outputs.dir.send(self.dir)
         self.Outputs.output.send(self.output)
 
     def __open_dialog(self):
         start_dir = os.path.expanduser("~/")
         if self.recent_paths:
             start_dir = os.path.dirname(self.recent_paths[0].abspath)
 
@@ -525,15 +574,18 @@
                     self.start()
             dlg.open()
         else:
             dir_path = QFileDialog.getExistingDirectory(
                 self, "Select Directory to Download to", start_dir
             )
             if dir_path:
-                self.current_path = dir_path
+                self.dir = dir_path
+                self.commit.deferred()
+
+                self.output_dir.setText(self.dir)
 
     def handleClicked(self, qDate):
         if self.calendar.selectedDate() == self.startDate:
             # If the selected date is the start date, update the end date
             self.endDate = qDate
         elif self.calendar.selectedDate() == self.endDate:
             # If the selected date is the end date, update the start date
@@ -543,14 +595,12 @@
             # reset the range
             self.startDate = qDate
             self.endDate = qDate
 
         # Select the range of dates
         self.calendar.setMaximumDate(self.startDate)
         self.calendar.setMaximumDate(self.endDate)
-        print(self.startDate)
-        print(self.endDate)
 
 
 if __name__ == "__main__":
     from orangewidget.utils.widgetpreview import WidgetPreview
     WidgetPreview(OWDataCatalog).run()
```

### Comparing `orange-earth-observation-1.0.2/orangecontrib/earth_observation/widgets/cloud_mask.py` & `orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/cloud_mask.py`

 * *Files identical despite different names*

### Comparing `orange-earth-observation-1.0.2/orangecontrib/earth_observation/widgets/crop_image.py` & `orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/crop_image.py`

 * *Files identical despite different names*

### Comparing `orange-earth-observation-1.0.2/orangecontrib/earth_observation/widgets/histogram.py` & `orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/histogram.py`

 * *Files identical despite different names*

### Comparing `orange-earth-observation-1.0.2/orangecontrib/earth_observation/widgets/icons/catalog.svg` & `orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/icons/catalog.svg`

 * *Files identical despite different names*

### Comparing `orange-earth-observation-1.0.2/orangecontrib/earth_observation/widgets/icons/category.svg` & `orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/icons/category.svg`

 * *Files identical despite different names*

### Comparing `orange-earth-observation-1.0.2/orangecontrib/earth_observation/widgets/icons/cloud.svg` & `orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/icons/cloud.svg`

 * *Files identical despite different names*

### Comparing `orange-earth-observation-1.0.2/orangecontrib/earth_observation/widgets/icons/crop.svg` & `orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/icons/crop.svg`

 * *Files identical despite different names*

### Comparing `orange-earth-observation-1.0.2/orangecontrib/earth_observation/widgets/icons/load.svg` & `orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/icons/load.svg`

 * *Files identical despite different names*

### Comparing `orange-earth-observation-1.0.2/orangecontrib/earth_observation/widgets/icons/mosaic.svg` & `orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/icons/mosaic.svg`

 * *Files identical despite different names*

### Comparing `orange-earth-observation-1.0.2/orangecontrib/earth_observation/widgets/icons/projection.svg` & `orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/icons/projection.svg`

 * *Files identical despite different names*

### Comparing `orange-earth-observation-1.0.2/orangecontrib/earth_observation/widgets/icons/view.svg` & `orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/icons/view.svg`

 * *Files identical despite different names*

### Comparing `orange-earth-observation-1.0.2/orangecontrib/earth_observation/widgets/load_image.py` & `orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/load_image.py`

 * *Files identical despite different names*

### Comparing `orange-earth-observation-1.0.2/orangecontrib/earth_observation/widgets/mosaic_image.py` & `orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/mosaic_image.py`

 * *Files identical despite different names*

### Comparing `orange-earth-observation-1.0.2/orangecontrib/earth_observation/widgets/nuts_shape.py` & `orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/nuts_shape.py`

 * *Files identical despite different names*

### Comparing `orange-earth-observation-1.0.2/orangecontrib/earth_observation/widgets/reproject_image.py` & `orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/reproject_image.py`

 * *Files identical despite different names*

### Comparing `orange-earth-observation-1.0.2/orangecontrib/earth_observation/widgets/view_image.py` & `orange-earth-observation-1.1.0/orangecontrib/earth_observation/widgets/view_image.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+import os
 from typing import List, Optional, Iterable
 from Orange.widgets import widget, gui, settings
 from Orange.widgets.widget import Input, Output, MultiInput
 from PyQt5.QtCore import QSize
 from PyQt5.QtGui import QPixmap, QIcon
+from PyQt5.QtCore import pyqtSlot as Slot
 from PyQt5.QtWidgets import QWidget, QListWidget, QListWidgetItem, QListView
-from drb.drivers.file import DrbFileFactory
+from drb.drivers.file import DrbFileFactory, DrbFileNode
 from drb.drivers.image import DrbImageFactory, DrbImageBaseNode
 
 
 class IconView(QListWidget):
     """
     A list view (in QListView.IconMode).
     """
@@ -30,23 +32,25 @@
 class OWViewImage(widget.OWWidget):
     name = "EO View Image"
     description = "Views image(s), also can be used to save an" \
                   " image in the directory structure"
     icon = "icons/view.svg"
     priority = 80
 
+    files = []
     input_nodes = []
     selection = None
 
     want_main_area = True
     graph_name = "thumbnailView"
     image_size = settings.Setting(100)
     auto_commit = settings.Setting(True)
 
     class Inputs:
+        dir = Input("Dir", str, auto_summary=False)
         data = MultiInput("List[DrbImageBaseNode]",
                           DrbImageBaseNode, auto_summary=False)
 
     class Outputs:
         output = Output("Selected[DrbImageBaseNode]",
                         DrbImageBaseNode, auto_summary=False)
 
@@ -75,16 +79,16 @@
         self.mainArea.setMinimumWidth(200)
 
     def view_image(self):
 
         self.thumbnailView.clear()
         if self.input_nodes:
             for image_node in self.input_nodes:
-                print(image_node)
                 path = image_node.path.path
+                print(path)
 
                 item = QListWidgetItem()
                 icon = QIcon()
                 icon.addPixmap(QPixmap(path))
                 item.setIcon(icon)
                 self.thumbnailView.addItem(item)
 
@@ -124,22 +128,42 @@
         self.input_nodes.pop(index)
 
         if not self.input_nodes:
             self.combobox_image.clear()
 
         self.view_image()
 
+    @Inputs.dir
+    def set_dir(self, dir):
+        self.files = [os.path.join(dir, file) for file in os.listdir(dir)]
+        self.input_nodes = [_load_image(file) for file in self.files]
+        self.view_image()
+
     @gui.deferred
     def commit(self):
         """
         Commits the result the next widget in the line.
         """
 
         if self.input_nodes:
             if self.selection is not None:
                 self.output = self.input_nodes[self.selection]
                 self.Outputs.output.send(self.output)
 
 
+def _load_image(file):
+    """
+    Loads and create a DrbImageBaseNode from local file.
+    Parameters:
+        file (str): path to local file
+    Returns:
+        DrbImageBaseNode: a Drb Node of the TC Image
+    """
+    base_node = DrbFileFactory().create(file)
+    image_node = DrbImageFactory().create(base_node)
+
+    return image_node
+
+
 if __name__ == "__main__":
     from orangewidget.utils.widgetpreview import WidgetPreview
     WidgetPreview(OWViewImage).run()
```

### Comparing `orange-earth-observation-1.0.2/setup.cfg` & `orange-earth-observation-1.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `orange-earth-observation-1.0.2/versioneer.py` & `orange-earth-observation-1.1.0/versioneer.py`

 * *Files identical despite different names*

