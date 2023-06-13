# Comparing `tmp/rcsb.utils.validation-0.30.tar.gz` & `tmp/rcsb.utils.validation-0.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcsb.utils.validation-0.30.tar", last modified: Wed Mar 22 20:01:28 2023, max compression
+gzip compressed data, was "rcsb.utils.validation-0.31.tar", last modified: Tue Jun 13 13:40:20 2023, max compression
```

## Comparing `rcsb.utils.validation-0.30.tar` & `rcsb.utils.validation-0.31.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-22 20:01:28.897975 rcsb.utils.validation-0.30/
--rw-r--r--   0 vsts      (1001) docker     (122)     1379 2023-03-22 20:00:07.000000 rcsb.utils.validation-0.30/HISTORY.txt
--rw-r--r--   0 vsts      (1001) docker     (122)    11357 2023-03-22 20:00:07.000000 rcsb.utils.validation-0.30/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)      114 2023-03-22 20:00:07.000000 rcsb.utils.validation-0.30/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)     1679 2023-03-22 20:01:28.897975 rcsb.utils.validation-0.30/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)      985 2023-03-22 20:00:07.000000 rcsb.utils.validation-0.30/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-22 20:01:28.897975 rcsb.utils.validation-0.30/rcsb/
--rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-03-22 20:00:07.000000 rcsb.utils.validation-0.30/rcsb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-22 20:01:28.897975 rcsb.utils.validation-0.30/rcsb/utils/
--rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-03-22 20:00:07.000000 rcsb.utils.validation-0.30/rcsb/utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-22 20:01:28.897975 rcsb.utils.validation-0.30/rcsb/utils/validation/
--rw-r--r--   0 vsts      (1001) docker     (122)     3959 2023-03-22 20:00:07.000000 rcsb.utils.validation-0.30/rcsb/utils/validation/ValidationReportAdapter.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4019 2023-03-22 20:00:07.000000 rcsb.utils.validation-0.30/rcsb/utils/validation/ValidationReportProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    23102 2023-03-22 20:00:07.000000 rcsb.utils.validation-0.30/rcsb/utils/validation/ValidationReportReader.py
--rw-r--r--   0 vsts      (1001) docker     (122)    47343 2023-03-22 20:00:07.000000 rcsb.utils.validation-0.30/rcsb/utils/validation/ValidationReportSchemaUtils.py
--rw-r--r--   0 vsts      (1001) docker     (122)      144 2023-03-22 20:00:07.000000 rcsb.utils.validation-0.30/rcsb/utils/validation/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-22 20:01:28.897975 rcsb.utils.validation-0.30/rcsb.utils.validation.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)     1679 2023-03-22 20:01:28.000000 rcsb.utils.validation-0.30/rcsb.utils.validation.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)      619 2023-03-22 20:01:28.000000 rcsb.utils.validation-0.30/rcsb.utils.validation.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-03-22 20:01:28.000000 rcsb.utils.validation-0.30/rcsb.utils.validation.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-03-22 20:01:16.000000 rcsb.utils.validation-0.30/rcsb.utils.validation.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (122)      134 2023-03-22 20:01:28.000000 rcsb.utils.validation-0.30/rcsb.utils.validation.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        5 2023-03-22 20:01:28.000000 rcsb.utils.validation-0.30/rcsb.utils.validation.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      106 2023-03-22 20:00:07.000000 rcsb.utils.validation-0.30/requirements.txt
--rwxr-xr-x   0 vsts      (1001) docker     (122)      108 2023-03-22 20:01:28.897975 rcsb.utils.validation-0.30/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (122)     2234 2023-03-22 20:00:07.000000 rcsb.utils.validation-0.30/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-13 13:40:20.661293 rcsb.utils.validation-0.31/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1461 2023-06-13 13:38:47.000000 rcsb.utils.validation-0.31/HISTORY.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)    11357 2023-06-13 13:38:47.000000 rcsb.utils.validation-0.31/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)      114 2023-06-13 13:38:47.000000 rcsb.utils.validation-0.31/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)     1679 2023-06-13 13:40:20.661293 rcsb.utils.validation-0.31/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)      985 2023-06-13 13:38:47.000000 rcsb.utils.validation-0.31/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-13 13:40:20.653293 rcsb.utils.validation-0.31/rcsb/
+-rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-06-13 13:38:47.000000 rcsb.utils.validation-0.31/rcsb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-13 13:40:20.657292 rcsb.utils.validation-0.31/rcsb/utils/
+-rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-06-13 13:38:47.000000 rcsb.utils.validation-0.31/rcsb/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-13 13:40:20.661293 rcsb.utils.validation-0.31/rcsb/utils/validation/
+-rw-r--r--   0 vsts      (1001) docker     (122)     3959 2023-06-13 13:38:47.000000 rcsb.utils.validation-0.31/rcsb/utils/validation/ValidationReportAdapter.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4019 2023-06-13 13:38:47.000000 rcsb.utils.validation-0.31/rcsb/utils/validation/ValidationReportProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    23209 2023-06-13 13:38:47.000000 rcsb.utils.validation-0.31/rcsb/utils/validation/ValidationReportReader.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    47343 2023-06-13 13:38:47.000000 rcsb.utils.validation-0.31/rcsb/utils/validation/ValidationReportSchemaUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      144 2023-06-13 13:38:47.000000 rcsb.utils.validation-0.31/rcsb/utils/validation/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-13 13:40:20.657292 rcsb.utils.validation-0.31/rcsb.utils.validation.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1679 2023-06-13 13:40:20.000000 rcsb.utils.validation-0.31/rcsb.utils.validation.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)      619 2023-06-13 13:40:20.000000 rcsb.utils.validation-0.31/rcsb.utils.validation.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-06-13 13:40:20.000000 rcsb.utils.validation-0.31/rcsb.utils.validation.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-06-13 13:40:09.000000 rcsb.utils.validation-0.31/rcsb.utils.validation.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (122)      134 2023-06-13 13:40:20.000000 rcsb.utils.validation-0.31/rcsb.utils.validation.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        5 2023-06-13 13:40:20.000000 rcsb.utils.validation-0.31/rcsb.utils.validation.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      106 2023-06-13 13:38:47.000000 rcsb.utils.validation-0.31/requirements.txt
+-rwxr-xr-x   0 vsts      (1001) docker     (122)      108 2023-06-13 13:40:20.661293 rcsb.utils.validation-0.31/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     2234 2023-06-13 13:38:47.000000 rcsb.utils.validation-0.31/setup.py
```

### Comparing `rcsb.utils.validation-0.30/HISTORY.txt` & `rcsb.utils.validation-0.31/HISTORY.txt`

 * *Files 6% similar despite different names*

```diff
@@ -16,8 +16,9 @@
 20-Aug-2021 V0.24 Suppress verbose logging details in ValidationReportProvider
 26-Aug-2021 V0.25 Additional test for failed cases in ValidationReportProvider
 11-Sep-2021 V0.26 Further adjustments to ValidationReportProvider cache file management
  8-Oct-2021 V0.27 Add ValidationReportAdapter() and deprecate ValidationReportProvider()
 30-Mar-2022 V0.28 Resolve pylint issues
 23-Dec-2022 V0.29 Configuration changes to support tox 4
 22-Mar-2023 V0.30 Update references to py-rcsb_exdb_assets master branch
