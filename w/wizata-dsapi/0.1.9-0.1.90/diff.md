# Comparing `tmp/wizata-dsapi-0.1.9.tar.gz` & `tmp/wizata-dsapi-0.1.90.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wizata-dsapi-0.1.9.tar", last modified: Thu Apr 13 18:30:46 2023, max compression
+gzip compressed data, was "wizata-dsapi-0.1.90.tar", last modified: Tue Jun 13 07:39:26 2023, max compression
```

## Comparing `wizata-dsapi-0.1.9.tar` & `wizata-dsapi-0.1.90.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 18:30:46.558856 wizata-dsapi-0.1.9/
--rw-rw-rw-   0        0        0    11556 2023-03-17 16:15:58.000000 wizata-dsapi-0.1.9/LICENSE.txt
--rw-rw-rw-   0        0        0      246 2023-04-13 18:30:46.557865 wizata-dsapi-0.1.9/PKG-INFO
--rw-rw-rw-   0        0        0      253 2023-03-17 16:15:58.000000 wizata-dsapi-0.1.9/README.rst
--rw-rw-rw-   0        0        0       42 2023-04-13 18:30:46.559353 wizata-dsapi-0.1.9/setup.cfg
--rw-rw-rw-   0        0        0     1241 2023-04-13 18:30:41.000000 wizata-dsapi-0.1.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-13 18:30:46.534553 wizata-dsapi-0.1.9/wizata_dsapi/
--rw-rw-rw-   0        0        0      756 2023-04-13 17:52:10.000000 wizata-dsapi-0.1.9/wizata_dsapi/__init__.py
--rw-rw-rw-   0        0        0      632 2023-03-24 09:46:21.000000 wizata-dsapi-0.1.9/wizata_dsapi/api_dto.py
--rw-rw-rw-   0        0        0     2958 2023-04-10 07:55:31.000000 wizata-dsapi-0.1.9/wizata_dsapi/dataframe_toolkit.py
--rw-rw-rw-   0        0        0     1856 2023-04-03 07:22:42.000000 wizata-dsapi-0.1.9/wizata_dsapi/ds_dataframe.py
--rw-rw-rw-   0        0        0     2846 2023-03-21 09:56:23.000000 wizata-dsapi-0.1.9/wizata_dsapi/dsapi_json_encoder.py
--rw-rw-rw-   0        0        0    13455 2023-04-13 15:54:05.000000 wizata-dsapi-0.1.9/wizata_dsapi/execution.py
--rw-rw-rw-   0        0        0     3555 2023-04-06 06:19:02.000000 wizata-dsapi-0.1.9/wizata_dsapi/experiment.py
--rw-rw-rw-   0        0        0     5447 2023-04-06 06:19:02.000000 wizata-dsapi-0.1.9/wizata_dsapi/mlmodel.py
--rw-rw-rw-   0        0        0     1594 2023-04-06 06:19:02.000000 wizata-dsapi-0.1.9/wizata_dsapi/model_toolkit.py
--rw-rw-rw-   0        0        0     2136 2023-03-27 08:16:15.000000 wizata-dsapi-0.1.9/wizata_dsapi/plot.py
--rw-rw-rw-   0        0        0     9756 2023-04-10 07:55:31.000000 wizata-dsapi-0.1.9/wizata_dsapi/request.py
--rw-rw-rw-   0        0        0     6914 2023-04-03 07:22:42.000000 wizata-dsapi-0.1.9/wizata_dsapi/script.py
--rw-rw-rw-   0        0        0      392 2023-04-13 17:47:12.000000 wizata-dsapi-0.1.9/wizata_dsapi/sql_dto.py
--rw-rw-rw-   0        0        0     3563 2023-04-13 15:54:05.000000 wizata-dsapi-0.1.9/wizata_dsapi/template.py
--rw-rw-rw-   0        0        0      952 2023-04-13 17:47:12.000000 wizata-dsapi-0.1.9/wizata_dsapi/twin.py
--rw-rw-rw-   0        0        0     2256 2023-04-13 18:30:41.000000 wizata-dsapi-0.1.9/wizata_dsapi/twinregistration.py
--rw-rw-rw-   0        0        0      489 2023-03-27 08:16:15.000000 wizata-dsapi-0.1.9/wizata_dsapi/wizard_function.py
--rw-rw-rw-   0        0        0    33193 2023-04-07 15:57:41.000000 wizata-dsapi-0.1.9/wizata_dsapi/wizata_dsapi_client.py
-drwxrwxrwx   0        0        0        0 2023-04-13 18:30:46.555384 wizata-dsapi-0.1.9/wizata_dsapi.egg-info/
--rw-rw-rw-   0        0        0      246 2023-04-13 18:30:46.000000 wizata-dsapi-0.1.9/wizata_dsapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      703 2023-04-13 18:30:46.000000 wizata-dsapi-0.1.9/wizata_dsapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 18:30:46.000000 wizata-dsapi-0.1.9/wizata_dsapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      555 2023-04-13 18:30:46.000000 wizata-dsapi-0.1.9/wizata_dsapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-13 18:30:46.000000 wizata-dsapi-0.1.9/wizata_dsapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-13 07:39:26.859189 wizata-dsapi-0.1.90/
+-rw-rw-rw-   0        0        0    11556 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.90/LICENSE.txt
+-rw-rw-rw-   0        0        0      177 2023-06-13 07:39:26.858205 wizata-dsapi-0.1.90/PKG-INFO
+-rw-rw-rw-   0        0        0      323 2023-05-24 07:05:28.000000 wizata-dsapi-0.1.90/README.rst
+-rw-rw-rw-   0        0        0       42 2023-06-13 07:39:26.859685 wizata-dsapi-0.1.90/setup.cfg
+-rw-rw-rw-   0        0        0     1242 2023-06-13 07:39:17.000000 wizata-dsapi-0.1.90/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 07:39:26.827240 wizata-dsapi-0.1.90/wizata_dsapi/
+-rw-rw-rw-   0        0        0      933 2023-06-13 07:36:28.000000 wizata-dsapi-0.1.90/wizata_dsapi/__init__.py
+-rw-rw-rw-   0        0        0      632 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.90/wizata_dsapi/api_dto.py
+-rw-rw-rw-   0        0        0     2958 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.90/wizata_dsapi/dataframe_toolkit.py
+-rw-rw-rw-   0        0        0     5714 2023-06-08 15:23:14.000000 wizata-dsapi-0.1.90/wizata_dsapi/datapoint.py
+-rw-rw-rw-   0        0        0     1877 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.90/wizata_dsapi/ds_dataframe.py
+-rw-rw-rw-   0        0        0     2846 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.90/wizata_dsapi/dsapi_json_encoder.py
+-rw-rw-rw-   0        0        0    14612 2023-06-13 07:36:51.000000 wizata-dsapi-0.1.90/wizata_dsapi/execution.py
+-rw-rw-rw-   0        0        0     3810 2023-06-08 07:54:01.000000 wizata-dsapi-0.1.90/wizata_dsapi/experiment.py
+-rw-rw-rw-   0        0        0     6159 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.90/wizata_dsapi/mlmodel.py
+-rw-rw-rw-   0        0        0     1594 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.90/wizata_dsapi/model_toolkit.py
+-rw-rw-rw-   0        0        0    11227 2023-06-12 20:23:50.000000 wizata-dsapi-0.1.90/wizata_dsapi/pipeline.py
+-rw-rw-rw-   0        0        0     2136 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.90/wizata_dsapi/plot.py
+-rw-rw-rw-   0        0        0    13575 2023-06-12 20:23:50.000000 wizata-dsapi-0.1.90/wizata_dsapi/request.py
+-rw-rw-rw-   0        0        0     8716 2023-06-12 20:23:50.000000 wizata-dsapi-0.1.90/wizata_dsapi/script.py
+-rw-rw-rw-   0        0        0     3929 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.90/wizata_dsapi/template.py
+-rw-rw-rw-   0        0        0     2597 2023-06-08 07:54:01.000000 wizata-dsapi-0.1.90/wizata_dsapi/twin.py
+-rw-rw-rw-   0        0        0     2701 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.90/wizata_dsapi/twinregistration.py
+-rw-rw-rw-   0        0        0      489 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.90/wizata_dsapi/wizard_function.py
+-rw-rw-rw-   0        0        0    54309 2023-06-12 21:07:08.000000 wizata-dsapi-0.1.90/wizata_dsapi/wizata_dsapi_client.py
+drwxrwxrwx   0        0        0        0 2023-06-13 07:39:26.855716 wizata-dsapi-0.1.90/wizata_dsapi.egg-info/
+-rw-rw-rw-   0        0        0      177 2023-06-13 07:39:26.000000 wizata-dsapi-0.1.90/wizata_dsapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      730 2023-06-13 07:39:26.000000 wizata-dsapi-0.1.90/wizata_dsapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 07:39:26.000000 wizata-dsapi-0.1.90/wizata_dsapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      555 2023-06-13 07:39:26.000000 wizata-dsapi-0.1.90/wizata_dsapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-13 07:39:26.000000 wizata-dsapi-0.1.90/wizata_dsapi.egg-info/top_level.txt
```

### Comparing `wizata-dsapi-0.1.9/LICENSE.txt` & `wizata-dsapi-0.1.90/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.9/setup.py` & `wizata-dsapi-0.1.90/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='wizata-dsapi',
-    version='0.1.9',
+    version='0.1.90',
     description='Wizata Data Science Toolkit',
     author='Wizata S.A.',
     author_email='info@wizata.com',
     packages=['wizata_dsapi'],
     install_requires=[
         'dill==0.3.6',
         'pandas==1.5.3',
```

### Comparing `wizata-dsapi-0.1.9/wizata_dsapi/api_dto.py` & `wizata-dsapi-0.1.90/wizata_dsapi/api_dto.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.9/wizata_dsapi/dataframe_toolkit.py` & `wizata-dsapi-0.1.90/wizata_dsapi/dataframe_toolkit.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.9/wizata_dsapi/ds_dataframe.py` & `wizata-dsapi-0.1.90/wizata_dsapi/ds_dataframe.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,21 +8,21 @@
     A DS Dataframe is a definition of a pandas Dataframe that can be stored and shared on Wizata.
 
     :ivar df_id: The UUID of the dataframe.
     :ivar generatedById: The UUID of the Execution from which the dataframe was created.
     :ivar dataframe: Pandas Dataframe.
     """
 
-    def __init__(self, df_id=None):
+    def __init__(self, df_id=None, dataframe=None):
         if df_id is None:
             self.df_id = uuid.uuid4()
         else:
             self.df_id = df_id
         self.generatedById = None
-        self.dataframe = None
+        self.dataframe = dataframe
 
     def api_id(self) -> str:
         """
         Id of the dataframe (df_id)
 
         :return: string formatted UUID of the dataframe.
         """
```

### Comparing `wizata-dsapi-0.1.9/wizata_dsapi/dsapi_json_encoder.py` & `wizata-dsapi-0.1.90/wizata_dsapi/dsapi_json_encoder.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.9/wizata_dsapi/execution.py` & `wizata-dsapi-0.1.90/wizata_dsapi/execution.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,22 +2,32 @@
 import pickle
 import uuid
 
 import string
 import random
 import pandas
 import wizata_dsapi
+from enum import Enum
 
 from .dataframe_toolkit import df_to_json, df_from_json
 from .api_dto import ApiDto
 from .ds_dataframe import DSDataFrame
 from .mlmodel import MLModel
 from .plot import Plot
 from .request import Request
 from .script import Script
+from .pipeline import Pipeline
+
+
+class ExecutionStatus(Enum):
+    RECEIVED = "received"
+    QUEUED = "queued"
+    STARTED = "started"
+    COMPLETED = "completed"
+    FAILED = "failed"
 
 
 class Execution(ApiDto):
     """
     Execution Context defining an experimentation historical run.
 
     Execution can be run in the platform or directly within your script.
@@ -74,14 +84,16 @@
         self.script = None
         self.request = None
         self.properties = None
         self.input_ds_dataframe = None
         self.ml_model = None
         self.function = None
         self.isAnomalyDetection = False
+        self.pipeline = None
+        self.status = None
 
         # created/updated
         self.createdById = None
         self.createdDate = None
         self.updatedById = None
         self.updatedDate = None
 
@@ -212,14 +224,16 @@
             obj["dataframe"] = df_to_json(self.dataframe)
         if self.input_ds_dataframe is not None:
             obj["dataframeId"] = str(self.input_ds_dataframe.df_id)
         if self.script is not None:
             obj["scriptId"] = str(self.script.script_id)
         if self.ml_model is not None:
             obj["mlModelId"] = str(self.ml_model.model_id)
+        if self.pipeline is not None:
+            obj["pipelineId"] = str(self.pipeline.pipeline_id)
         if self.function is not None:
             obj["function"] = self.function
         if self.isAnomalyDetection:
             obj["isAnomalyDetection"] = str(True)
         if self.plots is not None:
             plots_ids = []
             for plot in self.plots:
@@ -246,14 +260,16 @@
             obj["createdDate"] = self.createdDate
         if self.updatedById is not None:
             obj["updatedById"] = self.updatedById
         if self.updatedDate is not None:
             obj["updatedDate"] = self.updatedDate
         if self.warnings is not None:
             obj["warnings"] = self.warnings
+        if self.status is not None and isinstance(self.status, ExecutionStatus):
+            obj["status"] = self.status.value
         return obj
 
     def from_json(self, obj):
         """
         Load an execution from a stored JSON model.
         :param obj: dictionnary representing an execution.
         """
@@ -261,18 +277,18 @@
             self.execution_id = uuid.UUID(obj["id"])
         if "experimentId" in obj.keys() and obj["experimentId"] is not None:
             self.experiment_id = uuid.UUID(obj["experimentId"])
         if "request" in obj.keys() and obj["request"] is not None:
             self.request = Request()
             if isinstance(obj["request"], str):
                 self.request.from_json(json.loads(obj["request"]))
-                self.add_properties(json.loads(obj["request"]))
+                self.copy_properties(json.loads(obj["request"]))
             else:
                 self.request.from_json(obj["request"])
-                self.add_properties(obj["request"])
+                self.copy_properties(obj["request"])
         if "properties" in obj.keys() and obj["properties"] is not None:
             if isinstance(obj["properties"], str):
                 self.add_properties(json.loads(obj["properties"]))
             else:
                 self.add_properties(obj["properties"])
         if "dataframe" in obj.keys() and obj["dataframe"] is not None:
             if isinstance(obj["dataframe"], str):
@@ -280,14 +296,17 @@
             else:
                 self.dataframe = df_from_json(obj["dataframe"])
         elif "dataframeId" in obj.keys() and obj["dataframeId"] is not None:
             self.input_ds_dataframe = DSDataFrame(df_id=uuid.UUID(obj["dataframeId"]))
         if "scriptId" in obj.keys() and obj["scriptId"] is not None:
             self.script = Script()
             self.script.script_id = uuid.UUID(obj["scriptId"])
+        if "pipelineId" in obj.keys() and obj["pipelineId"] is not None:
+            self.pipeline = Pipeline()
+            self.pipeline.pipeline_id = uuid.UUID(obj["pipelineId"])
         if "mlModelId" in obj.keys() and obj["mlModelId"] is not None:
             self.ml_model = MLModel()
             self.ml_model.model_id = uuid.UUID(obj["mlModelId"])
         if "function" in obj.keys() and obj["function"] is not None:
             self.function = obj["function"]
         if "isAnomalyDetection" in obj.keys() and obj["isAnomalyDetection"] is not None:
             if isinstance(obj["isAnomalyDetection"], bool):
@@ -305,30 +324,44 @@
         if "warnings" in obj.keys() and obj["warnings"] is not None:
             self.warnings = obj["warnings"]
         if "anomaliesList" in obj.keys() and obj["anomaliesList"] is not None:
             if isinstance(obj["anomaliesList"], str):
                 self.anomalies = json.loads(obj["anomaliesList"])
             else:
                 self.anomalies = obj["anomaliesList"]
+        if "status" in obj.keys():
+            self.status = ExecutionStatus(str(obj["status"]))
 
     def to_pickle(self):
         """
         Convert the Execution to a pickle object.
         :return: Pickle object.
         """
         return pickle.dumps(self)
 
-    def add_properties(self, obj: dict, replace=True):
+    def add_properties(self, obj: dict):
         """
         load properties from a dictionary
 
         :param obj: dictionary with potential properties
         """
+        for key in obj.keys():
+            if self.properties is None:
+                self.properties = {}
+            self.properties[key] = obj[key]
+
+    def copy_properties(self, obj: dict):
+        """
+        copy properties from a dictionary originating from a Request object.
+        filtering on specific properties (Execution.keys)
+
+        :param obj: dictionary with potential properties
+        """
         for key in Execution.keys:
-            if key in obj and (replace or key not in self.properties):
+            if key in obj:
                 if self.properties is None:
                     self.properties = {}
                 self.properties[key] = obj[key]
 
     def get_interval(self) -> int:
         """
         Determine interval from either request, properties or loaded dataframe.
```

### Comparing `wizata-dsapi-0.1.9/wizata_dsapi/experiment.py` & `wizata-dsapi-0.1.90/wizata_dsapi/experiment.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
         if experiment_id is None:
             self.experiment_id = uuid.uuid4()
         else:
             self.experiment_id = experiment_id
         self.key = key
         self.name = name
         self.description = description
+        self.templateId = None
         self.twinId = None
         self.twinGraphId = None
         self.createdById = None
         self.createdDate = None
         self.updatedById = None
         self.updatedDate = None
 
@@ -49,14 +50,16 @@
         }
         if self.key is not None:
             obj["key"] = str(self.key)
         if self.name is not None:
             obj["name"] = str(self.name)
         if self.description is not None:
             obj["description"] = str(self.description)
+        if self.templateId is not None:
+            obj["templateId"] = str(self.templateId)
         if self.twinId is not None:
             obj["twinId"] = str(self.twinId)
         if self.twinGraphId is not None:
             obj["twinGraphId"] = str(self.twinGraphId)
         if self.createdById is not None:
             obj["createdById"] = str(self.createdById)
         if self.createdDate is not None:
@@ -75,18 +78,20 @@
             self.experiment_id = uuid.UUID(obj["id"])
         if "key" in obj.keys() and obj["key"] is not None:
             self.key = obj["key"]
         if "name" in obj.keys() and obj["name"] is not None:
             self.name = obj["name"]
         if "description" in obj.keys() and obj["description"] is not None:
             self.description = obj["description"]
+        if "templateId" in obj.keys() and obj["templateId"] is not None:
+            self.templateId = obj["templateId"]
         if "twinId" in obj.keys() and obj["twinId"] is not None:
             self.twinId = obj["twinId"]
         if "twinGraphId" in obj.keys() and obj["twinGraphId"] is not None:
-            self.twinId = obj["twinGraphId"]
+            self.twinGraphId = obj["twinGraphId"]
         if "createdById" in obj.keys() and obj["createdById"] is not None:
             self.createdById = obj["createdById"]
         if "createdDate" in obj.keys() and obj["createdDate"] is not None:
             self.createdDate = obj["createdDate"]
         if "updatedById" in obj.keys() and obj["updatedById"] is not None:
             self.updatedById = obj["updatedById"]
         if "updatedDate" in obj.keys() and obj["updatedDate"] is not None:
```

### Comparing `wizata-dsapi-0.1.9/wizata_dsapi/mlmodel.py` & `wizata-dsapi-0.1.90/wizata_dsapi/mlmodel.py`

 * *Files 13% similar despite different names*

```diff
@@ -105,21 +105,33 @@
         if "inputColumns" in obj.keys():
             self.input_columns = json.loads(obj["inputColumns"])
         if "outputColumns" in obj.keys():
             self.output_columns = json.loads(obj["outputColumns"])
         if "labelCount" in obj.keys():
             self.label_counts = int(obj["labelCount"])
         if "hasAnomalies" in obj.keys():
-            self.has_anomalies = bool(obj["hasAnomalies"])
+            if isinstance(obj["hasAnomalies"], str) and obj["hasAnomalies"].lower() == "false":
+                self.has_anomalies = False
+            else:
+                self.has_anomalies = bool(obj["hasAnomalies"])
         if "hasTargetFeat" in obj.keys():
-            self.has_target_feat = bool(obj["hasTargetFeat"])
+            if isinstance(obj["hasTargetFeat"], str) and obj["hasTargetFeat"].lower() == "false":
+                self.has_target_feat = False
+            else:
+                self.has_target_feat = bool(obj["hasTargetFeat"])
         if "needExactColumnNumbers" in obj.keys():
-            self.needExactColumnNumbers = bool(obj["needExactColumnNumbers"])
+            if isinstance(obj["needExactColumnNumbers"], str) and obj["needExactColumnNumbers"].lower() == "false":
+                self.needExactColumnNumbers = False
+            else:
+                self.needExactColumnNumbers = bool(obj["needExactColumnNumbers"])
         if "needExactColumnNames" in obj.keys():
-            self.needExactColumnNames = bool(obj["needExactColumnNames"])
+            if isinstance(obj["needExactColumnNames"], str) and obj["needExactColumnNames"].lower() == "false":
+                self.needExactColumnNames = False
+            else:
+                self.needExactColumnNames = bool(obj["needExactColumnNames"])
 
     def get_sample_payload(self):
         """
         Get a JSON formatted sample payload to call the ML Model.
         :return: JSON formatted sample payload.
         """
         pl_columns = {"timestamp": "[timestamp]"}
```

### Comparing `wizata-dsapi-0.1.9/wizata_dsapi/model_toolkit.py` & `wizata-dsapi-0.1.90/wizata_dsapi/model_toolkit.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.9/wizata_dsapi/plot.py` & `wizata-dsapi-0.1.90/wizata_dsapi/plot.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.9/wizata_dsapi/request.py` & `wizata-dsapi-0.1.90/wizata_dsapi/request.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 import uuid
-from datetime import datetime, timedelta
+from datetime import datetime, timedelta, timezone
 
 
 class Request:
     """
     A Request to fetch dataframes from Wizata App.
 
     To execute the request please use a DS API client.
 
     :ivar equipments: List of Equipments containing Digital Twin item and datapoints to fetch.
+
+    :ivar template_id: UUID of the template.
+    :ivar template: str unique id of the template.
+    :ivar twin_id: UUID of the Digital Twin.
+    :ivar twin: str hardware id of the Digital Twin.
+
     :ivar start: Datetime defining beginning of period.
     :ivar end: Datetime defining end of period.
     :ivar aggregation: Aggregation method to fetch, accept "mean" and "stddev".
     :ivar interval: Interval in seconds between each aggregation.
     :ivar filters: Filter to apply on the query (not yet fully implemented).
     :ivar connections: Connections rules between equipment to align data in time (not yet fully implemented).
     :ivar null: By default at 'drop' and dropping NaN values. If not intended behavior please set it to 'ignore' or 'all'.
@@ -20,28 +26,51 @@
 
     def __init__(self,
                  datapoints=None,
                  start=None,
                  end=None,
                  agg_method='mean',
                  interval=None,
-                 null='drop'):
+                 null='drop',
+                 template_id=None,
+                 template=None,
+                 twin_id=None,
+                 twin=None,
+                 request_id=None,
+                 filters=None,
+                 options=None):
+        if request_id is None:
+            request_id = uuid.uuid4()
+        self.request_id = request_id
         self.function = None
