# Comparing `tmp/BDMLtools-0.3.6.tar.gz` & `tmp/BDMLtools-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BDMLtools-0.3.6.tar", last modified: Fri May 12 08:15:01 2023, max compression
+gzip compressed data, was "BDMLtools-0.3.7.tar", last modified: Wed May 24 02:40:59 2023, max compression
```

## Comparing `BDMLtools-0.3.6.tar` & `BDMLtools-0.3.7.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 zengke     (501) staff       (20)        0 2023-05-12 08:15:01.290393 BDMLtools-0.3.6/
-drwxr-xr-x   0 zengke     (501) staff       (20)        0 2023-05-12 08:15:01.272845 BDMLtools-0.3.6/BDMLtools/
--rwxr-xr-x   0 zengke     (501) staff       (20)     1490 2023-04-19 03:35:33.000000 BDMLtools-0.3.6/BDMLtools/__init__.py
--rw-r--r--   0 zengke     (501) staff       (20)     7931 2022-09-16 05:41:25.000000 BDMLtools-0.3.6/BDMLtools/base.py
-drwxr-xr-x   0 zengke     (501) staff       (20)        0 2023-05-12 08:15:01.275288 BDMLtools-0.3.6/BDMLtools/clearner/
--rw-r--r--   0 zengke     (501) staff       (20)      303 2022-05-30 05:46:05.000000 BDMLtools-0.3.6/BDMLtools/clearner/__init__.py
--rw-r--r--   0 zengke     (501) staff       (20)    21550 2023-05-10 02:08:49.000000 BDMLtools-0.3.6/BDMLtools/clearner/cleaner.py
-drwxr-xr-x   0 zengke     (501) staff       (20)        0 2023-05-12 08:15:01.276077 BDMLtools-0.3.6/BDMLtools/encoder/
--rw-r--r--   0 zengke     (501) staff       (20)      230 2022-09-09 08:32:26.000000 BDMLtools-0.3.6/BDMLtools/encoder/__init__.py
--rwxr-xr-x   0 zengke     (501) staff       (20)    13123 2022-10-26 06:18:44.000000 BDMLtools-0.3.6/BDMLtools/encoder/woe.py
--rw-r--r--   0 zengke     (501) staff       (20)      617 2022-05-30 05:46:05.000000 BDMLtools-0.3.6/BDMLtools/exception.py
--rwxr-xr-x   0 zengke     (501) staff       (20)     5965 2022-07-22 07:30:31.000000 BDMLtools-0.3.6/BDMLtools/fun.py
-drwxr-xr-x   0 zengke     (501) staff       (20)        0 2023-05-12 08:15:01.277091 BDMLtools-0.3.6/BDMLtools/plotter/
--rw-r--r--   0 zengke     (501) staff       (20)      280 2022-07-08 09:08:07.000000 BDMLtools-0.3.6/BDMLtools/plotter/__init__.py
--rw-r--r--   0 zengke     (501) staff       (20)    32833 2022-08-30 04:00:04.000000 BDMLtools-0.3.6/BDMLtools/plotter/base.py
--rw-r--r--   0 zengke     (501) staff       (20)    16452 2023-04-03 07:45:25.000000 BDMLtools-0.3.6/BDMLtools/plotter/eval.py
-drwxr-xr-x   0 zengke     (501) staff       (20)        0 2023-05-12 08:15:01.278048 BDMLtools-0.3.6/BDMLtools/report/
--rw-r--r--   0 zengke     (501) staff       (20)      379 2022-05-30 05:46:05.000000 BDMLtools-0.3.6/BDMLtools/report/__init__.py
--rwxr-xr-x   0 zengke     (501) staff       (20)    49254 2023-05-11 06:09:02.000000 BDMLtools-0.3.6/BDMLtools/report/report.py
-drwxr-xr-x   0 zengke     (501) staff       (20)        0 2023-05-12 08:15:01.281151 BDMLtools-0.3.6/BDMLtools/selector/
--rw-r--r--   0 zengke     (501) staff       (20)      902 2022-11-22 04:09:12.000000 BDMLtools-0.3.6/BDMLtools/selector/__init__.py
--rwxr-xr-x   0 zengke     (501) staff       (20)    30341 2023-01-31 10:03:44.000000 BDMLtools-0.3.6/BDMLtools/selector/bin.py
--rwxr-xr-x   0 zengke     (501) staff       (20)    61178 2023-03-29 06:28:50.000000 BDMLtools-0.3.6/BDMLtools/selector/bin_fun.py
--rw-r--r--   0 zengke     (501) staff       (20)    12019 2023-04-03 06:42:57.000000 BDMLtools-0.3.6/BDMLtools/selector/embeded.py
--rw-r--r--   0 zengke     (501) staff       (20)    16406 2023-04-19 06:45:01.000000 BDMLtools-0.3.6/BDMLtools/selector/fa.py
--rw-r--r--   0 zengke     (501) staff       (20)    25071 2023-03-30 01:22:06.000000 BDMLtools-0.3.6/BDMLtools/selector/lgbm.py
--rw-r--r--   0 zengke     (501) staff       (20)    27613 2022-10-08 09:45:23.000000 BDMLtools-0.3.6/BDMLtools/selector/logtit.py
--rw-r--r--   0 zengke     (501) staff       (20)    30242 2023-03-29 06:26:13.000000 BDMLtools-0.3.6/BDMLtools/selector/simple.py
-drwxr-xr-x   0 zengke     (501) staff       (20)        0 2023-05-12 08:15:01.284382 BDMLtools-0.3.6/BDMLtools/tuner/
--rw-r--r--   0 zengke     (501) staff       (20)      384 2022-05-30 05:46:05.000000 BDMLtools-0.3.6/BDMLtools/tuner/__init__.py
--rw-r--r--   0 zengke     (501) staff       (20)     3149 2023-04-18 10:14:12.000000 BDMLtools-0.3.6/BDMLtools/tuner/base.py
--rwxr-xr-x   0 zengke     (501) staff       (20)    17803 2023-04-19 02:58:32.000000 BDMLtools-0.3.6/BDMLtools/tuner/bayesian.py
--rwxr-xr-x   0 zengke     (501) staff       (20)     5750 2023-04-19 06:49:36.000000 BDMLtools-0.3.6/BDMLtools/tuner/fun.py
--rwxr-xr-x   0 zengke     (501) staff       (20)    23169 2023-04-19 03:22:16.000000 BDMLtools-0.3.6/BDMLtools/tuner/gridcv.py
--rwxr-xr-x   0 zengke     (501) staff       (20)    24712 2023-04-19 03:29:39.000000 BDMLtools-0.3.6/BDMLtools/tuner/halvingcv.py
-drwxr-xr-x   0 zengke     (501) staff       (20)        0 2023-05-12 08:15:01.274464 BDMLtools-0.3.6/BDMLtools.egg-info/
--rw-r--r--   0 zengke     (501) staff       (20)     2099 2023-05-12 08:15:01.000000 BDMLtools-0.3.6/BDMLtools.egg-info/PKG-INFO
--rw-r--r--   0 zengke     (501) staff       (20)     1046 2023-05-12 08:15:01.000000 BDMLtools-0.3.6/BDMLtools.egg-info/SOURCES.txt
--rw-r--r--   0 zengke     (501) staff       (20)        1 2023-05-12 08:15:01.000000 BDMLtools-0.3.6/BDMLtools.egg-info/dependency_links.txt
--rw-r--r--   0 zengke     (501) staff       (20)      481 2023-05-12 08:15:01.000000 BDMLtools-0.3.6/BDMLtools.egg-info/requires.txt
--rw-r--r--   0 zengke     (501) staff       (20)       15 2023-05-12 08:15:01.000000 BDMLtools-0.3.6/BDMLtools.egg-info/top_level.txt
--rw-r--r--   0 zengke     (501) staff       (20)     1062 2022-09-07 02:01:45.000000 BDMLtools-0.3.6/LICENSE
--rw-r--r--   0 zengke     (501) staff       (20)     2099 2023-05-12 08:15:01.289831 BDMLtools-0.3.6/PKG-INFO
--rw-r--r--   0 zengke     (501) staff       (20)     1573 2023-05-11 09:25:34.000000 BDMLtools-0.3.6/README.md
--rw-r--r--   0 zengke     (501) staff       (20)       38 2023-05-12 08:15:01.290543 BDMLtools-0.3.6/setup.cfg
--rwxr-xr-x   0 zengke     (501) staff       (20)     3662 2023-05-11 10:01:26.000000 BDMLtools-0.3.6/setup.py
-drwxr-xr-x   0 zengke     (501) staff       (20)        0 2023-05-12 08:15:01.289101 BDMLtools-0.3.6/test/
--rwxr-xr-x   0 zengke     (501) staff       (20)        0 2022-07-12 06:58:12.000000 BDMLtools-0.3.6/test/__init__.py
--rw-r--r--   0 zengke     (501) staff       (20)     9104 2022-09-06 10:00:06.000000 BDMLtools-0.3.6/test/test_base.py
--rw-r--r--   0 zengke     (501) staff       (20)     4500 2022-09-06 10:08:22.000000 BDMLtools-0.3.6/test/test_clearner.py
--rw-r--r--   0 zengke     (501) staff       (20)     1966 2022-08-30 07:06:15.000000 BDMLtools-0.3.6/test/test_eval.py
--rw-r--r--   0 zengke     (501) staff       (20)     4873 2023-05-12 07:52:29.000000 BDMLtools-0.3.6/test/test_report.py
--rw-r--r--   0 zengke     (501) staff       (20)    18928 2023-05-12 07:52:56.000000 BDMLtools-0.3.6/test/test_selector.py
--rw-r--r--   0 zengke     (501) staff       (20)    20045 2023-02-17 09:55:41.000000 BDMLtools-0.3.6/test/test_tunner.py
+drwxr-xr-x   0 zengke     (501) staff       (20)        0 2023-05-24 02:40:59.453074 BDMLtools-0.3.7/
+drwxr-xr-x   0 zengke     (501) staff       (20)        0 2023-05-24 02:40:59.431130 BDMLtools-0.3.7/BDMLtools/
+-rwxr-xr-x   0 zengke     (501) staff       (20)     1544 2023-05-23 09:54:46.000000 BDMLtools-0.3.7/BDMLtools/__init__.py
+-rw-r--r--   0 zengke     (501) staff       (20)     7931 2022-09-16 05:41:25.000000 BDMLtools-0.3.7/BDMLtools/base.py
+drwxr-xr-x   0 zengke     (501) staff       (20)        0 2023-05-24 02:40:59.434763 BDMLtools-0.3.7/BDMLtools/clearner/
+-rw-r--r--   0 zengke     (501) staff       (20)      303 2022-05-30 05:46:05.000000 BDMLtools-0.3.7/BDMLtools/clearner/__init__.py
+-rw-r--r--   0 zengke     (501) staff       (20)    21550 2023-05-10 02:08:49.000000 BDMLtools-0.3.7/BDMLtools/clearner/cleaner.py
+drwxr-xr-x   0 zengke     (501) staff       (20)        0 2023-05-24 02:40:59.435751 BDMLtools-0.3.7/BDMLtools/encoder/
+-rw-r--r--   0 zengke     (501) staff       (20)      230 2022-09-09 08:32:26.000000 BDMLtools-0.3.7/BDMLtools/encoder/__init__.py
+-rwxr-xr-x   0 zengke     (501) staff       (20)    13123 2022-10-26 06:18:44.000000 BDMLtools-0.3.7/BDMLtools/encoder/woe.py
+-rw-r--r--   0 zengke     (501) staff       (20)      617 2022-05-30 05:46:05.000000 BDMLtools-0.3.7/BDMLtools/exception.py
+-rwxr-xr-x   0 zengke     (501) staff       (20)     5965 2022-07-22 07:30:31.000000 BDMLtools-0.3.7/BDMLtools/fun.py
+drwxr-xr-x   0 zengke     (501) staff       (20)        0 2023-05-24 02:40:59.437502 BDMLtools-0.3.7/BDMLtools/plotter/
+-rw-r--r--   0 zengke     (501) staff       (20)      280 2022-07-08 09:08:07.000000 BDMLtools-0.3.7/BDMLtools/plotter/__init__.py
+-rw-r--r--   0 zengke     (501) staff       (20)    32833 2022-08-30 04:00:04.000000 BDMLtools-0.3.7/BDMLtools/plotter/base.py
+-rw-r--r--   0 zengke     (501) staff       (20)    16452 2023-04-03 07:45:25.000000 BDMLtools-0.3.7/BDMLtools/plotter/eval.py
+drwxr-xr-x   0 zengke     (501) staff       (20)        0 2023-05-24 02:40:59.439099 BDMLtools-0.3.7/BDMLtools/report/
+-rw-r--r--   0 zengke     (501) staff       (20)      379 2022-05-30 05:46:05.000000 BDMLtools-0.3.7/BDMLtools/report/__init__.py
+-rwxr-xr-x   0 zengke     (501) staff       (20)    49254 2023-05-11 06:09:02.000000 BDMLtools-0.3.7/BDMLtools/report/report.py
+drwxr-xr-x   0 zengke     (501) staff       (20)        0 2023-05-24 02:40:59.444082 BDMLtools-0.3.7/BDMLtools/selector/
+-rw-r--r--   0 zengke     (501) staff       (20)      902 2022-11-22 04:09:12.000000 BDMLtools-0.3.7/BDMLtools/selector/__init__.py
+-rwxr-xr-x   0 zengke     (501) staff       (20)    30341 2023-01-31 10:03:44.000000 BDMLtools-0.3.7/BDMLtools/selector/bin.py
+-rwxr-xr-x   0 zengke     (501) staff       (20)    61178 2023-03-29 06:28:50.000000 BDMLtools-0.3.7/BDMLtools/selector/bin_fun.py
+-rw-r--r--   0 zengke     (501) staff       (20)    12019 2023-04-03 06:42:57.000000 BDMLtools-0.3.7/BDMLtools/selector/embeded.py
+-rw-r--r--   0 zengke     (501) staff       (20)    16406 2023-04-19 06:45:01.000000 BDMLtools-0.3.7/BDMLtools/selector/fa.py
+-rw-r--r--   0 zengke     (501) staff       (20)    25071 2023-03-30 01:22:06.000000 BDMLtools-0.3.7/BDMLtools/selector/lgbm.py
+-rw-r--r--   0 zengke     (501) staff       (20)    27613 2022-10-08 09:45:23.000000 BDMLtools-0.3.7/BDMLtools/selector/logtit.py
+-rw-r--r--   0 zengke     (501) staff       (20)    30242 2023-03-29 06:26:13.000000 BDMLtools-0.3.7/BDMLtools/selector/simple.py
+drwxr-xr-x   0 zengke     (501) staff       (20)        0 2023-05-24 02:40:59.447754 BDMLtools-0.3.7/BDMLtools/tuner/
+-rw-r--r--   0 zengke     (501) staff       (20)      438 2023-05-23 09:53:29.000000 BDMLtools-0.3.7/BDMLtools/tuner/__init__.py
+-rw-r--r--   0 zengke     (501) staff       (20)     6112 2023-05-23 07:03:18.000000 BDMLtools-0.3.7/BDMLtools/tuner/base.py
+-rwxr-xr-x   0 zengke     (501) staff       (20)    34492 2023-05-23 08:19:23.000000 BDMLtools-0.3.7/BDMLtools/tuner/bayesian.py
+-rwxr-xr-x   0 zengke     (501) staff       (20)     5750 2023-04-19 06:49:36.000000 BDMLtools-0.3.7/BDMLtools/tuner/fun.py
+-rwxr-xr-x   0 zengke     (501) staff       (20)    45735 2023-05-23 09:50:24.000000 BDMLtools-0.3.7/BDMLtools/tuner/gridcv.py
+-rwxr-xr-x   0 zengke     (501) staff       (20)    24712 2023-04-19 03:29:39.000000 BDMLtools-0.3.7/BDMLtools/tuner/halvingcv.py
+drwxr-xr-x   0 zengke     (501) staff       (20)        0 2023-05-24 02:40:59.433335 BDMLtools-0.3.7/BDMLtools.egg-info/
+-rw-r--r--   0 zengke     (501) staff       (20)     2136 2023-05-24 02:40:59.000000 BDMLtools-0.3.7/BDMLtools.egg-info/PKG-INFO
+-rw-r--r--   0 zengke     (501) staff       (20)     1046 2023-05-24 02:40:59.000000 BDMLtools-0.3.7/BDMLtools.egg-info/SOURCES.txt
+-rw-r--r--   0 zengke     (501) staff       (20)        1 2023-05-24 02:40:59.000000 BDMLtools-0.3.7/BDMLtools.egg-info/dependency_links.txt
+-rw-r--r--   0 zengke     (501) staff       (20)      481 2023-05-24 02:40:59.000000 BDMLtools-0.3.7/BDMLtools.egg-info/requires.txt
+-rw-r--r--   0 zengke     (501) staff       (20)       15 2023-05-24 02:40:59.000000 BDMLtools-0.3.7/BDMLtools.egg-info/top_level.txt
+-rw-r--r--   0 zengke     (501) staff       (20)     1062 2022-09-07 02:01:45.000000 BDMLtools-0.3.7/LICENSE
+-rw-r--r--   0 zengke     (501) staff       (20)     2136 2023-05-24 02:40:59.452629 BDMLtools-0.3.7/PKG-INFO
+-rw-r--r--   0 zengke     (501) staff       (20)     1610 2023-05-24 01:49:35.000000 BDMLtools-0.3.7/README.md
+-rw-r--r--   0 zengke     (501) staff       (20)       38 2023-05-24 02:40:59.453204 BDMLtools-0.3.7/setup.cfg
+-rwxr-xr-x   0 zengke     (501) staff       (20)     3662 2023-05-11 10:01:26.000000 BDMLtools-0.3.7/setup.py
+drwxr-xr-x   0 zengke     (501) staff       (20)        0 2023-05-24 02:40:59.451935 BDMLtools-0.3.7/test/
+-rwxr-xr-x   0 zengke     (501) staff       (20)        0 2022-07-12 06:58:12.000000 BDMLtools-0.3.7/test/__init__.py
+-rw-r--r--   0 zengke     (501) staff       (20)     9104 2022-09-06 10:00:06.000000 BDMLtools-0.3.7/test/test_base.py
+-rw-r--r--   0 zengke     (501) staff       (20)     4500 2022-09-06 10:08:22.000000 BDMLtools-0.3.7/test/test_clearner.py
+-rw-r--r--   0 zengke     (501) staff       (20)     1966 2022-08-30 07:06:15.000000 BDMLtools-0.3.7/test/test_eval.py
+-rw-r--r--   0 zengke     (501) staff       (20)     4873 2023-05-12 07:52:29.000000 BDMLtools-0.3.7/test/test_report.py
+-rw-r--r--   0 zengke     (501) staff       (20)    18928 2023-05-12 07:52:56.000000 BDMLtools-0.3.7/test/test_selector.py
+-rw-r--r--   0 zengke     (501) staff       (20)    26124 2023-05-24 01:22:44.000000 BDMLtools-0.3.7/test/test_tunner.py
```

### Comparing `BDMLtools-0.3.6/BDMLtools/__init__.py` & `BDMLtools-0.3.7/BDMLtools/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,25 +8,27 @@
 from BDMLtools.selector import preSelector,prefitModel
 from BDMLtools.selector import LgbmSeqSelector,LgbmPISelector,LgbmShapRFECVSelector
 #from BDMLtools.selector import RFECVSelector
 from BDMLtools.selector import LassoLogit
 from BDMLtools.plotter import BaseWoePlotter
 from BDMLtools.plotter import perfEval,perfEval2
 from BDMLtools.encoder import woeTransformer,binTransformer
