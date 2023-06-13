# Comparing `tmp/pz-rail-flexzboost-0.0.9.tar.gz` & `tmp/pz-rail-flexzboost-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pz-rail-flexzboost-0.0.9.tar", last modified: Thu May  4 05:17:19 2023, max compression
+gzip compressed data, was "pz-rail-flexzboost-0.1.0.tar", last modified: Tue Jun 13 20:32:48 2023, max compression
```

## Comparing `pz-rail-flexzboost-0.0.9.tar` & `pz-rail-flexzboost-0.1.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:17:19.146789 pz-rail-flexzboost-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-04 05:17:04.000000 pz-rail-flexzboost-0.0.9/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:17:19.138789 pz-rail-flexzboost-0.0.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:17:19.142789 pz-rail-flexzboost-0.0.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-05-04 05:17:04.000000 pz-rail-flexzboost-0.0.9/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-04 05:17:04.000000 pz-rail-flexzboost-0.0.9/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-05-04 05:17:04.000000 pz-rail-flexzboost-0.0.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-04 05:17:04.000000 pz-rail-flexzboost-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-04 05:17:19.146789 pz-rail-flexzboost-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-04 05:17:04.000000 pz-rail-flexzboost-0.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:17:19.142789 pz-rail-flexzboost-0.0.9/archive/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-04 05:17:04.000000 pz-rail-flexzboost-0.0.9/archive/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-04 05:17:04.000000 pz-rail-flexzboost-0.0.9/archive/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-04 05:17:04.000000 pz-rail-flexzboost-0.0.9/archive/x_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-04 05:17:04.000000 pz-rail-flexzboost-0.0.9/archive/x_setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:17:19.138789 pz-rail-flexzboost-0.0.9/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:17:19.142789 pz-rail-flexzboost-0.0.9/docs/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)    12042 2023-05-04 05:17:04.000000 pz-rail-flexzboost-0.0.9/docs/notebooks/fzboost_pdf_representation_comparison.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-05-04 05:17:04.000000 pz-rail-flexzboost-0.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 05:17:19.146789 pz-rail-flexzboost-0.0.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:17:19.138789 pz-rail-flexzboost-0.0.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:17:19.142789 pz-rail-flexzboost-0.0.9/src/pz_rail_flexzboost.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-04 05:17:19.000000 pz-rail-flexzboost-0.0.9/src/pz_rail_flexzboost.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-04 05:17:19.000000 pz-rail-flexzboost-0.0.9/src/pz_rail_flexzboost.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 05:17:19.000000 pz-rail-flexzboost-0.0.9/src/pz_rail_flexzboost.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-04 05:17:19.000000 pz-rail-flexzboost-0.0.9/src/pz_rail_flexzboost.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-04 05:17:19.000000 pz-rail-flexzboost-0.0.9/src/pz_rail_flexzboost.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:17:19.138789 pz-rail-flexzboost-0.0.9/src/rail/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:17:19.138789 pz-rail-flexzboost-0.0.9/src/rail/estimation/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:17:19.142789 pz-rail-flexzboost-0.0.9/src/rail/estimation/algos/
--rw-r--r--   0 runner    (1001) docker     (123)    11071 2023-05-04 05:17:04.000000 pz-rail-flexzboost-0.0.9/src/rail/estimation/algos/flexzboost.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:17:19.146789 pz-rail-flexzboost-0.0.9/src/rail/flexzboost/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-04 05:17:04.000000 pz-rail-flexzboost-0.0.9/src/rail/flexzboost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-04 05:17:19.000000 pz-rail-flexzboost-0.0.9/src/rail/flexzboost/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:17:19.146789 pz-rail-flexzboost-0.0.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7288 2023-05-04 05:17:04.000000 pz-rail-flexzboost-0.0.9/tests/test_algos.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:32:48.260604 pz-rail-flexzboost-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-13 20:32:37.000000 pz-rail-flexzboost-0.1.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:32:48.256605 pz-rail-flexzboost-0.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:32:48.256605 pz-rail-flexzboost-0.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-06-13 20:32:37.000000 pz-rail-flexzboost-0.1.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-13 20:32:37.000000 pz-rail-flexzboost-0.1.0/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-06-13 20:32:37.000000 pz-rail-flexzboost-0.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-13 20:32:37.000000 pz-rail-flexzboost-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-13 20:32:48.260604 pz-rail-flexzboost-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-13 20:32:37.000000 pz-rail-flexzboost-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:32:48.256605 pz-rail-flexzboost-0.1.0/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-13 20:32:37.000000 pz-rail-flexzboost-0.1.0/archive/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-13 20:32:37.000000 pz-rail-flexzboost-0.1.0/archive/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-13 20:32:37.000000 pz-rail-flexzboost-0.1.0/archive/x_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-13 20:32:37.000000 pz-rail-flexzboost-0.1.0/archive/x_setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:32:48.256605 pz-rail-flexzboost-0.1.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:32:48.256605 pz-rail-flexzboost-0.1.0/docs/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)    12042 2023-06-13 20:32:37.000000 pz-rail-flexzboost-0.1.0/docs/notebooks/fzboost_pdf_representation_comparison.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-06-13 20:32:37.000000 pz-rail-flexzboost-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 20:32:48.260604 pz-rail-flexzboost-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:32:48.256605 pz-rail-flexzboost-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:32:48.256605 pz-rail-flexzboost-0.1.0/src/pz_rail_flexzboost.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-13 20:32:48.000000 pz-rail-flexzboost-0.1.0/src/pz_rail_flexzboost.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-13 20:32:48.000000 pz-rail-flexzboost-0.1.0/src/pz_rail_flexzboost.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 20:32:48.000000 pz-rail-flexzboost-0.1.0/src/pz_rail_flexzboost.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-13 20:32:48.000000 pz-rail-flexzboost-0.1.0/src/pz_rail_flexzboost.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-13 20:32:48.000000 pz-rail-flexzboost-0.1.0/src/pz_rail_flexzboost.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:32:48.256605 pz-rail-flexzboost-0.1.0/src/rail/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:32:48.256605 pz-rail-flexzboost-0.1.0/src/rail/estimation/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:32:48.256605 pz-rail-flexzboost-0.1.0/src/rail/estimation/algos/
+-rw-r--r--   0 runner    (1001) docker     (123)    13115 2023-06-13 20:32:37.000000 pz-rail-flexzboost-0.1.0/src/rail/estimation/algos/flexzboost.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:32:48.256605 pz-rail-flexzboost-0.1.0/src/rail/flexzboost/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-13 20:32:37.000000 pz-rail-flexzboost-0.1.0/src/rail/flexzboost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-13 20:32:48.000000 pz-rail-flexzboost-0.1.0/src/rail/flexzboost/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:32:48.260604 pz-rail-flexzboost-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7288 2023-06-13 20:32:37.000000 pz-rail-flexzboost-0.1.0/tests/test_algos.py
```

### Comparing `pz-rail-flexzboost-0.0.9/.github/workflows/main.yml` & `pz-rail-flexzboost-0.1.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-flexzboost-0.0.9/.github/workflows/publish-to-pypi.yml` & `pz-rail-flexzboost-0.1.0/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-flexzboost-0.0.9/.gitignore` & `pz-rail-flexzboost-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pz-rail-flexzboost-0.0.9/LICENSE` & `pz-rail-flexzboost-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pz-rail-flexzboost-0.0.9/PKG-INFO` & `pz-rail-flexzboost-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-flexzboost
-Version: 0.0.9
+Version: 0.1.0
 Summary: RAIL Flexzboost Interface
 Author-email: The LSST DESC PZ WG <samuel.j.schmidt@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pz-rail-flexzboost-0.0.9/archive/README.md` & `pz-rail-flexzboost-0.1.0/archive/README.md`

 * *Files identical despite different names*

### Comparing `pz-rail-flexzboost-0.0.9/archive/pypi.yaml` & `pz-rail-flexzboost-0.1.0/archive/pypi.yaml`

 * *Files identical despite different names*

### Comparing `pz-rail-flexzboost-0.0.9/docs/notebooks/fzboost_pdf_representation_comparison.ipynb` & `pz-rail-flexzboost-0.1.0/docs/notebooks/fzboost_pdf_representation_comparison.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-flexzboost-0.0.9/pyproject.toml` & `pz-rail-flexzboost-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -17,26 +17,26 @@
     "Programming Language :: Python :: 3.10",
     "Natural Language :: English",
     "Operating System :: POSIX"
 ]
 dynamic = ["version"]
 dependencies = [
     "flexcode",
-    "pz-rail",
+    "pandas",
+    "pz-rail-base",
+    "qp-prob[full]",
     "qp-flexzboost",
     "scikit-learn",
     "xgboost"
 ]
 
 [project.optional-dependencies]
 dev = [
     "coverage",
-    "ipykernel",
     "matplotlib",
-    "numpy",
     "pylint",
     "pytest",
     "pytest-cov",
     "yamllint",
 ]
 
 [build-system]
