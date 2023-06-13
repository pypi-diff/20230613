# Comparing `tmp/rcsb.workflow-0.40.tar.gz` & `tmp/rcsb.workflow-0.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcsb.workflow-0.40.tar", last modified: Mon Jun  5 14:55:07 2023, max compression
+gzip compressed data, was "rcsb.workflow-0.41.tar", last modified: Tue Jun 13 21:43:04 2023, max compression
```

## Comparing `rcsb.workflow-0.40.tar` & `rcsb.workflow-0.41.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:55:07.709616 rcsb.workflow-0.40/
--rw-r--r--   0 vsts      (1001) docker     (122)     2425 2023-06-05 14:02:56.000000 rcsb.workflow-0.40/HISTORY.txt
--rw-r--r--   0 vsts      (1001) docker     (122)    11357 2023-06-05 14:02:56.000000 rcsb.workflow-0.40/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)      106 2023-06-05 14:02:56.000000 rcsb.workflow-0.40/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)     1839 2023-06-05 14:55:07.709616 rcsb.workflow-0.40/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     1143 2023-06-05 14:02:56.000000 rcsb.workflow-0.40/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:55:07.705616 rcsb.workflow-0.40/rcsb/
--rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-06-05 14:02:56.000000 rcsb.workflow-0.40/rcsb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:55:07.709616 rcsb.workflow-0.40/rcsb/workflow/
--rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-06-05 14:02:56.000000 rcsb.workflow-0.40/rcsb/workflow/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:55:07.709616 rcsb.workflow-0.40/rcsb/workflow/chem/
--rw-r--r--   0 vsts      (1001) docker     (122)     3781 2023-06-05 14:02:56.000000 rcsb.workflow-0.40/rcsb/workflow/chem/ChemCompFileWorkflow.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5191 2023-06-05 14:02:56.000000 rcsb.workflow-0.40/rcsb/workflow/chem/ChemCompImageWorkflow.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3928 2023-06-05 14:02:56.000000 rcsb.workflow-0.40/rcsb/workflow/chem/ChemCompSearchIndexWorkflow.py
--rw-r--r--   0 vsts      (1001) docker     (122)      144 2023-06-05 14:02:56.000000 rcsb.workflow-0.40/rcsb/workflow/chem/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:55:07.709616 rcsb.workflow-0.40/rcsb/workflow/targets/
--rw-r--r--   0 vsts      (1001) docker     (122)    10335 2023-06-05 14:02:56.000000 rcsb.workflow-0.40/rcsb/workflow/targets/ProteinTargetSequenceExecutionWorkflow.py
--rw-r--r--   0 vsts      (1001) docker     (122)    28750 2023-06-05 14:02:56.000000 rcsb.workflow-0.40/rcsb/workflow/targets/ProteinTargetSequenceWorkflow.py
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-05 14:02:56.000000 rcsb.workflow-0.40/rcsb/workflow/targets/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-05 14:55:07.709616 rcsb.workflow-0.40/rcsb.workflow.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)     1839 2023-06-05 14:55:07.000000 rcsb.workflow-0.40/rcsb.workflow.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)      661 2023-06-05 14:55:07.000000 rcsb.workflow-0.40/rcsb.workflow.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-06-05 14:55:07.000000 rcsb.workflow-0.40/rcsb.workflow.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-06-05 14:55:06.000000 rcsb.workflow-0.40/rcsb.workflow.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (122)      196 2023-06-05 14:55:07.000000 rcsb.workflow-0.40/rcsb.workflow.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        5 2023-06-05 14:55:07.000000 rcsb.workflow-0.40/rcsb.workflow.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      230 2023-06-05 14:02:56.000000 rcsb.workflow-0.40/requirements.txt
--rwxr-xr-x   0 vsts      (1001) docker     (122)      108 2023-06-05 14:55:07.709616 rcsb.workflow-0.40/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (122)     2447 2023-06-05 14:02:56.000000 rcsb.workflow-0.40/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-13 21:43:04.305581 rcsb.workflow-0.41/
+-rw-r--r--   0 vsts      (1001) docker     (122)     2498 2023-06-13 20:51:12.000000 rcsb.workflow-0.41/HISTORY.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)    11357 2023-06-13 20:51:12.000000 rcsb.workflow-0.41/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)      106 2023-06-13 20:51:12.000000 rcsb.workflow-0.41/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)     1839 2023-06-13 21:43:04.305581 rcsb.workflow-0.41/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     1143 2023-06-13 20:51:12.000000 rcsb.workflow-0.41/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-13 21:43:04.301581 rcsb.workflow-0.41/rcsb/
+-rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-06-13 20:51:12.000000 rcsb.workflow-0.41/rcsb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-13 21:43:04.301581 rcsb.workflow-0.41/rcsb/workflow/
+-rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-06-13 20:51:12.000000 rcsb.workflow-0.41/rcsb/workflow/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-13 21:43:04.301581 rcsb.workflow-0.41/rcsb/workflow/chem/
+-rw-r--r--   0 vsts      (1001) docker     (122)     3781 2023-06-13 20:51:12.000000 rcsb.workflow-0.41/rcsb/workflow/chem/ChemCompFileWorkflow.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5191 2023-06-13 20:51:12.000000 rcsb.workflow-0.41/rcsb/workflow/chem/ChemCompImageWorkflow.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3928 2023-06-13 20:51:12.000000 rcsb.workflow-0.41/rcsb/workflow/chem/ChemCompSearchIndexWorkflow.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      144 2023-06-13 20:51:12.000000 rcsb.workflow-0.41/rcsb/workflow/chem/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-13 21:43:04.305581 rcsb.workflow-0.41/rcsb/workflow/targets/
+-rw-r--r--   0 vsts      (1001) docker     (122)    10408 2023-06-13 20:51:12.000000 rcsb.workflow-0.41/rcsb/workflow/targets/ProteinTargetSequenceExecutionWorkflow.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    28823 2023-06-13 20:51:12.000000 rcsb.workflow-0.41/rcsb/workflow/targets/ProteinTargetSequenceWorkflow.py
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-13 20:51:12.000000 rcsb.workflow-0.41/rcsb/workflow/targets/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-13 21:43:04.301581 rcsb.workflow-0.41/rcsb.workflow.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1839 2023-06-13 21:43:04.000000 rcsb.workflow-0.41/rcsb.workflow.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)      661 2023-06-13 21:43:04.000000 rcsb.workflow-0.41/rcsb.workflow.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-06-13 21:43:04.000000 rcsb.workflow-0.41/rcsb.workflow.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-06-13 21:43:02.000000 rcsb.workflow-0.41/rcsb.workflow.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (122)      196 2023-06-13 21:43:04.000000 rcsb.workflow-0.41/rcsb.workflow.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        5 2023-06-13 21:43:04.000000 rcsb.workflow-0.41/rcsb.workflow.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      230 2023-06-13 20:51:12.000000 rcsb.workflow-0.41/requirements.txt
+-rwxr-xr-x   0 vsts      (1001) docker     (122)      108 2023-06-13 21:43:04.305581 rcsb.workflow-0.41/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     2447 2023-06-13 20:51:12.000000 rcsb.workflow-0.41/setup.py
```

### Comparing `rcsb.workflow-0.40/HISTORY.txt` & `rcsb.workflow-0.41/HISTORY.txt`

 * *Files 3% similar despite different names*

```diff
@@ -26,7 +26,8 @@
  9-Jan-2023 - V0.34 Configuration changes to support tox 4
  3-Mar-2023 - V0.35 Standardize args in ProteinTargetSequenceExecutionWorkflow
 14-Mar-2023 - V0.36 Generate CARD annotations instead of features during ProteinTargetSequenceExecutionWorkflow
 21-Mar-2023 - V0.37 Allow backing up Pharos-targets to stash
  5-May-2023 - V0.38 Add fromDbPharos and reloadPharos parameters to ProteinTargetSequenceExecutionWorkflow.exportFasta()
 22-May-2023 - V0.39 Add retries to tox task for MMseqs2 download
  1-Jun-2023 - V0.40 Don't back up resources to GitHub during cache update workflows
