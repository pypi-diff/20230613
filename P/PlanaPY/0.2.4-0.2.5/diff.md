# Comparing `tmp/PlanaPY-0.2.4.tar.gz` & `tmp/PlanaPY-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PlanaPY-0.2.4.tar", last modified: Fri Jun  9 23:34:45 2023, max compression
+gzip compressed data, was "PlanaPY-0.2.5.tar", last modified: Mon Jun 12 23:16:31 2023, max compression
```

## Comparing `PlanaPY-0.2.4.tar` & `PlanaPY-0.2.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 23:34:45.384091 PlanaPY-0.2.4/
--rw-rw-rw-   0        0        0      286 2023-06-09 23:34:45.383094 PlanaPY-0.2.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-09 23:34:45.369589 PlanaPY-0.2.4/PlanaPY/
--rw-rw-rw-   0        0        0    13477 2023-06-09 23:09:30.000000 PlanaPY-0.2.4/PlanaPY/PlanaPY.py
--rw-rw-rw-   0        0        0       21 2023-06-09 20:22:08.000000 PlanaPY-0.2.4/PlanaPY/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 23:34:45.381101 PlanaPY-0.2.4/PlanaPY.egg-info/
--rw-rw-rw-   0        0        0      286 2023-06-09 23:34:45.000000 PlanaPY-0.2.4/PlanaPY.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      211 2023-06-09 23:34:45.000000 PlanaPY-0.2.4/PlanaPY.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 23:34:45.000000 PlanaPY-0.2.4/PlanaPY.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-06-09 23:34:45.000000 PlanaPY-0.2.4/PlanaPY.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-09 23:34:45.000000 PlanaPY-0.2.4/PlanaPY.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2023-06-06 05:35:28.000000 PlanaPY-0.2.4/README.md
--rw-rw-rw-   0        0        0       42 2023-06-09 23:34:45.385095 PlanaPY-0.2.4/setup.cfg
--rw-rw-rw-   0        0        0      485 2023-06-09 23:34:25.000000 PlanaPY-0.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 23:16:31.076651 PlanaPY-0.2.5/
+-rw-rw-rw-   0        0        0      286 2023-06-12 23:16:31.076651 PlanaPY-0.2.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-12 23:16:31.070490 PlanaPY-0.2.5/PlanaPY/
+-rw-rw-rw-   0        0        0    15821 2023-06-12 23:11:46.000000 PlanaPY-0.2.5/PlanaPY/PlanaPY.py
+-rw-rw-rw-   0        0        0       21 2023-06-09 20:22:08.000000 PlanaPY-0.2.5/PlanaPY/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 23:16:31.075656 PlanaPY-0.2.5/PlanaPY.egg-info/
+-rw-rw-rw-   0        0        0      286 2023-06-12 23:16:30.000000 PlanaPY-0.2.5/PlanaPY.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      211 2023-06-12 23:16:31.000000 PlanaPY-0.2.5/PlanaPY.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 23:16:30.000000 PlanaPY-0.2.5/PlanaPY.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-06-12 23:16:30.000000 PlanaPY-0.2.5/PlanaPY.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-12 23:16:30.000000 PlanaPY-0.2.5/PlanaPY.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2023-06-06 05:35:28.000000 PlanaPY-0.2.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-12 23:16:31.076651 PlanaPY-0.2.5/setup.cfg
+-rw-rw-rw-   0        0        0      485 2023-06-12 23:16:17.000000 PlanaPY-0.2.5/setup.py
```

### Comparing `PlanaPY-0.2.4/PlanaPY/PlanaPY.py` & `PlanaPY-0.2.5/PlanaPY/PlanaPY.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import requests
 from requests.structures import CaseInsensitiveDict
 import json
 import pandas as pd
 from time import gmtime, strftime
 import time
+import io 
 
 class AnaplanAPI: 
     def __init__(self):
         self.headers = CaseInsensitiveDict()
         self.headers['Content-Length'] = "0"
         self.token = ""
         self.response_results = dict()
@@ -235,14 +236,67 @@
         self.api.headers.pop('Content-Type')
         
         if self.resp.status_code == 204:
             print("Delete action {0} successfully ran in model {1}".format(file, model))
         
         return self.resp 
     
+    def get_export_actions(self, model, workspace):
+        exports_dict = {}
+        
+        model_id = self.models[(self.models.name == model) & (self.models.currentWorkspaceName == workspace)]['id'].iloc[0]
+        URL = self.api.api_url + "models/{0}/exports".format(model_id)
+        
+        actions = self.get_request(URL)['exports']
+        
+        for a in actions:
+            exports_dict[a['name']] = a
+        
+        return exports_dict
+        
+    def run_export_action(self, model, workspace, export):
+        self.api.headers['Content-Type'] = 'application/json'
+        model_id = self.models[(self.models.name == model) & (self.models.currentWorkspaceName == workspace)]['id'].iloc[0]
+        action_id = self.get_export_actions(model=model, workspace=workspace)[export]['id']
+        
+        URL = self.api.api_url + "models/{0}/exports/{1}/tasks".format(model_id, action_id)
+        body = {'localeName': 'en_US'}
+        
+        self.resp = requests.post(URL, headers=self.api.headers, json=body)
+        self.api.headers.pop('Content-Type')
+        
+        if self.resp.status_code == 204:
+            print("Export action {0} successfully ran in model {1}".format(file, model))
+        
+        return self.resp 
+    
+    def export_data(self, model, workspace, export):
+        model_id = self.models[(self.models.name == model) & (self.models.currentWorkspaceName == workspace)]['id'].iloc[0]
+        file_id = self.get_model_files(model=model, workspace = workspace)[export]['id']
+        
+        URL = self.api.api_url + "models/{0}/files/{1}/chunks".format(model_id, file_id)
+        
+        chunks = self.get_request(URL)['chunks']
+        
+        chunk_list = []
+        
+        for c in chunks:
+            chunk_id = c['id']
+            chunk_URL = self.api.api_url + "models/{0}/files/{1}/chunks/{2}".format(model_id, file_id, chunk_id)
+            chunk = requests.get(chunk_URL, headers = self.api.headers).content
+            df = pd.read_csv(io.StringIO(chunk.decode('utf-8')), header=None)
+            chunk_list.append(df)
+
+        all_chunks = pd.concat(chunk_list).reset_index()
+        all_chunks.columns = all_chunks.iloc[0]
+        all_chunks.drop(all_chunks.index[0], inplace=True)
+        all_chunks = all_chunks.iloc[:,1:]
+        
+        return all_chunks       
+        
     def change_model_status(self, model, workspace, status):
         model_id = self.models[(self.models.name == model) & (self.models.currentWorkspaceName == workspace)]['id'].iloc[0]
         URL = self.api.api_url + "models/{0}/onlineStatus".format(model_id)
         body = {'status': status}
         
         resp = self.put_request(URL, body)
```

