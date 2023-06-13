# Comparing `tmp/wwpdb.apps.entity_transform-0.17.3.tar.gz` & `tmp/wwpdb.apps.entity_transform-0.17.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wwpdb.apps.entity_transform-0.17.3.tar", last modified: Fri Mar 17 20:32:19 2023, max compression
+gzip compressed data, was "wwpdb.apps.entity_transform-0.17.4.tar", last modified: Tue Jun 13 02:00:33 2023, max compression
```

## Comparing `wwpdb.apps.entity_transform-0.17.3.tar` & `wwpdb.apps.entity_transform-0.17.4.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-17 20:32:19.295661 wwpdb.apps.entity_transform-0.17.3/
--rw-r--r--   0 vsts      (1001) docker     (123)      739 2023-03-17 20:32:19.295661 wwpdb.apps.entity_transform-0.17.3/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)       59 2023-03-17 20:30:36.000000 wwpdb.apps.entity_transform-0.17.3/README.md
--rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-03-17 20:32:19.295661 wwpdb.apps.entity_transform-0.17.3/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (123)     2439 2023-03-17 20:30:36.000000 wwpdb.apps.entity_transform-0.17.3/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-17 20:32:19.283661 wwpdb.apps.entity_transform-0.17.3/wwpdb/
--rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-03-17 20:30:36.000000 wwpdb.apps.entity_transform-0.17.3/wwpdb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-17 20:32:19.287661 wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/
--rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-03-17 20:30:36.000000 wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-17 20:32:19.287661 wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/
--rw-r--r--   0 vsts      (1001) docker     (123)      152 2023-03-17 20:30:36.000000 wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-17 20:32:19.287661 wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/depict/
--rw-r--r--   0 vsts      (1001) docker     (123)     3008 2023-03-17 20:30:36.000000 wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/depict/DepictBase.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2941 2023-03-17 20:30:36.000000 wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/depict/LinkDepict.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7538 2023-03-17 20:30:36.000000 wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/depict/PrdSummaryDepict.py
--rw-r--r--   0 vsts      (1001) docker     (123)    19491 2023-03-17 20:30:36.000000 wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/depict/ProcessPrdSummary.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1905 2023-03-17 20:30:36.000000 wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/depict/ProcessSummary_main.py
--rw-r--r--   0 vsts      (1001) docker     (123)    11097 2023-03-17 20:30:36.000000 wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/depict/ResultDepict.py
--rw-r--r--   0 vsts      (1001) docker     (123)    15972 2023-03-17 20:30:36.000000 wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/depict/SeqDepict.py
--rw-r--r--   0 vsts      (1001) docker     (123)    16966 2023-03-17 20:30:36.000000 wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/depict/StrFormDepict.py
--rw-r--r--   0 vsts      (1001) docker     (123)    11163 2023-03-17 20:30:36.000000 wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/depict/StrSummaryDepict.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-03-17 20:30:36.000000 wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/depict/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-17 20:32:19.287661 wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/openeye_util/
--rw-r--r--   0 vsts      (1001) docker     (123)    11226 2023-03-17 20:30:36.000000 wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/openeye_util/OpenEyeUtil.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-03-17 20:30:36.000000 wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/openeye_util/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-17 20:32:19.291661 wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/prd/
--rw-r--r--   0 vsts      (1001) docker     (123)     6296 2023-03-17 20:30:36.000000 wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/prd/BuildPrd.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7726 2023-03-17 20:30:36.000000 wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/prd/BuildPrdUtil.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5520 2023-03-17 20:30:36.000000 wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/prd/CVSCommit.py
--rw-r--r--   0 vsts      (1001) docker     (123)    12737 2023-03-17 20:30:36.000000 wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/prd/DepictPrd.py
--rw-r--r--   0 vsts      (1001) docker     (123)    12192 2023-03-17 20:30:36.000000 wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/prd/DepictUtil.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3149 2023-03-17 20:30:36.000000 wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/prd/HtmlUtil.py
--rw-r--r--   0 vsts      (1001) docker     (123)    13935 2023-03-17 20:30:36.000000 wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/prd/ReadFormUtil.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4403 2023-03-17 20:30:36.000000 wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/prd/UpdatePrd.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-03-17 20:30:36.000000 wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/prd/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-17 20:32:19.291661 wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/update/
--rw-r--r--   0 vsts      (1001) docker     (123)     7032 2023-03-17 20:30:36.000000 wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/update/ChopperHandler.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5210 2023-03-17 20:30:36.000000 wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/update/CombineCoord.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2337 2023-03-17 20:30:36.000000 wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/update/EditPolymer.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1229 2023-03-17 20:30:36.000000 wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/update/MergeLigand.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1225 2023-03-17 20:30:36.000000 wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/update/MergePolymer.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2335 2023-03-17 20:30:36.000000 wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/update/SplitPolymer.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7591 2023-03-17 20:30:36.000000 wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/update/UpdateBase.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5386 2023-03-17 20:30:36.000000 wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/update/UpdateFile.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-03-17 20:30:36.000000 wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/update/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-17 20:32:19.295661 wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/utils/
--rw-r--r--   0 vsts      (1001) docker     (123)     8092 2023-03-17 20:30:36.000000 wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/utils/CommandUtil.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3203 2023-03-17 20:30:36.000000 wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/utils/CompUtil.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5283 2023-03-17 20:30:36.000000 wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/utils/DownloadFile.py
--rw-r--r--   0 vsts      (1001) docker     (123)      687 2023-03-17 20:30:36.000000 wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/utils/GetLogMessage.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4035 2023-03-17 20:30:36.000000 wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/utils/ImageGenerator.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6104 2023-03-17 20:30:36.000000 wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/utils/LinkUtil.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2191 2023-03-17 20:30:36.000000 wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/utils/RemoveEmptyCategories.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6825 2023-03-17 20:30:36.000000 wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/utils/SummaryCifUtil.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2748 2023-03-17 20:30:36.000000 wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/utils/WFDataIOUtil.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-03-17 20:30:36.000000 wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/utils/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3391 2023-03-17 20:30:36.000000 wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/utils/mmCIFUtil.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-17 20:32:19.295661 wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/webapp/
--rw-r--r--   0 vsts      (1001) docker     (123)    55271 2023-03-17 20:30:36.000000 wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/webapp/EntityWebApp.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6414 2023-03-17 20:30:36.000000 wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/webapp/FormPreProcess.py
--rwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-17 20:30:36.000000 wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/webapp/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-17 20:32:19.287661 wwpdb.apps.entity_transform-0.17.3/wwpdb.apps.entity_transform.egg-info/
--rw-rw-rw-   0 vsts      (1001) docker     (123)      739 2023-03-17 20:32:19.000000 wwpdb.apps.entity_transform-0.17.3/wwpdb.apps.entity_transform.egg-info/PKG-INFO
--rw-rw-rw-   0 vsts      (1001) docker     (123)     2601 2023-03-17 20:32:19.000000 wwpdb.apps.entity_transform-0.17.3/wwpdb.apps.entity_transform.egg-info/SOURCES.txt
--rw-rw-rw-   0 vsts      (1001) docker     (123)        1 2023-03-17 20:32:19.000000 wwpdb.apps.entity_transform-0.17.3/wwpdb.apps.entity_transform.egg-info/dependency_links.txt
--rw-rw-rw-   0 vsts      (1001) docker     (123)        1 2023-03-17 20:32:03.000000 wwpdb.apps.entity_transform-0.17.3/wwpdb.apps.entity_transform.egg-info/not-zip-safe
--rw-rw-rw-   0 vsts      (1001) docker     (123)      194 2023-03-17 20:32:19.000000 wwpdb.apps.entity_transform-0.17.3/wwpdb.apps.entity_transform.egg-info/requires.txt
--rw-rw-rw-   0 vsts      (1001) docker     (123)        6 2023-03-17 20:32:19.000000 wwpdb.apps.entity_transform-0.17.3/wwpdb.apps.entity_transform.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:00:33.193601 wwpdb.apps.entity_transform-0.17.4/
+-rw-r--r--   0 vsts      (1001) docker     (123)      739 2023-06-13 02:00:33.193601 wwpdb.apps.entity_transform-0.17.4/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)       59 2023-06-13 01:59:02.000000 wwpdb.apps.entity_transform-0.17.4/README.md
+-rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-06-13 02:00:33.193601 wwpdb.apps.entity_transform-0.17.4/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (123)     2439 2023-06-13 01:59:02.000000 wwpdb.apps.entity_transform-0.17.4/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:00:33.185601 wwpdb.apps.entity_transform-0.17.4/wwpdb/
+-rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-06-13 01:59:02.000000 wwpdb.apps.entity_transform-0.17.4/wwpdb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:00:33.185601 wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/
+-rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-06-13 01:59:02.000000 wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:00:33.189601 wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/
+-rw-r--r--   0 vsts      (1001) docker     (123)      152 2023-06-13 01:59:02.000000 wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:00:33.189601 wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/depict/
+-rw-r--r--   0 vsts      (1001) docker     (123)     3008 2023-06-13 01:59:02.000000 wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/depict/DepictBase.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2941 2023-06-13 01:59:02.000000 wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/depict/LinkDepict.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7538 2023-06-13 01:59:02.000000 wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/depict/PrdSummaryDepict.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    19491 2023-06-13 01:59:02.000000 wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/depict/ProcessPrdSummary.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1905 2023-06-13 01:59:02.000000 wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/depict/ProcessSummary_main.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    11023 2023-06-13 01:59:02.000000 wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/depict/ResultDepict.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    15972 2023-06-13 01:59:02.000000 wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/depict/SeqDepict.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    16966 2023-06-13 01:59:02.000000 wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/depict/StrFormDepict.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    11163 2023-06-13 01:59:02.000000 wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/depict/StrSummaryDepict.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 01:59:02.000000 wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/depict/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:00:33.189601 wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/openeye_util/
+-rw-r--r--   0 vsts      (1001) docker     (123)    11226 2023-06-13 01:59:02.000000 wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/openeye_util/OpenEyeUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 01:59:02.000000 wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/openeye_util/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:00:33.189601 wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/prd/
+-rw-r--r--   0 vsts      (1001) docker     (123)     6296 2023-06-13 01:59:02.000000 wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/prd/BuildPrd.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7726 2023-06-13 01:59:02.000000 wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/prd/BuildPrdUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5529 2023-06-13 01:59:02.000000 wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/prd/CVSCommit.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    12737 2023-06-13 01:59:02.000000 wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/prd/DepictPrd.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    12192 2023-06-13 01:59:02.000000 wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/prd/DepictUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3149 2023-06-13 01:59:02.000000 wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/prd/HtmlUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    13935 2023-06-13 01:59:02.000000 wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/prd/ReadFormUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4403 2023-06-13 01:59:02.000000 wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/prd/UpdatePrd.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 01:59:02.000000 wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/prd/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:00:33.193601 wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/update/
+-rw-r--r--   0 vsts      (1001) docker     (123)     7032 2023-06-13 01:59:02.000000 wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/update/ChopperHandler.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5210 2023-06-13 01:59:02.000000 wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/update/CombineCoord.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2337 2023-06-13 01:59:02.000000 wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/update/EditPolymer.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1229 2023-06-13 01:59:02.000000 wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/update/MergeLigand.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1225 2023-06-13 01:59:02.000000 wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/update/MergePolymer.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2335 2023-06-13 01:59:02.000000 wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/update/SplitPolymer.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7591 2023-06-13 01:59:02.000000 wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/update/UpdateBase.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5386 2023-06-13 01:59:02.000000 wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/update/UpdateFile.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 01:59:02.000000 wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/update/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:00:33.193601 wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/utils/
+-rw-r--r--   0 vsts      (1001) docker     (123)     8180 2023-06-13 01:59:02.000000 wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/utils/CommandUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3003 2023-06-13 01:59:02.000000 wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/utils/CompUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5283 2023-06-13 01:59:02.000000 wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/utils/DownloadFile.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      687 2023-06-13 01:59:02.000000 wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/utils/GetLogMessage.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4035 2023-06-13 01:59:02.000000 wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/utils/ImageGenerator.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6104 2023-06-13 01:59:02.000000 wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/utils/LinkUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2191 2023-06-13 01:59:02.000000 wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/utils/RemoveEmptyCategories.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6825 2023-06-13 01:59:02.000000 wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/utils/SummaryCifUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2748 2023-06-13 01:59:02.000000 wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/utils/WFDataIOUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 01:59:02.000000 wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/utils/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3391 2023-06-13 01:59:02.000000 wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/utils/mmCIFUtil.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:00:33.193601 wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/webapp/
+-rw-r--r--   0 vsts      (1001) docker     (123)    55271 2023-06-13 01:59:02.000000 wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/webapp/EntityWebApp.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6426 2023-06-13 01:59:02.000000 wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/webapp/FormPreProcess.py
+-rwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 01:59:02.000000 wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/webapp/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:00:33.185601 wwpdb.apps.entity_transform-0.17.4/wwpdb.apps.entity_transform.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)      739 2023-06-13 02:00:33.000000 wwpdb.apps.entity_transform-0.17.4/wwpdb.apps.entity_transform.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     2601 2023-06-13 02:00:33.000000 wwpdb.apps.entity_transform-0.17.4/wwpdb.apps.entity_transform.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-13 02:00:33.000000 wwpdb.apps.entity_transform-0.17.4/wwpdb.apps.entity_transform.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-13 02:00:22.000000 wwpdb.apps.entity_transform-0.17.4/wwpdb.apps.entity_transform.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)      194 2023-06-13 02:00:33.000000 wwpdb.apps.entity_transform-0.17.4/wwpdb.apps.entity_transform.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        6 2023-06-13 02:00:33.000000 wwpdb.apps.entity_transform-0.17.4/wwpdb.apps.entity_transform.egg-info/top_level.txt
```

### Comparing `wwpdb.apps.entity_transform-0.17.3/PKG-INFO` & `wwpdb.apps.entity_transform-0.17.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.apps.entity_transform
-Version: 0.17.3
+Version: 0.17.4
 Summary: wwPDB entity transformer
 Home-page: https://github.com/rcsb/py-wwpdb_apps_entity_transform
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.apps.entity_transform-0.17.3/setup.py` & `wwpdb.apps.entity_transform-0.17.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         'Programming Language :: Python',
         'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
     ],
     #