```

### Comparing `pz-rail-flexzboost-0.0.9/src/pz_rail_flexzboost.egg-info/PKG-INFO` & `pz-rail-flexzboost-0.1.0/src/pz_rail_flexzboost.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-flexzboost
-Version: 0.0.9
+Version: 0.1.0
 Summary: RAIL Flexzboost Interface
 Author-email: The LSST DESC PZ WG <samuel.j.schmidt@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pz-rail-flexzboost-0.0.9/src/pz_rail_flexzboost.egg-info/SOURCES.txt` & `pz-rail-flexzboost-0.1.0/src/pz_rail_flexzboost.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pz-rail-flexzboost-0.0.9/src/rail/estimation/algos/flexzboost.py` & `pz-rail-flexzboost-0.1.0/src/rail/estimation/algos/flexzboost.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,23 +3,24 @@
 XGBoost to learn the relation, split training data into train and
 validation set and find best "bump_thresh" (eliminate small peaks in
 p(z) below threshold) and sharpening parameter (determines peakiness of
 p(z) shape) via cde-loss over a grid.
 """
 
 import numpy as np
+import pandas as pd
 import qp
 import qp_flexzboost
 from ceci.config import StageParameter as Param
 from flexcode.helpers import make_grid
 from rail.estimation.estimator import CatEstimator, CatInformer
 from rail.core.common_params import SHARED_PARAMS
 
 
-def make_color_data(data_dict, bands, err_bands, ref_band, nondetect_val, maglimdict):
+def make_color_data(data_dict, bands, err_bands, ref_band):
     """
     make a dataset consisting of the i-band mag and the five colors.
 
     Parameters
     -----------
     data_dict : `ndarray`
       array of magnitudes and errors, with names mag_{bands[i]}_lsst
