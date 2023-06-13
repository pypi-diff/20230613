# Comparing `tmp/proptables-0.0.5.tar.gz` & `tmp/proptables-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proptables-0.0.5.tar", last modified: Mon Jun 12 09:44:08 2023, max compression
+gzip compressed data, was "proptables-0.0.6.tar", last modified: Tue Jun 13 18:42:56 2023, max compression
```

## Comparing `proptables-0.0.5.tar` & `proptables-0.0.6.tar`

### file list

```diff
@@ -1,40 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 09:44:08.166547 proptables-0.0.5/
--rw-rw-rw-   0        0        0     1070 2023-06-03 19:14:15.000000 proptables-0.0.5/LICENCE.txt
--rw-rw-rw-   0        0        0       62 2023-06-11 10:30:34.000000 proptables-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0     2452 2023-06-12 09:44:08.166547 proptables-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1953 2023-06-07 09:25:23.000000 proptables-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 09:44:07.829018 proptables-0.0.5/proptables/
-drwxrwxrwx   0        0        0        0 2023-06-12 09:44:07.849117 proptables-0.0.5/proptables/R134a/
--rw-rw-rw-   0        0        0     2379 2023-06-11 10:30:34.000000 proptables-0.0.5/proptables/R134a/R134a_PresSat.csv
--rw-rw-rw-   0        0        0      239 2023-06-11 10:30:34.000000 proptables-0.0.5/proptables/R134a/R134a_SupPreSat.csv
--rw-rw-rw-   0        0        0     9904 2023-06-11 10:30:34.000000 proptables-0.0.5/proptables/R134a/R134a_Super.csv
--rw-rw-rw-   0        0        0     3782 2023-06-11 10:30:34.000000 proptables-0.0.5/proptables/R134a/R134a_TempSat.csv
--rw-rw-rw-   0        0        0       39 2023-06-11 10:30:34.000000 proptables-0.0.5/proptables/R134a/__init__.py
--rw-rw-rw-   0        0        0     4503 2023-06-11 10:30:34.000000 proptables-0.0.5/proptables/R134a/calSatData.py
--rw-rw-rw-   0        0        0     4210 2023-06-12 08:12:48.000000 proptables-0.0.5/proptables/R134a/calSuperHeatData.py
--rw-rw-rw-   0        0        0      574 2023-06-11 10:30:34.000000 proptables-0.0.5/proptables/R134a/import_data.py
--rw-rw-rw-   0        0        0      113 2023-06-11 10:30:34.000000 proptables-0.0.5/proptables/R134a/interpolate.py
--rw-rw-rw-   0        0        0     1389 2023-06-11 10:30:34.000000 proptables-0.0.5/proptables/R134a/main.py
--rw-rw-rw-   0        0        0     7288 2023-06-12 08:12:48.000000 proptables-0.0.5/proptables/R134a/superheated.py
--rw-rw-rw-   0        0        0     2068 2023-06-11 10:30:34.000000 proptables-0.0.5/proptables/R134a/test.py
--rw-rw-rw-   0        0        0       88 2023-06-11 10:30:34.000000 proptables-0.0.5/proptables/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 09:44:08.166547 proptables-0.0.5/proptables/water/
--rw-rw-rw-   0        0        0     3388 2023-06-11 10:30:34.000000 proptables-0.0.5/proptables/water/H2O_Compressed.csv
--rw-rw-rw-   0        0        0     3894 2023-06-11 10:30:34.000000 proptables-0.0.5/proptables/water/H2O_PresSat.csv
--rw-rw-rw-   0        0        0    15532 2023-06-11 10:30:34.000000 proptables-0.0.5/proptables/water/H2O_Super.csv
--rw-rw-rw-   0        0        0     4185 2023-06-11 10:30:34.000000 proptables-0.0.5/proptables/water/H2O_TempSat.csv
--rw-rw-rw-   0        0        0       39 2023-06-11 10:30:34.000000 proptables-0.0.5/proptables/water/__init__.py
--rw-rw-rw-   0        0        0        0 2023-06-11 10:30:34.000000 proptables-0.0.5/proptables/water/calwatercompressed.py
--rw-rw-rw-   0        0        0     4462 2023-06-11 10:30:34.000000 proptables-0.0.5/proptables/water/calwatersat.py
--rw-rw-rw-   0        0        0        0 2023-06-11 10:30:34.000000 proptables-0.0.5/proptables/water/calwatersuperheat.py
--rw-rw-rw-   0        0        0      419 2023-06-11 10:30:34.000000 proptables-0.0.5/proptables/water/import_data_water.py
--rw-rw-rw-   0        0        0      794 2023-06-11 10:30:34.000000 proptables-0.0.5/proptables/water/main.py
--rw-rw-rw-   0        0        0      161 2023-06-11 10:30:34.000000 proptables-0.0.5/proptables/water/mainwater.py
--rw-rw-rw-   0        0        0      956 2023-06-11 10:30:34.000000 proptables-0.0.5/proptables/water/test.py
-drwxrwxrwx   0        0        0        0 2023-06-12 09:44:07.839037 proptables-0.0.5/proptables.egg-info/
--rw-rw-rw-   0        0        0     2452 2023-06-12 09:44:07.000000 proptables-0.0.5/proptables.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      989 2023-06-12 09:44:07.000000 proptables-0.0.5/proptables.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 09:44:07.000000 proptables-0.0.5/proptables.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-12 09:44:07.000000 proptables-0.0.5/proptables.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2023-06-05 08:01:30.000000 proptables-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0      593 2023-06-12 09:44:08.175644 proptables-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-13 18:42:56.011305 proptables-0.0.6/
+-rw-rw-rw-   0        0        0     1070 2023-06-03 19:14:15.000000 proptables-0.0.6/LICENCE.txt
+-rw-rw-rw-   0        0        0       62 2023-06-11 10:30:34.000000 proptables-0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     2452 2023-06-13 18:42:56.011305 proptables-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1953 2023-06-07 09:25:23.000000 proptables-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-13 18:42:55.612055 proptables-0.0.6/proptables/
+drwxrwxrwx   0        0        0        0 2023-06-13 18:42:55.902417 proptables-0.0.6/proptables/R134a/
+-rw-rw-rw-   0        0        0     2379 2023-06-11 10:30:34.000000 proptables-0.0.6/proptables/R134a/R134a_PresSat.csv
+-rw-rw-rw-   0        0        0      239 2023-06-11 10:30:34.000000 proptables-0.0.6/proptables/R134a/R134a_SupPreSat.csv
+-rw-rw-rw-   0        0        0     9904 2023-06-11 10:30:34.000000 proptables-0.0.6/proptables/R134a/R134a_Super.csv
+-rw-rw-rw-   0        0        0     3782 2023-06-11 10:30:34.000000 proptables-0.0.6/proptables/R134a/R134a_TempSat.csv
+-rw-rw-rw-   0        0        0       39 2023-06-11 10:30:34.000000 proptables-0.0.6/proptables/R134a/__init__.py
+-rw-rw-rw-   0        0        0     4503 2023-06-11 10:30:34.000000 proptables-0.0.6/proptables/R134a/calSatData.py
+-rw-rw-rw-   0        0        0     4210 2023-06-12 08:12:48.000000 proptables-0.0.6/proptables/R134a/calSuperHeatData.py
+-rw-rw-rw-   0        0        0      574 2023-06-11 10:30:34.000000 proptables-0.0.6/proptables/R134a/import_data.py
+-rw-rw-rw-   0        0        0      113 2023-06-11 10:30:34.000000 proptables-0.0.6/proptables/R134a/interpolate.py
+-rw-rw-rw-   0        0        0     1389 2023-06-11 10:30:34.000000 proptables-0.0.6/proptables/R134a/main.py
+-rw-rw-rw-   0        0        0     7288 2023-06-12 08:12:48.000000 proptables-0.0.6/proptables/R134a/superheated.py
+-rw-rw-rw-   0        0        0     2068 2023-06-13 18:28:04.000000 proptables-0.0.6/proptables/R134a/test.py
+-rw-rw-rw-   0        0        0       88 2023-06-11 10:30:34.000000 proptables-0.0.6/proptables/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 18:42:56.011305 proptables-0.0.6/proptables/water/
+-rw-rw-rw-   0        0        0     3388 2023-06-11 10:30:34.000000 proptables-0.0.6/proptables/water/H2O_Compressed.csv
+-rw-rw-rw-   0        0        0     3894 2023-06-11 10:30:34.000000 proptables-0.0.6/proptables/water/H2O_PresSat.csv
+-rw-rw-rw-   0        0        0    15532 2023-06-11 10:30:34.000000 proptables-0.0.6/proptables/water/H2O_Super.csv
+-rw-rw-rw-   0        0        0     4185 2023-06-11 10:30:34.000000 proptables-0.0.6/proptables/water/H2O_TempSat.csv
+-rw-rw-rw-   0        0        0      395 2023-06-13 18:34:33.000000 proptables-0.0.6/proptables/water/H2O_superSat.csv
+-rw-rw-rw-   0        0        0       39 2023-06-11 10:30:34.000000 proptables-0.0.6/proptables/water/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-06-11 10:30:34.000000 proptables-0.0.6/proptables/water/calwatercompressed.py
+-rw-rw-rw-   0        0        0     4462 2023-06-11 10:30:34.000000 proptables-0.0.6/proptables/water/calwatersat.py
+-rw-rw-rw-   0        0        0     4108 2023-06-13 18:34:33.000000 proptables-0.0.6/proptables/water/calwatersuperheat.py
+-rw-rw-rw-   0        0        0      527 2023-06-13 18:34:33.000000 proptables-0.0.6/proptables/water/import_data_water.py
+-rw-rw-rw-   0        0        0     1383 2023-06-13 18:34:33.000000 proptables-0.0.6/proptables/water/main.py
+-rw-rw-rw-   0        0        0      161 2023-06-11 10:30:34.000000 proptables-0.0.6/proptables/water/mainwater.py
+-rw-rw-rw-   0        0        0    10703 2023-06-13 18:37:15.000000 proptables-0.0.6/proptables/water/superheated.py
+-rw-rw-rw-   0        0        0     1262 2023-06-13 18:34:33.000000 proptables-0.0.6/proptables/water/test.py
+drwxrwxrwx   0        0        0        0 2023-06-13 18:42:55.621233 proptables-0.0.6/proptables.egg-info/
+-rw-rw-rw-   0        0        0     2452 2023-06-13 18:42:55.000000 proptables-0.0.6/proptables.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1055 2023-06-13 18:42:55.000000 proptables-0.0.6/proptables.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 18:42:55.000000 proptables-0.0.6/proptables.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-13 18:42:55.000000 proptables-0.0.6/proptables.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2023-06-05 08:01:30.000000 proptables-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0      593 2023-06-13 18:42:56.022228 proptables-0.0.6/setup.cfg
```

### Comparing `proptables-0.0.5/LICENCE.txt` & `proptables-0.0.6/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `proptables-0.0.5/PKG-INFO` & `proptables-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proptables
-Version: 0.0.5
+Version: 0.0.6
 Summary: For generating property table values for given input
 Home-page: https://github.com/Buddhi19/PropertyTables_Python
 Author: Buddhi Wijenayake
 Author-email: wijenayakebuddhi34802@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `proptables-0.0.5/README.md` & `proptables-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `proptables-0.0.5/proptables/R134a/R134a_PresSat.csv` & `proptables-0.0.6/proptables/R134a/R134a_PresSat.csv`

 * *Files identical despite different names*

