# Comparing `tmp/c3-data-transfer-tool-jackdedobb-1.1.24.tar.gz` & `tmp/c3-data-transfer-tool-jackdedobb-1.1.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "c3-data-transfer-tool-jackdedobb-1.1.24.tar", last modified: Tue Jun 13 18:31:07 2023, max compression
+gzip compressed data, was "c3-data-transfer-tool-jackdedobb-1.1.25.tar", last modified: Tue Jun 13 18:34:40 2023, max compression
```

## Comparing `c3-data-transfer-tool-jackdedobb-1.1.24.tar` & `c3-data-transfer-tool-jackdedobb-1.1.25.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 jacksondedobbelaere   (501) staff       (20)        0 2023-06-13 18:31:07.424018 c3-data-transfer-tool-jackdedobb-1.1.24/
--rw-r--r--   0 jacksondedobbelaere   (501) staff       (20)    35148 2022-11-17 23:12:47.000000 c3-data-transfer-tool-jackdedobb-1.1.24/LICENSE
--rw-r--r--   0 jacksondedobbelaere   (501) staff       (20)    12542 2023-06-13 18:31:07.424187 c3-data-transfer-tool-jackdedobb-1.1.24/PKG-INFO
--rw-r--r--   0 jacksondedobbelaere   (501) staff       (20)    11998 2022-12-08 21:51:48.000000 c3-data-transfer-tool-jackdedobb-1.1.24/README.md
--rw-r--r--   0 jacksondedobbelaere   (501) staff       (20)      100 2022-11-17 23:12:47.000000 c3-data-transfer-tool-jackdedobb-1.1.24/pyproject.toml
--rw-r--r--   0 jacksondedobbelaere   (501) staff       (20)      719 2023-06-13 18:31:07.425054 c3-data-transfer-tool-jackdedobb-1.1.24/setup.cfg
-drwxr-xr-x   0 jacksondedobbelaere   (501) staff       (20)        0 2023-06-13 18:31:07.412107 c3-data-transfer-tool-jackdedobb-1.1.24/src/
-drwxr-xr-x   0 jacksondedobbelaere   (501) staff       (20)        0 2023-06-13 18:31:07.415005 c3-data-transfer-tool-jackdedobb-1.1.24/src/c3DataMigration/
--rw-r--r--   0 jacksondedobbelaere   (501) staff       (20)        0 2022-11-17 23:12:47.000000 c3-data-transfer-tool-jackdedobb-1.1.24/src/c3DataMigration/__init__.py
--rw-r--r--   0 jacksondedobbelaere   (501) staff       (20)     6869 2022-11-17 23:12:47.000000 c3-data-transfer-tool-jackdedobb-1.1.24/src/c3DataMigration/c3DataTransfer.py
-drwxr-xr-x   0 jacksondedobbelaere   (501) staff       (20)        0 2023-06-13 18:31:07.418765 c3-data-transfer-tool-jackdedobb-1.1.24/src/c3DataMigration/c3Helpers/
--rw-r--r--   0 jacksondedobbelaere   (501) staff       (20)        0 2022-11-17 23:12:47.000000 c3-data-transfer-tool-jackdedobb-1.1.24/src/c3DataMigration/c3Helpers/__init__.py
--rw-r--r--   0 jacksondedobbelaere   (501) staff       (20)     4734 2023-02-22 06:18:58.000000 c3-data-transfer-tool-jackdedobb-1.1.24/src/c3DataMigration/c3Helpers/c3BatchJobs.py
--rw-r--r--   0 jacksondedobbelaere   (501) staff       (20)     7586 2022-11-17 23:12:47.000000 c3-data-transfer-tool-jackdedobb-1.1.24/src/c3DataMigration/c3Helpers/c3FileSystem.py
--rw-r--r--   0 jacksondedobbelaere   (501) staff       (20)     5298 2022-11-17 23:12:47.000000 c3-data-transfer-tool-jackdedobb-1.1.24/src/c3DataMigration/c3Helpers/c3PythonClasses.py
--rw-r--r--   0 jacksondedobbelaere   (501) staff       (20)     3065 2022-11-17 23:12:47.000000 c3-data-transfer-tool-jackdedobb-1.1.24/src/c3DataMigration/c3Helpers/c3Queues.py
--rw-r--r--   0 jacksondedobbelaere   (501) staff       (20)     5214 2022-11-17 23:12:47.000000 c3-data-transfer-tool-jackdedobb-1.1.24/src/c3DataMigration/c3Helpers/c3Request.py
--rw-r--r--   0 jacksondedobbelaere   (501) staff       (20)     6140 2022-11-17 23:12:47.000000 c3-data-transfer-tool-jackdedobb-1.1.24/src/c3DataMigration/c3Helpers/c3UsageStats.py
--rw-r--r--   0 jacksondedobbelaere   (501) staff       (20)     5150 2022-11-17 23:12:47.000000 c3-data-transfer-tool-jackdedobb-1.1.24/src/c3DataMigration/c3Helpers/c3UtilityMethods.py
-drwxr-xr-x   0 jacksondedobbelaere   (501) staff       (20)        0 2023-06-13 18:31:07.421154 c3-data-transfer-tool-jackdedobb-1.1.24/src/c3DataMigration/c3MigrationMethods/
--rw-r--r--   0 jacksondedobbelaere   (501) staff       (20)        0 2022-11-17 23:12:47.000000 c3-data-transfer-tool-jackdedobb-1.1.24/src/c3DataMigration/c3MigrationMethods/__init__.py
--rw-r--r--   0 jacksondedobbelaere   (501) staff       (20)     6488 2023-02-22 06:18:58.000000 c3-data-transfer-tool-jackdedobb-1.1.24/src/c3DataMigration/c3MigrationMethods/c3DataDownload.py
--rw-r--r--   0 jacksondedobbelaere   (501) staff       (20)     2562 2023-02-22 06:18:58.000000 c3-data-transfer-tool-jackdedobb-1.1.24/src/c3DataMigration/c3MigrationMethods/c3DataRefreshCalcFields.py
--rw-r--r--   0 jacksondedobbelaere   (501) staff       (20)     4400 2022-11-17 23:12:47.000000 c3-data-transfer-tool-jackdedobb-1.1.24/src/c3DataMigration/c3MigrationMethods/c3DataRemove.py
--rw-r--r--   0 jacksondedobbelaere   (501) staff       (20)     5128 2023-02-22 06:18:58.000000 c3-data-transfer-tool-jackdedobb-1.1.24/src/c3DataMigration/c3MigrationMethods/c3DataUpload.py
-drwxr-xr-x   0 jacksondedobbelaere   (501) staff       (20)        0 2023-06-13 18:31:07.423676 c3-data-transfer-tool-jackdedobb-1.1.24/src/c3_data_transfer_tool_jackdedobb.egg-info/
--rw-r--r--   0 jacksondedobbelaere   (501) staff       (20)    12542 2023-06-13 18:31:07.000000 c3-data-transfer-tool-jackdedobb-1.1.24/src/c3_data_transfer_tool_jackdedobb.egg-info/PKG-INFO
--rw-r--r--   0 jacksondedobbelaere   (501) staff       (20)     1058 2023-06-13 18:31:07.000000 c3-data-transfer-tool-jackdedobb-1.1.24/src/c3_data_transfer_tool_jackdedobb.egg-info/SOURCES.txt
--rw-r--r--   0 jacksondedobbelaere   (501) staff       (20)        1 2023-06-13 18:31:07.000000 c3-data-transfer-tool-jackdedobb-1.1.24/src/c3_data_transfer_tool_jackdedobb.egg-info/dependency_links.txt
--rw-r--r--   0 jacksondedobbelaere   (501) staff       (20)       31 2023-06-13 18:31:07.000000 c3-data-transfer-tool-jackdedobb-1.1.24/src/c3_data_transfer_tool_jackdedobb.egg-info/requires.txt
--rw-r--r--   0 jacksondedobbelaere   (501) staff       (20)       16 2023-06-13 18:31:07.000000 c3-data-transfer-tool-jackdedobb-1.1.24/src/c3_data_transfer_tool_jackdedobb.egg-info/top_level.txt
+drwxr-xr-x   0 jacksondedobbelaere   (501) staff       (20)        0 2023-06-13 18:34:40.402490 c3-data-transfer-tool-jackdedobb-1.1.25/
+-rw-r--r--   0 jacksondedobbelaere   (501) staff       (20)    35148 2022-11-17 23:12:47.000000 c3-data-transfer-tool-jackdedobb-1.1.25/LICENSE
+-rw-r--r--   0 jacksondedobbelaere   (501) staff       (20)    12542 2023-06-13 18:34:40.402775 c3-data-transfer-tool-jackdedobb-1.1.25/PKG-INFO
+-rw-r--r--   0 jacksondedobbelaere   (501) staff       (20)    11998 2022-12-08 21:51:48.000000 c3-data-transfer-tool-jackdedobb-1.1.25/README.md
+-rw-r--r--   0 jacksondedobbelaere   (501) staff       (20)      100 2022-11-17 23:12:47.000000 c3-data-transfer-tool-jackdedobb-1.1.25/pyproject.toml
+-rw-r--r--   0 jacksondedobbelaere   (501) staff       (20)      719 2023-06-13 18:34:40.404085 c3-data-transfer-tool-jackdedobb-1.1.25/setup.cfg
+drwxr-xr-x   0 jacksondedobbelaere   (501) staff       (20)        0 2023-06-13 18:34:40.393086 c3-data-transfer-tool-jackdedobb-1.1.25/src/
+drwxr-xr-x   0 jacksondedobbelaere   (501) staff       (20)        0 2023-06-13 18:34:40.394805 c3-data-transfer-tool-jackdedobb-1.1.25/src/c3DataMigration/
+-rw-r--r--   0 jacksondedobbelaere   (501) staff       (20)        0 2022-11-17 23:12:47.000000 c3-data-transfer-tool-jackdedobb-1.1.25/src/c3DataMigration/__init__.py
+-rw-r--r--   0 jacksondedobbelaere   (501) staff       (20)     6869 2022-11-17 23:12:47.000000 c3-data-transfer-tool-jackdedobb-1.1.25/src/c3DataMigration/c3DataTransfer.py
+drwxr-xr-x   0 jacksondedobbelaere   (501) staff       (20)        0 2023-06-13 18:34:40.397329 c3-data-transfer-tool-jackdedobb-1.1.25/src/c3DataMigration/c3Helpers/
+-rw-r--r--   0 jacksondedobbelaere   (501) staff       (20)        0 2022-11-17 23:12:47.000000 c3-data-transfer-tool-jackdedobb-1.1.25/src/c3DataMigration/c3Helpers/__init__.py
+-rw-r--r--   0 jacksondedobbelaere   (501) staff       (20)     4734 2023-02-22 06:18:58.000000 c3-data-transfer-tool-jackdedobb-1.1.25/src/c3DataMigration/c3Helpers/c3BatchJobs.py
+-rw-r--r--   0 jacksondedobbelaere   (501) staff       (20)     7586 2022-11-17 23:12:47.000000 c3-data-transfer-tool-jackdedobb-1.1.25/src/c3DataMigration/c3Helpers/c3FileSystem.py
+-rw-r--r--   0 jacksondedobbelaere   (501) staff       (20)     5319 2023-06-13 18:33:42.000000 c3-data-transfer-tool-jackdedobb-1.1.25/src/c3DataMigration/c3Helpers/c3PythonClasses.py
+-rw-r--r--   0 jacksondedobbelaere   (501) staff       (20)     3065 2022-11-17 23:12:47.000000 c3-data-transfer-tool-jackdedobb-1.1.25/src/c3DataMigration/c3Helpers/c3Queues.py
+-rw-r--r--   0 jacksondedobbelaere   (501) staff       (20)     5214 2022-11-17 23:12:47.000000 c3-data-transfer-tool-jackdedobb-1.1.25/src/c3DataMigration/c3Helpers/c3Request.py
+-rw-r--r--   0 jacksondedobbelaere   (501) staff       (20)     6140 2022-11-17 23:12:47.000000 c3-data-transfer-tool-jackdedobb-1.1.25/src/c3DataMigration/c3Helpers/c3UsageStats.py
+-rw-r--r--   0 jacksondedobbelaere   (501) staff       (20)     5150 2022-11-17 23:12:47.000000 c3-data-transfer-tool-jackdedobb-1.1.25/src/c3DataMigration/c3Helpers/c3UtilityMethods.py
+drwxr-xr-x   0 jacksondedobbelaere   (501) staff       (20)        0 2023-06-13 18:34:40.399492 c3-data-transfer-tool-jackdedobb-1.1.25/src/c3DataMigration/c3MigrationMethods/
+-rw-r--r--   0 jacksondedobbelaere   (501) staff       (20)        0 2022-11-17 23:12:47.000000 c3-data-transfer-tool-jackdedobb-1.1.25/src/c3DataMigration/c3MigrationMethods/__init__.py
+-rw-r--r--   0 jacksondedobbelaere   (501) staff       (20)     6488 2023-02-22 06:18:58.000000 c3-data-transfer-tool-jackdedobb-1.1.25/src/c3DataMigration/c3MigrationMethods/c3DataDownload.py
+-rw-r--r--   0 jacksondedobbelaere   (501) staff       (20)     2562 2023-02-22 06:18:58.000000 c3-data-transfer-tool-jackdedobb-1.1.25/src/c3DataMigration/c3MigrationMethods/c3DataRefreshCalcFields.py
+-rw-r--r--   0 jacksondedobbelaere   (501) staff       (20)     4400 2022-11-17 23:12:47.000000 c3-data-transfer-tool-jackdedobb-1.1.25/src/c3DataMigration/c3MigrationMethods/c3DataRemove.py
+-rw-r--r--   0 jacksondedobbelaere   (501) staff       (20)     5128 2023-02-22 06:18:58.000000 c3-data-transfer-tool-jackdedobb-1.1.25/src/c3DataMigration/c3MigrationMethods/c3DataUpload.py
+drwxr-xr-x   0 jacksondedobbelaere   (501) staff       (20)        0 2023-06-13 18:34:40.402043 c3-data-transfer-tool-jackdedobb-1.1.25/src/c3_data_transfer_tool_jackdedobb.egg-info/
+-rw-r--r--   0 jacksondedobbelaere   (501) staff       (20)    12542 2023-06-13 18:34:40.000000 c3-data-transfer-tool-jackdedobb-1.1.25/src/c3_data_transfer_tool_jackdedobb.egg-info/PKG-INFO
+-rw-r--r--   0 jacksondedobbelaere   (501) staff       (20)     1058 2023-06-13 18:34:40.000000 c3-data-transfer-tool-jackdedobb-1.1.25/src/c3_data_transfer_tool_jackdedobb.egg-info/SOURCES.txt
+-rw-r--r--   0 jacksondedobbelaere   (501) staff       (20)        1 2023-06-13 18:34:40.000000 c3-data-transfer-tool-jackdedobb-1.1.25/src/c3_data_transfer_tool_jackdedobb.egg-info/dependency_links.txt
+-rw-r--r--   0 jacksondedobbelaere   (501) staff       (20)       31 2023-06-13 18:34:40.000000 c3-data-transfer-tool-jackdedobb-1.1.25/src/c3_data_transfer_tool_jackdedobb.egg-info/requires.txt
+-rw-r--r--   0 jacksondedobbelaere   (501) staff       (20)       16 2023-06-13 18:34:40.000000 c3-data-transfer-tool-jackdedobb-1.1.25/src/c3_data_transfer_tool_jackdedobb.egg-info/top_level.txt
```

### Comparing `c3-data-transfer-tool-jackdedobb-1.1.24/LICENSE` & `c3-data-transfer-tool-jackdedobb-1.1.25/LICENSE`

 * *Files identical despite different names*

### Comparing `c3-data-transfer-tool-jackdedobb-1.1.24/PKG-INFO` & `c3-data-transfer-tool-jackdedobb-1.1.25/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: c3-data-transfer-tool-jackdedobb
-Version: 1.1.24
+Version: 1.1.25
 Summary: Tool to help extracting and uploading data to C3 environments.
 Home-page: https://github.com/c3-e/c3open/tools/jack-transfer-tool
 Author: Jackson DeDobbelaere
 Author-email: jackson.dedobbelaere@c3.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `c3-data-transfer-tool-jackdedobb-1.1.24/README.md` & `c3-data-transfer-tool-jackdedobb-1.1.25/README.md`

 * *Files identical despite different names*

