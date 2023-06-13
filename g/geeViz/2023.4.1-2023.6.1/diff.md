# Comparing `tmp/geeViz-2023.4.1.tar.gz` & `tmp/geeViz-2023.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geeViz-2023.4.1.tar", last modified: Mon Apr 10 21:03:29 2023, max compression
+gzip compressed data, was "geeViz-2023.6.1.tar", last modified: Tue Jun 13 17:08:37 2023, max compression
```

## Comparing `geeViz-2023.4.1.tar` & `geeViz-2023.6.1.tar`

### file list

```diff
@@ -1,68 +1,74 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 21:03:23.710599 geeViz-2023.4.1/
--rw-rw-rw-   0        0        0      574 2021-03-05 23:03:09.000000 geeViz-2023.4.1/LICENSE
--rw-rw-rw-   0        0        0     3900 2023-04-10 21:03:29.304773 geeViz-2023.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     3180 2023-03-22 17:21:57.000000 geeViz-2023.4.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-10 21:03:24.741896 geeViz-2023.4.1/geeViz/
--rw-rw-rw-   0        0        0      118 2023-04-10 20:50:35.000000 geeViz-2023.4.1/geeViz/__init__.py
--rw-rw-rw-   0        0        0    23523 2023-04-10 20:44:55.000000 geeViz-2023.4.1/geeViz/assetManagerLib.py
--rw-rw-rw-   0        0        0    95071 2023-04-10 17:24:49.000000 geeViz-2023.4.1/geeViz/changeDetectionLib.py
-drwxrwxrwx   0        0        0        0 2023-04-10 21:03:27.507749 geeViz-2023.4.1/geeViz/examples/
--rw-rw-rw-   0        0        0     5366 2023-04-10 20:44:09.000000 geeViz-2023.4.1/geeViz/examples/CCDCViz.py
--rw-rw-rw-   0        0        0    11674 2023-03-17 22:07:28.000000 geeViz-2023.4.1/geeViz/examples/CCDCVizNotebook.ipynb
--rw-rw-rw-   0        0        0     7865 2022-02-07 19:59:20.000000 geeViz-2023.4.1/geeViz/examples/CCDCWrapper.py
--rw-rw-rw-   0        0        0     4342 2022-04-15 21:41:00.000000 geeViz-2023.4.1/geeViz/examples/GFSTimeLapse.py
--rw-rw-rw-   0        0        0     6156 2023-03-17 20:39:50.000000 geeViz-2023.4.1/geeViz/examples/LANDTRENDRViz.py
--rw-rw-rw-   0        0        0     9374 2023-03-22 17:42:33.000000 geeViz-2023.4.1/geeViz/examples/LANDTRENDRWrapper.py
--rw-rw-rw-   0        0        0    15519 2023-03-17 22:54:36.000000 geeViz-2023.4.1/geeViz/examples/LANDTRENDRWrapperNotebook.ipynb
--rw-rw-rw-   0        0        0    12431 2023-03-22 17:20:58.000000 geeViz-2023.4.1/geeViz/examples/LCMAP_and_LCMS_Viewer.py
--rw-rw-rw-   0        0        0    19316 2023-03-17 23:04:04.000000 geeViz-2023.4.1/geeViz/examples/LCMAP_and_LCMS_Viewer_Notebook.ipynb
--rw-rw-rw-   0        0        0      118 2023-04-10 20:50:35.000000 geeViz-2023.4.1/geeViz/examples/__init__.py
--rw-rw-rw-   0        0        0     5672 2023-03-22 19:24:09.000000 geeViz-2023.4.1/geeViz/examples/geeViewExample.py
--rw-rw-rw-   0        0        0    16777 2023-03-17 22:12:16.000000 geeViz-2023.4.1/geeViz/examples/geeViewExampleNotebook.ipynb
--rw-rw-rw-   0        0        0     5653 2022-02-07 23:21:45.000000 geeViz-2023.4.1/geeViz/examples/getClimateWrapper.py
--rw-rw-rw-   0        0        0    14015 2023-01-09 16:55:27.000000 geeViz-2023.4.1/geeViz/examples/getCombinedLandsatSentinel2Wrapper.py
--rw-rw-rw-   0        0        0    11238 2022-06-15 22:15:23.000000 geeViz-2023.4.1/geeViz/examples/getLandsatWrapper.py
--rw-rw-rw-   0        0        0    18281 2023-03-17 22:20:04.000000 geeViz-2023.4.1/geeViz/examples/getLandsatWrapperNotebook.ipynb
--rw-rw-rw-   0        0        0    12016 2022-08-23 16:04:44.000000 geeViz-2023.4.1/geeViz/examples/getSentinel2Wrapper.py
--rw-rw-rw-   0        0        0     8991 2022-10-26 19:30:20.000000 geeViz-2023.4.1/geeViz/examples/harmonicRegressionWrapper.py
--rw-rw-rw-   0        0        0     8050 2023-03-22 17:46:00.000000 geeViz-2023.4.1/geeViz/examples/lcmsViewerExample.py
--rw-rw-rw-   0        0        0    18271 2023-03-22 17:21:17.000000 geeViz-2023.4.1/geeViz/examples/lcmsViewerExampleNotebook.ipynb
--rw-rw-rw-   0        0        0    13051 2022-02-16 00:28:08.000000 geeViz-2023.4.1/geeViz/examples/phEEnoVizWrapper.py
--rw-rw-rw-   0        0        0     1038 2022-02-01 00:39:23.000000 geeViz-2023.4.1/geeViz/examples/taskTrackerExample.py
--rw-rw-rw-   0        0        0     6171 2022-02-01 00:38:52.000000 geeViz-2023.4.1/geeViz/examples/timeLapseExample.py
--rw-rw-rw-   0        0        0     1741 2021-04-01 17:15:14.000000 geeViz-2023.4.1/geeViz/gcpLib.py
-drwxrwxrwx   0        0        0        0 2023-04-10 21:03:27.539006 geeViz-2023.4.1/geeViz/geeView/
-drwxrwxrwx   0        0        0        0 2023-04-10 21:03:27.585886 geeViz-2023.4.1/geeViz/geeView/css/
--rw-rw-rw-   0        0        0    18958 2023-03-09 02:29:15.000000 geeViz-2023.4.1/geeViz/geeView/css/style.min.css
-drwxrwxrwx   0        0        0        0 2023-04-10 21:03:28.789104 geeViz-2023.4.1/geeViz/geeView/images/
--rw-rw-rw-   0        0        0     7295 2021-04-01 17:15:14.000000 geeViz-2023.4.1/geeViz/geeView/images/EE-logo-150.png
--rw-rw-rw-   0        0        0    10301 2021-04-01 17:15:14.000000 geeViz-2023.4.1/geeViz/geeView/images/GEE.png
--rw-rw-rw-   0        0        0     5692 2022-08-19 21:41:40.000000 geeViz-2023.4.1/geeViz/geeView/images/GEE_logo_transparent.png
--rw-rw-rw-   0        0        0     4551 2021-04-01 17:15:14.000000 geeViz-2023.4.1/geeViz/geeView/images/RCR-logo.jpg
--rw-rw-rw-   0        0        0    35328 2022-12-07 01:04:30.000000 geeViz-2023.4.1/geeViz/geeView/images/Thumbs.db
--rw-rw-rw-   0        0        0     8352 2021-04-01 17:15:14.000000 geeViz-2023.4.1/geeViz/geeView/images/cumulative_icon.png
--rw-rw-rw-   0        0        0     1502 2021-04-01 17:15:15.000000 geeViz-2023.4.1/geeViz/geeView/images/layer_icon.png
--rw-rw-rw-   0        0        0   230271 2022-06-28 20:18:38.000000 geeViz-2023.4.1/geeViz/geeView/images/logos_usda-fs.svg
--rw-rw-rw-   0        0        0   229463 2022-06-30 19:30:12.000000 geeViz-2023.4.1/geeViz/geeView/images/logos_usda-fs_bn-dk-01.svg
--rw-rw-rw-   0        0        0      635 2022-06-29 22:17:42.000000 geeViz-2023.4.1/geeViz/geeView/images/menu-hamburger_ffffff.svg
--rw-rw-rw-   0        0        0     1489 2021-04-01 17:15:15.000000 geeViz-2023.4.1/geeViz/geeView/images/usdalogo.png
--rw-rw-rw-   0        0        0     8174 2021-04-01 17:15:15.000000 geeViz-2023.4.1/geeViz/geeView/images/usfslogo.png
--rw-rw-rw-   0        0        0     3309 2023-03-08 18:54:11.000000 geeViz-2023.4.1/geeViz/geeView/index.html
-drwxrwxrwx   0        0        0        0 2023-04-10 21:03:29.195389 geeViz-2023.4.1/geeViz/geeView/js/
--rw-rw-rw-   0        0        0    45351 2020-01-16 17:35:18.000000 geeViz-2023.4.1/geeViz/geeView/js/gena-gee-palettes.js
--rw-rw-rw-   0        0        0   338389 2023-04-10 20:57:43.000000 geeViz-2023.4.1/geeViz/geeView/js/lcms-viewer.min.js
--rw-rw-rw-   0        0        0     1021 2023-03-08 18:47:59.000000 geeViz-2023.4.1/geeViz/geeView/js/load.min.js
--rw-rw-rw-   0        0        0    93058 2023-04-10 20:57:59.000000 geeViz-2023.4.1/geeViz/geeView/js/runGeeViz.js
--rw-rw-rw-   0        0        0    11675 2023-04-10 20:46:12.000000 geeViz-2023.4.1/geeViz/geeView.py
--rw-rw-rw-   0        0        0   174861 2023-04-03 16:39:39.000000 geeViz-2023.4.1/geeViz/getImagesLib.py
--rw-rw-rw-   0        0        0     7467 2021-04-01 17:15:14.000000 geeViz-2023.4.1/geeViz/migrateGEEAssets.py
--rw-rw-rw-   0        0        0    20743 2022-06-01 18:25:26.000000 geeViz-2023.4.1/geeViz/phEEnoViz.py
--rw-rw-rw-   0        0        0     9885 2022-11-30 20:14:56.000000 geeViz-2023.4.1/geeViz/taskManagerLib.py
-drwxrwxrwx   0        0        0        0 2023-04-10 21:03:25.023140 geeViz-2023.4.1/geeViz.egg-info/
--rw-rw-rw-   0        0        0     3900 2023-04-10 21:03:23.000000 geeViz-2023.4.1/geeViz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1945 2023-04-10 21:03:23.000000 geeViz-2023.4.1/geeViz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 21:03:23.000000 geeViz-2023.4.1/geeViz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2023-04-10 21:03:23.000000 geeViz-2023.4.1/geeViz.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-10 21:03:23.000000 geeViz-2023.4.1/geeViz.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-10 21:03:29.320396 geeViz-2023.4.1/setup.cfg
--rw-rw-rw-   0        0        0     2200 2022-07-06 19:24:37.000000 geeViz-2023.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 17:08:31.358141 geeViz-2023.6.1/
+-rw-rw-rw-   0        0        0      574 2021-03-05 23:03:09.000000 geeViz-2023.6.1/LICENSE
+-rw-rw-rw-   0        0        0     3851 2023-06-13 17:08:37.468005 geeViz-2023.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3180 2023-03-22 17:21:57.000000 geeViz-2023.6.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-13 17:08:32.451983 geeViz-2023.6.1/geeViz/
+-rw-rw-rw-   0        0        0      118 2023-06-13 17:08:07.000000 geeViz-2023.6.1/geeViz/__init__.py
+-rw-rw-rw-   0        0        0    23538 2023-06-06 19:41:46.000000 geeViz-2023.6.1/geeViz/assetManagerLib.py
+-rw-rw-rw-   0        0        0    95071 2023-04-10 17:24:49.000000 geeViz-2023.6.1/geeViz/changeDetectionLib.py
+drwxrwxrwx   0        0        0        0 2023-06-13 17:08:35.014776 geeViz-2023.6.1/geeViz/examples/
+-rw-rw-rw-   0        0        0     5366 2023-04-10 20:44:09.000000 geeViz-2023.6.1/geeViz/examples/CCDCViz.py
+-rw-rw-rw-   0        0        0    11674 2023-03-17 22:07:28.000000 geeViz-2023.6.1/geeViz/examples/CCDCVizNotebook.ipynb
+-rw-rw-rw-   0        0        0     7865 2022-02-07 19:59:20.000000 geeViz-2023.6.1/geeViz/examples/CCDCWrapper.py
+-rw-rw-rw-   0        0        0     4342 2022-04-15 21:41:00.000000 geeViz-2023.6.1/geeViz/examples/GFSTimeLapse.py
+-rw-rw-rw-   0        0        0     6156 2023-03-17 20:39:50.000000 geeViz-2023.6.1/geeViz/examples/LANDTRENDRViz.py
+-rw-rw-rw-   0        0        0     9374 2023-03-22 17:42:33.000000 geeViz-2023.6.1/geeViz/examples/LANDTRENDRWrapper.py
+-rw-rw-rw-   0        0        0    15140 2023-06-12 22:48:14.000000 geeViz-2023.6.1/geeViz/examples/LANDTRENDRWrapperNotebook.ipynb
+-rw-rw-rw-   0        0        0    12431 2023-06-12 23:07:18.000000 geeViz-2023.6.1/geeViz/examples/LCMAP_and_LCMS_Viewer.py
+-rw-rw-rw-   0        0        0    19047 2023-06-12 23:08:22.000000 geeViz-2023.6.1/geeViz/examples/LCMAP_and_LCMS_Viewer_Notebook.ipynb
+-rw-rw-rw-   0        0        0      118 2023-06-13 17:07:59.000000 geeViz-2023.6.1/geeViz/examples/__init__.py
+-rw-rw-rw-   0        0        0     1925 2023-06-12 22:06:57.000000 geeViz-2023.6.1/geeViz/examples/foliumViewerExample.py
+-rw-rw-rw-   0        0        0   225376 2023-06-13 16:56:55.000000 geeViz-2023.6.1/geeViz/examples/gee2PandasExample.ipynb
+-rw-rw-rw-   0        0        0     5672 2023-03-22 19:24:09.000000 geeViz-2023.6.1/geeViz/examples/geeViewExample.py
+-rw-rw-rw-   0        0        0    16183 2023-06-12 22:37:39.000000 geeViz-2023.6.1/geeViz/examples/geeViewExampleNotebook.ipynb
+-rw-rw-rw-   0        0        0    42932 2023-06-12 22:23:57.000000 geeViz-2023.6.1/geeViz/examples/geeViewVSFoliumViewerExampleNotebook.ipynb
+-rw-rw-rw-   0        0        0     5653 2022-02-07 23:21:45.000000 geeViz-2023.6.1/geeViz/examples/getClimateWrapper.py
+-rw-rw-rw-   0        0        0    14015 2023-01-09 16:55:27.000000 geeViz-2023.6.1/geeViz/examples/getCombinedLandsatSentinel2Wrapper.py
+-rw-rw-rw-   0        0        0    11238 2022-06-15 22:15:23.000000 geeViz-2023.6.1/geeViz/examples/getLandsatWrapper.py
+-rw-rw-rw-   0        0        0    17982 2023-06-12 22:41:46.000000 geeViz-2023.6.1/geeViz/examples/getLandsatWrapperNotebook.ipynb
+-rw-rw-rw-   0        0        0    12016 2022-08-23 16:04:44.000000 geeViz-2023.6.1/geeViz/examples/getSentinel2Wrapper.py
+-rw-rw-rw-   0        0        0     8991 2022-10-26 19:30:20.000000 geeViz-2023.6.1/geeViz/examples/harmonicRegressionWrapper.py
+-rw-rw-rw-   0        0        0     8047 2023-06-12 23:06:39.000000 geeViz-2023.6.1/geeViz/examples/lcmsViewerExample.py
+-rw-rw-rw-   0        0        0    18294 2023-06-12 23:03:39.000000 geeViz-2023.6.1/geeViz/examples/lcmsViewerExampleNotebook.ipynb
+-rw-rw-rw-   0        0        0    13051 2022-02-16 00:28:08.000000 geeViz-2023.6.1/geeViz/examples/phEEnoVizWrapper.py
+-rw-rw-rw-   0        0        0     1038 2022-02-01 00:39:23.000000 geeViz-2023.6.1/geeViz/examples/taskTrackerExample.py
+-rw-rw-rw-   0        0        0     6171 2022-02-01 00:38:52.000000 geeViz-2023.6.1/geeViz/examples/timeLapseExample.py
+-rw-rw-rw-   0        0        0     8568 2023-06-12 22:19:18.000000 geeViz-2023.6.1/geeViz/foliumView.py
+-rw-rw-rw-   0        0        0     1741 2021-04-01 17:15:14.000000 geeViz-2023.6.1/geeViz/gcpLib.py
+-rw-rw-rw-   0        0        0    10215 2023-06-13 15:59:58.000000 geeViz-2023.6.1/geeViz/gee2Pandas.py
+drwxrwxrwx   0        0        0        0 2023-06-13 17:08:35.217832 geeViz-2023.6.1/geeViz/geeView/
+drwxrwxrwx   0        0        0        0 2023-06-13 17:08:35.264706 geeViz-2023.6.1/geeViz/geeView/css/
+-rw-rw-rw-   0        0        0    19972 2023-06-12 22:58:01.000000 geeViz-2023.6.1/geeViz/geeView/css/style.min.css
+-rw-rw-rw-   0        0        0    10893 2023-06-13 17:05:14.000000 geeViz-2023.6.1/geeViz/geeView/foliumView.html
+drwxrwxrwx   0        0        0        0 2023-06-13 17:08:36.217910 geeViz-2023.6.1/geeViz/geeView/images/
+-rw-rw-rw-   0        0        0     7295 2021-04-01 17:15:14.000000 geeViz-2023.6.1/geeViz/geeView/images/EE-logo-150.png
+-rw-rw-rw-   0        0        0    10301 2021-04-01 17:15:14.000000 geeViz-2023.6.1/geeViz/geeView/images/GEE.png
+-rw-rw-rw-   0        0        0     5692 2022-08-19 21:41:40.000000 geeViz-2023.6.1/geeViz/geeView/images/GEE_logo_transparent.png
+-rw-rw-rw-   0        0        0     4551 2021-04-01 17:15:14.000000 geeViz-2023.6.1/geeViz/geeView/images/RCR-logo.jpg
+-rw-rw-rw-   0        0        0    35328 2022-12-07 01:04:30.000000 geeViz-2023.6.1/geeViz/geeView/images/Thumbs.db
+-rw-rw-rw-   0        0        0     8352 2021-04-01 17:15:14.000000 geeViz-2023.6.1/geeViz/geeView/images/cumulative_icon.png
+-rw-rw-rw-   0        0        0     1502 2021-04-01 17:15:15.000000 geeViz-2023.6.1/geeViz/geeView/images/layer_icon.png
+-rw-rw-rw-   0        0        0   230271 2022-06-28 20:18:38.000000 geeViz-2023.6.1/geeViz/geeView/images/logos_usda-fs.svg
+-rw-rw-rw-   0        0        0   229463 2022-06-30 19:30:12.000000 geeViz-2023.6.1/geeViz/geeView/images/logos_usda-fs_bn-dk-01.svg
+-rw-rw-rw-   0        0        0      635 2022-06-29 22:17:42.000000 geeViz-2023.6.1/geeViz/geeView/images/menu-hamburger_ffffff.svg
+-rw-rw-rw-   0        0        0     1489 2021-04-01 17:15:15.000000 geeViz-2023.6.1/geeViz/geeView/images/usdalogo.png
+-rw-rw-rw-   0        0        0     8174 2021-04-01 17:15:15.000000 geeViz-2023.6.1/geeViz/geeView/images/usfslogo.png
+-rw-rw-rw-   0        0        0     3309 2023-03-08 18:54:11.000000 geeViz-2023.6.1/geeViz/geeView/index.html
+drwxrwxrwx   0        0        0        0 2023-06-13 17:08:36.874206 geeViz-2023.6.1/geeViz/geeView/js/
+-rw-rw-rw-   0        0        0    45351 2020-01-16 17:35:18.000000 geeViz-2023.6.1/geeViz/geeView/js/gena-gee-palettes.js
+-rw-rw-rw-   0        0        0   342637 2023-06-13 17:05:09.000000 geeViz-2023.6.1/geeViz/geeView/js/lcms-viewer.min.js
+-rw-rw-rw-   0        0        0     1021 2023-03-08 18:47:59.000000 geeViz-2023.6.1/geeViz/geeView/js/load.min.js
+-rw-rw-rw-   0        0        0  1481815 2023-06-13 16:56:11.000000 geeViz-2023.6.1/geeViz/geeView/js/runGeeViz.js
+-rw-rw-rw-   0        0        0    13516 2023-06-13 15:20:03.000000 geeViz-2023.6.1/geeViz/geeView.py
+-rw-rw-rw-   0        0        0   174866 2023-04-19 18:43:30.000000 geeViz-2023.6.1/geeViz/getImagesLib.py
+-rw-rw-rw-   0        0        0     7467 2021-04-01 17:15:14.000000 geeViz-2023.6.1/geeViz/migrateGEEAssets.py
+-rw-rw-rw-   0        0        0    20743 2022-06-01 18:25:26.000000 geeViz-2023.6.1/geeViz/phEEnoViz.py
+-rw-rw-rw-   0        0        0     9885 2023-04-21 16:32:19.000000 geeViz-2023.6.1/geeViz/taskManagerLib.py
+drwxrwxrwx   0        0        0        0 2023-06-13 17:08:32.639459 geeViz-2023.6.1/geeViz.egg-info/
+-rw-rw-rw-   0        0        0     3851 2023-06-13 17:08:30.000000 geeViz-2023.6.1/geeViz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2156 2023-06-13 17:08:31.000000 geeViz-2023.6.1/geeViz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 17:08:30.000000 geeViz-2023.6.1/geeViz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       81 2023-06-13 17:08:30.000000 geeViz-2023.6.1/geeViz.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-13 17:08:30.000000 geeViz-2023.6.1/geeViz.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-13 17:08:37.514882 geeViz-2023.6.1/setup.cfg
+-rw-rw-rw-   0        0        0     2173 2023-06-13 15:31:46.000000 geeViz-2023.6.1/setup.py
```

### Comparing `geeViz-2023.4.1/LICENSE` & `geeViz-2023.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `geeViz-2023.4.1/PKG-INFO` & `geeViz-2023.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: geeViz
-Version: 2023.4.1
+Version: 2023.6.1
 Summary: A package to help with GEE data processing, analysis, and visualization
 Home-page: https://github.com/gee-community/geeViz
 Author: Ian Housman
 Author-email: ian.housman@gmail.com
 License: Apache
 Keywords: earthengine google remote sensing landsat sentinel modis forestry forest
-Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `geeViz-2023.4.1/README.md` & `geeViz-2023.6.1/README.md`

 * *Files identical despite different names*

### Comparing `geeViz-2023.4.1/geeViz/assetManagerLib.py` & `geeViz-2023.6.1/geeViz/assetManagerLib.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-   Copyright 2019 Leah Campbell
+   Copyright 2023 Leah Campbell and Ian Housman
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
 
@@ -479,15 +479,15 @@
 # pyramidingPolicy and noDataValues can be one for each band name or only one (that is then repeated for each band)
 # The system:time_start and system:time_end properties are handled automatically assuming the proper format or ee Date object is provided
 def ingestImageFromGCS(gcsURIs,assetPath,overwrite = False,bandNames = None,properties = None,pyramidingPolicy=None,noDataValues=None):
     if overwrite or not ee_asset_exists(assetPath):
         taskID= ee.data.newTaskId(1)[0]
 
         #Make sure collection or folder exists
-        create_image_collection(os.path.basename(assetPath))
+        create_image_collection(os.path.dirname(assetPath))
 
         # Handle if single image path is provided - changes to a list
         if str(type(gcsURIs)).find("'str'")>-1:
             gcsURIs = [gcsURIs]
 
         # Repeat the pyramiding policy and no data value if only one is provided
         if bandNames != None and pyramidingPolicy != None and str(type(pyramidingPolicy)).find("'str'")>-1:
```

### Comparing `geeViz-2023.4.1/geeViz/changeDetectionLib.py` & `geeViz-2023.6.1/geeViz/changeDetectionLib.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.4.1/geeViz/examples/CCDCViz.py` & `geeViz-2023.6.1/geeViz/examples/CCDCViz.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.4.1/geeViz/examples/CCDCVizNotebook.ipynb` & `geeViz-2023.6.1/geeViz/examples/CCDCVizNotebook.ipynb`

 * *Files identical despite different names*

### Comparing `geeViz-2023.4.1/geeViz/examples/CCDCWrapper.py` & `geeViz-2023.6.1/geeViz/examples/CCDCWrapper.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.4.1/geeViz/examples/GFSTimeLapse.py` & `geeViz-2023.6.1/geeViz/examples/GFSTimeLapse.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.4.1/geeViz/examples/LANDTRENDRViz.py` & `geeViz-2023.6.1/geeViz/examples/LANDTRENDRViz.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.4.1/geeViz/examples/LANDTRENDRWrapper.py` & `geeViz-2023.6.1/geeViz/examples/LANDTRENDRWrapper.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.4.1/geeViz/examples/LANDTRENDRWrapperNotebook.ipynb` & `geeViz-2023.6.1/geeViz/examples/LANDTRENDRWrapperNotebook.ipynb`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9931277797490651%*

 * *Differences: {"'cells'": "{0: {'attachments': OrderedDict()}, 1: {'outputs': {0: {'text': {insert: [(1, 'geeViz "*

 * *            "package folder: c:\\\\Python310\\\\lib\\\\site-packages\\\\geeViz\\n')], delete: "*

 * *            "[1]}}}}, 3: {'outputs': {0: {'text': {insert: [(3, 'Local web server at: "*

 * *            "http://localhost:8001/geeView/ already serving.\\n'), (4, 'cwd "*

 * *            "a:\\\\GEE\\\\gee_py_modules_package\\\\geeViz\\\\examples\\n')], delete: [6, 5, 4, "*

 * *            "3]}}, 1: {'data': {'text/html': {inser […]*

```diff
@@ -1,10 +1,11 @@
 {
     "cells": [
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "884438f5",
             "metadata": {},
             "source": [
                 "Copyright 2023 Ian Housman\n",
                 "\n",
                 "Licensed under the Apache License, Version 2.0 (the \"License\");\n",
@@ -29,15 +30,15 @@
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Initializing GEE\n",
-                        "geeViz package folder: C:\\Python310\\lib\\site-packages\\geeViz\n",
+                        "geeViz package folder: c:\\Python310\\lib\\site-packages\\geeViz\n",
                         "done\n"
                     ]
                 }
             ],
             "source": [
                 "#Example of how to get Landsat data using the getImagesLib, create median composites, run LandTrendr and then filter \n",
                 "#LandTrendr output into usable data depicting where, when, and the magnitude of loss and gain\n",
@@ -187,41 +188,38 @@
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Adding layer: Hansen Loss Year\n",
                         "Starting webmap\n",
                         "Using default refresh token for geeView: C:\\Users\\ihousman/.config/earthengine/credentials\n",
-                        "Starting local web server at: http://localhost:8001/geeView/\n",
-                        "HTTP server command: \"C:\\Python310\\python.exe\" -m http.server  8001\n",
-                        "Done\n",
-                        "cwd A:\\GEE\\gee_py_modules_package\\geeViz\\examples\n"
+                        "Local web server at: http://localhost:8001/geeView/ already serving.\n",
+                        "cwd a:\\GEE\\gee_py_modules_package\\geeViz\\examples\n"
                     ]
                 },
                 {
                     "data": {
                         "text/html": [
                             "\n",
                             "        <iframe\n",
                             "            width=\"100%\"\n",
                             "            height=\"525px\"\n",
-                            "            src=\"http://localhost:8001/geeView/?accessToken=ya29.a0AVvZVsqDTP9xVjMt-NX4xpHVgG1HxPuaZ9XWdpbThhwbvE99QDpaIv5dU12y4kCZDfewQbSsh5RuqsXpkJ1RD2aze0Yeai7WPl6oOM0Vm7vJJu2pEJleVETsJDinwgU4pVnEGwbIWjD7uOvGMF0hHLXUaBuMH4LdtdSd_C4aCgYKAQkSARASFQGbdwaIdBYsJBmjMDnIS2U9FwsCxA0174\"\n",
+                            "            src=\"http://localhost:8001/geeView/?accessToken=ya29.a0AWY7CkmOUcbu6sh0cMq_O99s5aEOYhfFh5zT2ENMXgeuuroaQAQ_PDVgrfI-dDGQ36PmGOA-pm-ktyjuWhF5JoVm22DI5woTsvTZhdtkGDVCQBj04hBhlklPJJc3qmi4FH2DQahwsH7yCc_xQlwcvZrtzi5hg2PVnodfZdUaCgYKAdoSARASFQG1tDrpZfWNBxWCabgg_6K-Q05vIQ0174\"\n",
                             "            frameborder=\"0\"\n",
                             "            allowfullscreen\n",
                             "            \n",
                             "        ></iframe>\n",
                             "        "
                         ],
                         "text/plain": [
-                            "<IPython.lib.display.IFrame at 0x17f846f7790>"
+                            "<IPython.lib.display.IFrame at 0x2a9adfd1990>"
                         ]
                     },
-                    "execution_count": 3,
                     "metadata": {},
-                    "output_type": "execute_result"
+                    "output_type": "display_data"
                 }
             ],
             "source": [
                 "####################################################################################################\n",
                 "#Start function calls\n",
                 "####################################################################################################\n",
                 "#First, let's look at the Hansen Global Forest Change output\n",
@@ -234,16 +232,15 @@
                 "hansen = ee.Image(\"UMD/hansen/global_forest_change_2020_v1_8\").select(['lossyear']).add(2000).int16()\n",
                 "hansen = hansen.updateMask(hansen.neq(2000).And(hansen.gte(startYear)).And(hansen.lte(endYear)))\n",
                 "Map1.addLayer(hansen,{'min':startYear,'max':endYear,'palette':changeDetectionLib.lossYearPalette},'Hansen Loss Year',True)\n",
                 "\n",
                 "#Bring in map\n",
                 "Map1.turnOnInspector()\n",
                 "Map1.centerObject(studyArea)\n",
-                "Map1.view(open_browser = False, open_iframe = True,iframe_height='525')\n",
-                "Map1.IFrame\n"
+                "Map1.view()\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 4,
             "id": "8a49bd8c",
             "metadata": {
@@ -263,38 +260,37 @@
                         "Applying scale factors for C2 L9 data\n",
                         "Applying Fmask Cloud Mask\n",
                         "Applying Fmask Shadow Mask\n",
                         "Adding layer: Composite Time Series\n",
                         "Starting webmap\n",
                         "Using default refresh token for geeView: C:\\Users\\ihousman/.config/earthengine/credentials\n",
                         "Local web server at: http://localhost:8001/geeView/ already serving.\n",
-                        "cwd A:\\GEE\\gee_py_modules_package\\geeViz\\examples\n"
+                        "cwd a:\\GEE\\gee_py_modules_package\\geeViz\\examples\n"
                     ]
                 },
                 {
                     "data": {
                         "text/html": [
                             "\n",
                             "        <iframe\n",
                             "            width=\"100%\"\n",
                             "            height=\"525px\"\n",
-                            "            src=\"http://localhost:8001/geeView/?accessToken=ya29.a0AVvZVspji71fDBcHU3_BorB2XMuQ1N7Wvnha4wgA75-mGHgf6QSYjJI4eNUfRLH1hpHe88JiTPmaoG2eN_Ht1oa6kDztY7JdQOf296B-8vhmYct-0CGFWSeWHJz4OD9EtKUUHPCijFHdmaQebH5_FGMkGM5ZYuT0V1oXWScaCgYKAfASARASFQGbdwaI2BXdeNDDfsTaBw8BtxPQ0g0174\"\n",
+                            "            src=\"http://localhost:8001/geeView/?accessToken=ya29.a0AWY7CkkJBiw-bHzw8YnuO5a5VHeSmtJ2vo56s8xTAZ4_wiO5459dQKVKNyGA--HUOzDnkKhg3N5VOBjyI2mvIoCCJJpd59ksMyjPSjVwBD7AxRIQR5aeNup-KhxTryQt5dCpL-48Bx3Z_2GR-9WQ5r8rrgOdlCEdHWM9AUsaCgYKAbkSARASFQG1tDrpap_uvuIDMcPBZJuQDzafVw0174\"\n",
                             "            frameborder=\"0\"\n",
                             "            allowfullscreen\n",
                             "            \n",
                             "        ></iframe>\n",
                             "        "
                         ],
                         "text/plain": [
-                            "<IPython.lib.display.IFrame at 0x17f84733340>"
+                            "<IPython.lib.display.IFrame at 0x2a9ae0111e0>"
                         ]
                     },
-                    "execution_count": 4,
                     "metadata": {},
-                    "output_type": "execute_result"
+                    "output_type": "display_data"
                 }
             ],
             "source": [
                 "####################################################################################################\n",
                 "#Clear the map in case it has been populated with layers/commands earlier\n",
                 "Map2.clearMap()\n",
                 "\n",
@@ -310,21 +306,20 @@
                 "                                     .set('system:time_start',ee.Date.fromYMD(yr,6,1).millis())\n",
                 "                                    ))\n",
                 "Map2.addTimeLapse(composites,getImagesLib.vizParamsFalse,'Composite Time Series')\n",
                 "\n",
                 "\n",
                 "#Bring in map\n",
                 "Map2.centerObject(studyArea)\n",
-                "Map2.view(open_browser = False, open_iframe = True,iframe_height = 525)\n",
-                "Map2.IFrame"
+                "Map2.view()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 6,
+            "execution_count": 5,
             "id": "149fca54",
             "metadata": {
                 "scrolled": false
             },
             "outputs": [
                 {
                     "name": "stdout",
@@ -338,38 +333,37 @@
                         "Adding layer: 1 NBR Gain Year\n",
                         "Adding layer: 1 NBR Gain Magnitude\n",
                         "Adding layer: 1 NBR Gain Duration\n",
                         "Adding layer: Study Area\n",
                         "Starting webmap\n",
                         "Using default refresh token for geeView: C:\\Users\\ihousman/.config/earthengine/credentials\n",
                         "Local web server at: http://localhost:8001/geeView/ already serving.\n",
-                        "cwd A:\\GEE\\gee_py_modules_package\\geeViz\\examples\n"
+                        "cwd a:\\GEE\\gee_py_modules_package\\geeViz\\examples\n"
                     ]
                 },
                 {
                     "data": {
                         "text/html": [
                             "\n",
                             "        <iframe\n",
                             "            width=\"100%\"\n",
                             "            height=\"525px\"\n",
-                            "            src=\"http://localhost:8001/geeView/?accessToken=ya29.a0AVvZVspz_c_OeyrhZh8cdLBxj3QcmlJ1eS6re_emc5-nfaA4konu8MfJcTS6SXKR6qz3gehASa03CRg7CUEtUAa3Ga4_0wAlVzNyXGBxOSyZWfzZsJMpKLQoURCLJLX44Oun3LbOYBMD5ZGCw0A136EWQdbUMN9sokK9a4oaCgYKAfoSARASFQGbdwaItJoQ_QcjtkeiW1e4O9c7pA0174\"\n",
+                            "            src=\"http://localhost:8001/geeView/?accessToken=ya29.a0AWY7Cknx83wd2Gf8QW0hu7TGOI2cDJm_UXxKci__Idl2IQDcmcqOULcVfWTegLJGgHV0t3j9r9iq0Ett1j4tb7N7vcsKTAYPCKZpNOUpalIl78nTrPSxZgm-M-o6894np6qPnLdTXTUE4N2n_vGnY-wEdvvB9Qh5a-iKDlgaCgYKAfESARASFQG1tDrp6xgJsmYcfU7do7d5cqbVGg0174\"\n",
                             "            frameborder=\"0\"\n",
                             "            allowfullscreen\n",
                             "            \n",
                             "        ></iframe>\n",
                             "        "
                         ],
                         "text/plain": [
-                            "<IPython.lib.display.IFrame at 0x17f847480d0>"
+                            "<IPython.lib.display.IFrame at 0x2a9ac1a6f80>"
                         ]
                     },
-                    "execution_count": 6,
                     "metadata": {},
-                    "output_type": "execute_result"
+                    "output_type": "display_data"
                 }
             ],
             "source": [
                 "#Clear the map in case it has been populated with layers/commands earlier\n",
                 "Map1.clearMap()\n",
                 "# Important that the range of data values of the composites match the run_params spikeThreshold and recoveryThreshold\n",
                 "# e.g. Reflectance bands that have a scale of 0-1 should have a spikeThreshold around 0.9\n",
@@ -381,16 +375,15 @@
                 "                                                gainMagThresh,gainSlopeThresh,slowLossDurationThresh,chooseWhichLoss,\\\n",
                 "                                                chooseWhichGain,addToMap,howManyToPull)\n",
                 "\n",
                 "#Bring in map\n",
                 "Map1.turnOnInspector()\n",
                 "Map1.centerObject(studyArea)\n",
                 "Map1.addLayer(studyArea, {'strokeColor': '0000FF'}, \"Study Area\", False)\n",
-                "Map1.view(open_browser = False, open_iframe = True)\n",
-                "Map1.IFrame"
+                "Map1.view()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "b652ec18",
             "metadata": {
```

### Comparing `geeViz-2023.4.1/geeViz/examples/LCMAP_and_LCMS_Viewer.py` & `geeViz-2023.6.1/geeViz/examples/LCMAP_and_LCMS_Viewer.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,16 +30,16 @@
 # User Parameters
 
 # Define the early time period 
 preStartYear = 1985
 preEndYear = 1990
 
 # Define the more recent time period
-postStartYear = 2016
-postEndYear = 2020
+postStartYear = 2021
+postEndYear = 2022
 
 # Specify whether to add time lapses of products. If True, loading the viewer will take much much much much longer
 addTimelapses = False
 ####################################################################################################
 # Bring in LCMAP outputs
 # This part was adapted from info available in the awesome-gee-community-datasets
 # https://samapriya.github.io/awesome-gee-community-datasets/projects/lcmap/
@@ -80,17 +80,17 @@
 lcachg_palette = ['E60000','A87000','E3E3C2','1D6330','476BA1','BAD9EB','FFFFFF','B3B0A3','A201FF']
 # sclast_palette = ['FFC7AA','F87E45','CC764E','86A7B6','46A4EE','7954C8','7A24AA','432172']
 # scstab_palette = ['BA4E16','EE964D','FFE29C','F4FBC1','E1F3C3','BCE6CA','46989C']
 # scmqa_palette = ['000000','A900E6','DF73FF','F5F5E3','DB8A00','924900','9C9C9C','FFFFFF']
 
 # Set up some visualization dictionaries
 lc_viz = {'min':1,'max':9,'palette':lcpri_palette,'classLegendDict':lc_legend_dict,'queryDict':lc_lookup_dict}
-loss_viz = {'min':1985,'max':2020,'palette':changeDetectionLib.lossYearPalette}
-gain_viz = {'min':1985,'max':2020,'palette':changeDetectionLib.gainYearPalette}
-change_viz = {'min':1985,'max':2020,'palette':['00F','F0F']}
+loss_viz = {'min':1985,'max':2022,'palette':changeDetectionLib.lossYearPalette}
+gain_viz = {'min':1985,'max':2022,'palette':changeDetectionLib.gainYearPalette}
+change_viz = {'min':1985,'max':2022,'palette':['00F','F0F']}
 
 # Map.addLayer(sctime.max(),{'min':100,'max':292,'palette':['151d44', '156c72', '7eb390', 'fdf5f4', 'db8d77', '9c3060', '340d35']},'SCTIME',True)
 # Map.addLayer(scmag.max(),{'min':651,'max':3700,'palette':['d7f9d0', 'a2d595', '64b463', '129450', '126e45', '1a482f', '122414']},'SCMAG',True)
 # Map.addLayer(ee.Image(sclast.sort('system:time_start',false).first()).mask(ee.Image(sclast.sort('system:time_start',false).first()).gt(0)),{min:518,max:4600,palette:sclast_palette},'SCLAST',false)
 # Map.addLayer(scstab.sort('system:time_start',false).first(),{min:70,max:13000,palette:scstab_palette},'SCSTAB',false)
 # Map.addLayer(scmqa.sort('system:time_start',false).first().remap([0,4,6,8,14,24,44,54],[0,1,2,3,4,5,6,7]).mask(ee.Image(scmqa.sort('system:time_start',false).first()).gt(0)),{min:0,max:7,palette:scmqa_palette},'SCMQA',false)
 ####################################################################################################
@@ -98,15 +98,15 @@
 # LCMS' homepage can be found here: https://data.fs.usda.gov/geodata/rastergateway/LCMS/index.php
 # LCMS methods are described here: https://data.fs.usda.gov/geodata/rastergateway/LCMS/LCMS_v2021-7_Methods.pdf
 # LCMS data can also be viewed and downloaded here: https://apps.fs.usda.gov/lcms-viewer
 # LCMS GEE data collections are available at:
   # https://developers.google.com/earth-engine/datasets/catalog/USFS_GTAC_LCMS_v20201-7 (CONUS and Southeastern AK)
   # https://developers.google.com/earth-engine/datasets/catalog/USFS_GTAC_LCMS_v2020-6 (Puerto Rico and US Virgin Islands
 # An in-depth look at the model predictor variables that go into making LCMS maps can be found here:https://apps.fs.usda.gov/lcms-viewer/lcms-base-learner.html
-lcms = ee.ImageCollection("USFS/GTAC/LCMS/v2021-7").filter(ee.Filter.eq('study_area','CONUS'))
+lcms = ee.ImageCollection("USFS/GTAC/LCMS/v2022-8").filter(ee.Filter.eq('study_area','CONUS'))
 ####################################################################################################
 
 ####################################################################################################
 #This section adds the land cover and land use maps from LCMAP and LCMS
 
 # Pull the LCMAP pre and post land cover data
 lcmap_pre = lcpri.filter(ee.Filter.calendarRange(preStartYear,preEndYear,'year')).mode()
```

### Comparing `geeViz-2023.4.1/geeViz/examples/LCMAP_and_LCMS_Viewer_Notebook.ipynb` & `geeViz-2023.6.1/geeViz/examples/LCMAP_and_LCMS_Viewer_Notebook.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.925398496558705%*

 * *Differences: {"'cells'": "{0: {'attachments': OrderedDict()}, 1: {'outputs': {0: {'text': {insert: [(1, 'geeViz "*

 * *            "package folder: c:\\\\Python310\\\\lib\\\\site-packages\\\\geeViz\\n')], delete: "*

 * *            "[1]}}}}, 2: {'execution_count': 22, 'source': {insert: [(7, 'postStartYear = "*

 * *            "2020\\n'), (8, 'postEndYear = 2021\\n')], delete: [8, 7]}}, 3: {'attachments': "*

 * *            "OrderedDict()}, 4: {'execution_count': 23}, 5: {'attachments': OrderedDict()}, 6: "*

 * *            "{'execution_count': […]*

```diff
@@ -1,10 +1,11 @@
 {
     "cells": [
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "ff459534",
             "metadata": {},
             "source": [
                 "## LCMAP and LCMS Outputs Viewer\n",
                 "* This script provides a view of LCMAP and LCMS GEE collections to help understand the strengths of each\n",
                 "* It displays the land cover and land use products as well as change products from each program\n",
@@ -34,15 +35,15 @@
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Initializing GEE\n",
-                        "geeViz package folder: C:\\Python310\\lib\\site-packages\\geeViz\n",
+                        "geeViz package folder: c:\\Python310\\lib\\site-packages\\geeViz\n",
                         "Done\n"
                     ]
                 }
             ],
             "source": [
                 "import os,sys\n",
                 "sys.path.append(os.getcwd())\n",
@@ -54,15 +55,15 @@
                 "Map = getImagesLib.Map\n",
                 "\n",
                 "print('Done')"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 2,
+            "execution_count": 22,
             "id": "6ec8ed53",
             "metadata": {
                 "scrolled": false
             },
             "outputs": [
                 {
                     "name": "stdout",
@@ -76,24 +77,25 @@
                 "# User Parameters\n",
                 "\n",
                 "# Define the early time period \n",
                 "preStartYear = 1985\n",
                 "preEndYear = 1990\n",
                 "\n",
                 "# Define the more recent time period\n",
-                "postStartYear = 2016\n",
-                "postEndYear = 2020\n",
+                "postStartYear = 2020\n",
+                "postEndYear = 2021\n",
                 "\n",
                 "# Specify whether to add time lapses of products. If True, loading the viewer will take much much much much longer\n",
                 "addTimelapses = False\n",
                 "\n",
                 "print('Done')"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "13abaf4c",
             "metadata": {},
             "source": [
                 "### Bring in LCMAP outputs\n",
                 "* This part was adapted from info available in the awesome-gee-community-datasets https://samapriya.github.io/awesome-gee-community-datasets/projects/lcmap/\n",
                 "* Playground example: https://code.earthengine.google.com/791aa894ce0abfe1a9eb1dc478bbc5d7\n",
@@ -102,15 +104,15 @@
                 "* LCMAP methods can be found here: https://www.sciencedirect.com/science/article/pii/S003442571930375X\n",
                 "* LCMAP data can be downloaded from: https://www.usgs.gov/core-science-systems/eros/lcmap/lcmap-data-access\n",
                 "* LCMAP data can also be viewed here: https://eros.usgs.gov/lcmap/viewer/"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 3,
+            "execution_count": 23,
             "id": "0026345a",
             "metadata": {
                 "scrolled": false
             },
             "outputs": [
                 {
                     "name": "stdout",
@@ -152,14 +154,15 @@
                 "# scstab_palette = ['BA4E16','EE964D','FFE29C','F4FBC1','E1F3C3','BCE6CA','46989C']\n",
                 "# scmqa_palette = ['000000','A900E6','DF73FF','F5F5E3','DB8A00','924900','9C9C9C','FFFFFF']\n",
                 "\n",
                 "print('Done')"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "62df699c",
             "metadata": {},
             "source": [
                 "### Bring in LCMS GEE collections\n",
                 "* LCMS' homepage can be found here: https://data.fs.usda.gov/geodata/rastergateway/LCMS/index.php\n",
                 "* LCMS methods are described here: https://data.fs.usda.gov/geodata/rastergateway/LCMS/LCMS_v2021-7_Methods.pdf\n",
@@ -169,202 +172,195 @@
                 "    * https://developers.google.com/earth-engine/datasets/catalog/USFS_GTAC_LCMS_v2020-6 (Puerto Rico and US Virgin Islands\n",
                 "* An in-depth look at the model predictor variables that go into making LCMS maps can be found here:\n",
                 "    * https://apps.fs.usda.gov/lcms-viewer/lcms-base-learner.html"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
+            "execution_count": 24,
             "id": "a3234d4c",
             "metadata": {
                 "scrolled": false
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Done\n"
                     ]
                 }
             ],
             "source": [
-                "lcms = ee.ImageCollection(\"USFS/GTAC/LCMS/v2021-7\").merge(ee.ImageCollection(\"USFS/GTAC/LCMS/v2020-6\"))\n",
+                "lcms = ee.ImageCollection(\"USFS/GTAC/LCMS/v2022-8\").merge(ee.ImageCollection(\"USFS/GTAC/LCMS/v2020-6\"))\n",
                 "print('Done')"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
-            "id": "e2a9f76b",
+            "execution_count": 25,
+            "id": "ab46aaea",
             "metadata": {
-                "scrolled": false
+                "scrolled": true
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Adding layer: LCMAP LC 1985-1990 mode\n",
-                        "Adding layer: LCMAP LC 2016-2020 mode\n",
-                        "Adding layer: LCMS LC 1985-1990 mode\n",
-                        "Adding layer: LCMS LC 2016-2020 mode\n",
-                        "Adding layer: LCMS LU 1985-1990 mode\n",
-                        "Adding layer: LCMS LU 2016-2020 mode\n",
+                        "Adding layer: LCMS Land Cover\n",
+                        "Adding layer: LCMS Land Use\n",
                         "Starting webmap\n",
                         "Using default refresh token for geeView: C:\\Users\\ihousman/.config/earthengine/credentials\n",
-                        "Starting local web server at: http://localhost:8001/geeView/\n",
-                        "HTTP server command: \"C:\\Python310\\python.exe\" -m http.server  8001\n",
-                        "Done\n",
-                        "cwd A:\\GEE\\gee_py_modules_package\\geeViz\\examples\n"
+                        "Local web server at: http://localhost:8001/geeView/ already serving.\n",
+                        "cwd a:\\GEE\\gee_py_modules_package\\geeViz\\examples\n"
                     ]
                 },
                 {
                     "data": {
                         "text/html": [
                             "\n",
                             "        <iframe\n",
                             "            width=\"100%\"\n",
                             "            height=\"525px\"\n",
-                            "            src=\"http://localhost:8001/geeView/?accessToken=ya29.a0AVvZVsoX7U0M07Ner7po8XdpTv5NfAg-NK5HVzhDozxoMXcQihVtTNHDpX4qfr5PLSXtwDVkQRaoX-yB2hIskU8mBlff4m5C34onUcM9lsVbSgWKw_GIHL32Gz2i88VE36Knnhb3EVFLMJVKRzYLpt_QzcARgwx4FwRENWsaCgYKATESARASFQGbdwaIFUE-kl6XOGGQQy5kMvk_kQ0174\"\n",
+                            "            src=\"http://localhost:8001/geeView/?accessToken=ya29.a0AWY7CknsBtKVvnMEU0JGH7My_aF9q3oVZO3UZ8fRqKoya6MBQ5XiIKaISzw41Eifm78khEwEM1EXs5Mgx1ZRrW_ByR6ssHDG4aapRDW1u0jCGj3b1qXCxdjtYqD-7XNu7L-umAFrrjj41eGmAZv56cXOkdY3ehBg-zHXYPkaCgYKAXQSARASFQG1tDrpAVNMJ28WSq4fS-X1wWWp4g0174\"\n",
                             "            frameborder=\"0\"\n",
                             "            allowfullscreen\n",
                             "            \n",
                             "        ></iframe>\n",
                             "        "
                         ],
                         "text/plain": [
-                            "<IPython.lib.display.IFrame at 0x1e217b8eda0>"
+                            "<IPython.lib.display.IFrame at 0x1c095d7fa60>"
                         ]
                     },
-                    "execution_count": 7,
                     "metadata": {},
-                    "output_type": "execute_result"
+                    "output_type": "display_data"
                 }
             ],
             "source": [
-                "#This section adds the land cover and land use maps from LCMAP and LCMS\n",
+                "# Add time lapses\n",
                 "\n",
                 "#First clear the map in case it has been populated with layers/commands earlier\n",
                 "Map.clearMap()\n",
                 "\n",
-                "# Set up some visualization dictionaries\n",
-                "lc_viz = {'min':1,'max':9,'palette':lcpri_palette,'classLegendDict':lc_legend_dict,'queryDict':lc_lookup_dict}\n",
-                "loss_viz = {'min':1985,'max':2020,'palette':changeDetectionLib.lossYearPalette}\n",
-                "gain_viz = {'min':1985,'max':2020,'palette':changeDetectionLib.gainYearPalette}\n",
-                "change_viz = {'min':1985,'max':2020,'palette':['00F','F0F']}\n",
-                "\n",
-                "\n",
-                "# Pull the LCMAP pre and post land cover data\n",
-                "lcmap_pre = lcpri.filter(ee.Filter.calendarRange(preStartYear,preEndYear,'year')).mode()\n",
-                "lcmap_post = lcpri.filter(ee.Filter.calendarRange(postStartYear,postEndYear,'year')).mode()\n",
-                "\n",
-                "# Pull the LCMS pre and post land cover data\n",
-                "lcms_pre = ee.Image(lcms.filter(ee.Filter.calendarRange(preStartYear,preEndYear,'year')).mode().copyProperties(lcms.first()))\n",
-                "lcms_post = ee.Image(lcms.filter(ee.Filter.calendarRange(postStartYear,postEndYear,'year')).mode().copyProperties(lcms.first()))\n",
-                "\n",
-                "\n",
-                "\n",
-                "# Add time lapses of LCMAP and LCMS land cover products if specified\n",
-                "if addTimelapses:\n",
-                "  Map.addTimeLapse(lcachg,lc_viz,'LCMAP LC Change')\n",
-                "  Map.addTimeLapse(lcpri,lc_viz,'LCMAP Primary Land Cover')\n",
-                "  Map.addTimeLapse(lcsec,lc_viz,'LCMAP Secondary Land Cover')\n",
-                "  Map.addTimeLapse(lcms.select(['Land_Cover']),{'autoViz':True},'LCMS Land Cover')\n",
-                "  Map.addTimeLapse(lcms.select(['Land_Use']),{'autoViz':True},'LCMS Land Use')\n",
-                "\n",
-                "# Add the early and recent land cover and land use mode maps\n",
-                "# LCMAP's LC outputs combine land cover and land use, so cross-walking these non-mutually exclusive classes to those of LCMS can pose challenges\n",
-                "# However, take note how well LCMAP maps agriculture and developed areas - it is much cleaner and seems much more accurate than LCMS.\n",
-                "# LCMAP does about as well as LCMS at mapping trees. They both do fairly well in sparse tree cover areas.\n",
-                "# Since wetlands are not exclusive of any land cover or land use, it is difficult to tell what land cover is over areas classified by LCMAP as wetland\n",
-                "# This is also true of LCMS' non forest wetland land use class - there are areas of rangeland and agriculture that could fall into non forest wetland\n",
-                "# One area the LCMS land cover maps do better is with water. \n",
-                "# LCMAP LC outputs tend to not change the water extent of fluctuating waterbodies very quickly\n",
-                "Map.addLayer(lcmap_pre,lc_viz, 'LCMAP LC {}-{} mode'.format(preStartYear,preEndYear),False)\n",
-                "Map.addLayer(lcmap_post,lc_viz, 'LCMAP LC {}-{} mode'.format(postStartYear,postEndYear),False)\n",
+                "# Map.addTimeLapse(lcpri,lc_viz,'LCMAP Primary Land Cover')\n",
+                "# Map.addTimeLapse(lcsec,lc_viz,'LCMAP Secondary Land Cover')\n",
+                "Map.addTimeLapse(lcms.select(['Land_Cover']),{'autoViz':True},'LCMS Land Cover')\n",
+                "Map.addTimeLapse(lcms.select(['Land_Use']),{'autoViz':True},'LCMS Land Use')\n",
                 "\n",
-                "for t in ['Cover','Use']:\n",
-                "  Map.addLayer(lcms_pre.select(['Land_{}'.format(t)]),{'autoViz':True}, 'LCMS L{} {}-{} mode'.format(t[0],preStartYear,preEndYear),False)\n",
-                "  Map.addLayer(lcms_post.select(['Land_{}'.format(t)]),{'autoViz':True}, 'LCMS L{} {}-{} mode'.format(t[0],postStartYear,postEndYear),False)\n",
+                "Map.centerObject(ee.Geometry.Polygon(\n",
+                "        [[-115.39350883763947, 36.32737127837443],\n",
+                "          [-115.39350883763947, 35.90803695452136],\n",
+                "          [-114.27015678685822, 35.90803695452136],\n",
+                "          [-114.27015678685822, 36.32737127837443]], None, False))\n",
                 "\n",
                 "Map.turnOnInspector()\n",
-                "Map.view(open_browser = False, open_iframe = True)\n",
-                "Map.IFrame"
+                "Map.view()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 8,
-            "id": "ab46aaea",
+            "execution_count": 26,
+            "id": "e2a9f76b",
             "metadata": {
                 "scrolled": false
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Adding layer: LCMAP Primary Land Cover\n",
-                        "Adding layer: LCMS Land Cover\n",
-                        "Adding layer: LCMS Land Use\n",
+                        "Adding layer: LCMAP LC 1985-1990 mode\n",
+                        "Adding layer: LCMAP LC 2020-2021 mode\n",
+                        "Adding layer: LCMS LC 1985-1990 mode\n",
+                        "Adding layer: LCMS LC 2020-2021 mode\n",
+                        "Adding layer: LCMS LU 1985-1990 mode\n",
+                        "Adding layer: LCMS LU 2020-2021 mode\n",
                         "Starting webmap\n",
                         "Using default refresh token for geeView: C:\\Users\\ihousman/.config/earthengine/credentials\n",
                         "Local web server at: http://localhost:8001/geeView/ already serving.\n",
-                        "cwd A:\\GEE\\gee_py_modules_package\\geeViz\\examples\n"
+                        "cwd a:\\GEE\\gee_py_modules_package\\geeViz\\examples\n"
                     ]
                 },
                 {
                     "data": {
                         "text/html": [
                             "\n",
                             "        <iframe\n",
                             "            width=\"100%\"\n",
                             "            height=\"525px\"\n",
-                            "            src=\"http://localhost:8001/geeView/?accessToken=ya29.a0AVvZVso_a-Yclbne4HERkhzOzuZ-6wQ0egNnVV9puP_tdA2kS9R-1kWfS_ySDjElbRzHrLgWBRbm1cj6QkXJM99OMIIWK7lrn6KzSATql9oAxM36aKZI_M8nZjslgK7flQ-gK5pylALHmI5iEvBB57C4PMoJVW7vwOqecnkaCgYKAd4SARASFQGbdwaIXIXshBATXUlsGhXIzoXnlw0174\"\n",
+                            "            src=\"http://localhost:8001/geeView/?accessToken=ya29.a0AWY7Ckk13Ku-oksSYhxE7XNEmBp1BsXv3F91LUum-iavsvHHluUmF38lJa4nEi0Dm1Ls4s0szZFgfzMPLaFQSUBlMcuT7Uov3i-rc49j2tiaKUERGnk_nOCCZwRsJq3vdIcXe9ieXeEoaoSU8h76-OPUvJGR38_Hy6zitEkaCgYKAe4SARASFQG1tDrpHZab8RMlcNxLcOD7_qOZaQ0174\"\n",
                             "            frameborder=\"0\"\n",
                             "            allowfullscreen\n",
                             "            \n",
                             "        ></iframe>\n",
                             "        "
                         ],
                         "text/plain": [
-                            "<IPython.lib.display.IFrame at 0x1e21786e050>"
+                            "<IPython.lib.display.IFrame at 0x1c095d72080>"
                         ]
                     },
-                    "execution_count": 8,
                     "metadata": {},
-                    "output_type": "execute_result"
+                    "output_type": "display_data"
                 }
             ],
             "source": [
-                "# Add time lapses\n",
+                "#This section adds the land cover and land use maps from LCMAP and LCMS\n",
                 "\n",
                 "#First clear the map in case it has been populated with layers/commands earlier\n",
                 "Map.clearMap()\n",
                 "\n",
-                "Map.addTimeLapse(lcpri,lc_viz,'LCMAP Primary Land Cover')\n",
-                "# Map.addTimeLapse(lcsec,lc_viz,'LCMAP Secondary Land Cover')\n",
-                "Map.addTimeLapse(lcms.select(['Land_Cover']),{'autoViz':True},'LCMS Land Cover')\n",
-                "Map.addTimeLapse(lcms.select(['Land_Use']),{'autoViz':True},'LCMS Land Use')\n",
+                "# Set up some visualization dictionaries\n",
+                "lc_viz = {'min':1,'max':9,'palette':lcpri_palette,'classLegendDict':lc_legend_dict,'queryDict':lc_lookup_dict}\n",
+                "loss_viz = {'min':1985,'max':2022,'palette':changeDetectionLib.lossYearPalette}\n",
+                "gain_viz = {'min':1985,'max':2022,'palette':changeDetectionLib.gainYearPalette}\n",
+                "change_viz = {'min':1985,'max':2022,'palette':['00F','F0F']}\n",
                 "\n",
-                "Map.centerObject(ee.Geometry.Polygon(\n",
-                "        [[-115.39350883763947, 36.32737127837443],\n",
-                "          [-115.39350883763947, 35.90803695452136],\n",
-                "          [-114.27015678685822, 35.90803695452136],\n",
-                "          [-114.27015678685822, 36.32737127837443]], None, False))\n",
+                "\n",
+                "# Pull the LCMAP pre and post land cover data\n",
+                "lcmap_pre = lcpri.filter(ee.Filter.calendarRange(preStartYear,preEndYear,'year')).mode()\n",
+                "lcmap_post = lcpri.filter(ee.Filter.calendarRange(postStartYear,postEndYear,'year')).mode()\n",
+                "\n",
+                "# Pull the LCMS pre and post land cover data\n",
+                "lcms_pre = ee.Image(lcms.filter(ee.Filter.calendarRange(preStartYear,preEndYear,'year')).mode().copyProperties(lcms.first()))\n",
+                "lcms_post = ee.Image(lcms.filter(ee.Filter.calendarRange(postStartYear,postEndYear,'year')).mode().copyProperties(lcms.first()))\n",
+                "\n",
+                "\n",
+                "\n",
+                "# Add time lapses of LCMAP and LCMS land cover products if specified\n",
+                "if addTimelapses:\n",
+                "  Map.addTimeLapse(lcachg,lc_viz,'LCMAP LC Change')\n",
+                "  Map.addTimeLapse(lcpri,lc_viz,'LCMAP Primary Land Cover')\n",
+                "  Map.addTimeLapse(lcsec,lc_viz,'LCMAP Secondary Land Cover')\n",
+                "  Map.addTimeLapse(lcms.select(['Land_Cover']),{'autoViz':True},'LCMS Land Cover')\n",
+                "  Map.addTimeLapse(lcms.select(['Land_Use']),{'autoViz':True},'LCMS Land Use')\n",
+                "\n",
+                "# Add the early and recent land cover and land use mode maps\n",
+                "# LCMAP's LC outputs combine land cover and land use, so cross-walking these non-mutually exclusive classes to those of LCMS can pose challenges\n",
+                "# However, take note how well LCMAP maps agriculture and developed areas - it is much cleaner and seems much more accurate than LCMS.\n",
+                "# LCMAP does about as well as LCMS at mapping trees. They both do fairly well in sparse tree cover areas.\n",
+                "# Since wetlands are not exclusive of any land cover or land use, it is difficult to tell what land cover is over areas classified by LCMAP as wetland\n",
+                "# This is also true of LCMS' non forest wetland land use class - there are areas of rangeland and agriculture that could fall into non forest wetland\n",
+                "# One area the LCMS land cover maps do better is with water. \n",
+                "# LCMAP LC outputs tend to not change the water extent of fluctuating waterbodies very quickly\n",
+                "Map.addLayer(lcmap_pre,lc_viz, 'LCMAP LC {}-{} mode'.format(preStartYear,preEndYear),False)\n",
+                "Map.addLayer(lcmap_post,lc_viz, 'LCMAP LC {}-{} mode'.format(postStartYear,postEndYear),False)\n",
+                "\n",
+                "for t in ['Cover','Use']:\n",
+                "  Map.addLayer(lcms_pre.select(['Land_{}'.format(t)]),{'autoViz':True}, 'LCMS L{} {}-{} mode'.format(t[0],preStartYear,preEndYear),False)\n",
+                "  Map.addLayer(lcms_post.select(['Land_{}'.format(t)]),{'autoViz':True}, 'LCMS L{} {}-{} mode'.format(t[0],postStartYear,postEndYear),False)\n",
                 "\n",
                 "Map.turnOnInspector()\n",
-                "Map.view(open_browser = False, open_iframe = True)\n",
-                "Map.IFrame"
+                "Map.view()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 9,
+            "execution_count": 27,
             "id": "6ede8ab3",
             "metadata": {
                 "scrolled": false
             },
             "outputs": [
                 {
                     "name": "stdout",
@@ -373,36 +369,36 @@
                         "Adding layer: LCMS Most Recent Fast Loss Year\n",
                         "Adding layer: LCMS Most Recent Slow Loss Year\n",
                         "Adding layer: LCMS Most Recent Gain Year\n",
                         "Adding layer: LCMAP Most Recent SC Date\n",
                         "Starting webmap\n",
                         "Using default refresh token for geeView: C:\\Users\\ihousman/.config/earthengine/credentials\n",
                         "Local web server at: http://localhost:8001/geeView/ already serving.\n",
-                        "cwd A:\\GEE\\gee_py_modules_package\\geeViz\\examples\n"
+                        "cwd a:\\GEE\\gee_py_modules_package\\geeViz\\examples\n"
                     ]
                 },
                 {
                     "data": {
                         "text/html": [
                             "\n",
                             "        <iframe\n",
                             "            width=\"100%\"\n",
                             "            height=\"525px\"\n",
-                            "            src=\"http://localhost:8001/geeView/?accessToken=ya29.a0AVvZVspDTdjtXjoSDx65uSBwG1xYeQEUqNjrljCCkD5BeqjYoE4OLTs3a0WC8RvILQWqk0CjxNbgi95Sg6DavGXGp054uWh5L461pE5QI3UMSj1mrcsA5wn2wjZ4tPNeIJS6yv2eWbbpcdp6q27isC14K1Zy-Fr6vuBPryEaCgYKAcMSARASFQGbdwaIWy83yuEtbcsgNbeN0eo2Bw0174\"\n",
+                            "            src=\"http://localhost:8001/geeView/?accessToken=ya29.a0AWY7Ckn6ji4eSAKnyAW_1ObAikPSKmyP39WrLSNWhvo2Nvx3c9WhRV62Jy1UQ90vcdJhY2bQm8ZUrh2H4iPyc8tNFW3AzP70n1-31JyYPuplGsJLT9k7vHFaMctl7Ey187xEcx_Z4qNo1PV0-4dx3NsJ8lf3lOjfNR1R18caCgYKAfMSARASFQG1tDrpBBgsb49KKVymNMmoEJg-jg0174\"\n",
                             "            frameborder=\"0\"\n",
                             "            allowfullscreen\n",
                             "            \n",
                             "        ></iframe>\n",
                             "        "
                         ],
                         "text/plain": [
-                            "<IPython.lib.display.IFrame at 0x1e217866ce0>"
+                            "<IPython.lib.display.IFrame at 0x1c0960953c0>"
                         ]
                     },
-                    "execution_count": 9,
+                    "execution_count": 27,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# This section adds the change maps from LCMAP and LCMS\n",
                 "\n",
@@ -444,39 +440,36 @@
                 "          [-105.34101860326447, 41.00173645518866]]], None, False))\n",
                 "\n",
                 "\n",
                 "Map.turnOnInspector()\n",
                 "Map.view(open_browser = False, open_iframe = True)\n",
                 "Map.IFrame"
             ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "9df6efee",
-            "metadata": {},
-            "outputs": [],
-            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3 (ipykernel)",
+            "display_name": "Python 3",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
             "version": "3.10.0"
+        },
+        "vscode": {
+            "interpreter": {
+                "hash": "369f2c481f4da34e4445cda3fffd2e751bd1c4d706f27375911949ba6bb62e1c"
+            }
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `geeViz-2023.4.1/geeViz/examples/geeViewExample.py` & `geeViz-2023.6.1/geeViz/examples/geeViewExample.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.4.1/geeViz/examples/geeViewExampleNotebook.ipynb` & `geeViz-2023.6.1/geeViz/examples/geeViewExampleNotebook.ipynb`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9280647161188713%*

 * *Differences: {"'cells'": "{0: {'attachments': OrderedDict()}, 1: {'outputs': {0: {'text': {insert: [(1, 'geeViz "*

 * *            "package folder: c:\\\\Python310\\\\lib\\\\site-packages\\\\geeViz\\n')], delete: "*

 * *            "[1]}}}}, 2: {'execution_count': 4, 'outputs': {0: {'text': {insert: [(4, 'cwd "*

 * *            "a:\\\\GEE\\\\gee_py_modules_package\\\\geeViz\\\\examples\\n')], delete: [4]}}, 1: "*

 * *            "{'data': {'text/html': {insert: [(4, '            "*

 * *            'src="http://localhost:8001/geeView/?accessToke […]*

```diff
@@ -1,10 +1,11 @@
 {
     "cells": [
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "5dd7431b",
             "metadata": {},
             "source": [
                 "## Example of how to utilize the Python visualization tools\n",
                 "* Uses the stock GEE NLCD assets and extracts the palette, names, and values from image properties\n",
                 "* Then uses those to color the raster and create a legend using the autoViz option setting it to True\n",
@@ -36,15 +37,15 @@
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Initializing GEE\n",
-                        "geeViz package folder: C:\\Python310\\lib\\site-packages\\geeViz\n",
+                        "geeViz package folder: c:\\Python310\\lib\\site-packages\\geeViz\n",
                         "done\n"
                     ]
                 }
             ],
             "source": [
                 "#Import modules\n",
                 "import  geeViz.geeView as geeView\n",
@@ -52,50 +53,49 @@
                 "Map = geeView.Map\n",
                 "Map.clearMap()\n",
                 "print('done')"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 2,
+            "execution_count": 4,
             "id": "c91f7f74",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Adding layer: NLCD 2011 Landcover/Landuse\n",
                         "Starting webmap\n",
                         "Using default refresh token for geeView: C:\\Users\\ihousman/.config/earthengine/credentials\n",
                         "Local web server at: http://localhost:8001/geeView/ already serving.\n",
-                        "cwd A:\\GEE\\gee_py_modules_package\\geeViz\\examples\n"
+                        "cwd a:\\GEE\\gee_py_modules_package\\geeViz\\examples\n"
                     ]
                 },
                 {
                     "data": {
                         "text/html": [
                             "\n",
                             "        <iframe\n",
                             "            width=\"100%\"\n",
                             "            height=\"525px\"\n",
-                            "            src=\"http://localhost:8001/geeView/?accessToken=ya29.a0AVvZVsoYFxj2Qf6U6lgqa8quFW0kW6l-S35xxN5hdjkU3jYYBGIsPhMcWUJKUDbDGI8At2TuLPHw1PM24F7Ij5KWA2_uUV8310KqLId8CVIPQd70p-rMjJq2WVC1kUmiBTW3GSDC58M0V4diPXGxJfvgwPhcFGaaWnJ41tEaCgYKAWQSARASFQGbdwaIFBIhNMQy7jh-aeJd1KGeFA0174\"\n",
+                            "            src=\"http://localhost:8001/geeView/?accessToken=ya29.a0AWY7CkkX-HAJnVRfrHGZYjBr_W2b6zfRiMDXqIdXI1j_-o7aYo7yxdrL5f4PrGmE26otcE1lXJYttAAcI4rJbkHYS-q-Bn2y0AB0BrIKF2IoJhhuG4ZtGTupm9_hD9GE9wTFHMURZwRBs_4p98AbX_T4SlqjF7kKm9NEieAaCgYKAXcSARASFQG1tDrpNXzoLrnyIvERgN1eHI1L7w0174\"\n",
                             "            frameborder=\"0\"\n",
                             "            allowfullscreen\n",
                             "            \n",
                             "        ></iframe>\n",
                             "        "
                         ],
                         "text/plain": [
-                            "<IPython.lib.display.IFrame at 0x1c74367dc00>"
+                            "<IPython.lib.display.IFrame at 0x1ec2f996cb0>"
                         ]
                     },
-                    "execution_count": 2,
                     "metadata": {},
-                    "output_type": "execute_result"
+                    "output_type": "display_data"
                 }
             ],
             "source": [
                 "#Clear any layers added to Map object\n",
                 "#If map is not cleared, layers are simply appended to the existing list of layers if layers have been added previously\n",
                 "Map.clearMap()\n",
                 "#Bring in NLCD 2011\n",
@@ -110,60 +110,57 @@
                 "\n",
                 "#Can center map on a GEE object\n",
                 "Map.centerObject(nlcd)\n",
                 "\n",
                 "#Turn on inspector to double-click and see values of visible layers\n",
                 "Map.turnOnInspector()\n",
                 "\n",
-                "Map.view(open_browser = False, open_iframe = True)\n",
-                "Map.IFrame\n",
-                "# IFrame(src=\"http://localhost:8005/geeView/\", width='100%', height='500px')"
+                "Map.view()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 3,
+            "execution_count": 5,
             "id": "2670e5e4",
             "metadata": {
                 "scrolled": false
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Adding layer: NLCD Landcover/Landuse Time Series\n",
                         "Adding layer: NLCD 2016 TCC\n",
                         "Starting webmap\n",
                         "Using default refresh token for geeView: C:\\Users\\ihousman/.config/earthengine/credentials\n",
                         "Local web server at: http://localhost:8001/geeView/ already serving.\n",
-                        "cwd A:\\GEE\\gee_py_modules_package\\geeViz\\examples\n"
+                        "cwd a:\\GEE\\gee_py_modules_package\\geeViz\\examples\n"
                     ]
                 },
                 {
                     "data": {
                         "text/html": [
                             "\n",
                             "        <iframe\n",
                             "            width=\"100%\"\n",
                             "            height=\"525px\"\n",
-                            "            src=\"http://localhost:8001/geeView/?accessToken=ya29.a0AVvZVsppVWwdL0dZNUnXS5UexIS5-rQmQvWwPj3bsAI6IDFiG8P5s7tJY1SFYtReTx2UfvZ3RMG2ivjhNvj3kVlTh_fh0jVAy4tjaaJA8TOWOFHsqbp51PBIEIioPafhPt4ZDEKYrubdcAqPQUhEmT4_SY-juku5e-ZcWOUaCgYKAYcSARASFQGbdwaIfFoggkA369EG_NZN2Hz1PA0174\"\n",
+                            "            src=\"http://localhost:8001/geeView/?accessToken=ya29.a0AWY7CklTDu0Uy0iqqf58NYzMOV67oTwTkeDLbqra3uuTj_vqECqMG1ISfZ4W5zlL4Dxzpmdf0DGDBADDgQZiis4MJlnvno36JNqM80wKYoGxGXhragFxk9YAtzFZQljSiSUKvclvwHgo-oFa75iZJhalZhXsJ-2IdRqhyl8aCgYKAfYSARASFQG1tDrpz73yNcXXp2pd_aBg3fqrGQ0174\"\n",
                             "            frameborder=\"0\"\n",
                             "            allowfullscreen\n",
                             "            \n",
                             "        ></iframe>\n",
                             "        "
                         ],
                         "text/plain": [
-                            "<IPython.lib.display.IFrame at 0x1c74188a4a0>"
+                            "<IPython.lib.display.IFrame at 0x1ec2f9969b0>"
                         ]
                     },
-                    "execution_count": 3,
                     "metadata": {},
-                    "output_type": "execute_result"
+                    "output_type": "display_data"
                 }
             ],
             "source": [
                 "Map.clearMap()\n",
                 "#Images or image collections can be added.  If an image collection is added, the first non null value is displayed on the map. A time series will be displayed when the layer is queried\n",
                 "nlcd = ee.ImageCollection('USGS/NLCD_RELEASES/2016_REL')\n",
                 "nlcd = nlcd.filter(ee.Filter.calendarRange(2000,2020,'year'))\n",
@@ -172,58 +169,56 @@
                 "Map.addLayer(nlcd.sort('system:time_start'),{'autoViz':True},'NLCD Landcover/Landuse Time Series',True)\n",
                 "\n",
                 "# Continuous data automatically have a legend added\n",
                 "nlcd = ee.Image('USGS/NLCD_RELEASES/2016_REL/2016')\n",
                 "Map.addLayer(nlcd.select(['percent_tree_cover']),{'min':20,'max':80,'palette':'555,0A0','opacity':0.5},'NLCD 2016 TCC',True)\n",
                 "\n",
                 "Map.turnOnInspector()\n",
-                "Map.view(open_browser = False, open_iframe = True)\n",
-                "Map.IFrame"
+                "Map.view()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
+            "execution_count": 6,
             "id": "29550202",
             "metadata": {
                 "scrolled": false
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Adding layer: MTBS 1984-2017 Highest Severity\n",
                         "Starting webmap\n",
                         "Using default refresh token for geeView: C:\\Users\\ihousman/.config/earthengine/credentials\n",
                         "Local web server at: http://localhost:8001/geeView/ already serving.\n",
-                        "cwd A:\\GEE\\gee_py_modules_package\\geeViz\\examples\n"
+                        "cwd a:\\GEE\\gee_py_modules_package\\geeViz\\examples\n"
                     ]
                 },
                 {
                     "data": {
                         "text/html": [
                             "\n",
                             "        <iframe\n",
                             "            width=\"100%\"\n",
                             "            height=\"525px\"\n",
-                            "            src=\"http://localhost:8001/geeView/?accessToken=ya29.a0AVvZVso2-xxS1R5GqHxNASrjunOlVHe1zw4ADEWw06z8EEhUwkCwEX-8-w9NGd-I1LwMaD8Fgh8IMUbl7OuCaIiC47rxXJkPyGuFepfswXVDrT5QqhNJxnT0Fr-k0M522-4g-kk0f30njrQgXQcuuEj307GP6cr1O7pqu10aCgYKAdQSARASFQGbdwaINJCDFqYA0SN575zyGE84tQ0174\"\n",
+                            "            src=\"http://localhost:8001/geeView/?accessToken=ya29.a0AWY7CkmecFQekf5EilvXnBjVJq5YTurqxIlEd7ggwCUWhgCBFO014_NaVoyHUlMH8kScWeCYpPSqlYXw1iakguh4f4JmJQTg0Hsf4AR2Q4QVs9kLVYw5qLaXc1xJNgPlXAhWAPCMVU6Mm16aH_jXjXWKOHH40eSfCcVJwXIaCgYKAagSARASFQG1tDrp3C5HTjPkrrzzPVES5RR-qg0174\"\n",
                             "            frameborder=\"0\"\n",
                             "            allowfullscreen\n",
                             "            \n",
                             "        ></iframe>\n",
                             "        "
                         ],
                         "text/plain": [
-                            "<IPython.lib.display.IFrame at 0x1c74182f5e0>"
+                            "<IPython.lib.display.IFrame at 0x1ec318732b0>"
                         ]
                     },
-                    "execution_count": 4,
                     "metadata": {},
-                    "output_type": "execute_result"
+                    "output_type": "display_data"
                 }
             ],
             "source": [
                 "Map.clearMap()\n",
                 "#Another example\n",
                 "mtbs = ee.ImageCollection('projects/gtac-mtbs/assets/burn_severity_mosaics/MTBS')\n",
                 "mtbs = mtbs.map(lambda img: img.updateMask(img.neq(0)).select([0],['Burn Severity']).byte())\n",
@@ -235,164 +230,158 @@
                 "mtbsQueryDict = {'1':'Unburned to Low','2':'Low','3':'Moderate','4':'High','5':'Increased Greenness','6':'Non-Processing Area Mask'}\n",
                 "severityViz = {'min':1,'max':6,'palette':mtbsColors\t,'classLegendDict':mtbsDict,'queryDict':mtbsQueryDict}\n",
                 "\n",
                 "#Add it to the map\n",
                 "Map.addLayer(mtbs.max(),severityViz,'MTBS 1984-2017 Highest Severity',True)\n",
                 "\n",
                 "Map.turnOnInspector()\n",
-                "Map.view(open_browser = False, open_iframe = True)\n",
-                "Map.IFrame"
+                "Map.view()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
+            "execution_count": 7,
             "id": "bda0482c",
             "metadata": {
                 "scrolled": true
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Adding layer: MTBS Burn Perimeters\n",
                         "Starting webmap\n",
                         "Using default refresh token for geeView: C:\\Users\\ihousman/.config/earthengine/credentials\n",
                         "Local web server at: http://localhost:8001/geeView/ already serving.\n",
-                        "cwd A:\\GEE\\gee_py_modules_package\\geeViz\\examples\n"
+                        "cwd a:\\GEE\\gee_py_modules_package\\geeViz\\examples\n"
                     ]
                 },
                 {
                     "data": {
                         "text/html": [
                             "\n",
                             "        <iframe\n",
                             "            width=\"100%\"\n",
                             "            height=\"525px\"\n",
-                            "            src=\"http://localhost:8001/geeView/?accessToken=ya29.a0AVvZVsphtSy-IpHtqzCuBgNVRPyQY5bvkL-rn9Tq5FfcUDdgu6K02ewP-XktHowzDnAQRsq4ZgmJaBBm3rHKyzD9p5jnmFyD3fTU6eNdkZ3lI0YROjebuBVB64JI01idEK88n7rrzaZx0DM5dReSI1OUGThADgnqkg2JJyUaCgYKARkSARASFQGbdwaIutQD3yvxdf4SXvRXQGFR_g0174\"\n",
+                            "            src=\"http://localhost:8001/geeView/?accessToken=ya29.a0AWY7Ckn8l5yQeCyu11KyDwx0kQja2Jg5NoQYZ5jPg3r2PM1s1mE0WybDJSkcsI765anymlkWHYS5boIdT6bXGL-RYKxC_chbpI-VSP7vtwqGvqYUFsK5ceKn46rySL8k59uBijtKJ-HptrW0K6kIWULhBThPMvrZhIt-2RkaCgYKASoSARASFQG1tDrpJiLoGYKCPIaQf0U6pYPNwA0174\"\n",
                             "            frameborder=\"0\"\n",
                             "            allowfullscreen\n",
                             "            \n",
                             "        ></iframe>\n",
                             "        "
                         ],
                         "text/plain": [
-                            "<IPython.lib.display.IFrame at 0x1c7436a0a90>"
+                            "<IPython.lib.display.IFrame at 0x1ec31752cb0>"
                         ]
                     },
-                    "execution_count": 5,
                     "metadata": {},
-                    "output_type": "execute_result"
+                    "output_type": "display_data"
                 }
             ],
             "source": [
                 "#Feature collections can be added to the map as well\n",
                 "#If they are very large, the geeVectorImage option is needed as the conversion from GEE object to geoJSON is too slow\n",
                 "#Instead of clearing the map, this time, we'll add it to the existing map above\n",
                 "perims = ee.FeatureCollection('projects/gtac-mtbs/assets/perimeters/mtbs_perims_DD')\n",
                 "Map.addLayer(perims,{'strokeColor':'00F','layerType':'geeVectorImage'},'MTBS Burn Perimeters',True)\n",
                 "\n",
                 "#Double click to see raster value of burn severity, as well as the attribute table of the feature\n",
-                "Map.view(open_browser = False, open_iframe = True)\n",
-                "Map.IFrame"
+                "Map.view()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 6,
+            "execution_count": 8,
             "id": "e3065817",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Adding layer: Yellowstone National Park\n",
                         "Starting webmap\n",
                         "Using default refresh token for geeView: C:\\Users\\ihousman/.config/earthengine/credentials\n",
                         "Local web server at: http://localhost:8001/geeView/ already serving.\n",
-                        "cwd A:\\GEE\\gee_py_modules_package\\geeViz\\examples\n"
+                        "cwd a:\\GEE\\gee_py_modules_package\\geeViz\\examples\n"
                     ]
                 },
                 {
                     "data": {
                         "text/html": [
                             "\n",
                             "        <iframe\n",
                             "            width=\"100%\"\n",
                             "            height=\"525px\"\n",
-                            "            src=\"http://localhost:8001/geeView/?accessToken=ya29.a0AVvZVsp0R7A-nevCs7DQ1t1wecNPRm-QHomguM5qSXS-2aZJAcVs9qcEZwaM4CBb_htf0oVnd9JOIZ3XwB1GLTXx6Q0AGzEAkVHCDuF9H975k4JGXye9sAiMQ7t_HJZhu-aqV6q936nqeKIQuEv25CZ3hMxLubyxhEmnZBIaCgYKAVASARASFQGbdwaI25_s8hDWgTqW1hxQvzOiig0174\"\n",
+                            "            src=\"http://localhost:8001/geeView/?accessToken=ya29.a0AWY7CkkiE_XUBgiP2O3R1JKK1IKphww-eQHXfAHEsmLA7cBk_JRUzERQuh4A6dif7CcUEtZyl6zNI7byzsvmwh2QljFdNq8G_JPs6sW70wnr-hxuZpP1WVOLJsL42mURQ5_WX_byAIxXwrSjy4QmiCRLdDNP9tZ8Mv-wgsMaCgYKAToSARASFQG1tDrpmRT2nxOF1w1qRF7oGuy-YA0174\"\n",
                             "            frameborder=\"0\"\n",
                             "            allowfullscreen\n",
                             "            \n",
                             "        ></iframe>\n",
                             "        "
                         ],
                         "text/plain": [
-                            "<IPython.lib.display.IFrame at 0x1c74367eaa0>"
+                            "<IPython.lib.display.IFrame at 0x1ec31873d00>"
                         ]
                     },
-                    "execution_count": 6,
                     "metadata": {},
-                    "output_type": "execute_result"
+                    "output_type": "display_data"
                 }
             ],
             "source": [
                 "Map.clearMap()\n",
                 "#Smaller feature collections can be added to the map as a geojson vector by specifying 'layerType':'geeVector'\n",
                 "#They will render more quickly than the raterized version of the vector\n",
                 "nps = ee.FeatureCollection('projects/USFS/LCMS-NFS/CONUS-Ancillary-Data/NPS_Boundaries').filter(ee.Filter.eq('PARKNAME','Yellowstone'))\n",
                 "Map.addLayer(nps,{'layerType': 'geeVector'},'Yellowstone National Park',True)\n",
                 "Map.centerObject(nps)\n",
                 "Map.turnOnInspector()\n",
-                "Map.view(open_browser = False, open_iframe = True)\n",
-                "Map.IFrame"
+                "Map.view()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
+            "execution_count": 9,
             "id": "ed19b1f3",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Adding layer: JRC Surface Water Time Series\n",
                         "Adding layer: JRC Surface Water Mode\n",
                         "Adding layer: JRC Surface Water Time Lapse\n",
                         "Starting webmap\n",
                         "Using default refresh token for geeView: C:\\Users\\ihousman/.config/earthengine/credentials\n",
                         "Local web server at: http://localhost:8001/geeView/ already serving.\n",
-                        "cwd A:\\GEE\\gee_py_modules_package\\geeViz\\examples\n"
+                        "cwd a:\\GEE\\gee_py_modules_package\\geeViz\\examples\n"
                     ]
                 },
                 {
                     "data": {
                         "text/html": [
                             "\n",
                             "        <iframe\n",
                             "            width=\"100%\"\n",
                             "            height=\"525px\"\n",
-                            "            src=\"http://localhost:8001/geeView/?accessToken=ya29.a0AVvZVsrOQQJaBWMosZCYcGx9c_9-Jhgy9_0HieC_t90KX7JLX3ndp96mw--fbDSlLZyQ2Zm7E6XMdfjMvsWNKVsLqcbX7RYp5BbmpZPUbrDLxvB1dBlpMRzc-VLpW9PgtDxRv5SJ73aqtTshbUXLAuoiFF4dTT1FGBbk8p0aCgYKAcYSARASFQGbdwaI6ySyKbjCLG8YNYlipQXmMA0174\"\n",
+                            "            src=\"http://localhost:8001/geeView/?accessToken=ya29.a0AWY7CklWxqm4OGJ130H501a9aRa1nIYUs29BQsRPt2qhbYga1z4DHyWppLAQRZSB6PCxnrV3y02uenpD5_GGPRc9fPIYrO-ME9RH7nIVZwpeqYVFxNT8VvYMKW5o1aVrev1_ZK8cJBIilI--8zkQO4fwtbIwNVWoNzHAApIaCgYKAWoSARASFQG1tDrpC2ZvfKx8cS7vOfswtMF_HA0174\"\n",
                             "            frameborder=\"0\"\n",
                             "            allowfullscreen\n",
                             "            \n",
                             "        ></iframe>\n",
                             "        "
                         ],
                         "text/plain": [
-                            "<IPython.lib.display.IFrame at 0x1c7436a06a0>"
+                            "<IPython.lib.display.IFrame at 0x1ec2f996f80>"
                         ]
                     },
-                    "execution_count": 7,
                     "metadata": {},
-                    "output_type": "execute_result"
+                    "output_type": "display_data"
                 }
             ],
             "source": [
                 "Map.clearMap()\n",
                 "#An interactive time lapse can also be created from an annual image collection\n",
                 "#Bring in the JRS Surface water data\n",
                 "water = ee.ImageCollection('JRC/GSW1_0/YearlyHistory')\n",
@@ -404,42 +393,38 @@
                 "waterQueryDict =  {str(i+1): waterLabels[i] for i in range(len(waterLabels))}\n",
                 "\n",
                 "#The lookup table is applied to the image, but only a graph is created when querying the imageCollection\n",
                 "Map.addLayer(water,{'min':1,'max':3,'palette':waterColors,'classLegendDict':waterDict,'queryDict':waterQueryDict},'JRC Surface Water Time Series',False)\n",
                 "Map.addLayer(water.mode(),{'min':1,'max':3,'palette':waterColors,'classLegendDict':waterDict,'queryDict':waterQueryDict},'JRC Surface Water Mode',True)\n",
                 "Map.addTimeLapse(water,{'min':1,'max':3,'palette':waterColors,'classLegendDict':waterDict},'JRC Surface Water Time Lapse',False)\n",
                 "Map.centerObject(water)\n",
-                "Map.view(False,True)\n",
-                "Map.IFrame"
+                "Map.view()"
             ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "6cea3da6",
-            "metadata": {},
-            "outputs": [],
-            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3 (ipykernel)",
+            "display_name": "Python 3",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
             "version": "3.10.0"
+        },
+        "vscode": {
+            "interpreter": {
+                "hash": "369f2c481f4da34e4445cda3fffd2e751bd1c4d706f27375911949ba6bb62e1c"
+            }
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `geeViz-2023.4.1/geeViz/examples/getClimateWrapper.py` & `geeViz-2023.6.1/geeViz/examples/getClimateWrapper.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.4.1/geeViz/examples/getCombinedLandsatSentinel2Wrapper.py` & `geeViz-2023.6.1/geeViz/examples/getCombinedLandsatSentinel2Wrapper.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.4.1/geeViz/examples/getLandsatWrapper.py` & `geeViz-2023.6.1/geeViz/examples/getLandsatWrapper.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.4.1/geeViz/examples/getLandsatWrapperNotebook.ipynb` & `geeViz-2023.6.1/geeViz/examples/getLandsatWrapperNotebook.ipynb`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9906393368746939%*

 * *Differences: {"'cells'": "{0: {'attachments': OrderedDict()}, 1: {'execution_count': 1, 'outputs': {0: {'text': "*

 * *            "{insert: [(0, 'Initializing GEE\\n'), (1, 'geeViz package folder: "*

 * *            "c:\\\\Python310\\\\lib\\\\site-packages\\\\geeViz\\n')]}}}}, 2: {'outputs': {0: "*

 * *            "{'text': {insert: [(12, 'Local web server at: http://localhost:8001/geeView/ already "*

 * *            "serving.\\n'), (13, 'cwd "*

 * *            "a:\\\\GEE\\\\gee_py_modules_package\\\\geeViz\\\\examples\\n')], delete: [15, 14,  […]*

```diff
@@ -1,10 +1,11 @@
 {
     "cells": [
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "3cf7f21d",
             "metadata": {},
             "source": [
                 "Copyright 2023 Ian Housman\n",
                 "\n",
                 "Licensed under the Apache License, Version 2.0 (the \"License\");\n",
@@ -18,22 +19,24 @@
                 "WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.\n",
                 "See the License for the specific language governing permissions and\n",
                 "limitations under the License."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 2,
+            "execution_count": 1,
             "id": "ce3c6688",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
+                        "Initializing GEE\n",
+                        "geeViz package folder: c:\\Python310\\lib\\site-packages\\geeViz\n",
                         "done\n"
                     ]
                 }
             ],
             "source": [
                 "#Example of how to get Landsat data using the getImagesLib and view outputs using the Python visualization tools\n",
                 "#Acquires Landsat data and then adds them to the viewer\n",
@@ -69,41 +72,38 @@
                         "Applying scale factors for C2 L7 data\n",
                         "Applying scale factors for C2 L9 data\n",
                         "Applying Fmask Cloud Mask\n",
                         "Applying Fmask Shadow Mask\n",
                         "Adding layer: Default Params 2009 153-152\n",
                         "Starting webmap\n",
                         "Using default refresh token for geeView: C:\\Users\\ihousman/.config/earthengine/credentials\n",
-                        "Starting local web server at: http://localhost:8001/geeView/\n",
-                        "HTTP server command: \"C:\\Python310\\python.exe\" -m http.server  8001\n",
-                        "Done\n",
-                        "cwd A:\\GEE\\gee_py_modules_package\\geeViz\\examples\n"
+                        "Local web server at: http://localhost:8001/geeView/ already serving.\n",
+                        "cwd a:\\GEE\\gee_py_modules_package\\geeViz\\examples\n"
                     ]
                 },
                 {
                     "data": {
                         "text/html": [
                             "\n",
                             "        <iframe\n",
                             "            width=\"100%\"\n",
                             "            height=\"525px\"\n",
-                            "            src=\"http://localhost:8001/geeView/?accessToken=ya29.a0AVvZVsonUwnG1L3Jaux-cCqyPQ0vBetqy0xXJFygPnoQmPNjIUvg_zmS2kprCD_sb0KGcjN3tJXn13A-gdwwKZwJYneE6_G7aFExinMO6LJ5HAIsgw0qev1oryy-J3yoO5cWPoK-B2TM86-wrcZpZCWkKJYIv2tyTqvRgnUaCgYKAaoSARASFQGbdwaIE_437ZwKZagcpwInRv0zug0174\"\n",
+                            "            src=\"http://localhost:8001/geeView/?accessToken=ya29.a0AWY7CklgQoy3b1zWeVTTq0l5mbVa1Cg1wySFANflqkxRT9hoe3SzhREZzU0WDYgj9Tgt2wj7sQwEnemkl-TAOXXsP1T2gIA7IYxh5rWq5PIM6muzS2NSM-0lITbEMtpyv9mwM1xD7qTUt9CPpbcdmyCLd0d2M_KnlidymkUaCgYKAU0SARASFQG1tDrpLQSb1vbkvaQLScrdV5fHjA0174\"\n",
                             "            frameborder=\"0\"\n",
                             "            allowfullscreen\n",
                             "            \n",
                             "        ></iframe>\n",
                             "        "
                         ],
                         "text/plain": [
-                            "<IPython.lib.display.IFrame at 0x1dfebac6fb0>"
+                            "<IPython.lib.display.IFrame at 0x220174e5870>"
                         ]
                     },
-                    "execution_count": 3,
                     "metadata": {},
-                    "output_type": "execute_result"
+                    "output_type": "display_data"
                 }
             ],
             "source": [
                 "#This example will use all default parameters to demonstrate how to use the basic composite functionality\n",
                 "\n",
                 "#First clear the map in case it has been populated with layers/commands earlier\n",
                 "Map.clearMap()\n",
@@ -148,16 +148,15 @@
                 "\n",
                 "Map.centerObject(ee.Geometry.Polygon(\n",
                 "        [[[-65.8337045819611, 18.329538797654042],\n",
                 "          [-65.8337045819611, 18.235653085671174],\n",
                 "          [-65.70461522649235, 18.235653085671174],\n",
                 "          [-65.70461522649235, 18.329538797654042]]], None, False))\n",
                 "Map.turnOnInspector()\n",
-                "Map.view(open_browser = False, open_iframe = True)\n",
-                "Map.IFrame\n",
+                "Map.view()\n",
                 "\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 4,
             "id": "48dc6ee9",
@@ -200,38 +199,37 @@
                         "Applying scale factors for C2 L9 data\n",
                         "Applying Fmask Cloud Mask\n",
                         "Applying Fmask Shadow Mask\n",
                         "Adding layer: L7 added 2009 153-152\n",
                         "Starting webmap\n",
                         "Using default refresh token for geeView: C:\\Users\\ihousman/.config/earthengine/credentials\n",
                         "Local web server at: http://localhost:8001/geeView/ already serving.\n",
-                        "cwd A:\\GEE\\gee_py_modules_package\\geeViz\\examples\n"
+                        "cwd a:\\GEE\\gee_py_modules_package\\geeViz\\examples\n"
                     ]
                 },
                 {
                     "data": {
                         "text/html": [
                             "\n",
                             "        <iframe\n",
                             "            width=\"100%\"\n",
                             "            height=\"525px\"\n",
-                            "            src=\"http://localhost:8001/geeView/?accessToken=ya29.a0AVvZVsqOxk6PX9FZ2-Owan6q4tJcXuh2cX07bm7ljgRINe4D7lkVg3ubOQM6z2h93cZ_C-t0fHyM3Kc5nX9Wa-mauYjfOq5XIvtHbZ1Kfm8-vfKxPqPOrJnH4TVSLpqbDeLnRZdQs1o9AkBOhcXpGjwhRtj69Xiud2K_gkYaCgYKAY0SARASFQGbdwaIeNr9Sk2piISrKkhu8d8iuQ0174\"\n",
+                            "            src=\"http://localhost:8001/geeView/?accessToken=ya29.a0AWY7Ckkp8ntha8NiS4f8rQCxmRX1gpnq6CatRSGQjg6uglVbdBOyIvDVfey3rpV3vGls96ESyKlXsd8gJI6Iv8e0BzPgBQU_qTHsmKgXXCWD8OdjAxyXliW6c34N0qhZKO7t0R7LMM05wths_Q8Xr12o_TmSSKO911QUj5AaCgYKAb0SARASFQG1tDrpmMxx_58u8nhJ4ymTFLI8qA0174\"\n",
                             "            frameborder=\"0\"\n",
                             "            allowfullscreen\n",
                             "            \n",
                             "        ></iframe>\n",
                             "        "
                         ],
                         "text/plain": [
-                            "<IPython.lib.display.IFrame at 0x1dfe9d1cc70>"
+                            "<IPython.lib.display.IFrame at 0x2201752d720>"
                         ]
                     },
-                    "execution_count": 5,
                     "metadata": {},
-                    "output_type": "execute_result"
+                    "output_type": "display_data"
                 }
             ],
             "source": [
                 "#Since there are not that many images available in this area for these years, let's try adding Landsat 7\n",
                 "includeSLCOffL7 = True\n",
                 "#Call on master wrapper function to get Landat scenes and composites\n",
                 "lsAndTs = getImagesLib.getLandsatWrapper(studyArea,startYear,endYear,startJulian,endJulian,includeSLCOffL7=includeSLCOffL7)\n",
@@ -246,16 +244,15 @@
                 "\n",
                 "# Map.addLayer(processedComposites.select(['NDVI','NBR']),{'addToLegend':'false'},'Time Series (NBR and NDVI)',False)\n",
                 "for year in range(startYear,endYear + 1 ):\n",
                 "     t = processedComposites.filter(ee.Filter.calendarRange(year,year,'year')).mosaic()\n",
                 "     Map.addLayer(t.float(),getImagesLib.vizParamsFalse,'L7 added {} {}-{}'.format(year,startJulian,endJulian),'True')\n",
                 "\n",
                 "\n",
-                "Map.view(open_browser = False, open_iframe = True)\n",
-                "Map.IFrame\n",
+                "Map.view()\n",
                 "\n",
                 "#You'll notice this helps fill in the holes, but introduces many cloud-related artifacts"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 6,
@@ -277,38 +274,37 @@
                         "Computing cloudScore offset\n",
                         "Applying Fmask Cloud Mask\n",
                         "Applying Fmask Shadow Mask\n",
                         "Adding layer: L7 and CloudScore added 2009 153-152\n",
                         "Starting webmap\n",
                         "Using default refresh token for geeView: C:\\Users\\ihousman/.config/earthengine/credentials\n",
                         "Local web server at: http://localhost:8001/geeView/ already serving.\n",
-                        "cwd A:\\GEE\\gee_py_modules_package\\geeViz\\examples\n"
+                        "cwd a:\\GEE\\gee_py_modules_package\\geeViz\\examples\n"
                     ]
                 },
                 {
                     "data": {
                         "text/html": [
                             "\n",
                             "        <iframe\n",
                             "            width=\"100%\"\n",
                             "            height=\"525px\"\n",
-                            "            src=\"http://localhost:8001/geeView/?accessToken=ya29.a0AVvZVsqndJaOP68J7DoEyR063yMLh2LXoIiB3qC-V33oIctVvqm4u-tgjDXibyaxvE4pDd78ZYejmHxBCB6919K_wnDyUxvFzUthAYHhOb2qtLxtHJR1xAsvwI6gD7TVOySewKAfXB37dQWDJEdJkixU_TzYYCnToUU_ATkaCgYKAQsSARASFQGbdwaIk0_16zj_NAGcE4ZxVMdkaw0174\"\n",
+                            "            src=\"http://localhost:8001/geeView/?accessToken=ya29.a0AWY7Ckk9GF6sOSzBSRRiv8Y-yv-YK6sWh22de8WWOmhkclmdDigJlVJ6xQXyPAdgtJRKVAKAtuRqs8KVkMQ4V8L_qPPl-IycxfWdfQezirNIxzX6Mizzi_8gc5_YdLk86cdCJh1paAgW9mazc499b5HOBuqNUYQG-_F77RAaCgYKAX4SARASFQG1tDrplvbYY7-o7iAlPL5kEtmeww0174\"\n",
                             "            frameborder=\"0\"\n",
                             "            allowfullscreen\n",
                             "            \n",
                             "        ></iframe>\n",
                             "        "
                         ],
                         "text/plain": [
-                            "<IPython.lib.display.IFrame at 0x1dfebb13be0>"
+                            "<IPython.lib.display.IFrame at 0x220174b0190>"
                         ]
                     },
-                    "execution_count": 6,
                     "metadata": {},
-                    "output_type": "execute_result"
+                    "output_type": "display_data"
                 }
             ],
             "source": [
                 "#Let's try to improve the cloud masking. Fmask is used by default, but misses some clouds\n",
                 "#We'll try the adding in the cloudScore method\n",
                 "applyCloudScore = True\n",
                 "\n",
@@ -325,16 +321,15 @@
                 "\n",
                 "# Map.addLayer(processedComposites.select(['NDVI','NBR']),{'addToLegend':'false'},'Time Series (NBR and NDVI)',False)\n",
                 "for year in range(startYear,endYear + 1 ):\n",
                 "     t = processedComposites.filter(ee.Filter.calendarRange(year,year,'year')).mosaic()\n",
                 "     Map.addLayer(t.float(),getImagesLib.vizParamsFalse,'L7 and CloudScore added {} {}-{}'.format(year,startJulian,endJulian),'True')\n",
                 "\n",
                 "\n",
-                "Map.view(open_browser = False, open_iframe = True)\n",
-                "Map.IFrame\n",
+                "Map.view()\n",
                 "\n",
                 "#You'll notice this cleans up the cloud masking a lot"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 7,
@@ -359,38 +354,37 @@
                         "Computing irMean for TDOM\n",
                         "Computing irStdDev for TDOM\n",
                         "Applying Fmask Shadow Mask\n",
                         "Adding layer: CloudScore and TDOM added 2009 153-152\n",
                         "Starting webmap\n",
                         "Using default refresh token for geeView: C:\\Users\\ihousman/.config/earthengine/credentials\n",
                         "Local web server at: http://localhost:8001/geeView/ already serving.\n",
-                        "cwd A:\\GEE\\gee_py_modules_package\\geeViz\\examples\n"
+                        "cwd a:\\GEE\\gee_py_modules_package\\geeViz\\examples\n"
                     ]
                 },
                 {
                     "data": {
                         "text/html": [
                             "\n",
                             "        <iframe\n",
                             "            width=\"100%\"\n",
                             "            height=\"525px\"\n",
-                            "            src=\"http://localhost:8001/geeView/?accessToken=ya29.a0AVvZVsox9OFPstE7374TsaoFeKgCUDEFhfCwlOfUZlbHEuAugFPRAwiDFPBLvX0quZ_kV0Wn56n3TagHkHigURxQLjZRIB0ygqJIgXu24BxrXqE-rXT-wgjMVKGHYQXr4F-R9Em5pS-rPkqqz8ZxyhwG27l5pz_pjUYPB3IaCgYKAQgSARASFQGbdwaI0O6DSoI1lc3j_ZpaV0zayA0174\"\n",
+                            "            src=\"http://localhost:8001/geeView/?accessToken=ya29.a0AWY7CkkjAUiWVCidNln_3yK4YC-nBSCUfowMnmwD53N0aFm46kgPqd4k1a1xP45frSre_zw7L9Bl-i2Vvzhdu85EcLvW1Bpu9iAsg0T9WJkE1RT8w4fKHkKIyMZNwWg7m1tGcV0mOBjZFM9BUSlkXKMLXKr2O0OXsM8RsgUaCgYKASASARASFQG1tDrpW-jWwyopjLk-G2mZdXUtiQ0174\"\n",
                             "            frameborder=\"0\"\n",
                             "            allowfullscreen\n",
                             "            \n",
                             "        ></iframe>\n",
                             "        "
                         ],
                         "text/plain": [
-                            "<IPython.lib.display.IFrame at 0x1dfebac7c70>"
+                            "<IPython.lib.display.IFrame at 0x220174da470>"
                         ]
                     },
-                    "execution_count": 7,
                     "metadata": {},
-                    "output_type": "execute_result"
+                    "output_type": "display_data"
                 }
             ],
             "source": [
                 "#You'll still notice there are some dark areas likely due to cloud shadow masking omission\n",
                 "#Fmasks's cloud shadow mask misses a lot typically. A temporal outlier method called the \n",
                 "#Temporal Dark Outlier Mask (TDOM) works well with masking cloud shadows\n",
                 "\n",
@@ -411,21 +405,21 @@
                 "\n",
                 "# Map.addLayer(processedComposites.select(['NDVI','NBR']),{'addToLegend':'false'},'Time Series (NBR and NDVI)',False)\n",
                 "for year in range(startYear,endYear + 1 ):\n",
                 "     t = processedComposites.filter(ee.Filter.calendarRange(year,year,'year')).mosaic()\n",
                 "     Map.addLayer(t.float(),getImagesLib.vizParamsFalse,'CloudScore and TDOM added {} {}-{}'.format(year,startJulian,endJulian),'True')\n",
                 "\n",
                 "\n",
-                "Map.view(open_browser = False, open_iframe = True)\n",
-                "Map.IFrame\n",
+                "Map.view()\n",
                 "\n",
                 "#You'll notice this cleans up the cloud masking a lot"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "fca2146c",
             "metadata": {},
             "source": [
                 "> There are many different parameters that can be changed in order to improve composites in different study areas\n",
                 "> This is just one example. Other parameters include changing date ranges, and reducers"
             ]
```

### Comparing `geeViz-2023.4.1/geeViz/examples/getSentinel2Wrapper.py` & `geeViz-2023.6.1/geeViz/examples/getSentinel2Wrapper.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.4.1/geeViz/examples/harmonicRegressionWrapper.py` & `geeViz-2023.6.1/geeViz/examples/harmonicRegressionWrapper.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.4.1/geeViz/examples/lcmsViewerExample.py` & `geeViz-2023.6.1/geeViz/examples/lcmsViewerExample.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,16 +32,16 @@
 Map = geeView.Map
 
 Map.clearMap()
 ####################################################################################################
 #############################################################################
 ### Define visualization parameters ###
 #############################################################################
-startYear = 1985;
-endYear = 2021;
+startYear = 1985
+endYear = 2022
 lossYearPalette = ['ffffe5', 'fff7bc', 'fee391', 'fec44f', 'fe9929',
                    'ec7014', 'cc4c02']
 gainYearPalette = ['c5ee93', '00a398']
 durationPalette = ['BD1600', 'E2F400','0C2780']
 
 lossYearViz = {'min': startYear, 'max': endYear, 'palette': lossYearPalette};
 gainYearViz = {'min': startYear, 'max': endYear, 'palette': gainYearPalette};
@@ -59,15 +59,15 @@
 	return c.map(wrapper)
   
 
 #############################################################################
 ### Bring in LCMS annual outputs ###
 #############################################################################
 
-lcms = ee.ImageCollection('USFS/GTAC/LCMS/v2021-7');
+lcms = ee.ImageCollection('USFS/GTAC/LCMS/v2022-8')
 bandNames =  lcms.first().bandNames().getInfo()
 print('Available study areas:', lcms.aggregate_histogram('study_area').keys().getInfo());
 print('Available LCMS products',bandNames);
 print('Learn more about visualization of LCMS products here', 'https://apps.fs.usda.gov/lcms-viewer/')
 
 #Filter out study area
 lcms = lcms.filter(ee.Filter.eq('study_area','CONUS'))
```

### Comparing `geeViz-2023.4.1/geeViz/examples/lcmsViewerExampleNotebook.ipynb` & `geeViz-2023.6.1/geeViz/examples/lcmsViewerExampleNotebook.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9974716421312517%*

 * *Differences: {"'cells'": "{1: {'outputs': {0: {'text': {insert: [(1, 'geeViz package folder: "*

 * *            "c:\\\\Python310\\\\lib\\\\site-packages\\\\geeViz\\n')], delete: [1]}}}}, 3: "*

 * *            "{'source': {insert: [(8, 'endYear = 2022;\\n')], delete: [8]}}, 4: {'source': "*

 * *            '{insert: [(4, "lcms = ee.ImageCollection(\'USFS/GTAC/LCMS/v2022-8\');\\n")], delete: '*

 * *            "[4]}}, 5: {'attachments': OrderedDict()}}"}*

```diff
@@ -32,15 +32,15 @@
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Initializing GEE\n",
-                        "geeViz package folder: c:\\python38\\lib\\site-packages\\geeViz\n",
+                        "geeViz package folder: c:\\Python310\\lib\\site-packages\\geeViz\n",
                         "Done\n"
                     ]
                 }
             ],
             "source": [
                 "#Boiler plate\n",
                 "#Import modules\n",
@@ -99,15 +99,15 @@
                 "#If map is not cleared, layers are simply appended to the existing list of layers if layers have been added previously\n",
                 "Map.clearMap()\n",
                 "\n",
                 "#############################################################################\n",
                 "### Define visualization parameters ###\n",
                 "#############################################################################\n",
                 "startYear = 1985;\n",
-                "endYear = 2020;\n",
+                "endYear = 2022;\n",
                 "lossYearPalette = ['ffffe5', 'fff7bc', 'fee391', 'fec44f', 'fe9929',\n",
                 "                   'ec7014', 'cc4c02']\n",
                 "gainYearPalette = ['c5ee93', '00a398']\n",
                 "durationPalette = ['BD1600', 'E2F400','0C2780']\n",
                 "\n",
                 "lossYearViz = {'min': startYear, 'max': endYear, 'palette': lossYearPalette};\n",
                 "gainYearViz = {'min': startYear, 'max': endYear, 'palette': gainYearPalette};\n",
@@ -142,29 +142,30 @@
                 }
             ],
             "source": [
                 "#############################################################################\n",
                 "### Bring in LCMS annual outputs ###\n",
                 "#############################################################################\n",
                 "\n",
-                "lcms = ee.ImageCollection('USFS/GTAC/LCMS/v2020-5');\n",
+                "lcms = ee.ImageCollection('USFS/GTAC/LCMS/v2022-8');\n",
                 "bandNames =  lcms.first().bandNames().getInfo()\n",
                 "print('Available study areas:', lcms.aggregate_histogram('study_area').keys().getInfo());\n",
                 "print('Available LCMS products',bandNames);\n",
                 "print('Learn more about visualization of LCMS products here', 'https://apps.fs.usda.gov/lcms-viewer/')\n",
                 "\n",
                 "#Filter out study area\n",
                 "# lcms = lcms.filter(ee.Filter.eq('study_area','CONUS'))\n",
                 "\n",
                 "#Set up time periods to compare land cover and land use\n",
                 "earlySpan = [startYear, startYear+4]\n",
                 "lateSpan = [endYear-4, endYear]\n"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "b9aa0633",
             "metadata": {},
             "source": [
                 "---\n",
                 "* Raw LCMS outputs are available for more customized analysis\n",
                 "* Double click anywhere within CONUS to plot the time series of raw LCMS outputs"
```

### Comparing `geeViz-2023.4.1/geeViz/examples/phEEnoVizWrapper.py` & `geeViz-2023.6.1/geeViz/examples/phEEnoVizWrapper.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.4.1/geeViz/examples/taskTrackerExample.py` & `geeViz-2023.6.1/geeViz/examples/taskTrackerExample.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.4.1/geeViz/examples/timeLapseExample.py` & `geeViz-2023.6.1/geeViz/examples/timeLapseExample.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.4.1/geeViz/gcpLib.py` & `geeViz-2023.6.1/geeViz/gcpLib.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.4.1/geeViz/geeView/css/style.min.css` & `geeViz-2023.6.1/geeViz/geeView/css/style.min.css`

 * *Files 16% similar despite different names*

```diff
@@ -1 +1 @@
-@import "https://fonts.googleapis.com/css?family=Roboto+Condensed&display=swap";:root{--teal-30:#B2ECE4;--teal-50:#80DFD2;--teal-80:#00BFA5;--teal-100:#00897b;--foo: true;--deep-brown-10:#D6D1CA;--deep-brown-20:#BFB7B0;--deep-brown-30:#ACA199;--deep-brown-50:#968B83;--deep-brown-70:#847779;--deep-brown-80:#6F6259;--deep-brown-100:#372e2c;--grayy:#6F6259;--black:#1B1716DD;--solid-black:#1B1716;--black:rgba(27, 23, 22, 0.9);--transparent:rgba(0,0,0,0);--white:#FFF;--almost-transparent:#BFB7B0DD;--orange:#FF834C;--transparent-teal:rgba(0, 137, 123, 0.3);--slider-border-radius:2px}html, body{height: 100%;margin: 0;padding: 0;background-color: var(--black);font-size: 16px;font-family: 'Roboto Condensed', sans-serif;font-weight: 100}@media only screen and (max-width: 1600px){html, body{font-size: 14px!important}}@media only screen and (max-width: 1400px){html, body{font-size: 12px!important}}@media only screen and (max-width: 1200px){html, body{font-size: 12px!important}}@media only screen and (max-width: 992){html, body{font-size: 11px!important}}@media only screen and (max-width: 768){html, body{font-size: 10px!important}}@media only screen and (max-width: 576px){html, body{font-size: 10px!important}}@media only screen and (max-width: 400px){html, body{font-size: 10px!important}}.custom-hidden{display: none}.center{display: block;margin-left: auto;margin-right: auto;width: 50%}.vcenter{display: inline-block;vertical-align: middle!important;float: none}.white{color:var(--deep-brown-20)}.gray{color:var(--deep-brown-70)}.dark-gray{color:var(--deep-brown-10)}.teal{color:var(--teal-100)!important}.teal80{color:var(--teal-80)!important}.teal-study-area-label{color:var(--teal-80)!important}.bg-teal{background-color: var(--teal-100)!important}.bg-gray{background-color: var(--deep-brown-100)!important;color:var(--deep-brown-20)!important}.bg-black,.btn{background-color: var(--black)!important;margin:0px!important;color:var(--white)!important;outline:none!important;vertical-align:middle!important}.shepherd-button{background-color: var(--deep-brown-100)!important;padding: 0.1rem 0.2rem;font-size:1.25rem}.shepherd-content,.shepherd-title,.shepherd-header,.shepherd-text,.shepherd-footer{background-color: var(--deep-brown-100)!important;color:var(--deep-brown-10)!important;overflow: auto}.shepherd-title{font-size:1.25rem}.shepherd-arrow:before{background-color: var(--teal-100)!important;outline-style: solid}.eraser{color: var(--deep-brown-100)!important;cursor:pointer}.eraser:active{transform: translate(3px) translateY(0px);color:var(--teal-100)!important}.eraser-all{height: 0.8rem;cursor:pointer;color:#000;background-color: var(--deep-brown-10);font-size:0.8rem!important;margin-top:0.0rem;margin-bottom: 0.0rem;margin-left:0.25rem;padding-left:0.25rem;padding-right:0.25rem;border-radius: 0.2rem;padding-bottom: 0rem}.fa-eraser{color:var(--deep-brown-100)!important}.eraser-all:active,.fa-eraser:active{transform: translate(4px) translateY(0px);color:var(--teal-100)!important}.eraser-all:hover{font-weight: 300}.bg-solid-black{background-color: var(--solid-black)!important;color:var(--white)!important}.time-lapse-active{background-color: var(--teal-100)!important;color:var(--deep-brown-70)!important}.time-lapse-slider-handle-label{padding-top:1.1em;margin-left:-2.2em;font-size:0.7em;width:5em;color:var(--teal-100)!important;text-align: center}.info-page{color:var(--deep-brown-70)!important;padding-top:4em}.simple-bg-black{background-color: var(--black)!important;color:var(--white)!important}.bg-transparent{background-color: var(--almost-transparent)!important;color:#000!important}.list-group-item,.list-group,.list-group-title{background-color: var(--deep-brown-10)!important;padding-left:0px;padding-right:0px}hr{border: 0;border-top: 1px solid var(--deep-brown-100);}.text-black{color:var(--black)!important}table{border: none!important}.dropdown-divider{margin-top:0.2em;margin-bottom:0em;padding-top:0.2em;padding-bottom:0.2em}.main-container{position: absolute}.map{width:100%;height:100%;position:absolute;z-index:1}.search-box,.form-control{height:1.5em}kbd{border: 1px solid #999}ul, li{list-style-type:none}th{font-weight:600!important}.select-layer-name{margin:0;color:var(--teal-100)}button{-webkit-appearance: button}.sidebar-toggler{position:absolute;top:0%;left:0%;z-index:5;margin-top:-0.2rem;height:3rem}.sidebar-toggler:hover{font-size:1.9em!important}.sidebar-toggler:active{transform: translate(4px) translateY(4px)}.teal-hover:hover{color:var(--teal-100)!important}.sidebar{overflow-y: auto;max-height:calc(100% - 1.7em);;background-color: var(--black)!important;z-index:3}.vl{border-left: 1px solid var(--deep-brown-20);height: 1.25rem;vertical-align: middle;display: inline-block;margin-left: 0.1rem;margin-right:0.25rem;margin-top:0.5rem}.vl2{border-left: 1px solid var(--deep-brown-100);height:2rem;display: inline;vertical-align: middle;display: inline-block;margin-left: 0rem;margin-right:0rem}.title-banner{font-weight:100;font-family: 'Roboto';margin-left:2.5rem;margin-right:0.5rem;margin-bottom:0.0rem;margin-top:0.25rem;font-size:1.5rem;display:flex}.search-bar{padding-left:2.75rem;padding-right:1rem;padding-bottom:0.5rem;padding-top:0.25rem;font-size:1.5rem;display: flex}.dashboard-results-container{position:absolute;bottom:0%;left:0%;width:100%;height:0px;z-index: 2}#dashboard-results-expander{height:0.75rem;background-color: var(--teal-100);margin:0;padding:0;cursor:grab}.dashboard-results{height:100%;width: 100%;overflow-x:scroll;overflow-y:hidden;white-space:nowrap;color:var(--white);background-color: var(--black)!important;margin:0;padding:0}.dashboard-highlights{position:absolute;top:0rem;right:0%;max-width:25rem;max-height:100%;overflow-y:auto;overflow-x:auto;z-index: 2}.dashboard-download-div{margin:0.5rem}.dashboard-download-button{background-color: var(--deep-brown-100)!important;font-size: 0.75rem;color:var(--deep-brown-10)!important;font-family: 'Roboto';font-size:1rem;border: 1px solid var(--deep-brown-100)}.dashboard-download-icon{color:var(--deep-brown-10)!important}.nav-tabs > li > a{color:var(--deep-brown-20);background-color: var(--deep-brown-100);}.nav-tabs .nav-link{border: 1px solid var(--deep-brown-20);border-top-left-radius: 0.25rem;border-top-right-radius: 0.25rem;height: 2rem;font-size: 0.85rem}.nav-tabs .nav-link:active{background-color: var(--teal-100)!important;transform: scale3d(1.05, 1, 1);color: var(--deep-brown-100)}.nav-tabs > li > a:hover{color:var(--teal-100)}.nav-tabs .nav-item.show .nav-link, .nav-tabs .nav-link.active{color: var(--deep-brown-100);background-color: var(--deep-brown-20);font-weight:bold}.highlights-table-tabs{max-width: 100%}.highlights-row{font-size: 0.65rem}.highlights-entry{padding:0.1rem;word-wrap: break-word}.highlights-insig{color:var(--deep-brown-80)}.highlights-sig{font-weight: 900;font-size:0.75rem;color:var(--deep-brown-100)}.highlights-title{color:var(--deep-brown-20);font-family: 'Roboto';font-size:1.75rem;text-align: center;margin-top:0.25rem;margin-bottom:0.25rem;margin-left:3rem!important;font-weight:200}.highlights-table-title{color:var(--deep-brown-20);font-family: 'Roboto';font-size:0.75rem;text-align: center;font-weight:200}.highlights-table-section-title{color:var(--deep-brown-20);background-color: var(--deep-brown-100)!important;font-family: 'Roboto';font-size:0.75rem;text-align: left;font-weight:300}.highlights-table{overflow-y:auto;padding-left: 0px!important}.dataTables_filter{text-align: left!important;margin-left: 0.5rem;margin-top:0.5rem;margin-bottom: 0.25rem;font-size: 0.75rem;color:var(--deep-brown-100);font-family: 'Roboto'}.highlights-disclaimer{margin-top:0.75rem;margin-left: 0.75rem;margin-right:0.75rem;margin-bottom:0.75rem;font-size: 0.75rem;max-width: 20rem;color: var(--deep-brown-20)}.btn-group>.btn{margin-left: 0.5rem!important;padding-bottom: 0px;border-radius: 3px;color: var(--deep-brown-20)!important;background-color: var(--deep-brown-100)!important;font-size: 0.75rem;margin-top: 0.5rem!important}.pac-container{background-color:var(--deep-brown-20)}.hr{height: 1px;border: none;background-color:var(--deep-brown-20)}#dashboard-progress-container{padding-left:1.75rem;padding-right:1rem}.progressbar{background: var(--deep-brown-80);width: 100%;font-size: 1rem;height:0.8rem;margin-top: 0rem;margin-bottom: 0.25rem}.progress-spinner{margin-left:0.25rem;margin-right:0.25rem;margin-top:0rem;margin-bottom:0rem}.progressbar span{display: block;text-align: center;color: #fff;transition: 300ms width linear;background: #00897B;height:0.8rem;font-size: 0.6rem;padding-bottom:0.5rem}.bottombar{position:absolute;bottom:0.0%;left:0%;width:100%;color:var(--white);background-color: var(--black)!important;font-size:1em;z-index:999}.image-icon-bar{max-height:1.3em;float:right;margin:0.1em;border-radius: 0px;background:rgba(255,255,255,0.2)}.home-image-icon-bar{max-height:2em;float:right;margin:0.3em;border-radius: 0px}.support-icons{max-width:4em;max-height:3em}.support-text{color: var(--deep-brown-100)!important}.support-text:hover{font-weight: bold}.text-capitalize{text-transform: uppercase!important}.table-bordered td{border-right: 1px solid #000!important;border-left: 1px solid #000!important}.chart-table{max-height:30rem;max-width:90rem;overflow-y:auto;overflow-x:auto;font-size: 0.8rem}.chart-table-graph-container{max-height:50rem;max-width:90rem;overflow-x:auto;overflow-y:auto}.chart-table-first-row{position: sticky!important;top: 0!important;z-index: 1}.chart-table-first-column{position: sticky!important;left: 0;z-index: 0}.chartjs-chart,.plotly-chart{display: inline-block;height:100%;padding-top:0.5rem;padding-bottom:0.5rem;padding-left:0.5rem;padding-right:0.5rem}.plotly-chart{padding-top:0.75rem;margin-left:0.5rem}.plotly-chart-download{display: none}.legendDiv{position:absolute;bottom:1.7em;right:0%;overflow-y:auto;max-height:60%;color:var(--white);background-color: var(--black)!important;z-index:2}.legend div span{display: inline-block;height: 0.9em;margin-right: 0.3em;width: 0.9em;font-size:0.9em}.legend-title{text-align: left;margin-bottom: 0.1rem;font-weight: bold;font-size: 0.9rem}.my-legend .legend-scale ul{margin: 0;margin-bottom: 0.3em;padding: 0;float: left;list-style: none}.my-legend .legend-scale ul li{font-size: 80%;list-style: none;margin-left: 0;line-height: 1em;margin-bottom: 0.3em}.my-legend ul.legend-labels li span{display: block;float: left;height: 1em;width: 2em;margin-right: 0.3em;margin-left: 0;border: 1px solid #999}.my-legend .legend-source{font-size: 70%;color: #999;clear: both}.my-legend a{color: #777}.leftLabel{float:left;font-size:0.85rem}.rightLabel{float:right;font-size:0.85rem}.colorRamp{width:100%;height:1.0rem}.legend-colorRamp{font-size: 0.9rem;width:100%}.layer-spinner{color: var(--black)!important;font-size:0.9em!important}.layer-container{margin-bottom:1px}.layer-list{padding-bottom: 1px;padding-top :1px;padding-left:0px;margin-bottom:0px}.time-lapse-layer-range-container{float:right;width:30%;margin-top:-0.95em}.time-lapse-label-container{padding-bottom:2em}.simple-time-lapse-layer-range{margin-top:1.8em;cursor:pointer;float:right;min-width:4rem}.simple-time-lapse-layer-range-first{float:right;min-width:4rem;margin-top:1.5em;cursor:pointer}.simple-layer-opacity-range{float:right;min-width:4rem;vertical-align:bottom;margin-top:0.7rem;cursor:pointer}.layer-span, .layer-spinner,.layer-container,.toggle_radio,.collapse-title,.nav-item,ul{cursor:pointer;-webkit-touch-callout: none;-webkit-user-select: none;-khtml-user-select: none;-moz-user-select: none;-ms-user-select: none;user-select: none}.toggle_radio{position: relative;background: rgba(255,255,255,.5);margin: 4px auto;overflow: hidden;padding: 0 !important;-webkit-border-radius: var(--slider-border-radius);-moz-border-radius: var(--slider-border-radius);border-radius: var(--slider-border-radius);position: relative;float:left;height: 26px;width: 214px}.toggle_radio > *{float: left}.toggle_radio input[type=radio]{display: none}.toggle_radio label{background:#FFF;color: #000;z-index: 0;display: block;width: 100px;height: 20px;margin: 3px 3px;-webkit-border-radius: var(--slider-border-radius);-moz-border-radius: var(--slider-border-radius);border-radius: var(--slider-border-radius);cursor: pointer;z-index: 1;text-align: center}.toggle_option_slider{width: 100px;height: 20px;position: absolute;top: 3px;-webkit-border-radius: var(--slider-border-radius);-moz-border-radius: var(--slider-border-radius);border-radius: var(--slider-border-radius);-webkit-transition: all .4s ease;-moz-transition: all .4s ease;-o-transition: all .4s ease;-ms-transition: all .4s ease;transition: all .4s ease}.first_toggle:checked ~ .toggle_option_slider{background: var(--transparent-teal);left: 3px;font-weight: 900!important}.second_toggle:checked ~ .toggle_option_slider{background: var(--transparent-teal);left: 109px;font-weight: 900!important}.third_toggle:checked ~ .toggle_option_slider{background: var(--transparent-teal);left: 215px}.param-title{font-weight: bold;padding-top:1rem;margin-bottom:0rem}::-webkit-scrollbar{width: 0.7rem;height:0.7rem}::-webkit-scrollbar-track{-webkit-box-shadow: inset 0 0 6px rgba(0,0,0,0.3)}::-webkit-scrollbar-thumb{background: var(--deep-brown-70);-webkit-box-shadow: inset 0 0 6px rgba(0,0,0,0.5)}.flexcroll::-webkit-scrollbar{width: 0.7rem}.flexcroll::-webkit-scrollbar-track{-webkit-box-shadow: inset 0 0 6px rgba(0,0,0,0.3)}.flexcroll::-webkit-scrollbar-thumb{background: var(--deep-brown-70);-webkit-box-shadow: inset 0 0 6px rgba(0,0,0,0.5)}.flexcroll{scrollbar-color: var(--deep-brown-70) rgba(0,0,0,0.3);scrollbar-width: thin;scrollbar-height: thin;-webkit-scrollbar-color: var(--deep-brown-70) rgba(0,0,0,0.3);-webkit-scrollbar-width: thin;-webkit-scrollbar-height: thin}.fa{font-size:1.1em;color:#FFF;cursor:pointer}.panel-heading{border-top: 0.05rem solid var(--deep-brown-10);background-color: var(--transparent)!important;color:var(--white)!important}.bg-white, .panel-body{background-color: var(--deep-brown-10)!important;margin:0px!important;color:#000!important;outline:none!important}.bg-download-select{background-color: var(--deep-brown-10)!important;margin:0px!important;color:var(--teal-100)!important;outline:none!important}.bg-download-select::selection{color: red;background: yellow}.panel-title{font-size: 1.25rem}.h3{font-size:1rem}.panel-title > a:after{float: right !important;font-family: FontAwesome;content:"\f068";padding-right: 5px}.panel-title-svg-lg{width:3rem;height:3rem;margin-right:-0.5rem;margin-left:-1.0rem;margin-top:-1.25rem;margin-bottom:-1rem}.panel-title-svg-sm{width:2rem;height:2rem;margin-right:0rem;margin-left:-0.5rem;margin-top:-0.75rem;margin-bottom:-0.5rem}.panel-title.collapsed > a:after{float: right !important;content:"\f067"}.sub-panel-title{padding-top:0.8em}.sub-panel-title > a:after{float: left !important;font-family: FontAwesome;content:"\f077" !important;padding-right: 5px}.sub-panel-title.collapsed > a:after{float: left !important;content:"\f078" !important}.sub-sub-panel-title.collapsed> a, .sub-panel-title.collapsed> a{font-weight: 100!important;color:var(--black)!important}.sub-sub-panel-title > a , .sub-panel-title > a{font-weight: 900!important}.sub-sub-panel-title > a:after{float: left !important;font-family: FontAwesome;content:"\f205" !important;padding-right: 5px;color:var(--teal-100)}.sub-sub-panel-title.collapsed > a:after{float: left !important;content:"\f204" !important;color:var(--black)}.sub-panel-title, .sub-sub-panel-title{background-color: var(--deep-brown-10)!important;color:var(--black);font-weight: bold!important;font-size:1.1em;border-top: 0.1em solid var(--deep-brown-30)}.collapse-title{color:var(--white)}.sub-sub-panel-title:hover,.sub-panel-title:hover,.collapse-title:hover,.panel-title:hover,.dropdown-item:hover,.nav-link:hover, .hover-teal:hover, a:hover{text-decoration: none;font-weight: 1000!important;;cursor:pointer}.panel-title:hover{color:var(--teal-100)!important}.card{border-radius: 0px!important;background-color: var(--white)!important}.gm-style-iw{border-radius: 1px!important}.dropdown{cursor: pointer}.btn{padding:0.3rem}.btn:active,.drawing-mode-selector:active{background-color: var(--teal-100)!important;transform: scale3d(1.05, 1, 1)}.btn:hover,.drawing-mode-selector:hover{font-weight: 300}.color-button{border-radius:0.2em;height:2.1em;width:2.1em;border:0.1em solid black;vertical-align: middle!important}.dropdown-menu:hover{display: block;cursor:pointer}.dropdown-item{padding:0px!important}input[type = 'checkbox'],label,input[type = 'radio']{cursor:pointer}input[type=checkbox],input[type=radio]{display:none}input[type=checkbox] + label:before ,input[type=radio] + label:before{font-family: FontAwesome;display: inline-block}input[type=checkbox] + label:before,input[type=radio].form-check-input + label:before{content: "\f10c"}input[type=checkbox] + label:before,input[type=radio].form-check-input + label:before{letter-spacing: 0.2em}input[type=checkbox]:checked + label:before,input[type=radio].form-check-input:checked + label:before{content: "\f111";color:#00897B}input[type=checkbox]:checked + label:before,input[type=radio].form-check-input:checked + label:before{letter-spacing: 0.2em}textarea{resize: none;overflow: hidden;min-height: 50px;max-height: 100px}.close{color:#FFF}.modal-md{max-width:550px}.modal-content{border-radius: 0!important}.modal-content{max-width:90em!important}.logo{height:3rem;display: inline;vertical-align: top;margin-bottom: 0.5rem}.splash-title{overflow: hidden;padding-left:1rem;padding-right:1rem;display: inline}.modal-full-screen-styling{background-color:rgba(230,230,230,0.8)}.modal-content-full-screen-styling{background-color:rgba(230,230,230,0.2);border-style: none}.intro-modal-links, .links{text-decoration: underline!important;font-size: 1.0rem;font-weight: bold;margin-right:0.3rem;color:var(--black)!important}.intro-modal-links:active{transform: translate(4px) translateY(4px)}.intro-modal-links:hover{font-weight: 1000}.intro-list li{display: block}.modal-content-not-full-screen-styling{background-color:rgba(230,230,230,0.8);border-style: none}.ui-slider-horizontal .ui-slider-handle{top: -.45rem;border-radius:0rem;margin-left: -0.3rem;width: 0.6rem;height: 1rem;border: 0.1rem solid var(--deep-brown-100)}.ui-widget-content .ui-state-default{background: var(--deep-brown-100)!important}.ui-slider-horizontal{height: .2rem;background:var(--deep-brown-70);border: 0.1rem solid var(--deep-brown-100)}.ui-slider-horizontal .ui-slider-handle .ui-state-focus{border-radius: 0rem!important}ul, #myUL{list-style-type: none}#myUL{margin: 0;padding: 0}.caret{cursor: pointer;user-select: none}.caret::before{font-family: FontAwesome;content:"\f07b";color: var(--teal-100);display: inline-block;margin-right: 0.2em}.caret-down::before{font-family: FontAwesome;content:"\f07c";color: var(--teal-100)}.nested{display: none}.active{display: block;padding-left:1.2em}
+@import "https://fonts.googleapis.com/css?family=Roboto+Condensed&display=swap";:root{--teal-30:#b2ece4;--teal-50:#80dfd2;--teal-80:#00bfa5;--teal-100:#00897b;--foo:true;--deep-brown-10:#d6d1ca;--deep-brown-20:#bfb7b0;--deep-brown-30:#aca199;--deep-brown-50:#968b83;--deep-brown-70:#847779;--deep-brown-80:#6f6259;--deep-brown-100:#372e2c;--grayy:#6f6259;--black:#1B1716DD;--solid-black:#1b1716;--black:rgba(27,23,22,0.9);--transparent:rgba(0,0,0,0);--white:#FFF;--almost-transparent:#BFB7B0DD;--orange:#ff834c;--transparent-teal:rgba(0,137,123,0.3);--slider-border-radius:2px}html,body{height:100%;margin:0;padding:0;background-color:var(--black);font-size:16px;font-family:'Roboto Condensed',sans-serif;font-weight:100}@media only screen and (max-width:1600px){html,body{font-size:14px !important}}@media only screen and (max-width:1400px){html,body{font-size:12px !important}}@media only screen and (max-width:1200px){html,body{font-size:12px !important}}@media only screen and (max-width:992){html,body{font-size:11px !important}}@media only screen and (max-width:768){html,body{font-size:10px !important}}@media only screen and (max-width:576px){html,body{font-size:10px !important}}@media only screen and (max-width:400px){html,body{font-size:10px !important}}.custom-hidden{display:none}.center{display:block;margin-left:auto;margin-right:auto;width:50%}.vcenter{display:inline-block;vertical-align:middle !important;float:none}.white{color:var(--deep-brown-20)}.gray{color:var(--deep-brown-70)}.dark-gray{color:var(--deep-brown-10)}.teal{color:var(--teal-100) !important}.teal80{color:var(--teal-80) !important}.teal-study-area-label{color:var(--teal-80) !important}.bg-teal{background-color:var(--teal-100) !important}.bg-gray{background-color:var(--deep-brown-100) !important;color:var(--deep-brown-20) !important}.bg-black,.btn{background-color:var(--black) !important;margin:0 !important;color:var(--white) !important;outline:none !important;vertical-align:middle !important}.shepherd-button{background-color:var(--deep-brown-100) !important;padding:.1rem .2rem;font-size:1.25rem}.shepherd-content,.shepherd-title,.shepherd-header,.shepherd-text,.shepherd-footer{background-color:var(--deep-brown-100) !important;color:var(--deep-brown-10) !important;overflow:auto}.shepherd-title{font-size:1.25rem}.shepherd-arrow:before{background-color:var(--teal-100) !important;outline-style:solid}.eraser{color:var(--deep-brown-100) !important;cursor:pointer}.eraser:active{transform:translate(3px) translateY(0);color:var(--teal-100) !important}.eraser-all{height:.8rem;cursor:pointer;color:#000;background-color:var(--deep-brown-10);font-size:.8rem !important;margin-top:0;margin-bottom:0;margin-left:.25rem;padding-left:.25rem;padding-right:.25rem;border-radius:.2rem;padding-bottom:0}.fa-eraser{color:var(--deep-brown-100) !important}.eraser-all:active,.fa-eraser:active{transform:translate(4px) translateY(0);color:var(--teal-100) !important}.eraser-all:hover{font-weight:300}.bg-solid-black{background-color:var(--solid-black) !important;color:var(--white) !important}.time-lapse-active{background-color:var(--teal-100) !important;color:var(--deep-brown-70) !important}.time-lapse-slider-handle-label{padding-top:1.1em;margin-left:-2.2em;font-size:.7em;width:5em;color:var(--teal-100) !important;text-align:center}.info-page{color:var(--deep-brown-20) !important;padding-top:4em}.simple-bg-black{background-color:var(--black) !important;color:var(--white) !important}.bg-transparent{background-color:var(--almost-transparent) !important;color:#000 !important}.list-group-item,.list-group,.list-group-title{background-color:var(--deep-brown-10) !important;padding-left:0;padding-right:0}hr{border:0;border-top:1px solid var(--deep-brown-100)}.text-black{color:var(--black) !important}table{border:none !important}.dropdown-divider{margin-top:.2em;margin-bottom:0;padding-top:.2em;padding-bottom:.2em}.figure{display:right;float:right}.figcaption{width:50%;text-align:justify;font-size:20em}.container-beforeIntro{padding-right:-50px;padding-left:100px;margin-right:-15px;margin-left:-15px}.container-intro{padding-right:25px;padding-left:45px;margin-right:0;margin-left:-15px}.main-container{position:absolute}.map{width:100%;height:100%;position:absolute;z-index:1}.search-box,.form-control{height:1.5em}kbd{border:1px solid #999}ul,li{list-style-type:none}th{font-weight:600 !important}.select-layer-name{margin:0;color:var(--teal-100)}button{-webkit-appearance:button}.sidebar-toggler{position:absolute;top:0;left:0;z-index:5;margin-top:-0.2rem;height:3rem}.sidebar-toggler:hover{font-size:1.9em !important}.sidebar-toggler:active{transform:translate(4px) translateY(4px)}.teal-hover:hover{color:var(--teal-100) !important}.sidebar{overflow-y:auto;max-height:calc(100% - 1.7em);background-color:var(--black) !important;z-index:3}.vl{border-left:1px solid var(--deep-brown-20);height:1.25rem;vertical-align:middle;display:inline-block;margin-left:.1rem;margin-right:.25rem;margin-top:.5rem}.vl2{border-left:1px solid var(--deep-brown-100);height:2rem;display:inline;vertical-align:middle;display:inline-block;margin-left:0;margin-right:0}.title-banner{font-weight:100;font-family:'Roboto';margin-left:2.5rem;margin-right:.5rem;margin-bottom:0;margin-top:.25rem;font-size:1.5rem;display:flex}.search-bar{padding-left:2.75rem;padding-right:1rem;padding-bottom:.5rem;padding-top:.25rem;font-size:1.5rem;display:flex}.dashboard-results-container{position:absolute;bottom:0;left:0;width:100%;height:0;z-index:2}#dashboard-results-expander{height:.75rem;background-color:var(--teal-100);margin:0;padding:0;cursor:grab}.dashboard-results{height:100%;width:100%;overflow-x:scroll;overflow-y:hidden;white-space:nowrap;color:var(--white);background-color:var(--black) !important;margin:0;padding:0}.dashboard-highlights{position:absolute;top:0;right:0;max-width:25rem;max-height:100%;overflow-y:auto;overflow-x:auto;z-index:2}.dashboard-download-div{margin:.5rem}.dashboard-download-button{background-color:var(--deep-brown-100) !important;font-size:.75rem;color:var(--deep-brown-10) !important;font-family:'Roboto';font-size:1rem;border:1px solid var(--deep-brown-100)}.dashboard-download-icon{color:var(--deep-brown-10) !important}.nav-tabs>li>a{color:var(--deep-brown-20);background-color:var(--deep-brown-100)}.nav-tabs .nav-link{border:1px solid var(--deep-brown-20);border-top-left-radius:.25rem;border-top-right-radius:.25rem;height:2rem;font-size:.85rem}.nav-tabs .nav-link:active{background-color:var(--teal-100) !important;transform:scale3d(1.05,1,1);color:var(--deep-brown-100)}.nav-tabs>li>a:hover{color:var(--teal-100)}.nav-tabs .nav-item.show .nav-link,.nav-tabs .nav-link.active{color:var(--deep-brown-100);background-color:var(--deep-brown-20);font-weight:bold}.highlights-table-tabs{max-width:100%}.highlights-row{font-size:.65rem}.highlights-entry{padding:.1rem;word-wrap:break-word}.highlights-insig{color:var(--deep-brown-80)}.highlights-sig{font-weight:900;font-size:.75rem;color:var(--deep-brown-100)}.highlights-title{color:var(--deep-brown-20);font-family:'Roboto';font-size:1.75rem;text-align:center;margin-top:.25rem;margin-bottom:.25rem;margin-left:3rem !important;font-weight:200}.highlights-table-title{color:var(--deep-brown-20);font-family:'Roboto';font-size:.75rem;text-align:center;font-weight:200}.highlights-table-section-title{color:var(--deep-brown-20);background-color:var(--deep-brown-100) !important;font-family:'Roboto';font-size:.75rem;text-align:left;font-weight:300}.highlights-table{overflow-y:auto;padding-left:0 !important}.dataTables_filter{text-align:left !important;margin-left:.5rem;margin-top:.5rem;margin-bottom:.25rem;font-size:.75rem;color:var(--deep-brown-100);font-family:'Roboto'}.highlights-disclaimer{margin-top:.75rem;margin-left:.75rem;margin-right:.75rem;margin-bottom:.75rem;font-size:.75rem;max-width:20rem;color:var(--deep-brown-20)}.btn-group>.btn{margin-left:.5rem !important;padding-bottom:0;border-radius:3px;color:var(--deep-brown-20) !important;background-color:var(--deep-brown-100) !important;font-size:.75rem;margin-top:.5rem !important}.pac-container{background-color:var(--deep-brown-20)}.hr{height:1px;border:0;background-color:var(--deep-brown-20)}#dashboard-progress-container{padding-left:1.75rem;padding-right:1rem}.progressbar{background:var(--deep-brown-80);width:100%;font-size:1rem;height:.8rem;margin-top:0;margin-bottom:.25rem}.progress-spinner{margin-left:.25rem;margin-right:.25rem;margin-top:0;margin-bottom:0}.progressbar span{display:block;text-align:center;color:#fff;transition:300ms width linear;background:#00897b;height:.8rem;font-size:.6rem;padding-bottom:.5rem}.bottombar{position:absolute;bottom:0;left:5rem;color:var(--white);background-color:var(--black) !important;font-size:.8rem;z-index:999}.image-icon-bar{max-height:1.3em;float:right;margin:.1em;border-radius:0;background:rgba(255,255,255,0.2)}.home-image-icon-bar{max-height:2em;float:right;margin:.3em;border-radius:0}.support-icons{max-width:4em;max-height:3em}.support-text{color:var(--deep-brown-100) !important}.support-text:hover{font-weight:bold}.text-capitalize{text-transform:uppercase !important}.table-bordered td{border-right:1px solid #000 !important;border-left:1px solid #000 !important}.chart-table{max-height:30rem;max-width:90rem;overflow-y:auto;overflow-x:auto;font-size:.8rem}.chart-table-graph-container{max-height:50rem;max-width:90rem;overflow-x:auto;overflow-y:auto}.chart-table-first-row{position:sticky !important;top:0 !important;z-index:1}.chart-table-first-column{position:sticky !important;left:0;z-index:0}.chartjs-chart,.plotly-chart{display:inline-block;height:100%;padding-top:.5rem;padding-bottom:.5rem;padding-left:.5rem;padding-right:.5rem}.lcms-change-table-columns td{font-size:12px;table-layout:fixed;padding:15px 75px 0 0;max-width:1000px}td{word-wrap:break-word}.plotly-chart{padding-top:.75rem;margin-left:.5rem}.plotly-chart-download{display:none}.legendDiv{position:absolute;bottom:1.7em;right:0;overflow-y:auto;max-height:60%;color:var(--white);background-color:var(--black) !important;z-index:2}.legend div span{display:inline-block;height:.9em;margin-right:.3em;width:.9em;font-size:.9em}.legend-title{text-align:left;margin-bottom:.1rem;font-weight:bold;font-size:.9rem}.my-legend .legend-scale ul{margin:0;margin-bottom:.3em;padding:0;float:left;list-style:none}.my-legend .legend-scale ul li{font-size:80%;list-style:none;margin-left:0;line-height:1em;margin-bottom:.3em}.my-legend ul.legend-labels li span{display:block;float:left;height:1em;width:2em;margin-right:.3em;margin-left:0;border:1px solid #999}.my-legend .legend-source{font-size:70%;color:#999;clear:both}.my-legend a{color:#777}.leftLabel{float:left;font-size:.85rem}.rightLabel{float:right;font-size:.85rem}.colorRamp{width:100%;height:1rem}.legend-colorRamp{font-size:.9rem;width:100%}.layer-spinner{color:var(--black) !important;font-size:.9em !important}.layer-container{margin-bottom:1px}.layer-list{padding-bottom:1px;padding-top:1px;padding-left:0;margin-bottom:0}.time-lapse-layer-range-container{float:right;width:30%;margin-top:-0.95em}.time-lapse-label-container{padding-bottom:2em}.simple-time-lapse-layer-range{margin-top:1.8em;cursor:pointer;float:right;min-width:4rem}.simple-time-lapse-layer-range-first{float:right;min-width:4rem;margin-top:1.5em;cursor:pointer}.simple-layer-opacity-range{float:right;min-width:4rem;vertical-align:bottom;margin-top:.7rem;cursor:pointer}.layer-span,.layer-spinner,.layer-container,.toggle_radio,.collapse-title,.nav-item,ul{cursor:pointer;-webkit-touch-callout:none;-webkit-user-select:none;-khtml-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none}.toggle_radio{position:relative;background:rgba(255,255,255,.5);margin:4px auto;overflow:hidden;padding:0 !important;-webkit-border-radius:var(--slider-border-radius);-moz-border-radius:var(--slider-border-radius);border-radius:var(--slider-border-radius);position:relative;float:left;height:26px;width:214px}.toggle_radio>*{float:left}.toggle_radio input[type=radio]{display:none}.toggle_radio label{background:#FFF;color:#000;z-index:0;display:block;width:100px;height:20px;margin:3px 3px;-webkit-border-radius:var(--slider-border-radius);-moz-border-radius:var(--slider-border-radius);border-radius:var(--slider-border-radius);cursor:pointer;z-index:1;text-align:center}.toggle_option_slider{width:100px;height:20px;position:absolute;top:3px;-webkit-border-radius:var(--slider-border-radius);-moz-border-radius:var(--slider-border-radius);border-radius:var(--slider-border-radius);-webkit-transition:all .4s ease;-moz-transition:all .4s ease;-o-transition:all .4s ease;-ms-transition:all .4s ease;transition:all .4s ease}.first_toggle:checked ~ .toggle_option_slider{background:var(--transparent-teal);left:3px;font-weight:900 !important}.second_toggle:checked ~ .toggle_option_slider{background:var(--transparent-teal);left:109px;font-weight:900 !important}.third_toggle:checked ~ .toggle_option_slider{background:var(--transparent-teal);left:215px}.param-title{font-weight:bold;padding-top:1rem;margin-bottom:0}::-webkit-scrollbar{width:.7rem;height:.7rem}::-webkit-scrollbar-track{-webkit-box-shadow:inset 0 0 6px rgba(0,0,0,0.3)}::-webkit-scrollbar-thumb{background:var(--deep-brown-70);-webkit-box-shadow:inset 0 0 6px rgba(0,0,0,0.5)}.flexcroll::-webkit-scrollbar{width:.7rem}.flexcroll::-webkit-scrollbar-track{-webkit-box-shadow:inset 0 0 6px rgba(0,0,0,0.3)}.flexcroll::-webkit-scrollbar-thumb{background:var(--deep-brown-70);-webkit-box-shadow:inset 0 0 6px rgba(0,0,0,0.5)}.flexcroll{scrollbar-color:var(--deep-brown-70) rgba(0,0,0,0.3);scrollbar-width:thin;scrollbar-height:thin;-webkit-scrollbar-color:var(--deep-brown-70) rgba(0,0,0,0.3);-webkit-scrollbar-width:thin;-webkit-scrollbar-height:thin}.fa{font-size:1.1em;color:#FFF;cursor:pointer}.panel-heading{border-top:.05rem solid var(--deep-brown-10);background-color:var(--transparent) !important;color:var(--white) !important}.bg-white,.panel-body{background-color:var(--deep-brown-10) !important;margin:0 !important;color:#000 !important;outline:none !important}.bg-download-select{background-color:var(--deep-brown-10) !important;margin:0 !important;color:var(--teal-100) !important;outline:none !important}.bg-download-select::selection{color:red;background:yellow}.panel-title{font-size:1.25rem}.h3{font-size:1rem}.panel-title>a:after{float:right !important;font-family:FontAwesome;content:"\f068";padding-right:5px}.panel-title-svg-lg{width:3rem;height:3rem;margin-right:-0.5rem;margin-left:-1rem;margin-top:-1.25rem;margin-bottom:-1rem}.panel-title-svg-sm{width:2rem;height:2rem;margin-right:0;margin-left:-0.5rem;margin-top:-0.75rem;margin-bottom:-0.5rem}.panel-title.collapsed>a:after{float:right !important;content:"\f067"}.sub-panel-title{padding-top:.8em}.sub-panel-title>a:after{float:left !important;font-family:FontAwesome;content:"\f077" !important;padding-right:5px}.sub-panel-title.collapsed>a:after{float:left !important;content:"\f078" !important}.sub-sub-panel-title.collapsed>a,.sub-panel-title.collapsed>a{font-weight:100 !important;color:var(--black) !important}.sub-sub-panel-title>a,.sub-panel-title>a{font-weight:900 !important}.sub-sub-panel-title>a:after{float:left !important;font-family:FontAwesome;content:"\f205" !important;padding-right:5px;color:var(--teal-100)}.sub-sub-panel-title.collapsed>a:after{float:left !important;content:"\f204" !important;color:var(--black)}.sub-panel-title,.sub-sub-panel-title{background-color:var(--deep-brown-10) !important;color:var(--black);font-weight:bold !important;font-size:1.1em;border-top:.1em solid var(--deep-brown-30)}.collapse-title{color:var(--white)}.sub-sub-panel-title:hover,.sub-panel-title:hover,.collapse-title:hover,.panel-title:hover,.dropdown-item:hover,.nav-link:hover,.hover-teal:hover,a:hover{text-decoration:none;font-weight:1000 !important;cursor:pointer}.panel-title:hover{color:var(--teal-100) !important}.card{border-radius:0 !important;background-color:var(--white) !important}.gm-style-iw{border-radius:1px !important}.gm-marker-label{background-color:#372e2c;bottom:1rem;right:60%;position:relative;font-size:.8rem;font-family:'Roboto Condensed',sans-serif}.dropdown{cursor:pointer}.btn{padding:.3rem}.btn:active,.drawing-mode-selector:active{background-color:var(--teal-100) !important;transform:scale3d(1.05,1,1)}.btn:hover,.drawing-mode-selector:hover{font-weight:300}.color-button{border-radius:.2em;height:2.1em;width:2.1em;border:.1em solid black;vertical-align:middle !important}.dropdown-menu:hover{display:block;cursor:pointer}.dropdown-item{padding:0 !important}input[type = 'checkbox'],label,input[type = 'radio']{cursor:pointer}input[type=checkbox],input[type=radio]{display:none}input[type=checkbox]+label:before,input[type=radio]+label:before{font-family:FontAwesome;display:inline-block}input[type=checkbox]+label:before,input[type=radio].form-check-input+label:before{content:"\f10c"}input[type=checkbox]+label:before,input[type=radio].form-check-input+label:before{letter-spacing:.2em}input[type=checkbox]:checked+label:before,input[type=radio].form-check-input:checked+label:before{content:"\f111";color:#00897b}input[type=checkbox]:checked+label:before,input[type=radio].form-check-input:checked+label:before{letter-spacing:.2em}textarea{resize:none;overflow:hidden;min-height:50px;max-height:100px}.close{color:#FFF}.modal-md{max-width:550px}.modal-content{border-radius:0 !important}.modal-content{max-width:90em !important}.logo{height:3rem;display:inline;vertical-align:top;margin-bottom:.5rem}.splash-title{overflow:hidden;padding-left:1rem;padding-right:1rem;display:inline}.modal-full-screen-styling{background-color:rgba(230,230,230,0.8)}.modal-content-full-screen-styling{background-color:rgba(230,230,230,0.2);border-style:none}.intro-modal-links,.links{text-decoration:underline !important;font-size:1rem;font-weight:bold;margin-right:.3rem;color:var(--black) !important}.intro-modal-links:active{transform:translate(4px) translateY(4px)}.intro-modal-links:hover{font-weight:1000}.intro-list li{display:block}.modal-content-not-full-screen-styling{background-color:rgba(230,230,230,0.8);border-style:none}.ui-slider-horizontal .ui-slider-handle{top:-.45rem;border-radius:0;margin-left:-0.3rem;width:.6rem;height:1rem;border:.1rem solid var(--deep-brown-100)}.ui-widget-content .ui-state-default{background:var(--deep-brown-100) !important}.ui-slider-horizontal{height:.2rem;background:var(--deep-brown-70);border:.1rem solid var(--deep-brown-100)}.ui-slider-horizontal .ui-slider-handle .ui-state-focus{border-radius:0 !important}ul,#myUL{list-style-type:none}#myUL{margin:0;padding:0}.caret{cursor:pointer;border-top:0;user-select:none;white-space:nowrap;padding-bottom:1.5rem;font-size:1.1rem}.caret::before{font-family:FontAwesome;content:"\f07b";color:var(--teal-100);display:inline-block;margin-right:.3em;padding-left:.25em}.caret-down::before{font-family:FontAwesome;content:"\f07c";color:var(--teal-100)}.nested{display:none}.active{display:block;padding-left:1.2em}#downloadTree{color:#00897b}.carousel-img{width:100%;max-width:600px;max-height:500px}.textFade{animation:fadeInAnimation ease 20s;animation-delay:ease 0;animation-iteration-count:1;animation-fill-mode:forwards}.textFade2{animation:fadeInAnimation ease 25s;animation-delay:ease 0;animation-iteration-count:1;animation-fill-mode:forwards}.textFade3{animation:fadeInAnimation ease 30s;animation-delay:ease 0;animation-iteration-count:1;animation-fill-mode:forwards}.textFade4{animation:fadeInAnimation ease 35s;animation-delay:ease 0;animation-iteration-count:1;animation-fill-mode:forwards}.textFade5{animation:fadeInAnimation ease 40s;animation-delay:ease 0;animation-iteration-count:1;animation-fill-mode:forwards}.textFade6{animation:fadeInAnimation ease 45s;animation-delay:ease 0;animation-iteration-count:1;animation-fill-mode:forwards}@keyframes fadeInAnimation{0%{opacity:0}100%{opacity:1}}
```

### Comparing `geeViz-2023.4.1/geeViz/geeView/images/EE-logo-150.png` & `geeViz-2023.6.1/geeViz/geeView/images/EE-logo-150.png`

 * *Files identical despite different names*

### Comparing `geeViz-2023.4.1/geeViz/geeView/images/GEE.png` & `geeViz-2023.6.1/geeViz/geeView/images/GEE.png`

 * *Files identical despite different names*

### Comparing `geeViz-2023.4.1/geeViz/geeView/images/GEE_logo_transparent.png` & `geeViz-2023.6.1/geeViz/geeView/images/GEE_logo_transparent.png`

 * *Files identical despite different names*

### Comparing `geeViz-2023.4.1/geeViz/geeView/images/RCR-logo.jpg` & `geeViz-2023.6.1/geeViz/geeView/images/RCR-logo.jpg`

 * *Files identical despite different names*

### Comparing `geeViz-2023.4.1/geeViz/geeView/images/Thumbs.db` & `geeViz-2023.6.1/geeViz/geeView/images/Thumbs.db`

 * *Files identical despite different names*

### Comparing `geeViz-2023.4.1/geeViz/geeView/images/cumulative_icon.png` & `geeViz-2023.6.1/geeViz/geeView/images/cumulative_icon.png`

 * *Files identical despite different names*

### Comparing `geeViz-2023.4.1/geeViz/geeView/images/layer_icon.png` & `geeViz-2023.6.1/geeViz/geeView/images/layer_icon.png`

 * *Files identical despite different names*

### Comparing `geeViz-2023.4.1/geeViz/geeView/images/logos_usda-fs.svg` & `geeViz-2023.6.1/geeViz/geeView/images/logos_usda-fs.svg`

 * *Files identical despite different names*

### Comparing `geeViz-2023.4.1/geeViz/geeView/images/logos_usda-fs_bn-dk-01.svg` & `geeViz-2023.6.1/geeViz/geeView/images/logos_usda-fs_bn-dk-01.svg`

 * *Files identical despite different names*

### Comparing `geeViz-2023.4.1/geeViz/geeView/images/menu-hamburger_ffffff.svg` & `geeViz-2023.6.1/geeViz/geeView/images/menu-hamburger_ffffff.svg`

 * *Files identical despite different names*

### Comparing `geeViz-2023.4.1/geeViz/geeView/images/usdalogo.png` & `geeViz-2023.6.1/geeViz/geeView/images/usdalogo.png`

 * *Files identical despite different names*

### Comparing `geeViz-2023.4.1/geeViz/geeView/images/usfslogo.png` & `geeViz-2023.6.1/geeViz/geeView/images/usfslogo.png`

 * *Files identical despite different names*

### Comparing `geeViz-2023.4.1/geeViz/geeView/index.html` & `geeViz-2023.6.1/geeViz/geeView/index.html`

 * *Files identical despite different names*

### Comparing `geeViz-2023.4.1/geeViz/geeView/js/gena-gee-palettes.js` & `geeViz-2023.6.1/geeViz/geeView/js/gena-gee-palettes.js`

 * *Files identical despite different names*

### Comparing `geeViz-2023.4.1/geeViz/geeView/js/lcms-viewer.min.js` & `geeViz-2023.6.1/geeViz/geeView/js/lcms-viewer.min.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -66,15 +66,15 @@
             Object.keys(urlParams[a]).map((e => t["OBJECT---" + a + "---" + e] = urlParams[a][e])), e += new URLSearchParams(t).toString() + "&"
         } else e += a + "=" + urlParams[a] + "&"
     })), e = e.slice(0, e.length - 1)
 }
 pageUrl = document.URL, tinyURL = "", urlParams = {};
 let cachedSettingskey = "settings",
     startYear = 1985,
-    endYear = 2021,
+    endYear = 2022,
     startJulian = 153,
     endJulian = 274,
     layerObj = null,
     crs = "EPSG:5070",
     transform = [30, 0, -2361915, 0, -30, 3177735],
     scale = null,
     queryObj = {},
@@ -87,15 +87,15 @@
 const studyAreaDict = {
     "USFS LCMS 1984-2020": {
         isPilot: !1,
         name: "USFS LCMS 1984-2020",
         center: [37.5334105816903, -105.6787109375, 5],
         crs: "EPSG:5070",
         startYear: 1985,
-        endYear: 2021,
+        endYear: 2022,
         conusSA: "projects/lcms-292214/assets/CONUS-Ancillary-Data/conus",
         conusLossThresh: .23,
         conusFastLossThresh: .29,
         conusSlowLossThresh: .18,
         conusGainThresh: .29,
         akSA: "projects/lcms-292214/assets/R10/CoastalAK/TCC_Boundary",
         akLossThresh: .26,
@@ -202,17 +202,17 @@
             },
             6: {
                 modelName: "Rangeland",
                 legendName: "Rangeland or Pasture",
                 color: "c2b34a"
             }
         },
-        final_collections: ["USFS/GTAC/LCMS/v2020-6", "USFS/GTAC/LCMS/v2021-7"],
-        composite_collections: ["projects/lcms-292214/assets/R10/CoastalAK/Composites/Composite-Collection", "projects/lcms-tcc-shared/assets/Composites/Composite-Collection-yesL7-1984-2020", "projects/lcms-292214/assets/R8/PR_USVI/Composites/Composite-Collection-1984-2020"],
-        lt_collections: ["projects/lcms-292214/assets/R10/CoastalAK/Base-Learners/LANDTRENDR-Collection", "projects/lcms-tcc-shared/assets/LandTrendr/LandTrendr-Collection-yesL7-1984-2020", "projects/lcms-292214/assets/R8/PR_USVI/Base-Learners/LandTrendr-Collection-1984-2020"],
+        final_collections: ["USFS/GTAC/LCMS/v2020-6", "USFS/GTAC/LCMS/v2022-8"],
+        composite_collections: ["projects/lcms-292214/assets/R10/CoastalAK/Composites/Composite-Collection", "projects/lcms-tcc-shared/assets/Composites/Composite-Collection-yesL7-1984-2020", "projects/lcms-292214/assets/R8/PR_USVI/Composites/Composite-Collection-1984-2020", "projects/lcms-tcc-shared/assets/OCONUS/Hawaii/Composites/Composite-Collection"],
+        lt_collections: ["projects/lcms-292214/assets/R10/CoastalAK/Base-Learners/LANDTRENDR-Collection", "projects/lcms-tcc-shared/assets/LandTrendr/LandTrendr-Collection-yesL7-1984-2020", "projects/lcms-292214/assets/R8/PR_USVI/Base-Learners/LandTrendr-Collection-1984-2020", "projects/lcms-tcc-shared/assets/OCONUS/Hawaii/Base-Learners/LandTrendr-Collection"],
         ccdc_collections: ["projects/lcms-292214/assets/R10/CoastalAK/Base-Learners/CCDC-Collection", "projects/lcms-292214/assets/CONUS-LCMS/Base-Learners/CCDC-Collection-1984-2022", "projects/lcms-292214/assets/R8/PR_USVI/Base-Learners/CCDC-Landsat-1984-2020"]
     }
 };
 let defaultStudyArea = "USFS LCMS 1984-2020",
     studyAreaName = studyAreaDict[defaultStudyArea].name,
     longStudyAreaName = defaultStudyArea,
     cachedStudyAreaName = null,
@@ -463,34 +463,34 @@
         allLossGain2Area: ["f39268", "d54309", "00a398", "ffbe2e"],
         test: ["#9A6324", "#6f6f6f", "#e6194B", "#14d4f4", "#880088", "#f58231"],
         testArea: ["#e6194B", "#14d4f4", "#880088", "#f58231"],
         ancillary: ["#cc0066", "#660033", "#9933ff", "#330080", "#ff3300", "#47d147", "#00cc99", "#ff9966", "#b37700"]
     },
     chartColors = chartColorsDict.standard;
 const zoomDict = {
-    20: "1,128.49",
-    19: "2,256.99",
-    18: "4,513.98",
-    17: "9,027.97",
-    16: "18,055.95",
-    15: "36,111.91",
-    14: "72,223.82",
-    13: "144,447.64",
-    12: "288,895.28",
-    11: "577,790.57",
-    10: "1,155,581.15",
-    9: "2,311,162.30",
-    8: "4,622,324.61",
-    7: "9,244,649.22",
-    6: "18,489,298.45",
-    5: "36,978,596.91",
-    4: "73,957,193.82",
-    3: "147,914,387.60",
-    2: "295,828,775.30",
-    1: "591,657,550.50"
+    20: "1,128",
+    19: "2,257",
+    18: "4,514",
+    17: "9,028",
+    16: "18,056",
+    15: "36,112",
+    14: "72,224",
+    13: "144,448",
+    12: "288,892",
+    11: "577,791",
+    10: "1,155,581",
+    9: "2,311,162",
+    8: "4,622,325",
+    7: "9,244,649",
+    6: "18,489,298",
+    5: "36,978,597",
+    4: "73,957,194",
+    3: "147,914,388",
+    2: "295,828,775",
+    1: "591,657,551"
 };
 null != urlParams.geeAuthProxyURL && null != urlParams.geeAuthProxyURL || (urlParams.geeAuthProxyURL = "https://rcr-ee-proxy-2.herokuapp.com");
 let authProxyAPIURL = urlParams.geeAuthProxyURL,
     geeAPIURL = "https://earthengine.googleapis.com";
 null !== urlParams.accessToken && void 0 !== urlParams.accessToken && "null" !== urlParams.accessToken && "None" !== urlParams.accessToken && (authProxyAPIURL = null, geeAPIURL = null, ee.data.setAuthToken("", "Bearer", urlParams.accessToken, 3600, [], void 0, !1));
 var plotsOn = !1;
 Array.prototype.max = function() {
@@ -561,101 +561,116 @@
     },
     quantile = (e, a) => {
         const t = asc(e),
             o = (t.length - 1) * a,
             l = Math.floor(o),
             r = o - l;
         return void 0 !== t[l + 1] ? t[l] + r * (t[l + 1] - t[l]) : t[l]
-    },
-    titles = {
-        "LCMS-pilot": {
-            leftWords: "LCMS",
-            centerWords: "DATA",
-            rightWords: "EXPLORER",
-            title: "LCMS Data Explorer"
-        },
-        LCMS: {
-            leftWords: "LCMS",
-            centerWords: "DATA",
-            rightWords: "EXPLORER",
-            title: "LCMS Data Explorer"
-        },
-        "lcms-base-learner": {
-            leftWords: "LCMS",
-            centerWords: "Base-Learner",
-            rightWords: "EXPLORER",
-            title: "LCMS Base Learner Explorer"
-        },
-        Ancillary: {
-            leftWords: "Ancillary",
-            centerWords: "DATA",
-            rightWords: "Viewer",
-            title: "TimeSync Ancillary Data Viewer"
-        },
-        LT: {
-            leftWords: "LandTrendr",
-            centerWords: "DATA",
-            rightWords: "EXPLORER",
-            title: "LandTrendr Data Explorer"
-        },
-        MTBS: {
-            leftWords: "MTBS",
-            centerWords: "DATA",
-            rightWords: "EXPLORER",
-            title: "MTBS Data Explorer"
-        },
-        TEST: {
-            leftWords: "TEST",
-            centerWords: "DATA",
-            rightWords: "Explorer",
-            title: "TEST Data Viewer"
-        },
-        IDS: {
-            leftWords: "IDS",
-            centerWords: "DATA",
-            rightWords: "EXPLORER",
-            title: "Insect and Disease Detection Survey Data Viewer"
-        },
-        geeViz: {
-            leftWords: "geeViz",
-            centerWords: "DATA",
-            rightWords: "Viewer",
-            title: "geeViz Data Viewer"
-        },
-        STORM: {
-            leftWords: "Storm",
-            centerWords: "Damage",
-            rightWords: "Viewer",
-            title: "Storm Damage Viewer"
-        },
-        LAMDA: {
-            leftWords: "LAMDA",
-            centerWords: "DATA",
-            rightWords: "EXPLORER",
-            title: "LAMDA Data Explorer"
-        },
-        "lcms-dashboard": {
-            leftWords: "LCMS",
-            centerWords: "DASHBOARD",
-            rightWords: "Beta",
-            title: "LCMS Dashboard Beta"
-        },
-        "Bloom-Mapper": {
-            leftWords: "Bloom",
-            centerWords: "MAPPER",
-            rightWords: "",
-            title: "Bloom Mapper"
-        },
-        TreeMap: {
-            leftWords: "",
-            centerWords: "TreeMap",
-            rightWords: "Explorer",
-            title: "TreeMap Explorer"
-        }
     };
+
+function loadJS(e, a = !0, t) {
+    let o = document.createElement("script");
+    o.setAttribute("src", e), o.setAttribute("type", "text/javascript"), o.setAttribute("async", a), document.body.appendChild(o), o.addEventListener("load", (() => {
+        console.log("File loaded"), t()
+    })), o.addEventListener("error", (e => {
+        console.log("Error on loading file", e)
+    }))
+}
+const titles = {
+    "LCMS-pilot": {
+        leftWords: "LCMS",
+        centerWords: "DATA",
+        rightWords: "EXPLORER",
+        title: "LCMS Data Explorer"
+    },
+    LCMS: {
+        leftWords: "LCMS",
+        centerWords: "DATA",
+        rightWords: "EXPLORER",
+        title: "LCMS Data Explorer"
+    },
+    "lcms-base-learner": {
+        leftWords: "LCMS",
+        centerWords: "Base-Learner",
+        rightWords: "EXPLORER",
+        title: "LCMS Base Learner Explorer"
+    },
+    Ancillary: {
+        leftWords: "Ancillary",
+        centerWords: "DATA",
+        rightWords: "Viewer",
+        title: "TimeSync Ancillary Data Viewer"
+    },
+    LT: {
+        leftWords: "LandTrendr",
+        centerWords: "DATA",
+        rightWords: "EXPLORER",
+        title: "LandTrendr Data Explorer"
+    },
+    MTBS: {
+        leftWords: "MTBS",
+        centerWords: "DATA",
+        rightWords: "EXPLORER",
+        title: "MTBS Data Explorer"
+    },
+    TEST: {
+        leftWords: "TEST",
+        centerWords: "DATA",
+        rightWords: "Explorer",
+        title: "TEST Data Viewer"
+    },
+    IDS: {
+        leftWords: "IDS",
+        centerWords: "DATA",
+        rightWords: "EXPLORER",
+        title: "Insect and Disease Detection Survey Data Viewer"
+    },
+    geeViz: {
+        leftWords: "geeViz",
+        centerWords: "DATA",
+        rightWords: "Viewer",
+        title: "geeViz Data Viewer"
+    },
+    STORM: {
+        leftWords: "Storm",
+        centerWords: "Damage",
+        rightWords: "Viewer",
+        title: "Storm Damage Viewer"
+    },
+    LAMDA: {
+        leftWords: "LAMDA",
+        centerWords: "DATA",
+        rightWords: "EXPLORER",
+        title: "LAMDA Data Explorer"
+    },
+    "lcms-dashboard": {
+        leftWords: "LCMS",
+        centerWords: "DASHBOARD",
+        rightWords: "",
+        title: "LCMS Dashboard"
+    },
+    "Bloom-Mapper": {
+        leftWords: "Bloom",
+        centerWords: "MAPPER",
+        rightWords: "",
+        title: "Bloom Mapper"
+    },
+    TreeMap: {
+        leftWords: "",
+        centerWords: "TreeMap",
+        rightWords: "Explorer",
+        title: "TreeMap Explorer"
+    },
+    "sequoia-view": {
+        leftWords: "Giant",
+        centerWords: "Sequoia",
+        rightWords: "Viewer",
+        title: "Sequoia View"
+    }
+};
 let specificAuthErrorMessages = {
         LCMS: '<p>Try <a class = \'support-text\' title = "A simple LCMS output viewer" href = "lcms-in-motion.html" target="_blank">this viewer</a> for a simple visualization of LCMS data products.</p>\n                                <p>The <kbd>DOWNLOAD DATA</kbd> menu on the left (of this page) is still available for downloading LCMS data.</p>\n                                <p>For more information on LCMS please visit the <a class = \'support-text\' title = "LCMS Clearinghouse Page" href = "https://data.fs.usda.gov/geodata/rastergateway/LCMS/" target="_blank">LCMS Clearinghouse Page</a>.</p>',
         MTBS: '<p>Try <a class = \'support-text\' title = "MTBS Interactive Data Viewer" href = "https://www.mtbs.gov/viewer/?region=all" target="_blank">this viewer</a> for a simple MTBS product viewer.</p>'
     },
     specificAuthErrorMessage = specificAuthErrorMessages[mode];
 void 0 === specificAuthErrorMessage && (specificAuthErrorMessage = "");
 let authErrorMessageContact = `<p>Please contact the LCMS help desk <a class = 'intro-modal-links' href = "mailto: sm.fs.lcms@usda.gov">(sm.fs.lcms@usda.gov)</a> if you have questions/comments about the ${mode} viewer or have feedback.</p>`;
@@ -675,50 +690,51 @@
     lcmsSpinner: "<div id='lcms-spinner' style='position:absolute;right:40%; bottom:40%;width:10rem;height:8rem;z-index:10000000;display:none;'><img  alt= \"LCMS logo spinner\" title=\"Background processing is occurring\" class=\"fa fa-spin\" src=\"./images/lcms-icon.png\"  style='width:100%;height:100%'><span id = 'lcms-spinner-message'></span></div>",
     authErrorMessage: `<p>---  Error --- Map Loading Error ---</p>\n                                                              <p>Map data did not load correctly and cannot be used at this time. We apologize for this inconvenience and are working to resolve this issue.</p>\n                                                              ${specificAuthErrorMessage} \n                                                              ${authErrorMessageContact}\n    `,
     exportContainer: "<div class = 'py-2' id = 'export-list-container'>\n                        <h5>Choose which images to export:</h5>\n                        <div class = 'py-2' id=\"export-list\"></div>\n                        <hr>\n                        <div class = 'pl-3'>\n                            <form class=\"form-inline\" title = 'Provide projection. Web mercator: \"EPSG:4326\", USGS Albers: \"EPSG:5070\", WGS 84 UTM Northern Hemisphere: \"EPSG:326\" + zone number (e.g. zone 17 would be EPSG:32617), NAD 83 UTM Northern Hemisphere: \"EPSG:269\" + zone number (e.g. zone 17 would be EPSG:26917) '>\n                              <label for=\"export-crs\">Projection: </label>\n                              <div class=\"form-group pl-1\">\n                                <input type=\"text\" id=\"export-crs\" oninput = 'cacheCRS()' name=\"rg-from\" value=\"EPSG:4326\" class=\"form-control\">\n                              </div>\n                            </form>\n                            <div class = 'py-2' id = 'export-area-drawing-div'>\n                                <button class = 'btn' onclick = 'selectExportArea()' title = 'Draw polygon by clicking on map. Double-click to complete polygon, press ctrl+z to undo most recent point, press Delete or Backspace to start over.'><i class=\"pr-1 fa fa-pencil\" aria-hidden=\"true\"></i> Draw area to download</button>\n                                <a href=\"#\" onclick = 'undoExportArea()' title = 'Click to undo last drawn point (ctrl z)'><i class=\"btn fa fa-undo\"></i></a>\n                                <a href=\"#\" onclick = 'deleteExportArea()' title = 'Click to clear current drawing'><i class=\"btn fa fa-trash\"></i></a>\n                            </div>\n                            <hr>  \n                            <div class = 'pt-1 pb-3' >\n                                <div id = 'export-button-div'>\n                                    <button class = 'btn' onclick = 'exportImages()' title = 'Click to export selected images across selected area'><i class=\"pr-1 fa fa-cloud-download\" aria-hidden=\"true\"></i>Export Images</button>\n                                    <button class = 'btn' onclick = 'cancelAllTasks()' title = 'Click to cancel all active exports'></i>Cancel All Exports</button>\n                                </div>\n                                <hr>\n                                <span style = 'display:none;' class=\"fa-stack fa-2x py-0\" id='export-spinner' title=\"\">\n\t\t\t\t\t\t    \t\t<img alt= \"Google Earth Engine logo spinner\" class=\"fa fa-spin fa-stack-2x\" src=\"images/GEE_logo_transparent.png\" alt=\"\" style='width:2em;height:2em;'>\n\t\t\t\t\t\t   \t\t\t<strong id = 'export-count'  class=\"fa-stack-1x\" style = 'padding-left: 0.2em;padding-top: 0.1em;cursor:pointer;'></strong>\n\t\t\t\t\t\t\t\t</span>\n                                <div id = 'export-count-div'></div>\n                            </div>  \n                        </div>\n                        \n                    </div>",
     topBanner: ` <div id = 'title-banner' class = 'white  title-banner '>\n                    <img id='title-banner-icon-left' style = 'height:1.7rem;margin-top:0.25rem;'  alt="USDA Forest Service icon" src="images/logos_usda-fs.svg">\n                    <div class="vl"></div>\n                    <img id='title-banner-icon-right' style = 'width:1.6rem;height:1.7rem;margin-left:0.0rem;margin-right:0.1rem;margin-top:0.25rem;' >\n                    <div  class='my-0'>\n                    ${topBannerParams.leftWords} <span class = 'gray' style="font-weight:1000;font-family: 'Roboto Black', sans-serif;">${topBannerParams.centerWords}</span> ${topBannerParams.rightWords}</div>\n                </div>`,
     studyAreaDropdown: "<li   id = 'study-area-dropdown' class=\"nav-item dropdown navbar-dark navbar-nav nav-link p-0 col-12  \"  data-toggle=\"dropdown\">\n\t\t                <h5 href = '#' onclick = \"$('#sidebar-left').show('fade');$('#study-area-list').toggle();\" class = 'teal-study-area-label p-0 caret nav-link dropdown-toggle ' id='study-area-label'></h5> \n\t\t                <div class=\"dropdown-menu\" id=\"study-area-list\">  \n\t\t                </div>\n\t\t            </li>",
     placesSearchDiv: '<section id = \'search-share-div\' class="input-group  text-center search-bar" \'>\n\t\t\t            <div role=\'list\' class="input-group-prepend">\n                            <button onclick = \'getLocation()\' title = \'Click to center map at your location\' class=" btn input-group-text bg-white search-box pr-1 pl-2" id="get-location-button"><i class="fa fa-map-marker text-black "></i></button>\n\t    \t\t\t\t\t<button onclick = \'TweetThis()\' title = \'Click to share your current view\' class=" btn input-group-text bg-white search-box pr-1 pl-2" id="share-button"><i class="fa fa-share-alt teal "></i></button>\n                            <buttom class="input-group-text bg-white search-box" id="search-icon"><i class="fa fa-search text-black "></i></buttom>\n\t  \t\t\t\t\t</div>\n\t\t\t            <input id = \'pac-input\' class="form-control bg-white search-box" title = \'Search for places on the map\' type="text" placeholder="Search Places">\n                        <div class="input-group-prepend">\n                            <button onclick = \'backView()\' title = \'Click to go back a view\' class=" btn input-group-text bg-white search-box pr-1 pl-2" id="back-view-button"><i class="fa fa-chevron-left teal "></i></button>\n                            <button onclick = \'forwardView()\' title = \'Click to go forward a view\' style = \'border-radius: 0px 3px 3px 0px\' class=" btn input-group-text bg-white search-box pr-1 pl-2" id="forward-view-button"><i class="fa fa-chevron-right teal "></i></button>\n                        </div>\n                    </section>\n                    <p class = \'mt-0 mb-1 text-center white\' style = \'display:none;font-size:1.25rem;font-weight:bold\' id = \'time-lapse-year-label\'></p>',
     introModal: {
-        LCMS: getIntroModal("./images/lcms-icon.png", "Welcome to the Landscape Change Monitoring System (LCMS) Data Explorer!", "<p class='my-2'>\n                                    This Data Explorer provides the ability to view, analyze, summarize, and download LCMS data. \n                                    </p>\n                                    <p class='my-2'>\n                            LCMS is a remote sensing-based system for mapping and monitoring landscape change across the United States produced by the USDA Forest Service. LCMS provides a \"best available\" map of landscape change that leverages advances in time series-based change detection techniques, Landsat and Sentinel 2 data availability, cloud-based computing power, and big data analysis methods.\n\n                            </p>\n                            ", '<div style=\'display:inline-block;margin-top:0.5rem;\'>\n                            <div style =\'float:left;\' title=\'LCMS is produced by the USDA Forest Service\'>\n                                <img class = \'logo\' alt="USDA Forest Service icon" src="images/logos_usda-fs_bn-dk-01.svg">\n                                \n                            </div>\n                            <div style =\'float:left;\'>\n                                <ul class="intro-list">\n                                  <li title = "The Geospatial Technology and Applications Center (GTAC) provides leadership in geospatial science implementation in the USDA Forest Service by delivering vital services, data products, tools, training, and innovation to solve today\'s land and resource management challenges. All operational LCMS production and support takes place at GTAC."><a class="intro-modal-links" href="https://www.fs.usda.gov/about-agency/gtac" target="_blank">GTAC</a> Geospatial Technology and Applications Center\n                                  </li>\n                                  <li title = \'RedCastle Resources Inc. is the on-site contractor that has provided the technical expertise for LCMS\' operational production, documentation, and delivery at GTAC.\'><a class="intro-modal-links" href="https://www.redcastleresources.com/" target="_blank">RCR</a> RedCastle Resources Inc.\n                                  </li>\n                                  <li title = \'The Rocky Mountain Research Station provides the scientific foundation LCMS is built upon. They have been instrumental in developing and publishing the original LCMS methodology and continue to provide ongoing research and development to further improve LCMS methods.\'><a class="intro-modal-links" href="https://www.fs.usda.gov/rmrs/tools/landscape-change-monitoring-system-lcms" target="_blank">RMRS</a> Rocky Mountain Research Station\n                                  </li>\n                                  <li title = \'LCMS utilizes Google Earth Engine for most of its data acqusition, processing, and visualization through an enterprise agreement between the USDA Forest Service and Google. In its current form, LCMS would not be possible without Google Earth Engine.\'><a class="intro-modal-links" href="https://earthengine.google.com/" target="_blank">GEE</a> Google Earth Engine\n                                  </li>\n                                </ul>\n                                \n                            </div>\n                        \n                        </div>', '<p>Google Earth Engine data acquisition, processing, and visualization is possible by a USDA Forest Service enterprise agreement with Google.</p>\n                        <div class =\'my-3\'>\n                           <a  class = \'intro-modal-links\' onclick = \'downloadTutorial()\' title="Click to launch tutorial that explains how to utilize the Data Explorer">TUTORIAL</a>\n                            <a class="intro-modal-links" onclick="downloadMethods(\'v2021-7\')" title="Open in-depth LCMS v2021.7 methods documentation">LCMS METHODS</a>\n                            <a  class = \'intro-modal-links\'  onclick = \'openLCMSSurvey("splashScreen")\' title="Click to help us learn how you use LCMS and how we can make it better">LCMS USER SURVEY</a>\n                            <a class = "intro-modal-links" title = "Send us an E-mail" href = "mailto: sm.fs.lcms@usda.gov" >LCMS HELPDESK/FEEDBACK</a> \n                        </div>\n                        \n                        <div class =\'my-3\' title=\'There are additional data visualization tools available in these other sites\'>Other LCMS EXPLORERS:\n                            <a class = \'intro-modal-links\' title = "Visualize and explore summaries of LCMS data over different areas" href = "dashboard.html" target="_blank">LCMS Dashboard</a>\n                            <a class = \'intro-modal-links\' title = "Visualize and explore time series datasets used to create the LCMS map outputs" href = "lcms-base-learner.html" target="_blank">LCMS Base Learner Explorer</a>\n                            <a class = \'intro-modal-links\' title = "Visualize pre-made gifs illustrating patterns of change across USFS Forests and Districts" href = "lcms-in-motion.html" target="_blank">LCMS-in-Motion</a>\n                            \n                        </div>'),
-        "lcms-base-learner": getIntroModal("./images/lcms-icon.png", "Welcome to the Landscape Change Monitoring System (LCMS) Base-Learner Explorer!", "<p>LCMS is a landscape change detection program developed by the USDA Forest Service. This application is designed to provide a visualization of the change detection algorithm outputs that are used to produce LCMS products.</p>", "<p>In addition to the map layers, LandTrendr and CCDC outputs can be compared through charting under the <kbd>Tools</kbd> -> <kbd>Pixel Tools</kbd> and <kbd>Area Tools</kbd>\n                                    </p>", '<p>Please review this <a class = \'support-text\' onclick = \'downloadMethods("v2021-7")\' title = \'Open in-depth LCMS v2021.7 methods documentation\'>methods document</a> for more information about how these datasets are used to create LCMS products.   \n                            </p>\n                            <p>Google Earth Engine data acquisition, processing, and visualization is possible by a USDA Forest Service enterprise agreement with Google.</p>\n                            <div class =\'my-3\'>\n                            <a class="intro-modal-links" onclick="downloadMethods(\'v2021-7\')" title="Open in-depth LCMS v2021.7 methods documentation">LCMS METHODS</a>\n                            <a  class = \'intro-modal-links\'  onclick = \'openLCMSSurvey("splashScreen")\' title="Click to help us learn how you use LCMS and how we can make it better">LCMS USER SURVEY</a>\n                            <a class = "intro-modal-links" title = "Send us an E-mail" href = "mailto: sm.fs.lcms@usda.gov" >LCMS HELPDESK/FEEDBACK</a> \n                        </div>\n                        \n                        <div class =\'my-3\' title=\'There are additional data visualization tools available in these other sites\'>Other LCMS EXPLORERS:\n                            <a class = \'intro-modal-links\' title = "Visualize and explore LCMS final outputs" href = "index.html" target="_blank">LCMS Data Explorer</a>\n                            <a class = \'intro-modal-links\' title = "Visualize and explore summaries of LCMS data over different areas" href = "dashboard.html" target="_blank">LCMS Dashboard</a>\n                            <a class = \'intro-modal-links\' title = "Visualize pre-made gifs illustrating patterns of change across USFS Forests and Districts" href = "lcms-in-motion.html" target="_blank">LCMS-in-Motion</a>\n                            \n                        </div>'),
-        "lcms-dashboard": getIntroModal("./images/lcms-icon.png", "Welcome to the Landscape Change Monitoring System (LCMS) Data Dashboard!", "<p>LCMS is a landscape change detection program developed by the USDA Forest Service. This application is designed to provide the ability to quickly visualize and generate reports of how our landscapes are changing.</p>", '<p>Pre-calculated summary areas are available for generating custom reports.</p>\n                                    <p>Disclaimer: All summary numbers are based on modeled LCMS outputs. Known as model-based inference, error margins are difficult to compute directly from the summary pixel counts. Currently, error margins are calculated from the LCMS refence sample for each year from each summary area plus a 210km buffer. This assumes the statistical properties of the model-based and reference sample-based estimates are similar. Since this assumption is difficult to uphold, this method is still under scientific review. Theses tables are useful for understanding broad patterns of change on our landscape. For details on valid statistical conclusions and understanding map error, please refer to the <a class="intro-modal-links" onclick="downloadMethods(\'v2021-7\')" title="Open in-depth LCMS v2021.7 methods documentation">LCMS METHODS</a> document or reach out to the <a class = "intro-modal-links" title = "Send us an E-mail" href = "mailto: sm.fs.lcms@usda.gov" >LCMS HELPDESK</a>.\n                                    </p>', '<p>Google Earth Engine data acquisition, processing, and visualization is possible by a USDA Forest Service enterprise agreement with Google.</p>\n                            <div class =\'my-3\'>\n                            <a class="intro-modal-links" onclick="startTour()" title="Click to take a tour of the LCMS Dashboard\'s features">DASHBOARD TOUR</a>\n                            <a class="intro-modal-links" onclick="downloadMethods(\'v2021-7\')" title="Open in-depth LCMS v2021.7 methods documentation">LCMS METHODS</a>\n                            <a  class = \'intro-modal-links\'  onclick = \'openLCMSSurvey("splashScreen")\' title="Click to help us learn how you use LCMS and how we can make it better">LCMS USER SURVEY</a>\n                            <a class = "intro-modal-links" title = "Send us an E-mail" href = "mailto: sm.fs.lcms@usda.gov" >LCMS HELPDESK/FEEDBACK</a> \n                        </div>\n                        \n                        <div class =\'my-3\' title=\'There are additional data visualization tools available in these other sites\'>Other LCMS EXPLORERS:\n                            <a class = \'intro-modal-links\' title = "Visualize and explore LCMS final outputs" href = "index.html" target="_blank">LCMS Data Explorer</a>\n                            <a class = \'intro-modal-links\' title = "Visualize pre-made gifs illustrating patterns of change across USFS Forests and Districts" href = "lcms-in-motion.html" target="_blank">LCMS-in-Motion</a>\n                            \n                        </div>', "Loading LCMS summary areas. This can take some time"),
-        IDS: getIntroModal("./images/lcms-icon.png", "Welcome to the Landscape Change Monitoring System (LCMS) Insect and Disease Detection Survey (IDS) Explorer!", "<p>LCMS is a landscape change detection program developed by the USDA Forest Service. This application is designed to provide a visualization of the LCMS outputs alongside outputs from the USFS Forest Health Protection's <a class='intro-modal-links' href='https://www.fs.usda.gov/foresthealth/applied-sciences/mapping-reporting/detection-surveys.shtml' title = 'IDS homepage' target=\"_blank\">Insect and Disease Detection Survey (IDS)</a>outputs.</p>\n           \n           <p>LCMS Change and IDS polygon data can be viewed simultaneously for each coincident year. These data can also be compared through charting under the <kbd>Tools</kbd> -> <kbd>Pixel Tools</kbd> and <kbd>Area Tools</kbd>\n           </p>", '\n    <p>Google Earth Engine data acquisition, processing, and visualization is possible by a USDA Forest Service enterprise agreement with Google.</p>\n    <div class =\'my-3\'>\n    <a class="intro-modal-links" onclick="downloadMethods(\'v2021-7\')" title="Open in-depth LCMS v2021.7 methods documentation">LCMS METHODS</a>\n    <a  class = \'intro-modal-links\'  onclick = \'openLCMSSurvey("splashScreen")\' title="Click to help us learn how you use LCMS and how we can make it better">LCMS USER SURVEY</a>\n    <a class = "intro-modal-links" title = "Send us an E-mail" href = "mailto: sm.fs.lcms@usda.gov" >LCMS HELPDESK/FEEDBACK</a> \n</div>\n\n<div class =\'my-3\' title=\'There are additional data visualization tools available in these other sites\'>Other LCMS EXPLORERS:\n    <a class = \'intro-modal-links\' title = "Visualize and explore LCMS final outputs" href = "index.html" target="_blank">LCMS Data Explorer</a>\n    <a class = \'intro-modal-links\' title = "Visualize and explore summaries of LCMS data over different areas" href = "dashboard.html" target="_blank">LCMS Dashboard</a>\n    <a class = \'intro-modal-links\' title = "Visualize pre-made gifs illustrating patterns of change across USFS Forests and Districts" href = "lcms-in-motion.html" target="_blank">LCMS-in-Motion</a>\n    \n</div>', ""),
+        LCMS: getIntroModal("./images/lcms-icon.png", "Welcome to the Landscape Change Monitoring System (LCMS) Data Explorer!", "<p class='my-2'>\n                                    This Data Explorer provides the ability to view, analyze, summarize, and download LCMS data. \n                                    </p>\n                                    <p class='my-2'>\n                            LCMS is a remote sensing-based system for mapping and monitoring landscape change across the United States produced by the USDA Forest Service. LCMS provides a \"best available\" map of landscape change that leverages advances in time series-based change detection techniques, Landsat and Sentinel 2 data availability, cloud-based computing power, and big data analysis methods.\n\n                            </p>\n                            ", '<div style=\'display:inline-block;margin-top:0.5rem;\'>\n                            <div style =\'float:left;\' title=\'LCMS is produced by the USDA Forest Service\'>\n                                <img class = \'logo\' alt="USDA Forest Service icon" src="images/logos_usda-fs_bn-dk-01.svg">\n                                \n                            </div>\n                            <div style =\'float:left;\'>\n                                <ul class="intro-list">\n                                  <li title = "The Geospatial Technology and Applications Center (GTAC) provides leadership in geospatial science implementation in the USDA Forest Service by delivering vital services, data products, tools, training, and innovation to solve today\'s land and resource management challenges. All operational LCMS production and support takes place at GTAC."><a class="intro-modal-links" href="https://www.fs.usda.gov/about-agency/gtac" target="_blank">GTAC</a> Geospatial Technology and Applications Center\n                                  </li>\n                                  <li title = \'RedCastle Resources Inc. is the on-site contractor that has provided the technical expertise for LCMS\' operational production, documentation, and delivery at GTAC.\'><a class="intro-modal-links" href="https://www.redcastleresources.com/" target="_blank">RCR</a> RedCastle Resources Inc.\n                                  </li>\n                                  <li title = \'The Rocky Mountain Research Station provides the scientific foundation LCMS is built upon. They have been instrumental in developing and publishing the original LCMS methodology and continue to provide ongoing research and development to further improve LCMS methods.\'><a class="intro-modal-links" href="https://www.fs.usda.gov/rmrs/tools/landscape-change-monitoring-system-lcms" target="_blank">RMRS</a> Rocky Mountain Research Station\n                                  </li>\n                                  <li title = \'LCMS utilizes Google Earth Engine for most of its data acqusition, processing, and visualization through an enterprise agreement between the USDA Forest Service and Google. In its current form, LCMS would not be possible without Google Earth Engine.\'><a class="intro-modal-links" href="https://earthengine.google.com/" target="_blank">GEE</a> Google Earth Engine\n                                  </li>\n                                </ul>\n                                \n                            </div>\n                        \n                        </div>', '<p>Google Earth Engine data acquisition, processing, and visualization is possible by a USDA Forest Service enterprise agreement with Google.</p>\n                        <div class =\'my-3\'>\n                           <a  class = \'intro-modal-links\' onclick = \'downloadTutorial()\' title="Click to launch tutorial that explains how to utilize the Data Explorer">TUTORIAL</a>\n                            <a class="intro-modal-links" onclick="downloadMethods(\'v2022-8\')" title="Open in-depth LCMS v2022.8 methods documentation">LCMS METHODS</a>\n                            <a  class = \'intro-modal-links\'  onclick = \'openLCMSSurvey("splashScreen")\' title="Click to help us learn how you use LCMS and how we can make it better">LCMS USER SURVEY</a>\n                            <a class = "intro-modal-links" title = "Send us an E-mail" href = "mailto: sm.fs.lcms@usda.gov" >LCMS HELPDESK/FEEDBACK</a> \n                        </div>\n                        \n                        <div class =\'my-3\' title=\'There are additional data visualization tools available in these other sites\'>Other LCMS EXPLORERS:\n                            <a class = \'intro-modal-links\' title = "Visualize and explore summaries of LCMS data over different areas" href = "dashboard.html" target="_blank">LCMS Dashboard</a>\n                            <a class = \'intro-modal-links\' title = "Visualize and explore time series datasets used to create the LCMS map outputs" href = "lcms-base-learner.html" target="_blank">LCMS Base Learner Explorer</a>\n                            <a class = \'intro-modal-links\' title = "Visualize pre-made gifs illustrating patterns of change across USFS Forests and Districts" href = "lcms-in-motion.html" target="_blank">LCMS-in-Motion</a>\n                            \n                        </div>'),
+        "lcms-base-learner": getIntroModal("./images/lcms-icon.png", "Welcome to the Landscape Change Monitoring System (LCMS) Base-Learner Explorer!", "<p>LCMS is a landscape change detection program developed by the USDA Forest Service. This application is designed to provide a visualization of the change detection algorithm outputs that are used to produce LCMS products.</p>", "<p>In addition to the map layers, LandTrendr and CCDC outputs can be compared through charting under the <kbd>Tools</kbd> -> <kbd>Pixel Tools</kbd> and <kbd>Area Tools</kbd>\n                                    </p>", '<p>Please review this <a class = \'support-text\' onclick = \'downloadMethods("v2022-8")\' title = \'Open in-depth LCMS v2022.8 methods documentation\'>methods document</a> for more information about how these datasets are used to create LCMS products.   \n                            </p>\n                            <p>Google Earth Engine data acquisition, processing, and visualization is possible by a USDA Forest Service enterprise agreement with Google.</p>\n                            <div class =\'my-3\'>\n                            <a class="intro-modal-links" onclick="downloadMethods(\'v2022-8\')" title="Open in-depth LCMS v2022.8 methods documentation">LCMS METHODS</a>\n                            <a  class = \'intro-modal-links\'  onclick = \'openLCMSSurvey("splashScreen")\' title="Click to help us learn how you use LCMS and how we can make it better">LCMS USER SURVEY</a>\n                            <a class = "intro-modal-links" title = "Send us an E-mail" href = "mailto: sm.fs.lcms@usda.gov" >LCMS HELPDESK/FEEDBACK</a> \n                        </div>\n                        \n                        <div class =\'my-3\' title=\'There are additional data visualization tools available in these other sites\'>Other LCMS EXPLORERS:\n                            <a class = \'intro-modal-links\' title = "Visualize and explore LCMS final outputs" href = "index.html" target="_blank">LCMS Data Explorer</a>\n                            <a class = \'intro-modal-links\' title = "Visualize and explore summaries of LCMS data over different areas" href = "dashboard.html" target="_blank">LCMS Dashboard</a>\n                            <a class = \'intro-modal-links\' title = "Visualize pre-made gifs illustrating patterns of change across USFS Forests and Districts" href = "lcms-in-motion.html" target="_blank">LCMS-in-Motion</a>\n                            \n                        </div>'),
+        "lcms-dashboard": getIntroModal("./images/lcms-icon.png", "Welcome to the Landscape Change Monitoring System (LCMS) Data Dashboard!", "<p>LCMS is a landscape change detection program developed by the USDA Forest Service. This application is designed to provide the ability to quickly visualize and generate reports of how our landscapes are changing.</p>", '<p>Pre-calculated summary areas are available for generating custom reports.</p>\n                                    <p>Disclaimer: All summary numbers are based on modeled LCMS outputs. These tables are useful for understanding broad patterns of change on our landscape. Known as model-based inference, error margins are difficult to compute directly from the summary pixel counts. Currently, error margins are calculated from the LCMS reference sample for each year from each summary area, plus a 210km buffer. This assumes the statistical properties of the model-based and reference sample-based estimates are similar. Since this assumption is difficult to uphold, this method is still under scientific review. For details on valid statistical conclusions and understanding map error, please refer to the <a class="intro-modal-links" onclick="downloadMethods(\'v2022-8\')" title="Open in-depth LCMS v2022.8 methods documentation">LCMS METHODS</a> document or reach out to the <a class = "intro-modal-links" title = "Send us an E-mail" href = "mailto: sm.fs.lcms@usda.gov" >LCMS HELPDESK</a>.\n                                    </p>', '<p>Google Earth Engine data acquisition, processing, and visualization is possible by a USDA Forest Service enterprise agreement with Google.</p>\n                            <div class =\'my-3\'>\n                            <a class="intro-modal-links" onclick="startTour()" title="Click to take a tour of the LCMS Dashboard\'s features">DASHBOARD TOUR</a>\n                            <a class="intro-modal-links" onclick="downloadMethods(\'v2022-8\')" title="Open in-depth LCMS v2022.8 methods documentation">LCMS METHODS</a>\n                            <a  class = \'intro-modal-links\'  onclick = \'openLCMSSurvey("splashScreen")\' title="Click to help us learn how you use LCMS and how we can make it better">LCMS USER SURVEY</a>\n                            <a class = "intro-modal-links" title = "Send us an E-mail" href = "mailto: sm.fs.lcms@usda.gov" >LCMS HELPDESK/FEEDBACK</a> \n                        </div>\n                        \n                        <div class =\'my-3\' title=\'There are additional data visualization tools available in these other sites\'>Other LCMS EXPLORERS:\n                            <a class = \'intro-modal-links\' title = "Visualize and explore LCMS final outputs" href = "index.html" target="_blank">LCMS Data Explorer</a>\n                            <a class = \'intro-modal-links\' title = "Visualize pre-made gifs illustrating patterns of change across USFS Forests and Districts" href = "lcms-in-motion.html" target="_blank">LCMS-in-Motion</a>\n                            \n                        </div>', "Loading LCMS summary areas. This can take some time"),
+        IDS: getIntroModal("./images/lcms-icon.png", "Welcome to the Landscape Change Monitoring System (LCMS) Insect and Disease Detection Survey (IDS) Explorer!", "<p>LCMS is a landscape change detection program developed by the USDA Forest Service. This application is designed to provide a visualization of the LCMS outputs alongside outputs from the USFS Forest Health Protection's <a class='intro-modal-links' href='https://www.fs.usda.gov/foresthealth/applied-sciences/mapping-reporting/detection-surveys.shtml' title = 'IDS homepage' target=\"_blank\">Insect and Disease Detection Survey (IDS)</a>outputs.</p>\n           \n           <p>LCMS Change and IDS polygon data can be viewed simultaneously for each coincident year. These data can also be compared through charting under the <kbd>Tools</kbd> -> <kbd>Pixel Tools</kbd> and <kbd>Area Tools</kbd>\n           </p>", '\n    <p>Google Earth Engine data acquisition, processing, and visualization is possible by a USDA Forest Service enterprise agreement with Google.</p>\n    <div class =\'my-3\'>\n    <a class="intro-modal-links" onclick="downloadMethods(\'v2022-8\')" title="Open in-depth LCMS v2022.8 methods documentation">LCMS METHODS</a>\n    <a  class = \'intro-modal-links\'  onclick = \'openLCMSSurvey("splashScreen")\' title="Click to help us learn how you use LCMS and how we can make it better">LCMS USER SURVEY</a>\n    <a class = "intro-modal-links" title = "Send us an E-mail" href = "mailto: sm.fs.lcms@usda.gov" >LCMS HELPDESK/FEEDBACK</a> \n</div>\n\n<div class =\'my-3\' title=\'There are additional data visualization tools available in these other sites\'>Other LCMS EXPLORERS:\n    <a class = \'intro-modal-links\' title = "Visualize and explore LCMS final outputs" href = "index.html" target="_blank">LCMS Data Explorer</a>\n    <a class = \'intro-modal-links\' title = "Visualize and explore summaries of LCMS data over different areas" href = "dashboard.html" target="_blank">LCMS Dashboard</a>\n    <a class = \'intro-modal-links\' title = "Visualize pre-made gifs illustrating patterns of change across USFS Forests and Districts" href = "lcms-in-motion.html" target="_blank">LCMS-in-Motion</a>\n    \n</div>', ""),
         Ancillary: '<div class="modal fade "  id="introModal" tabindex="-1" role="dialog" >\n                <div class="modal-dialog modal-md " role="document">\n                    <div class="modal-content text-dark" style = \'background-color:rgba(230,230,230,0.95);\'>\n                        <button type="button" class="close p-2 ml-auto text-dark" data-dismiss="modal">&times;</button>\n                        <div class = \'modal-header\'>\n                            <h3 class="mb-0 ">Welcome to the TimeSync Ancillary Data Viewer!</h3>\n                        </div>\n                        <div class="modal-body" id = \'introModal-body\'>\n                            <p class="pb-2 ">This viewer is intended to provide an efficient way of looking at ancillary data to help with responses for the TimeSync tool.</p>\n                        </div>\n                        <div class = \'modal-footer\' id = \'introModal-footer\'>\n                        <div class = \' ml-0\' id = \'intro-modal-loading-div\'>\n                            <p>\n                              <img style="width:1.8em;" class="image-icon fa-spin mr-1" alt= "Google Earth Engine logo spinner" src="images/GEE_logo_transparent.png">\n                                Creating map services within Google Earth Engine. \n                             </p>\n                        </div>\n\t\t\t\t\t\t<div class="form-check  mr-0">\n                                <input role="option" type="checkbox" class="form-check-input" id="dontShowAgainCheckbox"   name = \'dontShowAgain\' value = \'true\'>\n                                <label class=" text-uppercase form-check-label " for="dontShowAgainCheckbox" >Don\'t show again</label>\n                            </div>\n                        </div>\n                    </div>\n                </div>\n            </div>',
         LT: getIntroModal("./images/lcms-icon.png", "Welcome to the LandTrendr Data Explorer!", '<li>\n           <p class="pb-2 ">This tool allows for quick exploration of significant changes visible in the Landsat time series using the <a class = \'intro-modal-links\' href="https://emapr.github.io/LT-GEE/" target="_blank">LandTrendr temporal segmentation algorithm</a>. While this tool can run across any area on earth, the quality of the output will be related to the availability of cloud-free Landsat observations.</p>\n       </li>\n       <li>\n           <p class="pb-2 ">LandTrendr will run across the entire extent of the map when it is loaded. If you would like to map a different area, move to the view extent you would like to map, and then press the <kbd>Submit</kbd> button at the bottom of the <kbd>PARAMETERS</kbd> collapse menu.</p>\n       </li>\n        <li>\n           <p class="pb-2 ">All Landsat image processing and LandTrendr algorithm application is being performed on-the-fly. This can take some time to run. If you try to run this tool across a very large extent (zoom level < 9), it may not run.</p>\n       </li>', '\n    <p>Google Earth Engine data acquisition, processing, and visualization is possible by a USDA Forest Service enterprise agreement with Google.</p>\n    <div class =\'my-3\'>\n    <a class="intro-modal-links" href="https://emapr.github.io/LT-GEE/" target="_blank" title="Open additional LandTrendr resources">LandTrendr Guide</a>\n    <a class = "intro-modal-links" title = "Send us an E-mail" href = "mailto: sm.fs.lcms@usda.gov" >LCMS HELPDESK/FEEDBACK</a> \n</div>\n\n<div class =\'my-3\' title=\'There are additional data visualization tools available in these other sites\'>Other LCMS EXPLORERS:\n    <a class = \'intro-modal-links\' title = "Visualize and explore LCMS final outputs" href = "index.html" target="_blank">LCMS Data Explorer</a>\n    <a class = \'intro-modal-links\' title = "Visualize and explore time series datasets used to create the LCMS map outputs (Includes both LandTrendr and CCDC outputs)" href = "lcms-base-learner.html" target="_blank">LCMS Base Learner Explorer</a>\n    <a class = \'intro-modal-links\' title = "Visualize and explore summaries of LCMS data over different areas" href = "dashboard.html" target="_blank">LCMS Dashboard</a>\n    <a class = \'intro-modal-links\' title = "Visualize pre-made gifs illustrating patterns of change across USFS Forests and Districts" href = "lcms-in-motion.html" target="_blank">LCMS-in-Motion</a>\n    \n</div>', ""),
         MTBS: getIntroModal("./images/mtbs-logo.png", "Welcome to the MTBS Data Explorer!", "<p class='my-2'>This tool is intended to allow for interactive exploration of the Monitoring Trends in Burn Severity (MTBS) data record.\n            </p>\n            <p class='my-2'>\n            Monitoring Trends in Burn Severity (MTBS) is a multiagency program designed to consistently map the burn severity and perimeters of fires across all lands of the United States from 1984 and beyond. MTBS maps wildland and prescribed fires greater than 1,000 acres in the Western US and 500 acres in the Eastern US. \n    </p>\n    <p class='my-2'>\n    MTBS burn severity data are used to assess the impacts to landscape health and can be used to monitor trends in wildfire over time.\n    </p>\n    ", '<div style=\'display:inline-block;margin-top:0.5rem;\'>\n    <div style =\'float:left;display:block\' title=\'MTBS is jointly produced by the USDA Forest Service and USGS\'>\n        <img class = \'logo\' alt="USDA Forest Service icon" src="images/logos_usda-fs_bn-dk-01.svg">\n        <br>\n        <img class = \'logo\' style = \'margin-left:0.3rem;height:2.5rem;\' alt="USGS icon" src="images/USGS_logo_green.svg">\n    </div>\n    <div style =\'float:left;\'>\n        <ul class="intro-list">\n          <li title = "The Geospatial Technology and Applications Center (GTAC) provides leadership in geospatial science implementation in the USDA Forest Service by delivering vital services, data products, tools, training, and innovation to solve today\'s land and resource management challenges. This Explorer was developed at GTAC.""><a class="intro-modal-links" href="https://www.fs.usda.gov/about-agency/gtac" target="_blank">GTAC</a> Geospatial Technology and Applications Center\n          </li>\n          <li title = "The Earth Resources Observation and Science (EROS) Center studies land change and produce land change data products used by researchers, resource managers, and policy makers across the nation and around the world. They also operate the Landsat satellite program with NASA, and maintain the largest civilian collection of images of the Earth\'s land surface in existence, including tens of millions of satellite images.""><a class="intro-modal-links" href="https://www.usgs.gov/centers/eros" target="_blank">EROS</a> Earth Resources Observation and Science Center\n          </li>\n          <li title = "This site utilizes Google Earth Engine for most of its data acqusition, processing, and visualization through an enterprise agreement between the USDA Forest Service and Google.""><a class="intro-modal-links" href="https://earthengine.google.com/" target="_blank">GEE</a> Google Earth Engine\n          </li>\n        </ul>\n        \n    </div>\n\n</div>', '<p>Google Earth Engine data acquisition, processing, and visualization is possible by a USDA Forest Service enterprise agreement with Google.</p>\n<div class =\'my-3\'>\n   <a  class = \'intro-modal-links\' onclick = \'toggleWalkThroughCollapse()\' title="Run interactive walk-through of the features of the MTBS Data Explorer">Run Walk-Through</a>\n\n    <a class = "intro-modal-links" title = "Contact us" href="https://www.mtbs.gov/contact" target="_blank"  >CONTACT</a> \n</div>\n\n'),
         LAMDA: getIntroModal("./Icons_svg/logo_gtac_color-wt.svg", "Welcome to the Landscape Automated Monitoring and Detection Algorithm (LAMDA) Data Explorer!", "<li>\n           <p class=\"pb-2 \">LAMDA is a near real-time landscape-scale change detection program developed by the USDA Forest Service to serve as a 'hot spot' indicator for areas where finer resolution data may be used for further investigation and to serve as an indicator of severe changes over forested regions. This application is designed to provide a visualization of LAMDA outputs.</p>\n       </li>\n       ", '\n    <p>Google Earth Engine data acquisition, processing, and visualization is possible by a USDA Forest Service enterprise agreement with Google.</p>\n    <div class =\'my-3\'>\n    <a class = "intro-modal-links" title = "Publication outlining the methods used to derive these products" href = "https://www.mdpi.com/2072-4292/10/8/1184" target="_blank" >LAMDA Methods Publication</a>\n    <a class="intro-modal-links" href="./lamda-downloads.html" target="_blank" title="LAMDA product download page">Download LAMDA Data</a>\n    <a class = "intro-modal-links" title = "Send us an E-mail" href = "mailto: sm.fs.lcms@usda.gov" >HELPDESK/FEEDBACK</a> \n</div>\n<div class =\'my-3\' title=\'There are additional change data visualization tools available in these other sites\'>Other EXPLORERS:\n    <a class = \'intro-modal-links\' title = "Visualize and explore LCMS final outputs" href = "index.html" target="_blank">LCMS Data Explorer</a>\n    <a class = \'intro-modal-links\' title = "Visualize and explore time series datasets used to create the LCMS map outputs (Includes both LandTrendr and CCDC outputs)" href = "lcms-base-learner.html" target="_blank">LCMS Base Learner Explorer</a>\n    <a class = \'intro-modal-links\' title = "Visualize and explore summaries of LCMS data over different areas" href = "dashboard.html" target="_blank">LCMS Dashboard</a>\n    <a class = \'intro-modal-links\' title = "Visualize pre-made gifs illustrating patterns of change across USFS Forests and Districts" href = "lcms-in-motion.html" target="_blank">LCMS-in-Motion</a>\n    \n</div>', ""),
+        "sequoia-view": getIntroModal("./Icons_svg/logo_gtac_color-wt.svg", "Welcome to the Giant Sequoia Viewer!", "<li>\n<p class=\"pb-2 \">This near real-time program developed by the USDA Forest Service to serve as a 'hot spot' indicator for areas where finer resolution data may be used for further investigation and to serve as an indicator of severe changes over forested regions. This application is designed to provide first cut alarm of potentially declining named Giant Sequoias and the ability to view available remote sensing image data.</p>\n</li>\n", `\n<p>Google Earth Engine data acquisition, processing, and visualization is possible by a USDA Forest Service enterprise agreement with Google.</p>\n<div class ='my-3'>\n<a class="intro-modal-links" onclick="startTour()" title="Click to take a tour of the ${mode}'s features">TOUR</a>\n<a class = "intro-modal-links" title = "Publication outlining the methods used to derive these products" href = "https://www.mdpi.com/2072-4292/10/8/1184" target="_blank" >LAMDA Methods Publication</a>\n\n<a class = "intro-modal-links" title = "Send us an E-mail" href = "mailto: sm.fs.lcms@usda.gov" >HELPDESK/FEEDBACK</a> \n</div>\n<div class ='my-3' title='There are additional change data visualization tools available in these other sites'>Other EXPLORERS:\n<a class = 'intro-modal-links' title = "Visualize and explore LAMDA products" href = "lamda-downloads.html" target="_blank">LAMDA Explorer</a>\n\n\n</div>`, ""),
         STORM: getIntroModal("./Icons_svg/logo_gtac_color-wt.svg", "Welcome to the Storm Damage Viewer!", "<p class='my-2'>\n                            This tool provides an interactive ability to upload storm tracks and produce modeled wind fields and tree damage. These outputs can then be downloaded for further analysis.\n\n                            </p>", '<div style=\'display:inline-block;margin-top:0.5rem;\'>\n    <div style =\'float:left;display:block\' title=\'This tool is produced by the USDA Forest Service\'>\n        <img class = \'logo\' alt="USDA Forest Service icon" src="images/logos_usda-fs_bn-dk-01.svg">\n    </div>\n    <div style =\'float:left;\'>\n        <ul class="intro-list">\n          <li title = "The Geospatial Technology and Applications Center (GTAC) provides leadership in geospatial science implementation in the USDA Forest Service by delivering vital services, data products, tools, training, and innovation to solve today\'s land and resource management challenges. This Explorer was developed at GTAC."><a class="intro-modal-links" href="https://www.fs.usda.gov/about-agency/gtac" target="_blank">GTAC</a> Geospatial Technology and Applications Center\n          </li>\n          <li title = \'The Southern Research Station provided the original methods for this data explorer.\'><a class="intro-modal-links" href="https://www.srs.fs.usda.gov/" target="_blank">SRS</a> Southern Research Station\n                                  </li>\n            <li title = \'RedCastle Resources Inc. is the on-site contractor that has provided the technical expertise for adapting the original workflow from the SRS and developing this Viewer.\'><a class="intro-modal-links" href="https://www.redcastleresources.com/" target="_blank">RCR</a> RedCastle Resources Inc.\n            </li>\n          <li title = \'This site utilizes Google Earth Engine for most of its data acqusition, processing, and visualization through an enterprise agreement between the USDA Forest Service and Google.\'><a class="intro-modal-links" href="https://earthengine.google.com/" target="_blank">GEE</a> Google Earth Engine\n          </li>\n        </ul>\n        \n    </div>\n\n</div>', '<p>Google Earth Engine data acquisition, processing, and visualization is possible by a USDA Forest Service enterprise agreement with Google.</p>\n\n<div class =\'my-3\'>\n    <a class = "intro-modal-links" title = "Report highlighting a project that used this tool" href = "https://apps.fs.usda.gov/gtac/publications/2022/tree-structure-damage-impact-predictive-trees-dip-modeling-phase-ii" target="_blank" >PROJECT REPORT</a>\n    <a class = "intro-modal-links" title = "Send us an E-mail" href = "mailto: sm.fs.lcms@usda.gov" >HELPDESK/FEEDBACK</a> \n</div>\n<div class =\'my-3\' title=\'There are additional change data visualization tools available in these other sites\'>Other EXPLORERS:\n    <a class = \'intro-modal-links\' title = "Visualize and explore LCMS final outputs" href = "index.html" target="_blank">LCMS Data Explorer</a>\n    <a class = \'intro-modal-links\' title = "Visualize and explore time series datasets used to create the LCMS map outputs (Includes both LandTrendr and CCDC outputs)" href = "lcms-base-learner.html" target="_blank">LCMS Base Learner Explorer</a>\n    <a class = \'intro-modal-links\' title = "Visualize and explore summaries of LCMS data over different areas" href = "dashboard.html" target="_blank">LCMS Dashboard</a>\n    <a class = \'intro-modal-links\' title = "Visualize pre-made gifs illustrating patterns of change across USFS Forests and Districts" href = "lcms-in-motion.html" target="_blank">LCMS-in-Motion</a>\n    \n</div>'),
         "Bloom-Mapper": getIntroModal("./Icons_svg/logo_gtac_color-wt.svg", "Welcome to the Bloom MAPPER!", "<p class='my-2'>\n            This prototype tool provides an interactive map with the ability to view lakes with potential cyanobacteria or algae blooms. These outputs have been created as a collaborative effort between field experts throughout Wyoming and the Geospatial Technology and Applications Center. Current methods are being tested for preliminary review. These products are not conclusive and are intended for review purposes only. \n            </p>", `<div style='display:inline-block;margin-top:0.5rem;'>\n    <div style ='float:left;display:block' title='Bloom mapper is a joint effort between GTAC and WY USFS partners'>\n        <img class = 'logo' alt="USDA Forest Service icon" src="images/logos_usda-fs_bn-dk-01.svg">\n        \n       \n        \n    </div>\n    <div style ='float:left;'>\n        <ul class="intro-list">\n          <li title = "The Geospatial Technology and Applications Center (GTAC) provides leadership in geospatial science implementation in the USDA Forest Service by delivering vital services, data products, tools, training, and innovation to solve today's land and resource management challenges. This Explorer was developed at GTAC."><a class="intro-modal-links" href="https://www.fs.usda.gov/about-agency/gtac" target="_blank">GTAC</a> Geospatial Technology and Applications Center\n          </li>\n          \n         \n            <li title = 'RedCastle Resources Inc. is the on-site contractor that has provided the technical expertise for adapting the original workflow from the SRS and developing this Viewer.'><a class="intro-modal-links" href="https://www.redcastleresources.com/" target="_blank">RCR</a> RedCastle Resources Inc.\n            </li>\n          <li title = 'This site utilizes Google Earth Engine for most of its data acqusition, processing, and visualization through an enterprise agreement between the USDA Forest Service and Google.'><a class="intro-modal-links" href="https://earthengine.google.com/" target="_blank">GEE</a> Google Earth Engine\n          </li>\n        </ul>\n        \n    </div>\n    <div class ='my-3'>\n                            <a class="intro-modal-links" onclick="startTour()" title="Click to take a tour of the ${mode}'s features">TOUR</a>\n                            <a class="intro-modal-links" onclick="downloadAnyMethods('./literature/Bloom_Mapper_v3_Methods_2023.pdf')" title="Open Bloom Mapper data creation methods documentation">METHODS</a>\n                            <a class = "intro-modal-links" title = "Send us an E-mail" href = "mailto: sm.fs.lcms@usda.gov" >HELPDESK/FEEDBACK</a> \n                        </div>\n\n</div>`, "<p>Google Earth Engine data acquisition, processing, and visualization is possible by a USDA Forest Service enterprise agreement with Google.</p>\n\n"),
         TreeMap: getIntroModal("./Icons_svg/logo_gtac_color-wt.svg", "Welcome to the TreeMap Explorer!", "<p class='my-2'>\n            This prototype tool provides an interactive map with the ability to view the 2016 TreeMap attributes. Source Data: Riley, Karin L.; Grenfell, Isaac C.; Finney, Mark A.; Shaw, John D. (2023). TreeMap 2016: A tree-level model of the forests of the conterminous United States circa 2016. Forest Service Research Data Archive. https://doi.org/10.2737/RDS-2021-0074. Accessed 2023-03-13. \n            </p>", `<div style='display:inline-block;margin-top:0.5rem;'>\n    <div style ='float:left;display:block' title='TreeMap Explorer is a joint effort between GTAC and USDA Forest Service Research'>\n        <img class = 'logo' alt="USDA Forest Service icon" src="images/logos_usda-fs_bn-dk-01.svg">\n        \n       \n        \n    </div>\n    <div style ='float:left;'>\n        <ul class="intro-list">\n          <li title = "The Geospatial Technology and Applications Center (GTAC) provides leadership in geospatial science implementation in the USDA Forest Service by delivering vital services, data products, tools, training, and innovation to solve today's land and resource management challenges. This Explorer was developed at GTAC."><a class="intro-modal-links" href="https://www.fs.usda.gov/about-agency/gtac" target="_blank">GTAC</a> Geospatial Technology and Applications Center\n          </li>\n          \n         \n            <li title = 'RedCastle Resources Inc. is the on-site contractor that has provided the technical expertise for adapting the original workflow from the SRS and developing this Viewer.'><a class="intro-modal-links" href="https://www.redcastleresources.com/" target="_blank">RCR</a> RedCastle Resources Inc.\n            </li>\n          <li title = 'This site utilizes Google Earth Engine for most of its data acqusition, processing, and visualization through an enterprise agreement between the USDA Forest Service and Google.'><a class="intro-modal-links" href="https://earthengine.google.com/" target="_blank">GEE</a> Google Earth Engine\n          </li>\n          <li title = 'TreeMap 2016 Research Dataset source data.'><a class="intro-modal-links" href="https://data.nal.usda.gov/dataset/treemap-2016-tree-level-model-forests-conterminous-united-states-circa-2016" target="_blank">RDS</a> TreeMap 2016 Data Source\n          </li>\n        </ul>\n        \n    </div>\n    <div class ='my-3'>\n                            <a class="intro-modal-links" onclick="startTour()" title="Click to take a tour of the ${mode}'s features">TOUR</a>\n                            <a class="intro-modal-links" href="https://academic.oup.com/jof/article/120/6/607/6701541" target="_blank" title="Open 2016 TreeMap documentation">METHODS</a>\n                            <a class = "intro-modal-links" title = "Send us an E-mail" href = "mailto: sm.fs.lcms@usda.gov" >HELPDESK/FEEDBACK</a> \n                        </div>\n\n</div>`, "<p>Google Earth Engine data acquisition, processing, and visualization is possible by a USDA Forest Service enterprise agreement with Google.</p>\n\n")
     },
     loadingModal: {
         all: function(e, a, t = "map services within Google Earth Engine") {
             let o = `<img class = 'logo' src="./images/${e}"   alt="${mode} logo image">`;
             return "" !== e && null != e || (o = ""), `<span>\n                                                           ${o} \n                                                            <h2 id = 'intro-modal-title-banner' title="" class = 'splash-title' style="font-weight:100;font-family: 'Roboto';">${topBannerParams.leftWords}<span  style="font-weight:1000;font-family: 'Roboto Black', sans-serif;"> ${topBannerParams.centerWords} </span> ${topBannerParams.rightWords}</h2>\n                                                        </span>\n\n                            \n\n                        <p style = 'margin-top:1rem;'>Google Earth Engine data acquisition, processing, and visualization is possible by a USDA Forest Service enterprise agreement with Google.</p>\n                <p style='font-weight:bold;margin-top:1rem;' title='Creating map services within Google Earth Engine. This can take some time. Thank you for your patience!'>\n                  <img style="width:2.1em;" class="image-icon fa-spin mr-1" alt= "Google Earth Engine logo spinner" src="images/GEE_logo_transparent.png">\n                    ${a} ${t}. This can take some time.\n                  \n                 </p>\n                  `
         },
         geeViz: '\n                <p>\n                  <img style="width:2.1em;" class="image-icon fa-spin mr-1" alt= "Google Earth Engine logo spinner" src="images/GEE_logo_transparent.png">\n                    Creating map services within Google Earth Engine. \n                  <br>\n                   <img style="width:2.1em;" class="image-icon fa-spin mr-1" alt= "Google Earth Engine logo spinner" src="images/GEE_logo_transparent.png">\n                    This can take some time. Thank you for your patience!\n                   <div id = \'loading-number-box\'></div>\n                 </p>\n                  '
     },
-    bottomBar: '<footer class = \'bottombar\'  id = \'bottombar\' >\n        \t\t\t<span class = \'px-2\'  id=\'current-tool-selection\' title="Any tool that is currently active is shown here."></span>\n        \t\t\t<span class = \'px-2\' title="All map layers are dynamically requested from Google Earth Engine.  The number of outstanding requests is shown here.">Queue length for maps from GEE: <span id=\'outstanding-gee-requests\'>0</span></span>\n                    <span class = \'px-2\' title="The number of outstanding map layers currently loading tiles.">Number of map layers loading tiles: <span id=\'number-gee-tiles-downloading\'>0</span></span>\n                    <span title="Current location and elevation of mouse pointer and map zoom level and respective map scale" class = \'px-2\'  id=\'current-mouse-position\'  ></span>\n                    <span id = \'contributor-logos\' > \n                        <a href="https://earthengine.google.com/" target="_blank">\n                            <img src="images/GEE.png"   class = \'image-icon-bar\' alt="Powered by Google Earth Engine"  href="#" title="Click to learn more about Google Earth Engine">\n                        </a>\n                        <a href="https://www.fs.usda.gov/" target="_blank">\n                            <img src="images/usfslogo.png" class = \'image-icon-bar\'  href="#"  alt= "USDA Forest Service logo" title="Click to learn more about the US Forest Service">\n                        </a>\n                        <a href="http://www.usda.gov" target="_blank">\n                            <img src="images/usdalogo.png" class = \'image-icon-bar\'  href="#"   alt= "USDA logo" title="Click to learn more about the USDA">\n                        </a>\n                    </span>\n                </footer>',
+    bottomBar: '<footer class = \'bottombar\'  id = \'bottombar\' >\n        \t\t\t<span class = \'px-1\'  id=\'current-tool-selection\' title="Any tool that is currently active is shown here."></span>\n        \t\t\t<span id = \'gee-queue-len\' class = \'px-1\' style="display:none;" title="All map layers are dynamically requested from Google Earth Engine.  The number of outstanding requests is shown here.">Queue length for maps from GEE: <span id=\'outstanding-gee-requests\'>0</span></span>\n                    <span class = \'px-1\' title="The number of outstanding map layers currently loading tiles.">Number of map layers loading: <span id=\'number-gee-tiles-downloading\'>0</span></span>\n                    <span title="Current location and elevation of mouse pointer and map zoom level and respective map scale" class = \'px-1\'  id=\'current-mouse-position\'  ></span>\n                    <span id = \'contributor-logos\' style=\'display:none;\'> \n                        <a href="https://earthengine.google.com/" target="_blank">\n                            <img src="images/GEE.png"   class = \'image-icon-bar\' alt="Powered by Google Earth Engine"  href="#" title="Click to learn more about Google Earth Engine">\n                        </a>\n                        <a href="https://www.fs.usda.gov/" target="_blank">\n                            <img src="images/usfslogo.png" class = \'image-icon-bar\'  href="#"  alt= "USDA Forest Service logo" title="Click to learn more about the US Forest Service">\n                        </a>\n                        <a href="http://www.usda.gov" target="_blank">\n                            <img src="images/usdalogo.png" class = \'image-icon-bar\'  href="#"   alt= "USDA logo" title="Click to learn more about the USDA">\n                        </a>\n                    </span>\n                </footer>',
     dashboardResultsDiv: "<div class = 'dashboard-results-container' id = 'dashboard-results-container' style='display:none;'>\n                                <div id ='dashboard-results-expander' title='Click and drag up and down to resize charts'></div>\n                                <div id='dashboard-results-div' class='bg-black dashboard-results'></div>\n                            </div>",
-    dashboardHighlightsDisclaimerText: "LCMS Dashboard Beta Disclaimer: All summary numbers are based on modeled LCMS outputs. Known as model-based inference, error margins are difficult to compute directly from the summary pixel counts. Currently, error margins are calculated from the LCMS refence sample for each year from each summary area plus a 210km buffer. This assumes the statistical properties of the model-based and reference sample-based estimates are similar. Since this assumption is difficult to uphold, this method is still under scientific review. Theses tables are useful for understanding broad patterns of change on our landscape. For details on valid statistical conclusions and understanding map error, please refer to the LCMS methods document or reach out to the LCMS HELPDESK",
-    dashboardHighlightsDiv: "<div id='dashboard-highlights-container' class='dashboard-highlights bg-black'>\n        <img style='height:3rem;' title = 'Click to toggle highlights visibility' class='sidebar-toggler' src='./images/menu-hamburger_ffffff.svg' onclick = 'toggleHighlights()' >\n        <p class='highlights-title highlights-div' style='' title = 'As you move the map around, summary areas that are visible will be ranked according to classes selected within the PARAMETERS menu'>Change Highlights</p>\n        <div class='dashboard-download-div' id = 'download-dashboard-report-container' title='Click to download charts and tables in a single pdf report.'>\n        <button class='btn dashboard-download-button' id='dashboard-download-button' onclick='makeDashboardReport()' >\n          <i class=\"fa fa-download dashboard-download-icon\" aria-hidden=\"true\"></i>\n          Download Report\n          \n        </button>\n        \n        \n      </div>\n        <div id='highlights-tables-container'>\n            <ul class=\"nav nav-tabs px-2 highlights-table-tabs\"  role=\"tablist\" id='highlights-table-tabs'></ul>\n            <div class=\"tab-content\" id=\"highlights-table-divs\"></div>\n            <p class = 'highlights-disclaimer'>Disclaimer: All summary numbers are based on modeled LCMS outputs. Known as model-based inference, error margins are difficult to compute directly from the summary pixel counts. Currently, error margins are calculated from the LCMS refence sample for each year from each summary area plus a 210km buffer. This assumes the statistical properties of the model-based and reference sample-based estimates are similar. Since this assumption is difficult to uphold, this method is still under scientific review. Theses tables are useful for understanding broad patterns of change on our landscape. For details on valid statistical conclusions and understanding map error, please refer to the <a class=\"teal\" onclick=\"downloadMethods('v2021-7')\" title=\"Open in-depth LCMS v2021.7 methods documentation\">LCMS METHODS</a> document or reach out to the <a class = \"teal\" title = \"Send us an E-mail\" href = \"mailto: sm.fs.lcms@usda.gov\" >LCMS HELPDESK</a>.\n            </p>\n        </div>\n        \n        </p>",
+    dashboardHighlightsDisclaimerText: "LCMS Dashboard Disclaimer: All summary numbers are based on modeled LCMS outputs. These tables are useful for understanding broad patterns of change on our landscape. Known as model-based inference, error margins are difficult to compute directly from the summary pixel counts. Currently, error margins are calculated from the LCMS reference sample for each year from each summary area, plus a 210km buffer. This assumes the statistical properties of the model-based and reference sample-based estimates are similar. Since this assumption is difficult to uphold, this method is still under scientific review. For details on valid statistical conclusions and understanding map error, please refer to the LCMS methods document or reach out to the LCMS HELPDESK",
+    dashboardHighlightsDiv: "<div id='dashboard-highlights-container' class='dashboard-highlights bg-black'>\n        <img style='height:3rem;' title = 'Click to toggle highlights visibility' class='sidebar-toggler' src='./images/menu-hamburger_ffffff.svg' onclick = 'toggleHighlights()' >\n        <p class='highlights-title highlights-div' style='' title = 'As you move the map around, summary areas that are visible will be ranked according to classes selected within the PARAMETERS menu'>Change Highlights</p>\n        <div class='dashboard-download-div' id = 'download-dashboard-report-container' title='Click to download charts and tables in a single pdf report.'>\n        <button class='btn dashboard-download-button' id='dashboard-download-button' onclick='makeDashboardReport()' >\n          <i class=\"fa fa-download dashboard-download-icon\" aria-hidden=\"true\"></i>\n          Download Report\n          \n        </button>\n        \n        \n      </div>\n        <div id='highlights-tables-container'>\n            <ul class=\"nav nav-tabs px-2 highlights-table-tabs\"  role=\"tablist\" id='highlights-table-tabs'></ul>\n            <div class=\"tab-content\" id=\"highlights-table-divs\"></div>\n            <p class = 'highlights-disclaimer'>Disclaimer: All summary numbers are based on modeled LCMS outputs. These tables are useful for understanding broad patterns of change on our landscape. Known as model-based inference, error margins are difficult to compute directly from the summary pixel counts. Currently, error margins are calculated from the LCMS reference sample for each year from each summary area, plus a 210km buffer. This assumes the statistical properties of the model-based and reference sample-based estimates are similar. Since this assumption is difficult to uphold, this method is still under scientific review. For details on valid statistical conclusions and understanding map error, please refer to the <a class=\"teal\" onclick=\"downloadMethods('v2022-8')\" title=\"Open in-depth LCMS v2022.8 methods documentation\">LCMS METHODS</a> document or reach out to the <a class = \"teal\" title = \"Send us an E-mail\" href = \"mailto: sm.fs.lcms@usda.gov\" >LCMS HELPDESK</a>.\n            </p>\n        </div>\n        \n        </p>",
     dashboardProgressDiv: `<div id = 'dashboard-progress-container' class='ml-3'>\n        <span  style = 'display: flex;'>\n        <img id = 'loading-spinner-logo' class = 'fa-spin progress-spinner' style='display:none;' src="./images/GEE_logo_transparent.png" height="${convertRemToPixels(.8)}"  alt="GEE logo image">\n        \n        <div class="progressbar" id='highlights-progressbar' class = 'px-2' title='Percent of summary areas that have finished downloading LCMS summary data'>\n            <span style="width: 0%;">0%</span>\n        </div>\n        <i  onclick='clearAllSelectedDashboardFeatures()' id='erase-all-dashboard-selected' title="Click to clear all selected features from this layer" class="fa fa-eraser eraser-all" ></i>\n        \n        </span>\n        \n        \n        \n        </div>`,
     walkThroughPopup: "<div class = 'walk-through-popup'>\n                            <div id = 'walk-through-popup-content' class = 'walk-through-popup-content'></div>\n\t                       \t\t<hr>\n\t\t                        <div class=\"icon-bar py-1 \">\n\t\t\t\t\t\t\t\t  <a onclick = 'previousWalkThrough()' title = 'Previous tutorial slide'><i class=\"fa fa-chevron-left text-black\"></i></a>\n\t\t\t\t\t\t\t\t  <a onclick = 'nextWalkThrough()'  title = 'Next tutorial slide'><i class=\"fa fa-chevron-right text-black\"></i></a>\n\t\t\t\t\t\t\t\t  <a id = 'walk-through-popup-progress'></a>\n                                  <a onclick = 'removeWalkThroughCollapse()' style = 'float:right;'  title = 'Turn off Walk-Through'><i class=\"fa fa-stop text-black\" aria-hidden=\"true\"></i></a>\n                                </div>\n\t\t\t\t\t\t</div>",
     studyAreaDropdownButtonEnabledTooltip: "Choose your study area",
     studyAreaDropdownButtonDisabledTooltip: "Still waiting on previous map layer requests. Can change study area once the previous requests are finished.",
     reRunButtonEnabledTooltip: "Once finished changing parameters, press this button to refresh map layers",
     reRunButtonDisabledTooltip: "Still waiting on previous map layer requests. Can re-submit once the previous requests are finished.",
     reRunButton: "<button id = 'reRun-button' onclick = 'reRun()' class = 'mb-1 ml-1 btn ' title=\"\">Submit</button>",
     addTimelapsesButton: "<button id = 'addTimelapses-button' onclick = 'addLCMSTimeLapses()' class = 'mb-1 ml-1 btn ' title=\"Add interactive time lapse of LCMS Change and Land Cover products. This will slow down the map loading\">Add LCMS Time Lapses To Map</button>",
     downloadDiv: '<div class = \'py-2\'>\n                        <a id = \'product-descriptions\' target = \'_blank\'>Detailed Product Description</a>\n        \t\t\t\t<hr>\n                        <label  title = \'Choose from dropdown below to download LCMS products. There can be a small delay before a download will begin, especially over slower networks.\' for="downloadDropdown">Select product to download:</label>\n    \t\t\t\t\t<select class="form-control" id = "downloadDropdown" onchange = "downloadSelectedArea()""></select>\n    \t\t\t\t </div>',
-    lcmsProductionDownloadDiv: '<ul id="downloadTree" class = \'pl-0 mb-0\' title = \'Click through available LCMS products. Select which outputs to download, and then click the download button. Hold ctrl key to select multiples or shift to select blocks.\'>\n                                          <li class = \'pl-0\'><span class="caret caret-down">Conterminous United States (v2021.7)</span>\n                                            <ul class="nested active">\n                                              <li><span class="caret">Change</span>\n                                                <ul class="nested">\n                                                  <li><span class="caret" title = \'Single layer summaries of what year change was mapped by LCMS serve as the foundational LCMS product that is easiest to work with in your local GIS. These are the same as the Slow Loss, Fast Loss, and Gain Year layers in the viewer.\'>Summary</span>\n                                                    <ul class="nested" id = \'CONUS-change-summary-downloads\'></ul>\n                                                  </li>\n                                                  <li><span class="caret" title = \'Annual change layers provide a more flexible product that can suite more customized data analysis. These are the same as the layers shown in the change time lapse.\'>Annual</span>\n                                                    <ul class="nested" id = \'CONUS-change-annual-downloads\'></ul>\n                                                  </li>\n                                                </ul>\n                                              </li>\n                                              <li><span class="caret" title = \'Annual land cover layers provide a more flexible product that can suite more customized data analysis. These are the same as the layers shown in the land cover time lapse.\'>Land Cover</span>\n                                                <ul class="nested" id = \'CONUS-land_cover-annual-downloads\'></ul>\n                                              </li>\n                                              <li><span class="caret" title = \'Annual land use layers provide a more flexible product that can suite more customized data analysis. These are the same as the layers shown in the land use time lapse.\'>Land Use</span>\n                                                <ul class="nested" id = \'CONUS-land_use-annual-downloads\'></ul>\n                                              </li>\n                                              <li><span class="caret" title = \'Annual QA-bits depict ancillary information about the origin of the data used to produce LCMS products.\'>QA Bits</span>\n                                                <ul class="nested" id = \'CONUS-qa_bits-annual-downloads\'></ul>\n                                              </li>\n                                            </ul>\n                                          </li>\n                                          <li><span class="caret caret-down">Southeastern Alaska (v2021.7)</span>\n                                            <ul class="nested active">\n                                              <li><span class="caret">Change</span>\n                                                <ul class="nested">\n                                                  <li><span class="caret" title = \'Single layer summaries of what year change was mapped by LCMS serve as the foundational LCMS product that is easiest to work with in your local GIS. These are the same as the Slow Loss, Fast Loss, and Gain Year layers in the viewer.\'>Summary</span>\n                                                    <ul class="nested" id = \'SEAK-change-summary-downloads\'></ul>\n                                                  </li>\n                                                  <li><span class="caret" title = \'Annual change layers provide a more flexible product that can suite more customized data analysis. These are the same as the layers shown in the change time lapse.\'>Annual</span>\n                                                    <ul class="nested" id = \'SEAK-change-annual-downloads\'></ul>\n                                                  </li>\n                                                </ul>\n                                              </li>\n                                              <li><span class="caret" title = \'Annual land cover layers provide a more flexible product that can suite more customized data analysis. These are the same as the layers shown in the land cover time lapse.\'>Land Cover</span>\n                                                <ul class="nested" id = \'SEAK-land_cover-annual-downloads\'></ul>\n                                              </li>\n                                              <li><span class="caret" title = \'Annual land use layers provide a more flexible product that can suite more customized data analysis. These are the same as the layers shown in the land use time lapse.\'>Land Use</span>\n                                                <ul class="nested" id = \'SEAK-land_use-annual-downloads\'></ul>\n                                              </li>\n                                              <li><span class="caret" title = \'Annual QA-bits depict ancillary information about the origin of the data used to produce LCMS products.\'>QA Bits</span>\n                                                <ul class="nested" id = \'SEAK-qa_bits-annual-downloads\'></ul>\n                                              </li>\n                                            </ul>\n                                          </li>\n                                          <li><span class="caret caret-down">Puerto Rico - US Virgin Islands (v2020.6)</span>\n                                            <ul class="nested active">\n                                              <li><span class="caret">Change</span>\n                                                <ul class="nested">\n                                                  <li><span class="caret" title = \'Single layer summaries of what year change was mapped by LCMS serve as the foundational LCMS product that is easiest to work with in your local GIS. These are the same as the Fast Loss, and Gain Year layers in the viewer.\'>Summary</span>\n                                                    <ul class="nested" id = \'PRUSVI-change-summary-downloads\'></ul>\n                                                  </li>\n                                                  <li><span class="caret" title = \'Annual change layers provide a more flexible product that can suite more customized data analysis. These are the same as the layers shown in the change time lapse.\'>Annual</span>\n                                                    <ul class="nested" id = \'PRUSVI-change-annual-downloads\'></ul>\n                                                  </li>\n                                                </ul>\n                                              </li>\n                                              <li><span class="caret" title = \'Annual land cover layers provide a more flexible product that can suite more customized data analysis. These are the same as the layers shown in the land cover time lapse.\'>Land Cover</span>\n                                                <ul class="nested" id = \'PRUSVI-land_cover-annual-downloads\'></ul>\n                                              </li>\n                                              <li><span class="caret" title = \'Annual land use layers provide a more flexible product that can suite more customized data analysis. These are the same as the layers shown in the land use time lapse.\'>Land Use</span>\n                                                <ul class="nested" id = \'PRUSVI-land_use-annual-downloads\'></ul>\n                                              </li>\n                                            </ul>\n                                          </li>\n                                        </ul>',
-    supportDiv: `<div  class = 'py-2 pl-3 pr-1'>\n                        <header class = 'row ' title = 'Open LCMS Data Explorer tutorial'>\n                            <h3 class = ' text-capitalize'>Tutorial</h3>\n                        </header>\n                        <div class = 'row ' title = 'Open LCMS Data Explorer tutorial'>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <img class = 'support-icons' alt = 'Information icon' src = './images/information--v2.png'></a> \n                            </div>\n                            <div class = 'col-lg-10'>\n                                <a id = 'tutorial-download' class = 'links' onclick = 'downloadTutorial()'>\n                                Click to launch a tutorial that explains how to utilize the Data Explorer</a>\n                            </div>\n                        </div>\n                        <hr>\n                        \n                        <header class = 'row ' title = 'Click to help us learn how you use LCMS and how we can make it better'>\n                        <h3 class = ' text-capitalize'>LCMS Survey</h3>\n                    </header>\n                    <div class = 'row ' title = 'Click to help us learn how you use LCMS and how we can make it better'>\n                        <div class = 'col-lg-2 p-0 m-0'>\n                            <img class = 'support-icons' alt = 'Methods icon' src = './Icons_svg/documentation_372e2c.svg'></a> \n                        </div>\n                        <div class = 'col-lg-10'>\n                            Click to open the LCMS Survey:\n                            <li>\n                            <a  class = 'intro-modal-links'  onclick = 'openLCMSSurvey("supportMenu")' title="Click to help us learn how you use LCMS and how we can make it better">SURVEY</a>\n                            </li>\n                             \n                        </div>\n                    </div>\n                    <hr>\n                         <header class = 'row ' title = 'Open in-depth LCMS methods documentation'>\n                            <h3 class = ' text-capitalize'>LCMS Methods</h3>\n                        </header>\n                        <div class = 'row ' title = 'Open in-depth LCMS methods documentation'>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <img class = 'support-icons' alt = 'Methods icon' src = './images/methods-icon.png'></a> \n                            </div>\n                            <div class = 'col-lg-10'>\n                                Click to open in-depth methods document:\n                                <li>\n                                    <a class = 'links' onclick = 'downloadMethods("v2021-7")' title = 'Open in-depth LCMS v2021.7 methods documentation'>Version 2021.7 (CONUS and SEAK)</a>\n                                </li>\n                                <li>\n                                    <a class = 'links' onclick = 'downloadMethods("v2020-6")' title = 'Open in-depth LCMS v2020.6 methods documentation'>Version 2020.6 (PRUSVI)</a>\n                                </li>   \n                            </div>\n                        </div>\n                        <hr>\n                        <header class = 'row'>\n                            <h3 class = ' text-capitalize' title = "In addition to this viewer, there are viewers to help visualize and explore other aspects of the LCMS data flow">Other LCMS Viewers</h3>\n                        </header>\n                        <section class = 'row'>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <a title = "In addition to this viewer, there are viewers to help visualize and explore other aspects of the LCMS data flow" ><img class = 'support-icons' alt = 'Email icon' src = './images/lcms-icon.png'></a> \n                            </div>\n                            <div class = 'col-lg-10'>\n                                <a class = 'links' title = "Visualize and explore time series datasets used to create the LCMS map outputs" href = "lcms-base-learner.html" target="_blank">LCMS Base Learner Explorer</a>\n                                <hr>\n                                <a class = 'links' title = "Visualize pre-made gifs illustrating patterns of change across USFS Forests and Districts" href = "lcms-in-motion.html" target="_blank">LCMS-in-Motion</a>\n                            </div>\n                        </section>\n                        <hr>\n                        <header class = 'row'>\n                            <h3 class = ' text-capitalize'>Acknowledgements</h3>\n                        </header>\n                        <section class = 'row'>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <a href="https://www.fs.usda.gov/about-agency/gtac" target="_blank">\n                                <img src="./images/GTAC_Logo.png" class = 'support-icons' alt="GTAC Logo"  href="#" alt = "Geospatial Technology and Applications Center logo" title="Click to learn more about the Geospatial Technology and Applications Center (GTAC)">\n                                </a>\n                            </div>\n                            <div class = 'col-lg-10'>\n                                <a href="https://www.fs.usda.gov/about-agency/gtac" target="_blank">\n                                    <p class = 'support-text'>The Geospatial Technology and Applications Center (GTAC) provides leadership in geospatial science implementation in the USDA Forest Service by delivering vital services, data products, tools, training, and innovation to solve today's land and resource management challenges. All operational LCMS production and support takes place at GTAC.</p>\n                                </a>\n                            </div>\n                        </section>\n                        <hr>\n                        <section class = 'row '>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <a href="https://www.redcastleresources.com/" target="_blank">\n                                    <img src="images/RCR-logo.jpg"  class = 'support-icons' alt="RedCastle Inc. Logo"  href="#"   title="Click to learn more about RedCastle Resources Inc."> \n                                </a>\n                            </div>\n                            <div class = 'col-lg-10'>\n                                <a href="https://www.redcastleresources.com/" target="_blank">\n                                    <p class = 'support-text'>RedCastle Resources Inc. is the on-site contractor that has provided the technical expertise for LCMS' operational production, documentation, and delivery at GTAC.</p>\n                                </a>\n                            </div>\n                        </section>\n                        <hr>\n                        <section class = 'row '>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <a href="https://www.fs.usda.gov/rmrs/tools/landscape-change-monitoring-system-lcms" target="_blank">\n                                <img src="./images/usfslogo.png" class = 'support-icons' alt="USFS Logo"  href="#"  title="Click to learn more about the Rocky Mountain Research Station (RMRS)">\n                                </a>\n                            </div>\n                            <div class = 'col-lg-10'>\n                                <a href="https://www.fs.usda.gov/rmrs/tools/landscape-change-monitoring-system-lcms" target="_blank">\n                                    <p class = 'support-text'>The Rocky Mountain Research Station provides the scientific foundation LCMS is built upon. They have been instrumental in developing and publishing the original LCMS methodology and continue to provide ongoing research and development to further improve LCMS methods.</p>\n                                </a>\n                            </div>\n                        </section>\n                        \n                        <hr>\n                        <section class = 'row'>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <a href="https://earthengine.google.com/" target="_blank">\n                                    <img src="images/GEE_logo_transparent.png"  class = 'support-icons' alt="Google Earth Engine Logo"  href="#"   title="Click to learn more about Google Earth Engine">\n                                    \n                                </a>\n                            </div>\n                            <div class = 'col-lg-10'>\n                                <a href="https://earthengine.google.com/" target="_blank">\n                                    <p class = 'support-text'>LCMS utilizes Google Earth Engine for most of its data acqusition, processing, and visualization, through an enterprise agreement between the USDA Forest Service and Google. In its current form, LCMS would not be possible without Google Earth Engine.</p>\n                                </a>\n                            </div>\n                        </section>\n                        <hr>\n                        <section class = 'row'>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <h2>"..."</h2>\n                            </div>\n                            <div class = 'col-lg-10  support-text'>\n                                    Suggested citation: \n                                    <p class = 'support-text' onclick = 'copyText("suggested-citation-text","copiedCitationMessageBox")' id = 'suggested-citation-text' title='Click to copy suggested citation to clipboard'>Forest Service, U.S. Department of Agriculture (2022). Landscape Change Monitoring System Data Explorer [Online]. Available at: https://apps.fs.usda.gov/lcms-viewer (Accessed: ${(new Date).toStringFormat()}).\n                                    </p>\n                                    <span>\n                                        <button onclick = 'copyText("suggested-citation-text","copiedCitationMessageBox")'' title = 'Click to copy suggested citation to clipboard' class="py-0 pr-1 fa fa-copy btn input-group-text bg-white" >\n                                        </button>\n                                        <p id = 'copiedCitationMessageBox'></p>\n                                    </span>\n                            </div>\n                        </section>\n                        <hr>\n                        <header class ='row'>\n                            <h3 class ='text-capitalize'>Contact</h3>\n                        </header>\n                        <section class = 'row '>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <a title = "Send us an E-mail" href = "mailto: sm.fs.lcms@usda.gov"><img class = 'support-icons' alt = 'Email icon' src = './images/email.png'></a> \n                            </div>\n                            <div class = 'col-lg-10'>\n                                <a class = 'support-text' title = "Send us an E-mail" href = "mailto: sm.fs.lcms@usda.gov">\n                                Please contact the LCMS help desk <span href = "mailto: sm.fs.lcms@usda.gov">(sm.fs.lcms@usda.gov)</span> if you have questions/comments about LCMS or have feedback on the LCMS Data Explorer.</a>\n                            </div>\n                        </section>\n        \t\t\t</div>`,
-    supportDivDashboard: `<div  class = 'py-2 pl-3 pr-1'>\n                        <header class = 'row ' title = 'Open LCMS Data Explorer tutorial'>\n                            <h3 class = ' text-capitalize'>Tutorial</h3>\n                        </header>\n                        <div class = 'row ' onclick="startTour()" title="Click to take a tour of the LCMS Dashboard's features">\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <img class = 'support-icons' alt = 'Information icon' src = './images/information--v2.png'></a> \n                            </div>\n                            <div class = 'col-lg-10'>\n                            <a class="intro-modal-links" onclick="startTour()" title="Click to take a tour of the LCMS Dashboard's features">DASHBOARD TOUR</a>\n                            </div>\n                        </div>\n                        <hr>\n                                                \n                        <header class = 'row ' title = 'Click to help us learn how you use LCMS and how we can make it better'>\n                        <h3 class = ' text-capitalize'>LCMS Survey</h3>\n                    </header>\n                    <div class = 'row ' title = 'Click to help us learn how you use LCMS and how we can make it better'>\n                        <div class = 'col-lg-2 p-0 m-0'>\n                            <img class = 'support-icons' alt = 'Methods icon' src = './Icons_svg/documentation_372e2c.svg'></a> \n                        </div>\n                        <div class = 'col-lg-10'>\n                            Click to open the LCMS Survey:\n                            <li>\n                            <a  class = 'intro-modal-links'  onclick = 'openLCMSSurvey("supportMenu")' title="Click to help us learn how you use LCMS and how we can make it better">SURVEY</a>\n                            </li>\n                             \n                        </div>\n                    </div>\n                    <hr>\n                         <header class = 'row ' title = 'Open in-depth LCMS methods documentation'>\n                            <h3 class = ' text-capitalize'>LCMS Methods</h3>\n                        </header>\n                        <div class = 'row ' title = 'Open in-depth LCMS methods documentation'>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <img class = 'support-icons' alt = 'Methods icon' src = './images/methods-icon.png'></a> \n                            </div>\n                            <div class = 'col-lg-10'>\n                                Click to open in-depth methods document:\n                                <li>\n                                    <a class = 'links' onclick = 'downloadMethods("v2021-7")' title = 'Open in-depth LCMS v2021.7 methods documentation'>Version 2021.7 (CONUS and SEAK)</a>\n                                </li>\n                                <li>\n                                    <a class = 'links' onclick = 'downloadMethods("v2020-6")' title = 'Open in-depth LCMS v2020.6 methods documentation'>Version 2020.6 (PRUSVI)</a>\n                                </li>   \n                            </div>\n                        </div>\n                        <hr>\n                         <header class = 'row ' title = 'Open in-depth LCMS methods documentation'>\n                            <h3 class = ' text-capitalize'>LCMS Methods</h3>\n                        </header>\n                        <div class = 'row ' title = 'Open in-depth LCMS methods documentation'>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <img class = 'support-icons' alt = 'Methods icon' src = './images/methods-icon.png'></a> \n                            </div>\n                            <div class = 'col-lg-10'>\n                                Click to open in-depth methods document:\n                                <li>\n                                    <a class = 'links' onclick = 'downloadMethods("v2021-7")' title = 'Open in-depth LCMS v2021.7 methods documentation'>Version 2021.7 (CONUS and SEAK)</a>\n                                </li>\n                                <li>\n                                    <a class = 'links' onclick = 'downloadMethods("v2020-6")' title = 'Open in-depth LCMS v2020.6 methods documentation'>Version 2020.6 (PRUSVI)</a>\n                                </li>   \n                            </div>\n                        </div>\n                        <hr>\n                        <header class = 'row'>\n                            <h3 class = ' text-capitalize' title = "In addition to this viewer, there are viewers to help visualize and explore other aspects of the LCMS data flow">Other LCMS Viewers</h3>\n                        </header>\n                        <section class = 'row'>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <a title = "In addition to this viewer, there are viewers to help visualize and explore other aspects of the LCMS data flow" ><img class = 'support-icons' alt = 'LCMS icon' src = './images/lcms-icon.png'></a> \n                            </div>\n                            <div class = 'col-lg-10'>\n                                <a class = 'links' title = "Visualize and explore LCMS map outputs" href = "index.html" target="_blank">LCMS Data Explorer</a>\n                                <hr>\n                                <a class = 'links' title = "Visualize and explore time series datasets used to create the LCMS map outputs" href = "lcms-base-learner.html" target="_blank">LCMS Base Learner Explorer</a>\n                                <hr>\n                                <a class = 'links' title = "Visualize pre-made gifs illustrating patterns of change across USFS Forests and Districts" href = "lcms-in-motion.html" target="_blank">LCMS-in-Motion</a>\n                            </div>\n                        </section>\n                        <hr>\n                        <header class = 'row'>\n                            <h3 class = ' text-capitalize'>Acknowledgements</h3>\n                        </header>\n                        <section class = 'row'>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <a href="https://www.fs.usda.gov/about-agency/gtac" target="_blank">\n                                <img src="./images/GTAC_Logo.png" class = 'support-icons' alt="GTAC Logo"  href="#" alt = "Geospatial Technology and Applications Center logo" title="Click to learn more about the Geospatial Technology and Applications Center (GTAC)">\n                                </a>\n                            </div>\n                            <div class = 'col-lg-10'>\n                                <a href="https://www.fs.usda.gov/about-agency/gtac" target="_blank">\n                                    <p class = 'support-text'>The Geospatial Technology and Applications Center (GTAC) provides leadership in geospatial science implementation in the USDA Forest Service by delivering vital services, data products, tools, training, and innovation to solve today's land and resource management challenges. All operational LCMS production and support takes place at GTAC.</p>\n                                </a>\n                            </div>\n                        </section>\n                        <hr>\n                        <section class = 'row '>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <a href="https://www.redcastleresources.com/" target="_blank">\n                                    <img src="images/RCR-logo.jpg"  class = 'support-icons' alt="RedCastle Inc. Logo"  href="#"   title="Click to learn more about RedCastle Resources Inc."> \n                                </a>\n                            </div>\n                            <div class = 'col-lg-10'>\n                                <a href="https://www.redcastleresources.com/" target="_blank">\n                                    <p class = 'support-text'>RedCastle Resources Inc. is the on-site contractor that has provided the technical expertise for LCMS' operational production, documentation, and delivery at GTAC.</p>\n                                </a>\n                            </div>\n                        </section>\n                        <hr>\n                        <section class = 'row '>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <a href="https://www.fs.usda.gov/rmrs/tools/landscape-change-monitoring-system-lcms" target="_blank">\n                                <img src="./images/usfslogo.png" class = 'support-icons' alt="USFS Logo"  href="#"  title="Click to learn more about the Rocky Mountain Research Station (RMRS)">\n                                </a>\n                            </div>\n                            <div class = 'col-lg-10'>\n                                <a href="https://www.fs.usda.gov/rmrs/tools/landscape-change-monitoring-system-lcms" target="_blank">\n                                    <p class = 'support-text'>The Rocky Mountain Research Station provides the scientific foundation LCMS is built upon. They have been instrumental in developing and publishing the original LCMS methodology and continue to provide ongoing research and development to further improve LCMS methods.</p>\n                                </a>\n                            </div>\n                        </section>\n                        \n                        <hr>\n                        <section class = 'row'>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <a href="https://earthengine.google.com/" target="_blank">\n                                    <img src="images/GEE_logo_transparent.png"  class = 'support-icons' alt="Google Earth Engine Logo"  href="#"   title="Click to learn more about Google Earth Engine">\n                                    \n                                </a>\n                            </div>\n                            <div class = 'col-lg-10'>\n                                <a href="https://earthengine.google.com/" target="_blank">\n                                    <p class = 'support-text'>LCMS utilizes Google Earth Engine for most of its data acqusition, processing, and visualization, through an enterprise agreement between the USDA Forest Service and Google. In its current form, LCMS would not be possible without Google Earth Engine.</p>\n                                </a>\n                            </div>\n                        </section>\n                        <hr>\n                        <section class = 'row'>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <h2>"..."</h2>\n                            </div>\n                            <div class = 'col-lg-10  support-text'>\n                                    Suggested citation: \n                                    <p class = 'support-text' onclick = 'copyText("suggested-citation-text","copiedCitationMessageBox")' id = 'suggested-citation-text' title='Click to copy suggested citation to clipboard'>Forest Service, U.S. Department of Agriculture (2022). Landscape Change Monitoring System Dashboard [Online]. Available at: https://apps.fs.usda.gov/lcms-viewer/dashboard.html (Accessed: ${(new Date).toStringFormat()}).\n                                    </p>\n                                    <span>\n                                        <button onclick = 'copyText("suggested-citation-text","copiedCitationMessageBox")'' title = 'Click to copy suggested citation to clipboard' class="py-0 pr-1 fa fa-copy btn input-group-text bg-white" >\n                                        </button>\n                                        <p id = 'copiedCitationMessageBox'></p>\n                                    </span>\n                            </div>\n                        </section>\n                        <hr>\n                        <header class ='row'>\n                            <h3 class ='text-capitalize'>Contact</h3>\n                        </header>\n                        <section class = 'row '>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <a title = "Send us an E-mail" href = "mailto: sm.fs.lcms@usda.gov"><img class = 'support-icons' alt = 'Email icon' src = './images/email.png'></a> \n                            </div>\n                            <div class = 'col-lg-10'>\n                                <a class = 'support-text' title = "Send us an E-mail" href = "mailto: sm.fs.lcms@usda.gov">\n                                Please contact the LCMS help desk <span href = "mailto: sm.fs.lcms@usda.gov">(sm.fs.lcms@usda.gov)</span> if you have questions/comments about LCMS or have feedback on the LCMS Dashboard.</a>\n                            </div>\n                        </section>\n        \t\t\t</div>`,
-    supportDivAlgal: `<div  class = 'py-2 pl-3 pr-1'>\n                        <header class = 'row ' title = 'Open ${mode} tutorial'>\n                            <h3 class = ' text-capitalize'>Tutorial</h3>\n                        </header>\n                        <div class = 'row ' onclick="startTour()" title="Click to take a tour of the ${mode}'s features">\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <img class = 'support-icons' alt = 'Information icon' src = './images/information--v2.png'></a> \n                            </div>\n                            <div class = 'col-lg-10'>\n                            <a class="intro-modal-links" onclick="startTour()" title="Click to take a tour of the LCMS ${mode}'s features">${mode} TOUR</a>\n                            </div>\n                        </div>\n                        <hr>\n                         <header class = 'row ' title = 'Open in-depth ${mode} methods documentation'>\n                            <h3 class = ' text-capitalize'>${mode} Methods</h3>\n                        </header>\n                        <div class = 'row ' title = 'Open in-depth ${mode} methods documentation'>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <img class = 'support-icons' alt = 'Methods icon' src = './images/methods-icon.png'></a> \n                            </div>\n                            <div class = 'col-lg-10'>\n                                Click to open in-depth methods document:\n                                <li>\n                                <a class="intro-modal-links" onclick="downloadAnyMethods('./literature/Bloom_Mapper_v3_Methods_2023.pdf')" title="Open Bloom Mapper data creation methods documentation">Bloom Mapper V3 METHODS</a>\n                                </li>\n                            </div>\n                        </div>\n                        \n                        <hr>\n                        <header class = 'row'>\n                            <h3 class = ' text-capitalize'>Acknowledgements</h3>\n                        </header>\n                        <section class = 'row'>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <a href="https://www.fs.usda.gov/about-agency/gtac" target="_blank">\n                                <img src="./images/GTAC_Logo.png" class = 'support-icons' alt="GTAC Logo"  href="#" alt = "Geospatial Technology and Applications Center logo" title="Click to learn more about the Geospatial Technology and Applications Center (GTAC)">\n                                </a>\n                            </div>\n                            <div class = 'col-lg-10'>\n                                <a href="https://www.fs.usda.gov/about-agency/gtac" target="_blank">\n                                    <p class = 'support-text'>The Geospatial Technology and Applications Center (GTAC) provides leadership in geospatial science implementation in the USDA Forest Service by delivering vital services, data products, tools, training, and innovation to solve today's land and resource management challenges. All operational LCMS production and support takes place at GTAC.</p>\n                                </a>\n                            </div>\n                        </section>\n                        <hr>\n                        <section class = 'row '>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <a href="https://www.redcastleresources.com/" target="_blank">\n                                    <img src="images/RCR-logo.jpg"  class = 'support-icons' alt="RedCastle Inc. Logo"  href="#"   title="Click to learn more about RedCastle Resources Inc."> \n                                </a>\n                            </div>\n                            <div class = 'col-lg-10'>\n                                <a href="https://www.redcastleresources.com/" target="_blank">\n                                    <p class = 'support-text'>RedCastle Resources Inc. is the on-site contractor that has provided the technical expertise for ${mode}'s methods development, documentation, and visualization (this viewer) at GTAC.</p>\n                                </a>\n                            </div>\n                        </section>\n                        <hr>\n                        <section class = 'row '>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <a href="" target="_blank">\n                                    <img src="./images/usfslogo.png" class = 'support-icons' alt="USFS Logo"  href="#"  title="Click to learn more about our field collaborators ">\n                                </a>\n                                \n                                <a href="" target="_blank" >\n                                    <img class = 'support-icons' alt="Wyoming Department of Environmental Quality icon" src="images/WY-DEQ-Logo.png" style="margin-top: 1rem;padding-right: 0.5rem;">\n                                </a>\n                            </div>\n                            <div class = 'col-lg-10'>\n                                <a href="" target="_blank">\n                                    <p class = 'support-text'>\n                                    USFS units in Regions 2 and 4 in Wyoming collaborated to help GTAC develop and train this tool based on actual bloom data collected by the Wyoming Department of Environmental Quality, Water Quality Division, Watershed Protection Program as part of their state-wide monitoring efforts to document the occurrence of Harmful Cyanobacterial Blooms. Thousands of lakes over ~1 acre exist on Forest system lands in Wyoming. This tool is critical in helping Forest staff focus efforts to address this public safety concern.</p>\n                                </a>\n                            </div>\n                        </section>\n                        \n                        <hr>\n                        <section class = 'row'>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <a href="https://earthengine.google.com/" target="_blank">\n                                    <img src="images/GEE_logo_transparent.png"  class = 'support-icons' alt="Google Earth Engine Logo"  href="#"   title="Click to learn more about Google Earth Engine">\n                                    \n                                </a>\n                            </div>\n                            <div class = 'col-lg-10'>\n                                <a href="https://earthengine.google.com/" target="_blank">\n                                    <p class = 'support-text'>${mode} utilizes Google Earth Engine for most of its data acqusition, processing, and visualization, through an enterprise agreement between the USDA Forest Service and Google. In its current form, ${mode} would not be possible without Google Earth Engine.</p>\n                                </a>\n                            </div>\n                        </section>\n                        <hr>\n                        <section class = 'row'>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <h2>"..."</h2>\n                            </div>\n                            <div class = 'col-lg-10  support-text'>\n                                    Suggested citation: \n                                    <p class = 'support-text' onclick = 'copyText("suggested-citation-text","copiedCitationMessageBox")' id = 'suggested-citation-text' title='Click to copy suggested citation to clipboard'>Forest Service, U.S. Department of Agriculture (2022). ${mode} [Online]. Available at: https://apps.fs.usda.gov/lcms-viewer/${mode}.html (Accessed: ${(new Date).toStringFormat()}).\n                                    </p>\n                                    <span>\n                                        <button onclick = 'copyText("suggested-citation-text","copiedCitationMessageBox")'' title = 'Click to copy suggested citation to clipboard' class="py-0 pr-1 fa fa-copy btn input-group-text bg-white" >\n                                        </button>\n                                        <p id = 'copiedCitationMessageBox'></p>\n                                    </span>\n                            </div>\n                        </section>\n                        <hr>\n                        <header class ='row'>\n                            <h3 class ='text-capitalize'>Contact</h3>\n                        </header>\n                        <section class = 'row '>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <a title = "Send us an E-mail" href = "mailto: sm.fs.lcms@usda.gov"><img class = 'support-icons' alt = 'Email icon' src = './images/email.png'></a> \n                            </div>\n                            <div class = 'col-lg-10'>\n                                <a class = 'support-text' title = "Send us an E-mail" href = "mailto: sm.fs.lcms@usda.gov">\n                                Please contact the ${mode} help desk <span href = "mailto: sm.fs.lcms@usda.gov">(sm.fs.lcms@usda.gov)</span> if you have questions/comments about ${mode} or have feedback on the ${mode}.</a>\n                            </div>\n                        </section>\n        \t\t\t</div>`,
+    lcmsProductionDownloadDiv: '<ul id="downloadTree" class = \'pl-0 mb-0\' title = \'Click through available LCMS products. Select which outputs to download, and then click the download button. Hold ctrl key to select multiples or shift to select blocks.\'>\n                                          <li class = \'pl-0\'><span class="caret caret-down">Conterminous United States (v2022.8)</span>\n                                            <ul class="nested active">\n                                              <li><span class="caret">Change</span>\n                                                <ul class="nested">\n                                                  <li><span class="caret" title = \'Single layer summaries of what year change was mapped by LCMS serve as the foundational LCMS product that is easiest to work with in your local GIS. These are the same as the Slow Loss, Fast Loss, and Gain Year layers in the viewer.\'>Summary</span>\n                                                    <ul class="nested" id = \'CONUS-change-summary-downloads\'></ul>\n                                                  </li>\n                                                  <li><span class="caret" title = \'Annual change layers provide a more flexible product that can suite more customized data analysis. These are the same as the layers shown in the change time lapse.\'>Annual</span>\n                                                    <ul class="nested" id = \'CONUS-change-annual-downloads\'></ul>\n                                                  </li>\n                                                </ul>\n                                              </li>\n                                              <li><span class="caret" title = \'Annual land cover layers provide a more flexible product that can suite more customized data analysis. These are the same as the layers shown in the land cover time lapse.\'>Land Cover</span>\n                                                <ul class="nested" id = \'CONUS-land_cover-annual-downloads\'></ul>\n                                              </li>\n                                              <li><span class="caret" title = \'Annual land use layers provide a more flexible product that can suite more customized data analysis. These are the same as the layers shown in the land use time lapse.\'>Land Use</span>\n                                                <ul class="nested" id = \'CONUS-land_use-annual-downloads\'></ul>\n                                              </li>\n                                              <li><span class="caret" title = \'Annual QA-bits depict ancillary information about the origin of the data used to produce LCMS products.\'>QA Bits</span>\n                                                <ul class="nested" id = \'CONUS-qa_bits-annual-downloads\'></ul>\n                                              </li>\n                                            </ul>\n                                          </li>\n                                          <li><span class="caret caret-down">Southeastern Alaska (v2022.8)</span>\n                                            <ul class="nested active">\n                                              <li><span class="caret">Change</span>\n                                                <ul class="nested">\n                                                  <li><span class="caret" title = \'Single layer summaries of what year change was mapped by LCMS serve as the foundational LCMS product that is easiest to work with in your local GIS. These are the same as the Slow Loss, Fast Loss, and Gain Year layers in the viewer.\'>Summary</span>\n                                                    <ul class="nested" id = \'SEAK-change-summary-downloads\'></ul>\n                                                  </li>\n                                                  <li><span class="caret" title = \'Annual change layers provide a more flexible product that can suite more customized data analysis. These are the same as the layers shown in the change time lapse.\'>Annual</span>\n                                                    <ul class="nested" id = \'SEAK-change-annual-downloads\'></ul>\n                                                  </li>\n                                                </ul>\n                                              </li>\n                                              <li><span class="caret" title = \'Annual land cover layers provide a more flexible product that can suite more customized data analysis. These are the same as the layers shown in the land cover time lapse.\'>Land Cover</span>\n                                                <ul class="nested" id = \'SEAK-land_cover-annual-downloads\'></ul>\n                                              </li>\n                                              <li><span class="caret" title = \'Annual land use layers provide a more flexible product that can suite more customized data analysis. These are the same as the layers shown in the land use time lapse.\'>Land Use</span>\n                                                <ul class="nested" id = \'SEAK-land_use-annual-downloads\'></ul>\n                                              </li>\n                                              <li><span class="caret" title = \'Annual QA-bits depict ancillary information about the origin of the data used to produce LCMS products.\'>QA Bits</span>\n                                                <ul class="nested" id = \'SEAK-qa_bits-annual-downloads\'></ul>\n                                              </li>\n                                            </ul>\n                                          </li>\n                                          <li><span class="caret caret-down">Puerto Rico - US Virgin Islands (v2020.6)</span>\n                                            <ul class="nested active">\n                                              <li><span class="caret">Change</span>\n                                                <ul class="nested">\n                                                  <li><span class="caret" title = \'Single layer summaries of what year change was mapped by LCMS serve as the foundational LCMS product that is easiest to work with in your local GIS. These are the same as the Fast Loss, and Gain Year layers in the viewer.\'>Summary</span>\n                                                    <ul class="nested" id = \'PRUSVI-change-summary-downloads\'></ul>\n                                                  </li>\n                                                  <li><span class="caret" title = \'Annual change layers provide a more flexible product that can suite more customized data analysis. These are the same as the layers shown in the change time lapse.\'>Annual</span>\n                                                    <ul class="nested" id = \'PRUSVI-change-annual-downloads\'></ul>\n                                                  </li>\n                                                </ul>\n                                              </li>\n                                              <li><span class="caret" title = \'Annual land cover layers provide a more flexible product that can suite more customized data analysis. These are the same as the layers shown in the land cover time lapse.\'>Land Cover</span>\n                                                <ul class="nested" id = \'PRUSVI-land_cover-annual-downloads\'></ul>\n                                              </li>\n                                              <li><span class="caret" title = \'Annual land use layers provide a more flexible product that can suite more customized data analysis. These are the same as the layers shown in the land use time lapse.\'>Land Use</span>\n                                                <ul class="nested" id = \'PRUSVI-land_use-annual-downloads\'></ul>\n                                              </li>\n                                            </ul>\n                                          </li>\n                                        </ul>',
+    supportDiv: `<div  class = 'py-2 pl-3 pr-1'>\n                        <header class = 'row ' title = 'Open LCMS Data Explorer tutorial'>\n                            <h3 class = ' text-capitalize'>Tutorial</h3>\n                        </header>\n                        <div class = 'row ' title = 'Open LCMS Data Explorer tutorial'>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <img class = 'support-icons' alt = 'Information icon' src = './images/information--v2.png'></a> \n                            </div>\n                            <div class = 'col-lg-10'>\n                                <a id = 'tutorial-download' class = 'links' onclick = 'downloadTutorial()'>\n                                Click to launch a tutorial that explains how to utilize the Data Explorer</a>\n                            </div>\n                        </div>\n                        <hr>\n                        \n                        <header class = 'row ' title = 'Click to help us learn how you use LCMS and how we can make it better'>\n                        <h3 class = ' text-capitalize'>LCMS Survey</h3>\n                    </header>\n                    <div class = 'row ' title = 'Click to help us learn how you use LCMS and how we can make it better'>\n                        <div class = 'col-lg-2 p-0 m-0'>\n                            <img class = 'support-icons' alt = 'Methods icon' src = './Icons_svg/documentation_372e2c.svg'></a> \n                        </div>\n                        <div class = 'col-lg-10'>\n                            Click to open the LCMS Survey:\n                            <li>\n                            <a  class = 'intro-modal-links'  onclick = 'openLCMSSurvey("supportMenu")' title="Click to help us learn how you use LCMS and how we can make it better">SURVEY</a>\n                            </li>\n                             \n                        </div>\n                    </div>\n                    <hr>\n                         <header class = 'row ' title = 'Open in-depth LCMS methods documentation'>\n                            <h3 class = ' text-capitalize'>LCMS Methods</h3>\n                        </header>\n                        <div class = 'row ' title = 'Open in-depth LCMS methods documentation'>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <img class = 'support-icons' alt = 'Methods icon' src = './images/methods-icon.png'></a> \n                            </div>\n                            <div class = 'col-lg-10'>\n                                Click to open in-depth methods document:\n                                <li>\n                                    <a class = 'links' onclick = 'downloadMethods("v2022-8")' title = 'Open in-depth LCMS v2022.8 methods documentation'>Version 2022.8 (CONUS and SEAK)</a>\n                                </li>\n                                <li>\n                                    <a class = 'links' onclick = 'downloadMethods("v2020-6")' title = 'Open in-depth LCMS v2020.6 methods documentation'>Version 2020.6 (PRUSVI)</a>\n                                </li>   \n                            </div>\n                        </div>\n                        <hr>\n                        <header class = 'row'>\n                            <h3 class = ' text-capitalize' title = "In addition to this viewer, there are viewers to help visualize and explore other aspects of the LCMS data flow">Other LCMS Viewers</h3>\n                        </header>\n                        <section class = 'row'>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <a title = "In addition to this viewer, there are viewers to help visualize and explore other aspects of the LCMS data flow" ><img class = 'support-icons' alt = 'Email icon' src = './images/lcms-icon.png'></a> \n                            </div>\n                            <div class = 'col-lg-10'>\n                                <a class = 'links' title = "Visualize and explore time series datasets used to create the LCMS map outputs" href = "lcms-base-learner.html" target="_blank">LCMS Base Learner Explorer</a>\n                                <hr>\n                                <a class = 'links' title = "Visualize pre-made gifs illustrating patterns of change across USFS Forests and Districts" href = "lcms-in-motion.html" target="_blank">LCMS-in-Motion</a>\n                            </div>\n                        </section>\n                        <hr>\n                        <header class = 'row'>\n                            <h3 class = ' text-capitalize'>Acknowledgements</h3>\n                        </header>\n                        <section class = 'row'>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <a href="https://www.fs.usda.gov/about-agency/gtac" target="_blank">\n                                <img src="./images/GTAC_Logo.png" class = 'support-icons' alt="GTAC Logo"  href="#" alt = "Geospatial Technology and Applications Center logo" title="Click to learn more about the Geospatial Technology and Applications Center (GTAC)">\n                                </a>\n                            </div>\n                            <div class = 'col-lg-10'>\n                                <a href="https://www.fs.usda.gov/about-agency/gtac" target="_blank">\n                                    <p class = 'support-text'>The Geospatial Technology and Applications Center (GTAC) provides leadership in geospatial science implementation in the USDA Forest Service by delivering vital services, data products, tools, training, and innovation to solve today's land and resource management challenges. All operational LCMS production and support takes place at GTAC.</p>\n                                </a>\n                            </div>\n                        </section>\n                        <hr>\n                        <section class = 'row '>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <a href="https://www.redcastleresources.com/" target="_blank">\n                                    <img src="images/RCR-logo.jpg"  class = 'support-icons' alt="RedCastle Inc. Logo"  href="#"   title="Click to learn more about RedCastle Resources Inc."> \n                                </a>\n                            </div>\n                            <div class = 'col-lg-10'>\n                                <a href="https://www.redcastleresources.com/" target="_blank">\n                                    <p class = 'support-text'>RedCastle Resources Inc. is the on-site contractor that has provided the technical expertise for LCMS' operational production, documentation, and delivery at GTAC.</p>\n                                </a>\n                            </div>\n                        </section>\n                        <hr>\n                        <section class = 'row '>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <a href="https://www.fs.usda.gov/rmrs/tools/landscape-change-monitoring-system-lcms" target="_blank">\n                                <img src="./images/usfslogo.png" class = 'support-icons' alt="USFS Logo"  href="#"  title="Click to learn more about the Rocky Mountain Research Station (RMRS)">\n                                </a>\n                            </div>\n                            <div class = 'col-lg-10'>\n                                <a href="https://www.fs.usda.gov/rmrs/tools/landscape-change-monitoring-system-lcms" target="_blank">\n                                    <p class = 'support-text'>The Rocky Mountain Research Station provides the scientific foundation LCMS is built upon. They have been instrumental in developing and publishing the original LCMS methodology and continue to provide ongoing research and development to further improve LCMS methods.</p>\n                                </a>\n                            </div>\n                        </section>\n                        \n                        <hr>\n                        <section class = 'row'>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <a href="https://earthengine.google.com/" target="_blank">\n                                    <img src="images/GEE_logo_transparent.png"  class = 'support-icons' alt="Google Earth Engine Logo"  href="#"   title="Click to learn more about Google Earth Engine">\n                                    \n                                </a>\n                            </div>\n                            <div class = 'col-lg-10'>\n                                <a href="https://earthengine.google.com/" target="_blank">\n                                    <p class = 'support-text'>LCMS utilizes Google Earth Engine for most of its data acqusition, processing, and visualization, through an enterprise agreement between the USDA Forest Service and Google. In its current form, LCMS would not be possible without Google Earth Engine.</p>\n                                </a>\n                            </div>\n                        </section>\n                        <hr>\n                        <section class = 'row'>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <h2>"..."</h2>\n                            </div>\n                            <div class = 'col-lg-10  support-text'>\n                                    Suggested citation: \n                                    <p class = 'support-text' onclick = 'copyText("suggested-citation-text","copiedCitationMessageBox")' id = 'suggested-citation-text' title='Click to copy suggested citation to clipboard'>Forest Service, U.S. Department of Agriculture (2023). Landscape Change Monitoring System Data Explorer [Online]. Available at: https://apps.fs.usda.gov/lcms-viewer (Accessed: ${(new Date).toStringFormat()}).\n                                    </p>\n                                    <span>\n                                        <button onclick = 'copyText("suggested-citation-text","copiedCitationMessageBox")'' title = 'Click to copy suggested citation to clipboard' class="py-0 pr-1 fa fa-copy btn input-group-text bg-white" >\n                                        </button>\n                                        <p id = 'copiedCitationMessageBox'></p>\n                                    </span>\n                            </div>\n                        </section>\n                        <hr>\n                        <header class ='row'>\n                            <h3 class ='text-capitalize'>Contact</h3>\n                        </header>\n                        <section class = 'row '>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <a title = "Send us an E-mail" href = "mailto: sm.fs.lcms@usda.gov"><img class = 'support-icons' alt = 'Email icon' src = './images/email.png'></a> \n                            </div>\n                            <div class = 'col-lg-10'>\n                                <a class = 'support-text' title = "Send us an E-mail" href = "mailto: sm.fs.lcms@usda.gov">\n                                Please contact the LCMS help desk <span href = "mailto: sm.fs.lcms@usda.gov">(sm.fs.lcms@usda.gov)</span> if you have questions/comments about LCMS or have feedback on the LCMS Data Explorer.</a>\n                            </div>\n                        </section>\n        \t\t\t</div>`,
+    supportDivDashboard: `<div  class = 'py-2 pl-3 pr-1'>\n                        <header class = 'row ' title = 'Open LCMS Data Explorer tutorial'>\n                            <h3 class = ' text-capitalize'>Tutorial</h3>\n                        </header>\n                        <div class = 'row ' onclick="startTour()" title="Click to take a tour of the LCMS Dashboard's features">\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <img class = 'support-icons' alt = 'Information icon' src = './images/information--v2.png'></a> \n                            </div>\n                            <div class = 'col-lg-10'>\n                            <a class="intro-modal-links" onclick="startTour()" title="Click to take a tour of the LCMS Dashboard's features">DASHBOARD TOUR</a>\n                            </div>\n                        </div>\n                        <hr>\n                                                \n                        <header class = 'row ' title = 'Click to help us learn how you use LCMS and how we can make it better'>\n                        <h3 class = ' text-capitalize'>LCMS Survey</h3>\n                    </header>\n                    <div class = 'row ' title = 'Click to help us learn how you use LCMS and how we can make it better'>\n                        <div class = 'col-lg-2 p-0 m-0'>\n                            <img class = 'support-icons' alt = 'Methods icon' src = './Icons_svg/documentation_372e2c.svg'></a> \n                        </div>\n                        <div class = 'col-lg-10'>\n                            Click to open the LCMS Survey:\n                            <li>\n                            <a  class = 'intro-modal-links'  onclick = 'openLCMSSurvey("supportMenu")' title="Click to help us learn how you use LCMS and how we can make it better">SURVEY</a>\n                            </li>\n                             \n                        </div>\n                    </div>\n                    <hr>\n                         <header class = 'row ' title = 'Open in-depth LCMS methods documentation'>\n                            <h3 class = ' text-capitalize'>LCMS Methods</h3>\n                        </header>\n                        <div class = 'row ' title = 'Open in-depth LCMS methods documentation'>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <img class = 'support-icons' alt = 'Methods icon' src = './images/methods-icon.png'></a> \n                            </div>\n                            <div class = 'col-lg-10'>\n                                Click to open in-depth methods document:\n                                <li>\n                                    <a class = 'links' onclick = 'downloadMethods("v2022-8")' title = 'Open in-depth LCMS v2022.8 methods documentation'>Version 2022.8 (CONUS and SEAK)</a>\n                                </li>\n                                <li>\n                                    <a class = 'links' onclick = 'downloadMethods("v2020-6")' title = 'Open in-depth LCMS v2020.6 methods documentation'>Version 2020.6 (PRUSVI)</a>\n                                </li>   \n                            </div>\n                        </div>\n                        <hr>\n                         <header class = 'row ' title = 'Open in-depth LCMS methods documentation'>\n                            <h3 class = ' text-capitalize'>LCMS Methods</h3>\n                        </header>\n                        <div class = 'row ' title = 'Open in-depth LCMS methods documentation'>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <img class = 'support-icons' alt = 'Methods icon' src = './images/methods-icon.png'></a> \n                            </div>\n                            <div class = 'col-lg-10'>\n                                Click to open in-depth methods document:\n                                <li>\n                                    <a class = 'links' onclick = 'downloadMethods("v2022-8")' title = 'Open in-depth LCMS v2022.8 methods documentation'>Version 2022.8 (CONUS and SEAK)</a>\n                                </li>\n                                <li>\n                                    <a class = 'links' onclick = 'downloadMethods("v2020-6")' title = 'Open in-depth LCMS v2020.6 methods documentation'>Version 2020.6 (PRUSVI)</a>\n                                </li>   \n                            </div>\n                        </div>\n                        <hr>\n                        <header class = 'row'>\n                            <h3 class = ' text-capitalize' title = "In addition to this viewer, there are viewers to help visualize and explore other aspects of the LCMS data flow">Other LCMS Viewers</h3>\n                        </header>\n                        <section class = 'row'>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <a title = "In addition to this viewer, there are viewers to help visualize and explore other aspects of the LCMS data flow" ><img class = 'support-icons' alt = 'LCMS icon' src = './images/lcms-icon.png'></a> \n                            </div>\n                            <div class = 'col-lg-10'>\n                                <a class = 'links' title = "Visualize and explore LCMS map outputs" href = "index.html" target="_blank">LCMS Data Explorer</a>\n                                <hr>\n                                <a class = 'links' title = "Visualize and explore time series datasets used to create the LCMS map outputs" href = "lcms-base-learner.html" target="_blank">LCMS Base Learner Explorer</a>\n                                <hr>\n                                <a class = 'links' title = "Visualize pre-made gifs illustrating patterns of change across USFS Forests and Districts" href = "lcms-in-motion.html" target="_blank">LCMS-in-Motion</a>\n                            </div>\n                        </section>\n                        <hr>\n                        <header class = 'row'>\n                            <h3 class = ' text-capitalize'>Acknowledgements</h3>\n                        </header>\n                        <section class = 'row'>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <a href="https://www.fs.usda.gov/about-agency/gtac" target="_blank">\n                                <img src="./images/GTAC_Logo.png" class = 'support-icons' alt="GTAC Logo"  href="#" alt = "Geospatial Technology and Applications Center logo" title="Click to learn more about the Geospatial Technology and Applications Center (GTAC)">\n                                </a>\n                            </div>\n                            <div class = 'col-lg-10'>\n                                <a href="https://www.fs.usda.gov/about-agency/gtac" target="_blank">\n                                    <p class = 'support-text'>The Geospatial Technology and Applications Center (GTAC) provides leadership in geospatial science implementation in the USDA Forest Service by delivering vital services, data products, tools, training, and innovation to solve today's land and resource management challenges. All operational LCMS production and support takes place at GTAC.</p>\n                                </a>\n                            </div>\n                        </section>\n                        <hr>\n                        <section class = 'row '>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <a href="https://www.redcastleresources.com/" target="_blank">\n                                    <img src="images/RCR-logo.jpg"  class = 'support-icons' alt="RedCastle Inc. Logo"  href="#"   title="Click to learn more about RedCastle Resources Inc."> \n                                </a>\n                            </div>\n                            <div class = 'col-lg-10'>\n                                <a href="https://www.redcastleresources.com/" target="_blank">\n                                    <p class = 'support-text'>RedCastle Resources Inc. is the on-site contractor that has provided the technical expertise for LCMS' operational production, documentation, and delivery at GTAC.</p>\n                                </a>\n                            </div>\n                        </section>\n                        <hr>\n                        <section class = 'row '>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <a href="https://www.fs.usda.gov/rmrs/tools/landscape-change-monitoring-system-lcms" target="_blank">\n                                <img src="./images/usfslogo.png" class = 'support-icons' alt="USFS Logo"  href="#"  title="Click to learn more about the Rocky Mountain Research Station (RMRS)">\n                                </a>\n                            </div>\n                            <div class = 'col-lg-10'>\n                                <a href="https://www.fs.usda.gov/rmrs/tools/landscape-change-monitoring-system-lcms" target="_blank">\n                                    <p class = 'support-text'>The Rocky Mountain Research Station provides the scientific foundation LCMS is built upon. They have been instrumental in developing and publishing the original LCMS methodology and continue to provide ongoing research and development to further improve LCMS methods.</p>\n                                </a>\n                            </div>\n                        </section>\n                        \n                        <hr>\n                        <section class = 'row'>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <a href="https://earthengine.google.com/" target="_blank">\n                                    <img src="images/GEE_logo_transparent.png"  class = 'support-icons' alt="Google Earth Engine Logo"  href="#"   title="Click to learn more about Google Earth Engine">\n                                    \n                                </a>\n                            </div>\n                            <div class = 'col-lg-10'>\n                                <a href="https://earthengine.google.com/" target="_blank">\n                                    <p class = 'support-text'>LCMS utilizes Google Earth Engine for most of its data acqusition, processing, and visualization, through an enterprise agreement between the USDA Forest Service and Google. In its current form, LCMS would not be possible without Google Earth Engine.</p>\n                                </a>\n                            </div>\n                        </section>\n                        <hr>\n                        <section class = 'row'>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <h2>"..."</h2>\n                            </div>\n                            <div class = 'col-lg-10  support-text'>\n                                    Suggested citation: \n                                    <p class = 'support-text' onclick = 'copyText("suggested-citation-text","copiedCitationMessageBox")' id = 'suggested-citation-text' title='Click to copy suggested citation to clipboard'>Forest Service, U.S. Department of Agriculture (2023). Landscape Change Monitoring System Dashboard [Online]. Available at: https://apps.fs.usda.gov/lcms-viewer/dashboard.html (Accessed: ${(new Date).toStringFormat()}).\n                                    </p>\n                                    <span>\n                                        <button onclick = 'copyText("suggested-citation-text","copiedCitationMessageBox")'' title = 'Click to copy suggested citation to clipboard' class="py-0 pr-1 fa fa-copy btn input-group-text bg-white" >\n                                        </button>\n                                        <p id = 'copiedCitationMessageBox'></p>\n                                    </span>\n                            </div>\n                        </section>\n                        <hr>\n                        <header class ='row'>\n                            <h3 class ='text-capitalize'>Contact</h3>\n                        </header>\n                        <section class = 'row '>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <a title = "Send us an E-mail" href = "mailto: sm.fs.lcms@usda.gov"><img class = 'support-icons' alt = 'Email icon' src = './images/email.png'></a> \n                            </div>\n                            <div class = 'col-lg-10'>\n                                <a class = 'support-text' title = "Send us an E-mail" href = "mailto: sm.fs.lcms@usda.gov">\n                                Please contact the LCMS help desk <span href = "mailto: sm.fs.lcms@usda.gov">(sm.fs.lcms@usda.gov)</span> if you have questions/comments about LCMS or have feedback on the LCMS Dashboard.</a>\n                            </div>\n                        </section>\n        \t\t\t</div>`,
+    supportDivAlgal: `<div  class = 'py-2 pl-3 pr-1'>\n                        <header class = 'row ' title = 'Open ${mode} tutorial'>\n                            <h3 class = ' text-capitalize'>Tutorial</h3>\n                        </header>\n                        <div class = 'row ' onclick="startTour()" title="Click to take a tour of the ${mode}'s features">\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <img class = 'support-icons' alt = 'Information icon' src = './images/information--v2.png'></a> \n                            </div>\n                            <div class = 'col-lg-10'>\n                            <a class="intro-modal-links" onclick="startTour()" title="Click to take a tour of the LCMS ${mode}'s features">${mode} TOUR</a>\n                            </div>\n                        </div>\n                        <hr>\n                         <header class = 'row ' title = 'Open in-depth ${mode} methods documentation'>\n                            <h3 class = ' text-capitalize'>${mode} Methods</h3>\n                        </header>\n                        <div class = 'row ' title = 'Open in-depth ${mode} methods documentation'>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <img class = 'support-icons' alt = 'Methods icon' src = './images/methods-icon.png'></a> \n                            </div>\n                            <div class = 'col-lg-10'>\n                                Click to open in-depth methods document:\n                                <li>\n                                <a class="intro-modal-links" onclick="downloadAnyMethods('./literature/Bloom_Mapper_v3_Methods_2023.pdf')" title="Open Bloom Mapper data creation methods documentation">Bloom Mapper V3 METHODS</a>\n                                </li>\n                            </div>\n                        </div>\n                        \n                        <hr>\n                        <header class = 'row'>\n                            <h3 class = ' text-capitalize'>Acknowledgements</h3>\n                        </header>\n                        <section class = 'row'>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <a href="https://www.fs.usda.gov/about-agency/gtac" target="_blank">\n                                <img src="./images/GTAC_Logo.png" class = 'support-icons' alt="GTAC Logo"  href="#" alt = "Geospatial Technology and Applications Center logo" title="Click to learn more about the Geospatial Technology and Applications Center (GTAC)">\n                                </a>\n                            </div>\n                            <div class = 'col-lg-10'>\n                                <a href="https://www.fs.usda.gov/about-agency/gtac" target="_blank">\n                                    <p class = 'support-text'>The Geospatial Technology and Applications Center (GTAC) provides leadership in geospatial science implementation in the USDA Forest Service by delivering vital services, data products, tools, training, and innovation to solve today's land and resource management challenges. All operational LCMS production and support takes place at GTAC.</p>\n                                </a>\n                            </div>\n                        </section>\n                        <hr>\n                        <section class = 'row '>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <a href="https://www.redcastleresources.com/" target="_blank">\n                                    <img src="images/RCR-logo.jpg"  class = 'support-icons' alt="RedCastle Inc. Logo"  href="#"   title="Click to learn more about RedCastle Resources Inc."> \n                                </a>\n                            </div>\n                            <div class = 'col-lg-10'>\n                                <a href="https://www.redcastleresources.com/" target="_blank">\n                                    <p class = 'support-text'>RedCastle Resources Inc. is the on-site contractor that has provided the technical expertise for ${mode}'s methods development, documentation, and visualization (this viewer) at GTAC.</p>\n                                </a>\n                            </div>\n                        </section>\n                        <hr>\n                        <section class = 'row '>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <a href="" target="_blank">\n                                    <img src="./images/usfslogo.png" class = 'support-icons' alt="USFS Logo"  href="#"  title="Click to learn more about our field collaborators ">\n                                </a>\n                                \n                                <a href="" target="_blank" >\n                                    <img class = 'support-icons' alt="Wyoming Department of Environmental Quality icon" src="images/WY-DEQ-Logo.png" style="margin-top: 1rem;padding-right: 0.5rem;">\n                                </a>\n                            </div>\n                            <div class = 'col-lg-10'>\n                                <a href="" target="_blank">\n                                    <p class = 'support-text'>\n                                    USFS units in Regions 2 and 4 in Wyoming collaborated to help GTAC develop and train this tool based on actual bloom data collected by the Wyoming Department of Environmental Quality, Water Quality Division, Watershed Protection Program as part of their state-wide monitoring efforts to document the occurrence of Harmful Cyanobacterial Blooms. Thousands of lakes over ~1 acre exist on Forest system lands in Wyoming. This tool is critical in helping Forest staff focus efforts to address this public safety concern.</p>\n                                </a>\n                            </div>\n                        </section>\n                        \n                        <hr>\n                        <section class = 'row'>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <a href="https://earthengine.google.com/" target="_blank">\n                                    <img src="images/GEE_logo_transparent.png"  class = 'support-icons' alt="Google Earth Engine Logo"  href="#"   title="Click to learn more about Google Earth Engine">\n                                    \n                                </a>\n                            </div>\n                            <div class = 'col-lg-10'>\n                                <a href="https://earthengine.google.com/" target="_blank">\n                                    <p class = 'support-text'>${mode} utilizes Google Earth Engine for most of its data acqusition, processing, and visualization, through an enterprise agreement between the USDA Forest Service and Google. In its current form, ${mode} would not be possible without Google Earth Engine.</p>\n                                </a>\n                            </div>\n                        </section>\n                        <hr>\n                        <section class = 'row'>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <h2>"..."</h2>\n                            </div>\n                            <div class = 'col-lg-10  support-text'>\n                                    Suggested citation: \n                                    <p class = 'support-text' onclick = 'copyText("suggested-citation-text","copiedCitationMessageBox")' id = 'suggested-citation-text' title='Click to copy suggested citation to clipboard'>Forest Service, U.S. Department of Agriculture (2023). ${mode} [Online]. Available at: https://apps.fs.usda.gov/lcms-viewer/${mode}.html (Accessed: ${(new Date).toStringFormat()}).\n                                    </p>\n                                    <span>\n                                        <button onclick = 'copyText("suggested-citation-text","copiedCitationMessageBox")'' title = 'Click to copy suggested citation to clipboard' class="py-0 pr-1 fa fa-copy btn input-group-text bg-white" >\n                                        </button>\n                                        <p id = 'copiedCitationMessageBox'></p>\n                                    </span>\n                            </div>\n                        </section>\n                        <hr>\n                        <header class ='row'>\n                            <h3 class ='text-capitalize'>Contact</h3>\n                        </header>\n                        <section class = 'row '>\n                            <div class = 'col-lg-2 p-0 m-0'>\n                                <a title = "Send us an E-mail" href = "mailto: sm.fs.lcms@usda.gov"><img class = 'support-icons' alt = 'Email icon' src = './images/email.png'></a> \n                            </div>\n                            <div class = 'col-lg-10'>\n                                <a class = 'support-text' title = "Send us an E-mail" href = "mailto: sm.fs.lcms@usda.gov">\n                                Please contact the ${mode} help desk <span href = "mailto: sm.fs.lcms@usda.gov">(sm.fs.lcms@usda.gov)</span> if you have questions/comments about ${mode} or have feedback on the ${mode}.</a>\n                            </div>\n                        </section>\n        \t\t\t</div>`,
     tooltipToggle: " <label class = 'mt-2'>If you turned off tool tips, but want them back:</label>\n                        <button  class = 'btn  bg-black' onclick = 'showToolTipsAgain()'>Show tooltips</button>",
     walkThroughButton: `<div >\n                            <label class = 'mt-2'>Run a walk-through of the ${mode} Data Explorer's features</label>\n                            <a  class = 'intro-modal-links ' onclick = 'toggleWalkThroughCollapse()' title = 'Run interactive walk-through of the features of the ${mode} Data Explorer'>Run Walk-Through</a>\n                          </div>`,
     distanceDiv: "Click on map to measure distance",
     distanceTip: "Click on map to measure distance. Press <kbd>ctrl+z</kbd> to undo most recent point. Double-click, press <kbd>Delete</kbd>, or press <kbd>Backspace</kbd> to clear measurment and start over.",
     areaDiv: "Click on map to measure area<variable-radio onclick1 = 'updateArea()' onclick2 = 'updateArea()' var='metricOrImperialArea' title2='' name2='Metric' name1='Imperial' value2='metric' value1='imperial' type='string' title='Toggle between imperial or metric units'></variable-radio>\n       ",
     areaTip: "Click on map to measure area. Double-click to complete polygon, press <kbd>ctrl+z</kbd> to undo most recent point, press <kbd>Delete</kbd> or <kbd>Backspace</kbd> to start over. Any number of polygons can be defined by repeating this process.",
     queryDiv: "<div>Double-click on map to query values of displayed layers at that location</div>",
@@ -861,15 +877,15 @@
 
 function appendMessage2(e, a) {
     null == e && (e = ""), null == a && (a = "error-modal"), $("#" + a + "-body").append(e)
 }
 
 function showTip(e, a) {
     null != localStorage.showToolTipModal && "undefined" != localStorage.showToolTipModal || (localStorage.showToolTipModal = "true"), "true" === localStorage.showToolTipModal && 0 == walkThroughAdded && (showMessage("", '<span class = "font-weight-bold text-uppercase" >' + e + " </span><span>" + a + "</span>", "tip-modal", !1), $("#tip-modal-body").append('<form class="form-inline pt-3 pb-0">\n\t\t\t\t\t\t\t\t  <div class="form-check  mr-0">\n                                \t<input role="option" type="checkbox" class="form-check-input" id="dontShowTipAgainCheckbox"   name = \'dontShowAgain\' value = \'true\'>\n                                \t<label class=" text-uppercase form-check-label " for="dontShowTipAgainCheckbox" >Turn off tips</label>\n                            \t\t</div>\n\t\t\t\t\t\t\t\t</form>'), $("#tip-modal").modal().show()), $("#dontShowTipAgainCheckbox").change((function() {
-        console.log(this.checked), localStorage.showToolTipModal = !this.checked, "false" === localStorage.showToolTipModal ? $("#tooltip-radio-second_toggle_label").click() : "true" === localStorage.showToolTipModal && $("#tooltip-radio-first_toggle_label").click()
+        localStorage.showToolTipModal = !this.checked, "false" === localStorage.showToolTipModal ? $("#tooltip-radio-second_toggle_label").click() : "true" === localStorage.showToolTipModal && $("#tooltip-radio-first_toggle_label").click()
     }))
 }
 
 function addStudyAreaToDropdown(e, a) {
     var t = e.replaceAll(" ", "-");
     $("#study-area-list").append(`<a id = '${t}' name = '${e}' class="dropdown-item "   data-toggle="tooltip" title="${a}">${e}</a>`), $("#" + t).on("click", (function() {
         $("#study-area-list").hide(), longStudyAreaName = this.name, dropdownUpdateStudyArea(this.name)
@@ -1052,15 +1068,16 @@
 }
 
 function moveCollapse(e, a = getWalkThroughCollapseContainerID()) {
     $("#" + e + "-label").detach().appendTo("#" + a), $("#" + e + "-div").detach().appendTo("#" + a)
 }
 
 function addLegendCollapse() {
-    addCollapse(getWalkThroughCollapseContainerID(), "legend-collapse-label", "legend-collapse-div", "LEGEND", '<i class="fa fa-location-arrow fa-rotate-45 mx-1" aria-hidden="true"></i>', !0, "", "LEGEND of the layers displayed on the map"), addCollapse(getWalkThroughCollapseContainerID(), "chart-collapse-label", "chart-collapse-div", "QUERY OUTPUTS", '<i class="fa fa-graph fa-rotate-45 mx-1" aria-hidden="true"></i>', !0, "", "Charts go here"), $("#chart-collapse-div").append('<div role="list" id="chart-list"></div>'), $("#chart-collapse-label-chart-collapse-div").hide(), $("#chart-collapse-div").removeClass("px-5"), $("#chart-collapse-div").addClass("px-3"), $("#legend-collapse-div").append('<div role="list" id="legend-layer-list"></div>'), $("#legend-collapse-div").append('<div role="list" id="legend-reference-layer-list"></div>'), $("#legend-collapse-div").append('<div role="list" id="legend-fhp-div"></div>'), $("#legend-collapse-div").append('<div role="list" id="time-lapse-legend-list"></div>'), $("#legend-collapse-div").append('<div role="list" id="legend-area-charting-select-layer-list"></div>')
+    var e = getWalkThroughCollapseContainerID();
+    addCollapse(getWalkThroughCollapseContainerID(), "chart-collapse-label", "chart-collapse-div", "QUERY OUTPUTS", '<i class="fa fa-list  mx-0" aria-hidden="true"></i>', !0, "", "Query Visible Map Layers outputs will appear here"), addCollapse(e, "legend-collapse-label", "legend-collapse-div", "LEGEND", '<i class="fa fa-location-arrow fa-rotate-45 mx-1" aria-hidden="true"></i>', !0, "", "LEGEND of the layers displayed on the map"), $("#chart-collapse-div").append('<div role="list" id="chart-list"></div>'), $("#chart-collapse-label-chart-collapse-div").hide(), $("#chart-collapse-div").removeClass("px-5"), $("#chart-collapse-div").addClass("px-3"), $("#legend-collapse-div").append('<div role="list" id="legend-layer-list"></div>'), $("#legend-collapse-div").append('<div role="list" id="legend-reference-layer-list"></div>'), $("#legend-collapse-div").append('<div role="list" id="legend-fhp-div"></div>'), $("#legend-collapse-div").append('<div role="list" id="time-lapse-legend-list"></div>'), $("#legend-collapse-div").append('<div role="list" id="legend-area-charting-select-layer-list"></div>')
 }
 
 function addLegendContainer(e, a, t, o) {
     null == a && (a = "legend-collapse-div"), null == t && (t = !0), t = t ? "block" : "none", $("#" + a).prepend(`<div class = 'py-1 row' title= '${o}' style = 'display:${t};' id = '${e}'>\n\t\t\t\t\t\t\t\t</div>`)
 }
 
 function addClassLegendContainer(e, a, t) {
@@ -1076,15 +1093,15 @@
 }
 
 function regulateReRunButton() {
     outstandingGEERequests > 0 ? ($("#reRun-button").prop("disabled", !0), $("#reRun-button").prop("title", staticTemplates.reRunButtonDisabledTooltip)) : ($("#reRun-button").prop("disabled", !1), $("#reRun-button").prop("title", staticTemplates.reRunButtonEnabledTooltip))
 }
 
 function updateOutstandingGEERequests() {
-    $("#outstanding-gee-requests").html(outstandingGEERequests), regulateReRunButton()
+    0 === outstandingGEERequests ? $("#gee-queue-len").hide() : ($("#gee-queue-len").show(), $("#outstanding-gee-requests").html(outstandingGEERequests)), regulateReRunButton()
 }
 
 function updateGEETileLayersLoading() {
     $("#number-gee-tiles-downloading").html(geeTileLayersDownloading)
 }
 
 function incrementOutstandingGEERequests() {
@@ -1198,15 +1215,15 @@
             y()
         })))), "geeImage" === e.layerType || "geeVectorImage" === e.layerType || "geeImageCollection" === e.layerType) {
         if ("geeImageCollection" === e.layerType) {
             e.imageCollection = e.item, null !== e.viz.reducer && void 0 !== e.viz.reducer || (e.viz.reducer = ee.Reducer.lastNonNull());
             var w = ee.Image(e.item.first()).bandNames();
             e.item = ee.ImageCollection(e.item).reduce(e.viz.reducer).rename(w).copyProperties(e.imageCollection.first())
         } else if ("geeVectorImage" === e.layerType || "geeVector" === e.layerType) {
-            var C;
+            var S;
             if (e.viz.isSelectLayer && (selectedFeaturesJSON[e.name] = {
                     layerName: e.name,
                     filterList: [],
                     geoJSON: new google.maps.Data,
                     id: e.id,
                     rawGeoJSON: {},
                     selection: ee.FeatureCollection([])
@@ -1216,31 +1233,31 @@
                     y()
                 })), $(".vector-layer-checkbox").on("turnOffAll", (function() {
                     f()
                 })), $(".vector-layer-checkbox").on("turnOnAll", (function() {
                     y()
                 }))), e.queryItem = e.item, "geeVectorImage" === e.layerType && (e.item = ee.Image().paint(e.item, null, e.viz.strokeWeight), e.viz.palette = e.viz.strokeColor), e.viz.isSelectLayer)
                 if (void 0 === e.viz.selectLayerNameProperty) e.queryItem.first().propertyNames().evaluate((function(a, t) {
-                    void 0 !== t ? C = "system:index" : (a.map((function(e) {
-                        -1 !== e.toLowerCase().indexOf("name") && (C = e)
-                    })), void 0 === C && (C = "system:index")), selectedFeaturesJSON[e.name].fieldName = C, selectedFeaturesJSON[e.name].eeObject = e.queryItem.select([C], ["name"])
+                    void 0 !== t ? S = "system:index" : (a.map((function(e) {
+                        -1 !== e.toLowerCase().indexOf("name") && (S = e)
+                    })), void 0 === S && (S = "system:index")), selectedFeaturesJSON[e.name].fieldName = S, selectedFeaturesJSON[e.name].eeObject = e.queryItem.select([S], ["name"])
                 }));
                 else selectedFeaturesJSON[e.name].fieldName = e.viz.selectLayerNamePropertyname, selectedFeaturesJSON[e.name].eeObject = e.queryItem.select([e.viz.selectLayerNameProperty], ["name"]);
             e.viz.isSelectedLayer && ($("#" + s).addClass("selected-layer-checkbox"), $(".vector-layer-checkbox").on("turnOffAllSelectLayers", (function() {
                 f()
             })), $(".vector-layer-checkbox").on("turnOnAllSelectLayers", (function() {
                 y()
             })), $(".vector-layer-checkbox").on("turnOffAllSelectedLayers", (function() {
                 f()
             })), $(".vector-layer-checkbox").on("turnOnAllSelectedLayers", (function() {
                 y()
             })), selectionTracker.seletedFeatureLayerIndices.push(e.layerId))
         }
 
-        function S() {
+        function C() {
             var a = Object.values(layerObj).filter((function(a) {
                     return a.loading && a.viz.isTimeLapse && a.whichLayerList === e.whichLayerList
                 })).length,
                 t = (Object.values(layerObj).filter((function(a) {
                     return !a.loading && a.viz.isTimeLapse && a.whichLayerList === e.whichLayerList
                 })).length, 100 * (1 - a / timeLapseObj[e.viz.timeLapseID].nFrames));
             $("#" + e.viz.timeLapseID + "-collapse-label").css("background", `-webkit-linear-gradient(0deg, #FFF, #FFF ${t}%, transparent ${t}%, transparent 100%)`), t < 100 ? $("#" + e.viz.timeLapseID + "-loading-gear").show() : $("#" + e.viz.timeLapseID + "-loading-gear").hide()
@@ -1268,18 +1285,18 @@
                         if ($("#" + s).show(), e.currentGEERunID === geeRunID)
                             if (void 0 === t || void 0 !== o) h(o);
                             else {
                                 const a = t.urlFormat;
                                 e.layer = new google.maps.ImageMapType({
                                     getTileUrl: function(t, o) {
                                         let l = a.replace("{x}", t.x).replace("{y}", t.y).replace("{z}", o);
-                                        return e.loading || (e.loading = !0, e.percent = 10, $("#" + i + "2").show(), updateGEETileLayersDownloading(), u(), e.viz.isTimeLapse && S()), l
+                                        return e.loading || (e.loading = !0, e.percent = 10, $("#" + i + "2").show(), updateGEETileLayersDownloading(), u(), e.viz.isTimeLapse && C()), l
                                     }
                                 }), e.layer.addListener("tilesloaded", (function() {
-                                    e.percent = 100, e.loading = !1, $("#" + i + "2").hide(), updateGEETileLayersDownloading(), u(), e.viz.isTimeLapse && S()
+                                    e.percent = 100, e.loading = !1, $("#" + i + "2").hide(), updateGEETileLayersDownloading(), u(), e.viz.isTimeLapse && C()
                                 })), e.visible ? (e.map.overlayMapTypes.setAt(e.layerId, e.layer), e.rangeOpacity = e.opacity, e.layer.setOpacity(e.opacity), $("#" + e.legendDivID).show()) : e.rangeOpacity = 0, $("#" + i).hide(), $("#" + s).show(), p()
                             }
                     }(l, r)
                 })), e.mapServiceTryNumber++
             }()
     } else if ("geeVector" === e.layerType || "geoJSONVector" === e.layerType) {
         function L(a) {
@@ -1653,43 +1670,52 @@
                         return a.geometry = l[e].geometry, a.properties = {}, a.properties.current = l[e].properties, a.properties.future = r[e].properties, a
                     }));
                 $("#summary-spinner").slideUp(), createHurricaneDamageWrapper(ee.FeatureCollection(n))
             }, e.readAsText(jQuery("#stormTrackUpload")[0].files[0])
         } else $("#summary-spinner").hide(), showMessage("No storm track provided", 'Please download storm track from <a href="https://www.wunderground.com/hurricane" target="_blank">here</a> . Copy and paste the storm track coordinates into a text editor. Save the table. Then upload that table above.')
     }
     canExport = !0, addCollapse("sidebar-left", "parameters-collapse-label", "parameters-collapse-div", "PARAMETERS", '<i role="img" class="fa fa-sliders mr-1" aria-hidden="true"></i>', !0, null, "Adjust parameters used to prepare storm outputs"), $("#parameters-collapse-div").append('\n    <label>Download storm track from <a href="https://www.wunderground.com/hurricane" target="_blank">here</a>. Copy and paste the storm track coordinates into a text editor. Save the table. Then upload that table below. <a href="./geojson/michael.txt" download="michael.txt" >Download test data here.</a></label>\n    <input class = \'file-input my-1\' type="file" id="stormTrackUpload" name="upload"  style="display: inline-block;" title = "Download storm track from https://www.wunderground.com/hurricane">\n    <hr>\n    <label>Provide name for storm (optional):</label>\n    <input title = \'Provide a name for the storm. The name of the provided storm track file will be used if left blank.\'  type="user-selected-area-name" class="form-control" id="storm-name"  placeholder="Name your storm!" style=\'width:80%;\'><hr>'), addRangeSlider("parameters-collapse-div", "Refinement iterations", "refinementIterations", 0, 10, 5, 1, "refinement-factor-slider", "null", "Specify number of iterations to perform a linear interpolation of provided track. A higher number is needed for tracks with fewer real observations"), addRangeSlider("parameters-collapse-div", "Max distance (km)", "maxDistance", 50, 500, 200, 50, "max-distance-slider", "null", "Specify max distance in km from storm track to include in output"), addRangeSlider("parameters-collapse-div", "Min wind (mph)", "minWind", 0, 75, 30, 5, "min-wind-slider", "null", "Specify min wind speed in mph to include in output"), $("#parameters-collapse-div").append('\n        <hr>\n        <label style = \'width:90%\'>The MOD of Rupture is intended to indicate how much force it takes to snap a tree. A single value can be provided by providing a constant image (e.g. ee.Image(1)) and a simple lookup to convert that image to a desired MOD of Rupture (e.g. {1:8500}). If different MOD of Rupture values are needed for different tree types, you can provide an EE image that may have tree classes or land cover classes that can then be cross-walked to a MOD of Rupture image with different values for different tree/land cover classes (e.g. ee.Image( "USGS/NLCD_RELEASES/2016_REL/2016" ).select([ 0 ]) with a lookup of {41:8500,42:2000,43:5000,90:4000}</label>\n        <hr>\n        <label>MOD of Rupture Image</label>\n        <textarea   title = \'Provide an image with relevant land cover/tree classes. Provide a constant raster (ee.Image(1)) if you would like to use a constant\'   class="form-control" id="mod-image"   oninput="auto_grow(this)" style=\'width:90%;\'>ee.Image("USGS/NLCD_RELEASES/2016_REL/2016").select([0])</textarea>\n        <hr>\n        <label>MOD of Rupture Lookup</label>\n        <textarea   title = \'Provide a lookup table to remap each class of the image provided above with a MOD of Rupture value.\'  type="user-selected-area-name" class="form-control" id="mod-lookup" oninput="auto_grow(this)" style=\'width:90%;\'>{41:8500, 42:2000, 43:5000, 90:4000}</textarea>\n       '), $("#parameters-collapse-div").append("<hr>\n      <button class = 'btn' style = 'margin-bottom: 0.5em!important;' onclick = 'ingestStormTrack()' title = 'Click to ingest storm track and map damage'>Ingest Storm Track</button>\n      <button class = 'btn' style = 'margin-bottom: 0.5em!important;' onclick = 'reRun()' title = 'Click to remove existing layers and exports'>Clear All Layers/Exports</button><br>"), addCollapse("sidebar-left", "layer-list-collapse-label", "layer-list-collapse-div", mode + " DATA", "<img style = 'width:1.1em;' class='image-icon mr-1' alt=\"Layers icon\" src=\"images/layer_icon.png\">", !0, null, mode + " DATA layers to view on map"), $("#layer-list-collapse-div").append('<ul id="layer-list" class = "layer-list"></ul>'), addCollapse("sidebar-left", "tools-collapse-label", "tools-collapse-div", "TOOLS", '<i role="img" class="fa fa-gear mr-1" aria-hidden="true"></i>', !1, "", "Tools to measure and chart data provided on the map"), addCollapse("sidebar-left", "download-collapse-label", "download-collapse-div", "DOWNLOAD DATA", '<i role="img" class="fa fa-cloud-download mr-1" aria-hidden="true"></i>', !1, "", "Download " + mode + " products for further analysis")
-} else "TreeMap" === mode ? (addCollapse("sidebar-left", "layer-list-collapse-label", "layer-list-collapse-div", "TreeMap DATA", "<img style = 'width:1.1em;' class='image-icon mr-1' alt=\"Layers icon\" src=\"images/layer_icon.png\">", !0, null, mode + " DATA layers to view on map"), addCollapse("sidebar-left", "tools-collapse-label", "tools-collapse-div", "TOOLS", '<i role="img" class="fa fa-gear mr-1" aria-hidden="true"></i>', !1, "", "Tools to measure and chart data provided on the map"), $("#layer-list-collapse-div").append('<ul id="layer-list" class = "layer-list"></ul>')) : (addCollapse("sidebar-left", "layer-list-collapse-label", "layer-list-collapse-div", "ANCILLARY DATA", "<img style = 'width:1.1em;' class='image-icon mr-1' alt=\"Layers icon\" src=\"images/layer_icon.png\">", !0, null, mode + " DATA layers to view on map"), addCollapse("sidebar-left", "reference-layer-list-collapse-label", "reference-layer-list-collapse-div", "PLOT DATA", "<img style = 'width:1.1em;' class='image-icon mr-1' alt=\"Layers icon\" src=\"images/layer_icon.png\">", !1, null, "Additional relevant layers to view on map intended to provide context for " + mode + " DATA"), addCollapse("sidebar-left", "tools-collapse-label", "tools-collapse-div", "TOOLS", '<i role="img" class="fa fa-gear mr-1" aria-hidden="true"></i>', !1, "", "Tools to measure and chart data provided on the map"), $("#layer-list-collapse-div").append('<ul id="layer-list" class = "layer-list"></ul>'), $("#reference-layer-list-collapse-div").append('<ul id="reference-layer-list" class = "layer-list"></ul>'), plotsOn = !0);
+} else if ("TreeMap" === mode) addCollapse("sidebar-left", "layer-list-collapse-label", "layer-list-collapse-div", "TreeMap DATA", "<img style = 'width:1.1em;' class='image-icon mr-1' alt=\"Layers icon\" src=\"images/layer_icon.png\">", !0, null, mode + " DATA layers to view on map"), addCollapse("sidebar-left", "tools-collapse-label", "tools-collapse-div", "TOOLS", '<i role="img" class="fa fa-gear mr-1" aria-hidden="true"></i>', !1, "", "Tools to measure and chart data provided on the map"), $("#layer-list-collapse-div").append('<ul id="layer-list" class = "layer-list"></ul>');
+else if ("sequoia-view" === mode) {
+    addCollapse("sidebar-left", "parameters-collapse-label", "parameters-collapse-div", "PARAMETERS", '<i role="img" class="fa fa-sliders mr-1" aria-hidden="true"></i>', !0, null, "Adjust parameters used to prepare storm outputs");
+    var minYear = 2017,
+        maxYear = (new Date).getFullYear(),
+        dayOfYear = (new Date).dayofYear();
+    null != urlParams.preStartYear && null != urlParams.preStartYear || (urlParams.preStartYear = minYear), null != urlParams.preEndYear && null != urlParams.preEndYear || (urlParams.preEndYear = maxYear - 1), null != urlParams.postStartYear && null != urlParams.postStartYear || (urlParams.postStartYear = maxYear), null != urlParams.postEndYear && null != urlParams.postEndYear || (urlParams.postEndYear = maxYear), null != urlParams.startJulian && null != urlParams.startJulian || (urlParams.startJulian = dayOfYear - 16), null != urlParams.endJulian && null != urlParams.endJulian || (urlParams.endJulian = dayOfYear - 2), console.log(maxYear), addDualRangeSlider("parameters-collapse-div", "Choose start year range:", "urlParams.preStartYear", "urlParams.preEndYear", minYear, maxYear - 1, urlParams.preStartYear, urlParams.preEndYear, 1, "pre-years-slider", "null", "Years to include for the past image data"), addDualRangeSlider("parameters-collapse-div", "Choose analysis year range:", "urlParams.postStartYear", "urlParams.postEndYear", minYear, maxYear, urlParams.postStartYear, urlParams.postEndYear, 1, "post-years-slider", "null", "Years to include for the current image data"), addDualRangeSlider("parameters-collapse-div", "Choose analysis date range:", "urlParams.startJulian", "urlParams.endJulian", 1, 365, urlParams.startJulian, urlParams.endJulian, 1, "julian-day-slider", "julian", "Days of year of " + mode + " data to include for land cover, land use, loss, and gain"), addCollapse("sidebar-left", "layer-list-collapse-label", "layer-list-collapse-div", "MAP LAYERS", "<img style = 'width:1.1em;' class='image-icon mr-1' alt=\"Layers icon\" src=\"images/layer_icon.png\">", !0, null, mode + " DATA layers to view on map"), addCollapse("sidebar-left", "table-collapse-label", "table-collapse-div", "MONITORING SITES", '<img class=\'panel-title-svg-lg\'  alt="Graph icon" src="./Icons_svg/graph_ffffff.svg">', !0, "", "Giant Sequoia monitoring sites output table"), addCollapse("sidebar-left", "tools-collapse-label", "tools-collapse-div", "TOOLS", '<i role="img" class="fa fa-gear mr-1" aria-hidden="true"></i>', !1, "", "Tools to measure and chart data provided on the map"), $("#layer-list-collapse-div").append('<ul id="layer-list" class = "layer-list"></ul>'), $("#parameters-collapse-div").append(staticTemplates.reRunButton)
+} else addCollapse("sidebar-left", "layer-list-collapse-label", "layer-list-collapse-div", "ANCILLARY DATA", "<img style = 'width:1.1em;' class='image-icon mr-1' alt=\"Layers icon\" src=\"images/layer_icon.png\">", !0, null, mode + " DATA layers to view on map"), addCollapse("sidebar-left", "reference-layer-list-collapse-label", "reference-layer-list-collapse-div", "PLOT DATA", "<img style = 'width:1.1em;' class='image-icon mr-1' alt=\"Layers icon\" src=\"images/layer_icon.png\">", !1, null, "Additional relevant layers to view on map intended to provide context for " + mode + " DATA"), addCollapse("sidebar-left", "tools-collapse-label", "tools-collapse-div", "TOOLS", '<i role="img" class="fa fa-gear mr-1" aria-hidden="true"></i>', !1, "", "Tools to measure and chart data provided on the map"), $("#layer-list-collapse-div").append('<ul id="layer-list" class = "layer-list"></ul>'), $("#reference-layer-list-collapse-div").append('<ul id="reference-layer-list" class = "layer-list"></ul>'), plotsOn = !0;
 if ($("body").append("<div class = 'legendDiv flexcroll col-sm-5 col-md-3 col-lg-3 col-xl-2 p-0 m-0' id = 'legendDiv'></div>"), $(".legendDiv").css("bottom", $(".bottombar").height()), $(".sidebar").css("max-height", $("body").height() - $(".bottombar").height()), addLegendCollapse(), addAccordianContainer("tools-collapse-div", "tools-accordian"), $("#tools-accordian").append("<h5 class = 'pt-2' style = 'border-top: 0.0em solid black;'>Measuring Tools</h5>"), addSubAccordianCard("tools-accordian", "measure-distance-label", "measure-distance-div", "Distance Measuring", staticTemplates.distanceDiv, !1, "toggleTool(toolFunctions.measuring.distance)", staticTemplates.distanceTipHover), addSubAccordianCard("tools-accordian", "measure-area-label", "measure-area-div", "Area Measuring", staticTemplates.areaDiv, !1, "toggleTool(toolFunctions.measuring.area)", staticTemplates.areaTipHover), addRadio("measure-distance-div", "metricOrImperialDistance-radio", "", "Imperial", "Metric", "metricOrImperialDistance", "imperial", "metric", "updateDistance()", "updateDistance()", "Toggle between imperial or metric units"), addRadio("measure-area-div", "metricOrImperialArea-radio", "", "Imperial", "Metric", "metricOrImperialArea", "imperial", "metric", "updateArea()", "updateArea()", "Toggle between imperial or metric units"), addShapeEditToolbar("measure-distance-div", "measure-distance-div-icon-bar", "undoDistanceMeasuring()", "resetPolyline()"), addColorPicker("measure-distance-div-icon-bar", "distance-color-picker", "updateDistanceColor", distancePolylineOptions.strokeColor), addShapeEditToolbar("measure-area-div", "measure-area-div-icon-bar", "undoAreaMeasuring()", "resetPolys()"), addColorPicker("measure-area-div-icon-bar", "area-color-picker", "updateAreaColor", areaPolygonOptions.strokeColor), $("#tools-accordian").append("<h5 class = 'pt-2' style = 'border-top: 0.1em solid black;'>Pixel Tools</h5>"), addSubAccordianCard("tools-accordian", "query-label", "query-div", "Query Visible Map Layers", staticTemplates.queryDiv, !1, "toggleTool(toolFunctions.pixel.query)", staticTemplates.queryTipHover), -1 === ["Bloom-Mapper", "TreeMap"].indexOf(mode) && (addSubAccordianCard("tools-accordian", "pixel-chart-label", "pixel-chart-div", "Query " + mode + " Time Series", staticTemplates.pixelChartDiv, !1, "toggleTool(toolFunctions.pixel.chart)", staticTemplates.pixelChartTipHover), addDropdown("pixel-chart-div", "pixel-collection-dropdown", "Choose which " + mode + " time series to chart", "whichPixelChartCollection", "Choose which " + mode + " time series to chart.")), "geeViz" === mode) {
     $("#pixel-chart-label").remove(), $("#share-button").remove(), $("#tools-accordian").append("<hr>");
     var tShowToolTipModal = !0;
     null !== localStorage.showToolTipModal && void 0 !== localStorage.showToolTipModal && (tShowToolTipModal = localStorage.showToolTipModal), addRadio("tools-accordian", "tooltip-radio", "Show tool tips", "Yes", "No", "localStorage.showToolTipModal", "true", "false", "", "", "Whether to show tool tips to help explain how to use the tools."), "false" === tShowToolTipModal && $("#tooltip-radio-second_toggle_label").click()
 }
 if ("LAMDA" === mode && $("#pixel-chart-label").remove(), "LCMS-pilot" === mode || "MTBS" === mode || "lcms-base-learner" === mode || "IDS" === mode || "LCMS" === mode) {
     if ($("#tools-accordian").append("<h5 class = 'pt-2' style = 'border-top: 0.1em solid black;'>Area Tools</h5>"), addSubCollapse("tools-accordian", "area-chart-params-label", "area-chart-params-div", "Area Tools Parameters", "", !1, ""), $("#area-chart-params-label").prop("title", "Click here to select which LCMS products to chart, and change which area units are used. "), addDropdown("area-chart-params-div", "area-collection-dropdown", "Choose which " + mode + " product to summarize", "whichAreaChartCollection", "Choose which " + mode + " time series to summarize."), $("#parameters-collapse-div").append("<hr>"), addMultiRadio("area-chart-params-div", "area-summary-format", "Area Units", "areaChartFormat", {
             Percentage: !0,
             Acres: !1,
             Hectares: !1
-        }), "LCMS" === mode && ("true" === urlParams.sankey || "true" === urlParams.beta)) {
+        }), "LCMS" === mode) {
         var activeStartYear = urlParams.startYear,
             activeEndYear = urlParams.endYear;
-        $("#area-chart-params-div").append("<div id='transition-periods-container'></div>")
+        $("#area-chart-params-div").append("<div id='transition-periods-container'></div>"), $("#transition-periods-container").hide(), $("#area-collection-dropdown").change((e => {
+            $("#area-collection-dropdown").val().indexOf("-transition") > -1 ? $("#transition-periods-container").show() : $("#transition-periods-container").hide()
+        }))
     }
     $("#area-summary-format").prop("title", "Choose how to summarize area- as a percentage of the area, acres, or hectares."), addSubAccordianCard("tools-accordian", "user-defined-area-chart-label", "user-defined-area-chart-div", "User-Defined Area", staticTemplates.userDefinedAreaChartDiv, !1, "toggleTool(toolFunctions.area.userDefined)", staticTemplates.userDefinedAreaChartTipHover), addSubAccordianCard("tools-accordian", "upload-area-chart-label", "upload-area-chart-div", "Upload an Area", staticTemplates.uploadAreaChartDiv, !1, "toggleTool(toolFunctions.area.shpDefined)", staticTemplates.uploadAreaChartTipHover), addSubAccordianCard("tools-accordian", "select-area-interactive-chart-label", "select-area-interactive-chart-div", "Select an Area on Map", staticTemplates.selectAreaInteractiveChartDiv, !1, "toggleTool(toolFunctions.area.selectInteractive)", staticTemplates.selectAreaInteractiveChartTipHover), addRangeSlider("upload-reduction-factor-container", "Vertex Reduction Factor", "uploadReductionFactor", 1, 5, 1, 1, "upload-reduction-factor-slider", "null", "Every n vertex in uploaded file will be kept for polygons > 100 vertices (E.g. if 3 is chosen, every third vertex remains). This is intended to help enable use of uploaded areas that may have failed due to its size."), addRangeSlider("simplify-error-range-container", "Simplify Area - Max Error", "simplifyMaxError", 0, 500, 0, 50, "simplify-error-slider", "null", "If the selected area is very large and/or has a lot of vertices, it may not compute. In this instance, clear out any existing selections (trash can button below), and increase this value. The selected polygon will be simplified using a max error in meters equal to this value upon selection. Generally between 50 and 150 will get most areas to work."), addShapeEditToolbar("user-defined-edit-toolbar", "user-defined-area-icon-bar", "undoUserDefinedAreaCharting()", "restartUserDefinedAreaCarting()"), addColorPicker("user-defined-area-icon-bar", "user-defined-color-picker", "updateUDPColor", udpOptions.strokeColor), addShapeEditToolbar("select-features-edit-toolbar", "select-area-interactive-chart-icon-bar", "removeLastSelectArea()", "clearSelectedAreas()", "Click to unselect most recently selected polyogn", "Click to clear all selected polygons"), $("#tools-accordian").append("<hr>");
     var tShowToolTipModal = !0;
     null !== localStorage.showToolTipModal && void 0 !== localStorage.showToolTipModal && (tShowToolTipModal = localStorage.showToolTipModal), addRadio("tools-accordian", "tooltip-radio", "Show tool tips", "Yes", "No", "localStorage.showToolTipModal", "true", "false", "", "", "Whether to show tool tips to help explain how to use the tools."), "false" === tShowToolTipModal && $("#tooltip-radio-second_toggle_label").click()
 }
 if ("MTBS" !== mode && "Ancillary" !== mode || ($("#contributor-logos").prepend('<a href="https://www.usgs.gov/" target="_blank" >\n                                    <img src="images/usgslogo.png" class = \'image-icon-bar\' alt="USGS logo" title="Click to learn more about the US Geological Survey">\n                                  </a>'), $("#contributor-logos").prepend('<a href="https://www.mtbs.gov/" target="_blank" >\n                                    <img src="images/mtbs-logo-large.png" class = \'image-icon-bar\' alt="MTBS logo" title="Click to learn more about MTBS">\n                                  </a>')), canExport) {
     function cacheCRS() {
         localStorage.export_crs = $("#export-crs").val()
     }
     $("#download-collapse-div").append(staticTemplates.exportContainer), void 0 !== localStorage.export_crs && null !== localStorage.export_crs && localStorage.export_crs.indexOf("EPSG") > -1 ? $("#export-crs").val(localStorage.export_crs) : localStorage.export_crs = $("#export-crs").val(), "STORM" === mode && ($("#export-area-drawing-div").append("<hr>\n                                            <button class = 'btn' onclick = 'addTrackBounds()' title = 'Add bounds of storm track for export area.'><i class=\"pr-1 fa fa-square-o\" aria-hidden=\"true\"></i> Use storm track bound as area to download</button>\n                                            "), $("#export-button-div").append("<hr>"), addRangeSlider("export-button-div", "Quick look spatial resolution", "quickLookRes", 1200, 6e3, 3e3, 300, "quick-look-res-slider", "null", "Specify spatial resolution for quick look downloads."), $("#export-button-div").append("<button class = 'btn' onclick = 'downloadQuickLooks()'  title = 'Quickly download outputs at coarse resolution'><i class=\"pr-1 fa fa-cloud-download\" aria-hidden=\"true\"></i>Download Quick Look Outputs</button>\n                                            "))
 }
 
 function resizeViewerPanes() {
-    "lcms-dashboard" !== mode && (moveCollapse("legend-collapse"), moveCollapse("chart-collapse")), $(".legendDiv").css("bottom", $(".bottombar").height()), $(".legendDiv").css("max-height", window.innerHeight - $(".bottombar").height()), $(".sidebar").css("max-height", $("body").height() - $(".bottombar").height()), walkThroughAdded && moveCollapse("walk-through-collapse")
+    "lcms-dashboard" !== mode && (moveCollapse("chart-collapse"), moveCollapse("legend-collapse")), $(".legendDiv").css("bottom", $(".bottombar").height()), $(".legendDiv").css("max-height", window.innerHeight - $(".bottombar").height()), $(".sidebar").css("max-height", $("body").height() - $(".bottombar").height()), walkThroughAdded && moveCollapse("walk-through-collapse")
 }
 
 function resizeDashboardPanes() {
     let e = $("#layer-list-collapse-label-layer-list-collapse-div").width(),
         a = $(".bottombar").height(),
         t = $("#dashboard-results-container").height(),
         o = $("#sidebar-left-container").height(),
@@ -2111,15 +2137,15 @@
 
 function addTimeLapseToMap(e, a, t, o, l, r, n, s, i) {
     null != a && null !== a.serialized && void 0 !== a.serialized && !0 === a.serialized && (e = ee.Deserializer.decode(e), a.serialized = !1), null !== a.cumulativeMode && void 0 !== a.cumulativeMode || (a.cumulativeMode = !1);
     o = !1;
     void 0 !== a.opacity && null !== a.opacity || (a.opacity = 1), e = ee.ImageCollection(e);
     var d = "";
     var c = t.replaceAll(" ", "-") + "-" + NEXT_LAYER_ID.toString();
-    c = (c = (c = c.replaceAll("/", "-")).replaceAll("(", "-")).replaceAll(")", "-"), a.autoViz && (dicts = getLookupDicts(ee.Image(e.first()), null, "eeImage"), a.classLegendDict = dicts.classLegendDict, a.queryDict = dicts.queryDict, a.autoViz = !1), a.canQuery = !1, a.isSelectLayer = !1, a.isTimeLapse = !0, a.timeLapseID = c, a.layerType = "geeImage", null !== a.dateFormat && void 0 !== a.dateFormat || (a.dateFormat = "YYYY", a.advanceInterval = "year"), null !== a.dateField && void 0 !== a.dateField || (a.dateField = "system:time_start"), timeLapseObj[c] = {}, null == s && (s = "layer-list"), null !== a.years && void 0 !== a.years || (console.log("start computing years"), a.years = unique(e.sort(a.dateField, !0).toList(1e4, 0).map((function(e) {
+    c = c.replace(/[^A-Za-z0-9]/g, "-"), a.autoViz && (dicts = getLookupDicts(ee.Image(e.first()), null, "eeImage"), a.classLegendDict = dicts.classLegendDict, a.queryDict = dicts.queryDict, a.autoViz = !1), a.canQuery = !1, a.isSelectLayer = !1, a.isTimeLapse = !0, a.timeLapseID = c, a.layerType = "geeImage", null !== a.dateFormat && void 0 !== a.dateFormat || (a.dateFormat = "YYYY", a.advanceInterval = "year"), null !== a.dateField && void 0 !== a.dateField || (a.dateField = "system:time_start"), timeLapseObj[c] = {}, null == s && (s = "layer-list"), null !== a.years && void 0 !== a.years || (console.log("start computing years"), a.years = unique(e.sort(a.dateField, !0).toList(1e4, 0).map((function(e) {
         var t = ee.Date(ee.Image(e).get(a.dateField));
         return ee.Number.parse(t.format(a.dateFormat)).int32()
     })).getInfo()), console.log("done computing years"), console.log(a.years));
     var p = a.years[0],
         u = a.years[a.years.length - 1];
     timeLapseObj[c].years = a.years, timeLapseObj[c].frames = ee.List.sequence(0, a.years.length - 1).getInfo(), timeLapseObj[c].nFrames = a.years.length, timeLapseObj[c].loadingLayerIDs = [], timeLapseObj[c].loadingTilesLayerIDs = [], timeLapseObj[c].layerVisibleIDs = [], timeLapseObj[c].sliders = [], timeLapseObj[c].intervalValue = null, timeLapseObj[c].isReady = !1, timeLapseObj[c].visible = o, timeLapseObj[c].state = "inactive", timeLapseObj[c].opacity = 100 * a.opacity, queryObj[c] = {
         visible: timeLapseObj[c].visible,
@@ -2191,15 +2217,15 @@
 function addExport(e, a, t, o, l, r) {
     var n = {};
     null == l && (l = {}), null == o && (o = !0), null == r && (r = -32768);
     var s = "";
     o && (s = "checked");
     var i = Date().split(" ");
     i[2], i[1], i[3], i[4];
-    a = (a = (a = a.replace(/\s+/g, "_")).replaceAll("(", "_")).replaceAll(")", "_"), n.res = t, n.name = a, n.eeImage = e, n.Export = o, n.ID = exportID, exportImageDict[exportID] = {
+    a = a.replace(/[^A-Za-z0-9]/g, "_"), n.res = t, n.name = a, n.eeImage = e, n.Export = o, n.ID = exportID, exportImageDict[exportID] = {
         eeImage: e,
         name: a,
         res: t,
         shouldExport: o,
         metadataParams: l,
         noDataValue: r
     }, $("#export-list").append(`<div class = 'input-group'>\n                              <span  class="input-group-addon">\n                                <input  id = '${a}-checkbox-${exportID}' type="checkbox" ${s} >\n                                <label  style = 'margin-bottom:0px;'  for='${a}-checkbox-${exportID}'></label>\n                              </span>\n                              \n                              <input  id = '${a}-name-${exportID}' class="form-control export-name-input" type="text" value="${n.name}" title = 'Change export name if needed'>\n                            </div>`), $("#" + a + "-name-" + exportID.toString()).on("input", (function() {
@@ -2230,17 +2256,17 @@
     var d = geeRunID;
     if (null == s && (s = "layer-list"), null == a && (a = {}), null == t && (t = "Layer " + NEXT_LAYER_ID), null === a.layerType || void 0 === a.layerType) {
         var c = ee.Algorithms.ObjectType(e).getInfo();
         "Feature" === c && (e = ee.FeatureCollection([e]), c = ee.Algorithms.ObjectType(e).getInfo()), a.layerType = typeLookup[c]
     }
     "geoJSONVector" === a.layerType && (a.canQuery = !1), "geeVector" === a.layerType || "geoJSONVector" === a.layerType ? (void 0 !== a.strokeOpacity && null !== a.strokeOpacity || (a.strokeOpacity = 1), void 0 !== a.fillOpacity && null !== a.fillOpacity || (a.fillOpacity = .2), void 0 !== a.fillColor && null !== a.fillColor || (a.fillColor = "222222"), void 0 !== a.strokeColor && null !== a.strokeColor || (a.strokeColor = getColor()), void 0 !== a.strokeWeight && null !== a.strokeWeight || (a.strokeWeight = 3), a.opacityRatio = a.strokeOpacity / a.fillOpacity, -1 == a.fillColor.indexOf("#") && (a.fillColor = "#" + a.fillColor), -1 == a.strokeColor.indexOf("#") && (a.strokeColor = "#" + a.strokeColor), void 0 !== a.addToClassLegend && null !== a.addToClassLegend || (a.addToClassLegend = !0)) : "geeVectorImage" === a.layerType && (void 0 !== a.strokeOpacity && null !== a.strokeOpacity || (a.strokeOpacity = 1), a.fillOpacity = 0, void 0 !== a.fillColor && null !== a.fillColor || (a.fillColor = "222222"), void 0 !== a.strokeColor && null !== a.strokeColor || (a.strokeColor = getColor()), void 0 !== a.strokeWeight && null !== a.strokeWeight || (a.strokeWeight = 2), -1 == a.fillColor.indexOf("#") && (a.fillColor = "#" + a.fillColor), -1 == a.strokeColor.indexOf("#") && (a.strokeColor = "#" + a.strokeColor), void 0 !== a.addToClassLegend && null !== a.addToClassLegend || (a.addToClassLegend = !0, a.addToLegend = !1));
     var p = t.replaceAll(" ", "-") + "-" + NEXT_LAYER_ID.toString();
-    p = (p = (p = (p = (p = (p = p.replaceAll("/", "-")).replaceAll("(", "-")).replaceAll(")", "-")).replaceAll("&", "-")).replaceAll(",", "-")).replaceAll(".", "-"), null == o && (o = !0), null == a.opacity && (a.opacity = 1), -1 != Object.keys(layerObj).indexOf(p) && (o = layerObj[p].visible, a.opacity = layerObj[p].opacity, "geeVector" !== a.layerType && "geoJSONVector" !== a.layerType || (a.strokeOpacity = layerObj[p].opacity, a.fillOpacity = a.strokeOpacity / a.opacityRatio)), null != n && void 0 !== n || (n = ""), null !== a.title && void 0 !== a.title && (n = a.title);
+    p = p.replace(/[^A-Za-z0-9]/g, "-"), null == o && (o = !0), null == a.opacity && (a.opacity = 1), -1 != Object.keys(layerObj).indexOf(p) && (o = layerObj[p].visible, a.opacity = layerObj[p].opacity, "geeVector" !== a.layerType && "geoJSONVector" !== a.layerType || (a.strokeOpacity = layerObj[p].opacity, a.fillOpacity = a.strokeOpacity / a.opacityRatio)), null != n && void 0 !== n || (n = ""), null !== a.title && void 0 !== a.title && (n = a.title);
     var u = {};
-    if (u.ID = NEXT_LAYER_ID, NEXT_LAYER_ID += 1, u.layerChildID = layerChildID, layerChildID++, u.name = t, u.opacity = a.opacity, a.opacity = 1, u.map = map, u.helpBoxMessage = n, u.visible = o, u.label = l, u.fontColor = r, u.helpBox = n, u.legendDivID = p, null == i && (i = e), null !== a.canQuery && void 0 !== a.canQuery || (a.canQuery = !0), u.canQuery = a.canQuery, u.queryItem = i, u.layerType = a.layerType, a.autoViz && (dicts = getLookupDicts(e, null, a.layerType), a.classLegendDict = dicts.classLegendDict, a.queryDict = dicts.queryDict), null == a || null != a.bands || 0 == a.addToLegend || void 0 !== a.addToClassLegend && null !== a.addToClassLegend && !1 !== a.addToClassLegend || null != a.classLegendDict && null != a.classLegendDict) {
+    if (u.ID = NEXT_LAYER_ID, NEXT_LAYER_ID += 1, u.layerChildID = layerChildID, layerChildID++, u.name = t, u.opacity = a.opacity, a.opacity = 1, u.map = map, u.helpBoxMessage = n, u.visible = o, u.label = l, u.fontColor = r, u.helpBox = n, u.legendDivID = p, null == i && (i = e), null !== a.canQuery && void 0 !== a.canQuery || (a.canQuery = !0), u.canQuery = a.canQuery, u.queryItem = i, u.layerType = a.layerType, a.autoViz && (dicts = getLookupDicts(e, null, a.layerType), a.classLegendDict = dicts.classLegendDict, a.queryDict = dicts.queryDict), null == a || null != a.bands && 1 != a.bands.split(",").length || 0 == a.addToLegend || void 0 !== a.addToClassLegend && null !== a.addToClassLegend && !1 !== a.addToClassLegend || null != a.classLegendDict && null != a.classLegendDict) {
         if (null != a && (void 0 !== a.classLegendDict && null !== a.classLegendDict || !0 === a.addToClassLegend)) {
             addLegendContainer(p, "legend-" + s, !1, n);
             var m, h = p + "-class-container";
             if (m = null !== a.legendTitle && void 0 !== a.legendTitle ? a.legendTitle : t, addClassLegendContainer(h, p, m), "geeVector" !== a.layerType && "geoJSONVector" !== a.layerType && "geeVectorImage" !== a.layerType) {
                 Object.keys(a.classLegendDict).map((function(e) {
                     var o = {};
                     o.name = t, o.helpBoxMessage = n, o.classColor = a.classLegendDict[e], o.classStrokeColor = "999", o.classStrokeWeight = 1, o.className = e, addClassLegendEntry(h, o)
@@ -2263,16 +2289,16 @@
         var y = {};
         if (null !== a.legendTitle && void 0 !== a.legendTitle ? y.name = a.legendTitle : y.name = t, y.helpBoxMessage = n, null != a.palette) var b = a.palette;
         else b = "000,FFF";
         var w = b;
         "string" == typeof b && (w = w.split(",")), 1 == w.length && (w = [w[0], w[0]]), w = w.map((function(e) {
             return e.indexOf("#") > -1 && (e = e.slice(1)), e
         }));
-        var C = createColorRamp("colorRamp" + colorRampIndex.toString(), w, 180, 20);
-        y.colorRamp = C;
+        var S = createColorRamp("colorRamp" + colorRampIndex.toString(), w, 180, 20);
+        y.colorRamp = S;
         let e = a.min,
             o = a.max;
         a.legendNumbersWithCommas && (e = e.numberWithCommas(), o = o.numberWithCommas()), null != l && null != a.min ? y.min = e + " " + l : null != l && null == a.min ? y.min = minLabel : null == l && null != a.min && (y.min = e), null != l && null != a.max ? y.max = o + " " + l : null != l && null == a.max ? y.max = maxLabel : null == l && null != a.max && (y.max = o), null !== a.legendLabelLeft && void 0 !== a.legendLabelLeft && (y.min = a.legendLabelLeft + " " + e), null !== a.legendLabelRight && void 0 !== a.legendLabelRight && (y.max = a.legendLabelRight + " " + o), null !== a.legendLabelLeftAfter && void 0 !== a.legendLabelLeftAfter && (y.min = e + " " + a.legendLabelLeftAfter), null !== a.legendLabelRightAfter && void 0 !== a.legendLabelRightAfter && (y.max = o + " " + a.legendLabelRightAfter), null == y.min && (y.min = "min"), null == y.max && (y.max = "max"), y.fontColor = null != r ? "color:#" + r + ";" : "color:#DDD;", addColorRampLegendEntry(p, y)
     }
     u.visible = o, u.item = e, u.name = t, u.viz = a, u.whichLayerList = s, u.layerId = layerCount, u.currentGEERunID = d, addLayer(u), layerCount++
 }
 
@@ -2373,15 +2399,15 @@
         tileURLFunction = function(e, t) {
             return a + t + "/" + e.x + "/" + e.y
         }, addToMap(tileURLFunction, {
             layerType: "tileMapService"
         }, t, o)
     }));
     var s = t.replaceAll(" ", "-") + "-" + NEXT_LAYER_ID.toString();
-    s = (s = (s = (s = (s = (s = s.replaceAll("/", "-")).replaceAll("(", "-")).replaceAll(")", "-")).replaceAll("&", "-")).replaceAll(",", "-")).replaceAll(".", "-"), NEXT_LAYER_ID++, featureViewObj[s] = {
+    s = s.replace(/[^A-Za-z0-9]/g, "-"), NEXT_LAYER_ID++, featureViewObj[s] = {
         name: t,
         assetId: e
     }
 }
 
 function mp() {
     this.addLayer = function(e, a, t, o, l, r, n, s, i) {
@@ -2430,26 +2456,26 @@
 }
 
 function setGEERunID() {
     geeRunID = (new Date).getTime()
 }
 
 function reRun() {
-    void 0 === staticTemplates.loadingModal[mode] ? "MTBS" === mode ? showMessage("", staticTemplates.loadingModal.all("mtbs-logo.png", "Updating")) : "STORM" === mode || "Bloom-Mapper" === mode ? showMessage("", staticTemplates.loadingModal.all("", "Updating")) : showMessage("", staticTemplates.loadingModal.all("lcms-icon.png", "Updating")) : showMessage("Loading Updated Layers", staticTemplates.loadingModal[mode]), setGEERunID(), clearSelectedAreas(), clearUploadedAreas(), layerChildID = 0, geeTileLayersDownloading = 0, updateGEETileLayersLoading(), stopTimeLapse(), queryObj = {}, areaChartCollections = {}, pixelChartCollections = {}, timeLapseObj = {}, dashboardObj = {}, intervalPeriod = 666.6666666, timeLapseID = null, timeLapseFrame = 0, cumulativeMode = !1, NEXT_LAYER_ID = 1, clearSelectedAreas(), selectedFeaturesGeoJSON = {}, ["layer-list", "reference-layer-list", "area-charting-select-layer-list", "fhp-div", "time-lapse-legend-list"].map((function(e) {
+    void 0 === staticTemplates.loadingModal[mode] ? "MTBS" === mode ? showMessage("", staticTemplates.loadingModal.all("mtbs-logo.png", "Updating")) : "STORM" === mode || "Bloom-Mapper" === mode || "sequoia-view" === mode ? showMessage("", staticTemplates.loadingModal.all("", "Updating")) : showMessage("", staticTemplates.loadingModal.all("lcms-icon.png", "Updating")) : showMessage("Loading Updated Layers", staticTemplates.loadingModal[mode]), setGEERunID(), clearSelectedAreas(), clearUploadedAreas(), layerChildID = 0, geeTileLayersDownloading = 0, updateGEETileLayersLoading(), stopTimeLapse(), queryObj = {}, areaChartCollections = {}, pixelChartCollections = {}, timeLapseObj = {}, dashboardObj = {}, intervalPeriod = 666.6666666, timeLapseID = null, timeLapseFrame = 0, cumulativeMode = !1, NEXT_LAYER_ID = 1, clearSelectedAreas(), selectedFeaturesGeoJSON = {}, ["layer-list", "reference-layer-list", "area-charting-select-layer-list", "fhp-div", "time-lapse-legend-list"].map((function(e) {
         $("#" + e).empty(), $("#legend-" + e).empty()
     })), $("#export-list").empty(), Object.values(featureObj).map((function(e) {
         e.setMap(null)
     })), featureObj = {}, map.overlayMapTypes.getArray().forEach((function(e, a) {
         map.overlayMapTypes.setAt(a, null)
     })), refreshNumber++, exportImageDict = {};
     try {
         clearDownloadDropdown()
     } catch (e) {}
     google.maps.event.clearListeners(mapDiv, "click"), setTimeout((function() {
-        run(), "lcms-dashboard" !== mode && ($(".modal").modal("hide"), $(".modal-backdrop").remove()), setupAreaLayerSelection(), addLabelOverlay(), ("true" === urlParams.sankey || "true" === urlParams.beta) && urlParams.endYear - urlParams.startYear < 5 && showMessage("No Transition Charting", "The year range must be 5 years or more to perform transition charting")
+        run(), "lcms-dashboard" !== mode && ($(".modal").modal("hide"), $(".modal-backdrop").remove()), setupAreaLayerSelection(), addLabelOverlay(), urlParams.endYear - urlParams.startYear < 5 && "LCMS" === mode && showMessage("No Transition Charting", "The year range must be 5 years or more to perform transition charting")
     }), 1500)
 }
 
 function mulberry32(e) {
     return function() {
         var a = e += 1831565813;
         return a = Math.imul(a ^ a >>> 15, 1 | a), (((a ^= a + Math.imul(a ^ a >>> 7, 61 | a)) ^ a >>> 14) >>> 0) / 4294967296
@@ -2733,15 +2759,15 @@
         }
     }, e
 }
 
 function dropdownUpdateStudyArea(e) {
     $("#summary-spinner").show(), resetStudyArea(e);
     var a = studyAreaDict[e].center;
-    centerMap(a[1], a[0], a[2]), "Ancillary" === mode ? run = runAncillary : "LT" === mode ? run = runLT : "LCMS" === mode || "LCMS-pilot" === mode && 0 == studyAreaDict[longStudyAreaName].isPilot ? (run = runGTAC, run = function() {}) : "LCMS-pilot" === mode ? run = runUSFS : "STORM" === mode ? run = runStorm : "LAMDA" === mode ? run = runLAMDA : "TreeMap" === mode ? run = runTreeMap : "lcms-base-learner" === mode ? run = runBaseLearner : run = "CONUS" === studyAreaName ? runCONUS : runUSFS, reRun()
+    centerMap(a[1], a[0], a[2]), "Ancillary" === mode ? run = runAncillary : "LT" === mode ? run = runLT : "LCMS" === mode || "LCMS-pilot" === mode && 0 == studyAreaDict[longStudyAreaName].isPilot ? (run = runGTAC, run = function() {}) : "LCMS-pilot" === mode ? run = runUSFS : "STORM" === mode ? run = runStorm : "LAMDA" === mode ? run = runLAMDA : "TreeMap" === mode ? run = runTreeMap : "lcms-base-learner" === mode ? run = runBaseLearner : "sequoia-view" === mode ? run = runSequoia : run = "CONUS" === studyAreaName ? runCONUS : runUSFS, reRun()
 }
 updateDistance = function() {
     distance = google.maps.geometry.spherical.computeLength(distancePolyline.getPath());
     distancePolyline.getPath().j;
     clickCoords = clickLngLat;
     var e = unitNameDict[metricOrImperialDistance].distance,
         a = unitMultiplierDict[metricOrImperialDistance].distance;
@@ -2904,15 +2930,15 @@
     "undefined" != typeof Storage && (cachedStudyAreaName = localStorage.getItem("cachedStudyAreaName"), null !== urlParams.studyAreaName && void 0 !== urlParams.studyAreaName ? cachedStudyAreaName = decodeURIComponent(urlParams.studyAreaName) : null == cachedStudyAreaName && (cachedStudyAreaName = defaultStudyArea), studyAreaName = studyAreaDict[cachedStudyAreaName].name, longStudyAreaName = cachedStudyAreaName, $("#study-area-label").text(longStudyAreaName), $("#study-area-label").fitText(1.8), 1 == studyAreaSpecificPage && (cachedSettingskey = studyAreaName + "-settings"), o = JSON.parse(localStorage.getItem(cachedSettingskey)), layerObj = null), null != o && null != o.center && null != o.zoom && (a = o.center, t = o.zoom), null === layerObj && (layerObj = {}), void 0 !== urlParams.lng && null !== urlParams.lng && void 0 !== urlParams.lat && null !== urlParams.lat ? (print("Setting center from URL"), e.center = {
         lng: parseFloat(urlParams.lng),
         lat: parseFloat(urlParams.lat)
     }) : e.center = a, void 0 !== urlParams.zoom && null !== urlParams.zoom ? (print("Setting zoom from URL"), e.zoom = parseInt(urlParams.zoom)) : e.zoom = t, urlParams.lng = e.center.lng, urlParams.lat = e.center.lat, urlParams.zoom = e.zoom, map = new google.maps.Map(document.getElementById("map"), e);
     var l = map.getStreetView();
 
     function r(e, a, t, o) {
-        $(".legendDiv").css("bottom", $(".bottombar").height()), $("#current-mouse-position").html("Lng: " + e + ", Lat: " + a + ", " + o + "Zoom: " + t + ", 1:" + zoomDict[t])
+        $(".legendDiv").css("bottom", $(".bottombar").height()), $("#current-mouse-position").html("Lng: " + e + ", Lat: " + a + ", " + o + " Zoom: " + t + ", 1:" + zoomDict[t])
     }
     google.maps.event.addListener(l, "visible_changed", (function() {
         l.getVisible() ? (console.log("street view in use"), $("#sidebar-left-container").hide(), $(".sidebar-toggler").hide(), $("#legendDiv").hide(), $("#bottombar").hide(), $("#dashboard-results-container").hide(), $("#dashboard-highlights-container").hide()) : (console.log("street view not in use"), $("#sidebar-left-container").show(), $(".sidebar-toggler").show(), $("#legendDiv").show(), $("#bottombar").show(), $("#dashboard-results-container").show(), $("#dashboard-highlights-container").show())
     })), marker = new google.maps.Circle({
         center: {
             lat: 45,
             lng: -111
@@ -2926,27 +2952,27 @@
 
     function i(e) {
         mouseLat = e.lat().toFixed(4).toString(), mouseLng = e.lng().toFixed(4).toString();
         try {
             ee.Image("USGS/SRTMGL1_003").reduceRegion(ee.Reducer.first(), ee.Geometry.Point([e.lng(), e.lat()])).get("elevation").evaluate((function(e) {
                 if (null !== e) {
                     var a = parseInt(3.28084 * e);
-                    n = "Elevation: " + e.toString() + "(m)," + a.toString() + "(ft),"
+                    n = "Elevation: " + e.toString() + "(m), " + a.toString() + "(ft),"
                 } else {
                     a = "NA";
                     n = "Elevation: NA,"
                 }
                 r(mouseLng, mouseLat, t, n)
             }))
         } catch (e) {
             r(mouseLng, mouseLat, t, n = "Elevation: NA,")
         }
     }
-    google.maps.event.addListener(mapDiv, "mousemove", (function(e) {
-        var a = point2LatLng(e.clientX, e.clientY);
+    map.addListener("mousemove", (function(e) {
+        var a = e.latLng;
         if (null !== a) {
             var t = map.getZoom();
             mouseLat = a.lat().toFixed(4).toString(), mouseLng = a.lng().toFixed(4).toString();
             var o = (new Date).getTime();
             o - s > 1e3 ? (i(a), s = o) : r(mouseLng, mouseLat, t, n)
         }
     })), google.maps.event.addListener(map, "maptypeid_changed", (function() {
@@ -2970,15 +2996,15 @@
                 lat: o,
                 lng: a
             },
             zoom: t
         })), updateViewList = !0)
     })), ee.initialize(authProxyAPIURL, geeAPIURL, (function() {
         geeAuthenticated = !0, setTimeout((function() {
-            "true" === localStorage["showIntroModal-" + mode] ? $("#introModal").modal().show() : void 0 === staticTemplates.loadingModal[mode] ? "MTBS" === mode ? showMessage("", staticTemplates.loadingModal.all("mtbs-logo.png", "Creating")) : "STORM" === mode || "Bloom-Mapper" === mode ? showMessage("", staticTemplates.loadingModal.all("logos_usda-fs_bn-dk-01.svg", "Creating")) : "lcms-dashboard" === mode ? showMessage("", staticTemplates.loadingModal.all("lcms-icon.png", "Loading", "LCMS summary areas")) : showMessage("", staticTemplates.loadingModal.all("lcms-icon.png", "Creating")) : showMessage("Loading", staticTemplates.loadingModal[mode]), $("#dontShowAgainCheckbox").change((function() {
+            "true" === localStorage["showIntroModal-" + mode] ? $("#introModal").modal().show() : void 0 === staticTemplates.loadingModal[mode] ? "MTBS" === mode ? showMessage("", staticTemplates.loadingModal.all("mtbs-logo.png", "Creating")) : "STORM" === mode || "Bloom-Mapper" === mode || "sequoia-view" === mode ? showMessage("", staticTemplates.loadingModal.all("logos_usda-fs_bn-dk-01.svg", "Creating")) : "lcms-dashboard" === mode ? showMessage("", staticTemplates.loadingModal.all("lcms-icon.png", "Loading", "LCMS summary areas")) : showMessage("", staticTemplates.loadingModal.all("lcms-icon.png", "Creating")) : showMessage("Loading", staticTemplates.loadingModal[mode]), $("#dontShowAgainCheckbox").change((function() {
                 localStorage["showIntroModal-" + mode] = !this.checked
             }))
         }), 1e3), geeAuthenticated && $("#main-container").append(staticTemplates.introModal[mode]), null === cachedStudyAreaName && $("#study-area-label").text(defaultStudyArea), "Ancillary" === mode ? run = runAncillary : "LCMS" === mode || "LCMS-pilot" === mode && 0 == studyAreaDict[longStudyAreaName].isPilot ? run = runGTAC : "LT" === mode ? run = runLT : "MTBS" === mode ? run = runMTBS : "TEST" === mode ? run = runTest : "IDS" === mode ? run = runIDS : "geeViz" === mode ? run = runGeeViz : "LAMDA" === mode ? run = runLAMDA : "STORM" === mode ? run = runStorm : "lcms-base-learner" === mode ? run = runBaseLearner : "TreeMap" === mode ? run = runTreeMap : "lcms-dashboard" === mode ? (run = runDashboard, map.setOptions({
             mapTypeControlOptions: {
                 style: google.maps.MapTypeControlStyle.DROPDOWN_MENU,
                 position: google.maps.ControlPosition.TOP_CENTER,
                 style: google.maps.MapTypeControlStyle.SMALL
@@ -2990,27 +3016,27 @@
                 position: google.maps.ControlPosition.TOP_CENTER
             },
             zoomControlOptions: {
                 position: google.maps.ControlPosition.TOP_CENTER,
                 style: google.maps.ZoomControlStyle.SMALL
             },
             draggableCursor: "pointer"
-        })) : "Bloom-Mapper" === mode ? run = runAlgal : "CONUS" === studyAreaName ? (longStudyAreaName = cachedStudyAreaName, run = runCONUS) : null != cachedStudyAreaName ? (longStudyAreaName = cachedStudyAreaName, resetStudyArea(cachedStudyAreaName)) : run = runUSFS, "LCMS" === mode && (setupDropdownTreeDownloads(studyAreaName), populateLCMSDownloads()), setGEERunID(), setTimeout((function() {
+        })) : "Bloom-Mapper" === mode ? run = runAlgal : "sequoia-view" === mode ? run = runSequoia : "CONUS" === studyAreaName ? (longStudyAreaName = cachedStudyAreaName, run = runCONUS) : null != cachedStudyAreaName ? (longStudyAreaName = cachedStudyAreaName, resetStudyArea(cachedStudyAreaName)) : run = runUSFS, "LCMS" === mode && (setupDropdownTreeDownloads(studyAreaName), populateLCMSDownloads()), setGEERunID(), setTimeout((function() {
             var e = !1,
                 a = 0;
 
             function t() {
                 try {
                     run(), e = !0
                 } catch (e) {
                     console.log(e), console.log("Failed to load GEE run function. Waiting 5 seconds to retry"), a++
                 }
             }
-            for (; !1 === e && a < 5;) t(), !1 === e && sleepFor(5e3);
-            setupAreaLayerSelection(), plotsOn && (addPlotCollapse(), loadAllPlots()), "true" !== localStorage["showIntroModal-" + mode] ? ($(".modal").modal("hide"), $(".modal-backdrop").remove()) : ($("#intro-modal-loading-div").hide(), $("#summary-spinner").hide()), "lcms-dashboard" === mode && (dashboardBoxSelect(), startDashboardViewExtentSelect()), addLabelOverlay(), ("true" === urlParams.sankey || "true" === urlParams.beta) && urlParams.endYear - urlParams.startYear < 5 && showMessage("No Transition Charting", "The year range must be 5 years or more to perform transition charting")
+            for (; !1 === e && a < 2;) t(), !1 === e && sleepFor(3e3);
+            setupAreaLayerSelection(), plotsOn && (addPlotCollapse(), loadAllPlots()), "true" !== localStorage["showIntroModal-" + mode] ? ($(".modal").modal("hide"), $(".modal-backdrop").remove()) : ($("#intro-modal-loading-div").hide(), $("#summary-spinner").hide()), "lcms-dashboard" === mode && (dashboardBoxSelect(), startDashboardViewExtentSelect()), addLabelOverlay(), urlParams.endYear - urlParams.startYear < 5 && "LCMS" === mode && showMessage("No Transition Charting", "The year range must be 5 years or more to perform transition charting")
         }), 1500)
     }), (function(e) {
         console.log(`Failed to authenticate to GEE: ${e}`), "LCMS" === mode && (setupDropdownTreeDownloads(studyAreaName), populateLCMSDownloads()), ga("send", "event", mode + "-gee-auth-error", "failure", "failure"), showMessage("Map Loading Error", staticTemplates.authErrorMessage)
     }))
 }
 var mapWaitCount = 0,
     mapWaitMax = 3;
@@ -3145,16 +3171,17 @@
 
 function clearQueryGeoJSON() {
     queryGeoJSON.forEach((function(e) {
         queryGeoJSON.remove(e)
     }))
 }
 $(document).ready(map_load);
-var queryWindowMode = "infoWindow",
-    getQueryImages = function(e, a) {
+var queryWindowMode = "infoWindow";
+queryWindowMode = "sidepane";
+var getQueryImages = function(e, a) {
         var t = [e, a];
         $(".gm-ui-hover-effect").show(), $("#summary-spinner").slideDown();
         var o = " Queried Values for Lng " + e.toFixed(3) + " Lat " + a.toFixed(3),
             l = `<div>\n\t\t\t\t\t\t\t<h6 style = 'font-weight:bold;'>Queried values for<br>lng: ${e.toFixed(3).toString()} lat: ${a.toFixed(3).toString()}</h6>\n\t\t\t\t\t\t\t<li id = 'query-list-container'></li>\n\t\t\t\t\t\t\t\n\t\t\t\t\t\t</div>`;
         "infoWindow" === queryWindowMode ? ($("#chart-collapse-label-chart-collapse-div").hide(), $("#chart-collapse-div").empty(), $("#legendDiv").css("max-width", ""), $("#legendDiv").css("max-height", "60%"), infowindow.setMap(null), infowindow.setPosition({
             lng: e,
             lat: a
@@ -3166,20 +3193,20 @@
         function n(e, a, t) {
             var l = t + "-container-" + r.toString();
             if (r++, $("#query-list-container").append("<table class=\"table table-hover bg-white\">\n\t\t\t\t\t\t\t\t\t\t\t\t<tbody>\n\t\t\t\t\t\t\t\t\t\t\t\t\t<tr class = 'bg-black'><th></th></tr>\n\t\t\t\t\t\t\t\t\t\t\t\t</tbody>\n\t\t\t\t\t\t\t\t\t\t\t  </table>"), null == e) $("#query-list-container").append(`<table class="table table-hover bg-white">\n\t\t\t\t\t\t\t\t\t\t\t\t<tbody id = '${l}'></tbody>\n\t\t\t\t\t\t\t\t\t\t\t  </table>`), $("#" + l).append(`<tr><th>${a.name}</th><th>NULL</th></tr>`);
             else if ("geeImage" === a.type) {
                 $("#query-list-container").append(`<table class="table table-hover bg-white">\n\t\t\t\t\t\t\t\t\t\t\t\t<tbody id = '${l}'></tbody>\n\t\t\t\t\t\t\t\t\t\t\t  </table>`);
                 let t = Object.keys(e);
                 if (1 === t.length) {
-                    var n = JSON.stringify(Object.values(e)[0]);
-                    null !== a.queryDict && void 0 !== a.queryDict && (n = a.queryDict[parseInt(n)]), $("#" + l).append(`<tr><th>${a.name}</th><td>${n}</td></tr>`)
+                    var n = Object.values(e)[0];
+                    null !== a.queryDict && void 0 !== a.queryDict ? n = a.queryDict[parseInt(n)] : n % 1 && (n = n.toFixed(4)), $("#" + l).append(`<tr><th>${a.name}</th><td>${n}</td></tr>`)
                 } else if (4 === t.length && t.indexOf("viz-blue") > -1 && t.indexOf("viz-green") > -1 && t.indexOf("viz-red") > -1) {
                     let o = t.filter((e => -1 === e.indexOf("viz-")))[0];
                     n = JSON.stringify(e[o]);
-                    null !== a.queryDict && void 0 !== a.queryDict && (n = a.queryDict[parseInt(n)]), $("#" + l).append(`<tr><th>${a.name}</th><td>${n}</td></tr>`)
+                    null !== a.queryDict && void 0 !== a.queryDict ? n = a.queryDict[parseInt(n)] : n % 1 && (n = n.toFixed(4)), $("#" + l).append(`<tr><th>${a.name}</th><td>${n}</td></tr>`)
                 } else $("#" + l).append(`<tr><th>${a.name}</th><th>Multi band</th></tr>`), Object.keys(e).map((function(a) {
                     try {
                         var t = e[a];
                         null !== t && (t = t.toFixed(2).toString()), $("#" + l).append(`<tr><td>${a}</td><td>${t}</td></tr>`)
                     } catch (e) {
                         $("#" + l).append(`<tr><td>${a}</td><td>${JSON.stringify(t)}</td></tr>`)
                     }
@@ -3344,15 +3371,15 @@
         }))
     }
 }
 var udpList = [],
     whichAreaDrawingMethod;
 
 function areaChartingTabSelect(e) {
-    stopAreaCharting(), stopCharting(), whichAreaDrawingMethod = e, console.log(e), "#user-defined" === e ? startUserDefinedAreaCharting() : "#shp-defined" === e ? startShpDefinedCharting() : "#pre-defined" === e ? $("#pre-defined").slideDown() : "#user-selected" === e && (map.setOptions({
+    stopAreaCharting(), stopCharting(), whichAreaDrawingMethod = e, "#user-defined" === e ? startUserDefinedAreaCharting() : "#shp-defined" === e ? startShpDefinedCharting() : "#pre-defined" === e ? $("#pre-defined").slideDown() : "#user-selected" === e && (map.setOptions({
         draggableCursor: "pointer"
     }), map.setOptions({
         cursor: "pointer"
     }))
 }
 
 function restartUserDefinedAreaCarting(e) {
@@ -3367,15 +3394,15 @@
             udpPolygonNumber--, udpPolygonNumber < 1 && (udpPolygonNumber = 1, showMessage("Error!", "No more vertices to undo")), udpPolygonObj[udpPolygonNumber].getPath().pop(1)
         }
         updateUserDefinedAreaArea()
     }
 }
 
 function startUserDefinedAreaCharting() {
-    console.log("start clicking"), map.setOptions({
+    map.setOptions({
         draggableCursor: "crosshair"
     }), map.setOptions({
         disableDoubleClickZoom: !0
     }), google.maps.event.clearListeners(mapDiv, "dblclick"), google.maps.event.clearListeners(mapDiv, "click"), window.addEventListener("keydown", restartUserDefinedAreaCarting), window.addEventListener("keydown", undoUserDefinedAreaCharting);
     try {
         udp.setMap(null)
     } catch (e) {}
@@ -3481,15 +3508,15 @@
 
 function cancelMakeAreaChart() {
     currentChartID++, $("#summary-spinner").slideUp()
 }
 
 function makeAreaChart(e, a, t) {
     var o = ++currentChartID;
-    areaGeoJson = null, console.log("making chart"), null == t && (t = !1), areaChartingCount++;
+    areaGeoJson = null, null == t && (t = !1), areaChartingCount++;
     randomColor().slice(1, 7);
     if (centerObject(e = e.set("source", "LCMS_data_explorer")), e = e.geometry(), "transition" === areaChartCollections[whichAreaChartCollection].type) {
         $("#summary-spinner").slideDown();
         areaChartCollections[whichAreaChartCollection].collection.sort("system:time_start").first().date().get("year").getInfo(), areaChartCollections[whichAreaChartCollection].collection.sort("system:time_start", !1).first().date().get("year").getInfo();
         let t = getTransitionRowData();
         if (null !== t) {
             let l = getTransitionClasses(areaChartCollections[whichAreaChartCollection].collection, t, areaChartCollections[whichAreaChartCollection].values, areaChartCollections[whichAreaChartCollection].bandName),
@@ -3612,18 +3639,17 @@
         (c = c.map((function(e) {
             return e.replaceAll("_", " ") + " " + areaChartFormatDict[areaChartFormat].label
         }))).unshift(r);
         var p = getAreaSummaryTable(l, e, r, multiplier, i, crs, transform, scale),
             u = 0,
             m = new Date;
         ! function t() {
-            console.log("Evaluating area chart tables"), p.evaluate((function(l, r) {
-                print(u), print(l), print(r), print(areaChartingCount);
-                var i = new Date - m;
-                if (console.log("dt: " + i.toString()), void 0 !== r && u < 60 && currentChartID === o && i < 1e4) t();
+            p.evaluate((function(l, r) {
+                var i = new Date;
+                if (void 0 !== r && u < 60 && currentChartID === o && i - m < 1e4) t();
                 else if (void 0 === r && currentChartID === o) {
                     l.unshift(c), $("#summary-spinner").slideUp();
                     var d = areaChartCollections[whichAreaChartCollection].stacked,
                         p = areaChartCollections[whichAreaChartCollection].steppedLine,
                         h = areaChartCollections[whichAreaChartCollection].colors,
                         g = areaChartCollections[whichAreaChartCollection].chartType,
                         v = areaChartCollections[whichAreaChartCollection].fieldsHidden;
@@ -3696,15 +3722,15 @@
 }
 
 function startShpDefinedCharting() {
     turnOnUploadedLayers(), void 0 !== selectionTracker.uploadedLayerIndices && null !== selectionTracker.uploadedLayerIndices || (selectionTracker.uploadedLayerIndices = [])
 }
 
 function stopAreaCharting() {
-    window.removeEventListener("keydown", restartUserDefinedAreaCarting), window.removeEventListener("keydown", undoUserDefinedAreaCharting), console.log("stopping area charting");
+    window.removeEventListener("keydown", restartUserDefinedAreaCarting), window.removeEventListener("keydown", undoUserDefinedAreaCharting);
     try {
         Object.keys(udpPolygonObj).map((function(e) {
             udpPolygonObj[e].setMap(null)
         })), udpPolygonObj = {}, udpPolygonNumber = 1, updateUserDefinedAreaArea()
     } catch (e) {}
     $("#areaUpload").unbind("change"), $("#summary-spinner").slideUp()
 }
@@ -3712,15 +3738,15 @@
 function startQuery() {
     areaGeoJson = null;
     try {
         udp.setMap(null)
     } catch (e) {
         console.log(e)
     }
-    google.maps.event.clearListeners(mapDiv, "dblclick"), google.maps.event.clearListeners(mapDiv, "click"), map.setOptions({
+    "infoWindow" !== queryWindowMode && $("#chart-collapse-label-chart-collapse-div").show(), google.maps.event.clearListeners(mapDiv, "dblclick"), google.maps.event.clearListeners(mapDiv, "click"), map.setOptions({
         draggableCursor: "help"
     }), map.setOptions({
         cursor: "help"
     }), mapHammer = new Hammer(document.getElementById("map")), mapHammer.on("doubletap", (function(e) {
         $("#summary-spinner").slideDown(), map.setOptions({
             draggableCursor: "progress"
         }), map.setOptions({
@@ -3729,15 +3755,14 @@
         var a = e.center.x,
             t = e.center.y;
         center = point2LatLng(a, t), addClickMarker(ee.Geometry.Point([center.lng(), center.lat()]).buffer(plotRadius).bounds()), marker.setMap(map), getQueryImages(center.lng(), center.lat())
     }))
 }
 
 function stopQuery() {
-    print("stopping");
     try {
         mapHammer.destroy(), map.setOptions({
             draggableCursor: "hand"
         }), map.setOptions({
             cursor: "hand"
         }), google.maps.event.clearListeners(mapDiv, "dblclick"), map.setOptions({
             cursor: "hand"
@@ -3831,59 +3856,57 @@
 function configChartModal(e = "chartJS") {
     $(document).height() / $(document).width() > 1 ? (canvasHeight = "90%", canvasWidth = "100%") : (canvasHeight = "50%", canvasWidth = "100%"), clearModal("chart-modal"), $("#chart-modal-body").append("<div id = 'chart-modal-graph-table-container' class = 'flexcroll chart-table-graph-container'></div>"), "chartJS" === e ? $("#chart-modal-graph-table-container").append(`<div id = 'chart-modal-graph-container' class = 'pb-2'>\n\t    \t\t\t\t\t\t\t\t\t\t\t\t\t<canvas id="chart-canvas" width="${canvasWidth}" height = "${canvasHeight}" ></canvas>\n\t    \t\t\t\t\t\t\t\t\t\t\t\t</div>`) : $("#chart-modal-graph-table-container").append('<div id = \'chart-modal-graph-container\' class = \'pb-2\'>\n\t    \t\t\t\t\t\t\t\t\t\t\t\t\t<div id="chart-canvas"></div>\n\t    \t\t\t\t\t\t\t\t\t\t\t\t\t<div id="chart-download-canvas" style="display:none;"></div>\n\t    \t\t\t\t\t\t\t\t\t\t\t\t</div>'), $("#chart-modal-graph-table-container").append(`<div id="chart-table" style = 'display:none;' width="${canvasWidth}" height = "${canvasHeight}" ></div>`)
 }
 
 function addChartJS(e, a, t, o, l, r, n, s, i) {
     var d = !0,
         c = !0;
-    null == i && (i = null), null == n && (n = "", d = !1), null == s && (s = "", c = !1), null == r && (r = chartColors), null == t && (t = "line"), null == o && (o = !1), void 0 !== l && null != l || (l = !1), console.log("starting convert to table"), dataTable = dataTableNumbersToNames(e), console.log("finished convert to table"), configChartModal();
+    null == i && (i = null), null == n && (n = "", d = !1), null == s && (s = "", c = !1), null == r && (r = chartColors), null == t && (t = "line"), null == o && (o = !1), void 0 !== l && null != l || (l = !1), dataTable = dataTableNumbersToNames(e), configChartModal();
     var p = arrayColumn(e.slice(1), 0),
-        u = range(1, e[1].length);
-    console.log("starting to convert to chart");
-    var m = u.map((function(a) {
-        var t = !1;
-        null !== i && (t = i[a - 1]);
-        var n = arrayColumn(e, a),
-            s = n[0],
-            d = n.slice(1);
-        d = d.map((function(e) {
-            var a;
-            try {
-                a = e.toFixed(6)
-            } catch (t) {
-                a = e
-            }
-            return a
+        u = range(1, e[1].length).map((function(a) {
+            var t = !1;
+            null !== i && (t = i[a - 1]);
+            var n = arrayColumn(e, a),
+                s = n[0],
+                d = n.slice(1);
+            d = d.map((function(e) {
+                var a;
+                try {
+                    a = e.toFixed(6)
+                } catch (t) {
+                    a = e
+                }
+                return a
+            }));
+            var c = r[(a - 1) % r.length]; - 1 === c.indexOf("#") && (c = "#" + c);
+            var p = {
+                label: s,
+                pointStyle: "circle",
+                pointRadius: 1,
+                data: d,
+                fill: !1,
+                borderColor: c,
+                lineTension: 0,
+                borderWidth: 2,
+                steppedLine: l,
+                showLine: !0,
+                spanGaps: !0,
+                hidden: t
+            };
+            return o && (p.fill = !0, p.backgroundColor = c), p
         }));
-        var c = r[(a - 1) % r.length]; - 1 === c.indexOf("#") && (c = "#" + c);
-        var p = {
-            label: s,
-            pointStyle: "circle",
-            pointRadius: 1,
-            data: d,
-            fill: !1,
-            borderColor: c,
-            lineTension: 0,
-            borderWidth: 2,
-            steppedLine: l,
-            showLine: !0,
-            spanGaps: !0,
-            hidden: t
-        };
-        return o && (p.fill = !0, p.backgroundColor = c), p
-    }));
-    console.log("finished to convert to chart"), chartColorI = 0;
+    chartColorI = 0;
     try {
         chartJSChart.destroy()
     } catch (e) {}
     chartJSChart = new Chart($("#chart-canvas"), {
         type: t,
         data: {
             labels: p,
-            datasets: m
+            datasets: u
         },
         options: {
             title: {
                 display: !0,
                 position: "top",
                 text: a.replaceAll("_", " "),
                 fontSize: 16
@@ -3914,16 +3937,16 @@
                         labelString: n
                     },
                     maxBarThickness: 100
                 }]
             }
         }
     }), $("#chart-download-dropdown").empty(), $("#chart-modal-footer").append(`<div class="dropdown">\n\t\t\t\t\t\t\t\t\t\t  <div class=" dropdown-toggle"  id="chartDownloadDropdown" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">\n\t\t\t\t\t\t\t\t\t\t    Download\n\t\t\t\t\t\t\t\t\t\t  </div>\n\t\t\t\t\t\t\t\t\t\t  <div id = 'chart-download-dropdown' class="dropdown-menu px-2" aria-labelledby="chartDownloadDropdown">\n\t\t\t\t\t\t\t\t\t\t    <a class="dropdown-item" href="#" onclick = "downloadChartJS(chartJSChart,'${a}.png')">PNG</a>\n\t\t\t\t\t\t\t\t\t\t    <a class="dropdown-item" href="#" onclick = "exportToCsv('${a}.csv', dataTable)">CSV</a>\n\t\t\t\t\t\t\t\t\t\t  </div>\n\t\t\t\t\t\t\t\t\t\t</div>\n\t\t\t\t\t\t\t\t\t\t\n\t\t\t\t\t\t\t\t\t\t</div>\n\t\t\t\t\t\t\t\t\t\t<div class="dropdown">\n\t\t\t\t\t\t\t\t\t\t  <div class=" dropdown-toggle"  id="chartTypeDropdown" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">\n\t\t\t\t\t\t\t\t\t\t    Chart Type\n\t\t\t\t\t\t\t\t\t\t  </div>\n\t\t\t\t\t\t\t\t\t\t  <div id = 'chart-type-dropdown' class="dropdown-menu px-2" aria-labelledby="chartTypeDropdown">\n\t\t\t\t\t\t\t\t\t\t    <a class="dropdown-item" href="#" onclick = "toggleChartTable('chart');change('line',false,${l});">Line</a>\n\t\t\t\t\t\t\t\t\t\t    <a class="dropdown-item" href="#" onclick = "toggleChartTable('chart');change('line',true,${l});">Stacked Line</a>\n\t\t\t\t\t\t\t\t\t\t    <a class="dropdown-item" href="#" onclick = "toggleChartTable('chart');change('bar',false,${l});">Bar</a>\n\t\t\t\t\t\t\t\t\t\t    <a class="dropdown-item" href="#" onclick = "toggleChartTable('chart');change('bar',true,${l});">Stacked Bar</a>\n\t\t\t\t\t\t\t\t\t\t    <a class="dropdown-item" href="#" onclick = "toggleChartTable('table')">Table</a>\n\t\t\t\t\t\t\t\t\t\t  </div>\n\t\t\t\t\t\t\t\t\t\t</div>\n\t\t\t\t\t\t\t\t\t\t`);
-    var h = htmlTable(dataTable);
-    $("#chart-table").append(h), toggleChartTable(localStorage.tableOrChart), $("#chart-modal").modal()
+    var m = htmlTable(dataTable);
+    $("#chart-table").append(m), toggleChartTable(localStorage.tableOrChart), $("#chart-modal").modal()
 }
 
 function toggleChartTable(e) {
     "table" === e ? ($("#chart-modal-graph-container").hide(), $("#chart-table").show(), localStorage.tableOrChart = "table") : "chart" === e ? ($("#chart-modal-graph-container").show(), $("#chart-table").hide(), localStorage.tableOrChart = "chart") : ($("#chart-modal-graph-container").show(), $("#chart-table").show(), localStorage.tableOrChart = "both")
 }
 
 function change(e, a, t) {
@@ -4113,15 +4136,14 @@
         uriName = pixelChartCollections[whichPixelChartCollection].label.replaceAll(" ", "_") + "_lng_" + center.lng().toFixed(4).toString() + "_lat_" + center.lat().toFixed(4).toString(), chartTitle = pixelChartCollections[whichPixelChartCollection].label + " (lng: " + center.lng().toFixed(4).toString() + " lat: " + center.lat().toFixed(4).toString() + ")", csvName = uriName + ".csv", r.getRegion(l, scale, crs, transform).evaluate((function(e, a) {
             if ($("#summary-spinner").slideUp(), null != a && showMessage('<i class="text-dark text-uppercase fa fa-exclamation-triangle"></i> Error! Try again', a), null != e && e.length > 1) {
                 var t = r.size().getInfo() + 1;
                 e.length > t && (console.log("reducing number of inputs"), e = e.slice(0, t)),
                     function(e) {
                         if (chartIncludeDate) var a = 3;
                         else a = 4;
-                        print("Extracted values:"), print(e);
                         var t = e[0].slice(a);
                         e = e.slice(1).map((function(e) {
                             return e.slice(a)
                         })).sort(sortFunction), chartIncludeDate && (e = e.map((function(e) {
                             var a = e[0];
                             if (!1 === pixelChartCollections[whichPixelChartCollection].simplifyDate) var t = new Date(a).toGMTString();
                             else t = !0 === pixelChartCollections[whichPixelChartCollection].semiSimpleDate ? `${new Date(a).getFullYear()}-${new Date(a).getMonth()+1}-${new Date(a).getDate()}` : (new Date(a).getYear() + 1900).toString();
@@ -4255,15 +4277,15 @@
             o && e.push(l)
         }))
     })), e
 }
 
 function updateToolStatusBar() {
     var e = !1;
-    $("#current-tool-selection").empty(), $("#current-tool-selection").append("Currently active tools: "), Object.keys(toolFunctions).map((function(a) {
+    $("#current-tool-selection").empty(), $("#current-tool-selection").append("Ative tools: "), Object.keys(toolFunctions).map((function(a) {
         Object.keys(toolFunctions[a]).map((function(t) {
             var o = toolFunctions[a][t].state,
                 l = toolFunctions[a][t].title;
             o && ($("#current-tool-selection").append(`${l}`), e = !0)
         }))
     })), e ? ga("send", "event", "tool-active", mode, $("#current-tool-selection").html().split(": ")[1]) : $("#current-tool-selection").append("No active tools")
 }
```

### Comparing `geeViz-2023.4.1/geeViz/geeView/js/load.min.js` & `geeViz-2023.6.1/geeViz/geeView/js/load.min.js`

 * *Files identical despite different names*

### Comparing `geeViz-2023.4.1/geeViz/geeView.py` & `geeViz-2023.6.1/geeViz/geeView.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-   Copyright 2020 Ian Housman
+   Copyright 2023 Ian Housman
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
 
@@ -18,15 +18,15 @@
 ######################################################################
 #Import modules
 import ee,sys,os,webbrowser,json,socket,subprocess,site,time,requests
 from google.auth.transport import requests as gReq
 from google.oauth2 import service_account
 
 from threading import Thread
-from IPython.display import IFrame
+from IPython.display import IFrame,display, HTML
 if sys.version_info[0] < 3:
     import SimpleHTTPServer, SocketServer
 else:
     import http.server, socketserver 
 ######################################################################
 #Set up GEE and paths
 try:
@@ -55,14 +55,29 @@
 if os.path.exists(ee_run_dir) == False:os.makedirs(ee_run_dir)
 
 
 ######################################################################
 ######################################################################
 #Functions
 
+######################################################################
+# Function to check if being run inside a notebook
+# Taken from: https://stackoverflow.com/questions/15411967/how-can-i-check-if-code-is-executed-in-the-ipython-notebook
+def is_notebook():
+    try:
+        shell = get_ipython().__class__.__name__
+        if shell == 'ZMQInteractiveShell':
+            return True   # Jupyter notebook or qtconsole
+        elif shell == 'TerminalInteractiveShell':
+            return False  # Terminal running IPython
+        else:
+            return False  # Other type (?)
+    except NameError:
+        return False      # Probably standard Python interpreter
+######################################################################
 # Function for cleaning trailing .... in accessToken
 def cleanAccessToken(accessToken):
     while accessToken[-1] == '.': accessToken = accessToken[:-1]
     return accessToken
 
 # Function for using default GEE refresh token to get an access token for geeView
 def refreshToken(refresh_token_path = ee.oauth.get_credentials_path()):
@@ -129,14 +144,17 @@
 class mapper:
     def __init__(self,port = 8001):
         self.port = port
         self.layerNumber = 1
         self.idDictList = []
         self.mapCommandList  = []
         self.ee_run_name = 'runGeeViz'
+
+        self.isNotebook = is_notebook()
+
         self.refreshTokenPath = ee.oauth.get_credentials_path()
         self.serviceKeyPath = None
         self.queryWindowMode = 'sidePane'
         
     #Function for adding a layer to the map
     def addLayer(self,image,viz = {},name= None,visible= True):
         if name == None:
@@ -166,22 +184,22 @@
         idDict['viz'] = json.dumps(viz, sort_keys=False)
         idDict['function'] = 'addSerializedTimeLapse'
         self.idDictList.append(idDict)
 
     #Function for centering on a GEE object that has a geometry
     def centerObject(self,feature):
         try:
-            bounds = json.dumps(feature.geometry().bounds(100).getInfo())
+            bounds = json.dumps(feature.geometry().bounds(100,'EPSG:4326').getInfo())
         except Exception as e:
-            bounds = json.dumps(feature.bounds(100).getInfo())
+            bounds = json.dumps(feature.bounds(100,'EPSG:4326').getInfo())
         command = 'synchronousCenterObject('+bounds+')'
         
         self.mapCommandList.append(command)
     #Function for launching the web map after all adding to the map has been completed
-    def view(self,open_browser = True, open_iframe = False,iframe_height = 525):
+    def view(self,open_browser = None, open_iframe = None,iframe_height = 525):
         print('Starting webmap')
 
         # Get access token
         if self.serviceKeyPath == None:
             print('Using default refresh token for geeView:',self.refreshTokenPath)
             self.accessToken = refreshToken(self.refreshTokenPath)
         else:
@@ -213,28 +231,48 @@
         
         #Write out js file
         self.ee_run = os.path.join(ee_run_dir, '{}.js'.format(self.ee_run_name))
         oo = open(self.ee_run,'w')
         oo.writelines(lines)
         oo.close()
         # time.sleep(5)
+
+        # if not self.isNotebook:
+        #     self.Map.save(os.path.join(folium_html_folder,folium_html))
+        #     if not geeView.isPortActive(self.port):
+        #         print('Starting local web server at: http://localhost:{}/{}/'.format(self.port,geeView.geeViewFolder))
+        #         geeView.run_local_server(self.port)
+        #         print('Done')
+        #     else:
+        #         print('Local web server at: http://localhost:{}/{}/ already serving.'.format(self.port,geeView.geeViewFolder))
+        #     if open_browser:
+        #         geeView.webbrowser.open('http://localhost:{}/{}/{}'.format(self.port,geeView.geeViewFolder,folium_html),new = 1)
+
+        # else:
+        #     display(self.Map)
+        
         if not isPortActive(self.port):
             print('Starting local web server at: http://localhost:{}/{}/'.format(self.port,geeViewFolder))
             run_local_server(self.port)
             print('Done')
             
 
         else:
             print('Local web server at: http://localhost:{}/{}/ already serving.'.format(self.port,geeViewFolder))
             # print('Refresh browser instance')
+       
+
         print('cwd',os.getcwd())
-        if open_browser:
+        if not self.isNotebook or open_browser:
             webbrowser.open('http://localhost:{}/{}/?accessToken={}'.format(self.port,geeViewFolder,self.accessToken),new = 1)
-        if open_iframe:
+        elif open_browser == False and open_iframe:
+            self.IFrame = IFrame(src='http://localhost:{}/{}/?accessToken={}'.format(self.port,geeViewFolder,self.accessToken), width='100%', height='{}px'.format(iframe_height))
+        else:
             self.IFrame = IFrame(src='http://localhost:{}/{}/?accessToken={}'.format(self.port,geeViewFolder,self.accessToken), width='100%', height='{}px'.format(iframe_height))
+            display(self.IFrame)
     def clearMap(self):
         self.layerNumber = 1
         self.idDictList = []
         self.mapCommandList  = []
     def setMapTitle(self,title):
         query_command = "$('#title-banner').html('{0}');document.title = 'geeViz | {0}';".format(title)
         if query_command not in self.mapCommandList:
```

### Comparing `geeViz-2023.4.1/geeViz/getImagesLib.py` & `geeViz-2023.6.1/geeViz/getImagesLib.py`

 * *Files 0% similar despite different names*

```diff
@@ -10665,265 +10665,266 @@
 00029a80: 2072 6573 756c 7420 696e 2066 616c 7365   result in false
 00029a90: 206e 6567 6174 6976 6573 2028 6f6d 6973   negatives (omis
 00029aa0: 7369 6f6e 290d 0a64 6566 2073 696d 706c  sion)..def simpl
 00029ab0: 6557 6174 6572 4d61 736b 2869 6d67 2c63  eWaterMask(img,c
 00029ac0: 6f6e 7472 6163 7450 6978 656c 7320 3d20  ontractPixels = 
 00029ad0: 302c 736c 6f70 655f 7468 7265 7368 203d  0,slope_thresh =
 00029ae0: 2031 302c 656c 6576 6174 696f 6e49 6d61   10,elevationIma
-00029af0: 6765 5061 7468 203d 2022 5553 4753 2f4e  gePath = "USGS/N
-00029b00: 4544 222c 656c 6576 6174 696f 6e46 6f63  ED",elevationFoc
-00029b10: 616c 4d65 616e 5261 6469 7573 203d 2035  alMeanRadius = 5
-00029b20: 2e35 293a 0d0a 2020 696d 6720 3d20 6164  .5):..  img = ad
-00029b30: 6454 4341 6e67 6c65 7328 696d 6729 0d0a  dTCAngles(img)..
-00029b40: 2020 6e65 6420 3d20 6565 2e49 6d61 6765    ned = ee.Image
-00029b50: 2865 6c65 7661 7469 6f6e 496d 6167 6550  (elevationImageP
-00029b60: 6174 6829 2e72 6573 616d 706c 6528 2762  ath).resample('b
-00029b70: 6963 7562 6963 2729 0d0a 2020 736c 6f70  icubic')..  slop
-00029b80: 6520 3d20 6565 2e54 6572 7261 696e 2e73  e = ee.Terrain.s
-00029b90: 6c6f 7065 286e 6564 2e66 6f63 616c 5f6d  lope(ned.focal_m
-00029ba0: 6561 6e28 656c 6576 6174 696f 6e46 6f63  ean(elevationFoc
-00029bb0: 616c 4d65 616e 5261 6469 7573 2929 0d0a  alMeanRadius))..
-00029bc0: 2020 666c 6174 203d 2073 6c6f 7065 2e6c    flat = slope.l
-00029bd0: 7465 2873 6c6f 7065 5f74 6872 6573 6829  te(slope_thresh)
-00029be0: 0d0a 0d0a 2020 7761 7465 724d 6173 6b20  ....  waterMask 
-00029bf0: 3d20 696d 672e 7365 6c65 6374 285b 2774  = img.select(['t
-00029c00: 6341 6e67 6c65 4257 275d 292e 6774 6528  cAngleBW']).gte(
-00029c10: 2d30 2e30 3529 5c0d 0a20 2020 202e 416e  -0.05)\..    .An
-00029c20: 6428 696d 672e 7365 6c65 6374 285b 2774  d(img.select(['t
-00029c30: 6341 6e67 6c65 4247 275d 292e 6c74 6528  cAngleBG']).lte(
-00029c40: 302e 3035 2929 5c0d 0a20 2020 202e 416e  0.05))\..    .An
-00029c50: 6428 696d 672e 7365 6c65 6374 285b 2762  d(img.select(['b
-00029c60: 7269 6768 746e 6573 7327 5d29 2e6c 7428  rightness']).lt(
-00029c70: 302e 3329 295c 0d0a 2020 2020 2e41 6e64  0.3))\..    .And
-00029c80: 2866 6c61 7429 2e66 6f63 616c 5f6d 696e  (flat).focal_min
-00029c90: 2863 6f6e 7472 6163 7450 6978 656c 7329  (contractPixels)
-00029ca0: 0d0a 0d0a 2020 7265 7475 726e 2077 6174  ....  return wat
-00029cb0: 6572 4d61 736b 2e72 656e 616d 6528 5b27  erMask.rename(['
-00029cc0: 7761 7465 724d 6173 6b27 5d29 0d0a 2323  waterMask'])..##
-00029cd0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00029af0: 6765 5061 7468 203d 2022 5553 4753 2f33  gePath = "USGS/3
+00029b00: 4445 502f 3130 6d22 2c65 6c65 7661 7469  DEP/10m",elevati
+00029b10: 6f6e 466f 6361 6c4d 6561 6e52 6164 6975  onFocalMeanRadiu
+00029b20: 7320 3d20 352e 3529 3a0d 0a20 2069 6d67  s = 5.5):..  img
+00029b30: 203d 2061 6464 5443 416e 676c 6573 2869   = addTCAngles(i
+00029b40: 6d67 290d 0a20 206e 6564 203d 2065 652e  mg)..  ned = ee.
+00029b50: 496d 6167 6528 656c 6576 6174 696f 6e49  Image(elevationI
+00029b60: 6d61 6765 5061 7468 292e 7265 7361 6d70  magePath).resamp
+00029b70: 6c65 2827 6269 6375 6269 6327 290d 0a20  le('bicubic').. 
+00029b80: 2073 6c6f 7065 203d 2065 652e 5465 7272   slope = ee.Terr
+00029b90: 6169 6e2e 736c 6f70 6528 6e65 642e 666f  ain.slope(ned.fo
+00029ba0: 6361 6c5f 6d65 616e 2865 6c65 7661 7469  cal_mean(elevati
+00029bb0: 6f6e 466f 6361 6c4d 6561 6e52 6164 6975  onFocalMeanRadiu
+00029bc0: 7329 290d 0a20 2066 6c61 7420 3d20 736c  s))..  flat = sl
+00029bd0: 6f70 652e 6c74 6528 736c 6f70 655f 7468  ope.lte(slope_th
+00029be0: 7265 7368 290d 0a0d 0a20 2077 6174 6572  resh)....  water
+00029bf0: 4d61 736b 203d 2069 6d67 2e73 656c 6563  Mask = img.selec
+00029c00: 7428 5b27 7463 416e 676c 6542 5727 5d29  t(['tcAngleBW'])
+00029c10: 2e67 7465 282d 302e 3035 295c 0d0a 2020  .gte(-0.05)\..  
+00029c20: 2020 2e41 6e64 2869 6d67 2e73 656c 6563    .And(img.selec
+00029c30: 7428 5b27 7463 416e 676c 6542 4727 5d29  t(['tcAngleBG'])
+00029c40: 2e6c 7465 2830 2e30 3529 295c 0d0a 2020  .lte(0.05))\..  
+00029c50: 2020 2e41 6e64 2869 6d67 2e73 656c 6563    .And(img.selec
+00029c60: 7428 5b27 6272 6967 6874 6e65 7373 275d  t(['brightness']
+00029c70: 292e 6c74 2830 2e33 2929 5c0d 0a20 2020  ).lt(0.3))\..   
+00029c80: 202e 416e 6428 666c 6174 292e 666f 6361   .And(flat).foca
+00029c90: 6c5f 6d69 6e28 636f 6e74 7261 6374 5069  l_min(contractPi
+00029ca0: 7865 6c73 290d 0a0d 0a20 2072 6574 7572  xels)....  retur
+00029cb0: 6e20 7761 7465 724d 6173 6b2e 7265 6e61  n waterMask.rena
+00029cc0: 6d65 285b 2777 6174 6572 4d61 736b 275d  me(['waterMask']
+00029cd0: 290d 0a23 2323 2323 2323 2323 2323 2323  )..#############
 00029ce0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00029cf0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00029d00: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00029d10: 2323 230d 0a23 4a65 6666 2048 6f20 4d65  ###..#Jeff Ho Me
-00029d20: 7468 6f64 2066 6f72 2061 6c67 616c 2062  thod for algal b
-00029d30: 6c6f 6f6d 2064 6574 6563 7469 6f6e 0d0a  loom detection..
-00029d40: 2368 7474 7073 3a2f 2f77 7777 2e6e 6174  #https://www.nat
-00029d50: 7572 652e 636f 6d2f 6172 7469 636c 6573  ure.com/articles
-00029d60: 2f73 3431 3538 362d 3031 392d 3136 3438  /s41586-019-1648
-00029d70: 2d37 0d0a 0d0a 2320 5369 6d70 6c69 6669  -7....# Simplifi
-00029d80: 6564 2053 6372 6970 7420 666f 7220 4c61  ed Script for La
-00029d90: 6e64 7361 7420 5761 7465 7220 5175 616c  ndsat Water Qual
-00029da0: 6974 790d 0a23 2050 726f 6475 6365 7320  ity..# Produces 
-00029db0: 6120 6d61 7020 6f66 2061 6e20 616c 6761  a map of an alga
-00029dc0: 6c20 626c 6f6f 6d20 696e 204c 616b 6520  l bloom in Lake 
-00029dd0: 4572 6965 206f 6e20 3230 3131 2f39 2f33  Erie on 2011/9/3
-00029de0: 0d0a 2320 4372 6561 7465 6420 6f6e 2031  ..# Created on 1
-00029df0: 322f 372f 3230 3135 2062 7920 4a65 6666  2/7/2015 by Jeff
-00029e00: 2048 6f0d 0a0d 0a23 2053 7065 6369 6669   Ho....# Specifi
-00029e10: 6573 2061 2074 6872 6573 686f 6c64 2066  es a threshold f
-00029e20: 6f72 2068 7565 2074 6f20 6573 7469 6d61  or hue to estima
-00029e30: 7465 2022 6772 6565 6e22 2070 6978 656c  te "green" pixel
-00029e40: 730d 0a23 2074 6869 7320 6973 2075 7365  s..# this is use
-00029e50: 6420 6173 2061 6e20 6164 6469 7469 6f6e  d as an addition
-00029e60: 616c 2066 696c 7465 7220 746f 2072 6566  al filter to ref
-00029e70: 696e 6520 7468 6520 616c 676f 7269 7468  ine the algorith
-00029e80: 6d20 6162 6f76 650d 0a64 6566 2048 6f43  m above..def HoC
-00029e90: 616c 6347 7265 656e 6e65 7373 2869 6d67  alcGreenness(img
-00029ea0: 293a 0d0a 2020 236d 6170 2072 2c20 672c  ):..  #map r, g,
-00029eb0: 2061 6e64 2062 2066 6f72 206d 6f72 6520   and b for more 
-00029ec0: 7265 6164 6162 6c65 2061 6c67 6562 7261  readable algebra
-00029ed0: 2062 656c 6f77 0d0a 2020 7220 3d20 696d   below..  r = im
-00029ee0: 672e 7365 6c65 6374 285b 2772 6564 275d  g.select(['red']
-00029ef0: 290d 0a20 2067 203d 2069 6d67 2e73 656c  )..  g = img.sel
-00029f00: 6563 7428 5b27 6772 6565 6e27 5d29 0d0a  ect(['green'])..
-00029f10: 2020 6220 3d20 696d 672e 7365 6c65 6374    b = img.select
-00029f20: 285b 2762 6c75 6527 5d29 0d0a 0d0a 2020  (['blue'])....  
-00029f30: 2363 616c 6375 6c61 7465 2069 6e74 656e  #calculate inten
-00029f40: 7369 7479 2c20 6875 650d 0a20 2049 203d  sity, hue..  I =
-00029f50: 2072 2e61 6464 2867 292e 6164 6428 6229   r.add(g).add(b)
-00029f60: 2e72 656e 616d 6528 5b27 4927 5d29 0d0a  .rename(['I'])..
-00029f70: 2020 6d69 6e73 203d 2072 2e6d 696e 2867    mins = r.min(g
-00029f80: 292e 6d69 6e28 6229 2e72 656e 616d 6528  ).min(b).rename(
-00029f90: 5b27 6d69 6e73 275d 290d 0a20 2048 203d  ['mins'])..  H =
-00029fa0: 206d 696e 732e 7768 6572 6528 6d69 6e73   mins.where(mins
-00029fb0: 2e65 7128 7229 2c28 622e 7375 6274 7261  .eq(r),(b.subtra
-00029fc0: 6374 2872 2929 2e64 6976 6964 6528 492e  ct(r)).divide(I.
-00029fd0: 7375 6274 7261 6374 2872 2e6d 756c 7469  subtract(r.multi
-00029fe0: 706c 7928 3329 2929 2e61 6464 2831 2920  ply(3))).add(1) 
-00029ff0: 290d 0a20 2048 203d 2048 2e77 6865 7265  )..  H = H.where
-0002a000: 286d 696e 732e 6571 2867 292c 2872 2e73  (mins.eq(g),(r.s
-0002a010: 7562 7472 6163 7428 6729 292e 6469 7669  ubtract(g)).divi
-0002a020: 6465 2849 2e73 7562 7472 6163 7428 672e  de(I.subtract(g.
-0002a030: 6d75 6c74 6970 6c79 2833 2929 292e 6164  multiply(3))).ad
-0002a040: 6428 3229 2029 0d0a 2020 4820 3d20 482e  d(2) )..  H = H.
-0002a050: 7768 6572 6528 6d69 6e73 2e65 7128 6229  where(mins.eq(b)
-0002a060: 2c28 672e 7375 6274 7261 6374 2862 2929  ,(g.subtract(b))
-0002a070: 2e64 6976 6964 6528 492e 7375 6274 7261  .divide(I.subtra
-0002a080: 6374 2862 2e6d 756c 7469 706c 7928 3329  ct(b.multiply(3)
-0002a090: 2929 2029 0d0a 0d0a 2020 2370 6978 656c  )) )....  #pixel
-0002a0a0: 7320 7769 7468 2068 7565 2062 656c 6f77  s with hue below
-0002a0b0: 2031 2e36 206d 6f72 6520 6c69 6b65 6c79   1.6 more likely
-0002a0c0: 2074 6f20 6265 2062 6c6f 6f6d 2061 6e64   to be bloom and
-0002a0d0: 206e 6f74 2073 7573 7065 6e64 6564 2073   not suspended s
-0002a0e0: 6564 696d 656e 740d 0a20 2048 7468 7265  ediment..  Hthre
-0002a0f0: 7368 203d 2048 2e6c 7465 2831 2e36 290d  sh = H.lte(1.6).
-0002a100: 0a0d 0a20 2072 6574 7572 6e20 482e 7265  ...  return H.re
-0002a110: 6e61 6d65 2827 4827 290d 0a0d 0a0d 0a23  name('H')......#
-0002a120: 4170 706c 7920 626c 6f6f 6d20 6465 7465  Apply bloom dete
-0002a130: 6374 696f 6e20 616c 676f 7269 7468 6d0d  ction algorithm.
-0002a140: 0a64 6566 2048 6f43 616c 6341 6c67 6f72  .def HoCalcAlgor
-0002a150: 6974 686d 3128 696d 6167 6529 3a0d 0a20  ithm1(image):.. 
-0002a160: 2074 7275 6563 6f6c 6f72 203d 2031 2023   truecolor = 1 #
-0002a170: 7368 6f77 2074 7275 6520 636f 6c6f 7220  show true color 
-0002a180: 696d 6167 6520 6173 2077 656c 6c0d 0a20  image as well.. 
-0002a190: 2074 6573 7454 6872 6573 6820 3d20 4661   testThresh = Fa
-0002a1a0: 6c73 6520 2320 6164 6420 6120 6269 6e61  lse # add a bina
-0002a1b0: 7279 2069 6d61 6765 2063 6c61 7373 6966  ry image classif
-0002a1c0: 7969 6e67 2069 6e74 6f20 2262 6c6f 6f6d  ying into "bloom
-0002a1d0: 2261 6e64 2022 6e6f 6e2d 626c 6f6f 6d0d  "and "non-bloom.
-0002a1e0: 0a20 2062 6c6f 6f6d 5468 7265 7368 6f6c  .  bloomThreshol
-0002a1f0: 6420 3d20 302e 3032 3334 3620 2374 6872  d = 0.02346 #thr
-0002a200: 6573 686f 6c64 2066 6f72 2063 6c61 7373  eshold for class
-0002a210: 6966 6963 6174 696f 6e20 6669 7420 6261  ification fit ba
-0002a220: 7365 6420 6f6e 206f 7468 6572 2064 6174  sed on other dat
-0002a230: 610d 0a20 2067 7265 656e 6573 7354 6872  a..  greenessThr
-0002a240: 6573 686f 6c64 203d 2031 2e36 0d0a 0d0a  eshold = 1.6....
-0002a250: 2020 2320 416c 676f 7269 7468 6d20 3120    # Algorithm 1 
-0002a260: 6261 7365 6420 6f6e 3a0d 0a20 2023 2057  based on:..  # W
-0002a270: 616e 672c 204d 2e2c 2026 2053 6869 2c20  ang, M., & Shi, 
-0002a280: 572e 2028 3230 3037 292e 2054 6865 204e  W. (2007). The N
-0002a290: 4952 2d53 5749 5220 636f 6d62 696e 6564  IR-SWIR combined
-0002a2a0: 2061 746d 6f73 7068 6572 6963 0d0a 2020   atmospheric..  
-0002a2b0: 2320 2063 6f72 7265 6374 696f 6e20 6170  #  correction ap
-0002a2c0: 7072 6f61 6368 2066 6f72 204d 4f44 4953  proach for MODIS
-0002a2d0: 206f 6365 616e 2063 6f6c 6f72 2064 6174   ocean color dat
-0002a2e0: 6120 7072 6f63 6573 7369 6e67 2e0d 0a20  a processing... 
-0002a2f0: 2023 2020 4f70 7469 6373 2045 7870 7265   #  Optics Expre
-0002a300: 7373 2c20 3135 2832 3429 2c20 3135 3732  ss, 15(24), 1572
-0002a310: 32e2 8093 3135 3733 332e 0d0a 0d0a 2020  2...15733.....  
-0002a320: 2320 4164 6420 7365 636f 6e64 6172 7920  # Add secondary 
-0002a330: 6669 6c74 6572 2075 7369 6e67 2067 7265  filter using gre
-0002a340: 656e 6e65 7373 2066 756e 6374 696f 6e20  enness function 
-0002a350: 6265 6c6f 770d 0a20 2069 6d61 6765 203d  below..  image =
-0002a360: 2069 6d61 6765 2e61 6464 4261 6e64 7328   image.addBands(
-0002a370: 486f 4361 6c63 4772 6565 6e6e 6573 7328  HoCalcGreenness(
-0002a380: 696d 6167 6529 290d 0a0d 0a20 2023 2041  image))....  # A
-0002a390: 7070 6c79 2061 6c67 6f72 6974 686d 2031  pply algorithm 1
-0002a3a0: 3a20 4234 202d 2031 2e30 332a 4235 0d0a  : B4 - 1.03*B5..
-0002a3b0: 2020 2362 6c6f 6f6d 3120 3d20 696d 6167    #bloom1 = imag
-0002a3c0: 652e 7365 6c65 6374 2827 6e69 7227 292e  e.select('nir').
-0002a3d0: 7375 6274 7261 6374 2869 6d61 6765 2e73  subtract(image.s
-0002a3e0: 656c 6563 7428 2773 7769 7231 2729 2e6d  elect('swir1').m
-0002a3f0: 756c 7469 706c 7928 312e 3033 2929 2e72  ultiply(1.03)).r
-0002a400: 656e 616d 6528 2762 6c6f 6f6d 3127 290d  ename('bloom1').
-0002a410: 0a0d 0a20 2023 2047 6574 2062 696e 6172  ...  # Get binar
-0002a420: 7920 696d 6167 6520 6279 2061 7070 6c79  y image by apply
-0002a430: 696e 6720 7468 6520 7468 7265 7368 6f6c  ing the threshol
-0002a440: 640d 0a20 2062 6c6f 6f6d 315f 6d61 736b  d..  bloom1_mask
-0002a450: 203d 2069 6d61 6765 2e73 656c 6563 7428   = image.select(
-0002a460: 2248 2229 2e6c 7465 2867 7265 656e 6573  "H").lte(greenes
-0002a470: 7354 6872 6573 686f 6c64 292e 7265 6e61  sThreshold).rena
-0002a480: 6d65 285b 2262 6c6f 6f6d 315f 6d61 736b  me(["bloom1_mask
-0002a490: 225d 290d 0a0d 0a0d 0a20 2072 6574 7572  "])......  retur
-0002a4a0: 6e20 696d 6167 655c 0d0a 2020 2020 2020  n image\..      
-0002a4b0: 2020 2020 2e61 6464 4261 6e64 7328 626c      .addBands(bl
-0002a4c0: 6f6f 6d31 295c 0d0a 2020 2020 2020 2020  oom1)\..        
-0002a4d0: 2020 2e61 6464 4261 6e64 7328 626c 6f6f    .addBands(bloo
-0002a4e0: 6d31 5f6d 6173 6b29 0d0a 0d0a 0d0a 0d0a  m1_mask)........
-0002a4f0: 0d0a 2320 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f  ..# ////////////
+00029d10: 2323 2323 2323 2323 0d0a 234a 6566 6620  ########..#Jeff 
+00029d20: 486f 204d 6574 686f 6420 666f 7220 616c  Ho Method for al
+00029d30: 6761 6c20 626c 6f6f 6d20 6465 7465 6374  gal bloom detect
+00029d40: 696f 6e0d 0a23 6874 7470 733a 2f2f 7777  ion..#https://ww
+00029d50: 772e 6e61 7475 7265 2e63 6f6d 2f61 7274  w.nature.com/art
+00029d60: 6963 6c65 732f 7334 3135 3836 2d30 3139  icles/s41586-019
+00029d70: 2d31 3634 382d 370d 0a0d 0a23 2053 696d  -1648-7....# Sim
+00029d80: 706c 6966 6965 6420 5363 7269 7074 2066  plified Script f
+00029d90: 6f72 204c 616e 6473 6174 2057 6174 6572  or Landsat Water
+00029da0: 2051 7561 6c69 7479 0d0a 2320 5072 6f64   Quality..# Prod
+00029db0: 7563 6573 2061 206d 6170 206f 6620 616e  uces a map of an
+00029dc0: 2061 6c67 616c 2062 6c6f 6f6d 2069 6e20   algal bloom in 
+00029dd0: 4c61 6b65 2045 7269 6520 6f6e 2032 3031  Lake Erie on 201
+00029de0: 312f 392f 330d 0a23 2043 7265 6174 6564  1/9/3..# Created
+00029df0: 206f 6e20 3132 2f37 2f32 3031 3520 6279   on 12/7/2015 by
+00029e00: 204a 6566 6620 486f 0d0a 0d0a 2320 5370   Jeff Ho....# Sp
+00029e10: 6563 6966 6965 7320 6120 7468 7265 7368  ecifies a thresh
+00029e20: 6f6c 6420 666f 7220 6875 6520 746f 2065  old for hue to e
+00029e30: 7374 696d 6174 6520 2267 7265 656e 2220  stimate "green" 
+00029e40: 7069 7865 6c73 0d0a 2320 7468 6973 2069  pixels..# this i
+00029e50: 7320 7573 6564 2061 7320 616e 2061 6464  s used as an add
+00029e60: 6974 696f 6e61 6c20 6669 6c74 6572 2074  itional filter t
+00029e70: 6f20 7265 6669 6e65 2074 6865 2061 6c67  o refine the alg
+00029e80: 6f72 6974 686d 2061 626f 7665 0d0a 6465  orithm above..de
+00029e90: 6620 486f 4361 6c63 4772 6565 6e6e 6573  f HoCalcGreennes
+00029ea0: 7328 696d 6729 3a0d 0a20 2023 6d61 7020  s(img):..  #map 
+00029eb0: 722c 2067 2c20 616e 6420 6220 666f 7220  r, g, and b for 
+00029ec0: 6d6f 7265 2072 6561 6461 626c 6520 616c  more readable al
+00029ed0: 6765 6272 6120 6265 6c6f 770d 0a20 2072  gebra below..  r
+00029ee0: 203d 2069 6d67 2e73 656c 6563 7428 5b27   = img.select(['
+00029ef0: 7265 6427 5d29 0d0a 2020 6720 3d20 696d  red'])..  g = im
+00029f00: 672e 7365 6c65 6374 285b 2767 7265 656e  g.select(['green
+00029f10: 275d 290d 0a20 2062 203d 2069 6d67 2e73  '])..  b = img.s
+00029f20: 656c 6563 7428 5b27 626c 7565 275d 290d  elect(['blue']).
+00029f30: 0a0d 0a20 2023 6361 6c63 756c 6174 6520  ...  #calculate 
+00029f40: 696e 7465 6e73 6974 792c 2068 7565 0d0a  intensity, hue..
+00029f50: 2020 4920 3d20 722e 6164 6428 6729 2e61    I = r.add(g).a
+00029f60: 6464 2862 292e 7265 6e61 6d65 285b 2749  dd(b).rename(['I
+00029f70: 275d 290d 0a20 206d 696e 7320 3d20 722e  '])..  mins = r.
+00029f80: 6d69 6e28 6729 2e6d 696e 2862 292e 7265  min(g).min(b).re
+00029f90: 6e61 6d65 285b 276d 696e 7327 5d29 0d0a  name(['mins'])..
+00029fa0: 2020 4820 3d20 6d69 6e73 2e77 6865 7265    H = mins.where
+00029fb0: 286d 696e 732e 6571 2872 292c 2862 2e73  (mins.eq(r),(b.s
+00029fc0: 7562 7472 6163 7428 7229 292e 6469 7669  ubtract(r)).divi
+00029fd0: 6465 2849 2e73 7562 7472 6163 7428 722e  de(I.subtract(r.
+00029fe0: 6d75 6c74 6970 6c79 2833 2929 292e 6164  multiply(3))).ad
+00029ff0: 6428 3129 2029 0d0a 2020 4820 3d20 482e  d(1) )..  H = H.
+0002a000: 7768 6572 6528 6d69 6e73 2e65 7128 6729  where(mins.eq(g)
+0002a010: 2c28 722e 7375 6274 7261 6374 2867 2929  ,(r.subtract(g))
+0002a020: 2e64 6976 6964 6528 492e 7375 6274 7261  .divide(I.subtra
+0002a030: 6374 2867 2e6d 756c 7469 706c 7928 3329  ct(g.multiply(3)
+0002a040: 2929 2e61 6464 2832 2920 290d 0a20 2048  )).add(2) )..  H
+0002a050: 203d 2048 2e77 6865 7265 286d 696e 732e   = H.where(mins.
+0002a060: 6571 2862 292c 2867 2e73 7562 7472 6163  eq(b),(g.subtrac
+0002a070: 7428 6229 292e 6469 7669 6465 2849 2e73  t(b)).divide(I.s
+0002a080: 7562 7472 6163 7428 622e 6d75 6c74 6970  ubtract(b.multip
+0002a090: 6c79 2833 2929 2920 290d 0a0d 0a20 2023  ly(3))) )....  #
+0002a0a0: 7069 7865 6c73 2077 6974 6820 6875 6520  pixels with hue 
+0002a0b0: 6265 6c6f 7720 312e 3620 6d6f 7265 206c  below 1.6 more l
+0002a0c0: 696b 656c 7920 746f 2062 6520 626c 6f6f  ikely to be bloo
+0002a0d0: 6d20 616e 6420 6e6f 7420 7375 7370 656e  m and not suspen
+0002a0e0: 6465 6420 7365 6469 6d65 6e74 0d0a 2020  ded sediment..  
+0002a0f0: 4874 6872 6573 6820 3d20 482e 6c74 6528  Hthresh = H.lte(
+0002a100: 312e 3629 0d0a 0d0a 2020 7265 7475 726e  1.6)....  return
+0002a110: 2048 2e72 656e 616d 6528 2748 2729 0d0a   H.rename('H')..
+0002a120: 0d0a 0d0a 2341 7070 6c79 2062 6c6f 6f6d  ....#Apply bloom
+0002a130: 2064 6574 6563 7469 6f6e 2061 6c67 6f72   detection algor
+0002a140: 6974 686d 0d0a 6465 6620 486f 4361 6c63  ithm..def HoCalc
+0002a150: 416c 676f 7269 7468 6d31 2869 6d61 6765  Algorithm1(image
+0002a160: 293a 0d0a 2020 7472 7565 636f 6c6f 7220  ):..  truecolor 
+0002a170: 3d20 3120 2373 686f 7720 7472 7565 2063  = 1 #show true c
+0002a180: 6f6c 6f72 2069 6d61 6765 2061 7320 7765  olor image as we
+0002a190: 6c6c 0d0a 2020 7465 7374 5468 7265 7368  ll..  testThresh
+0002a1a0: 203d 2046 616c 7365 2023 2061 6464 2061   = False # add a
+0002a1b0: 2062 696e 6172 7920 696d 6167 6520 636c   binary image cl
+0002a1c0: 6173 7369 6679 696e 6720 696e 746f 2022  assifying into "
+0002a1d0: 626c 6f6f 6d22 616e 6420 226e 6f6e 2d62  bloom"and "non-b
+0002a1e0: 6c6f 6f6d 0d0a 2020 626c 6f6f 6d54 6872  loom..  bloomThr
+0002a1f0: 6573 686f 6c64 203d 2030 2e30 3233 3436  eshold = 0.02346
+0002a200: 2023 7468 7265 7368 6f6c 6420 666f 7220   #threshold for 
+0002a210: 636c 6173 7369 6669 6361 7469 6f6e 2066  classification f
+0002a220: 6974 2062 6173 6564 206f 6e20 6f74 6865  it based on othe
+0002a230: 7220 6461 7461 0d0a 2020 6772 6565 6e65  r data..  greene
+0002a240: 7373 5468 7265 7368 6f6c 6420 3d20 312e  ssThreshold = 1.
+0002a250: 360d 0a0d 0a20 2023 2041 6c67 6f72 6974  6....  # Algorit
+0002a260: 686d 2031 2062 6173 6564 206f 6e3a 0d0a  hm 1 based on:..
+0002a270: 2020 2320 5761 6e67 2c20 4d2e 2c20 2620    # Wang, M., & 
+0002a280: 5368 692c 2057 2e20 2832 3030 3729 2e20  Shi, W. (2007). 
+0002a290: 5468 6520 4e49 522d 5357 4952 2063 6f6d  The NIR-SWIR com
+0002a2a0: 6269 6e65 6420 6174 6d6f 7370 6865 7269  bined atmospheri
+0002a2b0: 630d 0a20 2023 2020 636f 7272 6563 7469  c..  #  correcti
+0002a2c0: 6f6e 2061 7070 726f 6163 6820 666f 7220  on approach for 
+0002a2d0: 4d4f 4449 5320 6f63 6561 6e20 636f 6c6f  MODIS ocean colo
+0002a2e0: 7220 6461 7461 2070 726f 6365 7373 696e  r data processin
+0002a2f0: 672e 0d0a 2020 2320 204f 7074 6963 7320  g...  #  Optics 
+0002a300: 4578 7072 6573 732c 2031 3528 3234 292c  Express, 15(24),
+0002a310: 2031 3537 3232 e280 9331 3537 3333 2e0d   15722...15733..
+0002a320: 0a0d 0a20 2023 2041 6464 2073 6563 6f6e  ...  # Add secon
+0002a330: 6461 7279 2066 696c 7465 7220 7573 696e  dary filter usin
+0002a340: 6720 6772 6565 6e6e 6573 7320 6675 6e63  g greenness func
+0002a350: 7469 6f6e 2062 656c 6f77 0d0a 2020 696d  tion below..  im
+0002a360: 6167 6520 3d20 696d 6167 652e 6164 6442  age = image.addB
+0002a370: 616e 6473 2848 6f43 616c 6347 7265 656e  ands(HoCalcGreen
+0002a380: 6e65 7373 2869 6d61 6765 2929 0d0a 0d0a  ness(image))....
+0002a390: 2020 2320 4170 706c 7920 616c 676f 7269    # Apply algori
+0002a3a0: 7468 6d20 313a 2042 3420 2d20 312e 3033  thm 1: B4 - 1.03
+0002a3b0: 2a42 350d 0a20 2023 626c 6f6f 6d31 203d  *B5..  #bloom1 =
+0002a3c0: 2069 6d61 6765 2e73 656c 6563 7428 276e   image.select('n
+0002a3d0: 6972 2729 2e73 7562 7472 6163 7428 696d  ir').subtract(im
+0002a3e0: 6167 652e 7365 6c65 6374 2827 7377 6972  age.select('swir
+0002a3f0: 3127 292e 6d75 6c74 6970 6c79 2831 2e30  1').multiply(1.0
+0002a400: 3329 292e 7265 6e61 6d65 2827 626c 6f6f  3)).rename('bloo
+0002a410: 6d31 2729 0d0a 0d0a 2020 2320 4765 7420  m1')....  # Get 
+0002a420: 6269 6e61 7279 2069 6d61 6765 2062 7920  binary image by 
+0002a430: 6170 706c 7969 6e67 2074 6865 2074 6872  applying the thr
+0002a440: 6573 686f 6c64 0d0a 2020 626c 6f6f 6d31  eshold..  bloom1
+0002a450: 5f6d 6173 6b20 3d20 696d 6167 652e 7365  _mask = image.se
+0002a460: 6c65 6374 2822 4822 292e 6c74 6528 6772  lect("H").lte(gr
+0002a470: 6565 6e65 7373 5468 7265 7368 6f6c 6429  eenessThreshold)
+0002a480: 2e72 656e 616d 6528 5b22 626c 6f6f 6d31  .rename(["bloom1
+0002a490: 5f6d 6173 6b22 5d29 0d0a 0d0a 0d0a 2020  _mask"])......  
+0002a4a0: 7265 7475 726e 2069 6d61 6765 5c0d 0a20  return image\.. 
+0002a4b0: 2020 2020 2020 2020 202e 6164 6442 616e           .addBan
+0002a4c0: 6473 2862 6c6f 6f6d 3129 5c0d 0a20 2020  ds(bloom1)\..   
+0002a4d0: 2020 2020 2020 202e 6164 6442 616e 6473         .addBands
+0002a4e0: 2862 6c6f 6f6d 315f 6d61 736b 290d 0a0d  (bloom1_mask)...
+0002a4f0: 0a0d 0a0d 0a0d 0a23 202f 2f2f 2f2f 2f2f  .......# ///////
 0002a500: 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f  ////////////////
 0002a510: 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f  ////////////////
 0002a520: 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f  ////////////////
-0002a530: 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 0d0a  //////////////..
-0002a540: 2320 2f2f 2045 4e44 2046 554e 4354 494f  # // END FUNCTIO
-0002a550: 4e53 0d0a 2320 2f2f 2f2f 2f2f 2f2f 2f2f  NS..# //////////
+0002a530: 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f  ////////////////
+0002a540: 2f2f 2f0d 0a23 202f 2f20 454e 4420 4655  ///..# // END FU
+0002a550: 4e43 5449 4f4e 530d 0a23 202f 2f2f 2f2f  NCTIONS..# /////
 0002a560: 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f  ////////////////
 0002a570: 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f  ////////////////
 0002a580: 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f  ////////////////
 0002a590: 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f 2f2f  ////////////////
-0002a5a0: 2f2f 2f2f 2f2f 0d0a 0d0a 0d0a 7465 7374  //////......test
-0002a5b0: 4172 6561 7320 3d20 7b7d 3b0d 0a74 6573  Areas = {};..tes
-0002a5c0: 7441 7265 6173 5b27 434f 275d 203d 2065  tAreas['CO'] = e
-0002a5d0: 652e 4765 6f6d 6574 7279 2e50 6f6c 7967  e.Geometry.Polyg
-0002a5e0: 6f6e 280d 0a20 2020 2020 2020 205b 5b5b  on(..        [[[
-0002a5f0: 2d31 3038 2e32 3836 3330 3530 3930 3634  -108.28630509064
-0002a600: 3735 392c 2033 382e 3038 3533 3433 3633  759, 38.08534363
-0002a610: 3831 3230 3932 355d 2c0d 0a20 2020 2020  8120925],..     
-0002a620: 2020 2020 205b 2d31 3038 2e32 3836 3330       [-108.28630
-0002a630: 3530 3930 3634 3735 392c 2033 372e 3138  509064759, 37.18
-0002a640: 3035 3132 3230 3039 3239 3435 5d2c 0d0a  051220092945],..
-0002a650: 2020 2020 2020 2020 2020 5b2d 3130 362e            [-106.
-0002a660: 3734 3832 3139 3135 3331 3437 3539 2c20  74821915314759, 
-0002a670: 3337 2e31 3830 3531 3232 3030 3932 3934  37.1805122009294
-0002a680: 355d 2c0d 0a20 2020 2020 2020 2020 205b  5],..          [
-0002a690: 2d31 3036 2e37 3438 3231 3931 3533 3134  -106.74821915314
-0002a6a0: 3735 392c 2033 382e 3038 3533 3433 3633  759, 38.08534363
-0002a6b0: 3831 3230 3932 355d 5d5d 2c20 4e6f 6e65  8120925]]], None
-0002a6c0: 2c20 4661 6c73 6529 0d0a 7465 7374 4172  , False)..testAr
-0002a6d0: 6561 735b 2743 4f5f 4e6f 7274 6827 5d20  eas['CO_North'] 
-0002a6e0: 3d20 6565 2e47 656f 6d65 7472 792e 506f  = ee.Geometry.Po
-0002a6f0: 6c79 676f 6e28 0d0a 2020 2020 2020 2020  lygon(..        
-0002a700: 5b5b 5b2d 3130 362e 3431 3937 3738 3639  [[[-106.41977869
-0002a710: 3333 3935 3234 2c20 3430 2e39 3739 3437  339524, 40.97947
-0002a720: 3730 3233 3933 3233 345d 2c0d 0a20 2020  702393234],..   
-0002a730: 2020 2020 2020 205b 2d31 3036 2e34 3139         [-106.419
-0002a740: 3737 3836 3933 3339 3532 342c 2033 392e  77869339524, 39.
-0002a750: 3936 3430 3633 3231 3831 3430 3031 5d2c  96406321814001],
-0002a760: 0d0a 2020 2020 2020 2020 2020 5b2d 3130  ..          [-10
-0002a770: 352e 3230 3537 3839 3433 3535 3832 3734  5.20578943558274
-0002a780: 2c20 3339 2e39 3634 3036 3332 3138 3134  , 39.96406321814
-0002a790: 3030 315d 2c0d 0a20 2020 2020 2020 2020  001],..         
-0002a7a0: 205b 2d31 3035 2e32 3035 3738 3934 3335   [-105.205789435
-0002a7b0: 3538 3237 342c 2034 302e 3937 3934 3737  58274, 40.979477
-0002a7c0: 3032 3339 3332 3334 5d5d 5d2c 204e 6f6e  02393234]]], Non
-0002a7d0: 652c 2046 616c 7365 290d 0a74 6573 7441  e, False)..testA
-0002a7e0: 7265 6173 5b27 4341 275d 203d 6565 2e47  reas['CA'] =ee.G
-0002a7f0: 656f 6d65 7472 792e 506f 6c79 676f 6e28  eometry.Polygon(
-0002a800: 0d0a 2020 2020 2020 2020 5b5b 5b2d 3131  ..        [[[-11
-0002a810: 392e 3936 3338 3337 3630 3238 3735 3036  9.96383760287506
-0002a820: 2c20 3337 2e31 3338 3135 3035 3734 3130  , 37.13815057410
-0002a830: 3837 3134 5d2c 0d0a 2020 2020 2020 2020  8714],..        
-0002a840: 2020 5b2d 3131 392e 3936 3338 3337 3630    [-119.96383760
-0002a850: 3238 3735 3036 2c20 3336 2e34 3037 3734  287506, 36.40774
-0002a860: 3431 3231 3036 3432 345d 2c0d 0a20 2020  412106424],..   
-0002a870: 2020 2020 2020 205b 2d31 3137 2e39 3533         [-117.953
-0002a880: 3333 3935 3536 3030 3030 362c 2033 362e  33955600006, 36.
-0002a890: 3430 3737 3434 3132 3130 3634 3234 5d2c  40774412106424],
-0002a8a0: 0d0a 2020 2020 2020 2020 2020 5b2d 3131  ..          [-11
-0002a8b0: 372e 3935 3333 3339 3535 3630 3030 3036  7.95333955600006
-0002a8c0: 2c20 3337 2e31 3338 3135 3035 3734 3130  , 37.13815057410
-0002a8d0: 3837 3134 5d5d 5d2c 204e 6f6e 652c 2046  8714]]], None, F
-0002a8e0: 616c 7365 290d 0a0d 0a74 6573 7441 7265  alse)....testAre
-0002a8f0: 6173 5b27 4341 5f53 6d61 6c6c 275d 203d  as['CA_Small'] =
-0002a900: 2065 652e 4765 6f6d 6574 7279 2e50 6f6c   ee.Geometry.Pol
-0002a910: 7967 6f6e 280d 0a20 2020 2020 2020 205b  ygon(..        [
-0002a920: 5b5b 2d31 3233 2e32 3235 3636 3936 3833  [[-123.225669683
-0002a930: 3734 3632 352c 2033 392e 3637 3732 3039  74625, 39.677209
-0002a940: 3539 3932 3639 3135 355d 2c0d 0a20 2020  599269155],..   
-0002a950: 2020 2020 2020 205b 2d31 3233 2e32 3235         [-123.225
-0002a960: 3636 3936 3833 3734 3632 352c 2033 382e  66968374625, 38.
-0002a970: 3939 3331 3739 3530 3436 3937 3538 365d  993179504697586]
-0002a980: 2c0d 0a20 2020 2020 2020 2020 205b 2d31  ,..          [-1
-0002a990: 3232 2e36 3034 3934 3231 3434 3638 3337  22.6049421446837
-0002a9a0: 352c 2033 382e 3939 3331 3739 3530 3436  5, 38.9931795046
-0002a9b0: 3937 3538 365d 2c0d 0a20 2020 2020 2020  97586],..       
-0002a9c0: 2020 205b 2d31 3232 2e36 3034 3934 3231     [-122.6049421
-0002a9d0: 3434 3638 3337 352c 2033 392e 3637 3732  4468375, 39.6772
-0002a9e0: 3039 3539 3932 3639 3135 355d 5d5d 2c20  09599269155]]], 
-0002a9f0: 4e6f 6e65 2c20 4661 6c73 6529 0d0a 0d0a  None, False)....
-0002aa00: 7465 7374 4172 6561 735b 2748 4927 5d20  testAreas['HI'] 
-0002aa10: 3d20 6565 2e47 656f 6d65 7472 792e 506f  = ee.Geometry.Po
-0002aa20: 6c79 676f 6e28 0d0a 2020 2020 2020 2020  lygon(..        
-0002aa30: 5b5b 5b2d 3136 302e 3530 3832 3438 3734  [[[-160.50824874
-0002aa40: 3435 3035 3434 2c20 3232 2e36 3539 3831  450544, 22.65981
-0002aa50: 3435 3133 3930 3934 3734 5d2c 0d0a 2020  4513909474],..  
-0002aa60: 2020 2020 2020 2020 5b2d 3136 302e 3530          [-160.50
-0002aa70: 3832 3438 3734 3435 3035 3434 2c20 3138  824874450544, 18
-0002aa80: 2e35 3437 3530 3330 3939 3539 3832 375d  .54750309959827]
-0002aa90: 2c0d 0a20 2020 2020 2020 2020 205b 2d31  ,..          [-1
-0002aaa0: 3534 2e33 3535 3930 3439 3934 3530 3534  54.3559049945054
-0002aab0: 342c 2031 382e 3534 3735 3033 3039 3935  4, 18.5475030995
-0002aac0: 3938 3237 5d2c 0d0a 2020 2020 2020 2020  9827],..        
-0002aad0: 2020 5b2d 3135 342e 3335 3539 3034 3939    [-154.35590499
-0002aae0: 3435 3035 3434 2c20 3232 2e36 3539 3831  450544, 22.65981
-0002aaf0: 3435 3133 3930 3934 3734 5d5d 5d2c 204e  4513909474]]], N
-0002ab00: 6f6e 652c 2046 616c 7365 290d 0a         one, False)..
+0002a5a0: 2f2f 2f2f 2f2f 2f2f 2f2f 2f0d 0a0d 0a0d  ///////////.....
+0002a5b0: 0a74 6573 7441 7265 6173 203d 207b 7d3b  .testAreas = {};
+0002a5c0: 0d0a 7465 7374 4172 6561 735b 2743 4f27  ..testAreas['CO'
+0002a5d0: 5d20 3d20 6565 2e47 656f 6d65 7472 792e  ] = ee.Geometry.
+0002a5e0: 506f 6c79 676f 6e28 0d0a 2020 2020 2020  Polygon(..      
+0002a5f0: 2020 5b5b 5b2d 3130 382e 3238 3633 3035    [[[-108.286305
+0002a600: 3039 3036 3437 3539 2c20 3338 2e30 3835  09064759, 38.085
+0002a610: 3334 3336 3338 3132 3039 3235 5d2c 0d0a  343638120925],..
+0002a620: 2020 2020 2020 2020 2020 5b2d 3130 382e            [-108.
+0002a630: 3238 3633 3035 3039 3036 3437 3539 2c20  28630509064759, 
+0002a640: 3337 2e31 3830 3531 3232 3030 3932 3934  37.1805122009294
+0002a650: 355d 2c0d 0a20 2020 2020 2020 2020 205b  5],..          [
+0002a660: 2d31 3036 2e37 3438 3231 3931 3533 3134  -106.74821915314
+0002a670: 3735 392c 2033 372e 3138 3035 3132 3230  759, 37.18051220
+0002a680: 3039 3239 3435 5d2c 0d0a 2020 2020 2020  092945],..      
+0002a690: 2020 2020 5b2d 3130 362e 3734 3832 3139      [-106.748219
+0002a6a0: 3135 3331 3437 3539 2c20 3338 2e30 3835  15314759, 38.085
+0002a6b0: 3334 3336 3338 3132 3039 3235 5d5d 5d2c  343638120925]]],
+0002a6c0: 204e 6f6e 652c 2046 616c 7365 290d 0a74   None, False)..t
+0002a6d0: 6573 7441 7265 6173 5b27 434f 5f4e 6f72  estAreas['CO_Nor
+0002a6e0: 7468 275d 203d 2065 652e 4765 6f6d 6574  th'] = ee.Geomet
+0002a6f0: 7279 2e50 6f6c 7967 6f6e 280d 0a20 2020  ry.Polygon(..   
+0002a700: 2020 2020 205b 5b5b 2d31 3036 2e34 3139       [[[-106.419
+0002a710: 3737 3836 3933 3339 3532 342c 2034 302e  77869339524, 40.
+0002a720: 3937 3934 3737 3032 3339 3332 3334 5d2c  97947702393234],
+0002a730: 0d0a 2020 2020 2020 2020 2020 5b2d 3130  ..          [-10
+0002a740: 362e 3431 3937 3738 3639 3333 3935 3234  6.41977869339524
+0002a750: 2c20 3339 2e39 3634 3036 3332 3138 3134  , 39.96406321814
+0002a760: 3030 315d 2c0d 0a20 2020 2020 2020 2020  001],..         
+0002a770: 205b 2d31 3035 2e32 3035 3738 3934 3335   [-105.205789435
+0002a780: 3538 3237 342c 2033 392e 3936 3430 3633  58274, 39.964063
+0002a790: 3231 3831 3430 3031 5d2c 0d0a 2020 2020  21814001],..    
+0002a7a0: 2020 2020 2020 5b2d 3130 352e 3230 3537        [-105.2057
+0002a7b0: 3839 3433 3535 3832 3734 2c20 3430 2e39  8943558274, 40.9
+0002a7c0: 3739 3437 3730 3233 3933 3233 345d 5d5d  7947702393234]]]
+0002a7d0: 2c20 4e6f 6e65 2c20 4661 6c73 6529 0d0a  , None, False)..
+0002a7e0: 7465 7374 4172 6561 735b 2743 4127 5d20  testAreas['CA'] 
+0002a7f0: 3d65 652e 4765 6f6d 6574 7279 2e50 6f6c  =ee.Geometry.Pol
+0002a800: 7967 6f6e 280d 0a20 2020 2020 2020 205b  ygon(..        [
+0002a810: 5b5b 2d31 3139 2e39 3633 3833 3736 3032  [[-119.963837602
+0002a820: 3837 3530 362c 2033 372e 3133 3831 3530  87506, 37.138150
+0002a830: 3537 3431 3038 3731 345d 2c0d 0a20 2020  574108714],..   
+0002a840: 2020 2020 2020 205b 2d31 3139 2e39 3633         [-119.963
+0002a850: 3833 3736 3032 3837 3530 362c 2033 362e  83760287506, 36.
+0002a860: 3430 3737 3434 3132 3130 3634 3234 5d2c  40774412106424],
+0002a870: 0d0a 2020 2020 2020 2020 2020 5b2d 3131  ..          [-11
+0002a880: 372e 3935 3333 3339 3535 3630 3030 3036  7.95333955600006
+0002a890: 2c20 3336 2e34 3037 3734 3431 3231 3036  , 36.40774412106
+0002a8a0: 3432 345d 2c0d 0a20 2020 2020 2020 2020  424],..         
+0002a8b0: 205b 2d31 3137 2e39 3533 3333 3935 3536   [-117.953339556
+0002a8c0: 3030 3030 362c 2033 372e 3133 3831 3530  00006, 37.138150
+0002a8d0: 3537 3431 3038 3731 345d 5d5d 2c20 4e6f  574108714]]], No
+0002a8e0: 6e65 2c20 4661 6c73 6529 0d0a 0d0a 7465  ne, False)....te
+0002a8f0: 7374 4172 6561 735b 2743 415f 536d 616c  stAreas['CA_Smal
+0002a900: 6c27 5d20 3d20 6565 2e47 656f 6d65 7472  l'] = ee.Geometr
+0002a910: 792e 506f 6c79 676f 6e28 0d0a 2020 2020  y.Polygon(..    
+0002a920: 2020 2020 5b5b 5b2d 3132 332e 3232 3536      [[[-123.2256
+0002a930: 3639 3638 3337 3436 3235 2c20 3339 2e36  6968374625, 39.6
+0002a940: 3737 3230 3935 3939 3236 3931 3535 5d2c  77209599269155],
+0002a950: 0d0a 2020 2020 2020 2020 2020 5b2d 3132  ..          [-12
+0002a960: 332e 3232 3536 3639 3638 3337 3436 3235  3.22566968374625
+0002a970: 2c20 3338 2e39 3933 3137 3935 3034 3639  , 38.99317950469
+0002a980: 3735 3836 5d2c 0d0a 2020 2020 2020 2020  7586],..        
+0002a990: 2020 5b2d 3132 322e 3630 3439 3432 3134    [-122.60494214
+0002a9a0: 3436 3833 3735 2c20 3338 2e39 3933 3137  468375, 38.99317
+0002a9b0: 3935 3034 3639 3735 3836 5d2c 0d0a 2020  9504697586],..  
+0002a9c0: 2020 2020 2020 2020 5b2d 3132 322e 3630          [-122.60
+0002a9d0: 3439 3432 3134 3436 3833 3735 2c20 3339  494214468375, 39
+0002a9e0: 2e36 3737 3230 3935 3939 3236 3931 3535  .677209599269155
+0002a9f0: 5d5d 5d2c 204e 6f6e 652c 2046 616c 7365  ]]], None, False
+0002aa00: 290d 0a0d 0a74 6573 7441 7265 6173 5b27  )....testAreas['
+0002aa10: 4849 275d 203d 2065 652e 4765 6f6d 6574  HI'] = ee.Geomet
+0002aa20: 7279 2e50 6f6c 7967 6f6e 280d 0a20 2020  ry.Polygon(..   
+0002aa30: 2020 2020 205b 5b5b 2d31 3630 2e35 3038       [[[-160.508
+0002aa40: 3234 3837 3434 3530 3534 342c 2032 322e  24874450544, 22.
+0002aa50: 3635 3938 3134 3531 3339 3039 3437 345d  659814513909474]
+0002aa60: 2c0d 0a20 2020 2020 2020 2020 205b 2d31  ,..          [-1
+0002aa70: 3630 2e35 3038 3234 3837 3434 3530 3534  60.5082487445054
+0002aa80: 342c 2031 382e 3534 3735 3033 3039 3935  4, 18.5475030995
+0002aa90: 3938 3237 5d2c 0d0a 2020 2020 2020 2020  9827],..        
+0002aaa0: 2020 5b2d 3135 342e 3335 3539 3034 3939    [-154.35590499
+0002aab0: 3435 3035 3434 2c20 3138 2e35 3437 3530  450544, 18.54750
+0002aac0: 3330 3939 3539 3832 375d 2c0d 0a20 2020  309959827],..   
+0002aad0: 2020 2020 2020 205b 2d31 3534 2e33 3535         [-154.355
+0002aae0: 3930 3439 3934 3530 3534 342c 2032 322e  90499450544, 22.
+0002aaf0: 3635 3938 3134 3531 3339 3039 3437 345d  659814513909474]
+0002ab00: 5d5d 2c20 4e6f 6e65 2c20 4661 6c73 6529  ]], None, False)
+0002ab10: 0d0a                                     ..
```

### Comparing `geeViz-2023.4.1/geeViz/migrateGEEAssets.py` & `geeViz-2023.6.1/geeViz/migrateGEEAssets.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.4.1/geeViz/phEEnoViz.py` & `geeViz-2023.6.1/geeViz/phEEnoViz.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.4.1/geeViz/taskManagerLib.py` & `geeViz-2023.6.1/geeViz/taskManagerLib.py`

 * *Files identical despite different names*

### Comparing `geeViz-2023.4.1/geeViz.egg-info/PKG-INFO` & `geeViz-2023.6.1/geeViz.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: geeViz
-Version: 2023.4.1
+Version: 2023.6.1
 Summary: A package to help with GEE data processing, analysis, and visualization
 Home-page: https://github.com/gee-community/geeViz
 Author: Ian Housman
 Author-email: ian.housman@gmail.com
 License: Apache
 Keywords: earthengine google remote sensing landsat sentinel modis forestry forest
-Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `geeViz-2023.4.1/geeViz.egg-info/SOURCES.txt` & `geeViz-2023.6.1/geeViz.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 LICENSE
 README.md
 setup.py
 geeViz/__init__.py
 geeViz/assetManagerLib.py
 geeViz/changeDetectionLib.py
+geeViz/foliumView.py
 geeViz/gcpLib.py
+geeViz/gee2Pandas.py
 geeViz/geeView.py
 geeViz/getImagesLib.py
 geeViz/migrateGEEAssets.py
 geeViz/phEEnoViz.py
 geeViz/taskManagerLib.py
 geeViz.egg-info/PKG-INFO
 geeViz.egg-info/SOURCES.txt
@@ -21,27 +23,31 @@
 geeViz/examples/GFSTimeLapse.py
 geeViz/examples/LANDTRENDRViz.py
 geeViz/examples/LANDTRENDRWrapper.py
 geeViz/examples/LANDTRENDRWrapperNotebook.ipynb
 geeViz/examples/LCMAP_and_LCMS_Viewer.py
 geeViz/examples/LCMAP_and_LCMS_Viewer_Notebook.ipynb
 geeViz/examples/__init__.py
+geeViz/examples/foliumViewerExample.py
+geeViz/examples/gee2PandasExample.ipynb
 geeViz/examples/geeViewExample.py
 geeViz/examples/geeViewExampleNotebook.ipynb
+geeViz/examples/geeViewVSFoliumViewerExampleNotebook.ipynb
 geeViz/examples/getClimateWrapper.py
 geeViz/examples/getCombinedLandsatSentinel2Wrapper.py
 geeViz/examples/getLandsatWrapper.py
 geeViz/examples/getLandsatWrapperNotebook.ipynb
 geeViz/examples/getSentinel2Wrapper.py
 geeViz/examples/harmonicRegressionWrapper.py
 geeViz/examples/lcmsViewerExample.py
 geeViz/examples/lcmsViewerExampleNotebook.ipynb
 geeViz/examples/phEEnoVizWrapper.py
 geeViz/examples/taskTrackerExample.py
 geeViz/examples/timeLapseExample.py
+geeViz/geeView/foliumView.html
 geeViz/geeView/index.html
 geeViz/geeView/css/style.min.css
 geeViz/geeView/images/EE-logo-150.png
 geeViz/geeView/images/GEE.png
 geeViz/geeView/images/GEE_logo_transparent.png
 geeViz/geeView/images/RCR-logo.jpg
 geeViz/geeView/images/Thumbs.db
```

### Comparing `geeViz-2023.4.1/setup.py` & `geeViz-2023.6.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,18 +45,17 @@
     long_description_content_type="text/markdown",
     url="https://github.com/gee-community/geeViz",
     # packages=setuptools.find_packages(),
     packages=packages,
     package_data=package_data,
     
     classifiers=[
-        "Programming Language :: Python :: 2",
         'Programming Language :: Python :: 3',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: Apache Software License',
         "Operating System :: OS Independent",
         'Development Status :: 4 - Beta'
     ],
-    install_requires=['earthengine-api','oauth2client','pandas','matplotlib','IPython','requests'],
+    install_requires=['earthengine-api','oauth2client','pandas','matplotlib','IPython','requests','folium','simpledbf'],
     # data_files = [('gee-py-viz',data_files)],
 
 )
```

