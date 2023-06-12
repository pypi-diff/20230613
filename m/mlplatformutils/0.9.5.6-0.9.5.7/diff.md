# Comparing `tmp/mlplatformutils-0.9.5.6.tar.gz` & `tmp/mlplatformutils-0.9.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mlplatformutils-0.9.5.6.tar", last modified: Mon Jun 12 23:43:46 2023, max compression
+gzip compressed data, was "dist\mlplatformutils-0.9.5.7.tar", last modified: Mon Jun 12 23:54:26 2023, max compression
```

## Comparing `mlplatformutils-0.9.5.6.tar` & `mlplatformutils-0.9.5.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 23:43:46.027120 mlplatformutils-0.9.5.6/
--rw-rw-rw-   0        0        0     6719 2023-06-12 23:43:46.028120 mlplatformutils-0.9.5.6/PKG-INFO
--rw-rw-rw-   0        0        0      420 2023-06-04 22:07:41.000000 mlplatformutils-0.9.5.6/README.rst
--rw-rw-rw-   0        0        0      115 2023-06-12 23:43:46.036653 mlplatformutils-0.9.5.6/setup.cfg
--rw-rw-rw-   0        0        0      825 2023-06-12 23:43:34.000000 mlplatformutils-0.9.5.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-12 23:43:45.591922 mlplatformutils-0.9.5.6/src/
-drwxrwxrwx   0        0        0        0 2023-06-12 23:43:45.639466 mlplatformutils-0.9.5.6/src/mlplatformutils/
--rw-rw-rw-   0        0        0        0 2023-06-04 21:52:02.000000 mlplatformutils-0.9.5.6/src/mlplatformutils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 23:43:46.025119 mlplatformutils-0.9.5.6/src/mlplatformutils/core/
--rw-rw-rw-   0        0        0        0 2023-06-03 20:39:09.000000 mlplatformutils-0.9.5.6/src/mlplatformutils/core/__init__.py
--rw-rw-rw-   0        0        0     5868 2023-06-03 20:42:19.000000 mlplatformutils-0.9.5.6/src/mlplatformutils/core/app_insights_logger.py
--rw-rw-rw-   0        0        0     1418 2023-06-12 20:54:48.000000 mlplatformutils-0.9.5.6/src/mlplatformutils/core/freshnessutils.py
--rw-rw-rw-   0        0        0    10096 2023-06-12 23:17:29.000000 mlplatformutils-0.9.5.6/src/mlplatformutils/core/lineagegraph.py
--rw-rw-rw-   0        0        0     6140 2023-06-08 20:01:59.000000 mlplatformutils-0.9.5.6/src/mlplatformutils/core/pandascoreutils.py
--rw-rw-rw-   0        0        0    12539 2023-06-12 23:43:27.000000 mlplatformutils-0.9.5.6/src/mlplatformutils/core/pandasutils.py
--rw-rw-rw-   0        0        0     3129 2023-06-04 21:06:24.000000 mlplatformutils-0.9.5.6/src/mlplatformutils/core/platformutils.py
--rw-rw-rw-   0        0        0     4675 2023-06-08 20:00:19.000000 mlplatformutils-0.9.5.6/src/mlplatformutils/core/sparkcoreutils.py
--rw-rw-rw-   0        0        0    10174 2023-06-12 23:42:09.000000 mlplatformutils-0.9.5.6/src/mlplatformutils/core/sparkutils.py
--rw-rw-rw-   0        0        0       23 2023-06-12 23:43:37.000000 mlplatformutils-0.9.5.6/src/mlplatformutils/core/version.py
-drwxrwxrwx   0        0        0        0 2023-06-12 23:43:45.720479 mlplatformutils-0.9.5.6/src/mlplatformutils.egg-info/
--rw-rw-rw-   0        0        0     6719 2023-06-12 23:43:45.000000 mlplatformutils-0.9.5.6/src/mlplatformutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      688 2023-06-12 23:43:45.000000 mlplatformutils-0.9.5.6/src/mlplatformutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 23:43:45.000000 mlplatformutils-0.9.5.6/src/mlplatformutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      103 2023-06-12 23:43:45.000000 mlplatformutils-0.9.5.6/src/mlplatformutils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-12 23:43:45.000000 mlplatformutils-0.9.5.6/src/mlplatformutils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-12 23:54:26.867264 mlplatformutils-0.9.5.7/
+-rw-rw-rw-   0        0        0     6719 2023-06-12 23:54:26.867264 mlplatformutils-0.9.5.7/PKG-INFO
+-rw-rw-rw-   0        0        0      420 2023-06-04 22:07:41.000000 mlplatformutils-0.9.5.7/README.rst
+-rw-rw-rw-   0        0        0      115 2023-06-12 23:54:26.867264 mlplatformutils-0.9.5.7/setup.cfg
+-rw-rw-rw-   0        0        0      825 2023-06-12 23:54:04.000000 mlplatformutils-0.9.5.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 23:54:26.632024 mlplatformutils-0.9.5.7/src/
+drwxrwxrwx   0        0        0        0 2023-06-12 23:54:26.647657 mlplatformutils-0.9.5.7/src/mlplatformutils/
+-rw-rw-rw-   0        0        0        0 2023-06-04 21:52:02.000000 mlplatformutils-0.9.5.7/src/mlplatformutils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 23:54:26.867264 mlplatformutils-0.9.5.7/src/mlplatformutils/core/
+-rw-rw-rw-   0        0        0        0 2023-06-03 20:39:09.000000 mlplatformutils-0.9.5.7/src/mlplatformutils/core/__init__.py
+-rw-rw-rw-   0        0        0     5868 2023-06-03 20:42:19.000000 mlplatformutils-0.9.5.7/src/mlplatformutils/core/app_insights_logger.py
+-rw-rw-rw-   0        0        0     1418 2023-06-12 20:54:48.000000 mlplatformutils-0.9.5.7/src/mlplatformutils/core/freshnessutils.py
+-rw-rw-rw-   0        0        0    10096 2023-06-12 23:17:29.000000 mlplatformutils-0.9.5.7/src/mlplatformutils/core/lineagegraph.py
+-rw-rw-rw-   0        0        0     6140 2023-06-08 20:01:59.000000 mlplatformutils-0.9.5.7/src/mlplatformutils/core/pandascoreutils.py
+-rw-rw-rw-   0        0        0    12811 2023-06-12 23:53:07.000000 mlplatformutils-0.9.5.7/src/mlplatformutils/core/pandasutils.py
+-rw-rw-rw-   0        0        0     3129 2023-06-04 21:06:24.000000 mlplatformutils-0.9.5.7/src/mlplatformutils/core/platformutils.py
+-rw-rw-rw-   0        0        0     4675 2023-06-08 20:00:19.000000 mlplatformutils-0.9.5.7/src/mlplatformutils/core/sparkcoreutils.py
+-rw-rw-rw-   0        0        0    10458 2023-06-12 23:53:54.000000 mlplatformutils-0.9.5.7/src/mlplatformutils/core/sparkutils.py
+-rw-rw-rw-   0        0        0       23 2023-06-12 23:54:07.000000 mlplatformutils-0.9.5.7/src/mlplatformutils/core/version.py
+drwxrwxrwx   0        0        0        0 2023-06-12 23:54:26.710559 mlplatformutils-0.9.5.7/src/mlplatformutils.egg-info/
+-rw-rw-rw-   0        0        0     6719 2023-06-12 23:54:26.000000 mlplatformutils-0.9.5.7/src/mlplatformutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      688 2023-06-12 23:54:26.000000 mlplatformutils-0.9.5.7/src/mlplatformutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 23:54:26.000000 mlplatformutils-0.9.5.7/src/mlplatformutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      103 2023-06-12 23:54:26.000000 mlplatformutils-0.9.5.7/src/mlplatformutils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-12 23:54:26.000000 mlplatformutils-0.9.5.7/src/mlplatformutils.egg-info/top_level.txt
```

### Comparing `mlplatformutils-0.9.5.6/PKG-INFO` & `mlplatformutils-0.9.5.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlplatformutils
-Version: 0.9.5.6
+Version: 0.9.5.7
 Author: Keshav Singh
 Author-email: keshav_singh@hotmail.com
 License: MIT
 Keywords: mlplatformutils
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
```

### Comparing `mlplatformutils-0.9.5.6/setup.py` & `mlplatformutils-0.9.5.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 else:
     long_description="#DESC"
 
 setup(
     name='mlplatformutils',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='0.9.5.6',
+    version='0.9.5.7',
     license='MIT',
     classifiers=[
         'Programming Language :: Python :: 3.8'
     ],
     author='Keshav Singh',
     author_email='keshav_singh@hotmail.com',
     packages=find_packages('src'),
```

### Comparing `mlplatformutils-0.9.5.6/src/mlplatformutils/core/app_insights_logger.py` & `mlplatformutils-0.9.5.7/src/mlplatformutils/core/app_insights_logger.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.9.5.6/src/mlplatformutils/core/freshnessutils.py` & `mlplatformutils-0.9.5.7/src/mlplatformutils/core/freshnessutils.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.9.5.6/src/mlplatformutils/core/lineagegraph.py` & `mlplatformutils-0.9.5.7/src/mlplatformutils/core/lineagegraph.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.9.5.6/src/mlplatformutils/core/pandascoreutils.py` & `mlplatformutils-0.9.5.7/src/mlplatformutils/core/pandascoreutils.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.9.5.6/src/mlplatformutils/core/pandasutils.py` & `mlplatformutils-0.9.5.7/src/mlplatformutils/core/pandasutils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import json
 def get_max_properties_starting_with(id, prefix,dataprop,LineageLogger):
 
-    document=LineageLogger.query_graph("g.V().hasLabel('amlrun').has('id', '"+id+"')")[0]
+    documents=LineageLogger.query_graph("g.V().hasLabel('amlrun').has('id', '"+id+"')")
+    if documents:
+        document = documents[0]
     jsondump = json.dumps(document)
     jsonload = json.loads(jsondump)
     for item in jsonload:
         properties = item.get('properties')
     if properties:
         matching_props = [prop[-1] for prop in properties.keys() if prop.startswith(prefix)]
         max_val = max(int(prop) for prop in matching_props) if matching_props else 0
@@ -30,15 +32,17 @@
         account_name=SOURCE_STORAGE_ACCOUNT_VALUE,\
         client_id=SOURCE_READ_SPN_VALUE,\
         client_secret=SOURCE_READ_SPNKEY_VALUE,\
         tenant_id=tenant_id
     )
     pandas_df = DeltaTable(AML_STORAGE_EXPERIMENT_DELTA_ROOT_PATH, file_system=fs).to_pandas()
 
