# Comparing `tmp/mlplatformutils-0.9.3.tar.gz` & `tmp/mlplatformutils-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mlplatformutils-0.9.3.tar", last modified: Sat Jun 10 01:12:48 2023, max compression
+gzip compressed data, was "dist\mlplatformutils-0.9.4.tar", last modified: Mon Jun 12 20:58:23 2023, max compression
```

## Comparing `mlplatformutils-0.9.3.tar` & `mlplatformutils-0.9.4.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-10 01:12:48.726470 mlplatformutils-0.9.3/
--rw-rw-rw-   0        0        0     6101 2023-06-10 01:12:48.726470 mlplatformutils-0.9.3/PKG-INFO
--rw-rw-rw-   0        0        0      420 2023-06-04 22:07:41.000000 mlplatformutils-0.9.3/README.rst
--rw-rw-rw-   0        0        0      115 2023-06-10 01:12:48.743474 mlplatformutils-0.9.3/setup.cfg
--rw-rw-rw-   0        0        0      808 2023-06-10 01:12:37.000000 mlplatformutils-0.9.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-10 01:12:48.556629 mlplatformutils-0.9.3/src/
-drwxrwxrwx   0        0        0        0 2023-06-10 01:12:48.580639 mlplatformutils-0.9.3/src/mlplatformutils/
--rw-rw-rw-   0        0        0        0 2023-06-04 21:52:02.000000 mlplatformutils-0.9.3/src/mlplatformutils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-10 01:12:48.726470 mlplatformutils-0.9.3/src/mlplatformutils/core/
--rw-rw-rw-   0        0        0        0 2023-06-03 20:39:09.000000 mlplatformutils-0.9.3/src/mlplatformutils/core/__init__.py
--rw-rw-rw-   0        0        0     5868 2023-06-03 20:42:19.000000 mlplatformutils-0.9.3/src/mlplatformutils/core/app_insights_logger.py
--rw-rw-rw-   0        0        0     8654 2023-06-07 03:10:08.000000 mlplatformutils-0.9.3/src/mlplatformutils/core/lineagegraph.py
--rw-rw-rw-   0        0        0     6140 2023-06-08 20:01:59.000000 mlplatformutils-0.9.3/src/mlplatformutils/core/pandascoreutils.py
--rw-rw-rw-   0        0        0    12536 2023-06-10 01:10:09.000000 mlplatformutils-0.9.3/src/mlplatformutils/core/pandasutils.py
--rw-rw-rw-   0        0        0     3129 2023-06-04 21:06:24.000000 mlplatformutils-0.9.3/src/mlplatformutils/core/platformutils.py
--rw-rw-rw-   0        0        0     4675 2023-06-08 20:00:19.000000 mlplatformutils-0.9.3/src/mlplatformutils/core/sparkcoreutils.py
--rw-rw-rw-   0        0        0    10171 2023-06-10 01:11:28.000000 mlplatformutils-0.9.3/src/mlplatformutils/core/sparkutils.py
--rw-rw-rw-   0        0        0       21 2023-06-10 01:12:32.000000 mlplatformutils-0.9.3/src/mlplatformutils/core/version.py
-drwxrwxrwx   0        0        0        0 2023-06-10 01:12:48.615703 mlplatformutils-0.9.3/src/mlplatformutils.egg-info/
--rw-rw-rw-   0        0        0     6101 2023-06-10 01:12:48.000000 mlplatformutils-0.9.3/src/mlplatformutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      645 2023-06-10 01:12:48.000000 mlplatformutils-0.9.3/src/mlplatformutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 01:12:48.000000 mlplatformutils-0.9.3/src/mlplatformutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       90 2023-06-10 01:12:48.000000 mlplatformutils-0.9.3/src/mlplatformutils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-10 01:12:48.000000 mlplatformutils-0.9.3/src/mlplatformutils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-12 20:58:23.220631 mlplatformutils-0.9.4/
+-rw-rw-rw-   0        0        0     6717 2023-06-12 20:58:23.221629 mlplatformutils-0.9.4/PKG-INFO
+-rw-rw-rw-   0        0        0      420 2023-06-04 22:07:41.000000 mlplatformutils-0.9.4/README.rst
+-rw-rw-rw-   0        0        0      115 2023-06-12 20:58:23.226626 mlplatformutils-0.9.4/setup.cfg
+-rw-rw-rw-   0        0        0      823 2023-06-12 20:57:58.000000 mlplatformutils-0.9.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 20:58:22.827486 mlplatformutils-0.9.4/src/
+drwxrwxrwx   0        0        0        0 2023-06-12 20:58:22.884011 mlplatformutils-0.9.4/src/mlplatformutils/
+-rw-rw-rw-   0        0        0        0 2023-06-04 21:52:02.000000 mlplatformutils-0.9.4/src/mlplatformutils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 20:58:23.216627 mlplatformutils-0.9.4/src/mlplatformutils/core/
+-rw-rw-rw-   0        0        0        0 2023-06-03 20:39:09.000000 mlplatformutils-0.9.4/src/mlplatformutils/core/__init__.py
+-rw-rw-rw-   0        0        0     5868 2023-06-03 20:42:19.000000 mlplatformutils-0.9.4/src/mlplatformutils/core/app_insights_logger.py
+-rw-rw-rw-   0        0        0     1418 2023-06-12 20:54:48.000000 mlplatformutils-0.9.4/src/mlplatformutils/core/freshnessutils.py
+-rw-rw-rw-   0        0        0     9532 2023-06-12 20:58:16.000000 mlplatformutils-0.9.4/src/mlplatformutils/core/lineagegraph.py
+-rw-rw-rw-   0        0        0     6140 2023-06-08 20:01:59.000000 mlplatformutils-0.9.4/src/mlplatformutils/core/pandascoreutils.py
+-rw-rw-rw-   0        0        0    12536 2023-06-10 01:10:09.000000 mlplatformutils-0.9.4/src/mlplatformutils/core/pandasutils.py
+-rw-rw-rw-   0        0        0     3129 2023-06-04 21:06:24.000000 mlplatformutils-0.9.4/src/mlplatformutils/core/platformutils.py
+-rw-rw-rw-   0        0        0     4675 2023-06-08 20:00:19.000000 mlplatformutils-0.9.4/src/mlplatformutils/core/sparkcoreutils.py
+-rw-rw-rw-   0        0        0    10171 2023-06-10 01:11:28.000000 mlplatformutils-0.9.4/src/mlplatformutils/core/sparkutils.py
+-rw-rw-rw-   0        0        0       21 2023-06-12 20:58:04.000000 mlplatformutils-0.9.4/src/mlplatformutils/core/version.py
+drwxrwxrwx   0        0        0        0 2023-06-12 20:58:22.962549 mlplatformutils-0.9.4/src/mlplatformutils.egg-info/
+-rw-rw-rw-   0        0        0     6717 2023-06-12 20:58:22.000000 mlplatformutils-0.9.4/src/mlplatformutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      688 2023-06-12 20:58:22.000000 mlplatformutils-0.9.4/src/mlplatformutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 20:58:22.000000 mlplatformutils-0.9.4/src/mlplatformutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      103 2023-06-12 20:58:22.000000 mlplatformutils-0.9.4/src/mlplatformutils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-12 20:58:22.000000 mlplatformutils-0.9.4/src/mlplatformutils.egg-info/top_level.txt
```

### Comparing `mlplatformutils-0.9.3/PKG-INFO` & `mlplatformutils-0.9.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlplatformutils
-Version: 0.9.3
+Version: 0.9.4
 Author: Keshav Singh
 Author-email: keshav_singh@hotmail.com
 License: MIT
 Keywords: mlplatformutils
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 
@@ -82,28 +82,35 @@
 **pandascoreutils** - Contains functions to read data from Azure Data Lake Gen2 (from Delta Format or Parquet Format) into Pandas Dataframe without Spark **without** integrated Lineage Graph Logging.
 
 * read_from_delta_as_pandas
 * read_parquet_file_from_adlsgen2_as_pandas
 * read_parquet_directory_from_adlsgen2_as_pandas
 * write_pandas_as_parquet_file_to_adlsgen2
 
