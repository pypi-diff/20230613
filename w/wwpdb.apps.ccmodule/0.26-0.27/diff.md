# Comparing `tmp/wwpdb.apps.ccmodule-0.26.tar.gz` & `tmp/wwpdb.apps.ccmodule-0.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wwpdb.apps.ccmodule-0.26.tar", last modified: Sun May 14 15:43:08 2023, max compression
+gzip compressed data, was "wwpdb.apps.ccmodule-0.27.tar", last modified: Tue Jun 13 11:18:38 2023, max compression
```

## Comparing `wwpdb.apps.ccmodule-0.26.tar` & `wwpdb.apps.ccmodule-0.27.tar`

### file list

```diff
@@ -1,77 +1,73 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 15:43:08.202798 wwpdb.apps.ccmodule-0.26/
--rw-r--r--   0 vsts      (1001) docker     (123)      779 2023-05-14 15:43:08.202798 wwpdb.apps.ccmodule-0.26/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)       80 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/README.md
--rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-05-14 15:43:08.206798 wwpdb.apps.ccmodule-0.26/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (123)     2595 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 15:43:08.194798 wwpdb.apps.ccmodule-0.26/wwpdb/
--rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 15:43:08.194798 wwpdb.apps.ccmodule-0.26/wwpdb/apps/
--rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 15:43:08.194798 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/
--rw-r--r--   0 vsts      (1001) docker     (123)      151 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 15:43:08.198798 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/chem/
--rw-r--r--   0 vsts      (1001) docker     (123)     5950 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/chem/ChemCompAnnotate.py
--rw-r--r--   0 vsts      (1001) docker     (123)   121176 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/chem/ChemCompAssign.py
--rw-r--r--   0 vsts      (1001) docker     (123)   102562 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/chem/ChemCompAssignDepict.py
--rw-r--r--   0 vsts      (1001) docker     (123)    73835 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/chem/ChemCompAssignDepictLite.py
--rw-r--r--   0 vsts      (1001) docker     (123)    11689 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/chem/PdbxChemCompAssign.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/chem/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 15:43:08.198798 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/depict/
--rw-r--r--   0 vsts      (1001) docker     (123)    11302 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/depict/ChemCompDepict.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/depict/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 15:43:08.198798 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/edit/
--rw-r--r--   0 vsts      (1001) docker     (123)    14647 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/edit/ChemCompTableEditor.py
--rw-r--r--   0 vsts      (1001) docker     (123)    25954 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/edit/ChemCompTableEditorDepict.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/edit/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 15:43:08.198798 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/extract/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/extract/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2951 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/extract/ccOps.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 15:43:08.198798 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/io/
--rw-r--r--   0 vsts      (1001) docker     (123)    90790 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/io/ChemCompAssignDataStore.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7123 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/io/ChemCompDataExport.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7305 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/io/ChemCompDataImport.py
--rw-r--r--   0 vsts      (1001) docker     (123)    12540 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/io/ChemCompEditStore.py
--rw-r--r--   0 vsts      (1001) docker     (123)    13230 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/io/ChemCompIo.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/io/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 15:43:08.198798 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/reports/
--rw-r--r--   0 vsts      (1001) docker     (123)     4801 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/reports/ChemCompAlignImageGenerator.py
--rwxr-xr-x   0 vsts      (1001) docker     (123)     4885 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/reports/ChemCompAlignImages.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2842 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/reports/ChemCompBigAlignImages.py
--rwxr-xr-x   0 vsts      (1001) docker     (123)     3367 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/reports/ChemCompGenImage.py
--rw-r--r--   0 vsts      (1001) docker     (123)    15551 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/reports/ChemCompReports.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6341 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/reports/InstanceDataGenerator.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/reports/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 15:43:08.202798 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/search/
--rw-r--r--   0 vsts      (1001) docker     (123)    10865 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/search/ChemCompSearch.py
--rw-r--r--   0 vsts      (1001) docker     (123)    13150 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/search/ChemCompSearchDb.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6259 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/search/ChemCompSearchDbDepict.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8708 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/search/ChemCompSearchDepict.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2942 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/search/DbSession.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/search/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 15:43:08.202798 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/sketch/
--rw-r--r--   0 vsts      (1001) docker     (123)     9280 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/sketch/ChemCompSketch.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6407 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/sketch/ChemCompSketchDepict.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/sketch/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 15:43:08.202798 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/utils/
--rw-r--r--   0 vsts      (1001) docker     (123)     7373 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/utils/ChemCompConfig.py
--rw-r--r--   0 vsts      (1001) docker     (123)    28706 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/utils/ChemCompDpUtility.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1136 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/utils/ChemCompWFInterface.py
--rw-r--r--   0 vsts      (1001) docker     (123)      586 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/utils/Exceptions.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7974 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/utils/LigandAnalysisState.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 15:43:08.202798 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/view/
--rw-r--r--   0 vsts      (1001) docker     (123)     7378 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/view/ChemCompView.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5738 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/view/ChemCompViewDepict.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/view/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 15:43:08.202798 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/webapp/
--rw-r--r--   0 vsts      (1001) docker     (123)   138409 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/webapp/ChemCompWebApp.py
--rw-r--r--   0 vsts      (1001) docker     (123)    96877 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/webapp/ChemCompWebAppLite.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/webapp/__init__.py
--rwxr-xr-x   0 vsts      (1001) docker     (123)     4642 2023-05-14 15:42:12.000000 wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/webapp/wsgi.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 15:43:08.194798 wwpdb.apps.ccmodule-0.26/wwpdb.apps.ccmodule.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)      779 2023-05-14 15:43:08.000000 wwpdb.apps.ccmodule-0.26/wwpdb.apps.ccmodule.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     2509 2023-05-14 15:43:08.000000 wwpdb.apps.ccmodule-0.26/wwpdb.apps.ccmodule.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-14 15:43:08.000000 wwpdb.apps.ccmodule-0.26/wwpdb.apps.ccmodule.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-14 15:42:57.000000 wwpdb.apps.ccmodule-0.26/wwpdb.apps.ccmodule.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)      250 2023-05-14 15:43:08.000000 wwpdb.apps.ccmodule-0.26/wwpdb.apps.ccmodule.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        6 2023-05-14 15:43:08.000000 wwpdb.apps.ccmodule-0.26/wwpdb.apps.ccmodule.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 11:18:38.367896 wwpdb.apps.ccmodule-0.27/
+-rw-r--r--   0 vsts      (1001) docker     (123)      779 2023-06-13 11:18:38.367896 wwpdb.apps.ccmodule-0.27/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)       80 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/README.md
+-rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-06-13 11:18:38.367896 wwpdb.apps.ccmodule-0.27/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (123)     2595 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 11:18:38.363896 wwpdb.apps.ccmodule-0.27/wwpdb/
+-rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 11:18:38.363896 wwpdb.apps.ccmodule-0.27/wwpdb/apps/
+-rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 11:18:38.363896 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/
+-rw-r--r--   0 vsts      (1001) docker     (123)      151 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 11:18:38.363896 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/chem/
+-rw-r--r--   0 vsts      (1001) docker     (123)     5950 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/chem/ChemCompAnnotate.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   121120 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/chem/ChemCompAssign.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   103161 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/chem/ChemCompAssignDepict.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    73659 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/chem/ChemCompAssignDepictLite.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    11689 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/chem/PdbxChemCompAssign.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/chem/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 11:18:38.363896 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/depict/
+-rw-r--r--   0 vsts      (1001) docker     (123)    11302 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/depict/ChemCompDepict.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/depict/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 11:18:38.363896 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/extract/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/extract/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2951 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/extract/ccOps.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 11:18:38.363896 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/io/
+-rw-r--r--   0 vsts      (1001) docker     (123)    90790 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/io/ChemCompAssignDataStore.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7123 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/io/ChemCompDataExport.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7305 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/io/ChemCompDataImport.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    12540 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/io/ChemCompEditStore.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    13230 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/io/ChemCompIo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/io/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 11:18:38.363896 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/reports/
+-rw-r--r--   0 vsts      (1001) docker     (123)     4801 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/reports/ChemCompAlignImageGenerator.py
+-rwxr-xr-x   0 vsts      (1001) docker     (123)     4885 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/reports/ChemCompAlignImages.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2842 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/reports/ChemCompBigAlignImages.py
+-rwxr-xr-x   0 vsts      (1001) docker     (123)     3367 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/reports/ChemCompGenImage.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    15516 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/reports/ChemCompReports.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6341 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/reports/InstanceDataGenerator.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/reports/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 11:18:38.367896 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/search/
+-rw-r--r--   0 vsts      (1001) docker     (123)    10865 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/search/ChemCompSearch.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    13150 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/search/ChemCompSearchDb.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6259 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/search/ChemCompSearchDbDepict.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8708 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/search/ChemCompSearchDepict.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2942 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/search/DbSession.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/search/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 11:18:38.367896 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/sketch/
+-rw-r--r--   0 vsts      (1001) docker     (123)     9350 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/sketch/ChemCompSketch.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6407 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/sketch/ChemCompSketchDepict.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/sketch/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 11:18:38.367896 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/utils/
+-rw-r--r--   0 vsts      (1001) docker     (123)     7201 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/utils/ChemCompConfig.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    28707 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/utils/ChemCompDpUtility.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1136 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/utils/ChemCompWFInterface.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      586 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/utils/Exceptions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7942 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/utils/LigandAnalysisState.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 11:18:38.367896 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/view/
+-rw-r--r--   0 vsts      (1001) docker     (123)     7378 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/view/ChemCompView.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5748 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/view/ChemCompViewDepict.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/view/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 11:18:38.367896 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/webapp/
+-rw-r--r--   0 vsts      (1001) docker     (123)   138698 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/webapp/ChemCompWebApp.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    96593 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/webapp/ChemCompWebAppLite.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/webapp/__init__.py
+-rwxr-xr-x   0 vsts      (1001) docker     (123)     4642 2023-06-13 11:17:32.000000 wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/webapp/wsgi.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 11:18:38.363896 wwpdb.apps.ccmodule-0.27/wwpdb.apps.ccmodule.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)      779 2023-06-13 11:18:38.000000 wwpdb.apps.ccmodule-0.27/wwpdb.apps.ccmodule.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     2370 2023-06-13 11:18:38.000000 wwpdb.apps.ccmodule-0.27/wwpdb.apps.ccmodule.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-13 11:18:38.000000 wwpdb.apps.ccmodule-0.27/wwpdb.apps.ccmodule.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-13 11:18:26.000000 wwpdb.apps.ccmodule-0.27/wwpdb.apps.ccmodule.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)      250 2023-06-13 11:18:38.000000 wwpdb.apps.ccmodule-0.27/wwpdb.apps.ccmodule.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        6 2023-06-13 11:18:38.000000 wwpdb.apps.ccmodule-0.27/wwpdb.apps.ccmodule.egg-info/top_level.txt
```

### Comparing `wwpdb.apps.ccmodule-0.26/PKG-INFO` & `wwpdb.apps.ccmodule-0.27/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.apps.ccmodule
-Version: 0.26
+Version: 0.27
 Summary: wwPDB workflow engine utils
 Home-page: https://github.com/rcsb/py-wwpdb_apps_wf_engine_utils
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.apps.ccmodule-0.26/setup.py` & `wwpdb.apps.ccmodule-0.27/setup.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/chem/ChemCompAnnotate.py` & `wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/chem/ChemCompAnnotate.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/chem/ChemCompAssign.py` & `wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/chem/ChemCompAssign.py`

 * *Files 0% similar despite different names*

```diff
@@ -162,17 +162,17 @@
             self.__modelDirPath = self.__sessionPath
             self.__ccReportPath = os.path.join(self.__sessionPath, 'assign')
         elif context == 'workflow' or context == 'unknown':
             self.__modelDirPath = self.__sessionPath
             self.__ccReportPath = os.path.join(self.__sessionPath, 'assign')
         elif context == 'deposition':
             self.__depId = self.__reqObj.getValue('identifier')
