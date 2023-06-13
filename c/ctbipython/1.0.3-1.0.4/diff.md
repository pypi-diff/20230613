# Comparing `tmp/ctbipython-1.0.3.tar.gz` & `tmp/ctbipython-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctbipython-1.0.3.tar", last modified: Tue Jun 13 16:45:52 2023, max compression
+gzip compressed data, was "ctbipython-1.0.4.tar", last modified: Tue Jun 13 19:29:13 2023, max compression
```

## Comparing `ctbipython-1.0.3.tar` & `ctbipython-1.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 16:45:52.060259 ctbipython-1.0.3/
--rw-rw-rw-   0        0        0      197 2023-06-13 16:45:52.060259 ctbipython-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1355 2023-05-24 14:03:51.000000 ctbipython-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-13 16:45:52.043307 ctbipython-1.0.3/ctbipython/
--rw-rw-rw-   0        0        0        0 2023-05-24 12:22:47.000000 ctbipython-1.0.3/ctbipython/__init__.py
--rw-rw-rw-   0        0        0    78961 2023-06-13 16:45:41.000000 ctbipython-1.0.3/ctbipython/ctbi.py
--rw-rw-rw-   0        0        0     3950 2023-06-13 13:13:47.000000 ctbipython-1.0.3/ctbipython/example.py
-drwxrwxrwx   0        0        0        0 2023-06-13 16:45:52.058269 ctbipython-1.0.3/ctbipython.egg-info/
--rw-rw-rw-   0        0        0      197 2023-06-13 16:45:51.000000 ctbipython-1.0.3/ctbipython.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      251 2023-06-13 16:45:51.000000 ctbipython-1.0.3/ctbipython.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 16:45:51.000000 ctbipython-1.0.3/ctbipython.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-06-13 16:45:51.000000 ctbipython-1.0.3/ctbipython.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-13 16:45:51.000000 ctbipython-1.0.3/ctbipython.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-13 16:45:52.061259 ctbipython-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      348 2023-06-13 16:45:45.000000 ctbipython-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 19:29:13.685350 ctbipython-1.0.4/
+-rw-rw-rw-   0        0        0      197 2023-06-13 19:29:13.685350 ctbipython-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1355 2023-05-24 14:03:51.000000 ctbipython-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-13 19:29:13.657957 ctbipython-1.0.4/ctbipython/
+-rw-rw-rw-   0        0        0        0 2023-05-24 12:22:47.000000 ctbipython-1.0.4/ctbipython/__init__.py
+-rw-rw-rw-   0        0        0    79058 2023-06-13 17:07:27.000000 ctbipython-1.0.4/ctbipython/ctbi.py
+-rw-rw-rw-   0        0        0     3950 2023-06-13 13:13:47.000000 ctbipython-1.0.4/ctbipython/example.py
+drwxrwxrwx   0        0        0        0 2023-06-13 19:29:13.684351 ctbipython-1.0.4/ctbipython.egg-info/
+-rw-rw-rw-   0        0        0      197 2023-06-13 19:29:13.000000 ctbipython-1.0.4/ctbipython.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2023-06-13 19:29:13.000000 ctbipython-1.0.4/ctbipython.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 19:29:13.000000 ctbipython-1.0.4/ctbipython.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-06-13 19:29:13.000000 ctbipython-1.0.4/ctbipython.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-13 19:29:13.000000 ctbipython-1.0.4/ctbipython.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-13 19:29:13.685350 ctbipython-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      348 2023-06-13 17:05:49.000000 ctbipython-1.0.4/setup.py
```

### Comparing `ctbipython-1.0.3/README.md` & `ctbipython-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `ctbipython-1.0.3/ctbipython/ctbi.py` & `ctbipython-1.0.4/ctbipython/ctbi.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import pandas as pd
 import numpy as np
 import re
 from datetime import datetime, timedelta
 from scipy.interpolate import interp1d
 import seaborn as sns
 import matplotlib.pyplot as plt
+import datatable as dt
 
 warnings.filterwarnings("ignore")
 
 def main(data_input,bin_side,bin_period,bin_center=None,bin_FUN='mean',bin_max_f_NA=0.2,SCI_min=0.6,coeff_outlier='auto',ylim=(float('-inf'),float('inf'))):
     """
     The goal of ctbi is to clean, decompose, impute and aggregate univariate time series. ctbi stands for Cyclic/Trend decomposition using Bin Interpolation: the time series is divided into a sequence of non-overlapping bins (inputs: bin_side or bin_center, and bin_period). Bins with enough data (input: bin_max_f_NA) are accepted, and otherwise rejected (their values are set to NA). The long-term trend is a linear interpolation of the mean values between successive bins. The cyclic component is the mean stack of detrended data within all accepted bins.
 
@@ -165,16 +166,20 @@
 
     # Calculate the minimum number of points for a bin to be accepted, n_bin_min
     n_bin_min = int(np.ceil(bin_size * (1 - bin_max_f_NA)))
     if n_bin_min < 1:
         n_bin_min = 1
 
     # Add columns to data1: bin_center, bin_start, bin_end and the number of NA values per bin
-    data1 = pd.merge(data1, data0.groupby('index_bin')['y'].apply(lambda x: np.sum(pd.isna(x))), on='index_bin', how='outer')
-    data1 = data1.rename(columns={'y': 'n_NA'})
+    df = data0
+    df['y_NA'] = df['y'].isna()
+    df = dt.Frame(df)
+
+    data1 = pd.merge(data1, df[:, dt.f['y_NA'].sum(), dt.by(dt.f['index_bin'])].to_pandas(), on='index_bin', how='outer')
+    data1 = data1.rename(columns={'y_NA': 'n_NA'})
     data1.loc[data1['n_NA'].isna(), 'n_NA'] = 0
     data1['bin_center'] = seq_bin_center
     data1['bin_start'] = seq_bin_side[:len(seq_bin_side)-1]
     data1['bin_end'] = seq_bin_side[1:]
 
     # Calculate the relative position of the values with respect to their bin.
     data0['time_bin'] = data0.apply(lambda row: hidd_rel_time(data0.loc[(data0['index_bin'] == row['index_bin']) & (data0['x'] >= row['x']), 'x'].reset_index(drop=True), seq_bin_side), axis=1)
```

### Comparing `ctbipython-1.0.3/ctbipython/example.py` & `ctbipython-1.0.4/ctbipython/example.py`

 * *Files identical despite different names*