+**freshnessutils** - Contains functions to add freshness details into Azure Cosmos (NoSQL) document db. This helps with the details on the freshness metrics on evaluating the SLA, and downstream processing. It captures and provides details on model, training dataset freshness for the most recent and historical processing.
+
+* add_freshness
+* upsert_freshness
+* query_freshness
+
 ### Examples
 
 <br />
 
 **from mlplatformutils.core.platformutils import is_package_installed** <br />
 **print(is_package_installed("pandas"))** <br />
 **from mlplatformutils.core.app_insights_logger import telemetrylogger** <br />
 **from mlplatformutils.core.lineagegraph import LineageGraph** <br />
 **from mlplatformutils.core.sparkutils import write_to_adls_gen2, read_from_adls_gen2** <br />
 **from mlplatformutils.core.pandasutils import write_pandas_as_parquet_file_to_adlsgen2, read_parquet_directory_from_adlsgen2_as_pandas** <br />
 **from mlplatformutils.core.sparkcoreutils import write_to_adls_gen2, read_from_adls_gen2** <br />
 **from mlplatformutils.core.pandascoreutils import write_pandas_as_parquet_file_to_adlsgen2, read_parquet_directory_from_adlsgen2_as_pandas** <br />
+**from mlplatformutils.core.freshnessutils import add_freshness, upsert_freshness, query_freshness** <br />
 **import mlplatformutils.core.version as vr** <br />