+12-Jun-2023 V0.31 Handle unknown attributes and element names when converting XML
 #
```

### Comparing `rcsb.utils.validation-0.30/LICENSE` & `rcsb.utils.validation-0.31/LICENSE`

 * *Files identical despite different names*

### Comparing `rcsb.utils.validation-0.30/PKG-INFO` & `rcsb.utils.validation-0.31/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.utils.validation
-Version: 0.30
+Version: 0.31
 Summary: RCSB Python Validation Data Utility Classes
 Home-page: https://github.com/rcsb/py-rcsb_utils_validation
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rcsb.utils.validation-0.30/README.md` & `rcsb.utils.validation-0.31/README.md`

 * *Files identical despite different names*

### Comparing `rcsb.utils.validation-0.30/rcsb/utils/validation/ValidationReportAdapter.py` & `rcsb.utils.validation-0.31/rcsb/utils/validation/ValidationReportAdapter.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.validation-0.30/rcsb/utils/validation/ValidationReportProvider.py` & `rcsb.utils.validation-0.31/rcsb/utils/validation/ValidationReportProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.validation-0.30/rcsb/utils/validation/ValidationReportReader.py` & `rcsb.utils.validation-0.31/rcsb/utils/validation/ValidationReportReader.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ##
 # File:    ValidationReportReader.py
 # Author:  J. Westbrook
 # Date:    24-Jan-2019
 # Version: 0.001
 #
 # Update:
-#
+# 12-Jun-2023 aae Handle unknown attributes and element names when converting XML
 #
 ##
 """
 Various utilities for extracting data wwPDB validation report data
 and transforming these data into mmCIF objects/files.
 
 """
@@ -81,15 +81,15 @@
             containers (list):  data container list
         """
         #
 
         curContainer = DataContainer(containerName)
         for elName in rD:
             catName = elName
-            if (not rD[elName]) or (not self.__attribD[catName]) or (catName in ["programs"]):
+            if (not rD[elName]) or (not self.__attribD.get(catName)) or (catName in ["programs"]):
                 continue
             hasOrdinal = "ordinal" in self.__attribD[catName]
             rowList = rD[elName]
             # Find the unique attribute content across the rowlist and the ordinal value
             atS = set()
             for ii, rowD in enumerate(rowList, 1):
                 if hasOrdinal:
@@ -99,15 +99,15 @@
                 if "altcode" in rowD:
                     rowD["altcode"] = str(rowD["altcode"]).strip()
                 atS.update(rowD.keys())
             attributeNameList = list(atS)
             #
             # Set a reasonable order for these attributes
             #
-            sD = {ky: self.__atOrdD[ky] for ky in attributeNameList}
+            sD = {ky: self.__atOrdD[ky] for ky in attributeNameList if ky in self.__atOrdD}
             srtAtL = [tup[0] for tup in sorted(sD.items(), key=operator.itemgetter(1))]
             logger.debug("Category %s sorted attributes %r", catName, srtAtL)
 
             aCat = DataCategory(catName, srtAtL, rowList)
             curContainer.append(aCat)
         #
         # Adjust schema names -
```

### Comparing `rcsb.utils.validation-0.30/rcsb/utils/validation/ValidationReportSchemaUtils.py` & `rcsb.utils.validation-0.31/rcsb/utils/validation/ValidationReportSchemaUtils.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.validation-0.30/rcsb.utils.validation.egg-info/PKG-INFO` & `rcsb.utils.validation-0.31/rcsb.utils.validation.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.utils.validation
-Version: 0.30
+Version: 0.31
 Summary: RCSB Python Validation Data Utility Classes
 Home-page: https://github.com/rcsb/py-rcsb_utils_validation
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rcsb.utils.validation-0.30/rcsb.utils.validation.egg-info/SOURCES.txt` & `rcsb.utils.validation-0.31/rcsb.utils.validation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rcsb.utils.validation-0.30/setup.py` & `rcsb.utils.validation-0.31/setup.py`

 * *Files identical despite different names*

