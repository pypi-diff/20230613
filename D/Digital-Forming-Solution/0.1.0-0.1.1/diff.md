# Comparing `tmp/Digital_Forming_Solution-0.1.0.tar.gz` & `tmp/Digital_Forming_Solution-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Digital_Forming_Solution-0.1.0.tar", last modified: Tue Jun 13 09:51:37 2023, max compression
+gzip compressed data, was "Digital_Forming_Solution-0.1.1.tar", last modified: Tue Jun 13 15:04:44 2023, max compression
```

## Comparing `Digital_Forming_Solution-0.1.0.tar` & `Digital_Forming_Solution-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 09:51:37.069816 Digital_Forming_Solution-0.1.0/
-drwxrwxrwx   0        0        0        0 2023-06-13 09:51:36.953122 Digital_Forming_Solution-0.1.0/Digital_Forming_Solution/
--rw-rw-rw-   0        0        0      821 2023-06-13 09:45:13.000000 Digital_Forming_Solution-0.1.0/Digital_Forming_Solution/Select_Operations.py
--rw-rw-rw-   0        0        0        0 2023-06-13 09:25:58.000000 Digital_Forming_Solution-0.1.0/Digital_Forming_Solution/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 09:51:37.059845 Digital_Forming_Solution-0.1.0/Digital_Forming_Solution.egg-info/
--rw-rw-rw-   0        0        0      427 2023-06-13 09:51:35.000000 Digital_Forming_Solution-0.1.0/Digital_Forming_Solution.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2023-06-13 09:51:36.000000 Digital_Forming_Solution-0.1.0/Digital_Forming_Solution.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 09:51:35.000000 Digital_Forming_Solution-0.1.0/Digital_Forming_Solution.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-06-13 09:51:35.000000 Digital_Forming_Solution-0.1.0/Digital_Forming_Solution.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      427 2023-06-13 09:51:37.067814 Digital_Forming_Solution-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-13 09:51:37.070806 Digital_Forming_Solution-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      666 2023-06-13 09:51:25.000000 Digital_Forming_Solution-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 15:04:44.562517 Digital_Forming_Solution-0.1.1/
+drwxrwxrwx   0        0        0        0 2023-06-13 15:04:44.506567 Digital_Forming_Solution-0.1.1/Digital_Forming_Solution/
+-rw-rw-rw-   0        0        0      923 2023-06-13 15:03:46.000000 Digital_Forming_Solution-0.1.1/Digital_Forming_Solution/Select_Operations.py
+-rw-rw-rw-   0        0        0        0 2023-06-13 09:25:58.000000 Digital_Forming_Solution-0.1.1/Digital_Forming_Solution/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 15:04:44.546420 Digital_Forming_Solution-0.1.1/Digital_Forming_Solution.egg-info/
+-rw-rw-rw-   0        0        0      386 2023-06-13 15:04:43.000000 Digital_Forming_Solution-0.1.1/Digital_Forming_Solution.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2023-06-13 15:04:44.000000 Digital_Forming_Solution-0.1.1/Digital_Forming_Solution.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 15:04:43.000000 Digital_Forming_Solution-0.1.1/Digital_Forming_Solution.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-06-13 15:04:43.000000 Digital_Forming_Solution-0.1.1/Digital_Forming_Solution.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      386 2023-06-13 15:04:44.552381 Digital_Forming_Solution-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-13 15:04:44.563511 Digital_Forming_Solution-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      514 2023-06-13 15:04:02.000000 Digital_Forming_Solution-0.1.1/setup.py
```

### Comparing `Digital_Forming_Solution-0.1.0/Digital_Forming_Solution/Select_Operations.py` & `Digital_Forming_Solution-0.1.1/Digital_Forming_Solution/Select_Operations.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 import numpy as np
 
 def Yield_Binning(datframe,column):
     
+    # Droping the Null Values
+    datframe = datframe.dropna(column)
+
+    # Copying the Dataframe
     data =  datframe.copy()
     
     # Calculating the yield quantiles
     col_values = list(data[column])
     Q_25 = np.percentile (col_values, 25) 
     Q_50 = np.percentile (col_values, 50)
     Q_75 = np.percentile (col_values, 75)
```