-            self.__depositPath = Path(PathInfo().getDepositPath(self.__depId)).parent
-            self.__modelDirPath = os.path.join(self.__depositPath, self.__depId)
-            self.__ccReportPath = os.path.join(self.__depositPath, self.__depId, self._CC_REPORT_DIR)
+            depositPath = Path(PathInfo().getDepositPath(self.__depId))
+            self.__modelDirPath = os.path.join(depositPath)
+            self.__ccReportPath = os.path.join(depositPath, self._CC_REPORT_DIR)
 
         self.normal = ['ALA', 'CYS', 'ASP', 'GLU', 'PHE', 'GLY', 'HIS', 'ILE',
                        'LYS', 'LEU', 'MET', 'ASN', 'PRO', 'GLN', 'ARG', 'SER',
                        'THR', 'VAL', 'TRP', 'TYR', 'C', 'G', 'T', 'A', 'U',
                        'DC', 'DA', 'DU', 'DT', 'DG',
                        'HOH', 'TIP', 'WAT', 'OH2', 'MSE']
         #
```

### Comparing `wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/chem/ChemCompAssignDepict.py` & `wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/chem/ChemCompAssignDepict.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,14 +97,15 @@
 from operator import itemgetter
 import inspect
 
 from wwpdb.apps.ccmodule.depict.ChemCompDepict import ChemCompDepict
 # from wwpdb.apps.ccmodule.chem.PdbxChemCompAssign import PdbxCategoryDefinition
 from wwpdb.apps.ccmodule.io.ChemCompAssignDataStore import ChemCompAssignDataStore
 from wwpdb.utils.config.ConfigInfo import ConfigInfo
