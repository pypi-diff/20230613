# Comparing `tmp/proptables-0.0.6.tar.gz` & `tmp/proptables-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proptables-0.0.6.tar", last modified: Tue Jun 13 18:42:56 2023, max compression
+gzip compressed data, was "proptables-0.0.7.tar", last modified: Tue Jun 13 19:26:21 2023, max compression
```

## Comparing `proptables-0.0.6.tar` & `proptables-0.0.7.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 18:42:56.011305 proptables-0.0.6/
--rw-rw-rw-   0        0        0     1070 2023-06-03 19:14:15.000000 proptables-0.0.6/LICENCE.txt
--rw-rw-rw-   0        0        0       62 2023-06-11 10:30:34.000000 proptables-0.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0     2452 2023-06-13 18:42:56.011305 proptables-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1953 2023-06-07 09:25:23.000000 proptables-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-13 18:42:55.612055 proptables-0.0.6/proptables/
-drwxrwxrwx   0        0        0        0 2023-06-13 18:42:55.902417 proptables-0.0.6/proptables/R134a/
--rw-rw-rw-   0        0        0     2379 2023-06-11 10:30:34.000000 proptables-0.0.6/proptables/R134a/R134a_PresSat.csv
--rw-rw-rw-   0        0        0      239 2023-06-11 10:30:34.000000 proptables-0.0.6/proptables/R134a/R134a_SupPreSat.csv
--rw-rw-rw-   0        0        0     9904 2023-06-11 10:30:34.000000 proptables-0.0.6/proptables/R134a/R134a_Super.csv
--rw-rw-rw-   0        0        0     3782 2023-06-11 10:30:34.000000 proptables-0.0.6/proptables/R134a/R134a_TempSat.csv
--rw-rw-rw-   0        0        0       39 2023-06-11 10:30:34.000000 proptables-0.0.6/proptables/R134a/__init__.py
--rw-rw-rw-   0        0        0     4503 2023-06-11 10:30:34.000000 proptables-0.0.6/proptables/R134a/calSatData.py
--rw-rw-rw-   0        0        0     4210 2023-06-12 08:12:48.000000 proptables-0.0.6/proptables/R134a/calSuperHeatData.py
--rw-rw-rw-   0        0        0      574 2023-06-11 10:30:34.000000 proptables-0.0.6/proptables/R134a/import_data.py
--rw-rw-rw-   0        0        0      113 2023-06-11 10:30:34.000000 proptables-0.0.6/proptables/R134a/interpolate.py
--rw-rw-rw-   0        0        0     1389 2023-06-11 10:30:34.000000 proptables-0.0.6/proptables/R134a/main.py
--rw-rw-rw-   0        0        0     7288 2023-06-12 08:12:48.000000 proptables-0.0.6/proptables/R134a/superheated.py
--rw-rw-rw-   0        0        0     2068 2023-06-13 18:28:04.000000 proptables-0.0.6/proptables/R134a/test.py
--rw-rw-rw-   0        0        0       88 2023-06-11 10:30:34.000000 proptables-0.0.6/proptables/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 18:42:56.011305 proptables-0.0.6/proptables/water/
--rw-rw-rw-   0        0        0     3388 2023-06-11 10:30:34.000000 proptables-0.0.6/proptables/water/H2O_Compressed.csv
--rw-rw-rw-   0        0        0     3894 2023-06-11 10:30:34.000000 proptables-0.0.6/proptables/water/H2O_PresSat.csv
--rw-rw-rw-   0        0        0    15532 2023-06-11 10:30:34.000000 proptables-0.0.6/proptables/water/H2O_Super.csv
--rw-rw-rw-   0        0        0     4185 2023-06-11 10:30:34.000000 proptables-0.0.6/proptables/water/H2O_TempSat.csv
--rw-rw-rw-   0        0        0      395 2023-06-13 18:34:33.000000 proptables-0.0.6/proptables/water/H2O_superSat.csv
--rw-rw-rw-   0        0        0       39 2023-06-11 10:30:34.000000 proptables-0.0.6/proptables/water/__init__.py
--rw-rw-rw-   0        0        0        0 2023-06-11 10:30:34.000000 proptables-0.0.6/proptables/water/calwatercompressed.py
--rw-rw-rw-   0        0        0     4462 2023-06-11 10:30:34.000000 proptables-0.0.6/proptables/water/calwatersat.py
--rw-rw-rw-   0        0        0     4108 2023-06-13 18:34:33.000000 proptables-0.0.6/proptables/water/calwatersuperheat.py
--rw-rw-rw-   0        0        0      527 2023-06-13 18:34:33.000000 proptables-0.0.6/proptables/water/import_data_water.py
--rw-rw-rw-   0        0        0     1383 2023-06-13 18:34:33.000000 proptables-0.0.6/proptables/water/main.py
--rw-rw-rw-   0        0        0      161 2023-06-11 10:30:34.000000 proptables-0.0.6/proptables/water/mainwater.py
--rw-rw-rw-   0        0        0    10703 2023-06-13 18:37:15.000000 proptables-0.0.6/proptables/water/superheated.py
--rw-rw-rw-   0        0        0     1262 2023-06-13 18:34:33.000000 proptables-0.0.6/proptables/water/test.py
-drwxrwxrwx   0        0        0        0 2023-06-13 18:42:55.621233 proptables-0.0.6/proptables.egg-info/
--rw-rw-rw-   0        0        0     2452 2023-06-13 18:42:55.000000 proptables-0.0.6/proptables.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1055 2023-06-13 18:42:55.000000 proptables-0.0.6/proptables.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 18:42:55.000000 proptables-0.0.6/proptables.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-13 18:42:55.000000 proptables-0.0.6/proptables.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2023-06-05 08:01:30.000000 proptables-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0      593 2023-06-13 18:42:56.022228 proptables-0.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-13 19:26:21.679477 proptables-0.0.7/
+-rw-rw-rw-   0        0        0     1070 2023-06-03 19:14:15.000000 proptables-0.0.7/LICENCE.txt
+-rw-rw-rw-   0        0        0       62 2023-06-11 10:30:34.000000 proptables-0.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     2427 2023-06-13 19:26:21.679477 proptables-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1928 2023-06-13 19:26:16.000000 proptables-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-13 19:26:21.578243 proptables-0.0.7/proptables/
+drwxrwxrwx   0        0        0        0 2023-06-13 19:26:21.651538 proptables-0.0.7/proptables/R134a/
+-rw-rw-rw-   0        0        0     2379 2023-06-11 10:30:34.000000 proptables-0.0.7/proptables/R134a/R134a_PresSat.csv
+-rw-rw-rw-   0        0        0      239 2023-06-11 10:30:34.000000 proptables-0.0.7/proptables/R134a/R134a_SupPreSat.csv
+-rw-rw-rw-   0        0        0     9904 2023-06-11 10:30:34.000000 proptables-0.0.7/proptables/R134a/R134a_Super.csv
+-rw-rw-rw-   0        0        0     3782 2023-06-11 10:30:34.000000 proptables-0.0.7/proptables/R134a/R134a_TempSat.csv
+-rw-rw-rw-   0        0        0       39 2023-06-11 10:30:34.000000 proptables-0.0.7/proptables/R134a/__init__.py
+-rw-rw-rw-   0        0        0     4503 2023-06-11 10:30:34.000000 proptables-0.0.7/proptables/R134a/calSatData.py
+-rw-rw-rw-   0        0        0     4210 2023-06-12 08:12:48.000000 proptables-0.0.7/proptables/R134a/calSuperHeatData.py
+-rw-rw-rw-   0        0        0      574 2023-06-11 10:30:34.000000 proptables-0.0.7/proptables/R134a/import_data.py
+-rw-rw-rw-   0        0        0      113 2023-06-11 10:30:34.000000 proptables-0.0.7/proptables/R134a/interpolate.py
+-rw-rw-rw-   0        0        0     1389 2023-06-11 10:30:34.000000 proptables-0.0.7/proptables/R134a/main.py
+-rw-rw-rw-   0        0        0     7334 2023-06-13 19:24:16.000000 proptables-0.0.7/proptables/R134a/superheated.py
+-rw-rw-rw-   0        0        0     2068 2023-06-13 18:28:04.000000 proptables-0.0.7/proptables/R134a/test.py
+-rw-rw-rw-   0        0        0       88 2023-06-11 10:30:34.000000 proptables-0.0.7/proptables/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 19:26:21.678480 proptables-0.0.7/proptables/water/
+-rw-rw-rw-   0        0        0     3388 2023-06-11 10:30:34.000000 proptables-0.0.7/proptables/water/H2O_Compressed.csv
+-rw-rw-rw-   0        0        0     3894 2023-06-11 10:30:34.000000 proptables-0.0.7/proptables/water/H2O_PresSat.csv
+-rw-rw-rw-   0        0        0    15532 2023-06-11 10:30:34.000000 proptables-0.0.7/proptables/water/H2O_Super.csv
+-rw-rw-rw-   0        0        0     4185 2023-06-11 10:30:34.000000 proptables-0.0.7/proptables/water/H2O_TempSat.csv
+-rw-rw-rw-   0        0        0      395 2023-06-13 18:34:33.000000 proptables-0.0.7/proptables/water/H2O_superSat.csv
+-rw-rw-rw-   0        0        0       39 2023-06-11 10:30:34.000000 proptables-0.0.7/proptables/water/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-06-11 10:30:34.000000 proptables-0.0.7/proptables/water/calwatercompressed.py
+-rw-rw-rw-   0        0        0     4462 2023-06-11 10:30:34.000000 proptables-0.0.7/proptables/water/calwatersat.py
+-rw-rw-rw-   0        0        0     4108 2023-06-13 18:34:33.000000 proptables-0.0.7/proptables/water/calwatersuperheat.py
+-rw-rw-rw-   0        0        0      527 2023-06-13 18:34:33.000000 proptables-0.0.7/proptables/water/import_data_water.py
+-rw-rw-rw-   0        0        0     1383 2023-06-13 18:34:33.000000 proptables-0.0.7/proptables/water/main.py
+-rw-rw-rw-   0        0        0      161 2023-06-11 10:30:34.000000 proptables-0.0.7/proptables/water/mainwater.py
+-rw-rw-rw-   0        0        0    10749 2023-06-13 19:23:27.000000 proptables-0.0.7/proptables/water/superheated.py
+-rw-rw-rw-   0        0        0     1262 2023-06-13 18:34:33.000000 proptables-0.0.7/proptables/water/test.py
+drwxrwxrwx   0        0        0        0 2023-06-13 19:26:21.630002 proptables-0.0.7/proptables.egg-info/
+-rw-rw-rw-   0        0        0     2427 2023-06-13 19:26:21.000000 proptables-0.0.7/proptables.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1055 2023-06-13 19:26:21.000000 proptables-0.0.7/proptables.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 19:26:21.000000 proptables-0.0.7/proptables.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-13 19:26:21.000000 proptables-0.0.7/proptables.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2023-06-05 08:01:30.000000 proptables-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0      593 2023-06-13 19:26:21.681510 proptables-0.0.7/setup.cfg
```

### Comparing `proptables-0.0.6/LICENCE.txt` & `proptables-0.0.7/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `proptables-0.0.6/PKG-INFO` & `proptables-0.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proptables
-Version: 0.0.6
+Version: 0.0.7
 Summary: For generating property table values for given input
 Home-page: https://github.com/Buddhi19/PropertyTables_Python
 Author: Buddhi Wijenayake
 Author-email: wijenayakebuddhi34802@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,23 +12,23 @@
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
 
 [![PyPI version](https://badge.fury.io/py/proptables.svg)](https://badge.fury.io/py/proptables)
 [![pypi supported versions](https://img.shields.io/pypi/pyversions/proptables.svg)](https://pypi.python.org/pypi/proptables)
 # Python proptables
 #### proptables is a Python library designed to provide easy access to comprehensive property tables for R134a 
-##### (water-steam tables will be implemented soon). 
 
 # To Install
 ```bash
 pip install proptables
 ```
 ## How to use
 ```python
 from proptables import R134a