+
+        # Equipments & Data Points
         self.equipments = []
         if datapoints is not None:
             self.add_datapoints(datapoints)
 
+        # Template & Registration
+        self.template = None
+        self.select_template(
+             template_id=template_id,
+             template_key=template,
+             twin_id=twin_id,
+             twin_hardware_id=twin
+        )
+
         self.start = start
         self.end = end
 
         self.aggregation = agg_method
         if interval is not None:
             self.interval = int(interval) / 1000
 
-        self.filters = None
+        self.filters = filters
+        self.options = options
+
         self.on_off_sensor = None
         self.restart_time = None
         self.sensitivity = None
         self.dataframe = None
         self.extra_data = None
         self.target_feat = None
         self.connections = None
@@ -52,14 +81,16 @@
     def prepare(self):
         """
         prepare a dict JSON compatible only for the QUERY part of the request.
 
         :return: a dict JSON compatible
         """
         query = {}
+        if self.request_id is not None:
+            query["id"] = str(self.request_id)
         if self.equipments is not None:
             query["equipments_list"] = self.equipments
         else:
             raise KeyError("Missing data points inside the query - add_datapoints")
         if self.start is not None and self.end is not None:
             query["timeframe"] = {
                 "start": self.__format_date(self.start),
@@ -72,14 +103,20 @@
                 "agg_method": self.aggregation,
                 "interval": self.interval * 1000
             }
         else:
             raise KeyError("Missing aggregations information inside the request")
         if self.null is not None and self.null != 'drop':
             query['null'] = self.null