+from wwpdb.utils.config.ConfigInfoApp import ConfigInfoAppCc
 from wwpdb.utils.oe_util.oedepict.OeDepict import OeDepict
 from wwpdb.utils.oe_util.build.OeBuildMol import OeBuildMol
 
 
 class ChemCompAssignDepict(ChemCompDepict):
     """ Class responsible for generating HTML depictions of
         chemical component assignment search results.
@@ -119,14 +120,15 @@
         """
         super(ChemCompAssignDepict, self).__init__(verbose, log)
         self.__verbose = verbose
         self.__lfh = log
         self.__debug = True
         #
         self.__cI = ConfigInfo()
+        self.__cIAppCc = ConfigInfoAppCc(verbose=self.__verbose, log=self.__lfh)
         #
         # self.__cDict = PdbxCategoryDefinition._cDict
         #
         # self.__noDisplayList = ['']
         #
         self.__pathGlblVwTmplts = "templates/workflow_ui/global_view"
         self.__pathInstncsVwTmplts = "templates/workflow_ui/instances_view"
@@ -378,14 +380,16 @@
         hlprDict['instance'] = wfInstId  # i.e. workflow instance ID
         hlprDict['identifier'] = depId
         hlprDict['html_template_path'] = htmlTmpltPth
         hlprDict['jmol_code_base'] = self.jmolCodeBase
         #
         oL = []
         #
