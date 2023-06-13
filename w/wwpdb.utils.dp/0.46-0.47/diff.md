# Comparing `tmp/wwpdb.utils.dp-0.46.tar.gz` & `tmp/wwpdb.utils.dp-0.47.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wwpdb.utils.dp-0.46.tar", last modified: Sun Jun 11 23:57:20 2023, max compression
+gzip compressed data, was "wwpdb.utils.dp-0.47.tar", last modified: Tue Jun 13 02:55:11 2023, max compression
```

## Comparing `wwpdb.utils.dp-0.46.tar` & `wwpdb.utils.dp-0.47.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-11 23:57:20.783711 wwpdb.utils.dp-0.46/
--rw-r--r--   0 vsts      (1001) docker     (123)       96 2023-06-11 23:56:32.000000 wwpdb.utils.dp-0.46/HISTORY.txt
--rw-r--r--   0 vsts      (1001) docker     (123)      552 2023-06-11 23:56:32.000000 wwpdb.utils.dp-0.46/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (123)      104 2023-06-11 23:56:32.000000 wwpdb.utils.dp-0.46/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (123)      755 2023-06-11 23:57:20.783711 wwpdb.utils.dp-0.46/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      180 2023-06-11 23:56:32.000000 wwpdb.utils.dp-0.46/README.md
--rwxr-xr-x   0 vsts      (1001) docker     (123)      108 2023-06-11 23:57:20.783711 wwpdb.utils.dp-0.46/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (123)     2125 2023-06-11 23:56:32.000000 wwpdb.utils.dp-0.46/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-11 23:57:20.783711 wwpdb.utils.dp-0.46/wwpdb/
--rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-06-11 23:56:32.000000 wwpdb.utils.dp-0.46/wwpdb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-11 23:57:20.783711 wwpdb.utils.dp-0.46/wwpdb/utils/
--rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-06-11 23:56:32.000000 wwpdb.utils.dp-0.46/wwpdb/utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-11 23:57:20.783711 wwpdb.utils.dp-0.46/wwpdb/utils/dp/
--rw-r--r--   0 vsts      (1001) docker     (123)     5332 2023-06-11 23:56:32.000000 wwpdb.utils.dp-0.46/wwpdb/utils/dp/CentreOfMass.py
--rw-r--r--   0 vsts      (1001) docker     (123)    11569 2023-06-11 23:56:32.000000 wwpdb.utils.dp-0.46/wwpdb/utils/dp/DataFileAdapter.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2358 2023-06-11 23:56:32.000000 wwpdb.utils.dp-0.46/wwpdb/utils/dp/DensityWrapper.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1782 2023-06-11 23:56:32.000000 wwpdb.utils.dp-0.46/wwpdb/utils/dp/DepositorSyncUtil.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1918 2023-06-11 23:56:32.000000 wwpdb.utils.dp-0.46/wwpdb/utils/dp/PdbxChemShiftReport.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2694 2023-06-11 23:56:32.000000 wwpdb.utils.dp-0.46/wwpdb/utils/dp/PdbxMergeCategory.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5231 2023-06-11 23:56:32.000000 wwpdb.utils.dp-0.46/wwpdb/utils/dp/PdbxSFMapCoefficients.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2368 2023-06-11 23:56:32.000000 wwpdb.utils.dp-0.46/wwpdb/utils/dp/PdbxStripCategory.py
--rw-r--r--   0 vsts      (1001) docker     (123)   207589 2023-06-11 23:56:32.000000 wwpdb.utils.dp-0.46/wwpdb/utils/dp/RcsbDpUtility.py
--rw-r--r--   0 vsts      (1001) docker     (123)    17219 2023-06-11 23:56:32.000000 wwpdb.utils.dp-0.46/wwpdb/utils/dp/RunRemote.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4429 2023-06-11 23:56:32.000000 wwpdb.utils.dp-0.46/wwpdb/utils/dp/ValidationWrapper.py
--rw-r--r--   0 vsts      (1001) docker     (123)      154 2023-06-11 23:56:32.000000 wwpdb.utils.dp-0.46/wwpdb/utils/dp/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-11 23:57:20.783711 wwpdb.utils.dp-0.46/wwpdb/utils/dp/electron_density/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-11 23:56:32.000000 wwpdb.utils.dp-0.46/wwpdb/utils/dp/electron_density/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3930 2023-06-11 23:56:32.000000 wwpdb.utils.dp-0.46/wwpdb/utils/dp/electron_density/common_functions.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3801 2023-06-11 23:56:32.000000 wwpdb.utils.dp-0.46/wwpdb/utils/dp/electron_density/em_density_map.py
--rw-r--r--   0 vsts      (1001) docker     (123)    10279 2023-06-11 23:56:32.000000 wwpdb.utils.dp-0.46/wwpdb/utils/dp/electron_density/x_ray_density_map.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-11 23:57:20.783711 wwpdb.utils.dp-0.46/wwpdb.utils.dp.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)      755 2023-06-11 23:57:20.000000 wwpdb.utils.dp-0.46/wwpdb.utils.dp.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      934 2023-06-11 23:57:20.000000 wwpdb.utils.dp-0.46/wwpdb.utils.dp.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-11 23:57:20.000000 wwpdb.utils.dp-0.46/wwpdb.utils.dp.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-11 23:57:10.000000 wwpdb.utils.dp-0.46/wwpdb.utils.dp.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)      103 2023-06-11 23:57:20.000000 wwpdb.utils.dp-0.46/wwpdb.utils.dp.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        6 2023-06-11 23:57:20.000000 wwpdb.utils.dp-0.46/wwpdb.utils.dp.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:55:11.806033 wwpdb.utils.dp-0.47/
+-rw-r--r--   0 vsts      (1001) docker     (123)       96 2023-06-13 02:54:10.000000 wwpdb.utils.dp-0.47/HISTORY.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)      552 2023-06-13 02:54:10.000000 wwpdb.utils.dp-0.47/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (123)      104 2023-06-13 02:54:10.000000 wwpdb.utils.dp-0.47/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (123)      755 2023-06-13 02:55:11.806033 wwpdb.utils.dp-0.47/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      180 2023-06-13 02:54:10.000000 wwpdb.utils.dp-0.47/README.md
+-rwxr-xr-x   0 vsts      (1001) docker     (123)      108 2023-06-13 02:55:11.806033 wwpdb.utils.dp-0.47/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (123)     2125 2023-06-13 02:54:10.000000 wwpdb.utils.dp-0.47/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:55:11.794033 wwpdb.utils.dp-0.47/wwpdb/
+-rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-06-13 02:54:10.000000 wwpdb.utils.dp-0.47/wwpdb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:55:11.798034 wwpdb.utils.dp-0.47/wwpdb/utils/
+-rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-06-13 02:54:10.000000 wwpdb.utils.dp-0.47/wwpdb/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:55:11.806033 wwpdb.utils.dp-0.47/wwpdb/utils/dp/
+-rw-r--r--   0 vsts      (1001) docker     (123)     5332 2023-06-13 02:54:10.000000 wwpdb.utils.dp-0.47/wwpdb/utils/dp/CentreOfMass.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    11569 2023-06-13 02:54:10.000000 wwpdb.utils.dp-0.47/wwpdb/utils/dp/DataFileAdapter.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2358 2023-06-13 02:54:10.000000 wwpdb.utils.dp-0.47/wwpdb/utils/dp/DensityWrapper.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1782 2023-06-13 02:54:10.000000 wwpdb.utils.dp-0.47/wwpdb/utils/dp/DepositorSyncUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1918 2023-06-13 02:54:10.000000 wwpdb.utils.dp-0.47/wwpdb/utils/dp/PdbxChemShiftReport.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2694 2023-06-13 02:54:10.000000 wwpdb.utils.dp-0.47/wwpdb/utils/dp/PdbxMergeCategory.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5231 2023-06-13 02:54:10.000000 wwpdb.utils.dp-0.47/wwpdb/utils/dp/PdbxSFMapCoefficients.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2368 2023-06-13 02:54:10.000000 wwpdb.utils.dp-0.47/wwpdb/utils/dp/PdbxStripCategory.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   208527 2023-06-13 02:54:10.000000 wwpdb.utils.dp-0.47/wwpdb/utils/dp/RcsbDpUtility.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    17219 2023-06-13 02:54:10.000000 wwpdb.utils.dp-0.47/wwpdb/utils/dp/RunRemote.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4429 2023-06-13 02:54:10.000000 wwpdb.utils.dp-0.47/wwpdb/utils/dp/ValidationWrapper.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      154 2023-06-13 02:54:10.000000 wwpdb.utils.dp-0.47/wwpdb/utils/dp/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:55:11.806033 wwpdb.utils.dp-0.47/wwpdb/utils/dp/electron_density/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 02:54:10.000000 wwpdb.utils.dp-0.47/wwpdb/utils/dp/electron_density/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3930 2023-06-13 02:54:10.000000 wwpdb.utils.dp-0.47/wwpdb/utils/dp/electron_density/common_functions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3801 2023-06-13 02:54:10.000000 wwpdb.utils.dp-0.47/wwpdb/utils/dp/electron_density/em_density_map.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    10279 2023-06-13 02:54:10.000000 wwpdb.utils.dp-0.47/wwpdb/utils/dp/electron_density/x_ray_density_map.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:55:11.798034 wwpdb.utils.dp-0.47/wwpdb.utils.dp.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)      755 2023-06-13 02:55:11.000000 wwpdb.utils.dp-0.47/wwpdb.utils.dp.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      934 2023-06-13 02:55:11.000000 wwpdb.utils.dp-0.47/wwpdb.utils.dp.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-13 02:55:11.000000 wwpdb.utils.dp-0.47/wwpdb.utils.dp.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-13 02:54:58.000000 wwpdb.utils.dp-0.47/wwpdb.utils.dp.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)      103 2023-06-13 02:55:11.000000 wwpdb.utils.dp-0.47/wwpdb.utils.dp.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        6 2023-06-13 02:55:11.000000 wwpdb.utils.dp-0.47/wwpdb.utils.dp.egg-info/top_level.txt
```

### Comparing `wwpdb.utils.dp-0.46/LICENSE` & `wwpdb.utils.dp-0.47/LICENSE`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.dp-0.46/PKG-INFO` & `wwpdb.utils.dp-0.47/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.utils.dp
-Version: 0.46
+Version: 0.47
 Summary: API for Common Data Processing Operations
 Home-page: https://github.com/wwpdb/py-wwpdb_utils_dp
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.utils.dp-0.46/setup.py` & `wwpdb.utils.dp-0.47/setup.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.dp-0.46/wwpdb/utils/dp/CentreOfMass.py` & `wwpdb.utils.dp-0.47/wwpdb/utils/dp/CentreOfMass.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.dp-0.46/wwpdb/utils/dp/DataFileAdapter.py` & `wwpdb.utils.dp-0.47/wwpdb/utils/dp/DataFileAdapter.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.dp-0.46/wwpdb/utils/dp/DensityWrapper.py` & `wwpdb.utils.dp-0.47/wwpdb/utils/dp/DensityWrapper.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.dp-0.46/wwpdb/utils/dp/DepositorSyncUtil.py` & `wwpdb.utils.dp-0.47/wwpdb/utils/dp/DepositorSyncUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.dp-0.46/wwpdb/utils/dp/PdbxChemShiftReport.py` & `wwpdb.utils.dp-0.47/wwpdb/utils/dp/PdbxChemShiftReport.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.dp-0.46/wwpdb/utils/dp/PdbxMergeCategory.py` & `wwpdb.utils.dp-0.47/wwpdb/utils/dp/PdbxMergeCategory.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.dp-0.46/wwpdb/utils/dp/PdbxSFMapCoefficients.py` & `wwpdb.utils.dp-0.47/wwpdb/utils/dp/PdbxSFMapCoefficients.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.dp-0.46/wwpdb/utils/dp/PdbxStripCategory.py` & `wwpdb.utils.dp-0.47/wwpdb/utils/dp/PdbxStripCategory.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.dp-0.46/wwpdb/utils/dp/RcsbDpUtility.py` & `wwpdb.utils.dp-0.47/wwpdb/utils/dp/RcsbDpUtility.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,14 +121,15 @@
 # 19-Mar-2020 zf  Add "annot-get-pdb-file", "annot-check-pdb-file", "annot-check-sf-file", "annot-check-mr-file", "annot-check-cs-file"
 # 20-Mar-2020 zf  Add "annot-add-version-info", "annot-release-update"
 # 17-Jun-2020 zf  Add "PDB2GLYCAN" environmental variable for pdb2glycan software setting
 # 17-Jun-2020 zf  Add "carbohydrate-remediation", "carbohydrate-remediation-test"
 # 30-Jun-2020 zf  Add image tar file output after svg file for "annot-wwpdb-validate-all" & "annot-wwpdb-validate-all-v2"
 # 08-Jul-2020 zf  Add "get-branch-polymer-info"
 # 28-Sep-2020 zf  Add "annot-get-close-contact" & "annot-convert-close-contact-to-link"
+# 26-May-2023 zf  Add "annot-public-pdbx-to-xml-noatom"
 ##
 """
 Wrapper class for data processing and chemical component utilities.
 
 Initial RCSB version - adapted from file utils method collections.
 
 
@@ -327,14 +328,15 @@
             "annot-depict-chemical-shift",
             "annot-edit-chemical-shift",
             "annot-misc-checking",
             "annot-dcc-validation",
             "annot-correct-freer-set",
             "annot-cif-to-public-pdbx",
             "annot-public-pdbx-to-xml",
+            "annot-public-pdbx-to-xml-noatom",
             "annot-release-update",
             "annot-get-pdb-bundle",
             "annot-get-biol-cif-file",
             "annot-get-biol-pdb-file",
             "annot-check-cif",
             "annot-check-xml-xmllint",
             "annot-check-xml-stdinparse",
@@ -2200,14 +2202,21 @@
         elif op == "annot-public-pdbx-to-xml":
             #
             cmdPath = os.path.join(self.__packagePath, "dict", "bin", "mmcif2XML")
             thisCmd = " ; " + cmdPath + " -prefix  pdbx-v50 -ns PDBx -funct mmcif2xmlall -dictName mmcif_pdbx.dic -df " + self.__nameToDictPath("archive_current", suffix=".odb")
             cmd += thisCmd + " -f " + iPath
             cmd += " 2> " + tPath + " 1> " + lPath
 
+        elif op == "annot-public-pdbx-to-xml-noatom":
+            #
+            cmdPath = os.path.join(self.__packagePath, "dict", "bin", "mmcif2XML")
+            thisCmd = " ; " + cmdPath + " -prefix  pdbx-v50 -ns PDBx -funct mmcif2xmlnoatom -dictName mmcif_pdbx.dic -df " + self.__nameToDictPath("archive_current", suffix=".odb")
+            cmd += thisCmd + " -f " + iPath
+            cmd += " 2> " + tPath + " 1> " + lPath
+
         elif op == "annot-check-cif":
             #
             cmdPath = os.path.join(self.__packagePath, "dict", "bin", "CifCheck")
             thisCmd = " ; " + cmdPath + " -dictSdb " + self.__nameToDictPath("archive_current") + " -f " + iPath
             if "first_block" in self.__inputParamDict:
                 cmd += " -checkFirstBlock"
 
@@ -2817,14 +2826,24 @@
                 outFile = os.path.join(self.__wrkPath, fileName)
                 if os.access(outFile, os.F_OK):
                     self.__resultPathList.append(outFile)
                 else:
                     self.__resultPathList.append("missing")
                 #
             #
+
+        elif op == "annot-public-pdbx-to-xml-noatom":
+            for fileName in (iPath + ".xml-noatom", lPath, tPath):
+                outFile = os.path.join(self.__wrkPath, fileName)
+                if os.access(outFile, os.F_OK):
+                    self.__resultPathList.append(outFile)
+                else:
+                    self.__resultPathList.append("missing")
+                #
+            #
 
         elif op == "annot-check-cif":
             for fileName in (iPath + "-diag.log", lPath):
                 outFile = os.path.join(self.__wrkPath, fileName)
                 if os.access(outFile, os.F_OK):
                     self.__resultPathList.append(outFile)
                 else:
```