+        if self.template is not None:
+            query['template'] = self.template
+        if self.filters is not None:
+            query['filters'] = self.filters
+        if self.options is not None:
+            query['options'] = self.options
         return query
 
     def __format_date(self, dt_to_format):
         if isinstance(dt_to_format, datetime):
             millisec = dt_to_format.timestamp() * 1000
             return int(millisec)
         else:
@@ -137,21 +174,56 @@
         :param method: 'mean' or 'stddev'
         :param interval: interval in ms (will be stored in seconds)
         """
         self.aggregation = method
         if interval is not None:
             self.interval = int(interval) / 1000
 
+    def select_template(self,
+                        template_id=None,
+                        template_key=None,
+                        twin_id=None,
+                        twin_hardware_id=None):
+        """
+        Select a template and its registration.
+        :param template_id: template UUID
+        :param template_key: template key ( ignored if template_id specified )
+        :param twin_id: Digital Twin UUID
+        :param twin_hardware_id: hardware ID of Digital Twin ( ignored if twin_id specified )
+        """
+        if template_id is None and template_key is None and twin_id is None and twin_hardware_id is None:
+            self.template = None
+            return
+        else:
+            self.template = {}
+
+            if template_id is not None:
+                self.template['template_id'] = uuid.UUID(template_id)
+            elif template_key is not None:
+                self.template['template_key'] = str(template_key)
+            else:
+                raise ValueError('A twin can only be specified with its template')
+
+            if twin_id is not None:
+                self.template['twin_id'] = uuid.UUID(twin_id)
+            elif twin_hardware_id is not None:
+                self.template['twin_hardware_id'] = str(twin_hardware_id)
+            else:
+                raise ValueError('A template can only be specified with its registered twin')
+
     def to_json(self):
         """
         convert to a dict JSON compatible for all properties. For query only, use prepare().
 
         :return: a dict JSON compatible
         """
+
+        # Prepare is 'to_json' without future obsolete properties
         obj = self.prepare()
+
         if self.target_feat is not None:
             obj["target_feat"] = {
                 "sensor": self.target_feat["sensor"],
                 "operator": self.target_feat["operator"],
                 "threshold": self.target_feat["threshold"]
             }
         if self.on_off_sensor is not None and self.restart_time is not None:
@@ -170,45 +242,74 @@
 
     def from_json(self, json_data):
         """
         load a request based on dict from a JSON file.
 
         :param json_data: JSON formatted dictionnary object representing a query.
         """
+        if "id" in json_data.keys():
+            self.request_id = uuid.UUID(json_data["id"])
+
         if "name" in json_data.keys():
             self.name = json_data["name"]
 
-        if "equipments_list" not in json_data.keys():
-            raise KeyError("No 'twin unit' nor 'data points' selected please select some and re-try.")
-        self.equipments = json_data["equipments_list"]
+        found_dps = False
+        if "equipments_list" in json_data.keys():
+            self.equipments = json_data["equipments_list"]
+            for equipment in self.equipments:
+                if "datapoints" not in equipment.keys():
+                    raise KeyError("No 'data points' have been provided for equipment with id '" +
+                                   str(equipment["id"]) + "'")
+                else:
+                    found_dps = True
+        elif "datapoints" in json_data.keys():
+            equipment = {"datapoints": []}
+            for datapoint in json_data["datapoints"]:
+                equipment["datapoints"].append(datapoint)
+            self.equipments.append(equipment)
+            found_dps = True
+
+        if "template" in json_data.keys():
+            self.template = json_data["template"]
+            found_dps = True
+
+        if not found_dps:
+            raise KeyError('no equipments_list datapoints, nor template specified inside the request.')
 
         if "timeframe" not in json_data.keys():
             raise KeyError("No 'time range' have been selected, please set it up and re-try.")
 
         if "start" not in json_data["timeframe"].keys():
             raise KeyError("No 'start time' have been selected, please set it up and re-try.")
-        self.start = datetime.fromtimestamp(json_data["timeframe"]["start"] / 1000)
+        self.start = datetime.fromtimestamp(json_data["timeframe"]["start"] / 1000, timezone.utc)
 
         if "end" not in json_data["timeframe"].keys():
             raise KeyError("No 'end time' have been selected, please set it up and re-try.")
-        self.end = datetime.fromtimestamp(json_data["timeframe"]["end"] / 1000)
+        self.end = datetime.fromtimestamp(json_data["timeframe"]["end"] / 1000, timezone.utc)
 
         if "aggregations" not in json_data.keys():
             raise KeyError("No 'aggregations' have been selected, please set it up and re-try.")
 
         if "agg_method" not in json_data["aggregations"].keys():
             raise KeyError("No 'Aggregation Method' have been selected, please set it up and re-try.")
         self.aggregation = json_data["aggregations"]["agg_method"]
 
         if "interval" not in json_data["aggregations"].keys():
             raise KeyError("No 'Aggregation Interval' have been selected, please set it up and re-try.")
         self.interval = int(json_data["aggregations"]["interval"] / 1000)
 
         if "filters" in json_data.keys():
             self.filters = json_data["filters"]
+        else:
+            self.filters = {}
+
+        if "options" in json_data.keys():
+            self.options = json_data["options"]
+        else:
+            self.options = {}
 
         if "connections" in json_data.keys():
             self.connections = json_data["connections"]
 
         if "null" in json_data.keys():
             self.null = json_data["null"]
 
@@ -227,7 +328,8 @@
 
         if "sensitivity" in json_data.keys():
             self.sensitivity = json_data["sensitivity"]
 
         if "extra_data" in json_data.keys():
             self.extra_data = json_data["extra_data"]
 
+
```

### Comparing `wizata-dsapi-0.1.9/wizata_dsapi/script.py` & `wizata-dsapi-0.1.90/wizata_dsapi/script.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,14 +4,39 @@
 import os
 import types
 from .api_dto import ApiDto
 import inspect
 from collections import OrderedDict
 
 
+class ScriptConfig(ApiDto):
+    """
+    a script config defines execution properties for a specific script.
+    usually to define how a pipeline should call your script.
+
+    :ivar function: name of function referencing the script.
+    """
+
+    def __init__(self, function=None):
+        self.function = function
+
+    def from_json(self, obj):
+        if isinstance(obj, str):
+            self.function = obj
+            return
+        else:
+            if "function" in obj:
+                self.function = obj["function"]
+
+    def to_json(self):
+        obj = {
+            "function": self.function
+        }
+        return obj
+
 class Script(ApiDto):
     """
     A piece of python code that can either transform data, generate plot or train Machine Learning Models.
 
     Scripts once validated can be used from Python or directly inside Wizata App by users.
 
     :ivar script_id: The UUID of the ML Model.
