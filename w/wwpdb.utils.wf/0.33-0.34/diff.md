# Comparing `tmp/wwpdb.utils.wf-0.33.tar.gz` & `tmp/wwpdb.utils.wf-0.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wwpdb.utils.wf-0.33.tar", last modified: Sun Apr 30 13:33:39 2023, max compression
+gzip compressed data, was "wwpdb.utils.wf-0.34.tar", last modified: Tue Jun 13 02:58:17 2023, max compression
```

## Comparing `wwpdb.utils.wf-0.33.tar` & `wwpdb.utils.wf-0.34.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-30 13:33:39.764764 wwpdb.utils.wf-0.33/
--rw-r--r--   0 vsts      (1001) docker     (123)      552 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (123)      745 2023-04-30 13:33:39.764764 wwpdb.utils.wf-0.33/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      485 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/README.md
--rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-04-30 13:33:39.764764 wwpdb.utils.wf-0.33/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (123)     2105 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-30 13:33:39.752764 wwpdb.utils.wf-0.33/wwpdb/
--rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/wwpdb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-30 13:33:39.756764 wwpdb.utils.wf-0.33/wwpdb/utils/
--rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/wwpdb/utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-30 13:33:39.760764 wwpdb.utils.wf-0.33/wwpdb/utils/wf/
--rw-r--r--   0 vsts      (1001) docker     (123)     3229 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/wwpdb/utils/wf/DataSelector.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4658 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/wwpdb/utils/wf/DataValueContainer.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3661 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/wwpdb/utils/wf/WfDataObject.py
--rw-r--r--   0 vsts      (1001) docker     (123)      150 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/wwpdb/utils/wf/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-30 13:33:39.760764 wwpdb.utils.wf-0.33/wwpdb/utils/wf/dbapi/
--rw-r--r--   0 vsts      (1001) docker     (123)     6846 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/wwpdb/utils/wf/dbapi/DbApiUtil.py
--rw-r--r--   0 vsts      (1001) docker     (123)    16002 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/wwpdb/utils/wf/dbapi/DbCommand.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4025 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/wwpdb/utils/wf/dbapi/DbConnection.py
--rwxr-xr-x   0 vsts      (1001) docker     (123)     1946 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/wwpdb/utils/wf/dbapi/LocalDbApi.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3018 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/wwpdb/utils/wf/dbapi/StatusDbApi.py
--rwxr-xr-x   0 vsts      (1001) docker     (123)     1281 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/wwpdb/utils/wf/dbapi/WFEtime.py
--rw-r--r--   0 vsts      (1001) docker     (123)    47456 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/wwpdb/utils/wf/dbapi/WfDbApi.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4251 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/wwpdb/utils/wf/dbapi/WfTracking.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/wwpdb/utils/wf/dbapi/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    11637 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/wwpdb/utils/wf/dbapi/dbAPI.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-30 13:33:39.764764 wwpdb.utils.wf-0.33/wwpdb/utils/wf/plugins/
--rw-r--r--   0 vsts      (1001) docker     (123)    59795 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/wwpdb/utils/wf/plugins/AnnotationUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)    11876 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/wwpdb/utils/wf/plugins/ChemCompUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3611 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/wwpdb/utils/wf/plugins/DictUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3595 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/wwpdb/utils/wf/plugins/DpUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)    16296 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/wwpdb/utils/wf/plugins/EmUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6275 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/wwpdb/utils/wf/plugins/FileUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)    13301 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/wwpdb/utils/wf/plugins/FormatUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)    50817 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/wwpdb/utils/wf/plugins/NmrUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)    13901 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/wwpdb/utils/wf/plugins/PdbxUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3840 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/wwpdb/utils/wf/plugins/PrdSearchUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3427 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/wwpdb/utils/wf/plugins/ReportUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5580 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/wwpdb/utils/wf/plugins/SFConvert.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5698 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/wwpdb/utils/wf/plugins/SeqStatsUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)    11212 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/wwpdb/utils/wf/plugins/SeqdbUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1456 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/wwpdb/utils/wf/plugins/UtilsBase.py
--rw-r--r--   0 vsts      (1001) docker     (123)    24022 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/wwpdb/utils/wf/plugins/ValidationUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/wwpdb/utils/wf/plugins/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-30 13:33:39.764764 wwpdb.utils.wf-0.33/wwpdb/utils/wf/process/
--rw-r--r--   0 vsts      (1001) docker     (123)    15843 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/wwpdb/utils/wf/process/ActionRegistry.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7456 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/wwpdb/utils/wf/process/ActionRegistryIo.py
--rw-r--r--   0 vsts      (1001) docker     (123)    11325 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/wwpdb/utils/wf/process/ProcessRunner.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/wwpdb/utils/wf/process/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-30 13:33:39.764764 wwpdb.utils.wf-0.33/wwpdb/utils/wf/schema/
--rw-r--r--   0 vsts      (1001) docker     (123)    12006 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/wwpdb/utils/wf/schema/WfSchemaMap.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/wwpdb/utils/wf/schema/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    11697 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/wwpdb/utils/wf/schema/database_descriptions.txt
--rw-r--r--   0 vsts      (1001) docker     (123)      233 2023-04-30 13:32:53.000000 wwpdb.utils.wf-0.33/wwpdb/utils/wf/schema/mandatory_items.txt
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-30 13:33:39.756764 wwpdb.utils.wf-0.33/wwpdb.utils.wf.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)      745 2023-04-30 13:33:39.000000 wwpdb.utils.wf-0.33/wwpdb.utils.wf.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     1724 2023-04-30 13:33:39.000000 wwpdb.utils.wf-0.33/wwpdb.utils.wf.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-04-30 13:33:39.000000 wwpdb.utils.wf-0.33/wwpdb.utils.wf.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-04-30 13:33:29.000000 wwpdb.utils.wf-0.33/wwpdb.utils.wf.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)      134 2023-04-30 13:33:39.000000 wwpdb.utils.wf-0.33/wwpdb.utils.wf.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        6 2023-04-30 13:33:39.000000 wwpdb.utils.wf-0.33/wwpdb.utils.wf.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:58:17.305676 wwpdb.utils.wf-0.34/
+-rw-r--r--   0 vsts      (1001) docker     (123)      552 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (123)      745 2023-06-13 02:58:17.305676 wwpdb.utils.wf-0.34/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      485 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/README.md
+-rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-06-13 02:58:17.305676 wwpdb.utils.wf-0.34/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (123)     2105 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:58:17.293676 wwpdb.utils.wf-0.34/wwpdb/
+-rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/wwpdb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:58:17.297676 wwpdb.utils.wf-0.34/wwpdb/utils/
+-rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/wwpdb/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:58:17.297676 wwpdb.utils.wf-0.34/wwpdb/utils/wf/
+-rw-r--r--   0 vsts      (1001) docker     (123)     3229 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/wwpdb/utils/wf/DataSelector.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4658 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/wwpdb/utils/wf/DataValueContainer.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3661 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/wwpdb/utils/wf/WfDataObject.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      150 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/wwpdb/utils/wf/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:58:17.297676 wwpdb.utils.wf-0.34/wwpdb/utils/wf/dbapi/
+-rw-r--r--   0 vsts      (1001) docker     (123)     6846 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/wwpdb/utils/wf/dbapi/DbApiUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    16002 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/wwpdb/utils/wf/dbapi/DbCommand.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4025 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/wwpdb/utils/wf/dbapi/DbConnection.py
+-rwxr-xr-x   0 vsts      (1001) docker     (123)     1946 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/wwpdb/utils/wf/dbapi/LocalDbApi.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3018 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/wwpdb/utils/wf/dbapi/StatusDbApi.py
+-rwxr-xr-x   0 vsts      (1001) docker     (123)     1281 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/wwpdb/utils/wf/dbapi/WFEtime.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    47456 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/wwpdb/utils/wf/dbapi/WfDbApi.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4251 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/wwpdb/utils/wf/dbapi/WfTracking.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/wwpdb/utils/wf/dbapi/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    11637 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/wwpdb/utils/wf/dbapi/dbAPI.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:58:17.305676 wwpdb.utils.wf-0.34/wwpdb/utils/wf/plugins/
+-rw-r--r--   0 vsts      (1001) docker     (123)    65750 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/wwpdb/utils/wf/plugins/AnnotationUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    11876 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/wwpdb/utils/wf/plugins/ChemCompUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3611 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/wwpdb/utils/wf/plugins/DictUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3595 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/wwpdb/utils/wf/plugins/DpUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    17700 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/wwpdb/utils/wf/plugins/EmUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6275 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/wwpdb/utils/wf/plugins/FileUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    13301 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/wwpdb/utils/wf/plugins/FormatUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    50817 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/wwpdb/utils/wf/plugins/NmrUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    13901 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/wwpdb/utils/wf/plugins/PdbxUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3840 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/wwpdb/utils/wf/plugins/PrdSearchUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3427 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/wwpdb/utils/wf/plugins/ReportUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5580 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/wwpdb/utils/wf/plugins/SFConvert.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5698 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/wwpdb/utils/wf/plugins/SeqStatsUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    11212 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/wwpdb/utils/wf/plugins/SeqdbUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1456 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/wwpdb/utils/wf/plugins/UtilsBase.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    24022 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/wwpdb/utils/wf/plugins/ValidationUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/wwpdb/utils/wf/plugins/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:58:17.305676 wwpdb.utils.wf-0.34/wwpdb/utils/wf/process/
+-rw-r--r--   0 vsts      (1001) docker     (123)    15843 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/wwpdb/utils/wf/process/ActionRegistry.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7456 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/wwpdb/utils/wf/process/ActionRegistryIo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    11325 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/wwpdb/utils/wf/process/ProcessRunner.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/wwpdb/utils/wf/process/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:58:17.305676 wwpdb.utils.wf-0.34/wwpdb/utils/wf/schema/
+-rw-r--r--   0 vsts      (1001) docker     (123)    12006 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/wwpdb/utils/wf/schema/WfSchemaMap.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/wwpdb/utils/wf/schema/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    11697 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/wwpdb/utils/wf/schema/database_descriptions.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)      233 2023-06-13 02:57:01.000000 wwpdb.utils.wf-0.34/wwpdb/utils/wf/schema/mandatory_items.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:58:17.293676 wwpdb.utils.wf-0.34/wwpdb.utils.wf.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)      745 2023-06-13 02:58:17.000000 wwpdb.utils.wf-0.34/wwpdb.utils.wf.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     1724 2023-06-13 02:58:17.000000 wwpdb.utils.wf-0.34/wwpdb.utils.wf.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-13 02:58:17.000000 wwpdb.utils.wf-0.34/wwpdb.utils.wf.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-13 02:58:03.000000 wwpdb.utils.wf-0.34/wwpdb.utils.wf.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)      134 2023-06-13 02:58:17.000000 wwpdb.utils.wf-0.34/wwpdb.utils.wf.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        6 2023-06-13 02:58:17.000000 wwpdb.utils.wf-0.34/wwpdb.utils.wf.egg-info/top_level.txt
```

### Comparing `wwpdb.utils.wf-0.33/LICENSE` & `wwpdb.utils.wf-0.34/LICENSE`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.33/PKG-INFO` & `wwpdb.utils.wf-0.34/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.utils.wf
-Version: 0.33
+Version: 0.34
 Summary: OneDep WF status DB access utilities
 Home-page: https://github.com/rcsb/py-wwpdb_utils_wf
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.utils.wf-0.33/setup.py` & `wwpdb.utils.wf-0.34/setup.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.33/wwpdb/utils/wf/DataSelector.py` & `wwpdb.utils.wf-0.34/wwpdb/utils/wf/DataSelector.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.33/wwpdb/utils/wf/DataValueContainer.py` & `wwpdb.utils.wf-0.34/wwpdb/utils/wf/DataValueContainer.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.33/wwpdb/utils/wf/WfDataObject.py` & `wwpdb.utils.wf-0.34/wwpdb/utils/wf/WfDataObject.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.33/wwpdb/utils/wf/dbapi/DbApiUtil.py` & `wwpdb.utils.wf-0.34/wwpdb/utils/wf/dbapi/DbApiUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.33/wwpdb/utils/wf/dbapi/DbCommand.py` & `wwpdb.utils.wf-0.34/wwpdb/utils/wf/dbapi/DbCommand.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.33/wwpdb/utils/wf/dbapi/DbConnection.py` & `wwpdb.utils.wf-0.34/wwpdb/utils/wf/dbapi/DbConnection.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.33/wwpdb/utils/wf/dbapi/LocalDbApi.py` & `wwpdb.utils.wf-0.34/wwpdb/utils/wf/dbapi/LocalDbApi.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.33/wwpdb/utils/wf/dbapi/StatusDbApi.py` & `wwpdb.utils.wf-0.34/wwpdb/utils/wf/dbapi/StatusDbApi.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.33/wwpdb/utils/wf/dbapi/WFEtime.py` & `wwpdb.utils.wf-0.34/wwpdb/utils/wf/dbapi/WFEtime.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.33/wwpdb/utils/wf/dbapi/WfDbApi.py` & `wwpdb.utils.wf-0.34/wwpdb/utils/wf/dbapi/WfDbApi.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.33/wwpdb/utils/wf/dbapi/WfTracking.py` & `wwpdb.utils.wf-0.34/wwpdb/utils/wf/dbapi/WfTracking.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.33/wwpdb/utils/wf/dbapi/dbAPI.py` & `wwpdb.utils.wf-0.34/wwpdb/utils/wf/dbapi/dbAPI.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.33/wwpdb/utils/wf/plugins/AnnotationUtils.py` & `wwpdb.utils.wf-0.34/wwpdb/utils/wf/plugins/AnnotationUtils.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 from wwpdb.utils.dp.DensityWrapper import DensityWrapper
 from wwpdb.utils.dp.RcsbDpUtility import RcsbDpUtility
 
 from wwpdb.utils.wf.plugins.UtilsBase import UtilsBase
 
 try:
     # We will have present on annotation system - but allow testing without
+    from wwpdb.apps.ann_tasks_v2.check.EmMapCheck import EmMapCheckTask
     from wwpdb.apps.ann_tasks_v2.io.PisaReader import PisaAssemblyReader
     from wwpdb.apps.ann_tasks_v2.em3d.EmAutoFix import EmAutoFix
     from wwpdb.apps.ann_tasks_v2.em3d.EmMapAutoFixVers import EmMapAutoFixVers
     from wwpdb.apps.ann_tasks_v2.em3d.EmHeaderUtils import EmHeaderUtils
     from wwpdb.apps.ann_tasks_v2.related.UpdateRelated import UpdateRelated
     from wwpdb.apps.ann_tasks_v2.expIoUtils.PdbxExpUpdate import PdbxExpUpdate
     from wwpdb.utils.session.WebRequest import InputRequest
@@ -236,14 +237,138 @@
                 self._lfh.write("+AnnotationUtils.dictCheckOp() - PDBx input  file path:  %s\n" % pdbxPath)
                 self._lfh.write("+AnnotationUtils.dictCheckOp() - Report file path:       %s\n" % reportPath)
             return True
         except Exception as _e:  # noqa: F841
             traceback.print_exc(file=self._lfh)
             return False
 
+    def xmlCheckOp(self, **kwArgs):
+        """ Performs PDBML XML check on PDBx format input file and returns a text check report.
+        """
+        try:
+            (inpObjD, outObjD, _uD, _pD) = self._getArgs(kwArgs)
+            pdbxPath = inpObjD["src"].getFilePathReference()
+            (_dir, fileName) = os.path.split(pdbxPath)
+
+            reportPath = outObjD["dst"].getFilePathReference()
+            dirPath = outObjD["dst"].getDirPathReference()
+            logPath = os.path.join(dirPath, "cif2pdbx-next.log")
+            expPath = os.path.join(dirPath, fileName + "_model-next_P1.cif")
+            #
+            cI = ConfigInfo()
+            siteId = cI.get("SITE_PREFIX")
+            dp = RcsbDpUtility(tmpPath=dirPath, siteId=siteId, verbose=self._verbose, log=self._lfh)
+            dp.imp(pdbxPath)
+            dp.addInput(name="destination", value="archive_next")
+            dp.op("cif2pdbx-ext")
+
+            dp.expLog(logPath)
+            dp.exp(expPath)
+            if self.__cleanUp:
+                dp.cleanup()
+            #
+            if os.access(expPath, os.R_OK):
+                xmlPath = self.__generateXMLFile(siteId, expPath, dirPath)
+                os.remove(expPath)
+                if xmlPath:
+                    self.__checkXMLFile(siteId, xmlPath, dirPath, reportPath, "annot-check-xml-xmllint")
+                    self.__checkXMLFile(siteId, xmlPath, dirPath, reportPath, "annot-check-xml-stdinparse")
+                    if self._verbose:
+                        self._lfh.write("+AnnotationUtils.dictCheckOp() - PDBx input  file path:  %s\n" % pdbxPath)
+                        self._lfh.write("+AnnotationUtils.dictCheckOp() - Report file path:       %s\n" % reportPath)
+                    #
+                    os.remove(xmlPath)
+                    return True
+                #
+            #
+            return False
+        except Exception as _e:  # noqa: F841
+            traceback.print_exc(file=self._lfh)
+            return False
+        #
+
+    def __generateXMLFile(self, siteId, pdbxPath, dirPath):
+        """ Generate noatom xml file
+        """
+        try:
+            xmlPath = pdbxPath + ".xml-noatom"
+            outputList = []
+            outputList.append(xmlPath)
+            outputList.append(os.path.join(dirPath, "generate_xml_v5.log"))
+            outputList.append(os.path.join(dirPath, "generate_xml_command_v5.log"))
+            for filePath in outputList:
+                if os.access(filePath, os.R_OK):
+                    os.remove(filePath)
+                #
+            #
+            dp = RcsbDpUtility(tmpPath=dirPath, siteId=siteId, verbose=self._verbose, log=self._lfh)
+            dp.imp(pdbxPath)
+            dp.op("annot-public-pdbx-to-xml-noatom")
+            dp.expList(outputList)
+            #
+            if self.__cleanUp:
+                dp.cleanup()
+            #
+            if os.access(xmlPath, os.R_OK):
+                return xmlPath
+            #
+        except:  # noqa: E722 pylint: disable=bare-except
+            traceback.print_exc(file=self._lfh)
+        #
+        return None
+
+    def __checkXMLFile(self, siteId, xmlPath, dirPath, reportPath, op):
+        """ Check noatom xml file
+        """
+        try:
+            if op == "annot-check-xml-xmllint":
+                statinfo = os.stat(xmlPath)
+                if statinfo.st_size > 100000000:
+                    return
+                #
+            #
+            inReportPath = os.path.join(dirPath, "check-xml.diag.txt")
+            if os.access(inReportPath, os.R_OK):
+                os.remove(inReportPath)
+            #
+            outputList = []
+            outputList.append(inReportPath)
+            #
+            dp = RcsbDpUtility(tmpPath=dirPath, siteId=siteId, verbose=self._verbose, log=self._lfh)
+            dp.imp(xmlPath)
+            dp.op(op)
+            dp.expList(outputList)
+            #
+            if os.access(inReportPath, os.R_OK):
+                ith = open(inReportPath, "r")
+                data = ith.read()
+                ith.close()
+                if len(data) > 0:
+                    oth = open(reportPath, "a")
+                    for line in data.split("\n"):
+                        strip_line = line.strip()
+                        if (strip_line == "") or (strip_line == "input_file_1 validates") or strip_line.startswith("stdin:"):
+                            continue
+                        elif strip_line.startswith("input_file_1:") or strip_line.startswith("input_file_1 "):
+                            oth.write("%s\n" % strip_line[13:])
+                        else:
+                            oth.write("%s\n" % strip_line)
+                        #
+                    #
+                    oth.close()
+                #
+                os.remove(inReportPath)
+            #
+            if self.__cleanUp:
+                dp.cleanup()
+            #
+        except:  # noqa: E722 pylint: disable=bare-except
+            traceback.print_exc(file=self._lfh)
+        #
+
     def dictCheckFirstOp(self, **kwArgs):
         """Performs PDBx dictionary check on the first block of a PDBx format input file
         and returns a text check report.
         """
         try:
             (inpObjD, outObjD, _uD, _pD) = self._getArgs(kwArgs)
             pdbxPath = inpObjD["src"].getFilePathReference()
@@ -1262,14 +1387,35 @@
 
             # Always return true - even if no work done
             return True
         except Exception as _e:  # noqa: F841
             traceback.print_exc(file=self._lfh)
             return False
 
+    def emMapCheckOp(self, **kwArgs):
+        """Checks em_map category"""
+        try:
+            (inpObjD, outObjD, _uD, _pD) = self._getArgs(kwArgs)
+            pdbxPath = inpObjD["src"].getFilePathReference()
+            depDataSetId = inpObjD["src"].getDepositionDataSetId()
+            #
+            reportPath = outObjD["dst"].getFilePathReference()
+            dirPath = outObjD["dst"].getDirPathReference()
+            #
+            cI = ConfigInfo()
+            siteId = cI.get("SITE_PREFIX")
+            #
+            checkTask = EmMapCheckTask(siteId=siteId, sessionPath=dirPath, verbose=self._verbose, log=self._lfh)
+            checkTask.run(depDataSetId, pdbxPath, reportPath)
+            # Always return true - even if no work done
+            return True
+        except Exception as _e:  # noqa: F841
+            traceback.print_exc(file=self._lfh)
+            return False
+
     def emVolumeBcifConversionOp(self, **kwArgs):
         """
         converts EM volume from map format into bcif
         :param kwArgs:
         :return bool: True if worked, False if failed
         """
         try:
```