+from proptables import water
 ```
 
 ## To find data in saturated liquid vapour region
 
 Use either one of followings
 ```python
 R134a(Pressure=VALUE_IN_KPA)
```

### Comparing `proptables-0.0.6/README.md` & `proptables-0.0.7/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [![PyPI version](https://badge.fury.io/py/proptables.svg)](https://badge.fury.io/py/proptables)
 [![pypi supported versions](https://img.shields.io/pypi/pyversions/proptables.svg)](https://pypi.python.org/pypi/proptables)
 # Python proptables
 #### proptables is a Python library designed to provide easy access to comprehensive property tables for R134a 
-##### (water-steam tables will be implemented soon). 
 
 # To Install
 ```bash
 pip install proptables
 ```
 ## How to use
 ```python
 from proptables import R134a
+from proptables import water
 ```
 
 ## To find data in saturated liquid vapour region
 
 Use either one of followings
 ```python
 R134a(Pressure=VALUE_IN_KPA)
```

### Comparing `proptables-0.0.6/proptables/R134a/R134a_PresSat.csv` & `proptables-0.0.7/proptables/R134a/R134a_PresSat.csv`

 * *Files identical despite different names*

### Comparing `proptables-0.0.6/proptables/R134a/R134a_Super.csv` & `proptables-0.0.7/proptables/R134a/R134a_Super.csv`

 * *Files identical despite different names*

### Comparing `proptables-0.0.6/proptables/R134a/R134a_TempSat.csv` & `proptables-0.0.7/proptables/R134a/R134a_TempSat.csv`

 * *Files identical despite different names*

### Comparing `proptables-0.0.6/proptables/R134a/calSatData.py` & `proptables-0.0.7/proptables/R134a/calSatData.py`

 * *Files identical despite different names*

### Comparing `proptables-0.0.6/proptables/R134a/calSuperHeatData.py` & `proptables-0.0.7/proptables/R134a/calSuperHeatData.py`

 * *Files identical despite different names*

### Comparing `proptables-0.0.6/proptables/R134a/import_data.py` & `proptables-0.0.7/proptables/R134a/import_data.py`

 * *Files identical despite different names*

### Comparing `proptables-0.0.6/proptables/R134a/main.py` & `proptables-0.0.7/proptables/R134a/main.py`

 * *Files identical despite different names*

### Comparing `proptables-0.0.6/proptables/R134a/superheated.py` & `proptables-0.0.7/proptables/R134a/superheated.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,14 +134,15 @@
     def superheatedTable_interpolate(self,result,Pressure):
         result=result.reset_index(drop=True)
         result=result.set_axis(["Temp","v","energy","enthalpy","entropy"],axis=1)
         if Pressure in self.dfSupSat["Pressure"].values:
             indexing=self.dfSupSat[self.dfSupSat["Pressure"].values==Pressure].index.values
             result["Temp"].values[1]=self.dfSupSat["SaturatedTemperature"].values[indexing][0]
         result=result.iloc[1:]
+        result=result.reset_index(drop=True)
         result=result.apply(pd.to_numeric)
         return result
     
     def superheated_Pres_unknown(self,table1,Pressure1,table2,Pressure2,Pressure):
         table1=self.superheatedTable_interpolate(table1,Pressure1)
         table2=self.superheatedTable_interpolate(table2,Pressure2)
```

### Comparing `proptables-0.0.6/proptables/R134a/test.py` & `proptables-0.0.7/proptables/R134a/test.py`

 * *Files identical despite different names*

### Comparing `proptables-0.0.6/proptables/water/H2O_Compressed.csv` & `proptables-0.0.7/proptables/water/H2O_Compressed.csv`

 * *Files identical despite different names*

### Comparing `proptables-0.0.6/proptables/water/H2O_PresSat.csv` & `proptables-0.0.7/proptables/water/H2O_PresSat.csv`

 * *Files identical despite different names*

### Comparing `proptables-0.0.6/proptables/water/H2O_Super.csv` & `proptables-0.0.7/proptables/water/H2O_Super.csv`

 * *Files identical despite different names*

### Comparing `proptables-0.0.6/proptables/water/H2O_TempSat.csv` & `proptables-0.0.7/proptables/water/H2O_TempSat.csv`

 * *Files identical despite different names*

### Comparing `proptables-0.0.6/proptables/water/calwatersat.py` & `proptables-0.0.7/proptables/water/calwatersat.py`

 * *Files identical despite different names*

### Comparing `proptables-0.0.6/proptables/water/calwatersuperheat.py` & `proptables-0.0.7/proptables/water/calwatersuperheat.py`

 * *Files identical despite different names*

### Comparing `proptables-0.0.6/proptables/water/import_data_water.py` & `proptables-0.0.7/proptables/water/import_data_water.py`

 * *Files identical despite different names*

### Comparing `proptables-0.0.6/proptables/water/main.py` & `proptables-0.0.7/proptables/water/main.py`

 * *Files identical despite different names*

### Comparing `proptables-0.0.6/proptables/water/superheated.py` & `proptables-0.0.7/proptables/water/superheated.py`

 * *Files 1% similar despite different names*

```diff
@@ -217,14 +217,15 @@
     def superheatedTable_interpolate(self,result,Pressure):
         result=result.reset_index(drop=True)
         result=result.set_axis(["Temp","v","energy","enthalpy","entropy"],axis=1)
         if Pressure in self.dfSupSat["Pressure"].values:
             indexing=self.dfSupSat[self.dfSupSat["Pressure"].values==Pressure].index.values
             result["Temp"].values[1]=self.dfSupSat["SaturatedTemp"].values[indexing][0]
         result=result.iloc[1:]
+        result=result.reset_index(drop=True)
         result=result.apply(pd.to_numeric)
         return result
     
     def superheated_Pres_unknown(self,table1,Pressure1,table2,Pressure2,Pressure):
         table1=self.superheatedTable_interpolate(table1,Pressure1)
         table2=self.superheatedTable_interpolate(table2,Pressure2)
```

### Comparing `proptables-0.0.6/proptables/water/test.py` & `proptables-0.0.7/proptables/water/test.py`

 * *Files identical despite different names*

### Comparing `proptables-0.0.6/proptables.egg-info/PKG-INFO` & `proptables-0.0.7/proptables.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proptables
-Version: 0.0.6
+Version: 0.0.7
 Summary: For generating property table values for given input
 Home-page: https://github.com/Buddhi19/PropertyTables_Python
 Author: Buddhi Wijenayake
 Author-email: wijenayakebuddhi34802@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,23 +12,23 @@
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
 
 [![PyPI version](https://badge.fury.io/py/proptables.svg)](https://badge.fury.io/py/proptables)
 [![pypi supported versions](https://img.shields.io/pypi/pyversions/proptables.svg)](https://pypi.python.org/pypi/proptables)
 # Python proptables
 #### proptables is a Python library designed to provide easy access to comprehensive property tables for R134a 
-##### (water-steam tables will be implemented soon). 
 
 # To Install
 ```bash
 pip install proptables
 ```
 ## How to use
 ```python
 from proptables import R134a
+from proptables import water
 ```
 
 ## To find data in saturated liquid vapour region
 
 Use either one of followings
 ```python
 R134a(Pressure=VALUE_IN_KPA)
```

### Comparing `proptables-0.0.6/proptables.egg-info/SOURCES.txt` & `proptables-0.0.7/proptables.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `proptables-0.0.6/setup.cfg` & `proptables-0.0.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 726f 7074 6162 6c65 730d 0a76   = proptables..v
-00000020: 6572 7369 6f6e 203d 2030 2e30 2e36 0d0a  ersion = 0.0.6..
+00000020: 6572 7369 6f6e 203d 2030 2e30 2e37 0d0a  ersion = 0.0.7..
 00000030: 6175 7468 6f72 203d 2042 7564 6468 6920  author = Buddhi 
 00000040: 5769 6a65 6e61 7961 6b65 0d0a 6175 7468  Wijenayake..auth
 00000050: 6f72 5f65 6d61 696c 203d 2077 696a 656e  or_email = wijen
 00000060: 6179 616b 6562 7564 6468 6933 3438 3032  ayakebuddhi34802
 00000070: 4067 6d61 696c 2e63 6f6d 0d0a 6465 7363  @gmail.com..desc
 00000080: 7269 7074 696f 6e20 3d20 466f 7220 6765  ription = For ge
 00000090: 6e65 7261 7469 6e67 2070 726f 7065 7274  nerating propert
```