+        if self.__cIAppCc.get_extended_ccd_supp():
+            oL.append('<script>max_ccd_width = 5;</script>\n')
         oL.append('<div id="cc_entity_browser">\n<h4>Browse Chem Components by Entity Group</h4>\n<div id="pagi" class="noprint fltlft"></div>\n<br class="clearfloat" />\n')
         oL.append('<div id="cc_entity_browse_content">\n')
         i = 0
         # prevGrp and newGrp to keep track of changes in the entity grouping as we move from ligand instance to ligand instance
         prevGrp = ''
         newGrp = False
         #
@@ -527,14 +531,20 @@
         ##
         grpAssgnCnt = p_ccAssgnDataStr.getAssgndInstncsCntForGrp(p_authAssignedGrp)
         if grpAssgnCnt is None:
             grpAssgnCnt = 0
         ##
         ############################################################
         #
+        # CCD ID width expansion
+        if self.__cIAppCc.get_extended_ccd_supp():
+            lclDict['max_ccd_width'] = '5'
+        else:
+            lclDict['max_ccd_width'] = '3'
+
         # ######## Rerun Search handling ############################
         ##
         lclDict['link_radius_dlta'] = p_ccAssgnDataStr.getGlblRerunSrchParam_lnkRadii(p_authAssignedGrp)
         lclDict['bond_radius_dlta'] = p_ccAssgnDataStr.getGlblRerunSrchParam_bndRadii(p_authAssignedGrp)
         displayClass = ''
         buttonLbl = ''
         if bGrpHadSearchRerun:
@@ -624,14 +634,19 @@
         #######################################################################################################################################################
         #######################################################################################################################################################
         #
         #    Establish dictionary of elements used to populate html template for instance profile
         #
         #######################################################################################################################################################
         #######################################################################################################################################################
+        if self.__cIAppCc.get_extended_ccd_supp():
+            p_hlprDict['max_ccd_width'] = '5'
+        else:
+            p_hlprDict['max_ccd_width'] = '3'
+
         p_hlprDict['top_hit_ccid'] = topHitCcId
         p_hlprDict['2dpath_labld_w_hy_ref'] = os.path.join(self.rltvSessionPath, 'assign', instId, 'image', topHitCcId + '_Big.svg')
         # p_hlprDict['2dpath_labld_w_hy_ref'] = os.path.join(self.rltvSessionPath, 'assign', 'rfrnc_reports', topHitCcId, topHitCcId + '_D3L3.gif')
         p_hlprDict['2dpath_labld_no_hy_ref'] = os.path.join(self.rltvSessionPath, 'assign', instId, 'image', topHitCcId + '_Big.svg')
         # p_hlprDict['2dpath_labld_no_hy_ref'] = os.path.join(self.rltvSessionPath, 'assign', 'rfrnc_reports', topHitCcId, topHitCcId + '_D3L1.gif')
         # p_hlprDict['2dpath_labld_no_hy_ref'] = os.path.join(self.rltvSessionPath, 'assign', 'rfrnc_reports', topHitCcId, topHitCcId + '_D3L0.gif')
         topHitsList = p_ccAssgnDataStr.getTopHitsList(instId)
```

### Comparing `wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/chem/ChemCompAssignDepictLite.py` & `wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/chem/ChemCompAssignDepictLite.py`

 * *Files 0% similar despite different names*

```diff
@@ -120,18 +120,16 @@
 
         # self.__deployPath = self.__cI.get('SITE_DEPLOY_PATH')
         self.__siteSrvcUrlPathPrefix = self.__cI.get('SITE_SERVICE_URL_PATH_PREFIX', '')
         self.__workingRltvAssgnSessionPath = ''
 
         self.__alternateTopHitMarkup = '''<input id="use_exact_mtch_id_%(auth_assgnd_grp)s_%(tophit_id)s" class="c_%(auth_assgnd_grp)s addrss_msmtch use_exact_mtch_id" type="radio" name="addrss_msmtch_chc" value="use_exact_mtch_id" %(use_exact_mtch_id_checked)s %(disabled)s /><label for="use_exact_mtch_id_%(auth_assgnd_grp)s_%(tophit_id)s">Use exact match ID of <span name="%(tophit_id)s" style="color: #F00;" class="strong tophit">%(tophit_id)s</span> (<a href="http://ligand-expo.rcsb.org/pyapps/ldHandler.py?formid=cc-index-search&target=%(tophit_id)s&operation=ccid" target="_blank">See Definition</a>) instead of originally proposed ID</label><br />'''  # noqa: E501
 