### Comparing `wwpdb.utils.wf-0.33/wwpdb/utils/wf/plugins/ChemCompUtils.py` & `wwpdb.utils.wf-0.34/wwpdb/utils/wf/plugins/ChemCompUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.33/wwpdb/utils/wf/plugins/DictUtils.py` & `wwpdb.utils.wf-0.34/wwpdb/utils/wf/plugins/DictUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.33/wwpdb/utils/wf/plugins/DpUtils.py` & `wwpdb.utils.wf-0.34/wwpdb/utils/wf/plugins/DpUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.33/wwpdb/utils/wf/plugins/EmUtils.py` & `wwpdb.utils.wf-0.34/wwpdb/utils/wf/plugins/EmUtils.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,14 +166,44 @@
             if self.__cleanUp:
                 dp.cleanup()
             return True
         except Exception as _e:  # noqa: F841
             traceback.print_exc(file=self._lfh)
             return False
 
+    def emmapcheck(self, **kwArgs):
+        """Run EM Map/Model validation on file upload"""
+        try:
+            (inpObjD, outObjD, _uD, _pD) = self._getArgs(kwArgs)
+            in_map_file = inpObjD["src1"].getFilePathReference()
+            in_model_file = inpObjD["src2"].getFilePathReference()
+            output_file = outObjD["dst"].getFilePathReference()
+            #
+            cI = ConfigInfo()
+            siteId = cI.get("SITE_PREFIX")
+            dp = RcsbDpUtility(tmpPath=output_file, siteId=siteId, verbose=self._verbose, log=self._lfh)
+            dp.setDebugMode(flag=True)
+
+            dp.addInput(name="input_map_file_path", value=in_map_file)
+            dp.addInput(name="input_model_file_path", value=in_model_file)
+            dp.addInput(name="output_file_path", value=output_file)
+            dp.op("em-map-model-upload-check")
+
+            if self._verbose:
+                self._lfh.write("+EmUtils.emmapcheck() - input map  file path:  %s\n" % in_map_file)
+                self._lfh.write("+EmUtils.emmapcheck() - input model  file path:  %s\n" % in_model_file)
+                self._lfh.write("+EmUtils.emmapcheck() - output json file path:  %s\n" % output_file)
+
+            if self.__cleanUp:
+                dp.cleanup()
+            return True
+        except Exception as _e:  # noqa: F841
+            traceback.print_exc(file=self._lfh)
+            return False
+
     def em2emSpiderOp(self, **kwArgs):
         """Run em2em to convert Spider map to CCP4 format"""
         try:
             (inpObjD, outObjD, uD, _pD) = self._getArgs(kwArgs)
             inpMapPath = inpObjD["src"].getFilePathReference()
             outMapPath = outObjD["dst1"].getFilePathReference()
             dirPath = outObjD["dst1"].getDirPathReference()