-**print(vr.__version__)** <br />
+**print(vr.\_\_version\_\_)** <br />
 
 ### Notes
 
 <br />
 
 When Running this Lineage Package from Jupyter Nootebook, the below 3 Lines Help overcome JupyterNotebook **RuntimeError: Cannot run the event loop while another loop is running** <br />
 **import asyncio** <br />
@@ -126,26 +133,28 @@
 |   |   |-- |-- __init__.py<br />
 |   |   |-- |-- sparkcoreutils.py<br />
 |   |   |-- |-- sparkutils.py<br />
 |   |   |-- |-- platformutils.py<br />
 |   |   |-- |-- pandascoreutils.py<br />
 |   |   |-- |-- pandasutils.py<br />
 |   |   |-- |-- lineagegraph.py<br />
+|   |   |-- |-- freshnessutils.py<br />
 |   |   |-- |-- app_insights_logger.py<br />
 |-- tests<br />
 |   |-- __init__.py<br />
 |   |-- core<br />
 |   |-- |--__init__.py<br />
-|   |-- |-- sparkcoreutils.py<br />
-|   |-- |-- sparkutils.py<br />
-|   |-- |-- platformutils.py<br />
-|   |-- |-- pandascoreutils.py<br />
-|   |-- |-- pandasutils.py<br />
-|   |-- |-- lineagegraph.py<br />
-|   |-- |-- app_insights_logger.py<br />
+|   |-- |-- test_sparkcoreutils.py<br />
+|   |-- |-- test_sparkutils.py<br />
+|   |-- |-- test_platformutils.py<br />
+|   |-- |-- test_pandascoreutils.py<br />
+|   |-- |-- test_pandasutils.py<br />
+|   |-- |-- test_lineagegraph.py<br />
+|   |-- |-- test_freshnessutils.py<br />
+|   |-- |-- test_app_insights_logger.py<br />
 <br />
 
 ## Instructions
 
 <br />
  install twine - twine is a utility package that is used for publishing Python packages on PyPI <br />