### Comparing `c3-data-transfer-tool-jackdedobb-1.1.24/setup.cfg` & `c3-data-transfer-tool-jackdedobb-1.1.25/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = c3-data-transfer-tool-jackdedobb
-version = 1.1.24
+version = 1.1.25
 author = Jackson DeDobbelaere
 author_email = jackson.dedobbelaere@c3.ai
 description = Tool to help extracting and uploading data to C3 environments.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/c3-e/c3open/tools/jack-transfer-tool
 classifiers =
```

### Comparing `c3-data-transfer-tool-jackdedobb-1.1.24/src/c3DataMigration/c3DataTransfer.py` & `c3-data-transfer-tool-jackdedobb-1.1.25/src/c3DataMigration/c3DataTransfer.py`

 * *Files identical despite different names*

### Comparing `c3-data-transfer-tool-jackdedobb-1.1.24/src/c3DataMigration/c3Helpers/c3BatchJobs.py` & `c3-data-transfer-tool-jackdedobb-1.1.25/src/c3DataMigration/c3Helpers/c3BatchJobs.py`

 * *Files identical despite different names*

### Comparing `c3-data-transfer-tool-jackdedobb-1.1.24/src/c3DataMigration/c3Helpers/c3FileSystem.py` & `c3-data-transfer-tool-jackdedobb-1.1.25/src/c3DataMigration/c3Helpers/c3FileSystem.py`

 * *Files identical despite different names*

### Comparing `c3-data-transfer-tool-jackdedobb-1.1.24/src/c3DataMigration/c3Helpers/c3PythonClasses.py` & `c3-data-transfer-tool-jackdedobb-1.1.25/src/c3DataMigration/c3Helpers/c3PythonClasses.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 
 
 
 @dataclass(frozen=True)
 class APIParameters:
   # Common