-    documentId = LineageLogger.query_graph("g.V().hasLabel('amlrun').has('RUN_ID', '"+RUN_ID+"').has('PIPELINE_STEP_NAME', '"+PIPELINE_STEP_NAME+"').values('id')")[0]
+    documentIds = LineageLogger.query_graph("g.V().hasLabel('amlrun').has('RUN_ID', '"+RUN_ID+"').has('PIPELINE_STEP_NAME', '"+PIPELINE_STEP_NAME+"').values('id')")
+    if documentIds:
+        documentId = documentIds[0]
     sourcePostfix,dataprop=get_max_properties_starting_with(documentId,"DataReadSourceColumns","DataReadSource",LineageLogger)
     if dataprop is None:
         dataprop = str({"DataReadSource_"+sourcePostfix: str("https://"+SOURCE_STORAGE_ACCOUNT_VALUE+".dfs.core.windows.net/"+AML_STORAGE_EXPERIMENT_DELTA_ROOT_PATH),\
                                        "Type":"ADLS"})
     else:
         dataprop = str(dataprop)+str(",")+str({"DataReadSource_"+sourcePostfix: str("https://"+SOURCE_STORAGE_ACCOUNT_VALUE+".dfs.core.windows.net/"+AML_STORAGE_EXPERIMENT_DELTA_ROOT_PATH),\
                                        "Type":"ADLS"})