-from BDMLtools.tuner import gridTuner,hgridTuner
-from BDMLtools.tuner import BayesianCVTuner,shapCheck
+from BDMLtools.tuner import gridTuner,hgridTuner,FLgridTuner
+from BDMLtools.tuner import BayesianCVTuner,FLBSTuner,shapCheck
 
 
-__version__ = '0.3.6'
+__version__ = '0.3.7'
 
 __all__ = (    
     dtStandardization,
     outliersTransformer,
     dtypeAllocator,
     nanTransformer,
+    FLBSTuner,
+    FLgridTuner,
     businessReport,
     prefitModel,
     EDAReport,
     varReportSinge,
     varReport,
     varGroupsReport,
     varGroupsPlot,
```

### Comparing `BDMLtools-0.3.6/BDMLtools/base.py` & `BDMLtools-0.3.7/BDMLtools/base.py`

 * *Files identical despite different names*

### Comparing `BDMLtools-0.3.6/BDMLtools/clearner/cleaner.py` & `BDMLtools-0.3.7/BDMLtools/clearner/cleaner.py`

 * *Files identical despite different names*

### Comparing `BDMLtools-0.3.6/BDMLtools/encoder/woe.py` & `BDMLtools-0.3.7/BDMLtools/encoder/woe.py`

 * *Files identical despite different names*

### Comparing `BDMLtools-0.3.6/BDMLtools/exception.py` & `BDMLtools-0.3.7/BDMLtools/exception.py`

 * *Files identical despite different names*

### Comparing `BDMLtools-0.3.6/BDMLtools/fun.py` & `BDMLtools-0.3.7/BDMLtools/fun.py`

 * *Files identical despite different names*

### Comparing `BDMLtools-0.3.6/BDMLtools/plotter/base.py` & `BDMLtools-0.3.7/BDMLtools/plotter/base.py`

 * *Files identical despite different names*

### Comparing `BDMLtools-0.3.6/BDMLtools/plotter/eval.py` & `BDMLtools-0.3.7/BDMLtools/plotter/eval.py`

 * *Files identical despite different names*

### Comparing `BDMLtools-0.3.6/BDMLtools/report/report.py` & `BDMLtools-0.3.7/BDMLtools/report/report.py`

 * *Files identical despite different names*

### Comparing `BDMLtools-0.3.6/BDMLtools/selector/__init__.py` & `BDMLtools-0.3.7/BDMLtools/selector/__init__.py`

 * *Files identical despite different names*

### Comparing `BDMLtools-0.3.6/BDMLtools/selector/bin.py` & `BDMLtools-0.3.7/BDMLtools/selector/bin.py`

 * *Files identical despite different names*

### Comparing `BDMLtools-0.3.6/BDMLtools/selector/bin_fun.py` & `BDMLtools-0.3.7/BDMLtools/selector/bin_fun.py`

 * *Files identical despite different names*

### Comparing `BDMLtools-0.3.6/BDMLtools/selector/embeded.py` & `BDMLtools-0.3.7/BDMLtools/selector/embeded.py`

 * *Files identical despite different names*

### Comparing `BDMLtools-0.3.6/BDMLtools/selector/fa.py` & `BDMLtools-0.3.7/BDMLtools/selector/fa.py`

 * *Files identical despite different names*

### Comparing `BDMLtools-0.3.6/BDMLtools/selector/lgbm.py` & `BDMLtools-0.3.7/BDMLtools/selector/lgbm.py`

 * *Files identical despite different names*

### Comparing `BDMLtools-0.3.6/BDMLtools/selector/logtit.py` & `BDMLtools-0.3.7/BDMLtools/selector/logtit.py`

 * *Files identical despite different names*

### Comparing `BDMLtools-0.3.6/BDMLtools/selector/simple.py` & `BDMLtools-0.3.7/BDMLtools/selector/simple.py`

 * *Files identical despite different names*

### Comparing `BDMLtools-0.3.6/BDMLtools/tuner/fun.py` & `BDMLtools-0.3.7/BDMLtools/tuner/fun.py`

 * *Files identical despite different names*

### Comparing `BDMLtools-0.3.6/BDMLtools/tuner/gridcv.py` & `BDMLtools-0.3.7/BDMLtools/tuner/halvingcv.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,84 +2,89 @@
 # -*- coding: utf-8 -*-
 """
 Created on Fri Oct 15 09:32:09 2021
 
 @author: zengke
 """
 
-from sklearn.model_selection import GridSearchCV,RandomizedSearchCV
-from sklearn.model_selection import RepeatedStratifiedKFold,train_test_split
-from sklearn.calibration import CalibratedClassifierCV
 from BDMLtools.base import Base
+from sklearn.experimental import enable_halving_search_cv
+from sklearn.model_selection import train_test_split
 from BDMLtools.tuner.base import BaseTunner
+from sklearn.model_selection import HalvingGridSearchCV,HalvingRandomSearchCV,RepeatedStratifiedKFold
+from sklearn.calibration import CalibratedClassifierCV
 from joblib import effective_n_jobs
+#from lightgbm import early_stopping as lgbm_early_stopping
 
 
-class gridTuner(Base,BaseTunner):
+class hgridTuner(Base,BaseTunner):
     
     '''
-    Xgb与Lgbm的网格搜索与随机搜索
+    Xgb与Lgbm的sucessive halving搜索与sucessive halving搜索
     Parameters:
     --
         Estimator:拟合器,XGBClassifier、LGBMClassifier或CatBoostClassifier
-        method:str,可选"grid"或"random_grid"
-        para_space:dict,参数空间,注意随机搜索与网格搜索对应不同的dict结构,参数空间写法见后                        
-        n_iter:随机网格搜索迭代次数,当method="grid"时该参数会被忽略
-        scoring:str,寻优准则,可选'auc','ks','lift','neglogloss',目前不支持sample_weight
+        method:str,可选"h_grid"或"h_random"
+        para_space:dict,参数空间,注意随机搜索与网格搜索对应不同的dict结构,参数空间写法见后                       
+        n_candidates:int or 'exhaust',halving random_search的抽样候选参数个数,当method="h_grid"时该参数会被忽略
+        factor:int,halving search中，1/factor的候选参数将被用于下一次迭代
+        scoring:str,寻优准则,可选'auc','ks','lift',目前不支持sample_weight
         repeats:int,RepeatedStratifiedKFold交叉验证重复次数
         cv:int,交叉验证的折数
         early_stopping_rounds=10,int,训练数据中validation_fraction比例的数据被作为验证数据进行early_stopping
         validation_fraction=0.1,float,进行early_stopping的验证集比例
         eval_metric=‘auc’,early_stopping的评价指标,为可被Estimator识别的格式,参考Estimator.fit中的eval_metric参数
         n_jobs,int,运行交叉验证时的joblib的并行数,默认-1
         verbose,int,并行信息输出等级
         random_state:int,随机种子
         calibration:使用sklearn的CalibratedClassifierCV对refit的模型进行概率校准
         cv_calibration:CalibratedClassifierCV的交叉验证数
         
         """参数空间写法
-            当Estimator=XGBClassifier,method="grid":
+        
+            当Estimator=XGBClassifier,method="h_grid":
                 
-               para_space={
-                     'n_estimators':[100],
+                param_space={
+                     'n_estimators':[100]
                      'learning_rate':[0.1],
                     
                      'max_depth':[3],
                      'gamma': [0,10],
+                     'min_child_weight': 
                      
-                     'subsample':[0.6],
-                     'colsample_bytree' :[0.6],
+                     'subsample':[0.6,0.8],
+                     'colsample_bytree' :[0.6,0.8],
                      'reg_lambda':[0,10], 
-                     'scale_pos_weight':[1],
-                     'max_delta_step':[0],
-                     'use_label_encoder':[False]
+                     'scale_pos_weight':[1,11],
+                     'max_delta_step':[0]
                      }
             
-            当Estimator=XGBClassifier,method="random_grid":     
-                  
+            当Estimator=XGBClassifier,method="h_random":     
+               
                from scipy.stats import randint as sp_randint
                from scipy.stats import uniform as sp_uniform 
                
-               para_space={
+               param_distributions={
                      'n_estimators':sp_randint(low=60,high=120),#迭代次数
                      'learning_rate':sp_uniform(loc=0.05,scale=0.15), #学习率
                     
                      'max_depth':sp_randint(low=2,high=4),
                      'gamma': sp_uniform(loc=0,scale=21),
                      'min_child_weight': sp_uniform(loc=0,scale=21),
                      
                      'subsample':sp_uniform(loc=0.5,scale=0.5),
                      'colsample_bytree' :sp_uniform(loc=0.5,scale=0.5),
                      
                      'reg_lambda':sp_randint(low=0,high=1), 
-                     'max_delta_step':sp_uniform(loc=0,scale=0),
-                     'use_label_encoder':[False]                      
-                     } 
+                     'scale_pos_weight':sp_uniform(loc=1,scale=0), 
+                     'max_delta_step':sp_uniform(loc=0,scale=0)
+                     }                     
+                     
               
-             当Estimator=LGBMClassifier,method="grid": 
+             当Estimator=LGBMClassifier,method="h_grid": 
                  
                 para_space={
                      'boosting_type':['gbdt','goss'], 
                      'n_estimators':[100],
                      'learning_rate':[0.1], 
                     
                      'max_depth':[3],#[0,∞],
@@ -88,48 +93,50 @@
                      
                      'scale_pos_weight':[1],
                      'subsample':[0.6,0.8],
                      'colsample_bytree' :[0.6,0.8],
                      'reg_lambda':[0,10], 
                      }
                 
-             当Estimator=LGBMClassifier,method="random_grid": 
+             当Estimator=LGBMClassifier,method="h_random": 
                  
                  from scipy.stats import randint as sp_randint
                  from scipy.stats import uniform as sp_uniform 
                  
                  para_space={
                      'boosting_type':['gbdt','goss'], #'goss','gbdt'
                      'n_estimators':sp_randint(low=100,high=110),
                      'learning_rate':sp_uniform(loc=0.1,scale=0), 
                     
                      'max_depth':sp_randint(low=2,high=4),#[0,∞],
                      'min_split_gain': sp_uniform(loc=0,scale=0),
-                     'min_child_samples': sp_randint(low=100,high=300),#[0,∞],
+                     'min_child_weight': sp_uniform(loc=0,scale=0),
                      
-                     'scale_pos_weight':[1],
+                     'scale_pos_weight':[1,11],
                      'subsample':sp_uniform(loc=0.5,scale=0.5),
                      'colsample_bytree' :sp_uniform(loc=0.5,scale=0.5),
                      'reg_lambda':sp_uniform(loc=0,scale=20),
                      }
                      
-            当Estimator=CatBoostClassifier,method="grid": 
+             
+             当Estimator=CatBoostClassifier,method="h_grid": 
             
-                    para_space={
+                 para_space={
                      'nan_mode':['Min'],
                      'n_estimators': [80, 100],
                      'learning_rate': [0.03,0.05, 0.1],
                      'max_depth': [2,3],
                      'scale_pos_weight': [1],
                      'subsample': [1],
                      'colsample_bylevel': [1],
-                     'reg_lambda': [0]}
+                     'reg_lambda': [0]
+                 }
             
             
-            当Estimator=CatBoostClassifier,method="random_grid": 
+             当Estimator=CatBoostClassifier,method="h_random": 
 
 
                  from scipy.stats import randint as sp_randint
                  from scipy.stats import uniform as sp_uniform 
                  
                  para_space={         
                      'nan_mode':['Min'],
@@ -137,64 +144,67 @@
                      'learning_rate':sp_uniform(loc=0.1,scale=0),                     
                      'max_depth':sp_randint(low=2,high=4),#[0,∞],                     
                      'scale_pos_weight':[1],
                      'subsample':sp_uniform(loc=0.5,scale=0.5),
                      'colsample_bylevel' :sp_uniform(loc=0.5,scale=0.5),
                      'reg_lambda':sp_uniform(loc=0,scale=20),
                      }
-                
+                     
         """   
     
     Attribute:    
     --
         cv_result:交叉验证结果,需先使用fit
         params_best:最优参数组合,需先使用fit
-        grid_res:method="grid"下的网格优化结果,需先使用fit
-        r_grid_res:method="random_grid"下的网格优化结果,需先使用fit
+        h_grid_res:method="h_grid"下的优化结果,需先使用fit
+        h_random_res:method="h_random"下的优化结果,需先使用fit
         model_refit:最优参数下的模型,需先使用fit
         
     Examples
-    --        
+    --
 
-    '''    
+    '''     
     
     
-    def __init__(self,Estimator,para_space,method='random_grid',n_iter=10,scoring='roc_auc',eval_metric='auc',repeats=1,cv=5,early_stopping_rounds=10,validation_fraction=0.1,
+    def __init__(self,Estimator,para_space,method='h_random',scoring='auc',eval_metric='auc',repeats=1,cv=5,
+                 factor=3,n_candidates='exhaust',early_stopping_rounds=10,validation_fraction=0.1,
                  n_jobs=-1,verbose=0,random_state=123,calibration=False,cv_calibration=5):
-       
+      
         self.Estimator=Estimator
         self.para_space=para_space
         self.method=method
-        self.n_iter=n_iter
+        self.factor=factor
+        self.n_candidates=n_candidates
         self.scoring=scoring
         self.cv=cv
         self.repeats=repeats
         self.early_stopping_rounds=early_stopping_rounds
         self.eval_metric=eval_metric
         self.validation_fraction=validation_fraction
         self.n_jobs=n_jobs
         self.verbose=verbose     
         self.random_state=random_state
         self.calibration=calibration
         self.cv_calibration=cv_calibration
         
         self._is_fitted=False
-
+        
         
     def predict_proba(self,X,y=None):
         '''
         最优参数下的模型的预测
         Parameters:
         --
         X:pd.DataFrame对象
         '''      
         self._check_is_fitted()
         self._check_X(X)
         
-        pred = self.model_refit.predict_proba(self.transform(X))[:,1]        
+        pred = self.model_refit.predict_proba(self.transform(X))[:,1]    
+        
         return pred
     
     def predict_score(self,X,y=None,PDO=75,base=660,ratio=1/15):
         '''
         最优参数下的模型的预测
         Parameters:
         --
@@ -204,77 +214,76 @@
         self._check_X(X)
         
         pred = self.model_refit.predict_proba(self.transform(X))[:,1]  
         pred = self._p_to_score(pred,PDO,base,ratio)
         
         return pred
     
-    def transform(self,X,y=None):  
-        
+    
+    def transform(self,X,y=None):   
+
         self._check_is_fitted()
         self._check_X(X)
         
         if self.Estimator.__module__ == 'catboost.core':
             
             out=X.apply(lambda col:col.astype('str') if col.name in self.cat_features else col) if self.cat_features else X
             
         elif self.Estimator.__module__ == 'lightgbm.sklearn':
         
             out=X.apply(lambda col:col.astype('category') if col.name in self.cat_features else col) if self.cat_features else X
             
         else:
             
-            out=X
-
+            out=X        
+         
         return out
           
     def fit(self,X,y,cat_features=None,sample_weight=None):
         '''
         进行参数优化
         Parameters:
         --
         X:pd.DataFrame对象
         y:目标变量,pd.Series对象
         cat_features:list,分类特征列名列表,None是数据中的object,category类列将被识别为cat_features，当Estimator为Xgboost时将忽略该参数        
         sample_weight:pd.Series,样本权重,index必须与X,y一致,注意目前不支持样本权重应用于交叉验证寻优指标(scorer)
         '''   
         
-        self._check_data(X, y)     
+        self._check_data(X, y)
         self._check_ws(y, sample_weight)
         
         self.cat_features=X.select_dtypes(['object','category']).columns.tolist() if cat_features is None else cat_features    
-
-
+        
         if self.Estimator.__module__ == 'catboost.core':
             
             X=X.apply(lambda col:col.astype('str') if col.name in self.cat_features else col) if self.cat_features else X
             
-        elif self.Estimator.__module__ == 'lightgbm.sklearn':       
+        elif self.Estimator.__module__ == 'lightgbm.sklearn':
         
             X=X.apply(lambda col:col.astype('category') if col.name in self.cat_features else col) if self.cat_features else X
             
         else:
             
             X=X   
 
-        
-        if self.method=='grid':
+            
+        if self.method=='h_grid':
             
             if self.early_stopping_rounds:
                 
                 X_tr, X_val, y_tr, y_val = train_test_split(X,y,test_size=self.validation_fraction,random_state=self.random_state,stratify=y)
                 
                 sample_weight_tr=sample_weight[y_tr.index] if sample_weight is not None else None
-
-                self._grid_search(X_tr,y_tr,sample_weight_tr)
-                
+            
+                self._h_grid_search(X_tr,y_tr,sample_weight_tr)
                 #输出最优参数组合
-                self.params_best=self.grid_res.best_params_
-                self.cv_result=self._cvresult_to_df(self.grid_res.cv_results_)
-                
+                self.params_best=self.h_grid_res.best_params_
+                self.cv_result=self._cvresult_to_df(self.h_grid_res.cv_results_)
+            
                 #refit with early_stopping_rounds  
                 if self.Estimator.__module__ == 'catboost.core':
                     
                     refit_Estimator=self.Estimator(random_state=self.random_state,
                                                    thread_count=effective_n_jobs(self.n_jobs),
                                                    **self.params_best)
                     
@@ -285,211 +294,226 @@
                     refit_Estimator.set_params(**{"eval_metric":self.eval_metric})
                     
                 else:
                     
                     refit_Estimator=self.Estimator(random_state=self.random_state,
                                                    n_jobs=effective_n_jobs(self.n_jobs),
                                                    **self.params_best)
-    
+                    
+            
                 self.model_refit = refit_Estimator.fit(**self._get_fit_params(self.Estimator,X_tr,y_tr,X_val,y_val,sample_weight,y_tr.index,y_val.index))   
                                                                                                      
                 self.params_best['best_iteration']=self.model_refit.best_iteration if self.Estimator.__module__ == 'xgboost.sklearn' else self.model_refit.best_iteration_ 
                 
             else:
                 
                 #search
-                self._grid_search(X,y,sample_weight)
+                
+                self._h_grid_search(X,y,sample_weight)
                 
                 #params_best
-                self.params_best=self.grid_res.best_params_
-         
+                self.params_best=self.h_grid_res.best_params_
+            
                 #cv_result
-                self.cv_result=self._cvresult_to_df(self.grid_res.cv_results_)
-                
-                #refit model
+                self.cv_result=self._cvresult_to_df(self.h_grid_res.cv_results_)
                 
-
+                #refit model            
                 if self.Estimator.__module__ == 'catboost.core':
                     
                     refit_Estimator=self.Estimator(random_state=self.random_state,
-                                                   thread_count=effective_n_jobs(self.n_jobs),
-                                                   **self.params_best)
+                                                   thread_count=effective_n_jobs(self.n_jobs),**self.params_best)
                     
                     refit_Estimator.set_params(**{'cat_features':self.cat_features})
                     
                 else:
                     
                     refit_Estimator=self.Estimator(random_state=self.random_state,
-                                                   n_jobs=effective_n_jobs(self.n_jobs),
-                                                   **self.params_best)
-
+                                                   n_jobs=effective_n_jobs(self.n_jobs),**self.params_best)
+            
                 self.model_refit = refit_Estimator.fit(X,y,sample_weight=sample_weight)          
 
