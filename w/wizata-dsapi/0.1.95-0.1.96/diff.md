# Comparing `tmp/wizata-dsapi-0.1.95.tar.gz` & `tmp/wizata-dsapi-0.1.96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wizata-dsapi-0.1.95.tar", last modified: Tue Jun 13 15:09:23 2023, max compression
+gzip compressed data, was "wizata-dsapi-0.1.96.tar", last modified: Tue Jun 13 15:13:14 2023, max compression
```

## Comparing `wizata-dsapi-0.1.95.tar` & `wizata-dsapi-0.1.96.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 15:09:23.697711 wizata-dsapi-0.1.95/
--rw-rw-rw-   0        0        0    11556 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.95/LICENSE.txt
--rw-rw-rw-   0        0        0      177 2023-06-13 15:09:23.696736 wizata-dsapi-0.1.95/PKG-INFO
--rw-rw-rw-   0        0        0      323 2023-05-24 07:05:28.000000 wizata-dsapi-0.1.95/README.rst
--rw-rw-rw-   0        0        0       42 2023-06-13 15:09:23.697711 wizata-dsapi-0.1.95/setup.cfg
--rw-rw-rw-   0        0        0     1242 2023-06-13 15:09:19.000000 wizata-dsapi-0.1.95/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-13 15:09:23.677757 wizata-dsapi-0.1.95/wizata_dsapi/
--rw-rw-rw-   0        0        0      933 2023-06-13 07:36:28.000000 wizata-dsapi-0.1.95/wizata_dsapi/__init__.py
--rw-rw-rw-   0        0        0      632 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.95/wizata_dsapi/api_dto.py
--rw-rw-rw-   0        0        0     2958 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.95/wizata_dsapi/dataframe_toolkit.py
--rw-rw-rw-   0        0        0     5714 2023-06-08 15:23:14.000000 wizata-dsapi-0.1.95/wizata_dsapi/datapoint.py
--rw-rw-rw-   0        0        0     1877 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.95/wizata_dsapi/ds_dataframe.py
--rw-rw-rw-   0        0        0     2846 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.95/wizata_dsapi/dsapi_json_encoder.py
--rw-rw-rw-   0        0        0    14658 2023-06-13 14:38:41.000000 wizata-dsapi-0.1.95/wizata_dsapi/execution.py
--rw-rw-rw-   0        0        0     3810 2023-06-08 07:54:01.000000 wizata-dsapi-0.1.95/wizata_dsapi/experiment.py
--rw-rw-rw-   0        0        0     6159 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.95/wizata_dsapi/mlmodel.py
--rw-rw-rw-   0        0        0     1594 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.95/wizata_dsapi/model_toolkit.py
--rw-rw-rw-   0        0        0    11227 2023-06-12 20:23:50.000000 wizata-dsapi-0.1.95/wizata_dsapi/pipeline.py
--rw-rw-rw-   0        0        0     2136 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.95/wizata_dsapi/plot.py
--rw-rw-rw-   0        0        0    13575 2023-06-12 20:23:50.000000 wizata-dsapi-0.1.95/wizata_dsapi/request.py
--rw-rw-rw-   0        0        0     8716 2023-06-12 20:23:50.000000 wizata-dsapi-0.1.95/wizata_dsapi/script.py
--rw-rw-rw-   0        0        0     3929 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.95/wizata_dsapi/template.py
--rw-rw-rw-   0        0        0     2597 2023-06-08 07:54:01.000000 wizata-dsapi-0.1.95/wizata_dsapi/twin.py
--rw-rw-rw-   0        0        0     2701 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.95/wizata_dsapi/twinregistration.py
--rw-rw-rw-   0        0        0      489 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.95/wizata_dsapi/wizard_function.py
--rw-rw-rw-   0        0        0    56691 2023-06-13 15:09:19.000000 wizata-dsapi-0.1.95/wizata_dsapi/wizata_dsapi_client.py
-drwxrwxrwx   0        0        0        0 2023-06-13 15:09:23.694734 wizata-dsapi-0.1.95/wizata_dsapi.egg-info/
--rw-rw-rw-   0        0        0      177 2023-06-13 15:09:23.000000 wizata-dsapi-0.1.95/wizata_dsapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      730 2023-06-13 15:09:23.000000 wizata-dsapi-0.1.95/wizata_dsapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 15:09:23.000000 wizata-dsapi-0.1.95/wizata_dsapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      555 2023-06-13 15:09:23.000000 wizata-dsapi-0.1.95/wizata_dsapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-13 15:09:23.000000 wizata-dsapi-0.1.95/wizata_dsapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-13 15:13:14.449827 wizata-dsapi-0.1.96/
+-rw-rw-rw-   0        0        0    11556 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.96/LICENSE.txt
+-rw-rw-rw-   0        0        0      177 2023-06-13 15:13:14.449334 wizata-dsapi-0.1.96/PKG-INFO
+-rw-rw-rw-   0        0        0      323 2023-05-24 07:05:28.000000 wizata-dsapi-0.1.96/README.rst
+-rw-rw-rw-   0        0        0       42 2023-06-13 15:13:14.450321 wizata-dsapi-0.1.96/setup.cfg
+-rw-rw-rw-   0        0        0     1242 2023-06-13 15:13:09.000000 wizata-dsapi-0.1.96/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 15:13:14.429986 wizata-dsapi-0.1.96/wizata_dsapi/
+-rw-rw-rw-   0        0        0      933 2023-06-13 07:36:28.000000 wizata-dsapi-0.1.96/wizata_dsapi/__init__.py
+-rw-rw-rw-   0        0        0      632 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.96/wizata_dsapi/api_dto.py
+-rw-rw-rw-   0        0        0     2958 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.96/wizata_dsapi/dataframe_toolkit.py
+-rw-rw-rw-   0        0        0     5714 2023-06-08 15:23:14.000000 wizata-dsapi-0.1.96/wizata_dsapi/datapoint.py
+-rw-rw-rw-   0        0        0     1877 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.96/wizata_dsapi/ds_dataframe.py
+-rw-rw-rw-   0        0        0     2846 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.96/wizata_dsapi/dsapi_json_encoder.py
+-rw-rw-rw-   0        0        0    14658 2023-06-13 14:38:41.000000 wizata-dsapi-0.1.96/wizata_dsapi/execution.py
+-rw-rw-rw-   0        0        0     3810 2023-06-08 07:54:01.000000 wizata-dsapi-0.1.96/wizata_dsapi/experiment.py
+-rw-rw-rw-   0        0        0     6159 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.96/wizata_dsapi/mlmodel.py
+-rw-rw-rw-   0        0        0     1594 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.96/wizata_dsapi/model_toolkit.py
+-rw-rw-rw-   0        0        0    11227 2023-06-12 20:23:50.000000 wizata-dsapi-0.1.96/wizata_dsapi/pipeline.py
+-rw-rw-rw-   0        0        0     2136 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.96/wizata_dsapi/plot.py
+-rw-rw-rw-   0        0        0    13575 2023-06-12 20:23:50.000000 wizata-dsapi-0.1.96/wizata_dsapi/request.py
+-rw-rw-rw-   0        0        0     8716 2023-06-12 20:23:50.000000 wizata-dsapi-0.1.96/wizata_dsapi/script.py
+-rw-rw-rw-   0        0        0     3929 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.96/wizata_dsapi/template.py
+-rw-rw-rw-   0        0        0     2597 2023-06-08 07:54:01.000000 wizata-dsapi-0.1.96/wizata_dsapi/twin.py
+-rw-rw-rw-   0        0        0     2701 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.96/wizata_dsapi/twinregistration.py
+-rw-rw-rw-   0        0        0      489 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.96/wizata_dsapi/wizard_function.py
+-rw-rw-rw-   0        0        0    56528 2023-06-13 15:13:09.000000 wizata-dsapi-0.1.96/wizata_dsapi/wizata_dsapi_client.py
+drwxrwxrwx   0        0        0        0 2023-06-13 15:13:14.447364 wizata-dsapi-0.1.96/wizata_dsapi.egg-info/
+-rw-rw-rw-   0        0        0      177 2023-06-13 15:13:14.000000 wizata-dsapi-0.1.96/wizata_dsapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      730 2023-06-13 15:13:14.000000 wizata-dsapi-0.1.96/wizata_dsapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 15:13:14.000000 wizata-dsapi-0.1.96/wizata_dsapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      555 2023-06-13 15:13:14.000000 wizata-dsapi-0.1.96/wizata_dsapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-13 15:13:14.000000 wizata-dsapi-0.1.96/wizata_dsapi.egg-info/top_level.txt
```

### Comparing `wizata-dsapi-0.1.95/LICENSE.txt` & `wizata-dsapi-0.1.96/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.95/setup.py` & `wizata-dsapi-0.1.96/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='wizata-dsapi',
-    version='0.1.95',
+    version='0.1.96',
     description='Wizata Data Science Toolkit',
     author='Wizata S.A.',
     author_email='info@wizata.com',
     packages=['wizata_dsapi'],
     install_requires=[
         'dill==0.3.6',
         'pandas==1.5.3',
```

### Comparing `wizata-dsapi-0.1.95/wizata_dsapi/__init__.py` & `wizata-dsapi-0.1.96/wizata_dsapi/__init__.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.95/wizata_dsapi/api_dto.py` & `wizata-dsapi-0.1.96/wizata_dsapi/api_dto.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.95/wizata_dsapi/dataframe_toolkit.py` & `wizata-dsapi-0.1.96/wizata_dsapi/dataframe_toolkit.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.95/wizata_dsapi/datapoint.py` & `wizata-dsapi-0.1.96/wizata_dsapi/datapoint.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.95/wizata_dsapi/ds_dataframe.py` & `wizata-dsapi-0.1.96/wizata_dsapi/ds_dataframe.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.95/wizata_dsapi/dsapi_json_encoder.py` & `wizata-dsapi-0.1.96/wizata_dsapi/dsapi_json_encoder.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.95/wizata_dsapi/execution.py` & `wizata-dsapi-0.1.96/wizata_dsapi/execution.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.95/wizata_dsapi/experiment.py` & `wizata-dsapi-0.1.96/wizata_dsapi/experiment.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.95/wizata_dsapi/mlmodel.py` & `wizata-dsapi-0.1.96/wizata_dsapi/mlmodel.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.95/wizata_dsapi/model_toolkit.py` & `wizata-dsapi-0.1.96/wizata_dsapi/model_toolkit.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.95/wizata_dsapi/pipeline.py` & `wizata-dsapi-0.1.96/wizata_dsapi/pipeline.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.95/wizata_dsapi/plot.py` & `wizata-dsapi-0.1.96/wizata_dsapi/plot.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.95/wizata_dsapi/request.py` & `wizata-dsapi-0.1.96/wizata_dsapi/request.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.95/wizata_dsapi/script.py` & `wizata-dsapi-0.1.96/wizata_dsapi/script.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.95/wizata_dsapi/template.py` & `wizata-dsapi-0.1.96/wizata_dsapi/template.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.95/wizata_dsapi/twin.py` & `wizata-dsapi-0.1.96/wizata_dsapi/twin.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.95/wizata_dsapi/twinregistration.py` & `wizata-dsapi-0.1.96/wizata_dsapi/twinregistration.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.95/wizata_dsapi/wizata_dsapi_client.py` & `wizata-dsapi-0.1.96/wizata_dsapi/wizata_dsapi_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -943,16 +943,14 @@
             elif isinstance(twin, str):
                 execution.properties["twinId"] = str(self.get(twin_hardware_id=twin).twin_id)
             elif isinstance(twin, Twin):
                 execution.properties["twinId"] = str(twin.twin_id)
 
         # Execute
         if isinstance(execution, Execution):
-            if execution.script is None and execution.ml_model is None:
-                raise ValueError("Execution must contains at least a Script or a Model")
             response = requests.post(self.__url() + "execute/test",
                                      headers=self.__header(),
                                      data=json.dumps(execution.to_json(), cls=DSAPIEncoder))
             if response.status_code == 200:
                 return dill.loads(response.content)
             else:
                 raise self.__raise_error(response)
```

### Comparing `wizata-dsapi-0.1.95/wizata_dsapi.egg-info/SOURCES.txt` & `wizata-dsapi-0.1.96/wizata_dsapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.95/wizata_dsapi.egg-info/requires.txt` & `wizata-dsapi-0.1.96/wizata_dsapi.egg-info/requires.txt`

 * *Files identical despite different names*

