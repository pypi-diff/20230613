# Comparing `tmp/filter_stations-0.3.6.tar.gz` & `tmp/filter_stations-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "filter_stations-0.3.6.tar", last modified: Tue Jun 13 06:08:10 2023, max compression
+gzip compressed data, was "filter_stations-0.3.7.tar", last modified: Tue Jun 13 06:33:31 2023, max compression
```

## Comparing `filter_stations-0.3.6.tar` & `filter_stations-0.3.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 06:08:10.067926 filter_stations-0.3.6/
--rw-rw-rw-   0        0        0      361 2023-06-13 06:08:10.064156 filter_stations-0.3.6/PKG-INFO
--rw-rw-rw-   0        0        0       55 2023-05-04 10:44:45.000000 filter_stations-0.3.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-13 06:08:09.988313 filter_stations-0.3.6/filter_stations/
--rw-rw-rw-   0        0        0    46800 2023-06-13 06:07:39.000000 filter_stations-0.3.6/filter_stations/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 06:08:10.058550 filter_stations-0.3.6/filter_stations.egg-info/
--rw-rw-rw-   0        0        0      361 2023-06-13 06:08:09.000000 filter_stations-0.3.6/filter_stations.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      282 2023-06-13 06:08:09.000000 filter_stations-0.3.6/filter_stations.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 06:08:09.000000 filter_stations-0.3.6/filter_stations.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-06-13 06:08:09.000000 filter_stations-0.3.6/filter_stations.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       92 2023-06-13 06:08:09.000000 filter_stations-0.3.6/filter_stations.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-13 06:08:09.000000 filter_stations-0.3.6/filter_stations.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-13 06:08:10.068986 filter_stations-0.3.6/setup.cfg
--rw-rw-rw-   0        0        0      933 2023-06-13 06:07:55.000000 filter_stations-0.3.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 06:33:31.444360 filter_stations-0.3.7/
+-rw-rw-rw-   0        0        0      361 2023-06-13 06:33:31.443864 filter_stations-0.3.7/PKG-INFO
+-rw-rw-rw-   0        0        0       55 2023-05-04 10:44:45.000000 filter_stations-0.3.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-13 06:33:31.407415 filter_stations-0.3.7/filter_stations/
+-rw-rw-rw-   0        0        0    47138 2023-06-13 06:33:18.000000 filter_stations-0.3.7/filter_stations/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 06:33:31.440802 filter_stations-0.3.7/filter_stations.egg-info/
+-rw-rw-rw-   0        0        0      361 2023-06-13 06:33:31.000000 filter_stations-0.3.7/filter_stations.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2023-06-13 06:33:31.000000 filter_stations-0.3.7/filter_stations.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 06:33:31.000000 filter_stations-0.3.7/filter_stations.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-06-13 06:33:31.000000 filter_stations-0.3.7/filter_stations.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       92 2023-06-13 06:33:31.000000 filter_stations-0.3.7/filter_stations.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-13 06:33:31.000000 filter_stations-0.3.7/filter_stations.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-13 06:33:31.444360 filter_stations-0.3.7/setup.cfg
+-rw-rw-rw-   0        0        0      933 2023-06-13 06:33:24.000000 filter_stations-0.3.7/setup.py
```

### Comparing `filter_stations-0.3.6/filter_stations/__init__.py` & `filter_stations-0.3.7/filter_stations/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -203,20 +203,25 @@
         -----------
         - dataframe (pandas.DataFrame): DataFrame containing weather variable data.
 
         Returns:
         -----------
         - pandas.DataFrame: DataFrame containing aggregated weather variable data, summed by day.
         """
+        # check if the column is all nan
+        
         # Reset index and rename columns
         dataframe = dataframe.reset_index()
         dataframe.rename(columns={'index':'Date'}, inplace=True)
-        
+        print(dataframe.columns[0])
         # Group by date and sum values
-        return dataframe.groupby(pd.Grouper(key='Date', axis=0, freq='1D')).sum()
+        return dataframe.groupby(pd.Grouper(key='Date', axis=0, 
+                                            freq='1D')).agg({f'{dataframe.columns[1]}': 
+                                                             lambda x: np.nan if x.isnull().all() 
+                                                             else x.isnull().sum()})
     
     # aggregate qualityflags
     def aggregate_qualityflags(self, dataframe):
         """
         Aggregate quality flags in a DataFrame by day.
 
         Parameters:
```

### Comparing `filter_stations-0.3.6/setup.py` & `filter_stations-0.3.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='filter_stations',
-    version='0.3.6',
+    version='0.3.7',
     packages=find_packages(),
     include_package_data=True,
     description='Making it easier to navigate and clean station data',
     author='Austin Kaburia',
     author_email='kaburiaaustin1@gmail.com',
     url='https://github.com/kaburia/Packaging/tree/main/filter_stations',
     install_requires=[
```