### Comparing `proptables-0.0.5/proptables/R134a/R134a_Super.csv` & `proptables-0.0.6/proptables/R134a/R134a_Super.csv`

 * *Files identical despite different names*

### Comparing `proptables-0.0.5/proptables/R134a/R134a_TempSat.csv` & `proptables-0.0.6/proptables/R134a/R134a_TempSat.csv`

 * *Files identical despite different names*

### Comparing `proptables-0.0.5/proptables/R134a/calSatData.py` & `proptables-0.0.6/proptables/R134a/calSatData.py`

 * *Files identical despite different names*

### Comparing `proptables-0.0.5/proptables/R134a/calSuperHeatData.py` & `proptables-0.0.6/proptables/R134a/calSuperHeatData.py`

 * *Files identical despite different names*

### Comparing `proptables-0.0.5/proptables/R134a/import_data.py` & `proptables-0.0.6/proptables/R134a/import_data.py`

 * *Files identical despite different names*

### Comparing `proptables-0.0.5/proptables/R134a/main.py` & `proptables-0.0.6/proptables/R134a/main.py`

 * *Files identical despite different names*

### Comparing `proptables-0.0.5/proptables/R134a/superheated.py` & `proptables-0.0.6/proptables/R134a/superheated.py`

 * *Files identical despite different names*