@@ -114,29 +139,50 @@
             self.script_id = uuid.UUID(obj["id"])
         if "name" in obj.keys():
             self._name = obj["name"]
         if "description" in obj.keys():
             if obj["description"] != "None":
                 self.description = obj["description"]
         if "canGeneratePlot" in obj.keys():
-            self.canGeneratePlot = bool(obj["canGeneratePlot"])
+            if isinstance(obj["canGeneratePlot"], str) and obj["canGeneratePlot"].lower() == "false":
+                self.canGeneratePlot = False
+            else:
+                self.canGeneratePlot = bool(obj["canGeneratePlot"])
         if "canGenerateModel" in obj.keys():
-            self.canGenerateModel = bool(obj["canGenerateModel"])
+            if isinstance(obj["canGenerateModel"], str) and obj["canGenerateModel"].lower() == "false":
+                self.canGenerateModel = False
+            else:
+                self.canGenerateModel = bool(obj["canGenerateModel"])
         if "canGenerateData" in obj.keys():
-            self.canGenerateData = bool(obj["canGenerateData"])
+            if isinstance(obj["canGenerateData"], str) and obj["canGenerateData"].lower() == "false":
+                self.canGenerateData = False
+            else:
+                self.canGenerateData = bool(obj["canGenerateData"])
         if "status" in obj.keys():
             self.status = str(obj["status"]).lower()
         if "needExactColumnNumbers" in obj.keys():