-        print("XXXX", self.__depId)
-        self.__depositPath = Path(PathInfo().getDepositPath(self.__depId)).parent
-        self.__ccReportPath = os.path.join(self.__depositPath, self.__depId, self._CC_REPORT_DIR)
-        # self.__depositAssignPath = os.path.join(self.__depositPath, self.__depId, self._CC_ASSIGN_DIR)
+        depositPath = Path(PathInfo().getDepositPath(self.__depId))
+        self.__ccReportPath = os.path.join(depositPath, self._CC_REPORT_DIR)
         self.__logger = self._setupLog(log)
 
     ################################################################################################################
     # ------------------------------------------------------------------------------------------------------------
     #      Top-level methods
     # ------------------------------------------------------------------------------------------------------------
     #
```

### Comparing `wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/chem/PdbxChemCompAssign.py` & `wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/chem/PdbxChemCompAssign.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/depict/ChemCompDepict.py` & `wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/depict/ChemCompDepict.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/extract/ccOps.py` & `wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/extract/ccOps.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/io/ChemCompAssignDataStore.py` & `wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/io/ChemCompAssignDataStore.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/io/ChemCompDataExport.py` & `wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/io/ChemCompDataExport.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/io/ChemCompDataImport.py` & `wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/io/ChemCompDataImport.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/io/ChemCompEditStore.py` & `wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/io/ChemCompEditStore.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/io/ChemCompIo.py` & `wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/io/ChemCompIo.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/reports/ChemCompAlignImageGenerator.py` & `wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/reports/ChemCompAlignImageGenerator.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/reports/ChemCompAlignImages.py` & `wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/reports/ChemCompAlignImages.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/reports/ChemCompBigAlignImages.py` & `wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/reports/ChemCompBigAlignImages.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/reports/ChemCompGenImage.py` & `wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/reports/ChemCompGenImage.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/reports/ChemCompReports.py` & `wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/reports/ChemCompReports.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,16 +68,16 @@
         if context == 'standalone':
             self.__depId = 'D_0'
             self.__ccReportPath = os.path.join(self.__sessionPath, 'assign')
         elif context == 'workflow' or context == 'unknown':
             self.__ccReportPath = os.path.join(self.__sessionPath, 'assign')
         elif context == 'deposition':
             self.__depId = self.__reqObj.getValue('identifier').upper()
-            self.__depositPath = Path(PathInfo().getDepositPath(self.__depId)).parent
-            self.__ccReportPath = os.path.join(self.__depositPath, self.__depId, 'cc_analysis')
+            depositPath = Path(PathInfo().getDepositPath(self.__depId))
+            self.__ccReportPath = os.path.join(depositPath, 'cc_analysis')
 
     def __getContext(self):
         filesource = self.__reqObj.getValue('filesource')
         depid = self.__reqObj.getValue('identifier')
 
         if depid == 'TMP_ID':
             return 'standalone'
```

### Comparing `wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/reports/InstanceDataGenerator.py` & `wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/reports/InstanceDataGenerator.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/search/ChemCompSearch.py` & `wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/search/ChemCompSearch.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/search/ChemCompSearchDb.py` & `wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/search/ChemCompSearchDb.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/search/ChemCompSearchDbDepict.py` & `wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/search/ChemCompSearchDbDepict.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/search/ChemCompSearchDepict.py` & `wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/search/ChemCompSearchDepict.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/search/DbSession.py` & `wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/search/DbSession.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/sketch/ChemCompSketch.py` & `wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/sketch/ChemCompSketch.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 import sys
 import shutil
 
 
 from wwpdb.apps.ccmodule.utils.ChemCompConfig import ChemCompConfig
 from wwpdb.apps.ccmodule.io.ChemCompIo import ChemCompReader
 from wwpdb.apps.ccmodule.extract.ccOps import ccOps
+from wwpdb.io.locator.ChemRefPathInfo import ChemRefPathInfo
 
 
 class ChemCompSketch(object):
     """Chemical component sketch launcher -
 
     """
     def __init__(self, reqObj, verbose=False, log=sys.stderr):
@@ -72,17 +73,18 @@
 
     def getFilePath(self):
         return self.__ccFilePath
 
     def __getFilePathFromId(self, ccId):
         """
         """
-        idUc = str(ccId).upper()
-        fileName = idUc + ".cif"
-        self.__ccFilePath = os.path.join(self.__ccConfig.getPath('chemCompCachePath'), idUc[0:1], idUc[0:3], fileName)
+        siteid = self.__reqObj.getValue("WWPDB_SITE_ID")
+        crpi = ChemRefPathInfo(siteid, verbose=self.__verbose, log=self.__lfh)
+
+        self.__ccFilePath = crpi.getFilePath(ccId, "CC")
         #
         if (not os.access(self.__ccFilePath, os.R_OK)):
             return False
         self.__ccFileFormat = 'cif'
         return True
 
     ##
