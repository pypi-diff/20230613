# Comparing `tmp/optim_esm_tools-0.1.0.tar.gz` & `tmp/optim_esm_tools-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optim_esm_tools-0.1.0.tar", last modified: Fri Jun  2 06:15:50 2023, max compression
+gzip compressed data, was "optim_esm_tools-0.1.1.tar", last modified: Tue Jun 13 14:34:50 2023, max compression
```

## Comparing `optim_esm_tools-0.1.0.tar` & `optim_esm_tools-0.1.1.tar`

### file list

```diff
@@ -1,32 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:15:50.725039 optim_esm_tools-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-06-02 06:15:50.725039 optim_esm_tools-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-02 06:15:47.000000 optim_esm_tools-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:15:50.721038 optim_esm_tools-0.1.0/extra_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-02 06:15:47.000000 optim_esm_tools-0.1.0/extra_requirements/requirements-tests.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:15:50.725039 optim_esm_tools-0.1.0/optim_esm_tools/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-02 06:15:47.000000 optim_esm_tools-0.1.0/optim_esm_tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:15:50.725039 optim_esm_tools-0.1.0/optim_esm_tools/analyze/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-02 06:15:47.000000 optim_esm_tools-0.1.0/optim_esm_tools/analyze/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6067 2023-06-02 06:15:47.000000 optim_esm_tools-0.1.0/optim_esm_tools/analyze/analyze.py
--rw-r--r--   0 runner    (1001) docker     (123)    19190 2023-06-02 06:15:47.000000 optim_esm_tools-0.1.0/optim_esm_tools/analyze/cmip_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-02 06:15:47.000000 optim_esm_tools-0.1.0/optim_esm_tools/analyze/xarray_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:15:50.725039 optim_esm_tools-0.1.0/optim_esm_tools/synda_files/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-02 06:15:47.000000 optim_esm_tools-0.1.0/optim_esm_tools/synda_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-06-02 06:15:47.000000 optim_esm_tools-0.1.0/optim_esm_tools/synda_files/format_synda.py
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-06-02 06:15:47.000000 optim_esm_tools-0.1.0/optim_esm_tools/synda_files/synda_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     6809 2023-06-02 06:15:47.000000 optim_esm_tools-0.1.0/optim_esm_tools/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:15:50.725039 optim_esm_tools-0.1.0/optim_esm_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-06-02 06:15:50.000000 optim_esm_tools-0.1.0/optim_esm_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-02 06:15:50.000000 optim_esm_tools-0.1.0/optim_esm_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 06:15:50.000000 optim_esm_tools-0.1.0/optim_esm_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 06:15:50.000000 optim_esm_tools-0.1.0/optim_esm_tools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-02 06:15:50.000000 optim_esm_tools-0.1.0/optim_esm_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-02 06:15:50.000000 optim_esm_tools-0.1.0/optim_esm_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-02 06:15:50.725039 optim_esm_tools-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-06-02 06:15:47.000000 optim_esm_tools-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:15:50.725039 optim_esm_tools-0.1.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-02 06:15:47.000000 optim_esm_tools-0.1.0/test/test_basics.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-02 06:15:47.000000 optim_esm_tools-0.1.0/test/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-02 06:15:47.000000 optim_esm_tools-0.1.0/test/test_viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-06-02 06:15:47.000000 optim_esm_tools-0.1.0/test/test_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-02 06:15:47.000000 optim_esm_tools-0.1.0/test/test_xarray_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:34:50.392854 optim_esm_tools-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-06-13 14:34:50.392854 optim_esm_tools-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-13 14:34:47.000000 optim_esm_tools-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:34:50.388853 optim_esm_tools-0.1.1/extra_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-13 14:34:47.000000 optim_esm_tools-0.1.1/extra_requirements/requirements-tests.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:34:50.392854 optim_esm_tools-0.1.1/optim_esm_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-13 14:34:47.000000 optim_esm_tools-0.1.1/optim_esm_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-06-13 14:34:47.000000 optim_esm_tools-0.1.1/optim_esm_tools/_test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:34:50.392854 optim_esm_tools-0.1.1/optim_esm_tools/analyze/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-13 14:34:47.000000 optim_esm_tools-0.1.1/optim_esm_tools/analyze/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-06-13 14:34:47.000000 optim_esm_tools-0.1.1/optim_esm_tools/analyze/analyze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-06-13 14:34:47.000000 optim_esm_tools-0.1.1/optim_esm_tools/analyze/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25487 2023-06-13 14:34:47.000000 optim_esm_tools-0.1.1/optim_esm_tools/analyze/cmip_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-13 14:34:47.000000 optim_esm_tools-0.1.1/optim_esm_tools/analyze/xarray_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:34:50.392854 optim_esm_tools-0.1.1/optim_esm_tools/synda_files/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-13 14:34:47.000000 optim_esm_tools-0.1.1/optim_esm_tools/synda_files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-06-13 14:34:47.000000 optim_esm_tools-0.1.1/optim_esm_tools/synda_files/format_synda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-06-13 14:34:47.000000 optim_esm_tools-0.1.1/optim_esm_tools/synda_files/synda_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7143 2023-06-13 14:34:47.000000 optim_esm_tools-0.1.1/optim_esm_tools/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:34:50.392854 optim_esm_tools-0.1.1/optim_esm_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-06-13 14:34:50.000000 optim_esm_tools-0.1.1/optim_esm_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-13 14:34:50.000000 optim_esm_tools-0.1.1/optim_esm_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 14:34:50.000000 optim_esm_tools-0.1.1/optim_esm_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 14:34:50.000000 optim_esm_tools-0.1.1/optim_esm_tools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-13 14:34:50.000000 optim_esm_tools-0.1.1/optim_esm_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-13 14:34:50.000000 optim_esm_tools-0.1.1/optim_esm_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-13 14:34:47.000000 optim_esm_tools-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-13 14:34:50.392854 optim_esm_tools-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-06-13 14:34:47.000000 optim_esm_tools-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:34:50.392854 optim_esm_tools-0.1.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-13 14:34:47.000000 optim_esm_tools-0.1.1/test/test_basics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-06-13 14:34:47.000000 optim_esm_tools-0.1.1/test/test_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-13 14:34:47.000000 optim_esm_tools-0.1.1/test/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-13 14:34:47.000000 optim_esm_tools-0.1.1/test/test_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-06-13 14:34:47.000000 optim_esm_tools-0.1.1/test/test_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-13 14:34:47.000000 optim_esm_tools-0.1.1/test/test_xarray_tools.py
```

### Comparing `optim_esm_tools-0.1.0/PKG-INFO` & `optim_esm_tools-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optim_esm_tools
-Version: 0.1.0
+Version: 0.1.1
 Summary: Tools for OptimESM
 Home-page: https://github.com/JoranAngevaare/optim_esm_tools
 Author: Joran R. Angevaare
 License: UNKNOWN
 Description: # OptimESM
         [![Coverage Status](https://coveralls.io/repos/github/JoranAngevaare/optim_esm_tools/badge.svg)](https://coveralls.io/github/JoranAngevaare/optim_esm_tools)
         
@@ -29,14 +29,15 @@
         * Upgrade CI/CD by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/19
         * Flexible loading by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/16
         * Initialize testing by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/20
         * Add test for synda viewer by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/28
         * fix lat lon handling by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/29
         
         **Full Changelog**: https://github.com/JoranAngevaare/optim_esm_tools/commits/v0.1.0
+        
 Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `optim_esm_tools-0.1.0/optim_esm_tools/analyze/analyze.py` & `optim_esm_tools-0.1.1/optim_esm_tools/analyze/analyze.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,50 +1,46 @@
+# -*- coding: utf-8 -*-
 """Scaffolding"""
 
-import optim_esm_tools as oet
-
-import pandas as pd
 import os
-from collections import defaultdict
 from functools import wraps
-from optim_esm_tools.synda_files import format_synda as st
+
 import matplotlib.pyplot as plt
 import xarray as xr
 import numpy as np
 
 
 def moving_average(a, n=3):
     ret = np.cumsum(a, dtype=float)
     ret[n:] = ret[n:] - ret[:-n]
-    return ret[n - 1:] / n
+    return ret[n - 1 :] / n
 
 
 def requires(*requirements, do_raise=True):
     def somedec_outer(fn):
         @wraps(fn)
         def somedec_inner(self, *args, **kwargs):
             missing = []
             for r in requirements:
                 if getattr(self, r, None) is None:
                     missing.append(r)
-            message = f'Missing \n\t' + "\n\t".join(missing)
+            message = f'Missing \n\t' + '\n\t'.join(missing)
             if do_raise and missing:
                 raise ValueError(message)
             elif missing:
                 print(message)
             response = fn(self, *args, **kwargs)
             return response
 
         return somedec_inner
 
     return somedec_outer
 
 
 class TippingCondition:
-
     @requires('pi_control', 'historical', 'scenario', do_raise=False)
     def i_mean_difference(self) -> dict:
         data_sets = 'pi_control', 'historical', 'scenario'
         result = {}
         for ds in data_sets:
             detrend = self.detrend(self.getattr(ds))
             result[ds] = (detrend[-1] - detrend[0]) / detrend[0]
@@ -53,15 +49,17 @@
     @requires('pi_control', 'historical', 'scenario', do_raise=False)
     def ii_std_difference(self) -> dict:
         data_sets = 'pi_control', 'historical', 'scenario'
         result = {}
         detrend_historical = self.detrend(self.historical)
         for ds in data_sets:
             detrend = self.detrend(self.getattr(ds))
-            result[ds] = np.max(np.abs(detrend - np.mean(detrend)) / np.std(detrend_historical))
+            result[ds] = np.max(
+                np.abs(detrend - np.mean(detrend)) / np.std(detrend_historical)
+            )
         return result
 
     @requires('pi_control', 'historical', 'scenario', do_raise=False)
     def iii_10yr_difference(self) -> dict:
         data_sets = 'pi_control', 'historical', 'scenario'
         result = {}
         for ds in data_sets:
@@ -93,25 +91,34 @@
 
         return result
 
     def show_time_series(self, dataset):
         data = self.time_series(dataset)
         plt.plot(data['time'], data[self.parameter], label='yearly')
         filter_width = self.filter_width
-        plt.plot(data['detrend_time'], data[f'detrend_{self.parameter}'], label='detrend')
+        plt.plot(
+            data['detrend_time'], data[f'detrend_{self.parameter}'], label='detrend'
+        )
         plt.legend()
         plt.ylabel(self.parameter)
 
     def getattr(self, k):
         return getattr(self, k)
 
 
 class TippingBase:
-    def __init__(self, pos, parameter, pi_control=None, historical=None, scenario=None,
-                 filter_width=10, ):
+    def __init__(
+        self,
+        pos,
+        parameter,
+        pi_control=None,
+        historical=None,
+        scenario=None,
+        filter_width=10,
+    ):
         self.pos = pos
         self.parameter = parameter
         self.filter_width = filter_width
         self.pi_control = self.xr_open(pi_control)
         self.historical = self.xr_open(historical)
         self.scenario = self.xr_open(scenario)
         self.check(do_raise=False)
@@ -133,14 +140,15 @@
     def xr_open(self, base):
         return xr.open_mfdataset(os.path.join(base, self.pos)).load()
 
 
 class Tipping(TippingBase, TippingCondition):
     pass
 
+
 # if __name__ == '__main__':
 #
 #     results = []
 #     for pos in tqdm.tqdm(positions):
 #         tip = Tipping(pos=pos, parameter='tas', **kw)
 #         res = dict(pos=pos)
 #         for k in 'i ii iii'.split():
```

### Comparing `optim_esm_tools-0.1.0/optim_esm_tools/analyze/cmip_handler.py` & `optim_esm_tools-0.1.1/optim_esm_tools/analyze/cmip_handler.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,29 @@
+# -*- coding: utf-8 -*-
 import optim_esm_tools as oet
 
 import os
 import xarray as xr
 import numpy as np
 
 import typing as ty
 import collections
 from warnings import warn
 from functools import wraps
-
-import matplotlib.pyplot as plt
-from matplotlib.gridspec import GridSpec
 import cartopy.crs as ccrs
+import matplotlib.pyplot as plt
+
+import datetime
 from immutabledict import immutabledict
 import xrft
 
 
-_seconds_to_year = 365.25*24*3600
+_seconds_to_year = 365.25 * 24 * 3600
 folder_fmt = 'model_group model scenario run domain variable grid version'.split()
-__OPTIM_VERSION__ = '0.1.7'
+__OPTIM_VERSION__ = '0.1.10'
 
 
 def _native_date_fmt(time_array: np.array, date: ty.Tuple[int, int, int]):
     """Create date object using the date formatting from the time-array"""
     if isinstance(time_array, xr.DataArray):
         return _native_date_fmt(time_array=time_array.values, date=date)
 
@@ -38,119 +39,136 @@
     base: str,
     variable_of_interest: ty.Tuple[str] = ('tas',),
     max_time: ty.Optional[ty.Tuple[int, int, int]] = (2100, 1, 1),
     min_time: ty.Optional[ty.Tuple[int, int, int]] = None,
     _time_var='time',
     _detrend_type='linear',
     _ma_window: int = 10,
-    _cache: bool = True
+    _cache: bool = True,
 ) -> xr.Dataset:
     """Read a dataset from a folder called "base".
 
     Args:
         base (str): Folder to load the data from
         variable_of_interest (ty.Tuple[str], optional): _description_. Defaults to ('tas',).
         _time_var (str, optional): Name of the time dimention. Defaults to 'time'.
         _detrend_type (str, optional): Type of detrending applied. Defaults to 'linear'.
         _ma_window (int, optional): Moving average window (assumed to be years). Defaults to 10.
         _cache (bool, optional): cache the dataset with it's extra fields to alow faster (re)loading. Defaults to True.
 
     Returns:
         xr.Dataset: An xarray dataset with the appropriate variables
     """
-    post_processed_file = os.path.join(
-        base,
-        f'{variable_of_interest}'
-        f'_{min_time if min_time else ""}'
-        f'_{max_time if max_time else ""}'
-        f'_ma{_ma_window}'
-        f'_optimesm_v{__OPTIM_VERSION__}.nc').replace('(', '').replace(')', '').replace(' ', '_').replace(',', '').replace('\'', '')
+    post_processed_file = (
+        os.path.join(
+            base,
+            f'{variable_of_interest}'
+            f'_{min_time if min_time else ""}'
+            f'_{max_time if max_time else ""}'
+            f'_ma{_ma_window}'
+            f'_optimesm_v{__OPTIM_VERSION__}.nc',
+        )
+        .replace('(', '')
+        .replace(')', '')
+        .replace(' ', '_')
+        .replace(',', '')
+        .replace('\'', '')
+    )
 
     if os.path.exists(post_processed_file) and _cache:
-        return oet.analyze.analyze.st.load_glob(post_processed_file)
+        return oet.synda_files.format_synda.load_glob(post_processed_file)
 
     data_path = os.path.join(base, 'merged.nc')
     if not os.path.exists(data_path):
         warn(f'No dataset at {data_path}')
         return None
 
-    data_set = oet.analyze.analyze.st.load_glob(data_path)
-    data_set = oet.analyze.analyze.st.recast(data_set)
+    data_set = oet.synda_files.format_synda.load_glob(data_path)
+    data_set = oet.synda_files.format_synda.recast(data_set)
 
     if min_time or max_time:
-        time_slice = [_native_date_fmt(data_set[_time_var], d)
-                      if d is not None else None
-                      for d in [min_time, max_time]]
+        time_slice = [
+            _native_date_fmt(data_set[_time_var], d) if d is not None else None
+            for d in [min_time, max_time]
+        ]
         data_set = data_set.sel(**{_time_var: slice(*time_slice)})
 
     # Detrend and run_mean on the fly
     for variable in variable_of_interest:
-
         # NB these are DataArrays not Datasets!
-        run_mean = data_set[variable].rolling(
-            time=_ma_window, center=True).mean()
+        run_mean = data_set[variable].rolling(time=_ma_window, center=True).mean()
         detrended = xrft.detrend(
-            data_set[variable], _time_var, detrend_type=_detrend_type)
-        detrended_run_mean = xrft.detrend(run_mean.dropna(
-            _time_var), _time_var, detrend_type=_detrend_type)
-
+            data_set[variable], _time_var, detrend_type=_detrend_type
+        )
+        detrended_run_mean = xrft.detrend(
+            run_mean.dropna(_time_var), _time_var, detrend_type=_detrend_type
+        )
+        detrended_run_mean.attrs['units'] = data_set[variable].attrs.get(
+            'units', '{units}'
+        )
         data_set[f'{variable}_run_mean_{_ma_window}'] = run_mean
         data_set[f'{variable}_detrend'] = detrended
         data_set[f'{variable}_detrend_run_mean_{_ma_window}'] = detrended_run_mean
 
     folders = base.split(os.sep)
 
     # start with -1 (for i==0)