@@ -27,68 +28,45 @@
 
     Returns
     --------
     input_data : `ndarray`
       array of imag and 5 colors
     """
     input_data = data_dict[ref_band]
-    # make colors and append to input data
-    for i in range(len(bands)-1):
-        band1name = bands[i]
-        band2name = bands[i+1]
-        err1name = err_bands[i]
-        err2name = err_bands[i+1]
-        band1 = data_dict[band1name]
-        band1err = data_dict[err1name]
-        band2 = data_dict[band2name]
-        band2err = data_dict[err2name]
-        for j, xx in enumerate(band1):
-            if np.isnan(nondetect_val): # pragma: no cover
-                if np.isnan(xx):
-                    band1[j] = maglimdict[band1name]
-                    band1err[j] = 1.0
-            else:
-                if np.isclose(xx, nondetect_val, atol=.01):
-                    band1[j] = maglimdict[band1name]
-                    band1err[j] = 1.0
-        for j, xx in enumerate(band2):
-            if np.isnan(nondetect_val): # pragma: no cover
-                if np.isnan(xx):
-                    band2[j] = maglimdict[band2name]
-                    band2err[j] = 1.0
-            else:
-                if np.isclose(xx, 99., atol=0.01):  #pragma: no cover
-                    band2[j] = maglimdict[band2name]
-                    band2err[j] = 1.0
-
-        input_data = np.vstack((input_data, band1-band2))
-        color_err = np.sqrt((band1err)**2 + (band2err)**2)
-        input_data = np.vstack((input_data, color_err))
+    nbands = len(bands) - 1
+    for i in range(nbands):
+        color = data_dict[bands[i]] - data_dict[bands[i + 1]]
+        input_data = np.vstack((input_data, color))
+        colorerr = np.sqrt(data_dict[err_bands[i]]**2 + data_dict[err_bands[i + 1]]**2)
+        np.vstack((input_data, colorerr))
     return input_data.T
 
 
-
 class Inform_FZBoost(CatInformer):
     """ Train a FZBoost CatEstimator
     """
     name = 'Inform_FZBoost'
     config_options = CatInformer.config_options.copy()
     config_options.update(zmin=SHARED_PARAMS,
                           zmax=SHARED_PARAMS,
                           nzbins=SHARED_PARAMS,
                           nondetect_val=SHARED_PARAMS,
                           mag_limits=SHARED_PARAMS,
                           bands=SHARED_PARAMS,
                           err_bands=SHARED_PARAMS,
                           ref_band=SHARED_PARAMS,
-                          redshift_col=SHARED_PARAMS,    
+                          redshift_col=SHARED_PARAMS,
+                          retrain_full=Param(bool, True, msg="if True, re-run the fit with the full training set, "
+                                             "including data set aside for bump/sharpen validation.  If False, only"
+                                             " use the subset defined via trainfrac fraction"),
                           trainfrac=Param(float, 0.75,
                                           msg="fraction of training "
                                           "data to use for training (rest used for bump thresh "
                                           "and sharpening determination)"),
+                          seed=Param(int, 1138, msg="Random number seed"),
                           bumpmin=Param(float, 0.02,
                                         msg="minimum value in grid of "
                                         "thresholds checked to optimize removal of spurious "
                                         "small bumps"),
                           bumpmax=Param(float, 0.35,
                                         msg="max value in grid checked "
                                             "for removal of small bumps"),
@@ -99,34 +77,33 @@
                           max_basis=Param(int, 35, msg="maximum number of basis funcitons to use in density estimate"),
                           basis_system=Param(str, 'cosine', msg="type of basis sytem to use with flexcode"),
                           regression_params=Param(dict, {'max_depth': 8, 'objective': 'reg:squarederror'},
                                                   msg="dictionary of options passed to flexcode, includes "
                                                   "max_depth (int), and objective, which should be set "
                                                   " to reg:squarederror"))
 
-
     def __init__(self, args, comm=None):
         """ Constructor
         Do CatInformer specific initialization, then check on bands """
         CatInformer.__init__(self, args, comm=comm)
         if self.config.ref_band not in self.config.bands:
             raise ValueError("ref_band not present in bands list! ")
 
     @staticmethod
-    def split_data(fz_data, sz_data, trainfrac):
+    def split_data(fz_data, sz_data, trainfrac, seed):
         """
         make a random partition of the training data into training and
         validation, validation data will be used to determine bump
         thresh and sharpen parameters.
         """
         nobs = fz_data.shape[0]
         ntrain = round(nobs * trainfrac)
         # set a specific seed for reproducibility
-        np.random.seed(1138)
-        perm = np.random.permutation(nobs)
+        rng = np.random.default_rng(seed=seed)
+        perm = rng.permutation(nobs)
         x_train = fz_data[perm[:ntrain], :]
         z_train = sz_data[perm[:ntrain]]
         x_val = fz_data[perm[ntrain:]]
         z_val = sz_data[perm[ntrain:]]
         return x_train, x_val, z_train, z_val
 
     def run(self):
@@ -134,24 +111,45 @@
         """
         import flexcode
         from flexcode.regression_models import XGBoost
         from flexcode.loss_functions import cde_loss
 
         if self.config.hdf5_groupname:
             training_data = self.get_data('input')[self.config.hdf5_groupname]