```

### Comparing `wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/sketch/ChemCompSketchDepict.py` & `wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/sketch/ChemCompSketchDepict.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/utils/ChemCompConfig.py` & `wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/utils/ChemCompConfig.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,24 +55,22 @@
         # JDW 2011-07-07 --- These are symbolic links in the web application top directory
         # self.__archBinPath      =  os.path.join(self.__topPath,"bin")
         # self.__archDataPath      =  os.path.join(self.__topPath,"data")
 
         # RPS 2011-11-29 --- use of above symbolic links for archBinPath and archDataPath being superseded by paths determined via calls to ConfigInfo
         self.__ccAppsBinPath = os.path.join(self.__cICommon.get_site_cc_apps_path(), "bin")
         self.__ccDictPath = self.__cIAppCc.get_site_cc_dict_path()
-        self.__ccCvsPath = self.__cIAppCc.get_site_cc_cvs_path()
         self.__oeLicenseFilePath = self.__cICommon.get_site_cc_oe_licence()
         self.__oeDirPath = self.__cICommon.get_site_cc_oe_dir()
 
         #
         if (self.__verbose):
             self.__lfh.write("+ChemCompConfig.__init() --------------------------------------------------------------------------\n")
             self.__lfh.write("+ChemCompConfig.__init() ------ self.__ccAppsBinPath is: %s \n" % self.__ccAppsBinPath)
             self.__lfh.write("+ChemCompConfig.__init() ------ self.__ccDictPath is: %s \n" % self.__ccDictPath)
-            self.__lfh.write("+ChemCompConfig.__init() ------ self.__ccCvsPath is: %s \n" % self.__ccCvsPath)
             self.__lfh.write("+ChemCompConfig.__init() --------------------------------------------------------------------------\n")
         #
         # Place holders for working path info -
         self.__workingPath = None
         self.__workingRelativePath = None
 
     def setWorkingPath(self, path):
@@ -143,16 +141,16 @@
             return os.path.join(self.__ccAppsBinPath, "makeReportFromFile.csh")
 
         ##
         #  Data resource files ---
         # elif (type == "sandboxPathV2"):
         #    return os.path.join("/data/components/ligand-dict-v1")
         #
-        elif (type == "sandboxPathV3" or type == "chemCompCachePath"):
-            return self.__ccCvsPath
+        # elif (type == "sandboxPathV3" or type == "chemCompCachePath"):
+        #    return self.__ccCvsPath
         elif (type == "fpPatternPath"):
             return self.__cICommon.get_cc_fp_patterns()
         elif (type == "serializedCcDictPath"):
             return self.__cICommon.get_cc_dict_serial()
         elif (type == "serializedCcIndexPath"):
             return self.__cICommon.get_cc_dict_idx()
         elif (type == "ccIdList"):
```

### Comparing `wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/utils/ChemCompDpUtility.py` & `wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/utils/ChemCompDpUtility.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,17 +53,17 @@
 
         # setting up chem comp config
         self._ccConfig = ChemCompConfig(self._reqObj, self._verbose, self._lfh)
 
         siteId = str(self._reqObj.getValue("WWPDB_SITE_ID"))
 
         self._ccRefPathInfo = ChemRefPathInfo(siteId, verbose=self._verbose, log=self._lfh)
-        self._depositPath = Path(PathInfo().getDepositPath(self._depId)).parent
-        self._ccReportPath = os.path.join(self._depositPath, self._depId, self._CC_REPORT_DIR)
-        self._depositAssignPath = os.path.join(self._depositPath, self._depId, self._CC_ASSIGN_DIR)
+        depositPath = Path(PathInfo().getDepositPath(self._depId))
+        self._ccReportPath = os.path.join(depositPath, self._CC_REPORT_DIR)
+        self._depositAssignPath = os.path.join(depositPath, self._CC_ASSIGN_DIR)
         self._ligState = LigandAnalysisState(self._depId, self._verbose, self._lfh)
 
     def doAnalysis(self):
         self._logger.info('Starting analysis for deposition "%s"', self._depId)
 
         try:
             # checking if there is already a cc_analysis folder and removing if so
@@ -548,15 +548,16 @@
                 if (self._verbose):
                     self._logger.debug('CC assign details export directory path: %s', pathDict['picFileDirPth'])
                     self._logger.debug('CC assign details export file path: %s', pathDict['picFileFlPth'])
             else:
                 self._logger.warning('---- WARNING ---- No path obtained for CC assign details export file, id %s', depId)
 
             # chem comp depositor progress file
-            pathDict['dpstrPrgrssFileFlPth'] = os.path.join(self._depositPath, depId, 'cc-dpstr-progress')
+            depositPath = Path(PathInfo().getDepositPath(depId))
+            pathDict['dpstrPrgrssFileFlPth'] = os.path.join(depositPath, 'cc-dpstr-progress')
             pathDict['dpstrPrgrssFileDirPth'] = os.path.split(pathDict['dpstrPrgrssFileFlPth'])[0]
 
             if (self._verbose):
                 self._logger.debug('CC assign dpstr progress directory path: %s', pathDict['dpstrPrgrssFileDirPth'])
                 self._logger.debug('CC assign dpstr progress file path: %s', pathDict['dpstrPrgrssFileFlPth'])
         else:
             self._logger.warning('processing undefined filesource %r', fileSource)