-    metadata = {k: folders[-i-1] for i, k in enumerate(folder_fmt[::-1])
-                }
-    metadata['path'] = base
-    metadata['file'] = post_processed_file
+    metadata = {k: folders[-i - 1] for i, k in enumerate(folder_fmt[::-1])}
+    metadata.update(
+        dict(path=base, file=post_processed_file, running_mean_period=_ma_window)
+    )
+
     data_set.attrs.update(metadata)
 
     if _cache:
-        print(f'Write {post_processed_file}' + ' '*100, flush=True, end='\r')
+        print(f'Write {post_processed_file}' + ' ' * 100, flush=True, end='\r')
         data_set.to_netcdf(post_processed_file)
     return data_set
 
 
-def example_time_series(ds_combined: xr.Dataset, variable='tas') -> None:
+def example_time_series(ds_combined: xr.Dataset, variable='tas', _ma_window=10) -> None:
     """Make an example of time series based on datset
 
     Args:
         ds_combined (xr.Dataset): dataset
     """
     sel = dict(x=20, y=20)
     detrend_variable = f'{variable}_detrend'
-    detrend_variable_running_mean = f'{variable}_detrend_run_mean_10'
+    detrend_variable_running_mean = f'{variable}_detrend_run_mean_{_ma_window}'
     time = 'time'
 
     _, axes = plt.subplots(3, 1, figsize=(12, 10))
     plt.sca(axes[0])
 
     ds_combined.isel(**sel)[detrend_variable].plot(label='detrended')
-    ds_combined.isel(
-        **sel)[detrend_variable_running_mean].plot(label='detrended, runmean')
+    ds_combined.isel(**sel)[detrend_variable_running_mean].plot(
+        label='detrended, runmean'
+    )
     plt.legend()
 
     plt.sca(axes[1])
     # ds_combined.differentiate("time").isel(**sel)[variable].plot(label='detrended')
     ds_combined[detrend_variable_running_mean].dropna(time).differentiate(time).isel(
-        **sel).plot(label='detrended, runmean')
+        **sel
+    ).plot(label='detrended, runmean')
     plt.legend()
 
     plt.sca(axes[2])
     # ds_combined.differentiate("time").differentiate("time").isel(**sel)[variable].plot(label='detrended')