```

### Comparing `mlplatformutils-0.9.3/setup.py` & `mlplatformutils-0.9.4/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 else:
     long_description="#DESC"
 
 setup(
     name='mlplatformutils',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='0.9.3',
+    version='0.9.4',
     license='MIT',
     classifiers=[
         'Programming Language :: Python :: 3.8'
     ],
     author='Keshav Singh',
     author_email='keshav_singh@hotmail.com',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     keywords='mlplatformutils',
     install_requires=[
-          'applicationinsights','gremlinpython','azureml-core','azure-identity','azure-storage-file-datalake'
+          'applicationinsights','gremlinpython','azureml-core','azure-identity','azure-storage-file-datalake','azure-cosmos'
       ],
 
 )
```

### Comparing `mlplatformutils-0.9.3/src/mlplatformutils/core/app_insights_logger.py` & `mlplatformutils-0.9.4/src/mlplatformutils/core/app_insights_logger.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.9.3/src/mlplatformutils/core/lineagegraph.py` & `mlplatformutils-0.9.4/src/mlplatformutils/core/lineagegraph.py`

 * *Files 9% similar despite different names*

```diff
@@ -41,32 +41,38 @@
                 print("Default error handling")
             traceback.print_exc(file=sys.stdout) 
             raise ValueError("Failed to connect to Cosmos Gremlin graph")
 
     def print_status_attributes(self,result):
         print("\tResponse status_attributes:\n\t{0}".format(result.status_attributes))
 
-    def add_vertex(self, label, properties):
+    def add_vertex(self, label, properties,run_id,pipeline_step_name):
         try:
-            if self.partition_key in properties.keys():
-                queryStr=""
-                queryStr = queryStr + "g.addV('" + label + "')"
-                for key, value in properties.items():
-                    queryStr = queryStr + ".property('" + key + "','" + str(value) + "')"
-                print(queryStr)
+            query = "g.V().hasLabel('amlrun').has('RUN_ID', '"+run_id+"').has('PIPELINE_STEP_NAME', '"+pipeline_step_name+"').values('id')"
+            documentId = self.query_graph(query)[0]
+            if documentId:
+                print("The Vertex Already Exists! Updating it..")
+                self.update_vertex(documentId,properties)
             else:
-                print("Unable To Add Vertex. Partition Key '"+ self.partition_key +"' Not Found! Failed to Add VERTEX to Cosmos Gremlin graph!")
-            callback = self.client.submitAsync(queryStr)
-            if callback.result() is not None:
-                print("\tInserted this vertex:\n\t{0}".format(callback.result().all().result()))
-            else:
-                print("Something went wrong with this query: {0}".format(queryStr))
-            print("\n")
-            self.print_status_attributes(callback.result())
-
+                print("Adding a new Vertex!")
+                if self.partition_key in properties.keys():
+                    queryStr=""
+                    queryStr = queryStr + "g.addV('" + label + "')"
+                    for key, value in properties.items():
+                        queryStr = queryStr + ".property('" + key + "','" + str(value) + "')"
+                    print(queryStr)
+                else:
+                    print("Unable To Add Vertex. Partition Key '"+ self.partition_key +"' Not Found! Failed to Add VERTEX to Cosmos Gremlin graph!")
+                callback = self.client.submitAsync(queryStr)
+                if callback.result() is not None:
+                    print("\tInserted this vertex:\n\t{0}".format(callback.result().all().result()))
+                else:
+                    print("Something went wrong with this query: {0}".format(queryStr))
+                print("\n")
+                self.print_status_attributes(callback.result())
         except Exception as e:
             traceback.print_exc()
             raise ValueError("Failed to add vertex to Cosmos Gremlin graph!")
 
     def get_vertices(self, label,id):
         try:
             StrQuery = "g.V().hasLabel('" + label + "')"+".has('id','" + id + "')"
