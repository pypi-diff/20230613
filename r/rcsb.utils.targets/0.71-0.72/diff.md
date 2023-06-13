# Comparing `tmp/rcsb.utils.targets-0.71.tar.gz` & `tmp/rcsb.utils.targets-0.72.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcsb.utils.targets-0.71.tar", last modified: Tue May 23 16:25:31 2023, max compression
+gzip compressed data, was "rcsb.utils.targets-0.72.tar", last modified: Tue Jun 13 13:17:42 2023, max compression
```

## Comparing `rcsb.utils.targets-0.71.tar` & `rcsb.utils.targets-0.72.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-23 16:25:31.408550 rcsb.utils.targets-0.71/
--rw-r--r--   0 vsts      (1001) docker     (122)     6044 2023-05-23 16:10:56.000000 rcsb.utils.targets-0.71/HISTORY.txt
--rw-r--r--   0 vsts      (1001) docker     (122)    11357 2023-05-23 16:10:56.000000 rcsb.utils.targets-0.71/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)      111 2023-05-23 16:10:56.000000 rcsb.utils.targets-0.71/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)     1645 2023-05-23 16:25:31.408550 rcsb.utils.targets-0.71/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)      953 2023-05-23 16:10:56.000000 rcsb.utils.targets-0.71/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-23 16:25:31.400550 rcsb.utils.targets-0.71/rcsb/
--rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-05-23 16:10:56.000000 rcsb.utils.targets-0.71/rcsb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-23 16:25:31.404550 rcsb.utils.targets-0.71/rcsb/utils/
--rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-05-23 16:10:56.000000 rcsb.utils.targets-0.71/rcsb/utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-23 16:25:31.408550 rcsb.utils.targets-0.71/rcsb/utils/targets/
--rw-r--r--   0 vsts      (1001) docker     (122)     9301 2023-05-23 16:10:56.000000 rcsb.utils.targets-0.71/rcsb/utils/targets/CARDTargetAnnotationProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7017 2023-05-23 16:10:56.000000 rcsb.utils.targets-0.71/rcsb/utils/targets/CARDTargetFeatureProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8021 2023-05-23 16:10:56.000000 rcsb.utils.targets-0.71/rcsb/utils/targets/CARDTargetOntologyProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10102 2023-05-23 16:10:56.000000 rcsb.utils.targets-0.71/rcsb/utils/targets/CARDTargetProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    19228 2023-05-23 16:10:56.000000 rcsb.utils.targets-0.71/rcsb/utils/targets/ChEMBLTargetActivityProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    13181 2023-05-23 16:10:56.000000 rcsb.utils.targets-0.71/rcsb/utils/targets/ChEMBLTargetCofactorProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5330 2023-05-23 16:10:56.000000 rcsb.utils.targets-0.71/rcsb/utils/targets/ChEMBLTargetMechanismProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8904 2023-05-23 16:10:56.000000 rcsb.utils.targets-0.71/rcsb/utils/targets/ChEMBLTargetProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9171 2023-05-23 16:10:56.000000 rcsb.utils.targets-0.71/rcsb/utils/targets/DrugBankTargetCofactorProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    12661 2023-05-23 16:10:56.000000 rcsb.utils.targets-0.71/rcsb/utils/targets/DrugBankTargetProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9505 2023-05-23 16:10:56.000000 rcsb.utils.targets-0.71/rcsb/utils/targets/IMGTTargetFeatureProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    20738 2023-05-23 16:10:56.000000 rcsb.utils.targets-0.71/rcsb/utils/targets/IMGTTargetProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10451 2023-05-23 16:10:56.000000 rcsb.utils.targets-0.71/rcsb/utils/targets/PharosTargetActivityProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    12770 2023-05-23 16:10:56.000000 rcsb.utils.targets-0.71/rcsb/utils/targets/PharosTargetCofactorProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9154 2023-05-23 16:10:56.000000 rcsb.utils.targets-0.71/rcsb/utils/targets/PharosTargetProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8898 2023-05-23 16:10:56.000000 rcsb.utils.targets-0.71/rcsb/utils/targets/SAbDabTargetFeatureProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9689 2023-05-23 16:10:56.000000 rcsb.utils.targets-0.71/rcsb/utils/targets/SAbDabTargetProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)      144 2023-05-23 16:10:56.000000 rcsb.utils.targets-0.71/rcsb/utils/targets/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-23 16:25:31.404550 rcsb.utils.targets-0.71/rcsb.utils.targets.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)     1645 2023-05-23 16:25:31.000000 rcsb.utils.targets-0.71/rcsb.utils.targets.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     1209 2023-05-23 16:25:31.000000 rcsb.utils.targets-0.71/rcsb.utils.targets.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-23 16:25:31.000000 rcsb.utils.targets-0.71/rcsb.utils.targets.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-23 16:12:21.000000 rcsb.utils.targets-0.71/rcsb.utils.targets.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (122)      216 2023-05-23 16:25:31.000000 rcsb.utils.targets-0.71/rcsb.utils.targets.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        5 2023-05-23 16:25:31.000000 rcsb.utils.targets-0.71/rcsb.utils.targets.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      190 2023-05-23 16:10:56.000000 rcsb.utils.targets-0.71/requirements.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      108 2023-05-23 16:25:31.408550 rcsb.utils.targets-0.71/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (122)     2273 2023-05-23 16:10:56.000000 rcsb.utils.targets-0.71/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-13 13:17:42.637845 rcsb.utils.targets-0.72/
+-rw-r--r--   0 vsts      (1001) docker     (122)     6083 2023-06-13 13:04:46.000000 rcsb.utils.targets-0.72/HISTORY.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)    11357 2023-06-13 13:04:46.000000 rcsb.utils.targets-0.72/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)      111 2023-06-13 13:04:46.000000 rcsb.utils.targets-0.72/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)     1645 2023-06-13 13:17:42.637845 rcsb.utils.targets-0.72/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)      953 2023-06-13 13:04:46.000000 rcsb.utils.targets-0.72/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-13 13:17:42.637845 rcsb.utils.targets-0.72/rcsb/
+-rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-06-13 13:04:46.000000 rcsb.utils.targets-0.72/rcsb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-13 13:17:42.637845 rcsb.utils.targets-0.72/rcsb/utils/
+-rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-06-13 13:04:46.000000 rcsb.utils.targets-0.72/rcsb/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-13 13:17:42.637845 rcsb.utils.targets-0.72/rcsb/utils/targets/
+-rw-r--r--   0 vsts      (1001) docker     (122)     9534 2023-06-13 13:04:46.000000 rcsb.utils.targets-0.72/rcsb/utils/targets/CARDTargetAnnotationProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7017 2023-06-13 13:04:46.000000 rcsb.utils.targets-0.72/rcsb/utils/targets/CARDTargetFeatureProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8021 2023-06-13 13:04:46.000000 rcsb.utils.targets-0.72/rcsb/utils/targets/CARDTargetOntologyProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10102 2023-06-13 13:04:46.000000 rcsb.utils.targets-0.72/rcsb/utils/targets/CARDTargetProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    19228 2023-06-13 13:04:46.000000 rcsb.utils.targets-0.72/rcsb/utils/targets/ChEMBLTargetActivityProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    13181 2023-06-13 13:04:46.000000 rcsb.utils.targets-0.72/rcsb/utils/targets/ChEMBLTargetCofactorProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5330 2023-06-13 13:04:46.000000 rcsb.utils.targets-0.72/rcsb/utils/targets/ChEMBLTargetMechanismProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8904 2023-06-13 13:04:46.000000 rcsb.utils.targets-0.72/rcsb/utils/targets/ChEMBLTargetProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9171 2023-06-13 13:04:46.000000 rcsb.utils.targets-0.72/rcsb/utils/targets/DrugBankTargetCofactorProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    12661 2023-06-13 13:04:46.000000 rcsb.utils.targets-0.72/rcsb/utils/targets/DrugBankTargetProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9505 2023-06-13 13:04:46.000000 rcsb.utils.targets-0.72/rcsb/utils/targets/IMGTTargetFeatureProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    20738 2023-06-13 13:04:46.000000 rcsb.utils.targets-0.72/rcsb/utils/targets/IMGTTargetProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10451 2023-06-13 13:04:46.000000 rcsb.utils.targets-0.72/rcsb/utils/targets/PharosTargetActivityProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    12770 2023-06-13 13:04:46.000000 rcsb.utils.targets-0.72/rcsb/utils/targets/PharosTargetCofactorProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9154 2023-06-13 13:04:46.000000 rcsb.utils.targets-0.72/rcsb/utils/targets/PharosTargetProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8898 2023-06-13 13:04:46.000000 rcsb.utils.targets-0.72/rcsb/utils/targets/SAbDabTargetFeatureProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9689 2023-06-13 13:04:46.000000 rcsb.utils.targets-0.72/rcsb/utils/targets/SAbDabTargetProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      144 2023-06-13 13:04:46.000000 rcsb.utils.targets-0.72/rcsb/utils/targets/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-13 13:17:42.637845 rcsb.utils.targets-0.72/rcsb.utils.targets.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1645 2023-06-13 13:17:42.000000 rcsb.utils.targets-0.72/rcsb.utils.targets.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     1209 2023-06-13 13:17:42.000000 rcsb.utils.targets-0.72/rcsb.utils.targets.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-06-13 13:17:42.000000 rcsb.utils.targets-0.72/rcsb.utils.targets.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-06-13 13:05:54.000000 rcsb.utils.targets-0.72/rcsb.utils.targets.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (122)      216 2023-06-13 13:17:42.000000 rcsb.utils.targets-0.72/rcsb.utils.targets.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        5 2023-06-13 13:17:42.000000 rcsb.utils.targets-0.72/rcsb.utils.targets.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      190 2023-06-13 13:04:47.000000 rcsb.utils.targets-0.72/requirements.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      108 2023-06-13 13:17:42.641846 rcsb.utils.targets-0.72/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)     2273 2023-06-13 13:04:47.000000 rcsb.utils.targets-0.72/setup.py
```

### Comparing `rcsb.utils.targets-0.71/HISTORY.txt` & `rcsb.utils.targets-0.72/HISTORY.txt`

 * *Files 1% similar despite different names*

```diff
@@ -56,8 +56,9 @@
   13-Mar-2023  - V0.64 Add CARDTargetAnnotationProvider (to replace CARDTargetFeatureProvider)
   22-Mar-2023  - V0.65 Add timeout to IMGT data file fetch, and update py-rcsb_exdb_assets locators
   24-Mar-2023  - V0.66 In PharosTargetProvider(), download sql file to separate dir
   11-Apr-2023  - V0.67 Fix issue with CARD lineage tree building--handle cases with two parents at same depth; Add treeNodeList building and exporting
   27-Apr-2023  - V0.68 Update CARD treeNodeList building
    2-May-2023  - V0.69 Remove depth field from CARD lineage tree
    5-May-2023  - V0.70 Actually check cache files exist in PharosTargetProvider testCache()