-    ds_combined[detrend_variable_running_mean].dropna(time).differentiate(time).differentiate(time).isel(
-        **sel).plot(label='detrended, runmean')
+    ds_combined[detrend_variable_running_mean].dropna(time).differentiate(
+        time
+    ).differentiate(time).isel(**sel).plot(label='detrended, runmean')
     plt.legend()
 
 
-def check_accepts(accepts: ty.Mapping[str, ty.Iterable] = immutabledict(unit=('absolute', 'std')),
-                  do_raise: bool = True):
-    """Wrapper for function if certain kwargs are from a defined list of variables. 
+def check_accepts(
+    accepts: ty.Mapping[str, ty.Iterable] = immutabledict(unit=('absolute', 'std')),
+    do_raise: bool = True,
+):
+    """Wrapper for function if certain kwargs are from a defined list of variables.
 
     Example:
         ```
             @check_accepts(accepts=dict(far=('boo', 'booboo')))
             def bla(far):
                 print(far)
 
@@ -164,14 +182,15 @@
         accepts (ty.Mapping[str, ty.Iterable], optional): which kwarg to accept a limited set of options.
             Defaults to immutabledict(unit=('absolute', 'std')).
         do_raise (bool, optional): if False, don't raise an error but just warn. Defaults to True.
 
     Returns:
         wrapped function
     """
+
     def somedec_outer(fn):
         @wraps(fn)
         def somedec_inner(*args, **kwargs):
             message = ''
             for k, v in kwargs.items():
                 if k in accepts and v not in accepts[k]:
                     message += f'{k} for {v} but only accepts {accepts[k]}'
@@ -183,55 +202,116 @@
             return response
 
         return somedec_inner
 
     return somedec_outer
 
 
+def apply_abs(apply=True, add_abs_to_name=True, _disable_kw='apply_abs'):
+    """Apply np.max() to output of function (if apply=True)
+    Disable in the function kwargs by using the _disable_kw argument
+
+    Example:
+        ```
+        @apply_abs(apply=True, add_abs_to_name=False)
+        def bla(a=1, **kw):
+            print(a, kw)
+            return a
+        assert bla(-1, apply_abs=True) == 1
+        assert bla(-1, apply_abs=False) == -1
+        assert bla(1) == 1
+        assert bla(1, apply_abs=False) == 1
+        ```
+    Args:
+        apply (bool, optional): apply np.abs. Defaults to True.
+        _disable_kw (str, optional): disable with this kw in the function. Defaults to 'apply_abs'.
+    """
+
+    def somedec_outer(fn):
+        @wraps(fn)
+        def somedec_inner(*args, **kwargs):
+            response = fn(*args, **kwargs)
+            do_abs = kwargs.get(_disable_kw)
+            if do_abs or (do_abs is None and apply):
+                if add_abs_to_name and isinstance(getattr(response, 'name'), str):
+                    response.name = f'Abs. {response.name}'
+                return np.abs(response)
+            return response
+
+        return somedec_inner
+
+    return somedec_outer
+
+
+def _remove_any_none_times(da, time_dim):
+    data_var = da.copy()
+    time_null = da.isnull().all(dim=set(da.dims) - {time_dim})
+    if np.any(time_null):
+        data_var = data_var.load().where(~time_null, drop=True)
+    return data_var
+
+
+@apply_abs()
 @check_accepts(accepts=dict(unit=('absolute', 'relative', 'std')))
-def running_mean_diff(data_set: xr.Dataset,
-                      variable: str = 'tas',
-                      time_var: str = 'time',
-                      naming: str = '{variable}_run_mean_10',
-                      rename_to: str = 'long_name',
-                      unit: str = 'absolute',
-                      _t_0_date: tuple = (2015, 1, 1),
-                      _t_1_date: tuple = (2100, 1, 1),
-                      ) -> xr.Dataset:
+def running_mean_diff(
+    data_set: xr.Dataset,
+    variable: str = 'tas',
+    time_var: str = 'time',
+    naming: str = '{variable}_run_mean_{running_mean}',
+    running_mean: int = 10,
+    rename_to: str = 'long_name',
+    unit: str = 'absolute',
+    apply_abs: bool = True,
+    _t_0_date: ty.Optional[tuple] = None,
+    _t_1_date: ty.Optional[tuple] = None,
+) -> xr.Dataset:
     """Return difference in running mean of data set
 
     Args:
-        data_set (xr.Dataset): data set
-        variable (str, optional): Defaults to 'tas'.
-        time_var (str, optional): Defaults to 'time_run_mean_10'.
-        naming (srt, optional): Defaults to '{variable}_run_mean_10'.
-        rename_to (str, optional): Defaults to 'long_name'.
-        unit (str, optional): Defaults to 'absolute'.
+        data_set (xr.Dataset):
+        variable (str, optional): . Defaults to 'tas'.
+        time_var (str, optional): . Defaults to 'time'.
+        naming (str, optional): . Defaults to '{variable}_run_mean_{running_mean}'.
+        running_mean (int, optional): . Defaults to 10.
+        rename_to (str, optional): . Defaults to 'long_name'.
+        unit (str, optional): . Defaults to 'absolute'.
+        apply_abs (bool, optional): . Defaults to True.
+        _t_0_date (ty.Optional[tuple], optional): . Defaults to (2015, 1, 1).
+        _t_1_date (ty.Optional[tuple], optional): . Defaults to (2100, 1, 1).
+
+    Raises:
+        ValueError: when no timestamps are not none?
 
     Returns:
-        xr.Dataset
+        xr.Dataset:
     """
-    var_name = naming.format(variable=variable)
+    var_name = naming.format(variable=variable, running_mean=running_mean)
     _time_values = data_set[time_var].dropna(time_var)
 
     if not len(_time_values):
         raise ValueError(f'No values for {time_var} in dataset?')
 
-    t_0 = _native_date_fmt(_time_values, _t_0_date)
-    t_1 = _native_date_fmt(_time_values, _t_1_date)
+    data_var = _remove_any_none_times(data_set[var_name], time_var)
 
-    data_t_0 = data_set[var_name].dropna(
-        time_var).sel(time=t_0, method='nearest')
-    data_t_1 = data_set[var_name].dropna(
-        time_var).sel(time=t_1, method='nearest')
+    if _t_0_date is not None:
+        t_0 = _native_date_fmt(_time_values, _t_0_date)
+        data_t_0 = data_var.sel(time=t_0, method='nearest')
+    else:
+        data_t_0 = data_var.isel(time=0)
+
+    if _t_0_date is not None:
+        t_1 = _native_date_fmt(_time_values, _t_1_date)
+        data_t_1 = data_var.sel(time=t_1, method='nearest')
+    else:
+        data_t_1 = data_var.isel(time=-1)
 
-    result = (data_t_1-data_t_0)
+    result = data_t_1 - data_t_0
     result = result.copy()
-    var_unit = data_set[variable].attrs.get('units', '{units}')
-    name = data_set[variable].attrs.get(rename_to, variable)
+    var_unit = data_var.attrs.get('units', '{units}')
+    name = data_var.attrs.get(rename_to, variable)
 
     if unit == 'absolute':
         result.name = f't[-1] - t[0] for {name} [{var_unit}]'
         return result
 
     if unit == 'relative':
         result = 100 * result / data_t_0
@@ -241,224 +321,248 @@
     # Redundant if just for clarity
     if unit == 'std':
         result = result / result.std()
         result.name = f't[-1] - t[0] for {name} [$\sigma$]'
         return result
 
 
+@apply_abs()
 @check_accepts(accepts=dict(unit=('absolute', 'relative', 'std')))
-def running_mean_std(data_set: xr.Dataset,
-                     variable: str = 'tas',
-                     time_var: str = 'time',
-                     naming: str = '{variable}_detrend_run_mean_10',
-                     rename_to: str = 'long_name',
-                     unit: str = 'absolute') -> xr.Dataset:
-    data_var = naming.format(variable=variable)
+def running_mean_std(
+    data_set: xr.Dataset,
+    variable: str = 'tas',
+    time_var: str = 'time',
+    naming: str = '{variable}_detrend_run_mean_{running_mean}',
+    running_mean: int = 10,
+    rename_to: str = 'long_name',
+    apply_abs: bool = True,
+    unit: str = 'absolute',
+) -> xr.Dataset:
+    data_var = naming.format(variable=variable, running_mean=running_mean)
     result = data_set[data_var].std(dim=time_var)
     result = result.copy()
     var_unit = data_set[data_var].attrs.get('units', '{units}')
     name = data_set[data_var].attrs.get(rename_to, variable)
 
     if unit == 'absolute':
         result.name = f'Std. {name} [{var_unit}]'
         return result
 
     if unit == 'relative':
-        result = result / data_set[data_var].mean(dim=time_var)
+        result = 100 * result / data_set[data_var].mean(dim=time_var)
         result.name = f'Relative Std. {name} [$\%$]'
         return result
 
     if unit == 'std':
         result = result / data_set[data_var].std()
         result.name = f'Std. {name} [$\sigma$]'
         return result
 
 
+@apply_abs()
 @check_accepts(accepts=dict(unit=('absolute', 'relative', 'std')))
 def max_change_xyr(
-        data_set: xr.Dataset,
-        variable: str = 'tas',
-        time_var: str = 'time',
-        naming: str = '{variable}_run_mean_10',
-        x_yr: ty.Union[int, float] = 10,
-        rename_to: str = 'long_name',
-        unit: str = 'absolute') -> xr.Dataset:
-    data_var = naming.format(variable=variable)
-    plus_10yr = data_set.isel({time_var: slice(x_yr, None)})[data_var]
-    to_min_10yr = data_set.isel({time_var: slice(None, -x_yr)})[data_var]
+    data_set: xr.Dataset,
+    variable: str = 'tas',
+    time_var: str = 'time',
+    naming: str = '{variable}_run_mean_{running_mean}',
+    x_yr: ty.Union[int, float] = 10,
+    running_mean: int = 10,
+    rename_to: str = 'long_name',
+    apply_abs: bool = True,
+    unit: str = 'absolute',
+) -> xr.Dataset:
+    data_var = naming.format(variable=variable, running_mean=running_mean)
+    plus_x_yr = data_set.isel({time_var: slice(x_yr, None)})[data_var]
+    to_min_x_yr = data_set.isel({time_var: slice(None, -x_yr)})[data_var]
 
-    # Keep the metadata (and time stamps of the to_min_10yr)
-    result = to_min_10yr.copy(data=plus_10yr.values - to_min_10yr.values)
+    # Keep the metadata (and time stamps of the to_min_x_yr)
+    result = to_min_x_yr.copy(data=plus_x_yr.values - to_min_x_yr.values)
 
     result = result.max(dim=time_var).copy()
     var_unit = data_set[data_var].attrs.get('units', '{units}')
     name = data_set[data_var].attrs.get(rename_to, variable)
 
     if unit == 'absolute':
         result.name = f'{x_yr} yr diff. {name} [{var_unit}]'
         return result
 
     if unit == 'relative':
-        result = 100 * result / to_min_10yr.mean(dim=time_var)
+        result = 100 * result / to_min_x_yr.mean(dim=time_var)
         result.name = f'{x_yr} yr diff. {name} [$\%$]'
         return result
 
     if unit == 'std':
         result = result / result.std()
         result.name = f'{x_yr} yr diff. {name} [$\sigma$]'
         return result
 
 
+@apply_abs()
 @check_accepts(accepts=dict(unit=('absolute', 'relative', 'std')))
 def max_derivative(
     data_set: xr.Dataset,
     variable: str = 'tas',
     time_var: str = 'time',
-    naming: str = '{variable}_run_mean_10',
+    naming: str = '{variable}_run_mean_{running_mean}',
+    running_mean: int = 10,
     rename_to: str = 'long_name',
+    apply_abs: bool = True,
     unit: str = 'absolute',
 ) -> xr.Dataset:
+    var_name = naming.format(variable=variable, running_mean=running_mean)
 
-    data_var = naming.format(variable=variable)
-    result = (data_set[data_var].dropna(time_var).differentiate(
-        time_var).max(dim=time_var)*_seconds_to_year).copy()
+    data_array = _remove_any_none_times(data_set[var_name], time_var)
+    result = data_array.differentiate(time_var).max(dim=time_var) * _seconds_to_year
 
-    var_unit = data_set[data_var].attrs.get('units', '{units}')
-    name = data_set[data_var].attrs.get(rename_to, variable)
+    var_unit = data_array.attrs.get('units', '{units}')
+    name = data_array.attrs.get(rename_to, variable)
 
     if unit == 'absolute':
         result.name = f'Max $\partial/\partial t$ {name} [{var_unit}/yr]'
         return result
 
     if unit == 'relative':
-        result = 100 * result / data_set[data_var].mean(dim=time_var)
+        result = 100 * result / data_array.mean(dim=time_var)
         result.name = f'Max $\partial/\partial t$ {name} [$\%$/yr]'
         return result
 
     if unit == 'std':
         # A local unit of sigma might be better X.std(dim=time_var)
-        result = result / data_set[data_var].std()
+        result = result / data_array.std()
         result.name = f'Max $\partial/\partial t$ {name} [$\sigma$/yr]'
         return result
 
 
-# TODO
-# Numerically instable? Maybe?
-def _max_double_derivative(
-    data_set,
-    variable='tas',
-    time_var='time',
-    naming='{variable}_run_mean_10',
-    rename_to='long_name',
-    unit='absolute'
-):
-
-    data_var = naming.format(variable=variable)
-    result = (data_set[data_var].dropna(time_var).differentiate(time_var).differentiate(time_var)
-              .max(dim=time_var)*(_seconds_to_year**2)).copy()
-
-    unit = data_set[data_var].attrs.get('units', '{units}')
-    name = data_set[data_var].attrs.get(rename_to, variable)
-    result.name = f'Max $\partial^2/\partial t^2$ {name} [{unit}/yr]'
-    return result
-
-
 class MapMaker(object):
     data_set: xr.Dataset
 
     # This is a bit rough, conditions is a mapping of keys to decsriptions and functions
     conditions: ty.Mapping[str, ty.Tuple] = immutabledict(
-        {'i ii iii iv v vi vii viii ix x'.split()[i]: props
-         for i, props in enumerate(
-             zip(
-                 ['Difference of running mean (10 yr) between start and end of time series. Not detrended',
-                  'Standard deviation of running mean (10 yr). Detrended',
-                  'Max change in 10 yr in the running mean (10 yr). Not detrended',
-                  'Max value of the first order derivative of the running mean. Not deterended',
-                  ],
-                 [running_mean_diff, running_mean_std,
-                     max_change_xyr, max_derivative]
-             ))})
+        {
+            'i ii iii iv v vi vii viii ix x'.split()[i]: props
+            for i, props in enumerate(
+                zip(
+                    [
+                        'Difference of running mean (10 yr) between start and end of time series. Not detrended',
+                        'Standard deviation of running mean (10 yr). Detrended',
+                        'Max change in 10 yr in the running mean (10 yr). Not detrended',
+                        'Max value of the first order derivative of the running mean. Not deterended',
+                    ],
+                    [
+                        running_mean_diff,
+                        running_mean_std,
+                        max_change_xyr,
+                        max_derivative,
+                    ],
+                )
+            )
+        }
+    )
 
     kw: ty.Mapping = immutabledict(
         fig=dict(dpi=200, figsize=(12, 8)),
         title=dict(fontsize=8),
         gridspec=dict(hspace=0.3),
         cbar=dict(orientation='horizontal', extend='both'),
         plot=dict(transform=ccrs.PlateCarree()),
     )
     normalizations: ty.Optional[ty.Mapping] = None
 
     _cache: bool = False
 
-    def __init__(self,
-                 data_set: xr.Dataset,
-                 normalizations: ty.Union[None,
-                                          ty.Mapping, ty.Iterable] = None,
-                 cache: bool = False):
+    def __init__(
+        self,
+        data_set: xr.Dataset,
+        normalizations: ty.Union[None, ty.Mapping, ty.Iterable] = None,
+        cache: bool = False,
+    ):
         self.data_set = data_set
         if normalizations is None:
-            self.normalizations = {i: [None, None]
-                                   for i in self.conditions.keys()}
+            self.normalizations = {i: [None, None] for i in self.conditions.keys()}
         elif isinstance(normalizations, collections.abc.Mapping):
             self.normalizations = normalizations
         elif isinstance(normalizations, collections.abc.Iterable):
             self.normalizations = {
-                i: normalizations[j] for j, i in enumerate(self.conditions.keys())}
+                i: normalizations[j] for j, i in enumerate(self.conditions.keys())
+            }
 
-        def _incorrect_format(): return (
-            any(not isinstance(v, collections.abc.Iterable)
-                for v in self.normalizations.values())
-            or any(len(v) != 2 for v in self.normalizations.values())
-            or any(k not in self.normalizations for k in self.conditions)
-        )
+        def _incorrect_format():
+            return (
+                any(
+                    not isinstance(v, collections.abc.Iterable)
+                    for v in self.normalizations.values()
+                )
+                or any(len(v) != 2 for v in self.normalizations.values())
+                or any(k not in self.normalizations for k in self.conditions)
+            )
 
         if self.normalizations is None or _incorrect_format():
-            raise TypeError(f'Normalizations should be mapping from'
-                            f'{self.conditions.keys()} to vmin, vmax, '
-                            f'got {self.normalizations} (from {normalizations})')
+            raise TypeError(
+                f'Normalizations should be mapping from'
+                f'{self.conditions.keys()} to vmin, vmax, '
+                f'got {self.normalizations} (from {normalizations})'
+            )
         self._cache = cache
 
     def plot(self, *a, **kw):
         print('Depricated use plot_all')
-        self.plot_all(*a, **kw)
+        return self.plot_all(*a, **kw)
 
-    def plot_all(self, nx,  fig=None, **kw,):
-        ny = np.ceil(len(self.conditions)/nx).astype(int)
+    def plot_all(
+        self,
+        nx=2,
+        fig=None,
+        **kw,
+    ):
+        ny = np.ceil(len(self.conditions) / nx).astype(int)
         if fig is None:
             fig = plt.figure(**self.kw['fig'])
+
+        from matplotlib.gridspec import GridSpec
+
         gs = GridSpec(nx, ny, **self.kw['gridspec'])
+        plt_axes = []
 
-        for i, (label, (_, _)) in enumerate(self.conditions.items()):
+        for i, label in enumerate(self.conditions.keys()):
             ax = fig.add_subplot(
-                gs[i], projection=ccrs.PlateCarree(central_longitude=0.0,))
-
-            plt_ax = self.plot_i(label, ax=ax, **kw)
+                gs[i],
+                projection=ccrs.PlateCarree(
+                    central_longitude=0.0,
+                ),
+            )
+            self.plot_i(label, ax=ax, **kw)
+            plt_axes.append(ax)
+        return plt_axes
 
     def plot_i(self, label, ax=None, coastlines=True, **kw):
         if ax is None:
             ax = plt.gca()
         if coastlines:
             ax.coastlines()
 
         prop = getattr(self, label)
 
         cmap = plt.get_cmap('viridis').copy()
         cmap.set_extremes(under='cyan', over='orange')
 
         c_kw = self.kw['cbar'].copy()
-        c_range_kw = {vm: self.normalizations[label][j]
-                      for j, vm in enumerate('vmin vmax'.split())}
-
-        for k, v in {**self.kw['plot'],
-                     **c_range_kw,
-                     **dict(cbar_kwargs=c_kw,
-                            cmap=cmap,
-                            )
-                     }.items():
+        c_range_kw = {
+            vm: self.normalizations[label][j]
+            for j, vm in enumerate('vmin vmax'.split())
+        }
+
+        for k, v in {
+            **self.kw['plot'],
+            **c_range_kw,
+            **dict(
+                cbar_kwargs=c_kw,
+                cmap=cmap,
+            ),
+        }.items():
             kw.setdefault(k, v)
 
         plt_ax = prop.plot(**kw)
 
         plt.xlim(-180, 180)
         plt.ylim(-90, 90)
         description = self.conditions[label][0]
@@ -466,15 +570,14 @@
         gl = ax.gridlines(draw_labels=True)
         gl.top_labels = False
         gl.right_labels = False
         return plt_ax
 
     def __getattr__(self, item):
         if item in self.conditions:
-
             _, function = self.conditions[item]
             key = f'_{item}'
             if self._cache:
                 if not isinstance(self._cache, dict):
                     self._cache = dict()
                 if key in self._cache:
                     data = self._cache.get(key)
@@ -483,54 +586,189 @@
             data = function(self.data_set)
             if self._cache or isinstance(self._cache, dict):
                 self._cache[key] = data.load()
             return data
 
         return self.__getattribute__(item)
 
-    def time_series(self, variable='tas'):
-        if variable != 'tas':
-            raise NotImplementedError('Currently only works for tas')
+    @staticmethod
+    def _ts_single(time_val, mean, std, plot_kw, fill_kw):
+        if fill_kw is None:
+            fill_kw = dict(alpha=0.4, step='mid')
+
+        l = mean.plot(**plot_kw)
+
+        if std is not None:
+            # TODO, make this more elegant!
+            # import cftime
+            # plt.fill_between(   [cftime.real_datetime(dd.year, dd.month, dd.day) for dd in time_val], mean - std, mean+std, **fill_kw)
+            (mean - std).plot(color=l[0]._color, alpha=0.4, drawstyle='steps-mid')
+            (mean + std).plot(color=l[0]._color, alpha=0.4, drawstyle='steps-mid')
+
+    def _ts(
+        self,
+        variable,
+        ds=None,
+        time='time',
+        other_dim=(),
+        running_mean=10,
+        fill_kw=None,
+        labels=dict(),
+        only_rm=False,
+        **plot_kw,
+    ):
+        if ds is None:
+            ds = self.data_set
+        if not only_rm:
+            mean, std = self._mean_and_std(ds, variable, other_dim)
+            # return mean, std
+            plot_kw['label'] = labels.get(variable, variable)
+            self._ts_single(ds[time].values, mean, std, plot_kw, fill_kw)
 
-        variable_rm = f'{variable}_run_mean_10'
-        variable_det = f'{variable}_detrend'
-        variable_det_rm = f'{variable}_detrend_run_mean_10'
-
-        time = 'time'
-        time_rm = time
-        ds = self.data_set.mean(dim=['x', 'y'])
-
-        _, axes = plt.subplots(3, 1,
-                               figsize=(12, 10),
-                               gridspec_kw=dict(hspace=0.3))
+        mean, std = self._mean_and_std(
+            ds, f'{variable}_run_mean_{running_mean}', other_dim
+        )
+        plot_kw['label'] = labels.get(
+            f'{variable}_run_mean_{running_mean}',
+            f'{variable} running mean {running_mean}',
+        )
+        self._ts_single(ds[time].values, mean, std, plot_kw, fill_kw)
 
-        plt.sca(axes[0])
-        ds[variable].plot(label='variable')
-        ds[variable_rm].plot(label='variable_rm')
         plt.ylabel('T [K]')
         plt.legend()
+        plt.title('')
 
-        plt.sca(axes[1])
-        ds[variable_det].plot(label='variable_det')
-        ds[variable_det_rm].plot(label='variable_det_rm')
+    def _det_ts(
+        self,
+        variable,
+        ds=None,
+        time='time',
+        other_dim=(),
+        running_mean=10,
+        fill_kw=None,
+        labels=dict(),
+        only_rm=False,
+        **plot_kw,
+    ):
+        if ds is None:
+            ds = self.data_set
+        if not only_rm:
+            mean, std = self._mean_and_std(ds, f'{variable}_detrend', other_dim)
+            plot_kw['label'] = labels.get(
+                f'{variable}_detrend', f'detrended {variable}'
+            )
+            self._ts_single(ds[time].values, mean, std, plot_kw, fill_kw)
+
+        mean, std = self._mean_and_std(
+            ds, f'{variable}_detrend_run_mean_{running_mean}', other_dim
+        )
+        plot_kw['label'] = labels.get(
+            f'{variable}_detrend_run_mean_{running_mean}',
+            f'detrended {variable} running mean {running_mean}',
+        )
+        self._ts_single(ds[time].values, mean, std, plot_kw, fill_kw)
         plt.ylabel('detrend(T) [K]')
         plt.legend()
+        plt.title('')
 
-        plt.sca(axes[2])
+    def _ddt_ts(
+        self,
+        variable,
+        ds=None,
+        time='time',
+        other_dim=(),
+        running_mean=10,
+        fill_kw=None,
+        labels=dict(),
+        only_rm=False,
+        **plot_kw,
+    ):
+        if ds is None:
+            ds = self.data_set
+        variable_rm = f'{variable}_run_mean_{running_mean}'
+
+        if not only_rm:
+            # Dropna should take care of any nones in the data-array
+            dy_dt = ds[variable].mean(other_dim).dropna(time).differentiate(time)
+            dy_dt *= _seconds_to_year
+            # mean, std = self._mean_and_std(dy_dt, variable=None, other_dim=other_dim)
+            # plot_kw['label'] = variable
+            # self._ts_single(ds[time].values, mean, std, plot_kw, fill_kw)
+            label = f'd/dt {labels.get(variable, variable)}'
+            dy_dt.plot(label=label, **plot_kw)
 
-        # Dropna should take care of any nones in the data-array
-        dy_dt = ds[variable].dropna(time).differentiate(time)
-        dy_dt *= _seconds_to_year
-        dy_dt.plot(label='d/dt variable')
-        dy_dt_rm = ds[variable_rm].dropna(time).differentiate(time_rm)
+        dy_dt_rm = ds[variable_rm].mean(other_dim).dropna(time).differentiate(time)
         dy_dt_rm *= _seconds_to_year
-        dy_dt_rm.plot(label='d/dt variable rm')
-        plt.ylim(dy_dt_rm.min()/1.05, dy_dt_rm.max()*1.05)
-        plt.ylabel('dT/dt [K/yr]')
+        label = (
+            f"d/dt {labels.get(variable_rm, f'{variable} running mean {running_mean}')}"
+        )
+        dy_dt_rm.plot(label=label, **plot_kw)
+        # mean, std = self._mean_and_std(dy_dt_rm, variable=None, other_dim=other_dim)
+        # plot_kw['label'] = variable
+        # self._ts_single(ds[time].values, mean, std, plot_kw, fill_kw)
+
+        plt.ylim(dy_dt_rm.min() / 1.05, dy_dt_rm.max() * 1.05)
+        plt.ylabel('$\partial T/\partial t$ [K/yr]')
         plt.legend()
+        plt.title('')
+
+    @staticmethod
+    def _mean_and_std(ds, variable, other_dim):
+        if variable is None:
+            da = ds
+        else:
+            da = ds[variable]
+        if other_dim is None:
+            return da.mean(other_dim), None
+        return da.mean(other_dim), da.std(other_dim)
+
+    def time_series(
+        self,
+        variable='tas',
+        time='time',
+        other_dim=('x', 'y'),
+        running_mean=10,
+        interval=True,
+        axes=None,
+        **kw,
+    ):
+        if variable != 'tas':
+            raise NotImplementedError('Currently only works for tas')
+
+        ds = self.data_set
+        if interval is False:
+            ds = ds.copy().mean(other_dim)
+            other_dim = None
+
+        plot_kw = dict(drawstyle='steps-mid', **kw)
+
+        if axes is None:
+            _, axes = plt.subplots(3, 1, figsize=(12, 10), gridspec_kw=dict(hspace=0.3))
+
+        plt.sca(axes[0])
+        self._ts(
+            variable, ds=ds, running_mean=running_mean, other_dim=other_dim, **plot_kw
+        )
+
+        plt.sca(axes[1])
+        self._det_ts(
+            variable, ds=ds, running_mean=running_mean, other_dim=other_dim, **plot_kw
+        )
+
+        plt.sca(axes[2])
+        self._ddt_ts(
+            variable,
+            ds=ds,
+            time=time,
+            running_mean=running_mean,
+            other_dim=other_dim,
+            **plot_kw,
+        )
+
+        return axes
 
     @property
     def ds(self):
         warn('MapMaker.ds is depricated, use MapMaker.data_set')
         return self.data_set
```

