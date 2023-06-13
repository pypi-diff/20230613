# Comparing `tmp/wizata-dsapi-0.1.91.tar.gz` & `tmp/wizata-dsapi-0.1.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wizata-dsapi-0.1.91.tar", last modified: Tue Jun 13 13:16:00 2023, max compression
+gzip compressed data, was "wizata-dsapi-0.1.92.tar", last modified: Tue Jun 13 14:38:51 2023, max compression
```

## Comparing `wizata-dsapi-0.1.91.tar` & `wizata-dsapi-0.1.92.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 13:16:00.253064 wizata-dsapi-0.1.91/
--rw-rw-rw-   0        0        0    11556 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.91/LICENSE.txt
--rw-rw-rw-   0        0        0      177 2023-06-13 13:16:00.252072 wizata-dsapi-0.1.91/PKG-INFO
--rw-rw-rw-   0        0        0      323 2023-05-24 07:05:28.000000 wizata-dsapi-0.1.91/README.rst
--rw-rw-rw-   0        0        0       42 2023-06-13 13:16:00.253064 wizata-dsapi-0.1.91/setup.cfg
--rw-rw-rw-   0        0        0     1242 2023-06-13 13:15:50.000000 wizata-dsapi-0.1.91/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-13 13:16:00.224270 wizata-dsapi-0.1.91/wizata_dsapi/
--rw-rw-rw-   0        0        0      933 2023-06-13 07:36:28.000000 wizata-dsapi-0.1.91/wizata_dsapi/__init__.py
--rw-rw-rw-   0        0        0      632 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.91/wizata_dsapi/api_dto.py
--rw-rw-rw-   0        0        0     2958 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.91/wizata_dsapi/dataframe_toolkit.py
--rw-rw-rw-   0        0        0     5714 2023-06-08 15:23:14.000000 wizata-dsapi-0.1.91/wizata_dsapi/datapoint.py
--rw-rw-rw-   0        0        0     1877 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.91/wizata_dsapi/ds_dataframe.py
--rw-rw-rw-   0        0        0     2846 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.91/wizata_dsapi/dsapi_json_encoder.py
--rw-rw-rw-   0        0        0    14642 2023-06-13 13:15:50.000000 wizata-dsapi-0.1.91/wizata_dsapi/execution.py
--rw-rw-rw-   0        0        0     3810 2023-06-08 07:54:01.000000 wizata-dsapi-0.1.91/wizata_dsapi/experiment.py
--rw-rw-rw-   0        0        0     6159 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.91/wizata_dsapi/mlmodel.py
--rw-rw-rw-   0        0        0     1594 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.91/wizata_dsapi/model_toolkit.py
--rw-rw-rw-   0        0        0    11227 2023-06-12 20:23:50.000000 wizata-dsapi-0.1.91/wizata_dsapi/pipeline.py
--rw-rw-rw-   0        0        0     2136 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.91/wizata_dsapi/plot.py
--rw-rw-rw-   0        0        0    13575 2023-06-12 20:23:50.000000 wizata-dsapi-0.1.91/wizata_dsapi/request.py
--rw-rw-rw-   0        0        0     8716 2023-06-12 20:23:50.000000 wizata-dsapi-0.1.91/wizata_dsapi/script.py
--rw-rw-rw-   0        0        0     3929 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.91/wizata_dsapi/template.py
--rw-rw-rw-   0        0        0     2597 2023-06-08 07:54:01.000000 wizata-dsapi-0.1.91/wizata_dsapi/twin.py
--rw-rw-rw-   0        0        0     2701 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.91/wizata_dsapi/twinregistration.py
--rw-rw-rw-   0        0        0      489 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.91/wizata_dsapi/wizard_function.py
--rw-rw-rw-   0        0        0    54309 2023-06-12 21:07:08.000000 wizata-dsapi-0.1.91/wizata_dsapi/wizata_dsapi_client.py
-drwxrwxrwx   0        0        0        0 2023-06-13 13:16:00.250086 wizata-dsapi-0.1.91/wizata_dsapi.egg-info/
--rw-rw-rw-   0        0        0      177 2023-06-13 13:15:59.000000 wizata-dsapi-0.1.91/wizata_dsapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      730 2023-06-13 13:15:59.000000 wizata-dsapi-0.1.91/wizata_dsapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 13:15:59.000000 wizata-dsapi-0.1.91/wizata_dsapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      555 2023-06-13 13:15:59.000000 wizata-dsapi-0.1.91/wizata_dsapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-13 13:15:59.000000 wizata-dsapi-0.1.91/wizata_dsapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-13 14:38:51.717791 wizata-dsapi-0.1.92/
+-rw-rw-rw-   0        0        0    11556 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.92/LICENSE.txt
+-rw-rw-rw-   0        0        0      177 2023-06-13 14:38:51.716303 wizata-dsapi-0.1.92/PKG-INFO
+-rw-rw-rw-   0        0        0      323 2023-05-24 07:05:28.000000 wizata-dsapi-0.1.92/README.rst
+-rw-rw-rw-   0        0        0       42 2023-06-13 14:38:51.717791 wizata-dsapi-0.1.92/setup.cfg
+-rw-rw-rw-   0        0        0     1242 2023-06-13 14:38:41.000000 wizata-dsapi-0.1.92/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 14:38:51.682989 wizata-dsapi-0.1.92/wizata_dsapi/
+-rw-rw-rw-   0        0        0      933 2023-06-13 07:36:28.000000 wizata-dsapi-0.1.92/wizata_dsapi/__init__.py
+-rw-rw-rw-   0        0        0      632 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.92/wizata_dsapi/api_dto.py
+-rw-rw-rw-   0        0        0     2958 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.92/wizata_dsapi/dataframe_toolkit.py
+-rw-rw-rw-   0        0        0     5714 2023-06-08 15:23:14.000000 wizata-dsapi-0.1.92/wizata_dsapi/datapoint.py
+-rw-rw-rw-   0        0        0     1877 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.92/wizata_dsapi/ds_dataframe.py
+-rw-rw-rw-   0        0        0     2846 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.92/wizata_dsapi/dsapi_json_encoder.py
+-rw-rw-rw-   0        0        0    14658 2023-06-13 14:38:41.000000 wizata-dsapi-0.1.92/wizata_dsapi/execution.py
+-rw-rw-rw-   0        0        0     3810 2023-06-08 07:54:01.000000 wizata-dsapi-0.1.92/wizata_dsapi/experiment.py
+-rw-rw-rw-   0        0        0     6159 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.92/wizata_dsapi/mlmodel.py
+-rw-rw-rw-   0        0        0     1594 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.92/wizata_dsapi/model_toolkit.py
+-rw-rw-rw-   0        0        0    11227 2023-06-12 20:23:50.000000 wizata-dsapi-0.1.92/wizata_dsapi/pipeline.py
+-rw-rw-rw-   0        0        0     2136 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.92/wizata_dsapi/plot.py
+-rw-rw-rw-   0        0        0    13575 2023-06-12 20:23:50.000000 wizata-dsapi-0.1.92/wizata_dsapi/request.py
+-rw-rw-rw-   0        0        0     8716 2023-06-12 20:23:50.000000 wizata-dsapi-0.1.92/wizata_dsapi/script.py
+-rw-rw-rw-   0        0        0     3929 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.92/wizata_dsapi/template.py
+-rw-rw-rw-   0        0        0     2597 2023-06-08 07:54:01.000000 wizata-dsapi-0.1.92/wizata_dsapi/twin.py
+-rw-rw-rw-   0        0        0     2701 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.92/wizata_dsapi/twinregistration.py
+-rw-rw-rw-   0        0        0      489 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.92/wizata_dsapi/wizard_function.py
+-rw-rw-rw-   0        0        0    54309 2023-06-12 21:07:08.000000 wizata-dsapi-0.1.92/wizata_dsapi/wizata_dsapi_client.py
+drwxrwxrwx   0        0        0        0 2023-06-13 14:38:51.712831 wizata-dsapi-0.1.92/wizata_dsapi.egg-info/
+-rw-rw-rw-   0        0        0      177 2023-06-13 14:38:51.000000 wizata-dsapi-0.1.92/wizata_dsapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      730 2023-06-13 14:38:51.000000 wizata-dsapi-0.1.92/wizata_dsapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 14:38:51.000000 wizata-dsapi-0.1.92/wizata_dsapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      555 2023-06-13 14:38:51.000000 wizata-dsapi-0.1.92/wizata_dsapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-13 14:38:51.000000 wizata-dsapi-0.1.92/wizata_dsapi.egg-info/top_level.txt
```

### Comparing `wizata-dsapi-0.1.91/LICENSE.txt` & `wizata-dsapi-0.1.92/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.91/setup.py` & `wizata-dsapi-0.1.92/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='wizata-dsapi',
-    version='0.1.91',
+    version='0.1.92',
     description='Wizata Data Science Toolkit',
     author='Wizata S.A.',
     author_email='info@wizata.com',
     packages=['wizata_dsapi'],
     install_requires=[
         'dill==0.3.6',
         'pandas==1.5.3',
```

### Comparing `wizata-dsapi-0.1.91/wizata_dsapi/__init__.py` & `wizata-dsapi-0.1.92/wizata_dsapi/__init__.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.91/wizata_dsapi/api_dto.py` & `wizata-dsapi-0.1.92/wizata_dsapi/api_dto.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.91/wizata_dsapi/dataframe_toolkit.py` & `wizata-dsapi-0.1.92/wizata_dsapi/dataframe_toolkit.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.91/wizata_dsapi/datapoint.py` & `wizata-dsapi-0.1.92/wizata_dsapi/datapoint.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.91/wizata_dsapi/ds_dataframe.py` & `wizata-dsapi-0.1.92/wizata_dsapi/ds_dataframe.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.91/wizata_dsapi/dsapi_json_encoder.py` & `wizata-dsapi-0.1.92/wizata_dsapi/dsapi_json_encoder.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.91/wizata_dsapi/execution.py` & `wizata-dsapi-0.1.92/wizata_dsapi/execution.py`

 * *Files 0% similar despite different names*

```diff
@@ -219,16 +219,16 @@
             obj["experimentId"] = str(self.experiment_id)
         if self.request is not None:
             obj["request"] = json.dumps(self.request.to_json())
         if self.properties is not None:
             obj["properties"] = json.dumps(self.properties)
         if self.dataframe is not None:
             obj["dataframe"] = df_to_json(self.dataframe)
-        if self.input_ds_dataframe is not None:
-            obj["dataframeId"] = str(self.input_ds_dataframe.df_id)
+        # if self.input_ds_dataframe is not None:
+        #     obj["dataframeId"] = str(self.input_ds_dataframe.df_id)
         if self.script is not None:
             obj["scriptId"] = str(self.script.script_id)
         if self.ml_model is not None:
             obj["mlModelId"] = str(self.ml_model.model_id)
         if self.pipeline is not None:
             obj["pipelineId"] = str(self.pipeline.pipeline_id)
         if self.function is not None:
@@ -247,18 +247,18 @@
         if self.models is not None:
             models_json = []
             for ml_model in self.models:
                 models_json.append({"id": str(ml_model.model_id)})
             obj["models"] = models_json
         if self.anomalies is not None:
             obj["anomaliesList"] = json.dumps(self.anomalies)
-        if self.result_dataframe is not None:
-            obj["resultDataframe"] = {
-                "id": str(self.output_ds_dataframe.df_id)
-            }
+        # if self.result_dataframe is not None:
+        #     obj["resultDataframe"] = {
+        #         "id": str(self.output_ds_dataframe.df_id)
+        #     }
         if self.createdById is not None:
             obj["createdById"] = self.createdById
         if self.createdDate is not None:
             obj["createdDate"] = self.createdDate
         if self.updatedById is not None:
             obj["updatedById"] = self.updatedById
         if self.updatedDate is not None:
@@ -292,16 +292,16 @@
             else:
                 self.add_properties(obj["properties"])
         if "dataframe" in obj.keys() and obj["dataframe"] is not None:
             if isinstance(obj["dataframe"], str):
                 self.request.from_json(json.loads(obj["dataframe"]))
             else:
                 self.dataframe = df_from_json(obj["dataframe"])
-        elif "dataframeId" in obj.keys() and obj["dataframeId"] is not None:
-            self.input_ds_dataframe = DSDataFrame(df_id=uuid.UUID(obj["dataframeId"]))
+        # elif "dataframeId" in obj.keys() and obj["dataframeId"] is not None:
+        #     self.input_ds_dataframe = DSDataFrame(df_id=uuid.UUID(obj["dataframeId"]))
         if "scriptId" in obj.keys() and obj["scriptId"] is not None:
             self.script = Script()
             self.script.script_id = uuid.UUID(obj["scriptId"])
         if "pipelineId" in obj.keys() and obj["pipelineId"] is not None:
             self.pipeline = Pipeline()
             self.pipeline.pipeline_id = uuid.UUID(obj["pipelineId"])
         if "mlModelId" in obj.keys() and obj["mlModelId"] is not None:
```

### Comparing `wizata-dsapi-0.1.91/wizata_dsapi/experiment.py` & `wizata-dsapi-0.1.92/wizata_dsapi/experiment.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.91/wizata_dsapi/mlmodel.py` & `wizata-dsapi-0.1.92/wizata_dsapi/mlmodel.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.91/wizata_dsapi/model_toolkit.py` & `wizata-dsapi-0.1.92/wizata_dsapi/model_toolkit.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.91/wizata_dsapi/pipeline.py` & `wizata-dsapi-0.1.92/wizata_dsapi/pipeline.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.91/wizata_dsapi/plot.py` & `wizata-dsapi-0.1.92/wizata_dsapi/plot.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.91/wizata_dsapi/request.py` & `wizata-dsapi-0.1.92/wizata_dsapi/request.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.91/wizata_dsapi/script.py` & `wizata-dsapi-0.1.92/wizata_dsapi/script.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.91/wizata_dsapi/template.py` & `wizata-dsapi-0.1.92/wizata_dsapi/template.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.91/wizata_dsapi/twin.py` & `wizata-dsapi-0.1.92/wizata_dsapi/twin.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.91/wizata_dsapi/twinregistration.py` & `wizata-dsapi-0.1.92/wizata_dsapi/twinregistration.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.91/wizata_dsapi/wizata_dsapi_client.py` & `wizata-dsapi-0.1.92/wizata_dsapi/wizata_dsapi_client.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.91/wizata_dsapi.egg-info/SOURCES.txt` & `wizata-dsapi-0.1.92/wizata_dsapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.91/wizata_dsapi.egg-info/requires.txt` & `wizata-dsapi-0.1.92/wizata_dsapi.egg-info/requires.txt`

 * *Files identical despite different names*