-                
-                
-        elif self.method=='random_grid':
+            
+        elif self.method=='h_random':
             
             if self.early_stopping_rounds:
                 
                 X_tr, X_val, y_tr, y_val = train_test_split(X,y,test_size=self.validation_fraction,random_state=self.random_state,stratify=y)
                 
                 sample_weight_tr=sample_weight[y_tr.index] if sample_weight is not None else None
-
             
-                self._random_search(X_tr,y_tr,sample_weight)
+                self._h_random_search(X_tr,y_tr,sample_weight_tr)
                 #输出最优参数组合
-                self.params_best=self.r_grid_res.best_params_
-                self.cv_result=self._cvresult_to_df(self.r_grid_res.cv_results_)                
+                self.params_best=self.h_random_res.best_params_
+                self.cv_result=self._cvresult_to_df(self.h_random_res.cv_results_)
             
-                #refit with early_stopping_rounds or None  
+                #refit with early_stopping_rounds  
                 if self.Estimator.__module__ == 'catboost.core':
                     
                     refit_Estimator=self.Estimator(random_state=self.random_state,
                                                    thread_count=effective_n_jobs(self.n_jobs),
                                                    **self.params_best)
-           
+                    
                     if self.eval_metric=='auc':
                         
                         self.eval_metric='AUC'
                     
                     refit_Estimator.set_params(**{"eval_metric":self.eval_metric})
                     
                 else:
                     
                     refit_Estimator=self.Estimator(random_state=self.random_state,
                                                    n_jobs=effective_n_jobs(self.n_jobs),
-                                                   **self.params_best)
-    
+                                                   **self.params_best)                    
+            
                 self.model_refit = refit_Estimator.fit(**self._get_fit_params(self.Estimator,X_tr,y_tr,X_val,y_val,sample_weight,y_tr.index,y_val.index))   
                                                                                                      
                 self.params_best['best_iteration']=self.model_refit.best_iteration if self.Estimator.__module__ == 'xgboost.sklearn' else self.model_refit.best_iteration_ 