### Comparing `optim_esm_tools-0.1.0/optim_esm_tools/analyze/xarray_tools.py` & `optim_esm_tools-0.1.1/optim_esm_tools/analyze/xarray_tools.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,37 @@
+# -*- coding: utf-8 -*-
 import numba
 import numpy as np
 
 
-def _mask2d_to_xy_slice(mask: np.array, cyclic:bool=False)->np.array:
+def _mask2d_to_xy_slice(mask: np.array, cyclic: bool = False) -> np.array:
     where = np.argwhere(mask)
     slices = np.zeros((len(mask), 2, 2), dtype=np.int64)
     n_slices = 1
     slices[0][0][0] = where[0][0]
-    slices[0][0][1] = where[0][0] + 1 
+    slices[0][0][1] = where[0][0] + 1
     slices[0][1][0] = where[0][1]
     slices[0][1][1] = where[0][1] + 1
-    
+
     for x, y in where[1:]:
         # x1 and y1 are EXLCUSIVE!
         for s_i, ((x0, x1), (y0, y1)) in enumerate(slices[:n_slices]):
             if x0 <= x <= x1 and y0 <= y <= y1:
                 if x == x1:
                     slices[s_i][0][1] += 1
                 if y == y1:
                     slices[s_i][1][1] += 1
                 if cyclic:
                     raise ValueError
                 break
         else:
             slices[n_slices][0][0] = x
             slices[n_slices][0][1] = x + 1