-  22-May-2023  - V0.71 Add retries to tox task for MMseqs2 download
+  22-May-2023  - V0.71 Add retries to tox task for MMseqs2 download
+  13-Jun-2023  - V0.72 Improve logging
```

### Comparing `rcsb.utils.targets-0.71/LICENSE` & `rcsb.utils.targets-0.72/LICENSE`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.71/PKG-INFO` & `rcsb.utils.targets-0.72/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.utils.targets
-Version: 0.71
+Version: 0.72
 Summary: RCSB Python Wrapper Module for Target Utilities
 Home-page: https://github.com/rcsb/py-rcsb_utils_targets
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rcsb.utils.targets-0.71/README.md` & `rcsb.utils.targets-0.72/README.md`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.71/rcsb/utils/targets/CARDTargetAnnotationProvider.py` & `rcsb.utils.targets-0.72/rcsb/utils/targets/CARDTargetAnnotationProvider.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,15 @@
         return fD
 
     def buildAnnotationList(self, sequenceMatchFilePath, useTaxonomy=False):
         """Build polymer entity annotation list for the matching entities in the input sequence match file.
 
         Args:
             sequenceMatchFilePath (str): sequence match output file path
-            useTaxonomy (bool): apply taxonomy criteria to filter matches. Defaults to False
+            useTaxonomy (bool): apply taxonomy criteria to filter matches (only include matches that have a defined taxonomyMatchStatus). Defaults to False
 
         Returns:
             bool: True for success or False otherwise
         """
         rDL = []
         cardP = CARDTargetProvider(cachePath=self.__cachePath, useCache=False)
         ontologyP = CARDTargetOntologyProvider(cachePath=self.__cachePath, useCache=False)