-  environmentArguments:     Namespace = Namespace()
+  environmentArguments:     Namespace = field(default_factory=Namespace)
   errorOutputFolder:        str = ''
   batchSize:                int = 250
   priority:                 int = 0
   errorSleepTimeSeconds:    int = 15
   refreshPollTimeSeconds:   int = 15
   masterRefreshDataSwitch:  bool = True
   maxColumnPrintLength:     int = 150
```

### Comparing `c3-data-transfer-tool-jackdedobb-1.1.24/src/c3DataMigration/c3Helpers/c3Queues.py` & `c3-data-transfer-tool-jackdedobb-1.1.25/src/c3DataMigration/c3Helpers/c3Queues.py`

 * *Files identical despite different names*

### Comparing `c3-data-transfer-tool-jackdedobb-1.1.24/src/c3DataMigration/c3Helpers/c3Request.py` & `c3-data-transfer-tool-jackdedobb-1.1.25/src/c3DataMigration/c3Helpers/c3Request.py`

 * *Files identical despite different names*

### Comparing `c3-data-transfer-tool-jackdedobb-1.1.24/src/c3DataMigration/c3Helpers/c3UsageStats.py` & `c3-data-transfer-tool-jackdedobb-1.1.25/src/c3DataMigration/c3Helpers/c3UsageStats.py`

 * *Files identical despite different names*

### Comparing `c3-data-transfer-tool-jackdedobb-1.1.24/src/c3DataMigration/c3Helpers/c3UtilityMethods.py` & `c3-data-transfer-tool-jackdedobb-1.1.25/src/c3DataMigration/c3Helpers/c3UtilityMethods.py`

 * *Files identical despite different names*

### Comparing `c3-data-transfer-tool-jackdedobb-1.1.24/src/c3DataMigration/c3MigrationMethods/c3DataDownload.py` & `c3-data-transfer-tool-jackdedobb-1.1.25/src/c3DataMigration/c3MigrationMethods/c3DataDownload.py`

 * *Files identical despite different names*

### Comparing `c3-data-transfer-tool-jackdedobb-1.1.24/src/c3DataMigration/c3MigrationMethods/c3DataRefreshCalcFields.py` & `c3-data-transfer-tool-jackdedobb-1.1.25/src/c3DataMigration/c3MigrationMethods/c3DataRefreshCalcFields.py`

 * *Files identical despite different names*

### Comparing `c3-data-transfer-tool-jackdedobb-1.1.24/src/c3DataMigration/c3MigrationMethods/c3DataRemove.py` & `c3-data-transfer-tool-jackdedobb-1.1.25/src/c3DataMigration/c3MigrationMethods/c3DataRemove.py`

 * *Files identical despite different names*

### Comparing `c3-data-transfer-tool-jackdedobb-1.1.24/src/c3DataMigration/c3MigrationMethods/c3DataUpload.py` & `c3-data-transfer-tool-jackdedobb-1.1.25/src/c3DataMigration/c3MigrationMethods/c3DataUpload.py`

 * *Files identical despite different names*

### Comparing `c3-data-transfer-tool-jackdedobb-1.1.24/src/c3_data_transfer_tool_jackdedobb.egg-info/PKG-INFO` & `c3-data-transfer-tool-jackdedobb-1.1.25/src/c3_data_transfer_tool_jackdedobb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: c3-data-transfer-tool-jackdedobb
-Version: 1.1.24
+Version: 1.1.25
 Summary: Tool to help extracting and uploading data to C3 environments.
 Home-page: https://github.com/c3-e/c3open/tools/jack-transfer-tool
 Author: Jackson DeDobbelaere
 Author-email: jackson.dedobbelaere@c3.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `c3-data-transfer-tool-jackdedobb-1.1.24/src/c3_data_transfer_tool_jackdedobb.egg-info/SOURCES.txt` & `c3-data-transfer-tool-jackdedobb-1.1.25/src/c3_data_transfer_tool_jackdedobb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