```

### Comparing `wwpdb.utils.wf-0.33/wwpdb/utils/wf/plugins/FileUtils.py` & `wwpdb.utils.wf-0.34/wwpdb/utils/wf/plugins/FileUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.33/wwpdb/utils/wf/plugins/FormatUtils.py` & `wwpdb.utils.wf-0.34/wwpdb/utils/wf/plugins/FormatUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.33/wwpdb/utils/wf/plugins/NmrUtils.py` & `wwpdb.utils.wf-0.34/wwpdb/utils/wf/plugins/NmrUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.33/wwpdb/utils/wf/plugins/PdbxUtils.py` & `wwpdb.utils.wf-0.34/wwpdb/utils/wf/plugins/PdbxUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.33/wwpdb/utils/wf/plugins/PrdSearchUtils.py` & `wwpdb.utils.wf-0.34/wwpdb/utils/wf/plugins/PrdSearchUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.33/wwpdb/utils/wf/plugins/ReportUtils.py` & `wwpdb.utils.wf-0.34/wwpdb/utils/wf/plugins/ReportUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.33/wwpdb/utils/wf/plugins/SFConvert.py` & `wwpdb.utils.wf-0.34/wwpdb/utils/wf/plugins/SFConvert.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.33/wwpdb/utils/wf/plugins/SeqStatsUtils.py` & `wwpdb.utils.wf-0.34/wwpdb/utils/wf/plugins/SeqStatsUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.33/wwpdb/utils/wf/plugins/SeqdbUtils.py` & `wwpdb.utils.wf-0.34/wwpdb/utils/wf/plugins/SeqdbUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.33/wwpdb/utils/wf/plugins/UtilsBase.py` & `wwpdb.utils.wf-0.34/wwpdb/utils/wf/plugins/UtilsBase.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.33/wwpdb/utils/wf/plugins/ValidationUtils.py` & `wwpdb.utils.wf-0.34/wwpdb/utils/wf/plugins/ValidationUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.33/wwpdb/utils/wf/process/ActionRegistry.py` & `wwpdb.utils.wf-0.34/wwpdb/utils/wf/process/ActionRegistry.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.33/wwpdb/utils/wf/process/ActionRegistryIo.py` & `wwpdb.utils.wf-0.34/wwpdb/utils/wf/process/ActionRegistryIo.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.33/wwpdb/utils/wf/process/ProcessRunner.py` & `wwpdb.utils.wf-0.34/wwpdb/utils/wf/process/ProcessRunner.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.33/wwpdb/utils/wf/schema/WfSchemaMap.py` & `wwpdb.utils.wf-0.34/wwpdb/utils/wf/schema/WfSchemaMap.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.33/wwpdb/utils/wf/schema/database_descriptions.txt` & `wwpdb.utils.wf-0.34/wwpdb/utils/wf/schema/database_descriptions.txt`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.33/wwpdb.utils.wf.egg-info/PKG-INFO` & `wwpdb.utils.wf-0.34/wwpdb.utils.wf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.utils.wf
-Version: 0.33
+Version: 0.34
 Summary: OneDep WF status DB access utilities
 Home-page: https://github.com/rcsb/py-wwpdb_utils_wf
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.utils.wf-0.33/wwpdb.utils.wf.egg-info/SOURCES.txt` & `wwpdb.utils.wf-0.34/wwpdb.utils.wf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

