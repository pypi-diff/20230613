# Comparing `tmp/pepe-granular-1.0.0.tar.gz` & `tmp/pepe-granular-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pepe-granular-1.0.0.tar", last modified: Tue May 31 18:49:55 2022, max compression
+gzip compressed data, was "pepe-granular-1.1.0.tar", last modified: Tue Jun 13 13:36:33 2023, max compression
```

## Comparing `pepe-granular-1.0.0.tar` & `pepe-granular-1.1.0.tar`

### file list

```diff
@@ -1,65 +1,67 @@
-drwxr-xr-x   0 jack      (1000) jack      (1000)        0 2022-05-31 18:49:55.000000 pepe-granular-1.0.0/
--rw-r--r--   0 jack      (1000) jack      (1000)     1057 2022-01-28 15:24:49.000000 pepe-granular-1.0.0/LICENSE.md
--rw-r--r--   0 jack      (1000) jack      (1000)     3491 2022-05-31 18:49:55.000000 pepe-granular-1.0.0/PKG-INFO
--rw-r--r--   0 jack      (1000) jack      (1000)     3014 2022-05-31 18:49:08.000000 pepe-granular-1.0.0/README.md
-drwxr-xr-x   0 jack      (1000) jack      (1000)        0 2022-05-31 18:49:55.000000 pepe-granular-1.0.0/pepe/
--rw-r--r--   0 jack      (1000) jack      (1000)     3914 2022-05-31 18:43:02.000000 pepe-granular-1.0.0/pepe/__init__.py
-drwxr-xr-x   0 jack      (1000) jack      (1000)        0 2022-05-31 18:49:55.000000 pepe-granular-1.0.0/pepe/analysis/
--rw-r--r--   0 jack      (1000) jack      (1000)     6078 2022-04-18 18:38:44.000000 pepe-granular-1.0.0/pepe/analysis/BrightnessGSquared.py
--rwxr-xr-x   0 jack      (1000) jack      (1000)     9765 2022-04-18 18:39:34.000000 pepe-granular-1.0.0/pepe/analysis/D2Min.py
--rw-r--r--   0 jack      (1000) jack      (1000)      565 2022-05-17 14:03:58.000000 pepe-granular-1.0.0/pepe/analysis/Derivative.py
--rw-r--r--   0 jack      (1000) jack      (1000)     7633 2022-05-17 14:03:58.000000 pepe-granular-1.0.0/pepe/analysis/ForceBalance.py
--rw-r--r--   0 jack      (1000) jack      (1000)    59691 2022-05-31 18:08:14.000000 pepe-granular-1.0.0/pepe/analysis/ForceSolve.py
--rw-r--r--   0 jack      (1000) jack      (1000)     3095 2022-05-17 14:03:58.000000 pepe-granular-1.0.0/pepe/analysis/LinearRegions.py
--rw-r--r--   0 jack      (1000) jack      (1000)     5046 2022-03-22 18:56:11.000000 pepe-granular-1.0.0/pepe/analysis/NetworkAnalysis.py
--rw-r--r--   0 jack      (1000) jack      (1000)      343 2022-05-17 14:03:58.000000 pepe-granular-1.0.0/pepe/analysis/__init__.py
-drwxr-xr-x   0 jack      (1000) jack      (1000)        0 2022-05-31 18:49:55.000000 pepe-granular-1.0.0/pepe/auto/
--rw-r--r--   0 jack      (1000) jack      (1000)    54739 2022-05-31 18:08:14.000000 pepe-granular-1.0.0/pepe/auto/ForceSolve.py
--rw-r--r--   0 jack      (1000) jack      (1000)     2190 2022-04-18 18:42:19.000000 pepe-granular-1.0.0/pepe/auto/ParameterSelect.py
--rw-r--r--   0 jack      (1000) jack      (1000)    16958 2022-05-31 18:12:43.000000 pepe-granular-1.0.0/pepe/auto/TrialObject.py
--rw-r--r--   0 jack      (1000) jack      (1000)      184 2022-05-17 14:03:58.000000 pepe-granular-1.0.0/pepe/auto/__init__.py
-drwxr-xr-x   0 jack      (1000) jack      (1000)        0 2022-05-31 18:49:55.000000 pepe-granular-1.0.0/pepe/preprocess/
--rw-r--r--   0 jack      (1000) jack      (1000)     5019 2022-04-18 18:45:54.000000 pepe-granular-1.0.0/pepe/preprocess/Filter.py
--rw-r--r--   0 jack      (1000) jack      (1000)     4470 2022-04-18 18:45:31.000000 pepe-granular-1.0.0/pepe/preprocess/Image.py
--rw-r--r--   0 jack      (1000) jack      (1000)     9022 2022-04-18 18:46:12.000000 pepe-granular-1.0.0/pepe/preprocess/Mask.py
--rw-r--r--   0 jack      (1000) jack      (1000)     6658 2022-04-18 18:47:36.000000 pepe-granular-1.0.0/pepe/preprocess/Rescale.py
--rw-r--r--   0 jack      (1000) jack      (1000)      144 2022-04-18 18:28:39.000000 pepe-granular-1.0.0/pepe/preprocess/__init__.py
-drwxr-xr-x   0 jack      (1000) jack      (1000)        0 2022-05-31 18:49:55.000000 pepe-granular-1.0.0/pepe/simulate/
--rw-r--r--   0 jack      (1000) jack      (1000)     9062 2022-04-18 18:47:58.000000 pepe-granular-1.0.0/pepe/simulate/SyntheticPE.py
--rw-r--r--   0 jack      (1000) jack      (1000)      120 2022-04-18 18:29:31.000000 pepe-granular-1.0.0/pepe/simulate/__init__.py
-drwxr-xr-x   0 jack      (1000) jack      (1000)        0 2022-05-31 18:49:55.000000 pepe-granular-1.0.0/pepe/test/
--rw-r--r--   0 jack      (1000) jack      (1000)       71 2022-05-17 14:03:58.000000 pepe-granular-1.0.0/pepe/test/__init__.py
--rw-r--r--   0 jack      (1000) jack      (1000)      558 2022-05-17 14:03:58.000000 pepe-granular-1.0.0/pepe/test/test_auto.py
--rw-r--r--   0 jack      (1000) jack      (1000)     4646 2022-04-12 15:46:00.000000 pepe-granular-1.0.0/pepe/test/test_utils.py
-drwxr-xr-x   0 jack      (1000) jack      (1000)        0 2022-05-31 18:49:55.000000 pepe-granular-1.0.0/pepe/topology/
--rw-r--r--   0 jack      (1000) jack      (1000)    28704 2022-04-18 18:48:53.000000 pepe-granular-1.0.0/pepe/topology/PersistentHomology.py
--rw-r--r--   0 jack      (1000) jack      (1000)       80 2022-04-18 18:30:58.000000 pepe-granular-1.0.0/pepe/topology/__init__.py
-drwxr-xr-x   0 jack      (1000) jack      (1000)        0 2022-05-31 18:49:55.000000 pepe-granular-1.0.0/pepe/tracking/
--rw-r--r--   0 jack      (1000) jack      (1000)     3881 2022-04-18 18:49:13.000000 pepe-granular-1.0.0/pepe/tracking/AngularConvolution.py
--rw-r--r--   0 jack      (1000) jack      (1000)       87 2022-04-18 18:49:58.000000 pepe-granular-1.0.0/pepe/tracking/CNNDetection.py
--rw-r--r--   0 jack      (1000) jack      (1000)    34680 2022-04-18 18:49:25.000000 pepe-granular-1.0.0/pepe/tracking/Convolution.py
--rw-r--r--   0 jack      (1000) jack      (1000)      746 2022-05-17 14:03:58.000000 pepe-granular-1.0.0/pepe/tracking/DTypes.py
--rw-r--r--   0 jack      (1000) jack      (1000)     5538 2022-04-18 18:49:45.000000 pepe-granular-1.0.0/pepe/tracking/Hough.py
--rw-r--r--   0 jack      (1000) jack      (1000)      193 2022-05-17 14:03:58.000000 pepe-granular-1.0.0/pepe/tracking/__init__.py
-drwxr-xr-x   0 jack      (1000) jack      (1000)        0 2022-05-31 18:49:55.000000 pepe-granular-1.0.0/pepe/utils/
--rw-r--r--   0 jack      (1000) jack      (1000)     1990 2022-04-18 18:50:41.000000 pepe-granular-1.0.0/pepe/utils/Coordinates.py
--rw-r--r--   0 jack      (1000) jack      (1000)     1763 2022-04-18 18:51:01.000000 pepe-granular-1.0.0/pepe/utils/FittingFunctions.py
--rw-r--r--   0 jack      (1000) jack      (1000)      823 2022-04-18 18:51:21.000000 pepe-granular-1.0.0/pepe/utils/Kwargs.py
--rw-r--r--   0 jack      (1000) jack      (1000)      709 2022-04-18 18:51:47.000000 pepe-granular-1.0.0/pepe/utils/Outer.py
--rw-r--r--   0 jack      (1000) jack      (1000)      466 2022-04-18 18:52:10.000000 pepe-granular-1.0.0/pepe/utils/Parse.py
--rw-r--r--   0 jack      (1000) jack      (1000)    14666 2022-05-31 18:08:14.000000 pepe-granular-1.0.0/pepe/utils/RectArr.py
--rw-r--r--   0 jack      (1000) jack      (1000)    14319 2022-05-31 18:08:14.000000 pepe-granular-1.0.0/pepe/utils/Sort.py
--rw-r--r--   0 jack      (1000) jack      (1000)      273 2022-04-18 18:33:14.000000 pepe-granular-1.0.0/pepe/utils/__init__.py
-drwxr-xr-x   0 jack      (1000) jack      (1000)        0 2022-05-31 18:49:55.000000 pepe-granular-1.0.0/pepe/visualize/
--rw-r--r--   0 jack      (1000) jack      (1000)     2234 2022-05-17 14:03:58.000000 pepe-granular-1.0.0/pepe/visualize/Circles.py
--rw-r--r--   0 jack      (1000) jack      (1000)     5620 2022-04-18 18:53:52.000000 pepe-granular-1.0.0/pepe/visualize/Colors.py
--rw-r--r--   0 jack      (1000) jack      (1000)     6942 2022-04-18 18:54:06.000000 pepe-granular-1.0.0/pepe/visualize/Forces.py
--rw-r--r--   0 jack      (1000) jack      (1000)     2092 2022-04-18 18:54:20.000000 pepe-granular-1.0.0/pepe/visualize/Rotation.py
--rw-r--r--   0 jack      (1000) jack      (1000)     1879 2022-04-18 18:38:25.000000 pepe-granular-1.0.0/pepe/visualize/__init__.py
-drwxr-xr-x   0 jack      (1000) jack      (1000)        0 2022-05-31 18:49:55.000000 pepe-granular-1.0.0/pepe_granular.egg-info/
--rw-r--r--   0 jack      (1000) jack      (1000)     3491 2022-05-31 18:49:55.000000 pepe-granular-1.0.0/pepe_granular.egg-info/PKG-INFO
--rw-r--r--   0 jack      (1000) jack      (1000)     1325 2022-05-31 18:49:55.000000 pepe-granular-1.0.0/pepe_granular.egg-info/SOURCES.txt
--rw-r--r--   0 jack      (1000) jack      (1000)        1 2022-05-31 18:49:55.000000 pepe-granular-1.0.0/pepe_granular.egg-info/dependency_links.txt
--rw-r--r--   0 jack      (1000) jack      (1000)        5 2022-05-31 18:49:55.000000 pepe-granular-1.0.0/pepe_granular.egg-info/top_level.txt
--rw-r--r--   0 jack      (1000) jack      (1000)       38 2022-05-31 18:49:55.000000 pepe-granular-1.0.0/setup.cfg
--rw-r--r--   0 jack      (1000) jack      (1000)      688 2022-05-31 18:45:49.000000 pepe-granular-1.0.0/setup.py
+drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-06-13 13:36:33.262053 pepe-granular-1.1.0/
+-rw-rw-r--   0 jack      (1000) jack      (1000)     1057 2023-06-01 02:53:33.000000 pepe-granular-1.1.0/LICENSE.md
+-rw-rw-r--   0 jack      (1000) jack      (1000)     3494 2023-06-13 13:36:33.262053 pepe-granular-1.1.0/PKG-INFO
+-rw-rw-r--   0 jack      (1000) jack      (1000)     2978 2023-06-13 13:34:32.000000 pepe-granular-1.1.0/README.md
+drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-06-13 13:36:33.262053 pepe-granular-1.1.0/pepe/
+-rw-rw-r--   0 jack      (1000) jack      (1000)     3860 2023-06-13 13:34:09.000000 pepe-granular-1.1.0/pepe/__init__.py
+drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-06-13 13:36:33.262053 pepe-granular-1.1.0/pepe/analysis/
+-rw-rw-r--   0 jack      (1000) jack      (1000)     6078 2023-06-01 02:53:33.000000 pepe-granular-1.1.0/pepe/analysis/BrightnessGSquared.py
+-rwxrwxr-x   0 jack      (1000) jack      (1000)     9765 2023-06-01 02:53:33.000000 pepe-granular-1.1.0/pepe/analysis/D2Min.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)      565 2023-06-01 02:53:33.000000 pepe-granular-1.1.0/pepe/analysis/Derivative.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     7633 2023-06-01 02:53:33.000000 pepe-granular-1.1.0/pepe/analysis/ForceBalance.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)    59695 2023-06-13 13:11:53.000000 pepe-granular-1.1.0/pepe/analysis/ForceSolve.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     3095 2023-06-01 02:53:33.000000 pepe-granular-1.1.0/pepe/analysis/LinearRegions.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     5046 2023-06-01 02:53:33.000000 pepe-granular-1.1.0/pepe/analysis/NetworkAnalysis.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)      343 2023-06-01 02:53:33.000000 pepe-granular-1.1.0/pepe/analysis/__init__.py
+drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-06-13 13:36:33.262053 pepe-granular-1.1.0/pepe/auto/
+-rw-rw-r--   0 jack      (1000) jack      (1000)    55624 2023-06-02 06:12:46.000000 pepe-granular-1.1.0/pepe/auto/ForceSolve.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     2190 2023-06-01 02:53:33.000000 pepe-granular-1.1.0/pepe/auto/ParameterSelect.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)    17216 2023-06-01 02:53:33.000000 pepe-granular-1.1.0/pepe/auto/TrialObject.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)      184 2023-06-01 02:53:33.000000 pepe-granular-1.1.0/pepe/auto/__init__.py
+drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-06-13 13:36:33.262053 pepe-granular-1.1.0/pepe/preprocess/
+-rw-rw-r--   0 jack      (1000) jack      (1000)     5019 2023-06-01 02:53:33.000000 pepe-granular-1.1.0/pepe/preprocess/Filter.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     4470 2023-06-01 02:53:33.000000 pepe-granular-1.1.0/pepe/preprocess/Image.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     9022 2023-06-02 13:54:48.000000 pepe-granular-1.1.0/pepe/preprocess/Mask.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     8840 2023-06-02 13:07:59.000000 pepe-granular-1.1.0/pepe/preprocess/Rescale.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)      144 2023-06-01 02:53:33.000000 pepe-granular-1.1.0/pepe/preprocess/__init__.py
+drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-06-13 13:36:33.262053 pepe-granular-1.1.0/pepe/simulate/
+-rw-rw-r--   0 jack      (1000) jack      (1000)     9091 2023-06-13 13:11:53.000000 pepe-granular-1.1.0/pepe/simulate/SyntheticPE.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)      120 2023-06-01 02:53:33.000000 pepe-granular-1.1.0/pepe/simulate/__init__.py
+drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-06-13 13:36:33.262053 pepe-granular-1.1.0/pepe/test/
+-rw-rw-r--   0 jack      (1000) jack      (1000)       71 2023-06-01 02:53:33.000000 pepe-granular-1.1.0/pepe/test/__init__.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)      614 2023-06-02 06:48:52.000000 pepe-granular-1.1.0/pepe/test/test_auto.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     1566 2023-06-02 13:33:29.000000 pepe-granular-1.1.0/pepe/test/test_conv_tracking.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     4590 2023-06-13 13:30:30.000000 pepe-granular-1.1.0/pepe/test/test_synthetic_force_solve.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     4646 2023-06-02 06:48:53.000000 pepe-granular-1.1.0/pepe/test/test_utils.py
+drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-06-13 13:36:33.262053 pepe-granular-1.1.0/pepe/topology/
+-rw-rw-r--   0 jack      (1000) jack      (1000)    28704 2023-06-01 02:53:33.000000 pepe-granular-1.1.0/pepe/topology/PersistentHomology.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)       80 2023-06-01 02:53:33.000000 pepe-granular-1.1.0/pepe/topology/__init__.py
+drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-06-13 13:36:33.262053 pepe-granular-1.1.0/pepe/tracking/
+-rw-rw-r--   0 jack      (1000) jack      (1000)     3881 2023-06-01 02:53:33.000000 pepe-granular-1.1.0/pepe/tracking/AngularConvolution.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)       87 2023-06-01 02:53:33.000000 pepe-granular-1.1.0/pepe/tracking/CNNDetection.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)    27865 2023-06-02 06:39:09.000000 pepe-granular-1.1.0/pepe/tracking/Convolution.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)      746 2023-06-01 02:53:33.000000 pepe-granular-1.1.0/pepe/tracking/DTypes.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     5538 2023-06-01 02:53:33.000000 pepe-granular-1.1.0/pepe/tracking/Hough.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)      193 2023-06-01 02:53:33.000000 pepe-granular-1.1.0/pepe/tracking/__init__.py
+drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-06-13 13:36:33.262053 pepe-granular-1.1.0/pepe/utils/
+-rw-rw-r--   0 jack      (1000) jack      (1000)     1990 2023-06-01 02:53:33.000000 pepe-granular-1.1.0/pepe/utils/Coordinates.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     1763 2023-06-01 02:53:33.000000 pepe-granular-1.1.0/pepe/utils/FittingFunctions.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)      823 2023-06-01 02:53:33.000000 pepe-granular-1.1.0/pepe/utils/Kwargs.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)      709 2023-06-01 02:53:33.000000 pepe-granular-1.1.0/pepe/utils/Outer.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)      466 2023-06-01 02:53:33.000000 pepe-granular-1.1.0/pepe/utils/Parse.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)    14666 2023-06-01 02:53:33.000000 pepe-granular-1.1.0/pepe/utils/RectArr.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)    14363 2023-06-13 13:18:14.000000 pepe-granular-1.1.0/pepe/utils/Sort.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)      273 2023-06-01 02:53:33.000000 pepe-granular-1.1.0/pepe/utils/__init__.py
+drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-06-13 13:36:33.262053 pepe-granular-1.1.0/pepe/visualize/
+-rw-rw-r--   0 jack      (1000) jack      (1000)     2234 2023-06-01 02:53:33.000000 pepe-granular-1.1.0/pepe/visualize/Circles.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     5620 2023-06-01 02:53:33.000000 pepe-granular-1.1.0/pepe/visualize/Colors.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     6942 2023-06-01 02:53:33.000000 pepe-granular-1.1.0/pepe/visualize/Forces.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     2092 2023-06-01 02:53:33.000000 pepe-granular-1.1.0/pepe/visualize/Rotation.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     1879 2023-06-01 02:53:33.000000 pepe-granular-1.1.0/pepe/visualize/__init__.py
+drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2023-06-13 13:36:33.262053 pepe-granular-1.1.0/pepe_granular.egg-info/
+-rw-rw-r--   0 jack      (1000) jack      (1000)     3494 2023-06-13 13:36:33.000000 pepe-granular-1.1.0/pepe_granular.egg-info/PKG-INFO
+-rw-rw-r--   0 jack      (1000) jack      (1000)     1397 2023-06-13 13:36:33.000000 pepe-granular-1.1.0/pepe_granular.egg-info/SOURCES.txt
+-rw-rw-r--   0 jack      (1000) jack      (1000)        1 2023-06-13 13:36:33.000000 pepe-granular-1.1.0/pepe_granular.egg-info/dependency_links.txt
+-rw-rw-r--   0 jack      (1000) jack      (1000)        5 2023-06-13 13:36:33.000000 pepe-granular-1.1.0/pepe_granular.egg-info/top_level.txt
+-rw-rw-r--   0 jack      (1000) jack      (1000)       38 2023-06-13 13:36:33.262053 pepe-granular-1.1.0/setup.cfg
+-rw-rw-r--   0 jack      (1000) jack      (1000)      747 2023-06-13 13:33:12.000000 pepe-granular-1.1.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pepe-granular-1.0.0/LICENSE.md` & `pepe-granular-1.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pepe-granular-1.0.0/PKG-INFO` & `pepe-granular-1.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: pepe-granular
-Version: 1.0.0
+Version: 1.1.0
 Summary: Toolbox for granular analysis of photoelastic images
 Home-page: https://jfeatherstone.github.io/pepe/pepe
 Author: Jack Featherstone