-            self.needExactColumnNumbers = bool(obj["needExactColumnNumbers"])
+            if isinstance(obj["needExactColumnNumbers"], str) and obj["needExactColumnNumbers"].lower() == "false":
+                self.needExactColumnNumbers = False
+            else:
+                self.needExactColumnNumbers = bool(obj["needExactColumnNumbers"])
         if "needExactColumnNames" in obj.keys():
-            self.needExactColumnNames = bool(obj["needExactColumnNames"])
+            if isinstance(obj["needExactColumnNames"], str) and obj["needExactColumnNames"].lower() == "false":
+                self.needExactColumnNames = False
+            else:
+                self.needExactColumnNames = bool(obj["needExactColumnNames"])
         if "inputColumns" in obj.keys():
-            self.inputColumns = json.loads(obj["inputColumns"])
+            if obj["inputColumns"].lower() == "false":
+                self.inputColumns = False
+            else:
+                self.inputColumns = json.loads(obj["inputColumns"])
         if "outputColumns" in obj.keys():
-            self.outputColumns = json.loads(obj["outputColumns"])
+            if obj["outputColumns"].lower() == "false":
+                self.outputColumns = False
+            else:
+                self.outputColumns = json.loads(obj["outputColumns"])
 
     def copy(self, myfunction):
         """
         Copy your function code and decorators to a format executable by the Wizata App.
         :param myfunction: your function - pass the function itself as parameter
         """