-            
+
             slices[n_slices][1][0] = y
             slices[n_slices][1][1] = y + 1
-            
+
             n_slices += 1
     return slices[:n_slices]
 
 
-mask2d_to_xy_slice = numba.njit(_mask2d_to_xy_slice)
+mask2d_to_xy_slice = numba.njit(_mask2d_to_xy_slice)
```

### Comparing `optim_esm_tools-0.1.0/optim_esm_tools/synda_files/format_synda.py` & `optim_esm_tools-0.1.1/optim_esm_tools/synda_files/format_synda.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
+# -*- coding: utf-8 -*-
 import typing
 from collections import defaultdict
 import os
 import glob
 import xarray as xr
 from tqdm import tqdm
 import numpy as np
-from xmip.preprocessing import promote_empty_dims, replace_x_y_nominal_lat_lon, rename_cmip6
-from xmip.preprocessing import correct_coordinates, parse_lon_lat_bounds, maybe_convert_bounds_to_vertex, \
-    maybe_convert_vertex_to_bounds, broadcast_lonlat
+
 from abc import ABC
 
 
 #
 # from cdo import Cdo
 # from netCDF4 import Dataset as ds
 # import bottleneck as bn
@@ -20,52 +19,57 @@
 # import pandas as pd
 # import matplotlib.pyplot as plt
 # import cartopy.crs as ccrs
 # from xmip.postprocessing import interpolate_grid_label
 
 
 def load_glob(
-        pattern,
-        **kw,
+    pattern,
+    **kw,
 ) -> xr.Dataset:
     for k, v in dict(
         use_cftime=True,
-        concat_dim="time",
-        combine="nested",
+        concat_dim='time',
+        combine='nested',
         data_vars='minimal',
         coords='minimal',
         compat='override',
         decode_times=True,
     ).items():
         kw.setdefault(k, v)