### Comparing `proptables-0.0.5/proptables/R134a/test.py` & `proptables-0.0.6/proptables/R134a/test.py`

 * *Files identical despite different names*

### Comparing `proptables-0.0.5/proptables/water/H2O_Compressed.csv` & `proptables-0.0.6/proptables/water/H2O_Compressed.csv`

 * *Files identical despite different names*

### Comparing `proptables-0.0.5/proptables/water/H2O_PresSat.csv` & `proptables-0.0.6/proptables/water/H2O_PresSat.csv`

 * *Files identical despite different names*

### Comparing `proptables-0.0.5/proptables/water/H2O_Super.csv` & `proptables-0.0.6/proptables/water/H2O_Super.csv`

 * *Files identical despite different names*

### Comparing `proptables-0.0.5/proptables/water/H2O_TempSat.csv` & `proptables-0.0.6/proptables/water/H2O_TempSat.csv`

 * *Files identical despite different names*

### Comparing `proptables-0.0.5/proptables/water/calwatersat.py` & `proptables-0.0.6/proptables/water/calwatersat.py`

 * *Files identical despite different names*

### Comparing `proptables-0.0.5/proptables/water/main.py` & `proptables-0.0.6/proptables/water/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,29 @@
 from proptables.water.calwatersat import SatwaterCal