```

### Comparing `wizata-dsapi-0.1.9/wizata_dsapi/template.py` & `wizata-dsapi-0.1.90/wizata_dsapi/template.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,23 @@
 import uuid
 import json
 from .api_dto import ApiDto
 
 
 class Template(ApiDto):
+    """
+    Template of a solution and/or asset.
+
+    :ivar template_id: UUID of the Template.
+    :ivar key: str unique id identifying the Template.
+    :ivar name: logical display name of the Template.
+    :ivar properties: list of Property { type , name } of the solution.
+
+    Properties only support type 'datapoint', 'float', 'integer' or 'string'
+    """
 
     def __init__(self, template_id=None, key=None, name=None, properties=None):
         if template_id is None:
             self.template_id = uuid.uuid4()
         else:
             self.template_id = template_id
         self.key = key
@@ -84,16 +94,17 @@
             if existing_property["name"] == property_value["name"]:
                 raise ValueError(f'property {property_value["name"]} already exists in template.')
         self.properties.append(property_value)
 
     def remove_property(self, name):
         """
         remove a property from the list based on its name
-        :param name: name of property to remove
+        :param name: property to remove
         """
         found_property = None
         for existing_property in self.properties:
             if existing_property["name"] == name:
                 found_property = existing_property
         if self.properties is not None and found_property is not None:
             self.properties.remove(found_property)
 
