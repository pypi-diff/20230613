# Comparing `tmp/filter_stations-0.3.7.tar.gz` & `tmp/filter_stations-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "filter_stations-0.3.7.tar", last modified: Tue Jun 13 06:33:31 2023, max compression
+gzip compressed data, was "filter_stations-0.3.8.tar", last modified: Tue Jun 13 06:51:36 2023, max compression
```

## Comparing `filter_stations-0.3.7.tar` & `filter_stations-0.3.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 06:33:31.444360 filter_stations-0.3.7/
--rw-rw-rw-   0        0        0      361 2023-06-13 06:33:31.443864 filter_stations-0.3.7/PKG-INFO
--rw-rw-rw-   0        0        0       55 2023-05-04 10:44:45.000000 filter_stations-0.3.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-13 06:33:31.407415 filter_stations-0.3.7/filter_stations/
--rw-rw-rw-   0        0        0    47138 2023-06-13 06:33:18.000000 filter_stations-0.3.7/filter_stations/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 06:33:31.440802 filter_stations-0.3.7/filter_stations.egg-info/
--rw-rw-rw-   0        0        0      361 2023-06-13 06:33:31.000000 filter_stations-0.3.7/filter_stations.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      282 2023-06-13 06:33:31.000000 filter_stations-0.3.7/filter_stations.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 06:33:31.000000 filter_stations-0.3.7/filter_stations.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-06-13 06:33:31.000000 filter_stations-0.3.7/filter_stations.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       92 2023-06-13 06:33:31.000000 filter_stations-0.3.7/filter_stations.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-13 06:33:31.000000 filter_stations-0.3.7/filter_stations.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-13 06:33:31.444360 filter_stations-0.3.7/setup.cfg
--rw-rw-rw-   0        0        0      933 2023-06-13 06:33:24.000000 filter_stations-0.3.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 06:51:36.652294 filter_stations-0.3.8/
+-rw-rw-rw-   0        0        0      361 2023-06-13 06:51:36.651285 filter_stations-0.3.8/PKG-INFO
+-rw-rw-rw-   0        0        0       55 2023-05-04 10:44:45.000000 filter_stations-0.3.8/README.md
+drwxrwxrwx   0        0        0        0 2023-06-13 06:51:36.616643 filter_stations-0.3.8/filter_stations/
+-rw-rw-rw-   0        0        0    47221 2023-06-13 06:51:22.000000 filter_stations-0.3.8/filter_stations/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 06:51:36.649653 filter_stations-0.3.8/filter_stations.egg-info/
+-rw-rw-rw-   0        0        0      361 2023-06-13 06:51:36.000000 filter_stations-0.3.8/filter_stations.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2023-06-13 06:51:36.000000 filter_stations-0.3.8/filter_stations.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 06:51:36.000000 filter_stations-0.3.8/filter_stations.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-06-13 06:51:36.000000 filter_stations-0.3.8/filter_stations.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       92 2023-06-13 06:51:36.000000 filter_stations-0.3.8/filter_stations.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-13 06:51:36.000000 filter_stations-0.3.8/filter_stations.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-13 06:51:36.652294 filter_stations-0.3.8/setup.cfg
+-rw-rw-rw-   0        0        0      933 2023-06-13 06:51:29.000000 filter_stations-0.3.8/setup.py
```

### Comparing `filter_stations-0.3.7/filter_stations/__init__.py` & `filter_stations-0.3.8/filter_stations/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import datetime
 import gc
 from math import ceil
 
 
 # Constants
 API_BASE_URL = 'https://datahub.tahmo.org'
-API_MAX_PERIOD = '1Y'
+API_MAX_PERIOD = 'Y'
 
 endpoints = {'VARIABLES': 'services/assets/v2/variables', # 28 different variables
              'STATION_INFO': 'services/assets/v2/stations',
              'WEATHER_DATA': 'services/measurements/v2/stations', # Configured before requesting
              'DATA_COMPLETE': 'custom/sensordx/latestmeasurements',
              'STATION_STATUS': 'custom/stations/status'}
 
@@ -203,25 +203,25 @@
         -----------
         - dataframe (pandas.DataFrame): DataFrame containing weather variable data.
 
         Returns:
         -----------
         - pandas.DataFrame: DataFrame containing aggregated weather variable data, summed by day.
         """
-        # check if the column is all nan
-        
-        # Reset index and rename columns
         dataframe = dataframe.reset_index()
         dataframe.rename(columns={'index':'Date'}, inplace=True)
-        print(dataframe.columns[0])
-        # Group by date and sum values
-        return dataframe.groupby(pd.Grouper(key='Date', axis=0, 
+        # check if the column is all nan
+        if dataframe.iloc[:, 1].isnull().all():
+                return dataframe.groupby(pd.Grouper(key='Date', axis=0, 
                                             freq='1D')).agg({f'{dataframe.columns[1]}': 
                                                              lambda x: np.nan if x.isnull().all() 
-                                                             else x.isnull().sum()})
+                                                             else x.isnull().sum()})    
+        else:
+                return dataframe.groupby(pd.Grouper(key='Date', axis=0, 
+                                            freq='1D')).sum()
     
     # aggregate qualityflags
     def aggregate_qualityflags(self, dataframe):
         """
         Aggregate quality flags in a DataFrame by day.
 
         Parameters:
```

### Comparing `filter_stations-0.3.7/setup.py` & `filter_stations-0.3.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='filter_stations',
-    version='0.3.7',
+    version='0.3.8',
     packages=find_packages(),
     include_package_data=True,
     description='Making it easier to navigate and clean station data',
     author='Austin Kaburia',
     author_email='kaburiaaustin1@gmail.com',
     url='https://github.com/kaburia/Packaging/tree/main/filter_stations',
     install_requires=[
```

