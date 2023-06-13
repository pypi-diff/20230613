# Comparing `tmp/Calkulate-3.0.1.tar.gz` & `tmp/Calkulate-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\Calkulate-3.0.1.tar", last modified: Wed Sep 23 08:59:44 2020, max compression
+gzip compressed data, was "dist\Calkulate-3.1.0.tar", last modified: Tue Oct 27 09:25:35 2020, max compression
```

## Comparing `Calkulate-3.0.1.tar` & `Calkulate-3.1.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2020-09-23 08:59:44.552699 Calkulate-3.0.1/
-drwxrwxrwx   0        0        0        0 2020-09-23 08:59:44.525881 Calkulate-3.0.1/Calkulate.egg-info/
--rw-rw-rw-   0        0        0     3368 2020-09-23 08:59:44.000000 Calkulate-3.0.1/Calkulate.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      614 2020-09-23 08:59:44.000000 Calkulate-3.0.1/Calkulate.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-09-23 08:59:44.000000 Calkulate-3.0.1/Calkulate.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       75 2020-09-23 08:59:44.000000 Calkulate-3.0.1/Calkulate.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2020-09-23 08:59:44.000000 Calkulate-3.0.1/Calkulate.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3368 2020-09-23 08:59:44.552699 Calkulate-3.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2245 2020-09-15 12:31:59.000000 Calkulate-3.0.1/README.md
-drwxrwxrwx   0        0        0        0 2020-09-23 08:59:44.538698 Calkulate-3.0.1/calkulate/
--rw-rw-rw-   0        0        0     2023 2020-09-23 08:55:08.000000 Calkulate-3.0.1/calkulate/__init__.py
--rw-rw-rw-   0        0        0      321 2020-09-10 09:46:23.000000 Calkulate-3.0.1/calkulate/constants.py
--rw-rw-rw-   0        0        0     1956 2020-09-14 09:58:37.000000 Calkulate-3.0.1/calkulate/convert.py
-drwxrwxrwx   0        0        0        0 2020-09-23 08:59:44.545697 Calkulate-3.0.1/calkulate/datasets/
--rw-rw-rw-   0        0        0      491 2020-09-14 10:00:48.000000 Calkulate-3.0.1/calkulate/datasets/__init__.py
--rw-rw-rw-   0        0        0     2658 2020-09-15 09:42:23.000000 Calkulate-3.0.1/calkulate/datasets/dataset.py
--rw-rw-rw-   0        0        0    11501 2020-09-23 08:03:14.000000 Calkulate-3.0.1/calkulate/datasets/get.py
--rw-rw-rw-   0        0        0     2865 2020-09-14 09:59:17.000000 Calkulate-3.0.1/calkulate/datasets/quantify.py
--rw-rw-rw-   0        0        0     2122 2020-09-11 08:42:43.000000 Calkulate-3.0.1/calkulate/datasets/read.py
--rw-rw-rw-   0        0        0     2238 2020-09-09 14:46:19.000000 Calkulate-3.0.1/calkulate/density.py
--rw-rw-rw-   0        0        0      451 2020-09-14 08:52:08.000000 Calkulate-3.0.1/calkulate/options.py
--rw-rw-rw-   0        0        0     2971 2020-09-14 06:44:48.000000 Calkulate-3.0.1/calkulate/simulate.py
--rw-rw-rw-   0        0        0    10564 2020-09-14 09:58:18.000000 Calkulate-3.0.1/calkulate/solvers.py
-drwxrwxrwx   0        0        0        0 2020-09-23 08:59:44.551699 Calkulate-3.0.1/calkulate/titrations/
--rw-rw-rw-   0        0        0      105 2020-09-15 06:56:07.000000 Calkulate-3.0.1/calkulate/titrations/__init__.py
--rw-rw-rw-   0        0        0     1717 2020-09-15 09:45:25.000000 Calkulate-3.0.1/calkulate/titrations/read.py
--rw-rw-rw-   0        0        0       88 2020-09-11 12:32:02.000000 Calkulate-3.0.1/calkulate/titrations/titration.py
--rw-rw-rw-   0        0        0      914 2020-09-11 08:13:41.000000 Calkulate-3.0.1/calkulate/titrations/write.py
--rw-rw-rw-   0        0        0      315 2020-09-23 08:59:44.553703 Calkulate-3.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1100 2020-09-15 12:23:24.000000 Calkulate-3.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2020-10-27 09:25:35.833277 Calkulate-3.1.0/
+drwxrwxrwx   0        0        0        0 2020-10-27 09:25:35.817278 Calkulate-3.1.0/Calkulate.egg-info/
+-rw-rw-rw-   0        0        0     3388 2020-10-27 09:25:35.000000 Calkulate-3.1.0/Calkulate.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      614 2020-10-27 09:25:35.000000 Calkulate-3.1.0/Calkulate.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2020-10-27 09:25:35.000000 Calkulate-3.1.0/Calkulate.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2020-10-27 09:25:35.000000 Calkulate-3.1.0/Calkulate.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2020-10-27 09:25:35.000000 Calkulate-3.1.0/Calkulate.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3388 2020-10-27 09:25:35.833277 Calkulate-3.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2265 2020-09-23 09:08:06.000000 Calkulate-3.1.0/README.md
+drwxrwxrwx   0        0        0        0 2020-10-27 09:25:35.825277 Calkulate-3.1.0/calkulate/
+-rw-rw-rw-   0        0        0     2023 2020-10-26 09:21:56.000000 Calkulate-3.1.0/calkulate/__init__.py
+-rw-rw-rw-   0        0        0      321 2020-09-10 09:46:23.000000 Calkulate-3.1.0/calkulate/constants.py
+-rw-rw-rw-   0        0        0     2079 2020-10-26 16:00:03.000000 Calkulate-3.1.0/calkulate/convert.py
+drwxrwxrwx   0        0        0        0 2020-10-27 09:25:35.829277 Calkulate-3.1.0/calkulate/datasets/
+-rw-rw-rw-   0        0        0      491 2020-09-14 10:00:48.000000 Calkulate-3.1.0/calkulate/datasets/__init__.py
+-rw-rw-rw-   0        0        0     2658 2020-09-15 09:42:23.000000 Calkulate-3.1.0/calkulate/datasets/dataset.py
+-rw-rw-rw-   0        0        0    12210 2020-10-26 16:07:05.000000 Calkulate-3.1.0/calkulate/datasets/get.py
+-rw-rw-rw-   0        0        0     2865 2020-09-14 09:59:17.000000 Calkulate-3.1.0/calkulate/datasets/quantify.py
+-rw-rw-rw-   0        0        0     2122 2020-09-11 08:42:43.000000 Calkulate-3.1.0/calkulate/datasets/read.py
+-rw-rw-rw-   0        0        0     2238 2020-09-09 14:46:19.000000 Calkulate-3.1.0/calkulate/density.py
+-rw-rw-rw-   0        0        0      451 2020-09-14 08:52:08.000000 Calkulate-3.1.0/calkulate/options.py
+-rw-rw-rw-   0        0        0     3604 2020-10-26 15:37:45.000000 Calkulate-3.1.0/calkulate/simulate.py
+-rw-rw-rw-   0        0        0    10567 2020-10-26 14:51:59.000000 Calkulate-3.1.0/calkulate/solvers.py
+drwxrwxrwx   0        0        0        0 2020-10-27 09:25:35.833277 Calkulate-3.1.0/calkulate/titrations/
+-rw-rw-rw-   0        0        0      105 2020-09-15 06:56:07.000000 Calkulate-3.1.0/calkulate/titrations/__init__.py
+-rw-rw-rw-   0        0        0     1717 2020-09-15 09:45:25.000000 Calkulate-3.1.0/calkulate/titrations/read.py
+-rw-rw-rw-   0        0        0       88 2020-09-11 12:32:02.000000 Calkulate-3.1.0/calkulate/titrations/titration.py
+-rw-rw-rw-   0        0        0      914 2020-09-11 08:13:41.000000 Calkulate-3.1.0/calkulate/titrations/write.py
+-rw-rw-rw-   0        0        0      315 2020-10-27 09:25:35.834277 Calkulate-3.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1098 2020-10-26 09:27:24.000000 Calkulate-3.1.0/setup.py
```

### Comparing `Calkulate-3.0.1/Calkulate.egg-info/PKG-INFO` & `Calkulate-3.1.0/Calkulate.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: Calkulate
-Version: 3.0.1
+Version: 3.1.0
 Summary: Seawater total alkalinity from titration data
 Home-page: https://github.com/mvdh7/calkulate
 Author: Humphreys, Matthew P. and Matthews, Ruth S.
 Author-email: m.p.humphreys@icloud.com
 License: UNKNOWN
 Description: # Calkulate
         
         [![PyPI version](https://badge.fury.io/py/Calkulate.svg)](https://badge.fury.io/py/Calkulate)
         [![DOI](https://img.shields.io/badge/DOI-10.5281%2Fzenodo.2634304-informational)](https://doi.org/10.5281/zenodo.2634304)
-        [![Docs](https://readthedocs.org/projects/calkulate/badge/?version=v3&style=flat)](https://calkulate.readthedocs.io/en/v3/)
-        [![Build Status](https://travis-ci.org/mvdh7/calkulate.svg?branch=v3)](https://travis-ci.org/mvdh7/calkulate)
-        [![Coverage](https://github.com/mvdh7/calkulate/blob/v3/misc/coverage.svg)](https://github.com/mvdh7/calkulate/blob/v3/misc/coverage.txt)
+        [![Docs](https://readthedocs.org/projects/calkulate/badge/?version=latest&style=flat)](https://calkulate.readthedocs.io/en/latest/)
+        [![Build Status](https://travis-ci.org/mvdh7/calkulate.svg?branch=master)](https://travis-ci.org/mvdh7/calkulate)
+        [![Coverage](https://github.com/mvdh7/calkulate/blob/master/misc/coverage.svg)](https://github.com/mvdh7/calkulate/blob/master/misc/coverage.txt)
         [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
         [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
         
         Calkulate is a Python package for finding total alkalinity from titration data using [PyCO2SYS](https://PyCO2SYS.rtfd.io).
         
         ## Installation
```

### Comparing `Calkulate-3.0.1/Calkulate.egg-info/SOURCES.txt` & `Calkulate-3.1.0/Calkulate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Calkulate-3.0.1/PKG-INFO` & `Calkulate-3.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: Calkulate
-Version: 3.0.1
+Version: 3.1.0
 Summary: Seawater total alkalinity from titration data
 Home-page: https://github.com/mvdh7/calkulate
 Author: Humphreys, Matthew P. and Matthews, Ruth S.
 Author-email: m.p.humphreys@icloud.com
 License: UNKNOWN
 Description: # Calkulate
         
         [![PyPI version](https://badge.fury.io/py/Calkulate.svg)](https://badge.fury.io/py/Calkulate)
         [![DOI](https://img.shields.io/badge/DOI-10.5281%2Fzenodo.2634304-informational)](https://doi.org/10.5281/zenodo.2634304)
-        [![Docs](https://readthedocs.org/projects/calkulate/badge/?version=v3&style=flat)](https://calkulate.readthedocs.io/en/v3/)
-        [![Build Status](https://travis-ci.org/mvdh7/calkulate.svg?branch=v3)](https://travis-ci.org/mvdh7/calkulate)
-        [![Coverage](https://github.com/mvdh7/calkulate/blob/v3/misc/coverage.svg)](https://github.com/mvdh7/calkulate/blob/v3/misc/coverage.txt)
+        [![Docs](https://readthedocs.org/projects/calkulate/badge/?version=latest&style=flat)](https://calkulate.readthedocs.io/en/latest/)
+        [![Build Status](https://travis-ci.org/mvdh7/calkulate.svg?branch=master)](https://travis-ci.org/mvdh7/calkulate)
+        [![Coverage](https://github.com/mvdh7/calkulate/blob/master/misc/coverage.svg)](https://github.com/mvdh7/calkulate/blob/master/misc/coverage.txt)
         [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
         [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
         
         Calkulate is a Python package for finding total alkalinity from titration data using [PyCO2SYS](https://PyCO2SYS.rtfd.io).
         
         ## Installation
```

### Comparing `Calkulate-3.0.1/README.md` & `Calkulate-3.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Calkulate
 
 [![PyPI version](https://badge.fury.io/py/Calkulate.svg)](https://badge.fury.io/py/Calkulate)
 [![DOI](https://img.shields.io/badge/DOI-10.5281%2Fzenodo.2634304-informational)](https://doi.org/10.5281/zenodo.2634304)
-[![Docs](https://readthedocs.org/projects/calkulate/badge/?version=v3&style=flat)](https://calkulate.readthedocs.io/en/v3/)
-[![Build Status](https://travis-ci.org/mvdh7/calkulate.svg?branch=v3)](https://travis-ci.org/mvdh7/calkulate)
-[![Coverage](https://github.com/mvdh7/calkulate/blob/v3/misc/coverage.svg)](https://github.com/mvdh7/calkulate/blob/v3/misc/coverage.txt)
+[![Docs](https://readthedocs.org/projects/calkulate/badge/?version=latest&style=flat)](https://calkulate.readthedocs.io/en/latest/)
+[![Build Status](https://travis-ci.org/mvdh7/calkulate.svg?branch=master)](https://travis-ci.org/mvdh7/calkulate)
+[![Coverage](https://github.com/mvdh7/calkulate/blob/master/misc/coverage.svg)](https://github.com/mvdh7/calkulate/blob/master/misc/coverage.txt)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 Calkulate is a Python package for finding total alkalinity from titration data using [PyCO2SYS](https://PyCO2SYS.rtfd.io).
 
 ## Installation
```

### Comparing `Calkulate-3.0.1/calkulate/__init__.py` & `Calkulate-3.1.0/calkulate/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
 calibrate_and_solve = calkulate
 
 
 # Package metadata
 _authorlist = ["Humphreys, Matthew P.", "Matthews, Ruth S."]
 __author__ = " and ".join(_authorlist)
-__version__ = "3.0.1"
+__version__ = "3.1.0"
 
 
 def say_hello():
     """Report the version number."""
     print(
         r"""
    .--.     . .         .      .
```

### Comparing `Calkulate-3.0.1/calkulate/convert.py` & `Calkulate-3.1.0/calkulate/convert.py`

 * *Files 13% similar despite different names*

```diff
@@ -55,16 +55,20 @@
     "total_sulfate": "TSO4",
     "k_ammonia": "KNH3",
     "k_borate": "KB",
     "k_bisulfate": "KSO4",
     "k_carbonic_1": "K1",
     "k_carbonic_2": "K2",
     "k_fluoride": "KF",
-    "k_phosphate_1": "KP1",
-    "k_phosphate_2": "KP2",
-    "k_phosphate_3": "KP3",
+    "k_phosphoric_1": "KP1",
+    "k_phosphoric_2": "KP2",
+    "k_phosphoric_3": "KP3",
     "k_silicate": "KSi",
     "k_sulfide": "KH2S",
     "k_water": "KW",
+    "k_alpha": "k_alpha",
+    "k_beta": "k_beta",
+    "total_alpha": "total_alpha",
+    "total_beta": "total_beta",
 }
 
 pyco2_to_calk = {v: k for k, v in calk_to_pyco2.items()}
```

### Comparing `Calkulate-3.0.1/calkulate/datasets/dataset.py` & `Calkulate-3.1.0/calkulate/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `Calkulate-3.0.1/calkulate/datasets/get.py` & `Calkulate-3.1.0/calkulate/datasets/get.py`

 * *Files 4% similar despite different names*

```diff
@@ -153,17 +153,20 @@
     """Make sure there is a molinity value for the undiluted analyte for every salt."""
     for salt in [
         "dic",
         "total_silicate",
         "total_phosphate",
         "total_ammonia",
         "total_sulfide",
+        "total_alpha",
+        "total_beta",
     ]:
         if salt not in dataset:
             dataset[salt] = 0
+        dataset[salt] = np.where(np.isnan(dataset[salt]), 0, dataset[salt])
     if "opt_k_carbonic" not in dataset:
         dataset["opt_k_carbonic"] = options.pyco2_opt_k_carbonic
     else:
         dataset["opt_k_carbonic"] = np.where(
             np.isnan(dataset.opt_k_carbonic),
             options.pyco2_opt_k_carbonic,
             dataset.opt_k_carbonic,
@@ -209,14 +212,16 @@
                 "total_silicate",
                 "total_phosphate",
                 "total_ammonia",
                 "total_sulfide",
                 "total_sulfate",
                 "total_borate",
                 "total_fluoride",
+                "total_alpha",
+                "total_beta",
             ]:
                 row.titration[salt] = row[salt] * row.titration.dilution_factor
 
 
 def get_titration_totals(dataset):
     """Get molinities of all salts throughout each titration."""
     dataset.apply(_get_titration_totals, axis=1)
@@ -231,36 +236,40 @@
 
 
 def _get_k_constants(row):
     if row.titration is not None:
         if "titrant_mass" in row.titration:
             totals = {
                 "Sal": row.salinity,
-                "TNH3": row.titration.total_ammonia.values,
-                "TPO4": row.titration.total_phosphate.values,
-                "TSi": row.titration.total_silicate.values,
-                "TH2S": row.titration.total_sulfide.values,
-                "TB": row.titration.total_borate.values,
-                "TF": row.titration.total_fluoride.values,
-                "TSO4": row.titration.total_sulfate.values,
+                "TNH3": row.titration.total_ammonia.values * 1e-6,
+                "TPO4": row.titration.total_phosphate.values * 1e-6,
+                "TSi": row.titration.total_silicate.values * 1e-6,
+                "TH2S": row.titration.total_sulfide.values * 1e-6,
+                "TB": row.titration.total_borate.values * 1e-6,
+                "TF": row.titration.total_fluoride.values * 1e-6,
+                "TSO4": row.titration.total_sulfate.values * 1e-6,
+                "alpha": row.titration.total_alpha.values * 1e-6,
+                "beta": row.titration.total_beta.values * 1e-6,
             }
             k_constants = {}
             for k in [
                 "k_ammonia",
                 "k_borate",
                 "k_bisulfate",
                 "k_carbonic_1",
                 "k_carbonic_2",
                 "k_fluoride",
-                "k_phosphate_1",
-                "k_phosphate_2",
-                "k_phosphate_3",
+                "k_phosphoric_1",
+                "k_phosphoric_2",
+                "k_phosphoric_3",
                 "k_silicate",
                 "k_sulfide",
                 "k_water",
+                "k_alpha",
+                "k_beta",
             ]:
                 if k in row:
                     if ~np.isnan(row[k]):
                         k_constants[convert.calk_to_pyco2[k]] = row[k]
             k_constants = pyco2.equilibria.assemble(
                 row.titration.temperature,
                 0,  # pressure
@@ -308,9 +317,17 @@
         dataset["opt_gas_constant"] = options.pyco2_opt_gas_constant
     else:
         dataset["opt_gas_constant"] = np.where(
             np.isnan(dataset.opt_gas_constant),
             options.pyco2_opt_gas_constant,
             dataset.opt_gas_constant,
         )
+    for extra in ["alpha", "beta"]:
+        k_extra = "k_" + extra
+        if k_extra not in dataset:
+            dataset[k_extra] = 1e-7
+        else:
+            dataset[k_extra] = np.where(
+                np.isnan(dataset[k_extra]), 1e-7, dataset[k_extra],
+            )
     dataset.apply(_get_k_constants, axis=1)
     return dataset
```

### Comparing `Calkulate-3.0.1/calkulate/datasets/quantify.py` & `Calkulate-3.1.0/calkulate/datasets/quantify.py`

 * *Files identical despite different names*

### Comparing `Calkulate-3.0.1/calkulate/datasets/read.py` & `Calkulate-3.1.0/calkulate/datasets/read.py`

 * *Files identical despite different names*

### Comparing `Calkulate-3.0.1/calkulate/density.py` & `Calkulate-3.1.0/calkulate/density.py`

 * *Files identical despite different names*

### Comparing `Calkulate-3.0.1/calkulate/simulate.py` & `Calkulate-3.1.0/calkulate/simulate.py`

 * *Files 21% similar despite different names*

```diff
@@ -12,27 +12,31 @@
     TB = titration["total_borate"] * 1e-6
     TSO4 = titration["total_sulfate"] * 1e-6
     TF = titration["total_fluoride"] * 1e-6
     TPO4 = titration["total_phosphate"] * 1e-6
     TSi = titration["total_silicate"] * 1e-6
     TNH3 = titration["total_ammonia"] * 1e-6
     TH2S = titration["total_sulfide"] * 1e-6
+    total_alpha = titration["total_alpha"] * 1e-6
+    total_beta = titration["total_beta"] * 1e-6
     # Unpack equilibrium constants (should all be on the Free scale)
     KW = titration["k_water"]
     K1 = titration["k_carbonic_1"]
     K2 = titration["k_carbonic_2"]
     KB = titration["k_borate"]
     KSO4 = titration["k_bisulfate"]
     KF = titration["k_fluoride"]
-    KP1 = titration["k_phosphate_1"]
-    KP2 = titration["k_phosphate_2"]
-    KP3 = titration["k_phosphate_3"]
+    KP1 = titration["k_phosphoric_1"]
+    KP2 = titration["k_phosphoric_2"]
+    KP3 = titration["k_phosphoric_3"]
     KSi = titration["k_silicate"]
     KNH3 = titration["k_ammonia"]
     KH2S = titration["k_sulfide"]
+    k_alpha = titration["k_alpha"]
+    k_beta = titration["k_beta"]
     # Calculate components
     h = 10.0 ** -pH
     hydroxide = KW / h
     aqueous_CO2 = TCO2 / (1 + K1 / h + K1 * K2 / h ** 2)
     bicarbonate = K1 * aqueous_CO2 / h
     carbonate = K2 * bicarbonate / h
     borate = TB * KB / (KB + h)
@@ -41,14 +45,21 @@
     phosphoric_denom = h ** 3 + KP1 * h ** 2 + KP1 * KP2 * h + KP1 * KP2 * KP3
     phosphoric_0 = TPO4 * h ** 3 / phosphoric_denom
     phosphoric_2 = TPO4 * KP1 * KP2 * h / phosphoric_denom
     phosphoric_3 = TPO4 * KP1 * KP2 * KP3 / phosphoric_denom
     silicate = TSi * KSi / (KSi + h)
     ammonia = TNH3 * KNH3 / (KNH3 + h)
     hydrogen_sulfide = TH2S * KH2S / (KH2S + h)
+    zlp = 4.5  # pK of 'zero level of protons' [WZK07]
+    alpha = total_alpha * k_alpha / (k_alpha + h)
+    alphaH = total_alpha - alpha
+    beta = total_beta * k_beta / (k_beta + h)
+    betaH = total_beta - beta
+    alk_alpha = np.where(-np.log10(k_alpha) <= zlp, -alphaH, alpha)
+    alk_beta = np.where(-np.log10(k_beta) <= zlp, -betaH, beta)
     return {
         "H": h,
         "OH": hydroxide,
         "CO2": aqueous_CO2,
         "HCO3": bicarbonate,
         "CO3": carbonate,
         "BOH4": borate,
@@ -56,14 +67,16 @@
         "HF": hydrogen_fluoride,
         "H3PO4": phosphoric_0,
         "HPO4": phosphoric_2,
         "PO4": phosphoric_3,
         "SiOOH3": silicate,
         "NH3": ammonia,
         "HS": hydrogen_sulfide,
+        "alk_alpha": alk_alpha,
+        "alk_beta": alk_beta,
     }
 
 
 # Multipliers for each component in the alkalinity equation.
 # Keys correspond to the output dict of alkalinity_components().
 component_multipliers = {
     "H": -1,
@@ -75,14 +88,16 @@
     "HF": -1,
     "H3PO4": -1,
     "HPO4": +1,
     "PO4": +2,
     "SiOOH3": +1,
     "NH3": +1,
     "HS": +1,
+    "alk_alpha": +1,
+    "alk_beta": +1,
 }
 
 
 def alkalinity(pH, titration):
     """Estimate total alkalinity from [H+] and total salts."""
     components = alkalinity_components(pH, titration)
     return np.sum([v * components[k] for k, v in component_multipliers.items()], axis=0)
```

### Comparing `Calkulate-3.0.1/calkulate/solvers.py` & `Calkulate-3.1.0/calkulate/solvers.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,17 +166,17 @@
 #         for k in [
 #             "k_ammonia",
 #             "k_borate",
 #             "k_bisulfate",
 #             "k_carbonic_1",
 #             "k_carbonic_2",
 #             "k_fluoride",
-#             "k_phosphate_1",
-#             "k_phosphate_2",
-#             "k_phosphate_3",
+#             "k_phosphoric_1",
+#             "k_phosphoric_2",
+#             "k_phosphoric_3",
 #             "k_silicate",
 #             "k_sulfide",
 #             "k_water",
 #         ]
 #     }
 #     k_constants = pyco2.convert.get_pHfactor_to_Free(
 #         titration["temperature"].values,
```

### Comparing `Calkulate-3.0.1/calkulate/titrations/read.py` & `Calkulate-3.1.0/calkulate/titrations/read.py`

 * *Files identical despite different names*

### Comparing `Calkulate-3.0.1/calkulate/titrations/write.py` & `Calkulate-3.1.0/calkulate/titrations/write.py`

 * *Files identical despite different names*

### Comparing `Calkulate-3.0.1/setup.py` & `Calkulate-3.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,19 +10,19 @@
     author=calk.__author__,
     author_email="m.p.humphreys@icloud.com",
     description="Seawater total alkalinity from titration data",
     url="https://github.com/mvdh7/calkulate",
     packages=setuptools.find_packages(),
     install_requires=[
         "numpy>=1.17",
-        "PyCO2SYS>=1.5.1",
-        "scipy>=1.4",
+        "PyCO2SYS>=1.6.0",
+        "scipy>=1.5",
         "pandas>=1",
-        "xlrd>=1.2",
-        "matplotlib>=3.2",
+        "xlrd>=1",
+        "matplotlib>=3.3",
     ],
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Programming Language :: Python :: 3.8",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
```