+
```

### Comparing `wizata-dsapi-0.1.9/wizata_dsapi/twinregistration.py` & `wizata-dsapi-0.1.90/wizata_dsapi/twinregistration.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,23 @@
 import uuid
 import json
 from .api_dto import ApiDto
 
 
 class TwinRegistration(ApiDto):
+    """
+    Registration of a Digital Twin on a solution Template.
+
+    :ivar twin_registration_id: UUID of the registration
+    :ivar twin_id: UUID of registered Digital Twin
+    :ivar template_id: UUID of the solution template.
+    :ivar properties: list of Properties { name , datapoint, float, integer, string }
+
+    A property must contains a name and the hardwareId of the datapoint or the value corresponding to the right type.
+    """
 
     def __init__(self, twin_registration_id=None, twin_id=None, template_id=None, properties=None):
         if twin_registration_id is None:
             self.twin_registration_id = uuid.uuid4()
         else:
             self.twin_registration_id = twin_registration_id
         self.twin_id = twin_id
@@ -33,18 +43,18 @@
         """
         Load the Registration entity from a dictionary.
 
         :param obj: Dict version of the Registration.
         """
         if "id" in obj.keys():
             self.twin_registration_id = uuid.UUID(obj["id"])
-        if "twin_id" in obj.keys() and obj["twin_id"] is not None:
-            self.twin_id = obj["twin_id"]
-        if "template_id" in obj.keys() and obj["template_id"] is not None:
-            self.template_id = obj["template_id"]
+        if "twinId" in obj.keys() and obj["twinId"] is not None:
+            self.twin_id = obj["twinId"]
+        if "templateId" in obj.keys() and obj["templateId"] is not None:
+            self.template_id = obj["templateId"]
         if "properties" in obj.keys() and obj["properties"] is not None:
             if isinstance(obj["properties"], str):
                 self.properties = json.loads(obj["properties"])
             else:
                 self.properties = obj["properties"]
 
     def to_json(self):