-        else:  #pragma: no cover
+        else:  # pragma: no cover
             training_data = self.get_data('input')
-        speczs = training_data[self.config['redshift_col']]
+        speczs = np.array(training_data[self.config['redshift_col']])
+
+        # replace nondetects
+        for bandname, errname in zip(self.config.bands, self.config.err_bands):
+            if np.isnan(self.config.nondetect_val):  # pragma: no cover
+                detmask = np.isnan(training_data[bandname])
+                if isinstance(training_data, pd.DataFrame):
+                    training_data.loc[detmask, bandname] = self.config.mag_limits[bandname]
+                    training_data.loc[detmask, errname] = 1.0
+                else:
+                    detmask = np.isnan(training_data[bandname])
+                    training_data[bandname][detmask] = self.config.mag_limits[bandname]
+                    training_data[errname][detmask] = 1.0
+            else:
+                detmask = np.isclose(training_data[bandname], self.config.nondetect_val, atol=0.01)
+                if isinstance(training_data, pd.DataFrame):  # pragma: no cover
+                    training_data.loc[detmask, bandname] = self.config.mag_limits[bandname]
+                    training_data.loc[detmask, errname] = 1.0
+                else:
+                    training_data[bandname][detmask] = self.config.mag_limits[bandname]
+                    training_data[errname][detmask] = 1.0
+
         print("stacking some data...")
         color_data = make_color_data(training_data, self.config.bands, self.config.err_bands,
-                                     self.config.ref_band, self.config.nondetect_val,
-                                     self.config.mag_limits)
+                                     self.config.ref_band)
         train_dat, val_dat, train_sz, val_sz = self.split_data(color_data,
                                                                speczs,
-                                                               self.config.trainfrac)
+                                                               self.config.trainfrac,
+                                                               self.config.seed)
         print("read in training data")
         model = flexcode.FlexCodeModel(XGBoost, max_basis=self.config.max_basis,
                                        basis_system=self.config.basis_system,
                                        z_min=self.config.zmin, z_max=self.config.zmax,
                                        regression_params=self.config.regression_params)
         print("fit the model...")
         model.fit(train_dat, train_sz)