@@ -172,15 +172,15 @@
                         mL.append(rD)
                     elif rD["match_status"] == "orthologous match (by lca)":
                         oL.append(rD)
                     else:
                         continue
                 if not mL and not oL:
                     continue
-                logger.debug("eId %r mL (%d) oL (%d)", eId, len(mL), len(oL))
+                logger.info("eId %r mL (%d) oL (%d)", eId, len(mL), len(oL))
                 fqD.setdefault(eId, []).extend(mL if mL else oL)
         else:
             fqD = qD
         # --
         # Determine whether entities demonstrate a perfect match or match multiple CARD annotations
         cqD = {}
         for eId, rDL in fqD.items():
@@ -199,14 +199,15 @@
                     rD["perfect_match"] = "N"
                 cqD[eId] = rD
         # --
         fp = self.__getAnnotationDataPath()
         tS = datetime.datetime.now().isoformat()
         vS = datetime.datetime.now().strftime("%Y-%m-%d")
         ok = self.__mU.doExport(fp, {"version": vS, "created": tS, "taxonomyFilter": useTaxonomy, "annotations": cqD}, fmt="json", indent=3)
+        logger.info("Done rebuilding CARD annotation features (status %r) version (%r) created (%r) useTaxonomy (%r) annotations (%d)", ok, vS, tS, useTaxonomy, len(cqD))
         return ok
 
     def __decodeComment(self, comment, separator="|"):
         dD = {}
         try:
             ti = iter(comment.split(separator))
             dD = {tup[1]: tup[0] for tup in zip(ti, ti)}
