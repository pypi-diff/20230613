# Comparing `tmp/filter_stations-0.3.4.tar.gz` & `tmp/filter_stations-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "filter_stations-0.3.4.tar", last modified: Sun Jun 11 16:28:34 2023, max compression
+gzip compressed data, was "filter_stations-0.3.5.tar", last modified: Tue Jun 13 05:59:05 2023, max compression
```

## Comparing `filter_stations-0.3.4.tar` & `filter_stations-0.3.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 16:28:34.312691 filter_stations-0.3.4/
--rw-rw-rw-   0        0        0      361 2023-06-11 16:28:34.312265 filter_stations-0.3.4/PKG-INFO
--rw-rw-rw-   0        0        0       55 2023-05-04 10:44:45.000000 filter_stations-0.3.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-11 16:28:34.265847 filter_stations-0.3.4/filter_stations/
--rw-rw-rw-   0        0        0    46699 2023-06-11 16:25:59.000000 filter_stations-0.3.4/filter_stations/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-11 16:28:34.309377 filter_stations-0.3.4/filter_stations.egg-info/
--rw-rw-rw-   0        0        0      361 2023-06-11 16:28:33.000000 filter_stations-0.3.4/filter_stations.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      282 2023-06-11 16:28:33.000000 filter_stations-0.3.4/filter_stations.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 16:28:33.000000 filter_stations-0.3.4/filter_stations.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-06-11 16:28:33.000000 filter_stations-0.3.4/filter_stations.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       92 2023-06-11 16:28:33.000000 filter_stations-0.3.4/filter_stations.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-11 16:28:33.000000 filter_stations-0.3.4/filter_stations.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-11 16:28:34.313190 filter_stations-0.3.4/setup.cfg
--rw-rw-rw-   0        0        0      933 2023-06-11 15:52:04.000000 filter_stations-0.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 05:59:05.177782 filter_stations-0.3.5/
+-rw-rw-rw-   0        0        0      361 2023-06-13 05:59:05.175248 filter_stations-0.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0       55 2023-05-04 10:44:45.000000 filter_stations-0.3.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-13 05:59:05.098594 filter_stations-0.3.5/filter_stations/
+-rw-rw-rw-   0        0        0    46790 2023-06-13 05:58:06.000000 filter_stations-0.3.5/filter_stations/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 05:59:05.167843 filter_stations-0.3.5/filter_stations.egg-info/
+-rw-rw-rw-   0        0        0      361 2023-06-13 05:59:02.000000 filter_stations-0.3.5/filter_stations.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2023-06-13 05:59:03.000000 filter_stations-0.3.5/filter_stations.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 05:59:02.000000 filter_stations-0.3.5/filter_stations.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-06-13 05:59:02.000000 filter_stations-0.3.5/filter_stations.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       92 2023-06-13 05:59:02.000000 filter_stations-0.3.5/filter_stations.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-13 05:59:02.000000 filter_stations-0.3.5/filter_stations.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-13 05:59:05.178128 filter_stations-0.3.5/setup.cfg
+-rw-rw-rw-   0        0        0      933 2023-06-13 05:58:13.000000 filter_stations-0.3.5/setup.py
```

### Comparing `filter_stations-0.3.4/filter_stations/__init__.py` & `filter_stations-0.3.5/filter_stations/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -377,19 +377,19 @@
                 df = pd.concat(series, axis=1, sort=True)
             else:
                 df = pd.DataFrame()
 
             # Clean up memory.
             del series
             gc.collect()
+            # check if dataframe is empty
+            if df.empty:
+                # add the date range in the dataframe and the column as the station filled with NaN
+                df = pd.DataFrame(index=pd.date_range(start=startDate, end=endDate, freq='5min'), columns=[f'{station}'])
             if quality_flags:
-                # cols = [col for col in df.columns if col.split('_')[-1] == 'Q_FLAG']
-                # print(cols)
-                # df = df[cols]
-                # df = df[[f'{station}_Q_Flag']]
                 if aggregate:
                     return self.aggregate_qualityflags(df)
                 else:
                     return df
             else:
                 if aggregate:
                     return self.aggregate_variables(df)
```

### Comparing `filter_stations-0.3.4/setup.py` & `filter_stations-0.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='filter_stations',
-    version='0.3.4',
+    version='0.3.5',
     packages=find_packages(),
     include_package_data=True,
     description='Making it easier to navigate and clean station data',
     author='Austin Kaburia',
     author_email='kaburiaaustin1@gmail.com',
     url='https://github.com/kaburia/Packaging/tree/main/filter_stations',
     install_requires=[
```