+from proptables.water.calwatersuperheat import steam
 
 def water(Temperature=None,Pressure=None,
           Enthalpy=None,Entropy=None,
           specificvolume=None,Superheated=None,Compressed=None):
 
+    if Temperature and Pressure:
+        return steam.findsuperTemp(Pressure,Temperature)
+    
+    if Superheated and Pressure and Enthalpy:
+        return steam.findsuperEnthalpy(Pressure,Enthalpy)
+    
+    if Superheated and Pressure and Entropy:
+        return steam.findsuperEntropy(Pressure,Entropy)
+    
+    if Superheated and Pressure and specificvolume:
+        return steam.findsuperspecificvolume(Pressure,specificvolume)
+    
+    if Superheated and Pressure:
+        return steam.superheatedTable(Pressure) 
+
     if Temperature and Enthalpy:
         return(SatwaterCal.calculate_x_temp(Temperature,Enthalpy))
 
     if Pressure and Enthalpy:
         return(SatwaterCal.calculate_x_pressure(Pressure,Enthalpy))
 
     if Pressure and Entropy:
```

### Comparing `proptables-0.0.5/proptables/water/test.py` & `proptables-0.0.6/proptables/water/test.py`

 * *Files 18% similar despite different names*

```diff
@@ -37,7 +37,22 @@
 
 #############################3 pressure entropy #############################3
 
 check_5=True
 
 if check_5:
         print(water(Pressure=1000,Entropy=5))
+
+############################# check for steam ######################################
+
+check_6=True
+
+if check_6:
+     print(water(Pressure=4000,Superheated=True))
+
+
+############################ check 
+
+check_7=True
+
+if check_7:
+     print(water(Pressure=4000,Entropy=6.6796,Superheated=True))
```

### Comparing `proptables-0.0.5/proptables.egg-info/PKG-INFO` & `proptables-0.0.6/proptables.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proptables
-Version: 0.0.5
+Version: 0.0.6
 Summary: For generating property table values for given input
 Home-page: https://github.com/Buddhi19/PropertyTables_Python
 Author: Buddhi Wijenayake
 Author-email: wijenayakebuddhi34802@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `proptables-0.0.5/proptables.egg-info/SOURCES.txt` & `proptables-0.0.6/proptables.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,17 @@
 proptables/R134a/main.py
 proptables/R134a/superheated.py
 proptables/R134a/test.py
 proptables/water/H2O_Compressed.csv
 proptables/water/H2O_PresSat.csv
 proptables/water/H2O_Super.csv
 proptables/water/H2O_TempSat.csv
+proptables/water/H2O_superSat.csv
 proptables/water/__init__.py
 proptables/water/calwatercompressed.py
 proptables/water/calwatersat.py
 proptables/water/calwatersuperheat.py
 proptables/water/import_data_water.py
 proptables/water/main.py
 proptables/water/mainwater.py
+proptables/water/superheated.py
 proptables/water/test.py
```

### Comparing `proptables-0.0.5/setup.cfg` & `proptables-0.0.6/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 726f 7074 6162 6c65 730d 0a76   = proptables..v
-00000020: 6572 7369 6f6e 203d 2030 2e30 2e35 0d0a  ersion = 0.0.5..
+00000020: 6572 7369 6f6e 203d 2030 2e30 2e36 0d0a  ersion = 0.0.6..
 00000030: 6175 7468 6f72 203d 2042 7564 6468 6920  author = Buddhi 
 00000040: 5769 6a65 6e61 7961 6b65 0d0a 6175 7468  Wijenayake..auth
 00000050: 6f72 5f65 6d61 696c 203d 2077 696a 656e  or_email = wijen
 00000060: 6179 616b 6562 7564 6468 6933 3438 3032  ayakebuddhi34802
 00000070: 4067 6d61 696c 2e63 6f6d 0d0a 6465 7363  @gmail.com..desc
 00000080: 7269 7074 696f 6e20 3d20 466f 7220 6765  ription = For ge
 00000090: 6e65 7261 7469 6e67 2070 726f 7065 7274  nerating propert
```