@@ -71,15 +75,17 @@
     
     handler=pyarrowfs_adlgen2.AccountHandler.from_account_name(SOURCE_STORAGE_ACCOUNT_VALUE,credential=credential)
     fs = pyarrow.fs.PyFileSystem(handler)
     #pandas_df = pd.read_parquet(AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH, filesystem=fs , engine="pyarrow")
     #pandas_df = pq.read_table(source=AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH, filesystem=fs, use_legacy_dataset= True).to_pandas()
     pandas_df = pq.ParquetDataset(AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH,filesystem=fs).read().to_pandas()
 
-    documentId = LineageLogger.query_graph("g.V().hasLabel('amlrun').has('RUN_ID', '"+RUN_ID+"').has('PIPELINE_STEP_NAME', '"+PIPELINE_STEP_NAME+"').values('id')")[0]
+    documentIds = LineageLogger.query_graph("g.V().hasLabel('amlrun').has('RUN_ID', '"+RUN_ID+"').has('PIPELINE_STEP_NAME', '"+PIPELINE_STEP_NAME+"').values('id')")
+    if documentIds:
+        documentId = documentIds[0]    
     sourcePostfix,dataprop=get_max_properties_starting_with(documentId,"DataReadSourceColumns","DataReadSource",LineageLogger)
     if dataprop is None:
         dataprop = str({"DataReadSource_"+sourcePostfix: str("https://"+SOURCE_STORAGE_ACCOUNT_VALUE+".dfs.core.windows.net/"+AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH),\
                                        "Type":"ADLS"})
     else:
         dataprop = str(dataprop)+str(",")+str({"DataReadSource_"+sourcePostfix: str("https://"+SOURCE_STORAGE_ACCOUNT_VALUE+".dfs.core.windows.net/"+AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH),\
                                        "Type":"ADLS"})