-    return xr.open_mfdataset(
-        pattern,
-        **kw
-    )
+    return xr.open_mfdataset(pattern, **kw)
 
 
 def _interp_nominal_lon_new(lon_1d):
     print('Using altered version')
     x = np.arange(len(lon_1d))
     idx = np.isnan(lon_1d)
     # TODO assume that longitudes are cyclic (i.e., don't)
     ret = np.interp(x, x[~idx], lon_1d[~idx], period=len(lon_1d))
     return ret
 
 
 def recast(data_set):
+    from xmip.preprocessing import (
+        promote_empty_dims,
+        replace_x_y_nominal_lat_lon,
+        rename_cmip6,
+        broadcast_lonlat,
+    )
+
     ds = data_set.copy()
     # See https://github.com/jbusecke/xMIP/issues/299
     for k, v in {'longitude': 'lon', 'latitude': 'lat'}.items():
         if k in ds:
-            ds.rename(k=v)
+            ds = ds.rename({k: v})
     ds = rename_cmip6(ds)
     ds = promote_empty_dims(ds)
     ds = broadcast_lonlat(ds)
     import xmip.preprocessing
+
     xmip.preprocessing._interp_nominal_lon = _interp_nominal_lon_new
     ds = replace_x_y_nominal_lat_lon(ds)
     return ds
 
 
 class _ResultBase(ABC):
     path: str
@@ -89,14 +93,15 @@
 
 
 class ResultOperations(_ResultBase):
     _warned = False
 
     def get_yearly_means(self, data: xr.Dataset) -> xr.Dataset:
         import warnings
+
         # https://stackoverflow.com/a/71963300
         if not self._warned:
             warnings.warn('Averaging monthly (not accounting for days/month)')
             self._warned = True
         data = data.groupby('time.year').mean('time')
         data = data.rename(year='time')
         return data
@@ -131,48 +136,43 @@
 class ExtractChange(_ResultBase):
     deg_res = 10
     y_bins = np.arange(-90, 90 + 1, deg_res)
     x_bins = np.arange(0, 360 + 1, deg_res)
     registry: typing.Dict[str, typing.Dict[str, xr.Dataset]] = None
 
     def set_slices(self) -> None:
-        pbar = self.tqdm(total=(len(self.x_bins) - 1) * (len(self.y_bins) - 1)
-                         )
+        pbar = self.tqdm(total=(len(self.x_bins) - 1) * (len(self.y_bins) - 1))
 
         if self.registry is None:
             self.registry = defaultdict(dict)
         else:
             raise ValueError('sliced already')
         for x_i, x_l in enumerate(self.x_bins[:-1]):
             x_r = self.x_bins[x_i + 1]
             for y_i, y_l in enumerate(self.y_bins[:-1]):
                 y_r = self.y_bins[y_i + 1]
                 x_label = f'_x_{x_l:03}:{x_r:03}'
                 y_label = f'_y_{y_l:03}:{y_r:03}'
                 pbar.desc = x_label + y_label
                 pbar.display()
                 pbar.n += 1
-                selection = self.data.sel(
-                    y=slice(y_l, y_r),
-                    x=slice(x_l, x_r)
-                )
-                check = [len(
-                    selection[xy].values
-                )
-                    for xy in 'xy']
+                selection = self.data.sel(y=slice(y_l, y_r), x=slice(x_l, x_r))
+                check = [len(selection[xy].values) for xy in 'xy']
                 if not all(check):
                     print(f'No result for {pbar.desc} {check}')
                     continue
                 self.registry[y_label][x_label] = selection.mean(['x', 'y'])
 
                 pbar.display()
         pbar.close()
 
 
 class Result(ResultIO, ResultShower, ResultOperations, ExtractChange):
     pass
 
 
 if __name__ == '__main__':
-    changes = Result('/nobackup/users/angevaar/synda/data/CMIP6/ScenarioMIP'
-                     '/MIROC/MIROC-ES2L/ssp585/r3i1p1f2/Omon/tos/gr1/v20201222/*.nc')
+    changes = Result(
+        '/nobackup/users/angevaar/synda/data/CMIP6/ScenarioMIP'
+        '/MIROC/MIROC-ES2L/ssp585/r3i1p1f2/Omon/tos/gr1/v20201222/*.nc'
+    )
     changes.set_slices()
```

### Comparing `optim_esm_tools-0.1.0/optim_esm_tools/synda_files/synda_files.py` & `optim_esm_tools-0.1.1/optim_esm_tools/synda_files/synda_files.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,23 @@
+# -*- coding: utf-8 -*-
 import os
 import typing
 
-from treelib import Node, Tree
-
 
 class SyndaViewer:
     """Visualize synda downloads as a tree structure"""
 
-    def __init__(self,
-                 base: str = '/nobackup/users/angevaar/synda/data',
-                 max_depth: typing.Optional[int] = None,
-                 show_files: bool = False,
-                 concatenate_folders: bool = True,
-                 count_files: bool = False,
-                 ):
+    def __init__(
+        self,
+        base: str = '/nobackup/users/angevaar/synda/data',
+        max_depth: typing.Optional[int] = None,
+        show_files: bool = False,
+        concatenate_folders: bool = True,
+        count_files: bool = False,
+    ):
         """
         Viewer for Synda Folder structure
 
         :param base: where to start looking
         :param max_depth: maximum recursion depth from the base to show folders
         :param show_files: list files as well as folders
         :param concatenate_folders: concatenate folder names if they contain only one subfolder
@@ -25,33 +25,43 @@
         """
         self.base = base
         self.max_depth = max_depth
         self.show_files = show_files
         self.concatenate_folders = concatenate_folders
         self.count_files = count_files
 
-    def tree(self) -> Tree:
+    def tree(self):
+        from treelib import Tree
+
         base = self.base
         tree = Tree()
         tree.create_node(base, base)
         last_head = base
         for head, directories, files in os.walk(base):
             if self._skip_deep(head):
                 continue
             split = self.chopped_path(head)
             for look_back in range(len(split) - 1):
                 last_head = os.sep.join(split[:-look_back])
                 if last_head in tree.nodes.keys():
                     break
             if last_head in ['', '/']:
-                print(head, directories, files, last_head, look_back, split[:-look_back], tree.nodes.keys())
+                print(
+                    head,
+                    directories,
+                    files,
+                    last_head,
+                    look_back,
+                    split[:-look_back],
+                    tree.nodes.keys(),
+                )
                 last_head = base
 
             if self._add_head(directories):