@@ -175,14 +173,23 @@
             model.sharpen_alpha = sharp
             tmpcdes, z_grid = model.predict(val_dat, n_grid=301)
             tmploss = cde_loss(tmpcdes, z_grid, val_sz)
             if tmploss < bestloss:
                 bestloss = tmploss
                 bestsharp = sharp
         model.sharpen_alpha = bestsharp
+
+        # retrain with full dataset or not
+        if self.config.retrain_full:
+            print("Retraining with full training set...")
+            model.fit(color_data, speczs)
+        else:  # pragma: no cover
+            print(f"Skipping retraining, only fraction {self.config.trainfrac}"
+                  "of training data used when training model")
+
         self.model = model
         self.add_data('model', self.model)
 
 
 class FZBoost(CatEstimator):
     """FZBoost-based CatEstimator
     """
@@ -203,33 +210,54 @@
         CatEstimator.__init__(self, args, comm=comm)
         if self.config.ref_band not in self.config.bands:
             raise ValueError("ref_band not present in bands list! ")
         self.zgrid = None
 
     def _process_chunk(self, start, end, data, first):
         print(f"Process {self.rank} estimating PZ PDF for rows {start:,} - {end:,}")
+
+        # replace nondetects
+        for bandname, errname in zip(self.config.bands, self.config.err_bands):
+            if np.isnan(self.config.nondetect_val):  # pragma: no cover
+                detmask = np.isnan(data[bandname])
+                if isinstance(data, pd.DataFrame):
+                    data.loc[detmask, bandname] = self.config.mag_limits[bandname]
+                    data.loc[detmask, errname] = 1.0
+                else:
+                    detmask = np.isnan(data[bandname])
+                    data[bandname][detmask] = self.config.mag_limits[bandname]
+                    data[errname][detmask] = 1.0
+            else:
+                detmask = np.isclose(data[bandname], self.config.nondetect_val, atol=0.01)
+                if isinstance(data, pd.DataFrame):  # pragma: no cover
+                    data.loc[detmask, bandname] = self.config.mag_limits[bandname]
+                    data.loc[detmask, errname] = 1.0
+                else:
+                    data[bandname][detmask] = self.config.mag_limits[bandname]
+                    data[errname][detmask] = 1.0
+
         color_data = make_color_data(data, self.config.bands, self.config.err_bands,
-                                     self.config.ref_band, self.config.nondetect_val,
-                                     self.config.mag_limits)
+                                     self.config.ref_band)
 
         if self.config.qp_representation == 'interp':
             pdfs, z_grid = self.model.predict(color_data, n_grid=self.config.nzbins)
             self.zgrid = np.array(z_grid).flatten()
+            zmode = np.expand_dims(self.zgrid[np.argmax(pdfs, axis=1)], -1)
             qp_dstn = qp.Ensemble(qp.interp, data=dict(xvals=self.zgrid, yvals=pdfs))
 
         elif self.config.qp_representation == 'flexzboost':
             basis_coefficients = self.model.predict_coefs(color_data)
             qp_dstn = qp.Ensemble(qp_flexzboost.flexzboost_create_from_basis_coef_object,
                                   data=dict(weights=basis_coefficients.coefs,
                                             basis_coefficients_object=basis_coefficients))
 
             # `make_grid` is a helper function from Flexcode that will create a nested
             # array of linearly spaced values. We then flatten that nested array.
             # so the final output will have the form `[0.0, 0.1, ..., 3.0]`.
             self.zgrid = np.array(make_grid(self.config.nzbins, basis_coefficients.z_min, basis_coefficients.z_max)).flatten()
+            zmode = qp_dstn.mode(grid=self.zgrid)
 
         else:
             raise ValueError(f"Unknown qp_representation in config: {self.config.qp_representation}. Should be one of [interp|flexzboost]")
 
-        zmode = qp_dstn.mode(grid=self.zgrid)
         qp_dstn.set_ancil(dict(zmode=zmode))
         self._do_chunk_output(qp_dstn, start, end, first)
```

### Comparing `pz-rail-flexzboost-0.0.9/tests/test_algos.py` & `pz-rail-flexzboost-0.1.0/tests/test_algos.py`

 * *Files identical despite different names*