@@ -113,32 +119,40 @@
         except Exception as e:
             traceback.print_exc()
             raise ValueError("Failed to UPDATE vertex to Cosmos Gremlin graph!")
 
 
     def insert_edges(self,source_v_id,target_v_id,edge_label,properties):
         try:
+            exists_query = "g.V('" + source_v_id + "').outE('" + edge_label + "').where(inV().hasId('" + target_v_id + "')).hasNext()"
+            exists_callback = self.client.submitAsync(exists_query)
+            exists_result = exists_callback.result().one()
+        
+            if exists_result:
+                print("Edge already exists.")
+                return
+        
             queryStr=""
             queryStr = queryStr + "g.V('" + source_v_id + "')" + ".addE('" + edge_label + "')" + ".to(g.V('" + target_v_id + "'))"
             if properties is not None:
                 for key, value in properties.items():
                     queryStr = queryStr + ".property('" + key + "','" + str(value) + "')"
             print(queryStr)
             callback = self.client.submitAsync(queryStr)
             if callback.result() is not None:
-                print("\tConnected the verteices with Edge:\n\t{0}".format(callback.result().all().result()))
+                print("\tConnected the Vertices with Edge:\n\t{0}".format(callback.result().all().result()))
             else:
                 print("Something went wrong with this query: {0}".format(queryStr))
             print("\n")
             self.print_status_attributes(callback.result())
 
         except Exception as e:
             traceback.print_exc()
             raise ValueError("Failed to add EDGE to Cosmos Gremlin graph!")
-
+        
     def drop_vertex(self,id):
         try:
             queryStr="g.V('id','"+id+"').drop()"
             callback = self.client.submitAsync(queryStr)
             for result in callback.result():
                 print(result)
             self.print_status_attributes(callback.result())
```

### Comparing `mlplatformutils-0.9.3/src/mlplatformutils/core/pandascoreutils.py` & `mlplatformutils-0.9.4/src/mlplatformutils/core/pandascoreutils.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.9.3/src/mlplatformutils/core/pandasutils.py` & `mlplatformutils-0.9.4/src/mlplatformutils/core/pandasutils.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.9.3/src/mlplatformutils/core/platformutils.py` & `mlplatformutils-0.9.4/src/mlplatformutils/core/platformutils.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.9.3/src/mlplatformutils/core/sparkcoreutils.py` & `mlplatformutils-0.9.4/src/mlplatformutils/core/sparkcoreutils.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.9.3/src/mlplatformutils/core/sparkutils.py` & `mlplatformutils-0.9.4/src/mlplatformutils/core/sparkutils.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.9.3/src/mlplatformutils.egg-info/PKG-INFO` & `mlplatformutils-0.9.4/src/mlplatformutils.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlplatformutils
-Version: 0.9.3
+Version: 0.9.4
 Author: Keshav Singh
 Author-email: keshav_singh@hotmail.com
 License: MIT
 Keywords: mlplatformutils
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 
@@ -82,28 +82,35 @@
 **pandascoreutils** - Contains functions to read data from Azure Data Lake Gen2 (from Delta Format or Parquet Format) into Pandas Dataframe without Spark **without** integrated Lineage Graph Logging.
 
 * read_from_delta_as_pandas
 * read_parquet_file_from_adlsgen2_as_pandas
 * read_parquet_directory_from_adlsgen2_as_pandas
 * write_pandas_as_parquet_file_to_adlsgen2
 