-                label = os.path.join(*(split[len(self.chopped_path(last_head)):]))
+                label = os.path.join(*(split[len(self.chopped_path(last_head)) :]))
                 if head not in tree.nodes.keys():
                     if self.count_files and files:
                         label += f' ({len(files)})'
                     tree.create_node(label, head, parent=last_head)
 
             if self.show_files and len(files):
                 for file in files:
@@ -61,15 +71,18 @@
     def _add_head(self, directories) -> bool:
         if not self.concatenate_folders:
             return True
         # Only skip if there is exactly ONE subfolder (then we concat)
         return len(directories) != 1
 
     def _skip_deep(self, head) -> bool:
-        return self.max_depth and self.count_depth(head) - self.count_depth(self.base) > self.max_depth
+        return (
+            self.max_depth
+            and self.count_depth(head) - self.count_depth(self.base) > self.max_depth
+        )
 
     @staticmethod
     def chopped_path(path) -> list:
         path = os.path.normpath(path)
         return path.split(os.sep)
 
     def count_depth(self, path) -> int:
```

### Comparing `optim_esm_tools-0.1.0/optim_esm_tools/utils.py` & `optim_esm_tools-0.1.1/optim_esm_tools/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,131 +1,159 @@
+# -*- coding: utf-8 -*-
 import os
 import socket
 import sys
 import typing as ty
 from collections import defaultdict
 from importlib import import_module
 from platform import python_version
 
-import matplotlib
-import matplotlib.pyplot as plt
+import warnings
+
 import numpy as np
 import pandas as pd
-from git import Repo, InvalidGitRepositoryError
-from cycler import cycler
-import json
-from base64 import b32encode
-from hashlib import sha1
-from collections.abc import Mapping
+
+try:
+    from git import Repo, InvalidGitRepositoryError
+
+    GIT_INSTALLED = True
+except (ImportError, ModuleNotFoundError):
+    GIT_INSTALLED = False
+
 import sys
 
 
 # From https://github.com/AxFoundation/strax/blob/136a16975b18ee87500051fd81a90c894d9b58dc/strax/utils.py#L33
 if any('jupyter' in arg for arg in sys.argv):
     # In some cases we are not using any notebooks,
     # Taken from 44952863 on stack overflow thanks!
     from tqdm.notebook import tqdm
 else:
     from tqdm import tqdm
 
 
 # https://github.com/JoranAngevaare/thesis_plots/blob/d828c08e6f6c9c6926527220a23fd0e61e5d8c60/thesis_plots/main.py
-
 root_folder = os.path.join(os.path.split(os.path.realpath(__file__))[0], '..')
 
 
-def setup_plt(use_tex=True):
+def get_plt_colors():
+    """Get matplotlib colors"""
+    import matplotlib.pyplot as plt
+    import matplotlib
+
+    my_colors = [matplotlib.colors.to_hex(c) for c in plt.cm.Set1.colors]
+    # I don't like the yellowish color
+    del my_colors[5]
+    return my_colors
+
+
+def setup_plt(use_tex=True, register_as='custom_map'):
     """Change the plots to have uniform style defaults"""
-    params = {'axes.grid': False,
-              'font.size': 20,
-              'axes.titlesize': 22,
-              'axes.labelsize': 20,
-              'axes.linewidth': 2,
-              'xtick.labelsize': 20,
-              'ytick.labelsize': 20,
-              'ytick.major.size': 8,
-              'ytick.minor.size': 4,
-              'xtick.major.size': 8,
-              'xtick.minor.size': 4,
-              'xtick.major.width': 2,
-              'xtick.minor.width': 2,
-              'ytick.major.width': 2,
-              'ytick.minor.width': 2,
-              'xtick.direction': 'in',
-              'ytick.direction': 'in',
-              'legend.fontsize': 20,
-              'figure.facecolor': 'w',
-              'figure.figsize': (10, 8),
-              'image.cmap': 'viridis',
-              'lines.linewidth': 2,
-              }
+
+    import matplotlib.pyplot as plt
+    import matplotlib
+    from cycler import cycler
+
+    params = {
+        'axes.grid': False,
+        'font.size': 20,
+        'axes.titlesize': 22,
+        'axes.labelsize': 20,
+        'axes.linewidth': 2,
+        'xtick.labelsize': 20,
+        'ytick.labelsize': 20,
+        'ytick.major.size': 8,
+        'ytick.minor.size': 4,
+        'xtick.major.size': 8,
+        'xtick.minor.size': 4,
+        'xtick.major.width': 2,
+        'xtick.minor.width': 2,
+        'ytick.major.width': 2,
+        'ytick.minor.width': 2,
+        'xtick.direction': 'in',
+        'ytick.direction': 'in',
+        'legend.fontsize': 20,
+        'figure.facecolor': 'w',
+        'figure.figsize': (8, 6),
+        'image.cmap': 'viridis',
+        'lines.linewidth': 2,
+        'font.family': 'Times New Roman',
+    }
     plt.rcParams.update(params)
-    # from https://github.com/XENONnT/nton/blob/d5d71b2798d74b9632a8846eb2e0f19ab0d1f563/nton/mplconfigs/stylelib/xenonnt.mplstyle
-    custom_cycler = (
-        cycler(
-            color=[f'#{c}' for c in
-                   ['000000', '0052FF', 'FF2A2A', '4AC124', 'ffa500', '00CFFF', 'FF6AFF', 'A54040']]
-        ) +
-        cycler(marker=['o', 's', 'v', '^', 'D', 'P', '>', 'x']))
+
+    custom_cycler = cycler(color=get_plt_colors())
+    # Could add cycler(marker=['o', 's', 'v', '^', 'D', 'P', '>', 'x'])
 
     plt.rcParams.update({'axes.prop_cycle': custom_cycler})
     if use_tex and not os.environ.get('DISABLE_LATEX', False):
-        # Allow latex to be disabled from the environment coverage see #30
+        # Allow latex to be disabled from the environment coverage see
         matplotlib.rc('text', usetex=True)
 
     from matplotlib.colors import ListedColormap
     import matplotlib as mpl
 
     # Create capped custom map for printing (yellow does not print well)
-    register_as = 'custom_map'
-    custom = ListedColormap(
-        mpl.colormaps['viridis'](np.linspace(0, 0.85, 1000)))
+    custom = ListedColormap(mpl.colormaps['viridis'](np.linspace(0, 0.85, 1000)))
     mpl.colormaps.register(custom, name=register_as, force=True)
     setattr(mpl.pyplot.cm, register_as, custom)
 
     register_as += '_r'
-    custom = ListedColormap(
-        mpl.colormaps['viridis_r'](np.linspace(0.15, 1, 1000)))
+    custom = ListedColormap(mpl.colormaps['viridis_r'](np.linspace(0.15, 1, 1000)))
     mpl.colormaps.register(custom, name=register_as, force=True)
     setattr(mpl.pyplot.cm, register_as, custom)
 
 
-def save_fig(name,
-             file_types=('png', 'pdf'),
-             save_in=root_folder,
-             **kwargs):
+def save_fig(
+    name,
+    file_types=('png', 'pdf'),
+    save_in=root_folder,
+    sub_dir='figures',
+    skip=False,
+    **kwargs,
+):
     """Save a figure in the figures dir"""
+    import matplotlib.pyplot as plt
+
     kwargs.setdefault('dpi', 150)
-    kwargs.setdefault('bbox_inches', "tight")
+    kwargs.setdefault('bbox_inches', 'tight')
+
+    if sub_dir is None:
+        sub_dir = ''
     for file_type in file_types:
-        path = os.path.join(save_in, 'figures', f'{name}.{file_type}')
-        if not os.path.exists(p := os.path.join(save_in, 'figures')):
+        path = os.path.join(save_in, sub_dir, f'{name}.{file_type}')
+        if not os.path.exists(p := os.path.join(save_in, sub_dir)):
             os.makedirs(p, exist_ok=True)
+        if skip:
+            print(f'Skip save {path}')
+            return
         plt.savefig(path, **kwargs)
 
 
 def print_versions(
-        modules=('optim_esm_tools',),
-        print_output=True,
-        include_python=True,
-        return_string=False,
-        include_git=True
+    modules=('optim_esm_tools',),
+    print_output=True,
+    include_python=True,
+    return_string=False,
+    include_git=True,
 ):
     """
     Print versions of modules installed.
 
     :param modules: Modules to print, should be str, tuple or list. E.g.
         print_versions(modules=('numpy', 'optim_esm_tools',))
     :param return_string: optional. Instead of printing the message,
         return a string
     :param include_git: Include the current branch and latest
         commit hash
     :return: optional, the message that would have been printed
     """
     versions = defaultdict(list)
+    if not GIT_INSTALLED and include_git:
+        warnings.warn('Git is not installed, maybe try pip install gitpython')
+        include_git = False
     if include_python:
         versions['module'] = ['python']
         versions['version'] = [python_version()]
         versions['path'] = [sys.executable]
         versions['git'] = [None]
     for m in to_str_tuple(modules):
         result = _version_info_for_module(m, include_git=include_git)
@@ -167,37 +195,44 @@
                 commit_hash = repo.head.object.hexsha
             except TypeError:
                 commit_hash = 'unknown'
             git = f'branch:{branch} | {commit_hash[:7]}'
     return version, module_path, git
 
 
-def to_str_tuple(x: ty.Union[str, bytes, list, tuple, pd.Series, np.ndarray]) -> ty.Tuple[str]:
+def to_str_tuple(
+    x: ty.Union[str, bytes, list, tuple, pd.Series, np.ndarray]
+) -> ty.Tuple[str]:
     """
     Convert any sensible instance to a tuple of strings
     from https://github.com/AxFoundation/strax/blob/d3608efc77acd52e1d5a208c3092b6b45b27a6e2/strax/utils.py#242
     """
     if isinstance(x, (str, bytes)):