-    
-    
+                
             else:
                 
                 #search
-                self._random_search(X,y,sample_weight)
+                
+                self._h_random_search(X,y,sample_weight)
                 
                 #params_best
-                self.params_best=self.r_grid_res.best_params_
-         
+                self.params_best=self.h_random_res.best_params_
+            
                 #cv_result
-                self.cv_result=self._cvresult_to_df(self.r_grid_res.cv_results_)
+                self.cv_result=self._cvresult_to_df(self.h_random_res.cv_results_)
                 
-                #refit with early_stopping_rounds or None      
+                #refit model
                 if self.Estimator.__module__ == 'catboost.core':
                     
                     refit_Estimator=self.Estimator(random_state=self.random_state,
-                                                   thread_count=effective_n_jobs(self.n_jobs),
-                                                   **self.params_best)
+                                                   thread_count=effective_n_jobs(self.n_jobs),**self.params_best)                   
                     
                     refit_Estimator.set_params(**{'cat_features':self.cat_features})
                     
                 else:
                     
                     refit_Estimator=self.Estimator(random_state=self.random_state,
-                                                   n_jobs=effective_n_jobs(self.n_jobs),
-                                                   **self.params_best)
-    
-                self.model_refit = refit_Estimator.fit(X,y,sample_weight=sample_weight) 
-                
-                
+                                                   n_jobs=effective_n_jobs(self.n_jobs),**self.params_best) 
+                    
+                    
+            
+                self.model_refit = refit_Estimator.fit(X,y,sample_weight=sample_weight)          
+                                                        
             
         else:
             