@@ -143,15 +149,17 @@
     client_id=SOURCE_READ_SPN_VALUE,
     client_secret=SOURCE_READ_SPNKEY_VALUE)
 
     handler=pyarrowfs_adlgen2.AccountHandler.from_account_name(SOURCE_STORAGE_ACCOUNT_VALUE,credential=credential)
     fs = pyarrow.fs.PyFileSystem(handler)
     pandas_df = pq.ParquetDataset(parquet_files_from_path_list,filesystem=fs).read().to_pandas()
 
-    documentId = LineageLogger.query_graph("g.V().hasLabel('amlrun').has('RUN_ID', '"+RUN_ID+"').has('PIPELINE_STEP_NAME', '"+PIPELINE_STEP_NAME+"').values('id')")[0]
+    documentIds = LineageLogger.query_graph("g.V().hasLabel('amlrun').has('RUN_ID', '"+RUN_ID+"').has('PIPELINE_STEP_NAME', '"+PIPELINE_STEP_NAME+"').values('id')")
+    if documentIds:
+        documentId = documentIds[0]    
     sourcePostfix,dataprop=get_max_properties_starting_with(documentId,"DataReadSourceColumns","DataReadSource",LineageLogger)
     if dataprop is None:
         dataprop = str({"DataReadSource_"+sourcePostfix: str("https://"+SOURCE_STORAGE_ACCOUNT_VALUE+".dfs.core.windows.net/"+AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH),\
                                        "Type":"ADLS"})
     else:
         dataprop = str(dataprop)+str(",")+str({"DataReadSource_"+sourcePostfix: str("https://"+SOURCE_STORAGE_ACCOUNT_VALUE+".dfs.core.windows.net/"+AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH),\
                                        "Type":"ADLS"})
