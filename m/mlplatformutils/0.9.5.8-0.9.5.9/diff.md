# Comparing `tmp/mlplatformutils-0.9.5.8.tar.gz` & `tmp/mlplatformutils-0.9.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mlplatformutils-0.9.5.8.tar", last modified: Tue Jun 13 00:30:13 2023, max compression
+gzip compressed data, was "dist\mlplatformutils-0.9.5.9.tar", last modified: Tue Jun 13 01:13:36 2023, max compression
```

## Comparing `mlplatformutils-0.9.5.8.tar` & `mlplatformutils-0.9.5.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 00:30:12.939420 mlplatformutils-0.9.5.8/
--rw-rw-rw-   0        0        0     6719 2023-06-13 00:30:12.940432 mlplatformutils-0.9.5.8/PKG-INFO
--rw-rw-rw-   0        0        0      420 2023-06-04 22:07:41.000000 mlplatformutils-0.9.5.8/README.rst
--rw-rw-rw-   0        0        0      115 2023-06-13 00:30:12.963196 mlplatformutils-0.9.5.8/setup.cfg
--rw-rw-rw-   0        0        0      825 2023-06-13 00:29:09.000000 mlplatformutils-0.9.5.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-13 00:30:11.629680 mlplatformutils-0.9.5.8/src/
-drwxrwxrwx   0        0        0        0 2023-06-13 00:30:11.802770 mlplatformutils-0.9.5.8/src/mlplatformutils/
--rw-rw-rw-   0        0        0        0 2023-06-04 21:52:02.000000 mlplatformutils-0.9.5.8/src/mlplatformutils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 00:30:12.920417 mlplatformutils-0.9.5.8/src/mlplatformutils/core/
--rw-rw-rw-   0        0        0        0 2023-06-03 20:39:09.000000 mlplatformutils-0.9.5.8/src/mlplatformutils/core/__init__.py
--rw-rw-rw-   0        0        0     5868 2023-06-03 20:42:19.000000 mlplatformutils-0.9.5.8/src/mlplatformutils/core/app_insights_logger.py
--rw-rw-rw-   0        0        0     1418 2023-06-12 20:54:48.000000 mlplatformutils-0.9.5.8/src/mlplatformutils/core/freshnessutils.py
--rw-rw-rw-   0        0        0     9225 2023-06-13 00:26:49.000000 mlplatformutils-0.9.5.8/src/mlplatformutils/core/lineagegraph.py
--rw-rw-rw-   0        0        0     6140 2023-06-08 20:01:59.000000 mlplatformutils-0.9.5.8/src/mlplatformutils/core/pandascoreutils.py
--rw-rw-rw-   0        0        0    12536 2023-06-13 00:17:37.000000 mlplatformutils-0.9.5.8/src/mlplatformutils/core/pandasutils.py
--rw-rw-rw-   0        0        0     3129 2023-06-04 21:06:24.000000 mlplatformutils-0.9.5.8/src/mlplatformutils/core/platformutils.py
--rw-rw-rw-   0        0        0     4675 2023-06-08 20:00:19.000000 mlplatformutils-0.9.5.8/src/mlplatformutils/core/sparkcoreutils.py
--rw-rw-rw-   0        0        0    10171 2023-06-13 00:18:10.000000 mlplatformutils-0.9.5.8/src/mlplatformutils/core/sparkutils.py
--rw-rw-rw-   0        0        0       23 2023-06-13 00:29:12.000000 mlplatformutils-0.9.5.8/src/mlplatformutils/core/version.py
-drwxrwxrwx   0        0        0        0 2023-06-13 00:30:11.979856 mlplatformutils-0.9.5.8/src/mlplatformutils.egg-info/
--rw-rw-rw-   0        0        0     6719 2023-06-13 00:30:10.000000 mlplatformutils-0.9.5.8/src/mlplatformutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      688 2023-06-13 00:30:10.000000 mlplatformutils-0.9.5.8/src/mlplatformutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 00:30:10.000000 mlplatformutils-0.9.5.8/src/mlplatformutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      103 2023-06-13 00:30:10.000000 mlplatformutils-0.9.5.8/src/mlplatformutils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-13 00:30:10.000000 mlplatformutils-0.9.5.8/src/mlplatformutils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-13 01:13:36.405673 mlplatformutils-0.9.5.9/
+-rw-rw-rw-   0        0        0     6719 2023-06-13 01:13:36.406672 mlplatformutils-0.9.5.9/PKG-INFO
+-rw-rw-rw-   0        0        0      420 2023-06-04 22:07:41.000000 mlplatformutils-0.9.5.9/README.rst
+-rw-rw-rw-   0        0        0      115 2023-06-13 01:13:36.410673 mlplatformutils-0.9.5.9/setup.cfg
+-rw-rw-rw-   0        0        0      825 2023-06-13 01:12:40.000000 mlplatformutils-0.9.5.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 01:13:36.023325 mlplatformutils-0.9.5.9/src/
+drwxrwxrwx   0        0        0        0 2023-06-13 01:13:36.062858 mlplatformutils-0.9.5.9/src/mlplatformutils/
+-rw-rw-rw-   0        0        0        0 2023-06-04 21:52:02.000000 mlplatformutils-0.9.5.9/src/mlplatformutils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 01:13:36.402678 mlplatformutils-0.9.5.9/src/mlplatformutils/core/
+-rw-rw-rw-   0        0        0        0 2023-06-03 20:39:09.000000 mlplatformutils-0.9.5.9/src/mlplatformutils/core/__init__.py
+-rw-rw-rw-   0        0        0     5868 2023-06-03 20:42:19.000000 mlplatformutils-0.9.5.9/src/mlplatformutils/core/app_insights_logger.py
+-rw-rw-rw-   0        0        0     1418 2023-06-12 20:54:48.000000 mlplatformutils-0.9.5.9/src/mlplatformutils/core/freshnessutils.py
+-rw-rw-rw-   0        0        0     9428 2023-06-13 01:13:11.000000 mlplatformutils-0.9.5.9/src/mlplatformutils/core/lineagegraph.py
+-rw-rw-rw-   0        0        0     6140 2023-06-08 20:01:59.000000 mlplatformutils-0.9.5.9/src/mlplatformutils/core/pandascoreutils.py
+-rw-rw-rw-   0        0        0    12536 2023-06-13 00:17:37.000000 mlplatformutils-0.9.5.9/src/mlplatformutils/core/pandasutils.py
+-rw-rw-rw-   0        0        0     3129 2023-06-04 21:06:24.000000 mlplatformutils-0.9.5.9/src/mlplatformutils/core/platformutils.py
+-rw-rw-rw-   0        0        0     4675 2023-06-08 20:00:19.000000 mlplatformutils-0.9.5.9/src/mlplatformutils/core/sparkcoreutils.py
+-rw-rw-rw-   0        0        0    10171 2023-06-13 00:18:10.000000 mlplatformutils-0.9.5.9/src/mlplatformutils/core/sparkutils.py
+-rw-rw-rw-   0        0        0       23 2023-06-13 01:12:44.000000 mlplatformutils-0.9.5.9/src/mlplatformutils/core/version.py
+drwxrwxrwx   0        0        0        0 2023-06-13 01:13:36.125871 mlplatformutils-0.9.5.9/src/mlplatformutils.egg-info/
+-rw-rw-rw-   0        0        0     6719 2023-06-13 01:13:35.000000 mlplatformutils-0.9.5.9/src/mlplatformutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      688 2023-06-13 01:13:35.000000 mlplatformutils-0.9.5.9/src/mlplatformutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 01:13:35.000000 mlplatformutils-0.9.5.9/src/mlplatformutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      103 2023-06-13 01:13:35.000000 mlplatformutils-0.9.5.9/src/mlplatformutils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-13 01:13:35.000000 mlplatformutils-0.9.5.9/src/mlplatformutils.egg-info/top_level.txt
```

### Comparing `mlplatformutils-0.9.5.8/PKG-INFO` & `mlplatformutils-0.9.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlplatformutils
-Version: 0.9.5.8
+Version: 0.9.5.9
 Author: Keshav Singh
 Author-email: keshav_singh@hotmail.com
 License: MIT
 Keywords: mlplatformutils
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
```

### Comparing `mlplatformutils-0.9.5.8/setup.py` & `mlplatformutils-0.9.5.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 else:
     long_description="#DESC"
 
 setup(
     name='mlplatformutils',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='0.9.5.8',
+    version='0.9.5.9',
     license='MIT',
     classifiers=[
         'Programming Language :: Python :: 3.8'
     ],
     author='Keshav Singh',
     author_email='keshav_singh@hotmail.com',
     packages=find_packages('src'),
```

### Comparing `mlplatformutils-0.9.5.8/src/mlplatformutils/core/app_insights_logger.py` & `mlplatformutils-0.9.5.9/src/mlplatformutils/core/app_insights_logger.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.9.5.8/src/mlplatformutils/core/freshnessutils.py` & `mlplatformutils-0.9.5.9/src/mlplatformutils/core/freshnessutils.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.9.5.8/src/mlplatformutils/core/lineagegraph.py` & `mlplatformutils-0.9.5.9/src/mlplatformutils/core/lineagegraph.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,18 +44,17 @@
 
     def print_status_attributes(self,result):
         print("\tResponse status_attributes:\n\t{0}".format(result.status_attributes))
 
     def add_vertex(self, label, properties,run_id,pipeline_step_name):
         try:
             query = "g.V().hasLabel('amlrun').has('RUN_ID', '"+run_id+"').has('PIPELINE_STEP_NAME', '"+pipeline_step_name+"').values('id')"
-            callback = self.client.submitAsync(query)
-            results = callback.result()
-            if results:
-                documentId = results[0]
+            documentIds = self.query_graph(query)
+            if documentIds:
+                documentId = documentId[0]
                 print("The Vertex Already Exists! Updating it..")
                 self.update_vertex(documentId,properties)
             else:
                 print("Adding a new Vertex!")
                 if self.partition_key in properties.keys():
                     queryStr=""
                     queryStr = queryStr + "g.addV('" + label + "')"
@@ -163,28 +162,34 @@
             self.print_status_attributes(callback.result())
         except Exception as e:
             traceback.print_exc()
             raise ValueError("Failed to DROP EDGE to Cosmos Gremlin graph!")
     
     def query_graph(self,query):
         try:
+            result = None
             callback = self.client.submitAsync(query)
             for result in callback.result():
                 print(result)
             self.print_status_attributes(callback.result())
             return result
         except Exception as e:
             traceback.print_exc()
             raise ValueError("Failed to QUERY Cosmos Gremlin graph!")
         
     def update_lineage_graph(self,run_id,pipeline_step_name,properties):
         try:
             query = "g.V().hasLabel('amlrun').has('RUN_ID', '"+run_id+"').has('PIPELINE_STEP_NAME', '"+pipeline_step_name+"').values('id')"
-            documentId = self.query_graph(query)[0]
-            self.update_vertex(documentId,properties)
+            documentIds = self.query_graph(query)
+            if documentIds:
+                documentId = documentId[0]
+                print("The Vertex Already Exists! Updating it..")            
+                self.update_vertex(documentId,properties)
+            else:
+                print("Document Not Found!")
             return
         except Exception as e:
             traceback.print_exc()
             raise ValueError("Failed to Update lineage graph!")
         
     def connect_lineage_graph(self,run_id,source_pipeline_step_name,dest_pipeline_step_name):
         try:
```

### Comparing `mlplatformutils-0.9.5.8/src/mlplatformutils/core/pandascoreutils.py` & `mlplatformutils-0.9.5.9/src/mlplatformutils/core/pandascoreutils.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.9.5.8/src/mlplatformutils/core/pandasutils.py` & `mlplatformutils-0.9.5.9/src/mlplatformutils/core/pandasutils.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.9.5.8/src/mlplatformutils/core/platformutils.py` & `mlplatformutils-0.9.5.9/src/mlplatformutils/core/platformutils.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.9.5.8/src/mlplatformutils/core/sparkcoreutils.py` & `mlplatformutils-0.9.5.9/src/mlplatformutils/core/sparkcoreutils.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.9.5.8/src/mlplatformutils/core/sparkutils.py` & `mlplatformutils-0.9.5.9/src/mlplatformutils/core/sparkutils.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.9.5.8/src/mlplatformutils.egg-info/PKG-INFO` & `mlplatformutils-0.9.5.9/src/mlplatformutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlplatformutils
-Version: 0.9.5.8
+Version: 0.9.5.9
 Author: Keshav Singh
 Author-email: keshav_singh@hotmail.com
 License: MIT
 Keywords: mlplatformutils
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
```

### Comparing `mlplatformutils-0.9.5.8/src/mlplatformutils.egg-info/SOURCES.txt` & `mlplatformutils-0.9.5.9/src/mlplatformutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