```

### Comparing `wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/utils/ChemCompWFInterface.py` & `wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/utils/ChemCompWFInterface.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/utils/Exceptions.py` & `wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/utils/Exceptions.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/utils/LigandAnalysisState.py` & `wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/utils/LigandAnalysisState.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,16 +24,16 @@
 
     def __init__(self, depId, verbose=False, log=sys.stderr):
         self._verbose = verbose
         self._logging = self._setupLog(log)
 
         self._cI = ConfigInfo()
         self._depId = depId
-        self._depositPath = Path(PathInfo().getDepositPath(self._depId)).parent
-        self._ccReportPath = os.path.join(self._depositPath, self._depId, 'cc_analysis')
+        depositPath = Path(PathInfo().getDepositPath(self._depId))
+        self._ccReportPath = os.path.join(depositPath, 'cc_analysis')
         self._ccStateFilePath = os.path.join(self._ccReportPath, self._CC_STATE_FILE)
 
         self._progress = 0
         self._state = 'unknown'
 
     def init(self):
         """Initialize the ligand analysis state for this deposition.
```

### Comparing `wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/view/ChemCompView.py` & `wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/view/ChemCompView.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/view/ChemCompViewDepict.py` & `wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/view/ChemCompViewDepict.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,16 +52,16 @@
         #
         #
         sessionId = p_reqOb.getSessionId()
         htmlTmpltPth = os.path.join(p_reqOb.getValue("TemplatePath"), self.__pathDictViewTmplts)
         #
         checked = ''
         #
-        sPathRel = os.path.join(self.rltvSessionPath, ccId)
-        sPathAbslt = os.path.join(self.absltSessionPath, ccId)
+        sPathRel = os.path.join(self.rltvAssgnSessionPath, ccId)
+        sPathAbslt = os.path.join(self.absltAssgnSessionPath, ccId)
         #
         p_ccDict['sess_path_rel'] = sPathRel
         p_ccDict['jmol_code_base'] = self.jmolCodeBase
         #
         #####################################################################################################################################
         # using p_ccDict to supply text substitution content for both cc_instnc_match_rslts_tbl_tmplt.html and cc_viz_cmp_li_tmplt.html
         #####################################################################################################################################
```

### Comparing `wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/webapp/ChemCompWebApp.py` & `wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/webapp/ChemCompWebApp.py`

 * *Files 0% similar despite different names*

```diff
@@ -162,15 +162,15 @@
 #
 from wwpdb.apps.ccmodule.io.ChemCompAssignDataStore import ChemCompAssignDataStore
 from wwpdb.apps.ccmodule.io.ChemCompDataImport import ChemCompDataImport
 from wwpdb.apps.ccmodule.io.ChemCompDataExport import ChemCompDataExport
 from wwpdb.apps.ccmodule.io.ChemCompIo import ChemCompReader
 #
 from wwpdb.utils.config.ConfigInfo import ConfigInfo
-from wwpdb.utils.config.ConfigInfoApp import ConfigInfoAppCommon
+from wwpdb.utils.config.ConfigInfoApp import ConfigInfoAppCommon, ConfigInfoAppCc
 #
 from wwpdb.io.file.mmCIFUtil import mmCIFUtil
 #
 from wwpdb.utils.oe_util.oedepict.OeDepict import OeDepict
 from wwpdb.utils.oe_util.build.OeBuildMol import OeBuildMol
 #
 from wwpdb.io.locator.PathInfo import PathInfo
@@ -294,14 +294,15 @@
         self.__reqObj = reqObj
         self.__sObj = None
         self.__sessionId = None
         self.__sessionPath = None
         self.__rltvSessionPath = None
         self.__siteId = str(self.__reqObj.getValue("WWPDB_SITE_ID"))
         self.__cI = ConfigInfo(self.__siteId)
+        self.__cIAppCc = ConfigInfoAppCc(self.__siteId, verbose=self.__verbose, log=self.__lfh)
         self.__modelFilePath = None
         #
         self.__pathInstncsVwTmplts = "templates/workflow_ui/instances_view"
         self.__pathSnglInstcTmplts = self.__pathInstncsVwTmplts + "/single_instance"
         self.__pathSnglInstcEditorTmplts = self.__pathSnglInstcTmplts + "/editor"
         #
         self.__appPathD = {'/service/environment/dump': '_dumpOp',
@@ -619,14 +620,19 @@
         myD['depositionid'] = depId
         myD['instanceid'] = instanceId
         myD['filesource'] = fileSource
         myD['identifier'] = depId
         myD['instance'] = wfInstId
         myD['pdbid'] = str(self.__reqObj.getValue("pdbid"))
         myD['annotator'] = str(self.__reqObj.getValue("annotator"))
+        # CCD ID width expansion
+        if self.__cIAppCc.get_extended_ccd_supp():
+            myD['max_ccd_width'] = '5'
+        else:
+            myD['max_ccd_width'] = '3'
         #
         myD['session_url_prefix'] = os.path.join(self.__rltvSessionPath, "assign", instanceId)
         myD['processing_site'] = self.__cI.get('SITE_NAME').upper()
         rC.setHtmlText(htmlText=self.__processTemplate(fn=os.path.join(self.__pathSnglInstcEditorTmplts, "cc_instnc_chop_tmplt.html"), parameterDict=myD))
         return rC
 
     def _ccAssign_3dEnvironView(self):
```

### Comparing `wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/webapp/ChemCompWebAppLite.py` & `wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/webapp/ChemCompWebAppLite.py`

 * *Files 1% similar despite different names*

```diff
@@ -244,17 +244,14 @@
         self.__siteId = str(self.__reqObj.getValue("WWPDB_SITE_ID"))
         self.__cI = ConfigInfo(self.__siteId)
         self.__deployPath = self.__cI.get('SITE_DEPLOY_PATH')
         self.__siteSrvcUrlPathPrefix = self.__cI.get('SITE_SERVICE_URL_PATH_PREFIX', '')
         # self.__siteConfigDir = self.__cI.get('TOP_WWPDB_SITE_CONFIG_DIR')
         # self.__siteLoc = self.__cI.get('WWPDB_SITE_LOC')
         self.__pathInfo = PathInfo()
-        self.__depositPath = Path(self.__pathInfo.getDepositPath(self.__depId)).parent
-        # self.__depositAssignPath = os.path.join(self.__depositPath, self.__depId, 'assign')
-        # self.__ccReportPath = os.path.join(self.__depositPath, self.__depId, 'cc_analysis')  # should we add 'cc_analysis' in a variable in site-config?
         self.__logger = self._setupLog(log)
 
         #
         # self.__pathInstncsVwTmplts = "templates/workflow_ui/instances_view"
         # self.__pathSnglInstcTmplts = self.__pathInstncsVwTmplts + "/single_instance"
         # self.__pathSnglInstcEditorTmplts = self.__pathSnglInstcTmplts + "/editor"
         #
@@ -376,15 +373,16 @@
 
         # sessionId = self.__reqObj.getValue("sessionid")
         depId = self.__reqObj.getValue("identifier").upper()
         source = self.__reqObj.getValue("source").lower()
         ligandId = self.__reqObj.getValue("ligid")
         filename = self.__reqObj.getValue("file")
 
-        ccReportPath = os.path.join(self.__depositPath, depId, "cc_analysis")
+        depositPath = Path(self.__pathInfo.getDepositPath(depId))
+        ccReportPath = os.path.join(depositPath, "cc_analysis")
         fileType = filename.split(".")[-1]
         filePath = None
 
         if (self.__verbose):
             self.__lfh.write("+%s.%s() Requesting file '%s' from '%s' for deposition '%s'\n" % (
                 self.__class__.__name__, inspect.currentframe().f_code.co_name, filename, source, depId
             ))
```

### Comparing `wwpdb.apps.ccmodule-0.26/wwpdb/apps/ccmodule/webapp/wsgi.py` & `wwpdb.apps.ccmodule-0.27/wwpdb/apps/ccmodule/webapp/wsgi.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ccmodule-0.26/wwpdb.apps.ccmodule.egg-info/PKG-INFO` & `wwpdb.apps.ccmodule-0.27/wwpdb.apps.ccmodule.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.apps.ccmodule
-Version: 0.26
+Version: 0.27
 Summary: wwPDB workflow engine utils
 Home-page: https://github.com/rcsb/py-wwpdb_apps_wf_engine_utils
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.apps.ccmodule-0.26/wwpdb.apps.ccmodule.egg-info/SOURCES.txt` & `wwpdb.apps.ccmodule-0.27/wwpdb.apps.ccmodule.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -14,17 +14,14 @@
 wwpdb/apps/ccmodule/chem/ChemCompAssign.py
 wwpdb/apps/ccmodule/chem/ChemCompAssignDepict.py
 wwpdb/apps/ccmodule/chem/ChemCompAssignDepictLite.py
 wwpdb/apps/ccmodule/chem/PdbxChemCompAssign.py
 wwpdb/apps/ccmodule/chem/__init__.py
 wwpdb/apps/ccmodule/depict/ChemCompDepict.py
 wwpdb/apps/ccmodule/depict/__init__.py
-wwpdb/apps/ccmodule/edit/ChemCompTableEditor.py
-wwpdb/apps/ccmodule/edit/ChemCompTableEditorDepict.py
-wwpdb/apps/ccmodule/edit/__init__.py
 wwpdb/apps/ccmodule/extract/__init__.py
 wwpdb/apps/ccmodule/extract/ccOps.py
 wwpdb/apps/ccmodule/io/ChemCompAssignDataStore.py
 wwpdb/apps/ccmodule/io/ChemCompDataExport.py
 wwpdb/apps/ccmodule/io/ChemCompDataImport.py
 wwpdb/apps/ccmodule/io/ChemCompEditStore.py
 wwpdb/apps/ccmodule/io/ChemCompIo.py
```