+**freshnessutils** - Contains functions to add freshness details into Azure Cosmos (NoSQL) document db. This helps with the details on the freshness metrics on evaluating the SLA, and downstream processing. It captures and provides details on model, training dataset freshness for the most recent and historical processing.
+
+* add_freshness
+* upsert_freshness
+* query_freshness
+
 ### Examples
 
 <br />
 
 **from mlplatformutils.core.platformutils import is_package_installed** <br />
 **print(is_package_installed("pandas"))** <br />
 **from mlplatformutils.core.app_insights_logger import telemetrylogger** <br />
 **from mlplatformutils.core.lineagegraph import LineageGraph** <br />
 **from mlplatformutils.core.sparkutils import write_to_adls_gen2, read_from_adls_gen2** <br />
 **from mlplatformutils.core.pandasutils import write_pandas_as_parquet_file_to_adlsgen2, read_parquet_directory_from_adlsgen2_as_pandas** <br />
 **from mlplatformutils.core.sparkcoreutils import write_to_adls_gen2, read_from_adls_gen2** <br />
 **from mlplatformutils.core.pandascoreutils import write_pandas_as_parquet_file_to_adlsgen2, read_parquet_directory_from_adlsgen2_as_pandas** <br />
+**from mlplatformutils.core.freshnessutils import add_freshness, upsert_freshness, query_freshness** <br />
 **import mlplatformutils.core.version as vr** <br />
-**print(vr.__version__)** <br />
+**print(vr.\_\_version\_\_)** <br />
 
 ### Notes
 
 <br />
 
 When Running this Lineage Package from Jupyter Nootebook, the below 3 Lines Help overcome JupyterNotebook **RuntimeError: Cannot run the event loop while another loop is running** <br />
 **import asyncio** <br />
@@ -126,26 +133,28 @@
 |   |   |-- |-- __init__.py<br />
 |   |   |-- |-- sparkcoreutils.py<br />
 |   |   |-- |-- sparkutils.py<br />
 |   |   |-- |-- platformutils.py<br />
 |   |   |-- |-- pandascoreutils.py<br />
 |   |   |-- |-- pandasutils.py<br />
 |   |   |-- |-- lineagegraph.py<br />
+|   |   |-- |-- freshnessutils.py<br />
 |   |   |-- |-- app_insights_logger.py<br />
 |-- tests<br />
 |   |-- __init__.py<br />
 |   |-- core<br />
 |   |-- |--__init__.py<br />
-|   |-- |-- sparkcoreutils.py<br />
-|   |-- |-- sparkutils.py<br />
-|   |-- |-- platformutils.py<br />
-|   |-- |-- pandascoreutils.py<br />
-|   |-- |-- pandasutils.py<br />
-|   |-- |-- lineagegraph.py<br />
-|   |-- |-- app_insights_logger.py<br />
+|   |-- |-- test_sparkcoreutils.py<br />
+|   |-- |-- test_sparkutils.py<br />
+|   |-- |-- test_platformutils.py<br />
+|   |-- |-- test_pandascoreutils.py<br />
+|   |-- |-- test_pandasutils.py<br />
+|   |-- |-- test_lineagegraph.py<br />
+|   |-- |-- test_freshnessutils.py<br />
+|   |-- |-- test_app_insights_logger.py<br />
 <br />
 
 ## Instructions
 
 <br />
  install twine - twine is a utility package that is used for publishing Python packages on PyPI <br />
```

### Comparing `mlplatformutils-0.9.3/src/mlplatformutils.egg-info/SOURCES.txt` & `mlplatformutils-0.9.4/src/mlplatformutils.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 src/mlplatformutils.egg-info/PKG-INFO
 src/mlplatformutils.egg-info/SOURCES.txt
 src/mlplatformutils.egg-info/dependency_links.txt
 src/mlplatformutils.egg-info/requires.txt
 src/mlplatformutils.egg-info/top_level.txt
 src/mlplatformutils/core/__init__.py
 src/mlplatformutils/core/app_insights_logger.py
+src/mlplatformutils/core/freshnessutils.py
 src/mlplatformutils/core/lineagegraph.py
 src/mlplatformutils/core/pandascoreutils.py
 src/mlplatformutils/core/pandasutils.py
 src/mlplatformutils/core/platformutils.py
 src/mlplatformutils/core/sparkcoreutils.py
 src/mlplatformutils/core/sparkutils.py
 src/mlplatformutils/core/version.py
```