-            raise ValueError('method should be "grid" or "random_grid".')
+            raise ValueError('method should be "h_random" or "h_grid".')
             
             
         if self.calibration:
             
             self.model_refit=CalibratedClassifierCV(self.model_refit,cv=self.cv_calibration,
-                                                 n_jobs=self.n_jobs).fit(X,y,sample_weight=sample_weight)
-            
+                                                  n_jobs=effective_n_jobs(self.n_jobs)).fit(X,y,sample_weight=sample_weight) 
+                       
         self._is_fitted=True
-            
+        
         return self    
     
-    def _grid_search(self,X,y,sample_weight):          
+    def _h_grid_search(self,X,y,sample_weight):          
         '''
         网格搜索
         '''  
         if self.scoring in ['ks','auc','lift','neglogloss']:
             
             scorer=self._get_scorer[self.scoring]
             
         else:
             
             scorer=self.scoring
             
         cv = RepeatedStratifiedKFold(n_splits=self.cv, n_repeats=self.repeats, random_state=self.random_state) 
         
-        n_jobs=effective_n_jobs(self.n_jobs)              
+        n_jobs=effective_n_jobs(self.n_jobs) 
+        
         
         if self.Estimator.__module__ == 'catboost.core':
             
-            grid=GridSearchCV(self.Estimator(random_state=self.random_state,thread_count=n_jobs),self.para_space,cv=cv,
-                              n_jobs=-1 if self.n_jobs==-1 else 1,
-                              refit=False,
-                              verbose=self.verbose,
-                              scoring=scorer,error_score=0)   
-            
-            self.grid_res=grid.fit(X,y,sample_weight=sample_weight,cat_features=self.cat_features)
+            hgrid=HalvingGridSearchCV(self.Estimator(random_state=self.random_state,thread_count=n_jobs),
+                                      param_grid=self.para_space,
+                                      cv=cv,
+                                      refit=False,
+                                      factor=self.factor,
+                                      scoring=scorer,
+                                      random_state=self.random_state,
+                                      verbose=self.verbose,
+                                      n_jobs=-1 if self.n_jobs==-1 else 1)
+        
+            self.h_grid_res=hgrid.fit(X,y,**{'sample_weight':sample_weight,'cat_features':self.cat_features})
             
         else:
             