+12-Jun-2023 - V0.41 Set useTaxonomy filter to False for CARD annotations
```

### Comparing `rcsb.workflow-0.40/LICENSE` & `rcsb.workflow-0.41/LICENSE`

 * *Files identical despite different names*

### Comparing `rcsb.workflow-0.40/PKG-INFO` & `rcsb.workflow-0.41/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.workflow
-Version: 0.40
+Version: 0.41
 Summary: RCSB Python data processing and ETL/ELT workflow entry points
 Home-page: https://github.com/rcsb/py-rcsb_workflow
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rcsb.workflow-0.40/README.md` & `rcsb.workflow-0.41/README.md`

 * *Files identical despite different names*

### Comparing `rcsb.workflow-0.40/rcsb/workflow/chem/ChemCompFileWorkflow.py` & `rcsb.workflow-0.41/rcsb/workflow/chem/ChemCompFileWorkflow.py`

 * *Files identical despite different names*

### Comparing `rcsb.workflow-0.40/rcsb/workflow/chem/ChemCompImageWorkflow.py` & `rcsb.workflow-0.41/rcsb/workflow/chem/ChemCompImageWorkflow.py`

 * *Files identical despite different names*

### Comparing `rcsb.workflow-0.40/rcsb/workflow/chem/ChemCompSearchIndexWorkflow.py` & `rcsb.workflow-0.41/rcsb/workflow/chem/ChemCompSearchIndexWorkflow.py`

 * *Files identical despite different names*

### Comparing `rcsb.workflow-0.40/rcsb/workflow/targets/ProteinTargetSequenceExecutionWorkflow.py` & `rcsb.workflow-0.41/rcsb/workflow/targets/ProteinTargetSequenceExecutionWorkflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # Author:  J. Westbrook
 # Date:    25-Jun-2021
 #
 # Updates:
 #   3-Mar-2023 Standard args passed into workflow
 #  21-Mar-2023 Allow backing up Pharos-targets to stash, more __init__ improvement
 #   5-May-2023 Pass in fromDbPharos and reloadPharos parameters to exportFasta()