-Author-email: jdfeathe@ncsu.edu
+Author-email: jack.featherstone@oist.jp
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # Photoelastic Python Environment
 
-<ins>P</ins>hoto<ins>e</ins>lastic
-<ins>P</ins>ython
-<ins>E</ins>nvironment
+<u>P</u>hoto-
+<u>e</u>lastic
+<u>P</u>ython
+<u>E</u>nvironment
 
-This is a collection of tools for working with photoelastic particle images, including common analysis methods like particle tracking, force solving, and trajectory identification.
+This is a collection of tools for working with photoelastic particle images, including common analysis methods like particle tracking and community analysis.
 
 ## Features
 
 - Common analysis techniques (G<sup>2</sup>, D<sup>2</sup>min, etc.)
 - Particle tracking
 - Masking and other preprocessing tools
 - Synthetic photoelastic response generation
@@ -47,15 +48,15 @@
 
 ## Documentation
 
 Available [here](http://jfeatherstone.github.io/pepe/pepe).
 
 ## Requirements
 
-Python 3.7 is the recommended version to use, with the following packages:
+Python 3.11 is the recommended version to use, with the following packages:
 
 - [numpy](https://numpy.org/)
 - [matplotlib](https://matplotlib.org/)
 - [lmfit](https://lmfit.github.io/lmfit-py/index.html)
 - [scikit-learn](https://scikit-learn.org/stable/)
 - [opencv](https://opencv.org/)
 - [Pillow](https://pillow.readthedocs.io/en/stable/)
@@ -83,9 +84,7 @@
 [1a] Jonathan Kollmer's implementation in Matlab: https://github.com/jekollmer/PEGS
 
 [1b] Olivier Lantsoght's implementation in Python: https://git.immc.ucl.ac.be/olantsoght/pegs_py
 
 [2] Abed Zadeh, A., Barés, J., Brzinski, T. A., Daniels, K. E., Dijksman, J., Docquier, N., Everitt, H. O., Kollmer, J. E., Lantsoght, O., Wang, D., Workamp, M., Zhao, Y., & Zheng, H. (2019). Enlightening force chains: A review of photoelasticimetry in granular matter. Granular Matter, 21(4), 83. https://doi.org/10.1007/s10035-019-0942-2
 
 [3] Photoelastic methods wiki. https://git-xen.lmgc.univ-montp2.fr/PhotoElasticity/Main/-/wikis/home
-
-
```

### Comparing `pepe-granular-1.0.0/README.md` & `pepe-granular-1.1.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Photoelastic Python Environment
 
-<ins>P</ins>hoto<ins>e</ins>lastic
-<ins>P</ins>ython
-<ins>E</ins>nvironment
+<u>P</u>hoto-
+<u>e</u>lastic
+<u>P</u>ython
+<u>E</u>nvironment
 
-This is a collection of tools for working with photoelastic particle images, including common analysis methods like particle tracking, force solving, and trajectory identification.
+This is a collection of tools for working with photoelastic particle images, including common analysis methods like particle tracking and community analysis.
 
 ## Features
 
 - Common analysis techniques (G<sup>2</sup>, D<sup>2</sup>min, etc.)
 - Particle tracking
 - Masking and other preprocessing tools
 - Synthetic photoelastic response generation
@@ -32,15 +33,15 @@
 
 ## Documentation
 
 Available [here](http://jfeatherstone.github.io/pepe/pepe).
 
 ## Requirements
 
-Python 3.7 is the recommended version to use, with the following packages:
+Python 3.11 is the recommended version to use, with the following packages:
 
 - [numpy](https://numpy.org/)
 - [matplotlib](https://matplotlib.org/)
 - [lmfit](https://lmfit.github.io/lmfit-py/index.html)
 - [scikit-learn](https://scikit-learn.org/stable/)
 - [opencv](https://opencv.org/)
 - [Pillow](https://pillow.readthedocs.io/en/stable/)
```

### Comparing `pepe-granular-1.0.0/pepe/__init__.py` & `pepe-granular-1.1.0/pepe/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 ```
 git clone https://github.com/Jfeatherstone/pepe
 cd pepe
 pip install .
 ```
 
-Theoretically, this should work for any Python >3, but Python 3.7 is the recommended version (primarily because OpenCV has some issues with newer versions).
+Theoretically, this should work for any Python >3, but Python 3.7 and 3.11 have been explicitly tested.
 
 Dependencies:
 
 - [numpy](https://numpy.org/)
 - [matplotlib](https://matplotlib.org/)
 - [lmfit](https://lmfit.github.io/lmfit-py/index.html)
 - [scikit-learn](https://scikit-learn.org/stable/)
@@ -70,14 +70,13 @@
 
 [2] Daniels, K. E., Kollmer, J. E., & Puckett, J. G. (2017). Photoelastic force measurements in granular materials. Review of Scientific Instruments, 88(5), 051808. https://doi.org/10.1063/1.4983049
 
 [2a] Jonathan Kollmer's implementation in Matlab: https://github.com/jekollmer/PEGS
 
 [2b] Olivier Lantsoght's implementation in Python: https://git.immc.ucl.ac.be/olantsoght/pegs_py
 
-
 [3] Photoelastic methods wiki. https://git-xen.lmgc.univ-montp2.fr/PhotoElasticity/Main/-/wikis/home
 """
 
-__version__ = '1.0.0'
+__version__ = '1.1.0'
 __author__ = 'Jack Featherstone'
 __credits__ = 'North Carolina State University'
```

### Comparing `pepe-granular-1.0.0/pepe/analysis/BrightnessGSquared.py` & `pepe-granular-1.1.0/pepe/analysis/BrightnessGSquared.py`

 * *Files identical despite different names*

### Comparing `pepe-granular-1.0.0/pepe/analysis/D2Min.py` & `pepe-granular-1.1.0/pepe/analysis/D2Min.py`

 * *Files identical despite different names*

### Comparing `pepe-granular-1.0.0/pepe/analysis/Derivative.py` & `pepe-granular-1.1.0/pepe/analysis/Derivative.py`

 * *Files identical despite different names*

### Comparing `pepe-granular-1.0.0/pepe/analysis/ForceBalance.py` & `pepe-granular-1.1.0/pepe/analysis/ForceBalance.py`

 * *Files identical despite different names*

### Comparing `pepe-granular-1.0.0/pepe/analysis/ForceSolve.py` & `pepe-granular-1.1.0/pepe/analysis/ForceSolve.py`

 * *Files 0% similar despite different names*

```diff
@@ -517,15 +517,15 @@
         realScaleFactor = 1/float(int(1/imageScaleFactor))
         scaledImage = downsample(realImage, int(1/imageScaleFactor))
     else:
         scaledImage = realImage
         realScaleFactor = 1
 
     scaledRadius = np.int64(radius * realScaleFactor)
-    scaledCenter = np.array(center * realScaleFactor, dtype=np.int64)
+    scaledCenter = np.array(center * realScaleFactor, dtype=np.float64)
     scaledPxPerMeter = np.int64(pxPerMeter * realScaleFactor)
     scaledContactMaskRadius = np.int64(contactMaskRadius * realScaleFactor)
     scaledParticleArea = scaledRadius**2 * np.pi
 
     # Setup our function based on what parameters we are fitting
     # We want to avoid any if statements within the function itself, since
     # that will be evaluated many many times.
@@ -828,16 +828,16 @@
         Slope found via linear regression to convert average g^2 to force.
     """
 
     # The magnitude of the forces that will be acting at each step
     forceValues = np.linspace(forceBounds[0], forceBounds[1], forceSteps)
     gSqrAvgArr = np.zeros(forceSteps)
 
-    imageSize = (np.int16(radius*2)+11, np.int16(radius*2)+11)
-    center = np.array([imageSize[0]/2, imageSize[1]/2], dtype=np.int64)
+    imageSize = (np.int64(radius*2)+11, np.int64(radius*2)+11)
+    center = np.array([imageSize[0]/2, imageSize[1]/2], dtype=np.float64)
     particleMask = circularMask(imageSize, center, radius - g2Padding)[:,:,0]
 
     # The contact mask is a circle placed over the edge of the particle where the force is applied
     #contactMask1 = circularMask(imageSize,
     #                            np.array([imageSize[0]/2 + radius*np.cos(betaArr[0]), imageSize[1]/2 + radius*np.sin(betaArr[0])]),
     #                            contactMaskRadius)[:,:,0]
```

### Comparing `pepe-granular-1.0.0/pepe/analysis/LinearRegions.py` & `pepe-granular-1.1.0/pepe/analysis/LinearRegions.py`

 * *Files identical despite different names*

### Comparing `pepe-granular-1.0.0/pepe/analysis/NetworkAnalysis.py` & `pepe-granular-1.1.0/pepe/analysis/NetworkAnalysis.py`

 * *Files identical despite different names*

### Comparing `pepe-granular-1.0.0/pepe/auto/ForceSolve.py` & `pepe-granular-1.1.0/pepe/auto/ForceSolve.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,34 +50,42 @@
             "brightfield": bool,
             "contactPadding": int,
             "g2MaskPadding": int,
             "contactMaskRadius": int,
             "peBlurKernel": int,
             "requireForceBalance": bool,
             "circleTrackingChannel": int,
+            "circleTrackingGain": float,
             "circleTrackingKwargs": dict,
             "photoelasticChannel": int,
+            "photoelasticGain": float,
             "optimizationKwargs": dict,
             "maxBetaDisplacement": float,
             "forceNoiseWidth": float,
             "alphaNoiseWidth": float,
             "saveMovie": bool,
             "pickleArrays": bool,
             "outputRootFolder": str,
             "outputExtension": str,
             "genFitReport": bool,
             "performOptimization": bool,
             "inputSettingsFile": str,
             "debug": bool}
 
+# These dtypes don't matter, so we don't need to carry them
+# through the settings file, but we want to explicitly define
+# them so that the test function in pepe/test/test_auto.py
+# doesn't catch them as missing
+excludedArgs = ["progressBarOffset", "progressBarTitle"]
+
 # Decorator that allows us to identify which keyword arguments were explicitly
 # passed to the function, and which were left as default values. See beginning
 # of method code for more information/motivation.
 @explicitKwargs()
-def forceSolve(imageDirectory, guessRadius=0.0, fSigma=0.0, pxPerMeter=0.0, brightfield=True, contactPadding=15, g2MaskPadding=2, contactMaskRadius=30, lightCorrectionImage=None, lightCorrectionHorizontalMask=None, lightCorrectionVerticalMask=None, g2CalibrationImage=None, g2CalibrationCutoffFactor=.9, maskImage=None, cropXMin=None, cropXMax=None, peBlurKernel=3, imageExtension='bmp', requireForceBalance=False, imageStartIndex=None, imageEndIndex=None, carryOverAlpha=True, carryOverForce=True, circleDetectionMethod='convolution', circleTrackingKwargs={}, circleTrackingChannel=0, maxBetaDisplacement=.5, photoelasticChannel=1, forceNoiseWidth=.03, alphaNoiseWidth=.01, optimizationKwargs={}, performOptimization=True, debug=False, showProgressBar=True, progressBarOffset=0, progressBarTitle=None, saveMovie=False, outputRootFolder='./', inputSettingsFile=None, pickleArrays=True, genFitReport=True, outputExtension=''):
+def forceSolve(imageDirectory, guessRadius=0.0, fSigma=0.0, pxPerMeter=0.0, brightfield=True, contactPadding=15, g2MaskPadding=2, contactMaskRadius=30, lightCorrectionImage=None, lightCorrectionHorizontalMask=None, lightCorrectionVerticalMask=None, g2CalibrationImage=None, g2CalibrationCutoffFactor=.9, maskImage=None, cropXMin=None, cropXMax=None, peBlurKernel=3, imageExtension='bmp', requireForceBalance=False, imageStartIndex=None, imageEndIndex=None, carryOverAlpha=True, carryOverForce=True, circleDetectionMethod='convolution', circleTrackingKwargs={}, circleTrackingChannel=0, circleTrackingGain=1., maxBetaDisplacement=.5, photoelasticChannel=1, photoelasticGain=1., forceNoiseWidth=.03, alphaNoiseWidth=.01, optimizationKwargs={}, performOptimization=True, debug=False, showProgressBar=True, progressBarOffset=0, progressBarTitle=None, saveMovie=False, outputRootFolder='./', inputSettingsFile=None, pickleArrays=True, genFitReport=True, outputExtension=''):
     """
     Complete pipeline to solve for forces and particle positions for all image files
     in a directory. Results will be returned and potentially written to various files.
     See `Returns` section for more information
 
     Expects all particles to be the same (or very similar) sizes. This assumption is made
     by the calculation of the gradient squared calibration value, which is computed just
@@ -207,23 +215,29 @@
 
         See `pepe.tracking.convCircle()` and `pepe.tracking.houghCircle()` for more information.
 
     circleTrackingChannel : int
         The channel of the image that will be used to track the particles. `0` for red, `1` for
         green, and `2` for blue.
 
+    circleTrackingGain : float
+        The gain applied to the intensity in the circle tracking channel.
+
     maxBetaDisplacement : float
         The maximum distance (angle) that a force can move between frames and still be identified
         as the same force. If a force moves more than this value, it will still be recorded as a force,
         but will be considered a new and independent force from any of the ones in the previous frame.
 
     photoelasticChannel : int
         The channel of the image that will be used to gauge the photoelastic response. `0` for red, `1` for
         green, and `2` for blue.
 
+    photoelasticGain : float
+        The gain applied to the intensity in the photoelastic channel.
+
     forceNoiseWidth : float or None
         The width of the gaussian distribution (centered at 0) that noise is sampled from to add to the
         force guesses (potentially from the previous frame). This is done to avoid getting stuck in a local
         minimum for too long (adds some Monte-Carlo-esque behavior to the solving).
 
     alphaNoiseWidth : float or None
         The width of the gaussian distribution (centered at 0) that noise is sampled from to add to the
@@ -347,15 +361,17 @@
                 "brightfield": brightfield,
                 "contactPadding": contactPadding,
                 "g2MaskPadding": g2MaskPadding,
                 "contactMaskRadius": contactMaskRadius,
                 "peBlurKernel": peBlurKernel,
                 "requireForceBalance": requireForceBalance,
                 "circleTrackingChannel": circleTrackingChannel,
+                "circleTrackingGain": circleTrackingGain,
                 "photoelasticChannel": photoelasticChannel,
+                "photoelasticGain": photoelasticGain,
                 "maxBetaDisplacement": maxBetaDisplacement,
                 "forceNoiseWidth": forceNoiseWidth,
                 "alphaNoiseWidth": alphaNoiseWidth,
                 "showProgressBar": showProgressBar,
                 "saveMovie": saveMovie,
                 "pickleArrays": pickleArrays,
                 "outputRootFolder": outputRootFolder,
@@ -449,14 +465,17 @@
     # error messages (and we have another one of these below)
     if len(imageFiles) < 1:
         print(f'Error: directory {imageDirectory} contains no files!')
         return None
 
     imageFiles = np.sort([img for img in imageFiles if img[-len(settings["imageExtension"]):] == settings["imageExtension"]])
 
+    # DEBUG:
+    #imageFiles = imageFiles[::-1]
+
     # We have to do the end index first, so it doesn't mess up the start one
     if settings["imageEndIndex"] is not None:
         imageFiles = imageFiles[:min(settings["imageEndIndex"], len(imageFiles))]
 
     if settings["imageStartIndex"] is not None:
         imageFiles = imageFiles[max(settings["imageStartIndex"], 0):]
 
@@ -528,17 +547,17 @@
 
     # Calculate the lowest g2 value that we care about, so we can throw everything
     # that is below that away when solving (optional)
     checkMinG2 = False
     if settings["g2CalibrationImage"] is not None:
         g2CalImage = checkImageType(settings["g2CalibrationImage"])[:,xB[0]:xB[1]]
 
-        g2CalPEImage = cv2.blur((g2CalImage[:,:,settings["photoelasticChannel"]] + peCorrection).astype(np.float64) / 255, (settings["peBlurKernel"],settings["peBlurKernel"]))
+        g2CalPEImage = cv2.blur(settings["photoelasticGain"]*(g2CalImage[:,:,settings["photoelasticChannel"]] + peCorrection).astype(np.float64) / 255, (settings["peBlurKernel"],settings["peBlurKernel"]))
         # Locate particles
-        centers, radii = circFunc((g2CalImage[:,:,settings["circleTrackingChannel"]] + trackCorrection) * maskArr[:,:,0], settings["guessRadius"], **circleTrackingKwargs)
+        centers, radii = circFunc(settings["circleTrackingGain"]*(g2CalImage[:,:,settings["circleTrackingChannel"]] + trackCorrection) * maskArr[:,:,0], settings["guessRadius"], **circleTrackingKwargs)
         # There should only be 1 particle in the calibration image
         if len(centers) < 0:
             print(f'Warning: Gradient-squared calibration image does not contain any particles! Ignoring...')
         else:
             particleMask = circularMask(g2CalPEImage.shape, centers[0], radii[0])[:,:,0]
             gSqr = gSquared(g2CalPEImage)
             minParticleG2 = np.sum(gSqr * particleMask) / np.sum(particleMask) * settings["g2CalibrationCutoffFactor"]
@@ -574,26 +593,26 @@
 
     # The big loop that iterates over every image
     for i in range(len(imageFiles)):
 
         image = checkImageType(settings["imageDirectory"] + imageFiles[i])[:,xB[0]:xB[1]]
         # Convert to floats on the domain [0,1], so we can compare to the output of 
         # genSyntheticResponse()
-        peImage = cv2.blur((image[:,:,settings["photoelasticChannel"]] + peCorrection).astype(np.float64) / 255, (settings["peBlurKernel"],settings["peBlurKernel"]))
+        peImage = cv2.blur(settings["photoelasticGain"]*(image[:,:,settings["photoelasticChannel"]] + peCorrection).astype(np.float64) / 255, (settings["peBlurKernel"],settings["peBlurKernel"]))
 
         # -------------
         # Track circles
         # -------------
         start = time.perf_counter()
-        centers, radii = circFunc((image[:,:,settings["circleTrackingChannel"]] + trackCorrection) * maskArr[:,:,0], settings["guessRadius"], **circleTrackingKwargs)
+        centers, radii = circFunc(settings["circleTrackingGain"]*(image[:,:,settings["circleTrackingChannel"]] + trackCorrection) * maskArr[:,:,0], settings["guessRadius"], **circleTrackingKwargs)
 
         # We do some indexing using the centers/radii, so it is helpful
         # to have them as an integer type
-        centers = centers.astype(np.int64)
-        radii = radii.astype(np.int64)
+        #centers = centers.astype(np.int64)
+        #radii = radii.astype(np.int64)
 
         # We want to keep the order of particles constant, so we make sure
         # that they are (to whatever extent possible) in the same order
         # as the previous frame. This involves finding the closest neighbor
         # from the previous frame.
         if len(centersArr) > 0:
             centerOrder = preserveOrderArgsort(centersArr[-1], centers, padMissingValues=False)
```

### Comparing `pepe-granular-1.0.0/pepe/auto/ParameterSelect.py` & `pepe-granular-1.1.0/pepe/auto/ParameterSelect.py`

 * *Files identical despite different names*

### Comparing `pepe-granular-1.0.0/pepe/auto/TrialObject.py` & `pepe-granular-1.1.0/pepe/auto/TrialObject.py`

 * *Files 1% similar despite different names*

```diff
@@ -314,13 +314,16 @@
 
 
     def averageForcePositions(self, particleIndex):
         """
         Calculates the time-averaged beta values of forces for the provided
         particle.
         """
-        averageBetaArr = np.array([np.nanmean(self.betaArr[particleIndex][i,:]) for i in range(self.numForces[particleIndex])])
+        #averageBetaArr = np.array([np.nanmean(self.betaArr[particleIndex][i,:]) for i in range(self.numForces[particleIndex])])
+        averageBetaArr = np.array([np.nanmedian(self.betaArr[particleIndex][i,:]) for i in range(self.numForces[particleIndex])])
+        # Now correct for periodicity
+        #return np.array([ab if ab <= np.pi else ab - 2*np.pi for ab in averageBetaArr])
         return averageBetaArr
                                     
 
     def __str__(self):
         return self.datasetPath.split('/')[-2] if self.datasetPath is not None else super.__str__()
```

### Comparing `pepe-granular-1.0.0/pepe/preprocess/Filter.py` & `pepe-granular-1.1.0/pepe/preprocess/Filter.py`

 * *Files identical despite different names*

### Comparing `pepe-granular-1.0.0/pepe/preprocess/Image.py` & `pepe-granular-1.1.0/pepe/preprocess/Image.py`

 * *Files identical despite different names*

### Comparing `pepe-granular-1.0.0/pepe/preprocess/Mask.py` & `pepe-granular-1.1.0/pepe/preprocess/Mask.py`

 * *Files identical despite different names*

### Comparing `pepe-granular-1.0.0/pepe/preprocess/Rescale.py` & `pepe-granular-1.1.0/pepe/preprocess/Rescale.py`

 * *Files 20% similar despite different names*

```diff
@@ -50,15 +50,59 @@
 # For the upscale() method, we presumably are only doing a single operation,
 # but it is still good practice to hold onto the model we generate. So this
 # will be assigned to a proper model after the first call to upscale()
 defaultModelInstance = None
 defaultModelType = 'FSRCNN'
 defaultModelFactor = 2
 
+def modelInstallHelp():
+    helpString = f"""
+    Note that the super-resolution models need to be downloaded separately, as they are not
+    my own original work. Four methods are compatible with this package:
+
+    - [EDSR](https://arxiv.org/pdf/1707.02921.pdf) ([implementation](https://github.com/Saafke/EDSR_Tensorflow))
+
+    - [ESPCN](https://arxiv.org/abs/1609.05158) ([implementation](https://github.com/fannymonori/TF-ESPCN))
+
+    - [FSRCNN](http://mmlab.ie.cuhk.edu.hk/projects/FSRCNN.html) ([implementation](https://github.com/Saafke/FSRCNN_Tensorflow))
+
+    - [LapSRN](https://arxiv.org/abs/1710.01992) ([implementation](https://github.com/fannymonori/TF-LapSRN))
+
+    The above implementations are simply the ones that I have used in the past; there are certainly others available, which should give comparable results. I am not the creator of any of the above listed implementations either, nor am I associated in any way (other than as a user) with them.
+
+    To install any of the above models, you should place the `.pb` weight files into an appropriately named directory within the following folder:
+    {MODELS_DIR}.
+
+    e.g. directory structure:
+
+    ```
+    .../preprocess/
+        |-- Rescale.py
+        |-- ...
+        `-- models/
+            |-- FSRCNN/
+            |   |-- FSRCNN_x2.pb
+            |   |-- FSRCNN_x3.pb
+            |   `-- FSRCNN_x4.pb
+            `-- LapSRN/
+                |-- LapSRN_x2.pb
+                |-- LapSRN_x4.pb
+                `-- LapSRN_x8.pb
+    ```
+    Make sure that the naming conventions are consistent: the name of the directory should be the same as the first part of the weight file name, and the second part (separated by an underscore `_`) should be `x` plus the upsample factor. These conventions are important for the package to automatically detect which models are available.
+    """
+
+    print(helpString)
+
 def listSuperResModels(debug=False):
+
+    if not os.path.exists(MODELS_DIR):
+        print(f'Warning: models folder ({MODELS_DIR}) does not exist!\nSee pepe.preprocess.modelInstallHelp() for more information about installing models.')
+        return {}
+
     # Determine what models are available
     availableModels = [d for d in os.listdir(MODELS_DIR) if os.path.isdir(MODELS_DIR + d)]
     availableModels = np.sort(availableModels)
 
     modelFactors = {}
 
     # Now see which upscale factors are available for each model
@@ -76,15 +120,15 @@
         for wF in weightFiles:
             try:
                 # Cut off the extension, take the portion after the 'x', and cast to int
                 upscaleFactor = int(wF[:-3].split('x')[-1])
                 availableScalingFactors.append(upscaleFactor)
             except:
                 if debug:
-                    print(f'Warning: file \'{d}/{wF}\' does not conform to naming conventions.\nAll files should be named in the format <model_type>_x<upscale_factor>.pb!')
+                    print(f'Warning: file \'{d}/{wF}\' does not conform to naming conventions.\nAll files should be named in the format <model_type>_x<upscale_factor>.pb!\nSee pepe.preprocess.modelInstallHelp() for more information about installing models.')
 
         modelFactors[d] = list(np.sort(availableScalingFactors))
 
     return modelFactors
 
 
 def prepareSuperResModel(modelName, upscaleFactor):
```

### Comparing `pepe-granular-1.0.0/pepe/simulate/SyntheticPE.py` & `pepe-granular-1.1.0/pepe/simulate/SyntheticPE.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,19 +48,19 @@
         The number of pixels per meter for the simulated image. If not provided (or set to 1), the radius
         value will be assumed to already have been converted to meters.
 
     brightfield : bool
         Whether the intensity should be simulated as seen through a brightfield (True)
         polariscope or darkfield (False) polariscope.
 
-    imageSize : [int, int]
+    imageSize : tuple(np.int64[2]) or None
         The size of the canvas the stress pattern will be drawn on. Set to None to automatically
         determine this based on the radius.
 
-    center : [int, int]
+    center : np.float64[2] or None
         Where the center of the particle should be position in on the image canvas. Useful for
         creating a composite image of many particles, as the final image can be made just by
         adding each individual matrix together. Set to None to center the particle automatically.
 
     mask : np.uint8[H,W]
         Array of values representing which points, within the circle, to calculate the intensity
         for. Points with non-zero value represented desired points, and locations with value of
@@ -71,18 +71,18 @@
     """
 
     # Deal with parameters about the image
     # Note that it is very helpful to have an odd size, such that there is
     # a central pixel
     if imageSize is None:
         # 11 is arbitrary, just a small, odd number
-        imageSize = (np.int16(radius*2)+11, np.int16(radius*2)+11)
+        imageSize = (np.int64(radius*2)+11, np.int64(radius*2)+11)
 
     if center is None:
-        center = np.array([imageSize[0]/2, imageSize[1]/2], dtype=np.int64)
+        center = np.array([imageSize[0]/2, imageSize[1]/2], dtype=np.float64)
 
     if mask is None:
         mask = circularMask(imageSize, center, radius)[:,:,0]
 
     # Create a mask representing the particle, to find the points we need
     # to simulate
     particleMask = circularMask(imageSize, center, radius)[:,:,0]
@@ -90,15 +90,15 @@
 
     # Normally we could just do this:
     #points = np.transpose(np.where(cMask > 0))
     # but numba doesn't quite like this way, so we have to be 
     # a little more creative
     fullMask = particleMask + mask
     whereIndices = np.where(fullMask > 1)
-    points = np.zeros((len(whereIndices[0]), 2), dtype=np.int16)
+    points = np.zeros((len(whereIndices[0]), 2), dtype=np.int64)
     # There is a chance that these indices are backwards, but
     # because we have rotational symmetry, it doesn't really matter...
     # BUT if there is ever some weird anisotropy bug or something,
     # try switching these indices
     points[:,0] = whereIndices[0]
     points[:,1] = whereIndices[1]
```

### Comparing `pepe-granular-1.0.0/pepe/test/test_auto.py` & `pepe-granular-1.1.0/pepe/test/test_auto.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import inspect
 import numpy as np
 
-from pepe.auto import forceSolve, forceSolveArgDTypes
+from pepe.auto import forceSolve, forceSolveArgDTypes, excludedArgs
 
 def test_forceSolve_DTypeCoverage():
     """
     Make sure that all of the dtypes for the arguments in
     pepe.auto.forceSolve are defined for the purpose of
     reading in values from a settings file.
     """
     args, counts= np.unique(list(inspect.signature(forceSolve).parameters.keys()) + list(forceSolveArgDTypes.keys()), return_counts=True) 
-    missingArgs = args[counts == 1]
-
+    missingArgs = [a for a in args[counts == 1] if a not in excludedArgs]
+    
     assert len(missingArgs) == 0, f"Missing data types for args: {missingArgs}"
```

### Comparing `pepe-granular-1.0.0/pepe/test/test_utils.py` & `pepe-granular-1.1.0/pepe/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `pepe-granular-1.0.0/pepe/topology/PersistentHomology.py` & `pepe-granular-1.1.0/pepe/topology/PersistentHomology.py`

 * *Files identical despite different names*

### Comparing `pepe-granular-1.0.0/pepe/tracking/AngularConvolution.py` & `pepe-granular-1.1.0/pepe/tracking/AngularConvolution.py`

 * *Files identical despite different names*

### Comparing `pepe-granular-1.0.0/pepe/tracking/Convolution.py` & `pepe-granular-1.1.0/pepe/tracking/Convolution.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 from scipy.fft import fft2, ifft2
 
 from pepe.preprocess import circularMask, rectMask
 from pepe.topology import findPeaks2D
 from pepe.utils import lorentzian
 from pepe.analysis import adjacencyMatrix
 
-from lmfit import minimize, Parameters
+from lmfit import minimize, Parameters, fit_report
 
-def convCircle(singleChannelFrame, radius, radiusTolerance=None, offscreenParticles=False, outlineOnly=False, outlineThickness=.05, negativeHalo=False, haloThickness=.03, negativeInside=False, peakDownsample=10, minPeakPrevalence=.1, intensitySoftmax=1.2, intensitySoftmin=.1, invert=False, allowOverlap=False, fitPeaks=True, debug=False):
+def convCircle(singleChannelFrame, radius, radiusTolerance=None, offscreenParticles=False, kernelBlurKernel=3, outlineOnly=False, outlineThickness=.05, negativeHalo=False, haloThickness=.03, negativeInside=False, peakDownsample=10, minPeakPrevalence=.1, intensitySoftmax=1.2, intensitySoftmin=.1, invert=False, allowOverlap=False, fitPeaks=True, debug=False):
     """
     Perform convolution circle detection on the provided image.
 
     A brief description of the technique is described below; for
     a more comprehensive discussion, see [1].
 
     The convolution method identifies circles in an image by convolving
@@ -217,15 +217,15 @@
         #else:
         #    imageArr[255 - imageArr <= softmin] = 0
 
     # Calculate convolution
     convArr = circularKernelFind(imageArr, initialRadius, fftPadding=int(initialRadius*paddingFactor),
                                  outlineOnly=outlineOnly, outlineThickness=outlineThickness,
                                  negativeHalo=negativeHalo, haloThickness=haloThickness,
-                                 negativeInside=negativeInside, debug=debug)
+                                 negativeInside=negativeInside, kernelBlurKernel=kernelBlurKernel, debug=debug)
 
     if debug:
         plt.show()
 
     # Downsample data by 5-10x and run peak detection
     downsampledConvArr = cv2.resize(cv2.blur(convArr, (peakDownsample,peakDownsample)), (0,0),
                                     fx=1/peakDownsample, fy=1/peakDownsample, interpolation=cv2.INTER_CUBIC)
@@ -284,146 +284,52 @@
             upsampledPosition = np.array([peakPositions[i][0]*peakDownsample, peakPositions[i][1]*peakDownsample])
             lorentzPositions[i] = upsampledPosition
 
     # Look around each peak to find the real peak in the full-resolution image
     refinedPeakPositions = []
     refinedRadii = []
 
-    localPadding = int(peakDownsample*1.5)
+    # To do this, we use a non-linear optimization scheme
     for i in range(len(peakPositions)):
-        # We want to vary the radius here as well, so we can maybe get a slightly more accurate result.
-        # Note that it is much more efficient to perform the kernel finding on a small image many times
-        # than to work on a large image just a few times. So we recalculate the kernel finding for each
-        # radii for each peak.
-        # TODO: This part is still WIP, because it doens't quite work correctly
-        if len(possibleRadii) > 1:
-            maximumValues = np.zeros(len(possibleRadii))
-            maximumPositions = np.zeros((len(possibleRadii), 2))
-
-            #upsampledPosition = np.array([peakPositions[i][0]*peakDownsample, peakPositions[i][1]*peakDownsample])
-            upsampledPosition = np.int16(lorentzPositions[i])
-            for j in range(len(possibleRadii)):
-                # This is the point in the real image (not the conv arr)
-                imagePadding = int(possibleRadii[j])
-                # Crop out the small area of the image that we are working with
-                localImage = imageArr[max(upsampledPosition[0]-imagePadding, 0):min(upsampledPosition[0]+imagePadding,imageArr.shape[0]-1),max(upsampledPosition[1]-imagePadding, 0):min(upsampledPosition[1]+imagePadding, imageArr.shape[1]-1)]
-
-                # Perform another convolution
-                # Don't need as much padding for this one, since we are quite sure the particle is somewhere
-                # near the center
-                localConvPadding = int(possibleRadii[j])
-                localConvArr = circularKernelFind(localImage, possibleRadii[j], fftPadding=localConvPadding,
-                                                  outlineOnly=outlineOnly, outlineThickness=outlineThickness,
-                                                  negativeHalo=negativeHalo, haloThickness=haloThickness,
-                                                  negativeInside=negativeInside, debug=False)
-                # Required if you set debug=True in above line
-                #plt.show()
-
-                # Add a *very* small weighting that favors circles closer to the center of the
-                # image. This is needed because otherwise the algorithm may place circles more
-                # offscreen than they actually are, because it would mean fewer pixels are included
-                # (since some are cropped off)
-                #Y = np.arange(localImage.shape[0]).reshape((localImage.shape[0], 1)) # Column vector
-                #X = np.arange(localImage.shape[1]).reshape((1, localImage.shape[1])) # Row vector
-                #localConvArr += 1e-3*np.exp(- ( (Y - localImage.shape[0]/2)**2 + (X - localImage.shape[1]/2)**2 ) / max(localImage.shape))
-
-                # Now setup a fit to this function
-                params = Parameters()
-
-                params.add('center_y', value=localImage.shape[0]/2, vary=True)
-                params.add('center_x', value=localImage.shape[1]/2, vary=True)
-                params.add('width', value=imagePadding, vary=True)
-                params.add('amp', value=np.max(localConvArr)/2, vary=True)
-                params.add('offset', value=np.mean(localConvArr), vary=True)
-                
-                try:
-                    result = minimize(objectiveFunction, params, args=[localConvArr], method='nelder', max_nfev=1000)
-                except:
-                    result = None
-                
-                if result is not None:
-                    realLocalMax = np.array([int(result.params["center_y"]), int(result.params["center_x"])])
-                else:
-                    realLocalMax = np.zeros(2)
-
-                #realLocalMax = np.unravel_index(np.argmax(localConvArr.flatten()), localConvArr.shape)
-                # We want to convert these back to real-space coordinates here
-                #maximumPositions[j] = upsampledPosition - realLocalMax - np.repeat(localConvPadding, 2)
-                maximumPositions[j,0] = upsampledPosition[0] - localConvArr.shape[0]/2 + realLocalMax[0]
-                maximumPositions[j,1] = upsampledPosition[1] - localConvArr.shape[1]/2 + realLocalMax[1]
-
-                # Need to convert to int16 since we might have negative values
-                pMask = circularMask(singleChannelFrame.shape, maximumPositions[j], possibleRadii[j])[:,:,0].astype(np.int16)
-
-                # The next couple if statements are for only doing an outline, adding a halo, removing the center, etc.
-                # If we only want the outline, we subtract another circular mask from the above one
-                if outlineOnly:
-                    # Should be 2 if negative inside is true, 1 otherwise
-                    negativeInsideFactor = 1 + int(negativeInside)
-                    if outlineThickness < 1:
-                        innerRadius = np.ceil((1 - outlineThickness) * possibleRadii[j])
-                    else:
-                        innerRadius = possibleRadii[j] - outlineThickness
-                        pMask -= negativeInsideFactor * circularMask(singleChannelFrame.shape, maximumPositions[j], innerRadius)[:,:,0]
-
-                    if negativeHalo:
-                        pMask = 2*pMask - (circularMask(singleChannelFrame.shape, maximumPositions[j], possibleRadii[j]+2)[:,:,0].astype(np.int16) - circularMask(singleChannelFrame.shape, maximumPositions[j], possibleRadii[j])[:,:,0].astype(np.int16))
-
-                elif negativeHalo:
-                    pMask = 2*pMask - circularMask(singleChannelFrame.shape, maximumPositions[j], possibleRadii[j]+2)[:,:,0].astype(np.int16)
-
-
-                if np.sum(pMask) == 0:
-                    maximumValues[j] = 0
-                else:
-                    maximumValues[j] = np.sum(singleChannelFrame * pMask) / np.sum(pMask)
-           
-            
 
-            # Noise can cause some slight variations in the maximum values making different
-            # radii give different maximum values, when they should give actually the same
-            # value (and then the largest one should be taken). We fix this by rounding
-            # after multiply by a large number. .5e3 was chosen by experimenting
+        costArr = []
 
-            maximumValues = [int(m*1e2) if not np.isnan(m) else 0 for m in maximumValues]
+        def refineObjectiveFunction(params):
+            kernelArr = genCircularKernel(np.array([params["y"].value, params["x"].value]), params["r"].value,
+                                          imageArr.shape, kernelBlurKernel, outlineOnly,
+                                          outlineThickness, negativeHalo, haloThickness, negativeInside)
 
-            #plt.plot(possibleRadii, maximumValues)
-            #plt.show()
+            # We are minimizing this function, so we need the cost to be negative
+            # (unless we have to invert the image)
+            costArr.append((np.sum(kernelArr * imageArr) / np.sum(kernelArr)) * (int(invert)*2 - 1))
+            return (np.sum(kernelArr * imageArr) / np.sqrt(np.sum(kernelArr))) * (int(invert)*2 - 1)
 
-            # Now save whichever on had the largest signal
-            # We want to sort the list backwards, because we want the largest possible radius
-            # that also gives the best value. If the radius is smaller than the actual one, you
-            # can end up with the same exact maximum value, since you are just cutting off extra
-            # parts of the circle.
-            refinedPeakPositions.append(tuple(maximumPositions[::-1][np.argmax(maximumValues[::-1])]))
-            refinedRadii.append(possibleRadii[::-1][np.argmax(maximumValues[::-1])])
+        params = Parameters()
 
-        else:
-            # Position of the peaks in the convolution image (NOT the real image)
-            upsampledPosition = np.int16(lorentzPositions[i])
+        params.add('y', value=lorentzPositions[i][0], min=lorentzPositions[i][0]-imageArr.shape[0]*.02, max=lorentzPositions[i][0]+imageArr.shape[0]*.02)
+        params.add('x', value=lorentzPositions[i][1], min=lorentzPositions[i][1]-imageArr.shape[1]*.02, max=lorentzPositions[i][1]+imageArr.shape[1]*.02)
+        # May or may not want to vary the radius
+        # Small tolerances on the radius are so that min != max
+        params.add('r', value=np.mean(possibleRadii), vary=(len(possibleRadii) > 1), max=np.max(possibleRadii)-.01, min=np.min(possibleRadii)+.01)
+
+        result = minimize(refineObjectiveFunction, params, method='powell', max_nfev=10000, options={"ftol": 1e-5, "xtol": 1e-5})
+
+        #print(fit_report(result))
+
+        if result is not None:
+            refinedPeakPositions.append([result.params["y"].value, result.params["x"].value])
+            refinedRadii.append(result.params["r"].value)
             
-            # We don't need to refine if we fit a peak, since that already did refine the
-            # position
-            if fitPeaks:
-                refinementOffset = 0
+            if debug:
+                plt.plot(costArr)
+                plt.show()
 
-            else:
-                # This just looks long because my naming is a little verbose
-                # + we also have to make sure we don't accidentally go off of the image
-                localRegion = convArr[max(upsampledPosition[0]-localPadding, 0):min(upsampledPosition[0]+localPadding,convArr.shape[0]-1),max(upsampledPosition[1]-localPadding, 0):min(upsampledPosition[1]+localPadding, convArr.shape[1]-1)]
-                # Find maximum intensity in small region around that position
-                realLocalMax = np.unravel_index(np.argmax(localRegion.flatten()), localRegion.shape)
-                # This is relative to the small region we just created, so we have to subtract off the bounds
-                # eg. if this local max was found to be in the center of the local image, that would mean
-                # that the original upsampled position was correct.
-                refinementOffset = realLocalMax - np.repeat(localPadding, 2)
-
-            # Now put everything together the coordinates of the circle in the original image
-            refinedPeakPositions.append(tuple(upsampledPosition + refinementOffset))
-            refinedRadii.append(initialRadius)
+        else:
+            refinedPeakPositions.append(lorentzPositions[i])
+            refinedRadii.append(np.mean(possibleRadii))
 
 
     # Now we (optionally) remove overlapping particles
     if not allowOverlap:
         # Calculate the contact matrix
         # negative contact padding because we don't want to remove particles that are
         # good but just close to each other
@@ -432,32 +338,17 @@
         # Locate all of the particles that are overlapping
         overlappingParticles = np.array([i for i in range(len(refinedPeakPositions)) if np.sum(adjMat[i,:]) > 0])
 
         # Now find how good of detections each of these is, and order them from worst to best.
         particleScores = np.zeros(len(overlappingParticles))
         for i in range(len(particleScores)):
             # Need to convert to int16 since we might have negative values
-            pMask = circularMask(singleChannelFrame.shape, refinedPeakPositions[i], refinedRadii[i])[:,:,0].astype(np.int16)
-
-            # The next couple if statements are for only doing an outline, adding a halo, removing the center, etc.
-            # If we only want the outline, we subtract another circular mask from the above one
-            if outlineOnly:
-                # Should be 2 if negative inside is true, 1 otherwise
-                negativeInsideFactor = 1 + int(negativeInside)
-                if outlineThickness < 1:
-                    innerRadius = np.ceil((1 - outlineThickness) * refinedRadii[i])
-                else:
-                    innerRadius = refinedRadii[i] - outlineThickness
-                    pMask -= negativeInsideFactor * circularMask(singleChannelFrame.shape, refinedPeakPositions[i], innerRadius)[:,:,0]
-
-                if negativeHalo:
-                    pMask = 2*pMask - (circularMask(singleChannelFrame.shape, refinedPeakPositions[i], refinedRadii[i]+2)[:,:,0].astype(np.int16) - circularMask(singleChannelFrame.shape, refinedPeakPositions[i], refinedRadii[i])[:,:,0].astype(np.int16))
-
-            elif negativeHalo:
-                pMask = 2*pMask - circularMask(singleChannelFrame.shape, refinedPeakPositions[i], refinedRadii[i]+2)[:,:,0].astype(np.int16)
+            pMask = genCircularKernel(refinedPeakPositions[i], refinedRadii[i],
+                                      singleChannelFrame.shape, kernelBlurKernel, outlineOnly,
+                                      outlineThickness, negativeHalo, haloThickness, negativeInside).astype(np.int16)
 
             if np.sum(pMask) > 0:
                 # I square-root the mask sum so that the particles at the edge don't
                 # always win out against actual particles
                 # TODO: This still doesn't give priority to particles on screen;
                 # need to figure out a way to do that
                 particleScores[i] = np.sum(singleChannelFrame * pMask) / np.sqrt(np.sum(pMask))
@@ -506,15 +397,15 @@
             ax3.add_artist(c)
 
         fig.tight_layout()
 
     return np.array(refinedPeakPositions), np.array(refinedRadii)
 
 
-def circularKernelFind(singleChannelFrame, radius, fftPadding, outlineOnly=False, outlineThickness=.05, negativeHalo=False, haloThickness=.03, negativeInside=False, paddingValue=None, debug=False):
+def circularKernelFind(singleChannelFrame, radius, fftPadding, kernelBlurKernel=3, outlineOnly=False, outlineThickness=.05, negativeHalo=False, haloThickness=.03, negativeInside=False, paddingValue=None, debug=False):
     """
     Calculate the convolution of a circular mask with an image,
     identifying likely locations of circles within the image. Adapted from
     method described in [1].
 
     To perform the convolution, we take the product of the fft of each the
     kernel and image, and then ifft the result to transform back to real space.
@@ -539,14 +430,18 @@
 
     fftPadding : int
         The amount of padding to add to each side of the image, to prevent the
         fft from having issues. A good choice is usually 1.5 times the radius,
         though, less padding can be used if circles are not expected to often
         be located near the edges.
 
+    kernelBlurKernel : int
+        The kernel size to use to blur the kernel that will be convolved with the image, in
+        pixels. A value of 0 or None will use the original kernel.
+
     outlineOnly : bool
         Whether to look for only a particle outline (True), or to look for a filled-in circle (False).
 
         See `outlineThickness`.
 
     outlineThickness : float or int
         Thickness of the particle outline in the kernel; only relevant if `outlineOnly=True`.
@@ -577,17 +472,14 @@
 
         `'sigmoid'` will create a smooth-ish transition to 0.
 
         Any float value will be inserted into every point.
 
     debug : bool
         Whether or not to plot various quantities of the calculation for inspection
-- `S`: Soft particles; shore hardness 40
-- `M`: Medium particles; shore hardness 50
-- `H`: Hard particles; shore hardness 60, thickness
         at the end of the evaluation.
 
     Returns
     -------
 
     chiSqr : np.ndarray[H,W]
         The convolution of the kernel with the image. Larger values represent
@@ -645,42 +537,17 @@
         paddedImageArr[fftPadding:-fftPadding,:fftPadding] = paddingValue
         paddedImageArr[fftPadding:-fftPadding,-fftPadding:] = paddingValue
 
     center = np.array([radius,radius])
     # To be able to properly convolute the kernel with the image, they have to
     # be the same size, so just just put our kernel into an array the same size
     # as the image (though most entries will just be zero)
-    kernelArr = circularMask(paddedImageArr.shape, center, radius)[:,:,0].astype(np.float64)
-   
-    # If we only want the outline, we subtract another circular mask from the above one
-    if outlineOnly:
-        # Should be 2 if negative inside is true, 1 otherwise
-        negativeInsideFactor = 1 + int(negativeInside)
-        if outlineThickness < 1:
-            innerRadius = np.ceil((1 - outlineThickness) * radius)
-        else:
-            innerRadius = radius - outlineThickness
-        
-        kernelArr = kernelArr - negativeInsideFactor * circularMask(paddedImageArr.shape, center, innerRadius)[:,:,0].astype(np.float64)
-
-        if negativeHalo:
-            if haloThickness < 1:
-                haloRadius = radius + np.ceil((1 - haloThickness) * radius)
-            else:
-                haloRadius = radius + haloThickness
-
-            kernelArr = 2*kernelArr - (circularMask(paddedImageArr.shape, center, haloRadius)[:,:,0].astype(np.float64) - circularMask(paddedImageArr.shape, center, radius)[:,:,0].astype(np.float64))
-
-    elif negativeHalo:
-        if haloThickness < 1:
-            haloRadius = np.ceil((1 + haloThickness) * radius)
-        else:
-            haloRadius = radius + haloThickness
-
-        kernelArr = 2*kernelArr - circularMask(paddedImageArr.shape, center, haloRadius)[:,:,0].astype(np.float64)
+    # See function below for more information on generating this kernel
+    kernelArr = genCircularKernel(center, radius, paddedImageArr.shape, kernelBlurKernel, outlineOnly,
+                                 outlineThickness, negativeHalo, haloThickness, negativeInside)
 
     # First convolutional term
     convTerm1 = ifft2(fft2(paddedImageArr**2) * fft2(kernelArr))
     # Trim padding
     convTerm1 = convTerm1[cropBounds[0]:cropBounds[1],cropBounds[0]:cropBounds[2]]
 
     # Second term is pretty easy since we choose our weight function to be our
@@ -716,7 +583,43 @@
         ax[3].imshow(chiSqr)
         ax[3].set_title('Real-space convolution (Re)')
 
         fig.tight_layout()
 
     return chiSqr
 
+
+def genCircularKernel(center, radius, imageShape, kernelBlurKernel=3, outlineOnly=False, outlineThickness=.05, negativeHalo=False, haloThickness=.03, negativeInside=False,):
+
+    kernelArr = circularMask(imageShape, center, radius)[:,:,0].astype(np.float64)
+
+    # If we only want the outline, we subtract another circular mask from the above one
+    if outlineOnly:
+        # Should be 2 if negative inside is true, 1 otherwise
+        negativeInsideFactor = 1 + int(negativeInside)
+        if outlineThickness < 1:
+            innerRadius = np.ceil((1 - outlineThickness) * radius)
+        else:
+            innerRadius = radius - outlineThickness
+        
+        kernelArr = kernelArr - negativeInsideFactor * circularMask(imageShape, center, innerRadius)[:,:,0].astype(np.float64)
+
+        if negativeHalo:
+            if haloThickness < 1:
+                haloRadius = radius + np.ceil((1 - haloThickness) * radius)
+            else:
+                haloRadius = radius + haloThickness
+
+            kernelArr = 2*kernelArr - (circularMask(imageShape, center, haloRadius)[:,:,0].astype(np.float64) - circularMask(imageShape, center, radius)[:,:,0].astype(np.float64))
+
+    elif negativeHalo:
+        if haloThickness < 1:
+            haloRadius = np.ceil((1 + haloThickness) * radius)
+        else:
+            haloRadius = radius + haloThickness
+
+        kernelArr = 2*kernelArr - circularMask(imageShape, center, haloRadius)[:,:,0].astype(np.float64)
+
+    if kernelBlurKernel is not None and kernelBlurKernel > 0:
+        kernelArr = cv2.blur(kernelArr, (kernelBlurKernel,kernelBlurKernel))
+
+    return kernelArr
```

### Comparing `pepe-granular-1.0.0/pepe/tracking/DTypes.py` & `pepe-granular-1.1.0/pepe/tracking/DTypes.py`

 * *Files identical despite different names*

### Comparing `pepe-granular-1.0.0/pepe/tracking/Hough.py` & `pepe-granular-1.1.0/pepe/tracking/Hough.py`

 * *Files identical despite different names*

### Comparing `pepe-granular-1.0.0/pepe/utils/Coordinates.py` & `pepe-granular-1.1.0/pepe/utils/Coordinates.py`

 * *Files identical despite different names*

### Comparing `pepe-granular-1.0.0/pepe/utils/FittingFunctions.py` & `pepe-granular-1.1.0/pepe/utils/FittingFunctions.py`

 * *Files identical despite different names*

### Comparing `pepe-granular-1.0.0/pepe/utils/Kwargs.py` & `pepe-granular-1.1.0/pepe/utils/Kwargs.py`

 * *Files identical despite different names*

### Comparing `pepe-granular-1.0.0/pepe/utils/Outer.py` & `pepe-granular-1.1.0/pepe/utils/Outer.py`

 * *Files identical despite different names*

### Comparing `pepe-granular-1.0.0/pepe/utils/RectArr.py` & `pepe-granular-1.1.0/pepe/utils/RectArr.py`

 * *Files identical despite different names*

### Comparing `pepe-granular-1.0.0/pepe/utils/Sort.py` & `pepe-granular-1.1.0/pepe/utils/Sort.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         The elements of `newValues` ordered according to proximity to the elements
         of `oldValues`.
     """
 
     # We already have preserveOrderArgsort written, so we can just wrap that
     order = preserveOrderArgsort(oldValues, newValues, padMissingValues, maxDistance, periodic, fillNanSpots)
 
-    dim = len(newValues[0])
+    dim = len(newValues[0]) if hasattr(newValues[0], '__iter__') else 1
 
     # Slightly different behavior for d=1 vs. d>1, since we don't want
     # an extra dimension nested in there if our data is 1d
     if dim == 1:
         return np.array([newValues[i] if i is not None else np.nan for i in order])
     else:
         return np.array([newValues[i] if i is not None else np.repeat(np.nan, dim) for i in order])
```

### Comparing `pepe-granular-1.0.0/pepe/visualize/Circles.py` & `pepe-granular-1.1.0/pepe/visualize/Circles.py`

 * *Files identical despite different names*

### Comparing `pepe-granular-1.0.0/pepe/visualize/Colors.py` & `pepe-granular-1.1.0/pepe/visualize/Colors.py`

 * *Files identical despite different names*

### Comparing `pepe-granular-1.0.0/pepe/visualize/Forces.py` & `pepe-granular-1.1.0/pepe/visualize/Forces.py`

 * *Files identical despite different names*

### Comparing `pepe-granular-1.0.0/pepe/visualize/Rotation.py` & `pepe-granular-1.1.0/pepe/visualize/Rotation.py`

 * *Files identical despite different names*

### Comparing `pepe-granular-1.0.0/pepe/visualize/__init__.py` & `pepe-granular-1.1.0/pepe/visualize/__init__.py`

 * *Files identical despite different names*

### Comparing `pepe-granular-1.0.0/pepe_granular.egg-info/PKG-INFO` & `pepe-granular-1.1.0/pepe_granular.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: pepe-granular
-Version: 1.0.0
+Version: 1.1.0
 Summary: Toolbox for granular analysis of photoelastic images
 Home-page: https://jfeatherstone.github.io/pepe/pepe
 Author: Jack Featherstone
-Author-email: jdfeathe@ncsu.edu
+Author-email: jack.featherstone@oist.jp
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # Photoelastic Python Environment
 
-<ins>P</ins>hoto<ins>e</ins>lastic
-<ins>P</ins>ython
-<ins>E</ins>nvironment
+<u>P</u>hoto-
+<u>e</u>lastic
+<u>P</u>ython
+<u>E</u>nvironment
 
-This is a collection of tools for working with photoelastic particle images, including common analysis methods like particle tracking, force solving, and trajectory identification.
+This is a collection of tools for working with photoelastic particle images, including common analysis methods like particle tracking and community analysis.
 
 ## Features
 
 - Common analysis techniques (G<sup>2</sup>, D<sup>2</sup>min, etc.)
 - Particle tracking
 - Masking and other preprocessing tools
 - Synthetic photoelastic response generation
@@ -47,15 +48,15 @@
 
 ## Documentation
 
 Available [here](http://jfeatherstone.github.io/pepe/pepe).
 
 ## Requirements
 
-Python 3.7 is the recommended version to use, with the following packages:
+Python 3.11 is the recommended version to use, with the following packages:
 
 - [numpy](https://numpy.org/)
 - [matplotlib](https://matplotlib.org/)
 - [lmfit](https://lmfit.github.io/lmfit-py/index.html)
 - [scikit-learn](https://scikit-learn.org/stable/)
 - [opencv](https://opencv.org/)
 - [Pillow](https://pillow.readthedocs.io/en/stable/)
@@ -83,9 +84,7 @@
 [1a] Jonathan Kollmer's implementation in Matlab: https://github.com/jekollmer/PEGS
 
 [1b] Olivier Lantsoght's implementation in Python: https://git.immc.ucl.ac.be/olantsoght/pegs_py
 
 [2] Abed Zadeh, A., Barés, J., Brzinski, T. A., Daniels, K. E., Dijksman, J., Docquier, N., Everitt, H. O., Kollmer, J. E., Lantsoght, O., Wang, D., Workamp, M., Zhao, Y., & Zheng, H. (2019). Enlightening force chains: A review of photoelasticimetry in granular matter. Granular Matter, 21(4), 83. https://doi.org/10.1007/s10035-019-0942-2
 
 [3] Photoelastic methods wiki. https://git-xen.lmgc.univ-montp2.fr/PhotoElasticity/Main/-/wikis/home
-
-
```

### Comparing `pepe-granular-1.0.0/pepe_granular.egg-info/SOURCES.txt` & `pepe-granular-1.1.0/pepe_granular.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 pepe/preprocess/Mask.py
 pepe/preprocess/Rescale.py
 pepe/preprocess/__init__.py
 pepe/simulate/SyntheticPE.py
 pepe/simulate/__init__.py
 pepe/test/__init__.py
 pepe/test/test_auto.py
+pepe/test/test_conv_tracking.py
+pepe/test/test_synthetic_force_solve.py
 pepe/test/test_utils.py
 pepe/topology/PersistentHomology.py
 pepe/topology/__init__.py
 pepe/tracking/AngularConvolution.py
 pepe/tracking/CNNDetection.py
 pepe/tracking/Convolution.py
 pepe/tracking/DTypes.py
```

### Comparing `pepe-granular-1.0.0/setup.py` & `pepe-granular-1.1.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
      name='pepe-granular',  
-     version='1.0.0',
+     version='1.1.0',
      author="Jack Featherstone",
-     author_email="jdfeathe@ncsu.edu",
+     author_email="jack.featherstone@oist.jp",
      license='MIT',
      url='https://jfeatherstone.github.io/pepe/pepe',
      description="Toolbox for granular analysis of photoelastic images",
      long_description=long_description,
      long_description_content_type="text/markdown",
      packages=setuptools.find_packages(),
      classifiers=[
          "Programming Language :: Python :: 3.7",
+         "Programming Language :: Python :: 3.11",
          "License :: OSI Approved :: MIT License",
          "Operating System :: OS Independent",
      ],
  )
```