-    install_requires=['wwpdb.utils.config ~= 0.24', 'wwpdb.apps.editormodule >= 0.13.1',
+    install_requires=['wwpdb.utils.config ~= 0.34', 'wwpdb.apps.editormodule >= 0.13.1',
                       'wwpdb.io', 'wwpdb.utils.dp', 'wwpdb.utils.detach',
                       'wwpdb.utils.session', 'wwpdb.utils.wf',
                       'wwpdb.utils.oe_util'],
     packages=find_packages(exclude=['wwpdb.apps.tests-entity_transform',
                                     'mock-data']),
     # Enables Manifest to be used
     # include_package_data = True,
```

### Comparing `wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/depict/DepictBase.py` & `wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/depict/DepictBase.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/depict/LinkDepict.py` & `wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/depict/LinkDepict.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/depict/PrdSummaryDepict.py` & `wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/depict/PrdSummaryDepict.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/depict/ProcessPrdSummary.py` & `wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/depict/ProcessPrdSummary.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/depict/ProcessSummary_main.py` & `wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/depict/ProcessSummary_main.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/depict/ResultDepict.py` & `wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/depict/ResultDepict.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,28 +20,28 @@
 __email__ = "zfeng@rcsb.rutgers.edu"
 __license__ = "Creative Commons Attribution 3.0 Unported"
 __version__ = "V0.07"
 
 import os
 import sys
 
-from wwpdb.utils.config.ConfigInfoApp import ConfigInfoAppCommon
 from wwpdb.io.file.mmCIFUtil import mmCIFUtil
+from wwpdb.io.locator.ChemRefPathInfo import ChemRefPathInfo
 from wwpdb.apps.entity_transform.depict.DepictBase import DepictBase
 #
 
 
 class ResultDepict(DepictBase):
     """ Class responsible for generating HTML depiction of PRD search results.
     """
     def __init__(self, reqObj=None, summaryCifObj=None, verbose=False, log=sys.stderr):
         super(ResultDepict, self).__init__(reqObj=reqObj, summaryCifObj=summaryCifObj, verbose=verbose, log=log)
         #
         self.__siteId = str(self._reqObj.getValue("WWPDB_SITE_ID"))
-        self.__cICommon = ConfigInfoAppCommon(self.__siteId)
+        self.__crpi = ChemRefPathInfo(siteId=self.__siteId, verbose=verbose, log=log)
         #
         self.__instIds = self._cifObj.getMatchInstIds()
         self.__matchResults = self._cifObj.getMatchResults()
 
     def getSeqs(self, instId):
         return self._cifObj.getSeq(instId)
 
@@ -253,20 +253,21 @@
         #
         return content
 
     def __getStatus(self, cid):
         sourcefile = ''
         category = ''
         item = ''
+
         if cid[:4] == 'PRD_':
-            sourcefile = os.path.join(self.__cICommon.get_site_prd_cvs_path(), cid[len(cid) - 1], cid + '.cif')
+            sourcefile = self.__crpi.getFilePath(cid, "PRD")
             category = 'pdbx_reference_molecule'
             item = 'release_status'
         else:
-            sourcefile = os.path.join(self.__cICommon.get_site_cc_cvs_path(), cid[0], cid, cid + '.cif')
+            sourcefile = self.__crpi.getFilePath(cid, "CC")
             category = 'chem_comp'
             item = 'pdbx_release_status'
         #
         if not sourcefile:
             return ''
         if not os.access(sourcefile, os.F_OK):
             return ''
```

### Comparing `wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/depict/SeqDepict.py` & `wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/depict/SeqDepict.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/depict/StrFormDepict.py` & `wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/depict/StrFormDepict.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/depict/StrSummaryDepict.py` & `wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/depict/StrSummaryDepict.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/openeye_util/OpenEyeUtil.py` & `wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/openeye_util/OpenEyeUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/prd/BuildPrd.py` & `wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/prd/BuildPrd.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/prd/BuildPrdUtil.py` & `wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/prd/BuildPrdUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/prd/CVSCommit.py` & `wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/prd/CVSCommit.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 __license__ = "Creative Commons Attribution 3.0 Unported"
 __version__ = "V0.07"
 
 import os
 import sys
 
 from wwpdb.utils.config.ConfigInfo import ConfigInfo
-from wwpdb.utils.config.ConfigInfoApp import ConfigInfoAppCommon
+from wwpdb.utils.config.ConfigInfoApp import ConfigInfoAppCc
 
 from wwpdb.apps.entity_transform.utils.GetLogMessage import GetLogMessage
 
 
 #
 
 class CVSCommit(object):
@@ -43,17 +43,17 @@
         self.__reqObj = reqObj
         self.__sObj = None
         self.__sessionId = None
         self.__sessionPath = None
         # self.__rltvSessionPath = None
         self.__siteId = str(self.__reqObj.getValue("WWPDB_SITE_ID"))
         self.__cI = ConfigInfo(self.__siteId)
-        self.__cICommon = ConfigInfoAppCommon(self.__siteId)
-        self.__prdRoot = self.__cICommon.get_site_prd_cvs_path()
-        self.__prdccRoot = self.__cICommon.get_site_prdcc_cvs_path()
+        self.__cIACc = ConfigInfoAppCc(self.__siteId, verbose=verbose, log=log)
+        self.__prdRoot = self.__cIACc.get_site_prd_cvs_path()
+        self.__prdccRoot = self.__cIACc.get_site_prdcc_cvs_path()
         #
         self.__PrdIDList = None
         self.__returnError = ""
 
         self.__getSession()
         #
```

### Comparing `wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/prd/DepictPrd.py` & `wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/prd/DepictPrd.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/prd/DepictUtil.py` & `wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/prd/DepictUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/prd/HtmlUtil.py` & `wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/prd/HtmlUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/prd/ReadFormUtil.py` & `wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/prd/ReadFormUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/prd/UpdatePrd.py` & `wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/prd/UpdatePrd.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/update/ChopperHandler.py` & `wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/update/ChopperHandler.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/update/CombineCoord.py` & `wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/update/CombineCoord.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/update/EditPolymer.py` & `wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/update/EditPolymer.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/update/MergeLigand.py` & `wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/update/MergeLigand.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/update/MergePolymer.py` & `wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/update/MergePolymer.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/update/SplitPolymer.py` & `wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/update/SplitPolymer.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/update/UpdateBase.py` & `wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/update/UpdateBase.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/update/UpdateFile.py` & `wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/update/UpdateFile.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/utils/CommandUtil.py` & `wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/utils/CommandUtil.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,28 +25,29 @@
 import os
 import signal
 import subprocess
 import sys
 import time
 import traceback
 
-from wwpdb.utils.config.ConfigInfoApp import ConfigInfoAppCommon
+from wwpdb.utils.config.ConfigInfoApp import ConfigInfoAppCommon, ConfigInfoAppCc
 
 
 class CommandUtil(object):
     """ Class for running back-end commands
     """
     def __init__(self, reqObj=None, verbose=False, log=sys.stderr):  # pylint: disable=unused-argument
         # self.__verbose = verbose
         self.__lfh = log
         self.__reqObj = reqObj
         self.__sObj = None
         self.__sessionPath = None
         self.__siteId = str(self.__reqObj.getValue("WWPDB_SITE_ID"))
         self.__cICommon = ConfigInfoAppCommon(self.__siteId)
+        self.__cIcc = ConfigInfoAppCc(self.__siteId, verbose=verbose, log=log)
         #
 
     def setSessionPath(self, sessionPath):
         """ Set session path
         """
         self.__sessionPath = sessionPath
 
@@ -166,16 +167,16 @@
         #
 
     def __getAnnotSetting(self):
         """ Get Annot package bash setting
         """
         setting = " RCSBROOT=" + self.__cICommon.get_site_annot_tools_path() + "; export RCSBROOT; PDB2GLYCAN=" \
             + os.path.join(os.path.abspath(self.__cICommon.get_site_packages_path()), "pdb2glycan", "bin", "PDB2Glycan") + "; export PDB2GLYCAN; " \
-            + " COMP_PATH=" + self.__cICommon.get_site_cc_cvs_path() + "; export COMP_PATH; " \
-            + " PRD_PATH=" + self.__cICommon.get_site_prd_cvs_path() + "; export PRD_PATH; " \
+            + " COMP_PATH=" + self.__cIcc.get_site_cc_cvs_path() + "; export COMP_PATH; " \
+            + " PRD_PATH=" + self.__cIcc.get_site_prd_cvs_path() + "; export PRD_PATH; " \
             + " BINPATH=${RCSBROOT}/bin; export BINPATH; "
         #
         return setting
 
     def __getCCToolSetting(self):
         """ Get CC_TOOLS package bash setting
         """
```

### Comparing `wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/utils/CompUtil.py` & `wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/utils/CompUtil.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,70 +21,69 @@
 __license__ = "Creative Commons Attribution 3.0 Unported"
 __version__ = "V0.07"
 
 import os
 import sys
 
 from wwpdb.io.file.mmCIFUtil import mmCIFUtil
-from wwpdb.utils.config.ConfigInfoApp import ConfigInfoAppCommon
+from wwpdb.io.locator.ChemRefPathInfo import ChemRefPathInfo
 
 
 class CompUtil(object):
     """ Class responsible for checking Comp/PRD ID and finding chemical component file.
     """
     def __init__(self, reqObj=None, verbose=False, log=sys.stderr):  # pylint: disable=unused-argument
+        self.__verbose = verbose
+        self.__lfh = log
+
         self.__reqObj = reqObj
         self.__siteId = str(self.__reqObj.getValue("WWPDB_SITE_ID"))
-        self.__cICommon = ConfigInfoAppCommon(self.__siteId)
-        #
-        self.__ccPath = self.__cICommon.get_site_cc_cvs_path()
-        self.__prdPath = self.__cICommon.get_site_prd_cvs_path()
-        self.__prdccPath = self.__cICommon.get_site_prdcc_cvs_path()
+        self.__crpi = ChemRefPathInfo(siteId=self.__siteId, verbose=self.__verbose, log=self.__lfh)
         #
 
     def checkInputId(self, id):  # pylint: disable=redefined-builtin
-        filePath = os.path.join(self.__ccPath, id[0], id, id + '.cif')
+        filePath = self.__crpi.getFilePath(id, "CC")
         if id[:4] == 'PRD_':
-            filePath = os.path.join(self.__prdPath, id[len(id) - 1], id + '.cif')
+            filePath = self.__crpi.getFilePath(id, "PRD")
         #
-        if not os.access(filePath, os.F_OK):
+        if filePath is None or not os.access(filePath, os.F_OK):
             return id + ' is not a valid Component or PRD ID.\n'
         #
         if id[:4] == 'PRD_':
             cf = mmCIFUtil(filePath=filePath)
             status = cf.GetSingleValue('pdbx_reference_molecule', 'release_status')
             if status.strip().upper() == "WAIT":
                 return id + ' has status "WAIT".\n'
             #
         #
         return ''
 
     def getTemplateFile(self, id):  # pylint: disable=redefined-builtin
         if id[:4] == 'PRD_':
             ccid = id.replace('PRD', 'PRDCC')
-            filePath1 = os.path.join(self.__prdccPath, ccid[len(ccid) - 1], ccid + '.cif')
+            filePath1 = self.__crpi.getFilePath(ccid, "PRDCC")
             if os.access(filePath1, os.F_OK):
                 return filePath1
             #
             # check single ligand defined in PRD entry
             #
-            fileName = os.path.join(self.__prdPath, id[len(id) - 1], id + '.cif')
+            fileName = self.__crpi.getFilePath(id, "PRD")
             cf = mmCIFUtil(filePath=fileName)
             dlist = cf.GetValue('pdbx_reference_molecule')
             if not dlist:
                 return ''
             #
             if 'chem_comp_id' not in dlist[0]:
                 return ''
             #
             ccid = dlist[0]['chem_comp_id'].strip().upper()
-            filePath1 = os.path.join(self.__ccPath, ccid[0], ccid, ccid + '.cif')
-            if os.access(filePath1, os.F_OK):
+            filePath1 = self.__crpi.getFilePath(ccid, "CC")
+            if filePath1 and os.access(filePath1, os.F_OK):
                 return filePath1
             #
         else:
-            filePath = os.path.join(self.__ccPath, id[0], id, id + '.cif')
-            if os.access(filePath, os.F_OK):
+            filePath = self.__crpi.getFilePath(id, "CC")
+            if filePath and os.access(filePath, os.F_OK):
                 return filePath
             #
         #
         return ''
```

### Comparing `wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/utils/DownloadFile.py` & `wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/utils/DownloadFile.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/utils/GetLogMessage.py` & `wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/utils/GetLogMessage.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/utils/ImageGenerator.py` & `wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/utils/ImageGenerator.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/utils/LinkUtil.py` & `wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/utils/LinkUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/utils/RemoveEmptyCategories.py` & `wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/utils/RemoveEmptyCategories.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/utils/SummaryCifUtil.py` & `wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/utils/SummaryCifUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/utils/WFDataIOUtil.py` & `wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/utils/WFDataIOUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/utils/mmCIFUtil.py` & `wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/utils/mmCIFUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/webapp/EntityWebApp.py` & `wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/webapp/EntityWebApp.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.entity_transform-0.17.3/wwpdb/apps/entity_transform/webapp/FormPreProcess.py` & `wwpdb.apps.entity_transform-0.17.4/wwpdb/apps/entity_transform/webapp/FormPreProcess.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,30 +90,30 @@
         self.__getUsrDefinedgroup(self.__chainList, 'chain_', group_id, dic)
         self.__getUsrDefinedgroup(self.__ligandList, 'ligand_', group_id, dic)
         self.__getUsrDefinedgroup(self.__groupList, 'group_', group_id, dic)
         #
         if not group_id:
             if ((self.__submitValue == 'Merge to polymer') or (self.__submitValue == 'Merge to ligand')) and \
                (len(self.__labelDic) == 1):
-                self.__errorMessage = 'Only one instance "' + self.__labelDic.keys()[0] + '" is selected.'
+                self.__errorMessage = 'Only one instance "' + list(self.__labelDic.keys())[0] + '" is selected.'
             #
             return
         #
         if (len(group_id) > 1) and (self.__submitValue == 'Merge/Split with chopper'):
             self.__errorMessage = 'Multiple User defind Group IDs are assigned. For "Merge/Split ' \
                 + 'with chopper" option, only one User defind Group can be processed each time.\n'
             return
         #
         for lid, label in self.__labelDic.items():
             if lid not in self.__valueDic:
                 self.__errorMessage += 'No User defind Group ID assigned for "' + label + '".<br/>\n'
             #
         #
         if ((self.__submitValue == 'Merge to polymer') or (self.__submitValue == 'Merge to ligand')):
-            for gid in sorted(dic.keys()):
+            for gid in sorted(list(dic.keys())):
                 if len(dic[gid]) == 1:
                     self.__errorMessage += 'For "User defind Group ' + gid + '", only one instance "' + dic[gid][0] + '" is selected.<br/>\n'
                 #
             #
         #
 
     def __getLabelDic(self, instList, label_prefix):
```

### Comparing `wwpdb.apps.entity_transform-0.17.3/wwpdb.apps.entity_transform.egg-info/PKG-INFO` & `wwpdb.apps.entity_transform-0.17.4/wwpdb.apps.entity_transform.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.apps.entity-transform
-Version: 0.17.3
+Version: 0.17.4
 Summary: wwPDB entity transformer
 Home-page: https://github.com/rcsb/py-wwpdb_apps_entity_transform
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.apps.entity_transform-0.17.3/wwpdb.apps.entity_transform.egg-info/SOURCES.txt` & `wwpdb.apps.entity_transform-0.17.4/wwpdb.apps.entity_transform.egg-info/SOURCES.txt`

 * *Files identical despite different names*