```

### Comparing `rcsb.utils.targets-0.71/rcsb/utils/targets/CARDTargetFeatureProvider.py` & `rcsb.utils.targets-0.72/rcsb/utils/targets/CARDTargetFeatureProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.71/rcsb/utils/targets/CARDTargetOntologyProvider.py` & `rcsb.utils.targets-0.72/rcsb/utils/targets/CARDTargetOntologyProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.71/rcsb/utils/targets/CARDTargetProvider.py` & `rcsb.utils.targets-0.72/rcsb/utils/targets/CARDTargetProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.71/rcsb/utils/targets/ChEMBLTargetActivityProvider.py` & `rcsb.utils.targets-0.72/rcsb/utils/targets/ChEMBLTargetActivityProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.71/rcsb/utils/targets/ChEMBLTargetCofactorProvider.py` & `rcsb.utils.targets-0.72/rcsb/utils/targets/ChEMBLTargetCofactorProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.71/rcsb/utils/targets/ChEMBLTargetMechanismProvider.py` & `rcsb.utils.targets-0.72/rcsb/utils/targets/ChEMBLTargetMechanismProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.71/rcsb/utils/targets/ChEMBLTargetProvider.py` & `rcsb.utils.targets-0.72/rcsb/utils/targets/ChEMBLTargetProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.71/rcsb/utils/targets/DrugBankTargetCofactorProvider.py` & `rcsb.utils.targets-0.72/rcsb/utils/targets/DrugBankTargetCofactorProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.71/rcsb/utils/targets/DrugBankTargetProvider.py` & `rcsb.utils.targets-0.72/rcsb/utils/targets/DrugBankTargetProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.71/rcsb/utils/targets/IMGTTargetFeatureProvider.py` & `rcsb.utils.targets-0.72/rcsb/utils/targets/IMGTTargetFeatureProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.71/rcsb/utils/targets/IMGTTargetProvider.py` & `rcsb.utils.targets-0.72/rcsb/utils/targets/IMGTTargetProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.71/rcsb/utils/targets/PharosTargetActivityProvider.py` & `rcsb.utils.targets-0.72/rcsb/utils/targets/PharosTargetActivityProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.71/rcsb/utils/targets/PharosTargetCofactorProvider.py` & `rcsb.utils.targets-0.72/rcsb/utils/targets/PharosTargetCofactorProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.71/rcsb/utils/targets/PharosTargetProvider.py` & `rcsb.utils.targets-0.72/rcsb/utils/targets/PharosTargetProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.71/rcsb/utils/targets/SAbDabTargetFeatureProvider.py` & `rcsb.utils.targets-0.72/rcsb/utils/targets/SAbDabTargetFeatureProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.71/rcsb/utils/targets/SAbDabTargetProvider.py` & `rcsb.utils.targets-0.72/rcsb/utils/targets/SAbDabTargetProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.71/rcsb.utils.targets.egg-info/PKG-INFO` & `rcsb.utils.targets-0.72/rcsb.utils.targets.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.utils.targets
-Version: 0.71
+Version: 0.72
 Summary: RCSB Python Wrapper Module for Target Utilities
 Home-page: https://github.com/rcsb/py-rcsb_utils_targets
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rcsb.utils.targets-0.71/rcsb.utils.targets.egg-info/SOURCES.txt` & `rcsb.utils.targets-0.72/rcsb.utils.targets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rcsb.utils.targets-0.71/setup.py` & `rcsb.utils.targets-0.72/setup.py`

 * *Files identical despite different names*