-        return x,
+        return (x,)
     if isinstance(x, list):
         return tuple(x)
     if isinstance(x, tuple):
         return x
-    raise TypeError(f"Expected string or tuple of strings, got {type(x)}")
+    raise TypeError(f'Expected string or tuple of strings, got {type(x)}')
+
+
+def mathrm(string):
+    return string_to_mathrm(string)
 
 
 def string_to_mathrm(string):
     """wrap a string in mathrm mode for latex labels"""
     string = string.replace(' ', '\ ')
     return f'$\mathrm{{{string}}}$'
 
 
 def legend_kw(**kw):
     options = dict(
-        bbox_to_anchor=(0., 1.02, 1, .32),
+        bbox_to_anchor=(0.0, 1.02, 1, 0.32),
         loc=3,
         ncol=3,
-        mode="expand",
-        borderaxespad=0.,
-        frameon=True)
+        mode='expand',
+        borderaxespad=0.0,
+        frameon=True,
+    )
     options.update(kw)
     return options
```

### Comparing `optim_esm_tools-0.1.0/optim_esm_tools.egg-info/PKG-INFO` & `optim_esm_tools-0.1.1/optim_esm_tools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optim-esm-tools
-Version: 0.1.0
+Version: 0.1.1
 Summary: Tools for OptimESM
 Home-page: https://github.com/JoranAngevaare/optim_esm_tools
 Author: Joran R. Angevaare
 License: UNKNOWN
 Description: # OptimESM
         [![Coverage Status](https://coveralls.io/repos/github/JoranAngevaare/optim_esm_tools/badge.svg)](https://coveralls.io/github/JoranAngevaare/optim_esm_tools)
         
@@ -29,14 +29,15 @@
         * Upgrade CI/CD by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/19
         * Flexible loading by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/16
         * Initialize testing by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/20
         * Add test for synda viewer by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/28
         * fix lat lon handling by @JoranAngevaare in https://github.com/JoranAngevaare/optim_esm_tools/pull/29
         
         **Full Changelog**: https://github.com/JoranAngevaare/optim_esm_tools/commits/v0.1.0
+        
 Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `optim_esm_tools-0.1.0/optim_esm_tools.egg-info/SOURCES.txt` & `optim_esm_tools-0.1.1/optim_esm_tools.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 README.md
+pyproject.toml
 setup.cfg
 setup.py
 extra_requirements/requirements-tests.txt
 optim_esm_tools/__init__.py
+optim_esm_tools/_test_utils.py
 optim_esm_tools/utils.py
 optim_esm_tools.egg-info/PKG-INFO
 optim_esm_tools.egg-info/SOURCES.txt
 optim_esm_tools.egg-info/dependency_links.txt
 optim_esm_tools.egg-info/not-zip-safe
 optim_esm_tools.egg-info/requires.txt
 optim_esm_tools.egg-info/top_level.txt
 optim_esm_tools/analyze/__init__.py
 optim_esm_tools/analyze/analyze.py
+optim_esm_tools/analyze/clustering.py
 optim_esm_tools/analyze/cmip_handler.py
 optim_esm_tools/analyze/xarray_tools.py
 optim_esm_tools/synda_files/__init__.py
 optim_esm_tools/synda_files/format_synda.py
 optim_esm_tools/synda_files/synda_files.py
 test/test_basics.py
+test/test_clustering.py
 test/test_utils.py
 test/test_viewer.py
 test/test_workflow.py
 test/test_xarray_tools.py
```

### Comparing `optim_esm_tools-0.1.0/setup.py` & `optim_esm_tools-0.1.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,50 +1,54 @@
+# -*- coding: utf-8 -*-
 import setuptools
 
 
 def open_requirements(path):
     with open(path) as f:
         requires = [
             r.split('/')[-1] if r.startswith('git+') else r
-            for r in f.read().splitlines()]
+            for r in f.read().splitlines()
+        ]
     return requires
 
 
 readme = open('README.md').read()
 history = open('HISTORY.md').read()
 requirements = open_requirements('requirements.txt')
 
 setuptools.setup(
     name='optim_esm_tools',
-    version='0.1.0',
+    version='0.1.1',
     description='Tools for OptimESM',
     long_description=readme + '\n\n' + history,
     long_description_content_type='text/markdown',
     author='Joran R. Angevaare',
     url='https://github.com/JoranAngevaare/optim_esm_tools',
     packages=setuptools.find_packages() + ['extra_requirements'],
-    package_dir={'optim_esm_tools': 'optim_esm_tools',
-                 'extra_requirements': 'extra_requirements'},
-    package_data={'optim_esm_tools': ['data/*'],
-                  'extra_requirements': ['requirements-tests.txt'],
-                  },
+    package_dir={
+        'optim_esm_tools': 'optim_esm_tools',
+        'extra_requirements': 'extra_requirements',
+    },
+    package_data={
+        'optim_esm_tools': ['data/*'],
+        'extra_requirements': ['requirements-tests.txt'],
+    },
     setup_requires=['pytest-runner'],
     install_requires=requirements,
-    python_requires=">=3.8",
-    tests_require=requirements + ['pytest',
-                                  'hypothesis-numpy',
-                                  'unittest',
-                                  'coverage'],
+    python_requires='>=3.8',
+    tests_require=requirements + open_requirements('requirements_tests.txt'),
     scripts=[],
     keywords=[],
-    classifiers=['Intended Audience :: Science/Research',
-                 'Development Status :: 2 - Pre-Alpha',
-                 'Programming Language :: Python :: 3.8',
-                 'Natural Language :: English',
-                 'Programming Language :: Python :: 3.8',
-                 'Programming Language :: Python :: 3.9',
-                 'Programming Language :: Python :: 3.10',
-                 'Intended Audience :: Science/Research',
-                 'Programming Language :: Python :: Implementation :: CPython',
-                 'Topic :: Scientific/Engineering :: Physics',
-                 ],
-    zip_safe=False)
+    classifiers=[
+        'Intended Audience :: Science/Research',
+        'Development Status :: 2 - Pre-Alpha',
+        'Programming Language :: Python :: 3.8',
+        'Natural Language :: English',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Intended Audience :: Science/Research',
+        'Programming Language :: Python :: Implementation :: CPython',
+        'Topic :: Scientific/Engineering :: Physics',
+    ],
+    zip_safe=False,
+)
```

### Comparing `optim_esm_tools-0.1.0/test/test_workflow.py` & `optim_esm_tools-0.1.1/test/test_workflow.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,55 +1,59 @@
+# -*- coding: utf-8 -*-
 import unittest
 import optim_esm_tools as oet
 import os
-import glob
 import matplotlib.pyplot as plt
 import subprocess
+from optim_esm_tools._test_utils import synda_test_available, get_example_data_loc
 
+
+@unittest.skipIf(not synda_test_available(), 'synda data not available')
 class TestMapMaker(unittest.TestCase):
-    example_data_set = 'CMIP6/ScenarioMIP/CCCma/CanESM5/ssp585/r3i1p2f1/Amon/tas/gn/v20190429/tas_Amon_CanESM5_ssp585_r3i1p2f1_gn_201501-210012.nc'
+    # example_data_set = oet._test_utils.EXAMPLE_DATA_SET
 
     def from_amon_to_ayear(self):
-
         if os.path.exists(self.ayear_file):
             return
 
         os.makedirs(os.path.split(self.ayear_file)[0], exist_ok=1)
         # Doesn't work?
         # cdo.Cdo().yearmonmean(self.amon_file, self.ayear_file)
         cmd = f'cdo yearmonmean {self.amon_file} {self.ayear_file}'
         print(cmd)
-        subprocess.call(cmd, shell=True)  
+        subprocess.call(cmd, shell=True)
         assert os.path.exists(self.ayear_file), self.ayear_file
 
     @classmethod
     def setUpClass(cls):
         cls.base = os.path.join(os.environ['ST_HOME'], 'data')
-        cls.amon_file = os.path.join(cls.base, cls.example_data_set)
-        cls.ayear_file = os.path.join(os.path.split(cls.amon_file.replace('Amon', 'AYear'))[0], 'merged.nc')
-        
+        cls.amon_file = get_example_data_loc()
+        cls.ayear_file = os.path.join(
+            os.path.split(cls.amon_file.replace('Amon', 'AYear'))[0], 'merged.nc'
+        )
+
     def setUp(self):
         self.from_amon_to_ayear()
         super().setUp()
 
     def test_read_data(self):
         data_set = oet.synda_files.format_synda.load_glob(self.ayear_file)
-    
+
     def test_make_map(self):
         data_set = oet.analyze.cmip_handler.read_ds(os.path.split(self.ayear_file)[0])
         oet.analyze.cmip_handler.MapMaker(data_set=data_set).plot_all(2)
         plt.clf()
 
     def test_example_time_series(self):
         data_set = oet.analyze.cmip_handler.read_ds(os.path.split(self.ayear_file)[0])
         oet.analyze.cmip_handler.example_time_series(data_set)
         plt.clf()
-    
+
     def test_map_maker_time_series(self):
         data_set = oet.analyze.cmip_handler.read_ds(os.path.split(self.ayear_file)[0])
         oet.analyze.cmip_handler.MapMaker(data_set=data_set).time_series()
         plt.clf()
 
     @classmethod
     def tearDownClass(cls) -> None:
         os.remove(cls.ayear_file)
-        return super().tearDownClass()
+        return super().tearDownClass()
```