-            grid=GridSearchCV(self.Estimator(random_state=self.random_state,n_jobs=n_jobs),self.para_space,cv=cv,
-                              n_jobs=-1 if self.n_jobs==-1 else 1,
-                              refit=False,
-                              verbose=self.verbose,
-                              scoring=scorer,error_score=0)   
+            hgrid=HalvingGridSearchCV(self.Estimator(random_state=self.random_state,n_jobs=n_jobs),
+                                      param_grid=self.para_space,
+                                      cv=cv,
+                                      refit=False,
+                                      factor=self.factor,
+                                      scoring=scorer,
+                                      random_state=self.random_state,
+                                      verbose=self.verbose,
+                                      n_jobs=-1 if self.n_jobs==-1 else 1)
             
-            self.grid_res=grid.fit(X,y,sample_weight=sample_weight)
-        
+            self.h_grid_res=hgrid.fit(X,y,sample_weight=sample_weight)
+           
         return self
         
         
-    def _random_search(self,X,y,sample_weight):          
+    def _h_random_search(self,X,y,sample_weight):  
         '''
         随机网格搜索
         '''         
         
         if self.scoring in ['ks','auc','lift','neglogloss']:
             
             scorer=self._get_scorer[self.scoring]
             
         else:
             
-            scorer=self.scoring
+           scorer=self.scoring
         
         cv = RepeatedStratifiedKFold(n_splits=self.cv, n_repeats=self.repeats, random_state=self.random_state) 
         
         n_jobs=effective_n_jobs(self.n_jobs) 
         
-        
         if self.Estimator.__module__ == 'catboost.core':
             
-            r_grid=RandomizedSearchCV(self.Estimator(random_state=self.random_state,thread_count=n_jobs),self.para_space,cv=cv,
-                                      n_jobs=-1 if self.n_jobs==-1 else 1,
-                                      verbose=self.verbose,refit=False,
-                                      random_state=self.random_state,
-                                      scoring=scorer,error_score=0,n_iter=self.n_iter)
+            h_r_grid=HalvingRandomSearchCV(self.Estimator(random_state=self.random_state,thread_count=n_jobs),
+                                         param_distributions=self.para_space,
+                                         n_candidates=self.n_candidates,
+                                         factor=self.factor,
+                                         cv=cv,
+                                         n_jobs=-1 if self.n_jobs==-1 else 1,
+                                         verbose=self.verbose,
+                                         refit=True,
+                                         random_state=self.random_state,
+                                         scoring=scorer,
+                                         error_score=0)
         
-            self.r_grid_res=r_grid.fit(X,y,sample_weight=sample_weight,cat_features=self.cat_features)
+            self.h_random_res=h_r_grid.fit(X,y,**{'sample_weight':sample_weight,'cat_features':self.cat_features})
             
         else:
             
-            r_grid=RandomizedSearchCV(self.Estimator(random_state=self.random_state,n_jobs=n_jobs),self.para_space,cv=cv,
-                                      n_jobs=-1 if self.n_jobs==-1 else 1,
-                                      verbose=self.verbose,refit=False,
-                                      random_state=self.random_state,
-                                      scoring=scorer,error_score=0,n_iter=self.n_iter)
+            h_r_grid=HalvingRandomSearchCV(self.Estimator(random_state=self.random_state,n_jobs=n_jobs),
+                                         param_distributions=self.para_space,
+                                         n_candidates=self.n_candidates,
+                                         factor=self.factor,
+                                         cv=cv,
+                                         n_jobs=-1 if self.n_jobs==-1 else 1,
+                                         verbose=self.verbose,
+                                         refit=True,
+                                         random_state=self.random_state,
+                                         scoring=scorer,
+                                         error_score=0)
             
-            self.r_grid_res=r_grid.fit(X,y,sample_weight=sample_weight)
+            self.h_random_res=h_r_grid.fit(X,y,sample_weight=sample_weight)       
         
-        return self  
+        return self   
     
     
     def _get_fit_params(self,Estimator,X_train,y_train,X_val,y_val,sample_weight=None,train_index=None,val_index=None):
         
         
         if Estimator.__module__ == "xgboost.sklearn":