+#  12-Jun-2023 dwp Set useTaxonomy filter to False for CARD annotations
 ##
 """
 Execution workflow for protein target data ETL operations.
 """
 __docformat__ = "google en"
 __author__ = "John Westbrook"
 __email__ = "jwest@rcsb.rutgers.edu"
@@ -184,15 +185,15 @@
         logger.info("Running buildFeatures...")
         ok = False
         try:
             ptsW = ProteinTargetSequenceWorkflow(self.__cfgOb, self.__cachePath)
             ok = ptsW.buildFeatureData(
                 referenceResourceName="pdbprent",
                 resourceNameList=["sabdab", "card", "imgt"],
-                useTaxonomy=True,
+                useTaxonomy=False,
                 backup=True,
                 remotePrefix=self.__stashRemotePrefix
             )
         except Exception as e:
             logger.exception("Failing with %s", str(e))
         return ok
```

### Comparing `rcsb.workflow-0.40/rcsb/workflow/targets/ProteinTargetSequenceWorkflow.py` & `rcsb.workflow-0.41/rcsb/workflow/targets/ProteinTargetSequenceWorkflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 #  25-Jul-2021 add new StashableBase options for git backup
 #  29-Jul-2021 DrugBankProvider needs useCache=False to always rebuild
 #   3-Mar-2023 Fix error for missing taxonPath
 #  14-Mar-2023 Generate CARD annotations instead of CARD features
 #  21-Mar-2023 Allow backing up Pharos-targets to stash
 #   5-May-2023 Restore from stash if fromDbPharos and reloadPharos parameters are False
 #   1-Jun-2023 aae Don't back up resources to GitHub during cache update workflows
+#  12-Jun-2023 dwp Set useTaxonomy filter to False for CARD annotations
 ##
 __docformat__ = "google en"
 __author__ = "John Westbrook"
 __email__ = "jwest@rcsb.rutgers.edu"
 __license__ = "Apache 2.0"
 
 import logging
@@ -327,15 +328,15 @@
                 time.strftime("%Y %m %d %H:%M:%S", time.localtime()),
                 time.time() - startTime,
             )
             retOk = retOk and ok
         #
         return retOk
 
-    def __buildFeatureData(self, referenceResourceName, resourceName, useTaxonomy=True, backup=False, remotePrefix=None):
+    def __buildFeatureData(self, referenceResourceName, resourceName, useTaxonomy=False, backup=False, remotePrefix=None):
         """Build features and annotations inferred from sequence comparison results between the input resources."""
         try:
             okB = True
             resultPath = self.__getFilteredSearchResultPath(resourceName, referenceResourceName)
             #
             if resourceName == "sabdab":
                 fP = SAbDabTargetFeatureProvider(cachePath=self.__cachePath, useCache=True)
```

### Comparing `rcsb.workflow-0.40/rcsb.workflow.egg-info/PKG-INFO` & `rcsb.workflow-0.41/rcsb.workflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.workflow
-Version: 0.40
+Version: 0.41
 Summary: RCSB Python data processing and ETL/ELT workflow entry points
 Home-page: https://github.com/rcsb/py-rcsb_workflow
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rcsb.workflow-0.40/rcsb.workflow.egg-info/SOURCES.txt` & `rcsb.workflow-0.41/rcsb.workflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rcsb.workflow-0.40/setup.py` & `rcsb.workflow-0.41/setup.py`

 * *Files identical despite different names*

