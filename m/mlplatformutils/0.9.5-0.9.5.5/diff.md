# Comparing `tmp/mlplatformutils-0.9.5.tar.gz` & `tmp/mlplatformutils-0.9.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mlplatformutils-0.9.5.tar", last modified: Mon Jun 12 23:13:30 2023, max compression
+gzip compressed data, was "dist\mlplatformutils-0.9.5.5.tar", last modified: Mon Jun 12 23:17:47 2023, max compression
```

## Comparing `mlplatformutils-0.9.5.tar` & `mlplatformutils-0.9.5.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 23:13:30.478416 mlplatformutils-0.9.5/
--rw-rw-rw-   0        0        0     6717 2023-06-12 23:13:30.479417 mlplatformutils-0.9.5/PKG-INFO
--rw-rw-rw-   0        0        0      420 2023-06-04 22:07:41.000000 mlplatformutils-0.9.5/README.rst
--rw-rw-rw-   0        0        0      115 2023-06-12 23:13:30.485414 mlplatformutils-0.9.5/setup.cfg
--rw-rw-rw-   0        0        0      823 2023-06-12 23:09:20.000000 mlplatformutils-0.9.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-12 23:13:29.992683 mlplatformutils-0.9.5/src/
-drwxrwxrwx   0        0        0        0 2023-06-12 23:13:30.044680 mlplatformutils-0.9.5/src/mlplatformutils/
--rw-rw-rw-   0        0        0        0 2023-06-04 21:52:02.000000 mlplatformutils-0.9.5/src/mlplatformutils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 23:13:30.475415 mlplatformutils-0.9.5/src/mlplatformutils/core/
--rw-rw-rw-   0        0        0        0 2023-06-03 20:39:09.000000 mlplatformutils-0.9.5/src/mlplatformutils/core/__init__.py
--rw-rw-rw-   0        0        0     5868 2023-06-03 20:42:19.000000 mlplatformutils-0.9.5/src/mlplatformutils/core/app_insights_logger.py
--rw-rw-rw-   0        0        0     1418 2023-06-12 20:54:48.000000 mlplatformutils-0.9.5/src/mlplatformutils/core/freshnessutils.py
--rw-rw-rw-   0        0        0    10115 2023-06-12 23:13:15.000000 mlplatformutils-0.9.5/src/mlplatformutils/core/lineagegraph.py
--rw-rw-rw-   0        0        0     6140 2023-06-08 20:01:59.000000 mlplatformutils-0.9.5/src/mlplatformutils/core/pandascoreutils.py
--rw-rw-rw-   0        0        0    12536 2023-06-10 01:10:09.000000 mlplatformutils-0.9.5/src/mlplatformutils/core/pandasutils.py
--rw-rw-rw-   0        0        0     3129 2023-06-04 21:06:24.000000 mlplatformutils-0.9.5/src/mlplatformutils/core/platformutils.py
--rw-rw-rw-   0        0        0     4675 2023-06-08 20:00:19.000000 mlplatformutils-0.9.5/src/mlplatformutils/core/sparkcoreutils.py
--rw-rw-rw-   0        0        0    10171 2023-06-10 01:11:28.000000 mlplatformutils-0.9.5/src/mlplatformutils/core/sparkutils.py
--rw-rw-rw-   0        0        0       21 2023-06-12 23:09:16.000000 mlplatformutils-0.9.5/src/mlplatformutils/core/version.py
-drwxrwxrwx   0        0        0        0 2023-06-12 23:13:30.112223 mlplatformutils-0.9.5/src/mlplatformutils.egg-info/
--rw-rw-rw-   0        0        0     6717 2023-06-12 23:13:29.000000 mlplatformutils-0.9.5/src/mlplatformutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      688 2023-06-12 23:13:29.000000 mlplatformutils-0.9.5/src/mlplatformutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 23:13:29.000000 mlplatformutils-0.9.5/src/mlplatformutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      103 2023-06-12 23:13:29.000000 mlplatformutils-0.9.5/src/mlplatformutils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-12 23:13:29.000000 mlplatformutils-0.9.5/src/mlplatformutils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-12 23:17:47.606733 mlplatformutils-0.9.5.5/
+-rw-rw-rw-   0        0        0     6719 2023-06-12 23:17:47.607732 mlplatformutils-0.9.5.5/PKG-INFO
+-rw-rw-rw-   0        0        0      420 2023-06-04 22:07:41.000000 mlplatformutils-0.9.5.5/README.rst
+-rw-rw-rw-   0        0        0      115 2023-06-12 23:17:47.613729 mlplatformutils-0.9.5.5/setup.cfg
+-rw-rw-rw-   0        0        0      825 2023-06-12 23:17:37.000000 mlplatformutils-0.9.5.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 23:17:47.421530 mlplatformutils-0.9.5.5/src/
+drwxrwxrwx   0        0        0        0 2023-06-12 23:17:47.444535 mlplatformutils-0.9.5.5/src/mlplatformutils/
+-rw-rw-rw-   0        0        0        0 2023-06-04 21:52:02.000000 mlplatformutils-0.9.5.5/src/mlplatformutils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 23:17:47.602728 mlplatformutils-0.9.5.5/src/mlplatformutils/core/
+-rw-rw-rw-   0        0        0        0 2023-06-03 20:39:09.000000 mlplatformutils-0.9.5.5/src/mlplatformutils/core/__init__.py
+-rw-rw-rw-   0        0        0     5868 2023-06-03 20:42:19.000000 mlplatformutils-0.9.5.5/src/mlplatformutils/core/app_insights_logger.py
+-rw-rw-rw-   0        0        0     1418 2023-06-12 20:54:48.000000 mlplatformutils-0.9.5.5/src/mlplatformutils/core/freshnessutils.py
+-rw-rw-rw-   0        0        0    10096 2023-06-12 23:17:29.000000 mlplatformutils-0.9.5.5/src/mlplatformutils/core/lineagegraph.py
+-rw-rw-rw-   0        0        0     6140 2023-06-08 20:01:59.000000 mlplatformutils-0.9.5.5/src/mlplatformutils/core/pandascoreutils.py
+-rw-rw-rw-   0        0        0    12536 2023-06-10 01:10:09.000000 mlplatformutils-0.9.5.5/src/mlplatformutils/core/pandasutils.py
+-rw-rw-rw-   0        0        0     3129 2023-06-04 21:06:24.000000 mlplatformutils-0.9.5.5/src/mlplatformutils/core/platformutils.py
+-rw-rw-rw-   0        0        0     4675 2023-06-08 20:00:19.000000 mlplatformutils-0.9.5.5/src/mlplatformutils/core/sparkcoreutils.py
+-rw-rw-rw-   0        0        0    10171 2023-06-10 01:11:28.000000 mlplatformutils-0.9.5.5/src/mlplatformutils/core/sparkutils.py
+-rw-rw-rw-   0        0        0       23 2023-06-12 23:17:41.000000 mlplatformutils-0.9.5.5/src/mlplatformutils/core/version.py
+drwxrwxrwx   0        0        0        0 2023-06-12 23:17:47.501166 mlplatformutils-0.9.5.5/src/mlplatformutils.egg-info/
+-rw-rw-rw-   0        0        0     6719 2023-06-12 23:17:47.000000 mlplatformutils-0.9.5.5/src/mlplatformutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      688 2023-06-12 23:17:47.000000 mlplatformutils-0.9.5.5/src/mlplatformutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 23:17:47.000000 mlplatformutils-0.9.5.5/src/mlplatformutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      103 2023-06-12 23:17:47.000000 mlplatformutils-0.9.5.5/src/mlplatformutils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-12 23:17:47.000000 mlplatformutils-0.9.5.5/src/mlplatformutils.egg-info/top_level.txt
```

### Comparing `mlplatformutils-0.9.5/PKG-INFO` & `mlplatformutils-0.9.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlplatformutils
-Version: 0.9.5
+Version: 0.9.5.5
 Author: Keshav Singh
 Author-email: keshav_singh@hotmail.com
 License: MIT
 Keywords: mlplatformutils
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
```

### Comparing `mlplatformutils-0.9.5/setup.py` & `mlplatformutils-0.9.5.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 else:
     long_description="#DESC"
 
 setup(
     name='mlplatformutils',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='0.9.5',
+    version='0.9.5.5',
     license='MIT',
     classifiers=[
         'Programming Language :: Python :: 3.8'
     ],
     author='Keshav Singh',
     author_email='keshav_singh@hotmail.com',
     packages=find_packages('src'),
```

### Comparing `mlplatformutils-0.9.5/src/mlplatformutils/core/app_insights_logger.py` & `mlplatformutils-0.9.5.5/src/mlplatformutils/core/app_insights_logger.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.9.5/src/mlplatformutils/core/freshnessutils.py` & `mlplatformutils-0.9.5.5/src/mlplatformutils/core/freshnessutils.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.9.5/src/mlplatformutils/core/lineagegraph.py` & `mlplatformutils-0.9.5.5/src/mlplatformutils/core/lineagegraph.py`

 * *Files 0% similar despite different names*

```diff
@@ -185,15 +185,15 @@
             traceback.print_exc()
             raise ValueError("Failed to QUERY Cosmos Gremlin graph!")
 
         
     def update_lineage_graph(self,run_id,pipeline_step_name,properties):
         try:
             query = "g.V().hasLabel('amlrun').has('RUN_ID', '"+run_id+"').has('PIPELINE_STEP_NAME', '"+pipeline_step_name+"').values('id')"
-            documentIds = self.query_graph(query)[0]
+            documentIds = self.query_graph(query)
             if documentIds:
                 documentId = documentIds[0]
                 self.update_vertex(documentId,properties)
             else:
                 print('Document Does not Exist!')
             return
         except Exception as e:
@@ -211,14 +211,14 @@
 
             dest_query = "g.V().hasLabel('amlrun').has('RUN_ID', '"+run_id+"').has('PIPELINE_STEP_NAME', '"+dest_pipeline_step_name+"').values('id')"
             dest_doc_ids = self.query_graph(dest_query)
             if dest_doc_ids:
                 dest_doc_id = dest_doc_ids[0]
             else:
                 print('Destination DocumentId doest not Exits!')
-                
+
             self.insert_edges(source_doc_id, dest_doc_id,"DependendsOn", None)
             return
         except Exception as e:
             traceback.print_exc()
             raise ValueError("Failed to connect lineage graph!")
```

### Comparing `mlplatformutils-0.9.5/src/mlplatformutils/core/pandascoreutils.py` & `mlplatformutils-0.9.5.5/src/mlplatformutils/core/pandascoreutils.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.9.5/src/mlplatformutils/core/pandasutils.py` & `mlplatformutils-0.9.5.5/src/mlplatformutils/core/pandasutils.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.9.5/src/mlplatformutils/core/platformutils.py` & `mlplatformutils-0.9.5.5/src/mlplatformutils/core/platformutils.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.9.5/src/mlplatformutils/core/sparkcoreutils.py` & `mlplatformutils-0.9.5.5/src/mlplatformutils/core/sparkcoreutils.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.9.5/src/mlplatformutils/core/sparkutils.py` & `mlplatformutils-0.9.5.5/src/mlplatformutils/core/sparkutils.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.9.5/src/mlplatformutils.egg-info/PKG-INFO` & `mlplatformutils-0.9.5.5/src/mlplatformutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlplatformutils
-Version: 0.9.5
+Version: 0.9.5.5
 Author: Keshav Singh
 Author-email: keshav_singh@hotmail.com
 License: MIT
 Keywords: mlplatformutils
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
```

### Comparing `mlplatformutils-0.9.5/src/mlplatformutils.egg-info/SOURCES.txt` & `mlplatformutils-0.9.5.5/src/mlplatformutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