```

### Comparing `BDMLtools-0.3.6/BDMLtools.egg-info/PKG-INFO` & `BDMLtools-0.3.7/BDMLtools.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: BDMLtools
-Version: 0.3.6
+Version: 0.3.7
 Summary: Ml learning tools for busniess data mining
 Author: 曾珂
 Author-email: zengke403@163.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 Provides-Extra: all
 License-File: LICENSE
 
-# BDMLtools-0.3.6
+# BDMLtools-0.3.7
 
 [![PyPI version](https://img.shields.io/pypi/pyversions/BDMLtools.svg)](https://pypi.python.org/pypi/BDMLtools)
-[![License](https://img.shields.io/github/license/zk403/mlearn)](https://github.com/zk403/mlearn/blob/master/LICENSE)
+[![License](https://img.shields.io/github/license/zk403/mlearn)](https://github.com/zk403/mlearn/blob/main/LICENSE)
 [![Build Status](https://github.com/zk403/mlearn/actions/workflows/python-test.yml/badge.svg)](https://github.com/zk403/mlearn/actions/workflows/python-test.yml)
 [![codecov](https://codecov.io/gh/zk403/mlearn/main/graphs/badge.svg)](https://app.codecov.io/gh/zk403/mlearn)
 [![PyPI release](https://img.shields.io/pypi/v/BDMLtools.svg)](https://pypi.python.org/pypi/BDMLtools)
 
 BDMLtools是适用于常见商业数据分析数据挖掘场景下，中小数据量的二分类模型的机器学习建模工具包。
 本模组将集成商业分析场景中二分类模型中常用的机器学习模型，并使之能够兼顾模型开发效率、报告制作与建模流程标准化。
 本模组涵盖数据清洗、数据探索、特征工程、评分卡制作、模型评估、统计学逐步回归、机器学习模型及其参数优化等内容
@@ -44,15 +44,14 @@
 
 ```
 pip uninstall BDMLtools
 ```
 
 更新
 ```
-v0.3.6
-1.优化代码，移除对xgboost与catboost库的依赖
-2.优化代码，对sklearn的最低依赖降低为1.0.2
-3.修复了shapcheck中的使用catboost时无法计算的bug
-4.修复了EDAreport在pandas==2.0.1版本下的bug
+v0.3.7
+1.新增支持二分类focal loss的损失函数FocalLoss
+2.新增支持二分类focal loss的lightgbm类FLLGBMSklearn
+3.新增支持二分类focal loss下lightgbm的贝叶斯搜索类FLBSTuner
+4.新增支持二分类focal loss下lightgbm的网格搜素、随机搜索类FLgridTuner
 5.更新单元测试脚本,更新部分代码说明
-6.更新example
 ```
```

### Comparing `BDMLtools-0.3.6/BDMLtools.egg-info/SOURCES.txt` & `BDMLtools-0.3.7/BDMLtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `BDMLtools-0.3.6/LICENSE` & `BDMLtools-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `BDMLtools-0.3.6/PKG-INFO` & `BDMLtools-0.3.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: BDMLtools
-Version: 0.3.6
+Version: 0.3.7
 Summary: Ml learning tools for busniess data mining
 Author: 曾珂
 Author-email: zengke403@163.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 Provides-Extra: all
 License-File: LICENSE
 
-# BDMLtools-0.3.6
+# BDMLtools-0.3.7
 
 [![PyPI version](https://img.shields.io/pypi/pyversions/BDMLtools.svg)](https://pypi.python.org/pypi/BDMLtools)
-[![License](https://img.shields.io/github/license/zk403/mlearn)](https://github.com/zk403/mlearn/blob/master/LICENSE)
+[![License](https://img.shields.io/github/license/zk403/mlearn)](https://github.com/zk403/mlearn/blob/main/LICENSE)
 [![Build Status](https://github.com/zk403/mlearn/actions/workflows/python-test.yml/badge.svg)](https://github.com/zk403/mlearn/actions/workflows/python-test.yml)
 [![codecov](https://codecov.io/gh/zk403/mlearn/main/graphs/badge.svg)](https://app.codecov.io/gh/zk403/mlearn)
 [![PyPI release](https://img.shields.io/pypi/v/BDMLtools.svg)](https://pypi.python.org/pypi/BDMLtools)
 
 BDMLtools是适用于常见商业数据分析数据挖掘场景下，中小数据量的二分类模型的机器学习建模工具包。
 本模组将集成商业分析场景中二分类模型中常用的机器学习模型，并使之能够兼顾模型开发效率、报告制作与建模流程标准化。
 本模组涵盖数据清洗、数据探索、特征工程、评分卡制作、模型评估、统计学逐步回归、机器学习模型及其参数优化等内容
@@ -44,15 +44,14 @@
 
 ```
 pip uninstall BDMLtools
 ```
 
 更新
 ```
-v0.3.6
-1.优化代码，移除对xgboost与catboost库的依赖
-2.优化代码，对sklearn的最低依赖降低为1.0.2
-3.修复了shapcheck中的使用catboost时无法计算的bug
-4.修复了EDAreport在pandas==2.0.1版本下的bug
+v0.3.7
+1.新增支持二分类focal loss的损失函数FocalLoss
+2.新增支持二分类focal loss的lightgbm类FLLGBMSklearn
+3.新增支持二分类focal loss下lightgbm的贝叶斯搜索类FLBSTuner
+4.新增支持二分类focal loss下lightgbm的网格搜素、随机搜索类FLgridTuner
 5.更新单元测试脚本,更新部分代码说明
-6.更新example
 ```
```

### Comparing `BDMLtools-0.3.6/setup.py` & `BDMLtools-0.3.7/setup.py`

 * *Files identical despite different names*

### Comparing `BDMLtools-0.3.6/test/test_base.py` & `BDMLtools-0.3.7/test/test_base.py`

 * *Files identical despite different names*

### Comparing `BDMLtools-0.3.6/test/test_clearner.py` & `BDMLtools-0.3.7/test/test_clearner.py`

 * *Files identical despite different names*

### Comparing `BDMLtools-0.3.6/test/test_eval.py` & `BDMLtools-0.3.7/test/test_eval.py`

 * *Files identical despite different names*

### Comparing `BDMLtools-0.3.6/test/test_report.py` & `BDMLtools-0.3.7/test/test_report.py`

 * *Files identical despite different names*

### Comparing `BDMLtools-0.3.6/test/test_selector.py` & `BDMLtools-0.3.7/test/test_selector.py`

 * *Files identical despite different names*

### Comparing `BDMLtools-0.3.6/test/test_tunner.py` & `BDMLtools-0.3.7/test/test_tunner.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 # -*- coding: utf-8 -*-
 """
 Created on Wed Jul 13 10:00:29 2022
 
 @author: zengke
 """
 
-from BDMLtools.tuner import gridTuner,hgridTuner
-from BDMLtools.tuner import BayesianCVTuner
+from BDMLtools.tuner import gridTuner,hgridTuner,FLgridTuner
+from BDMLtools.tuner import BayesianCVTuner,FLBSTuner
 from BDMLtools.tuner.fun import shapCheck
 from xgboost import XGBClassifier
 from lightgbm import LGBMClassifier
 from catboost import CatBoostClassifier
 from scipy.stats import randint as sp_randint
 from scipy.stats import uniform as sp_uniform 
 import pandas as pd
@@ -250,15 +250,95 @@
     res=hgridTuner(CatBoostClassifier,para_space_random,method='h_random',n_jobs=1,cv=2,n_candidates=1,
               validation_fraction=0.1,early_stopping_rounds=None).fit(X,y)  
     res=hgridTuner(CatBoostClassifier,para_space_random,method='h_random',n_jobs=1,cv=2,n_candidates=1,
               validation_fraction=None,early_stopping_rounds=10).fit(X,y)  
     res=hgridTuner(CatBoostClassifier,para_space_random,method='h_random',n_jobs=1,cv=2,n_candidates=1,
               validation_fraction=None,early_stopping_rounds=None,calibration=True).fit(X,y)  
     res.predict_proba(X);res.predict_score(X)      
+
+
+def test_FLgridTuner():    
+    
+
+    X=pd.DataFrame(
+            {
+             'a':[1,2,2,4,5,1,2,2,4,5,1,2,2,4,5,1,2,2,4,5],
+             'b':[1,2,3,4,5,1,2,3,4,5,1,2,3,4,5,1,2,3,4,5],
+             'c':['1','1','1','2','1','1','1','1','2','1','1','1','1','2','1','1','1','1','2','1']},
+            )
+    y=pd.Series([0,0,1,1,1,0,0,1,1,1,0,0,1,1,1,0,0,1,1,1],name='y')
+
+    para_space_gird={ 'boosting_type':['goss'], 
+                        'n_estimators':[10],
+                        'learning_rate':[0.1],                        
+                        'max_depth':[3],
+                        'min_split_gain': [0],                       
+                        'subsample':[1],
+                        'colsample_bytree' :[1],
+                        'reg_lambda':[0], 
+                         }
+    
+    
+    FLgridTuner(para_space=para_space_gird,gamma=2,alpha=0.2,method='grid',
+              scoring='roc_auc',eval_metric='auc',n_jobs=1,cv=2,
+              validation_fraction=None,early_stopping_rounds=None).fit(X,y)
+    
+    FLgridTuner(para_space=para_space_gird,gamma=0,alpha=None,method='grid',scoring='roc_auc',
+                eval_metric='auc',n_jobs=1,cv=2,        
+                validation_fraction=0.1,early_stopping_rounds=20).fit(X,y)
     
+    FLgridTuner(para_space_gird,gamma=2,alpha=0.2,method='grid',scoring='negfocalloss',eval_metric='negfocalloss',
+              n_jobs=1,cv=2,validation_fraction=None,early_stopping_rounds=None).fit(X,y)
+    
+    FLgridTuner(para_space_gird,gamma=2,alpha=0.2,method='grid',scoring='negfocalloss',eval_metric='negfocalloss',n_jobs=1,cv=2,             
+              validation_fraction=0.1,early_stopping_rounds=10).fit(X,y)
+    
+    FLgridTuner(para_space_gird,gamma=2,alpha=0.2,method='grid',scoring='negfocalloss',eval_metric='negfocalloss',n_jobs=1,cv=2,
+              validation_fraction=0.1,early_stopping_rounds=10,calibration=True).fit(X,y)    
+    
+
+    res=FLgridTuner(para_space_gird,gamma=2,alpha=0.2,method='grid',scoring='roc_auc',eval_metric='auc',n_jobs=1,cv=2,
+                    validation_fraction=None,early_stopping_rounds=None,calibration=True).fit(X,y)
+    
+    res.predict_proba(X);res.predict_score(X)    
+    
+    para_space_random={  
+                     'boosting_type':['gbdt','goss'], #'goss','gbdt'
+                     'n_estimators':sp_randint(low=100,high=110),
+                     'learning_rate':sp_uniform(loc=0.1,scale=0),                    
+                     'max_depth':sp_randint(low=2,high=4),#[0,∞],
+                     'min_split_gain': sp_uniform(loc=0,scale=0),
+                     'min_child_weight': sp_uniform(loc=0,scale=0),           
+                     'subsample':sp_uniform(loc=0.5,scale=0.5),
+                     'colsample_bytree' :sp_uniform(loc=0.5,scale=0.5),
+                     'reg_lambda':sp_uniform(loc=0,scale=20),
+                         }   
+    
+    FLgridTuner(para_space_random,gamma=2,alpha=0.2,method='random_grid',
+              scoring='roc_auc',eval_metric='auc',n_jobs=1,cv=2,
+              validation_fraction=None,early_stopping_rounds=None).fit(X,y)
+    
+    FLgridTuner(para_space_random,gamma=0,alpha=None,method='random_grid',scoring='roc_auc',
+                eval_metric='auc',n_jobs=1,cv=2,        
+                validation_fraction=0.1,early_stopping_rounds=20).fit(X,y)
+    
+    FLgridTuner(para_space_random,gamma=2,alpha=0.2,method='random_grid',scoring='negfocalloss',eval_metric='negfocalloss',
+              n_jobs=1,cv=2,validation_fraction=None,early_stopping_rounds=None).fit(X,y)
+    
+    FLgridTuner(para_space_random,gamma=2,alpha=0.2,method='random_grid',scoring='negfocalloss',eval_metric='negfocalloss',n_jobs=1,cv=2,             
+              validation_fraction=0.1,early_stopping_rounds=10).fit(X,y)
+    
+    FLgridTuner(para_space_random,gamma=2,alpha=0.2,method='random_grid',scoring='negfocalloss',eval_metric='negfocalloss',n_jobs=1,cv=2,
+              validation_fraction=0.1,early_stopping_rounds=10,calibration=True).fit(X,y)    
+    
+
+    res=FLgridTuner(para_space_random,gamma=2,alpha=0.2,method='random_grid',scoring='roc_auc',eval_metric='auc',n_jobs=1,cv=2,
+                    validation_fraction=None,early_stopping_rounds=None,calibration=True).fit(X,y)
+    
+    res.predict_proba(X);res.predict_score(X)       
     
     
 
 def test_BayesianCVTuner():    
     
     X=pd.DataFrame(
         {
@@ -314,14 +394,55 @@
                     init_points=1,n_iter=1,
                     validation_fraction=None,early_stopping_rounds=10).fit(X,y)      
     res=BayesianCVTuner(CatBoostClassifier,scoring='roc_auc',eval_metric='auc',n_jobs=1,cv=2,
                     init_points=1,n_iter=1,
                     validation_fraction=None,early_stopping_rounds=None,calibration=True).fit(X,y)      
     res.predict_proba(X);res.predict_score(X)
     
+    
+    
+def test_FLBSTuner():    
+    
+
+    X=pd.DataFrame(
+            {
+             'a':[1,2,2,4,5,1,2,2,4,5,1,2,2,4,5,1,2,2,4,5],
+             'b':[1,2,3,4,5,1,2,3,4,5,1,2,3,4,5,1,2,3,4,5],
+             'c':['1','1','1','2','1','1','1','1','2','1','1','1','1','2','1','1','1','1','2','1']},
+            )
+    y=pd.Series([0,0,1,1,1,0,0,1,1,1,0,0,1,1,1,0,0,1,1,1],name='y')
+    
+    FLBSTuner(gamma=2,alpha=0.2,scoring='roc_auc',eval_metric='auc',n_jobs=1,cv=2,
+              init_points=1,n_iter=1,
+              validation_fraction=None,early_stopping_rounds=None).fit(X,y)
+    
+    FLBSTuner(gamma=0,alpha=None,scoring='roc_auc',eval_metric='auc',n_jobs=1,cv=2,
+              init_points=1,n_iter=1,
+              validation_fraction=0.1,early_stopping_rounds=20).fit(X,y)
+    
+    FLBSTuner(gamma=2,alpha=0.2,scoring='negfocalloss',eval_metric='negfocalloss',n_jobs=1,cv=2,
+              init_points=1,n_iter=1,
+              validation_fraction=None,early_stopping_rounds=None).fit(X,y)
+    
+    FLBSTuner(gamma=2,alpha=0.2,scoring='negfocalloss',eval_metric='negfocalloss',n_jobs=1,cv=2,
+              init_points=1,n_iter=1,
+              validation_fraction=0.1,early_stopping_rounds=10).fit(X,y)
+    
+    FLBSTuner(gamma=2,alpha=0.2,scoring='negfocalloss',eval_metric='negfocalloss',n_jobs=1,cv=2,
+              init_points=1,n_iter=1,
+              validation_fraction=0.1,early_stopping_rounds=10,calibration=True).fit(X,y)    
+    
+
+    res=FLBSTuner(gamma=2,alpha=0.2,scoring='roc_auc',eval_metric='auc',n_jobs=1,cv=2,
+                    init_points=1,n_iter=1,
+                    validation_fraction=None,early_stopping_rounds=None,calibration=True).fit(X,y)
+    
+    res.predict_proba(X);res.predict_score(X)
+
+    
 
 @mock.patch('matplotlib.pyplot.show')
 def test_shapcheck(mock_show):
     
     X=pd.DataFrame(
         {
          'a':[1,2,2,4,5,1,2,2,4,5,1,2,2,4,5,1,2,2,4,5],
```