### Comparing `wwpdb.utils.dp-0.46/wwpdb/utils/dp/RunRemote.py` & `wwpdb.utils.dp-0.47/wwpdb/utils/dp/RunRemote.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.dp-0.46/wwpdb/utils/dp/ValidationWrapper.py` & `wwpdb.utils.dp-0.47/wwpdb/utils/dp/ValidationWrapper.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.dp-0.46/wwpdb/utils/dp/electron_density/common_functions.py` & `wwpdb.utils.dp-0.47/wwpdb/utils/dp/electron_density/common_functions.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.dp-0.46/wwpdb/utils/dp/electron_density/em_density_map.py` & `wwpdb.utils.dp-0.47/wwpdb/utils/dp/electron_density/em_density_map.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.dp-0.46/wwpdb/utils/dp/electron_density/x_ray_density_map.py` & `wwpdb.utils.dp-0.47/wwpdb/utils/dp/electron_density/x_ray_density_map.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.dp-0.46/wwpdb.utils.dp.egg-info/PKG-INFO` & `wwpdb.utils.dp-0.47/wwpdb.utils.dp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.utils.dp
-Version: 0.46
+Version: 0.47
 Summary: API for Common Data Processing Operations
 Home-page: https://github.com/wwpdb/py-wwpdb_utils_dp
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.utils.dp-0.46/wwpdb.utils.dp.egg-info/SOURCES.txt` & `wwpdb.utils.dp-0.47/wwpdb.utils.dp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