@@ -53,14 +63,14 @@
 
         :return: dictionary representation of the Registration object.
         """
         obj = {
             "id": str(self.twin_registration_id)
         }
         if self.twin_id is not None:
-            obj["twin_id"] = str(self.twin_id)
+            obj["twinId"] = str(self.twin_id)
         if self.template_id is not None:
-            obj["template_id"] = str(self.template_id)
+            obj["templateId"] = str(self.template_id)
         if self.properties is not None:
             obj["properties"] = json.dumps(self.properties)
         return obj
```

### Comparing `wizata-dsapi-0.1.9/wizata_dsapi.egg-info/SOURCES.txt` & `wizata-dsapi-0.1.90/wizata_dsapi.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 LICENSE.txt
 README.rst
 setup.py
 wizata_dsapi/__init__.py
 wizata_dsapi/api_dto.py
 wizata_dsapi/dataframe_toolkit.py
+wizata_dsapi/datapoint.py
 wizata_dsapi/ds_dataframe.py
 wizata_dsapi/dsapi_json_encoder.py
 wizata_dsapi/execution.py
 wizata_dsapi/experiment.py
 wizata_dsapi/mlmodel.py
 wizata_dsapi/model_toolkit.py
+wizata_dsapi/pipeline.py
 wizata_dsapi/plot.py
 wizata_dsapi/request.py
 wizata_dsapi/script.py
-wizata_dsapi/sql_dto.py
 wizata_dsapi/template.py
 wizata_dsapi/twin.py
 wizata_dsapi/twinregistration.py
 wizata_dsapi/wizard_function.py
 wizata_dsapi/wizata_dsapi_client.py
 wizata_dsapi.egg-info/PKG-INFO
 wizata_dsapi.egg-info/SOURCES.txt
```

### Comparing `wizata-dsapi-0.1.9/wizata_dsapi.egg-info/requires.txt` & `wizata-dsapi-0.1.90/wizata_dsapi.egg-info/requires.txt`

 * *Files identical despite different names*