@@ -196,15 +204,17 @@
     pyarrow.dataset.write_dataset(
         pyarrow_table,
         AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH,
         format='parquet',
         filesystem=pyarrow.fs.PyFileSystem(handler)
     )
     """
-    documentId = LineageLogger.query_graph("g.V().hasLabel('amlrun').has('RUN_ID', '"+RUN_ID+"').has('PIPELINE_STEP_NAME', '"+PIPELINE_STEP_NAME+"').values('id')")[0]
+    documentIds = LineageLogger.query_graph("g.V().hasLabel('amlrun').has('RUN_ID', '"+RUN_ID+"').has('PIPELINE_STEP_NAME', '"+PIPELINE_STEP_NAME+"').values('id')")
+    if documentIds:
+        documentId = documentIds[0]
     sourcePostfix,dataprop=get_max_properties_starting_with(documentId,"DataWriteColumns","DataWriteTarget",LineageLogger)
 
     if dataprop is None:
         dataprop = str({"DataWriteTarget_"+sourcePostfix: str("https://"+SOURCE_STORAGE_ACCOUNT_VALUE+".dfs.core.windows.net/"+AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH),\
                                        "Type":"ADLS"})
     else:
         dataprop = str(dataprop)+str(",")+str({"DataWriteTarget_"+sourcePostfix: str("https://"+SOURCE_STORAGE_ACCOUNT_VALUE+".dfs.core.windows.net/"+AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH),\
```

### Comparing `mlplatformutils-0.9.5.6/src/mlplatformutils/core/platformutils.py` & `mlplatformutils-0.9.5.7/src/mlplatformutils/core/platformutils.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.9.5.6/src/mlplatformutils/core/sparkcoreutils.py` & `mlplatformutils-0.9.5.7/src/mlplatformutils/core/sparkcoreutils.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.9.5.6/src/mlplatformutils/core/sparkutils.py` & `mlplatformutils-0.9.5.7/src/mlplatformutils/core/sparkutils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import json
 def get_max_properties_starting_with(id, prefix,dataprop,LineageLogger):
 
-    document=LineageLogger.query_graph("g.V().hasLabel('amlrun').has('id', '"+id+"')")[0]
+    documents=LineageLogger.query_graph("g.V().hasLabel('amlrun').has('id', '"+id+"')")
+    if documents:
+        document = documents[0]    
     jsondump = json.dumps(document)
     jsonload = json.loads(jsondump)
     for item in jsonload:
         properties = item.get('properties')
     if properties:
         matching_props = [prop[-1] for prop in properties.keys() if prop.startswith(prefix)]
         max_val = max(int(prop) for prop in matching_props) if matching_props else 0
@@ -28,15 +30,17 @@
     spark.conf.set("fs.azure.account.auth.type."+SOURCE_STORAGE_ACCOUNT_VALUE+".dfs.core.windows.net", "OAuth")
     spark.conf.set("fs.azure.account.oauth.provider.type."+SOURCE_STORAGE_ACCOUNT_VALUE+".dfs.core.windows.net",  "org.apache.hadoop.fs.azurebfs.oauth2.ClientCredsTokenProvider")
     spark.conf.set("fs.azure.account.oauth2.client.id."+SOURCE_STORAGE_ACCOUNT_VALUE+".dfs.core.windows.net", SOURCE_READ_SPN_VALUE)
     spark.conf.set("fs.azure.account.oauth2.client.secret."+SOURCE_STORAGE_ACCOUNT_VALUE+".dfs.core.windows.net", SOURCE_READ_SPNKEY_VALUE)
     spark.conf.set("fs.azure.account.oauth2.client.endpoint."+SOURCE_STORAGE_ACCOUNT_VALUE+".dfs.core.windows.net", "https://login.microsoftonline.com/"+AZURE_TENANT_ID+"/oauth2/token")
 
     df = spark.read.format(file_format).load(file_path)
-    documentId = LineageLogger.query_graph("g.V().hasLabel('amlrun').has('RUN_ID', '"+RUN_ID+"').has('PIPELINE_STEP_NAME', '"+PIPELINE_STEP_NAME+"').values('id')")[0]
+    documentIds = LineageLogger.query_graph("g.V().hasLabel('amlrun').has('RUN_ID', '"+RUN_ID+"').has('PIPELINE_STEP_NAME', '"+PIPELINE_STEP_NAME+"').values('id')")
+    if documentIds:
+        documentId = documentIds[0]    
     sourcePostfix,dataprop=get_max_properties_starting_with(documentId,"DataReadSourceColumns","DataReadSource",LineageLogger)
     if dataprop is None:
         dataprop = str({"DataReadSource_"+sourcePostfix: file_path,\
                                     "Type":"ADLS"})
     else:
         dataprop = str(dataprop)+str(",")+str({"DataReadSource_"+sourcePostfix: file_path,\
                                     "Type":"ADLS"})
@@ -80,15 +84,17 @@
             df.write.format(file_format).mode('overwrite').save(file_path)
     else:
         if partitionColumn:
             df.repartition(repartition).write.format(file_format).partitionBy(partitionColumn).mode("overwrite").save(file_path)
         else:
             df.repartition(repartition).write.format(file_format).mode('overwrite').save(file_path)
 
-    documentId = LineageLogger.query_graph("g.V().hasLabel('amlrun').has('RUN_ID', '"+RUN_ID+"').has('PIPELINE_STEP_NAME', '"+PIPELINE_STEP_NAME+"').values('id')")[0]
+    documentIds = LineageLogger.query_graph("g.V().hasLabel('amlrun').has('RUN_ID', '"+RUN_ID+"').has('PIPELINE_STEP_NAME', '"+PIPELINE_STEP_NAME+"').values('id')")
+    if documentIds:
+        documentId = documentIds[0]    
     targetPostfix,dataprop=get_max_properties_starting_with(documentId,"DataWriteColumns","DataWriteTarget",LineageLogger)  
     if dataprop is None:
         dataprop = str({"DataWriteTarget_"+targetPostfix: file_path,\
                                     "Type":"ADLS"})
     else:
         dataprop = str(dataprop)+str(",")+str({"DataWriteTarget_"+targetPostfix: file_path,\
                                     "Type":"ADLS"})
@@ -109,15 +115,17 @@
                 option("kustoDatabase", kustoOptions["kustoDatabase"]). \
                 option("kustoQuery", kustoOptions["kustoTable"]). \
                 option("kustoAadAppId", kustoOptions["kustoAADClientID"]). \
                 option("kustoAadAppSecret", kustoOptions["kustoClientAADClientPassword"]). \
                 option("kustoAadAuthorityID", kustoOptions["kustoAADAuthorityID"]). \
                 load()
     
-    documentId = LineageLogger.query_graph("g.V().hasLabel('amlrun').has('RUN_ID', '"+RUN_ID+"').has('PIPELINE_STEP_NAME', '"+PIPELINE_STEP_NAME+"').values('id')")[0]
+    documentIds = LineageLogger.query_graph("g.V().hasLabel('amlrun').has('RUN_ID', '"+RUN_ID+"').has('PIPELINE_STEP_NAME', '"+PIPELINE_STEP_NAME+"').values('id')")
+    if documentIds:
+        documentId = documentIds[0]    
     sourcePostfix,dataprop=get_max_properties_starting_with(documentId,"DataReadSourceColumns","DataReadSource",LineageLogger)
     if dataprop is None:
         dataprop = str({"DataReadSource_"+sourcePostfix: "ADX-Cluster "+str(kustoOptions["kustoCluster"])+" ADX-Database"+str(kustoOptions["kustoDatabase"])+ " ADX-Table "+str(kustoOptions["kustoTable"]),\
                                     "Type":"ADX"})
     else:
         dataprop = str(dataprop)+str(",")+str({"DataReadSource_"+sourcePostfix: "ADX-Cluster "+str(kustoOptions["kustoCluster"])+" ADX-Database"+str(kustoOptions["kustoDatabase"])+ " ADX-Table "+str(kustoOptions["kustoTable"]),\
                                     "Type":"ADX"})
@@ -137,15 +145,17 @@
         .option("url", SQL_SERVER_INSTANCE) \
         .option("query", Query) \
         .option("accessToken", access_token) \
         .option("encrypt", "true") \
         .option("hostNameInCertificate", "*.database.windows.net") \
         .load()
 
-    documentId = LineageLogger.query_graph("g.V().hasLabel('amlrun').has('RUN_ID', '"+RUN_ID+"').has('PIPELINE_STEP_NAME', '"+PIPELINE_STEP_NAME+"').values('id')")[0]
+    documentIds = LineageLogger.query_graph("g.V().hasLabel('amlrun').has('RUN_ID', '"+RUN_ID+"').has('PIPELINE_STEP_NAME', '"+PIPELINE_STEP_NAME+"').values('id')")
+    if documentIds:
+        documentId = documentIds[0]    
     sourcePostfix,dataprop=get_max_properties_starting_with(documentId,"DataReadSourceColumns","DataReadSource",LineageLogger)
     if dataprop is None:
         dataprop = str({"DataReadSource_"+sourcePostfix: "SQL SERVER INSTANCE "+str(SQL_SERVER_INSTANCE)+" SQL Query "+str(Query),\
                                     "Type":"AzureSQL"})
     else:
         dataprop = str(dataprop)+str(",")+str({"DataReadSource_"+sourcePostfix: "SQL SERVER INSTANCE "+str(SQL_SERVER_INSTANCE)+" SQL Query "+str(Query),\
                                     "Type":"AzureSQL"})
```

### Comparing `mlplatformutils-0.9.5.6/src/mlplatformutils.egg-info/PKG-INFO` & `mlplatformutils-0.9.5.7/src/mlplatformutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlplatformutils
-Version: 0.9.5.6
+Version: 0.9.5.7
 Author: Keshav Singh
 Author-email: keshav_singh@hotmail.com
 License: MIT
 Keywords: mlplatformutils
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
```

### Comparing `mlplatformutils-0.9.5.6/src/mlplatformutils.egg-info/SOURCES.txt` & `mlplatformutils-0.9.5.7/src/mlplatformutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

