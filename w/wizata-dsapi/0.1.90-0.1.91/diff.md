# Comparing `tmp/wizata-dsapi-0.1.90.tar.gz` & `tmp/wizata-dsapi-0.1.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wizata-dsapi-0.1.90.tar", last modified: Tue Jun 13 07:39:26 2023, max compression
+gzip compressed data, was "wizata-dsapi-0.1.91.tar", last modified: Tue Jun 13 13:16:00 2023, max compression
```

## Comparing `wizata-dsapi-0.1.90.tar` & `wizata-dsapi-0.1.91.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 07:39:26.859189 wizata-dsapi-0.1.90/
--rw-rw-rw-   0        0        0    11556 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.90/LICENSE.txt
--rw-rw-rw-   0        0        0      177 2023-06-13 07:39:26.858205 wizata-dsapi-0.1.90/PKG-INFO
--rw-rw-rw-   0        0        0      323 2023-05-24 07:05:28.000000 wizata-dsapi-0.1.90/README.rst
--rw-rw-rw-   0        0        0       42 2023-06-13 07:39:26.859685 wizata-dsapi-0.1.90/setup.cfg
--rw-rw-rw-   0        0        0     1242 2023-06-13 07:39:17.000000 wizata-dsapi-0.1.90/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-13 07:39:26.827240 wizata-dsapi-0.1.90/wizata_dsapi/
--rw-rw-rw-   0        0        0      933 2023-06-13 07:36:28.000000 wizata-dsapi-0.1.90/wizata_dsapi/__init__.py
--rw-rw-rw-   0        0        0      632 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.90/wizata_dsapi/api_dto.py
--rw-rw-rw-   0        0        0     2958 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.90/wizata_dsapi/dataframe_toolkit.py
--rw-rw-rw-   0        0        0     5714 2023-06-08 15:23:14.000000 wizata-dsapi-0.1.90/wizata_dsapi/datapoint.py
--rw-rw-rw-   0        0        0     1877 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.90/wizata_dsapi/ds_dataframe.py
--rw-rw-rw-   0        0        0     2846 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.90/wizata_dsapi/dsapi_json_encoder.py
--rw-rw-rw-   0        0        0    14612 2023-06-13 07:36:51.000000 wizata-dsapi-0.1.90/wizata_dsapi/execution.py
--rw-rw-rw-   0        0        0     3810 2023-06-08 07:54:01.000000 wizata-dsapi-0.1.90/wizata_dsapi/experiment.py
--rw-rw-rw-   0        0        0     6159 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.90/wizata_dsapi/mlmodel.py
--rw-rw-rw-   0        0        0     1594 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.90/wizata_dsapi/model_toolkit.py
--rw-rw-rw-   0        0        0    11227 2023-06-12 20:23:50.000000 wizata-dsapi-0.1.90/wizata_dsapi/pipeline.py
--rw-rw-rw-   0        0        0     2136 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.90/wizata_dsapi/plot.py
--rw-rw-rw-   0        0        0    13575 2023-06-12 20:23:50.000000 wizata-dsapi-0.1.90/wizata_dsapi/request.py
--rw-rw-rw-   0        0        0     8716 2023-06-12 20:23:50.000000 wizata-dsapi-0.1.90/wizata_dsapi/script.py
--rw-rw-rw-   0        0        0     3929 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.90/wizata_dsapi/template.py
--rw-rw-rw-   0        0        0     2597 2023-06-08 07:54:01.000000 wizata-dsapi-0.1.90/wizata_dsapi/twin.py
--rw-rw-rw-   0        0        0     2701 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.90/wizata_dsapi/twinregistration.py
--rw-rw-rw-   0        0        0      489 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.90/wizata_dsapi/wizard_function.py
--rw-rw-rw-   0        0        0    54309 2023-06-12 21:07:08.000000 wizata-dsapi-0.1.90/wizata_dsapi/wizata_dsapi_client.py
-drwxrwxrwx   0        0        0        0 2023-06-13 07:39:26.855716 wizata-dsapi-0.1.90/wizata_dsapi.egg-info/
--rw-rw-rw-   0        0        0      177 2023-06-13 07:39:26.000000 wizata-dsapi-0.1.90/wizata_dsapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      730 2023-06-13 07:39:26.000000 wizata-dsapi-0.1.90/wizata_dsapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 07:39:26.000000 wizata-dsapi-0.1.90/wizata_dsapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      555 2023-06-13 07:39:26.000000 wizata-dsapi-0.1.90/wizata_dsapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-13 07:39:26.000000 wizata-dsapi-0.1.90/wizata_dsapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-13 13:16:00.253064 wizata-dsapi-0.1.91/
+-rw-rw-rw-   0        0        0    11556 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.91/LICENSE.txt
+-rw-rw-rw-   0        0        0      177 2023-06-13 13:16:00.252072 wizata-dsapi-0.1.91/PKG-INFO
+-rw-rw-rw-   0        0        0      323 2023-05-24 07:05:28.000000 wizata-dsapi-0.1.91/README.rst
+-rw-rw-rw-   0        0        0       42 2023-06-13 13:16:00.253064 wizata-dsapi-0.1.91/setup.cfg
+-rw-rw-rw-   0        0        0     1242 2023-06-13 13:15:50.000000 wizata-dsapi-0.1.91/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 13:16:00.224270 wizata-dsapi-0.1.91/wizata_dsapi/
+-rw-rw-rw-   0        0        0      933 2023-06-13 07:36:28.000000 wizata-dsapi-0.1.91/wizata_dsapi/__init__.py
+-rw-rw-rw-   0        0        0      632 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.91/wizata_dsapi/api_dto.py
+-rw-rw-rw-   0        0        0     2958 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.91/wizata_dsapi/dataframe_toolkit.py
+-rw-rw-rw-   0        0        0     5714 2023-06-08 15:23:14.000000 wizata-dsapi-0.1.91/wizata_dsapi/datapoint.py
+-rw-rw-rw-   0        0        0     1877 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.91/wizata_dsapi/ds_dataframe.py
+-rw-rw-rw-   0        0        0     2846 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.91/wizata_dsapi/dsapi_json_encoder.py
+-rw-rw-rw-   0        0        0    14642 2023-06-13 13:15:50.000000 wizata-dsapi-0.1.91/wizata_dsapi/execution.py
+-rw-rw-rw-   0        0        0     3810 2023-06-08 07:54:01.000000 wizata-dsapi-0.1.91/wizata_dsapi/experiment.py
+-rw-rw-rw-   0        0        0     6159 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.91/wizata_dsapi/mlmodel.py
+-rw-rw-rw-   0        0        0     1594 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.91/wizata_dsapi/model_toolkit.py
+-rw-rw-rw-   0        0        0    11227 2023-06-12 20:23:50.000000 wizata-dsapi-0.1.91/wizata_dsapi/pipeline.py
+-rw-rw-rw-   0        0        0     2136 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.91/wizata_dsapi/plot.py
+-rw-rw-rw-   0        0        0    13575 2023-06-12 20:23:50.000000 wizata-dsapi-0.1.91/wizata_dsapi/request.py
+-rw-rw-rw-   0        0        0     8716 2023-06-12 20:23:50.000000 wizata-dsapi-0.1.91/wizata_dsapi/script.py
+-rw-rw-rw-   0        0        0     3929 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.91/wizata_dsapi/template.py
+-rw-rw-rw-   0        0        0     2597 2023-06-08 07:54:01.000000 wizata-dsapi-0.1.91/wizata_dsapi/twin.py
+-rw-rw-rw-   0        0        0     2701 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.91/wizata_dsapi/twinregistration.py
+-rw-rw-rw-   0        0        0      489 2023-05-12 09:43:16.000000 wizata-dsapi-0.1.91/wizata_dsapi/wizard_function.py
+-rw-rw-rw-   0        0        0    54309 2023-06-12 21:07:08.000000 wizata-dsapi-0.1.91/wizata_dsapi/wizata_dsapi_client.py
+drwxrwxrwx   0        0        0        0 2023-06-13 13:16:00.250086 wizata-dsapi-0.1.91/wizata_dsapi.egg-info/
+-rw-rw-rw-   0        0        0      177 2023-06-13 13:15:59.000000 wizata-dsapi-0.1.91/wizata_dsapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      730 2023-06-13 13:15:59.000000 wizata-dsapi-0.1.91/wizata_dsapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 13:15:59.000000 wizata-dsapi-0.1.91/wizata_dsapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      555 2023-06-13 13:15:59.000000 wizata-dsapi-0.1.91/wizata_dsapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-13 13:15:59.000000 wizata-dsapi-0.1.91/wizata_dsapi.egg-info/top_level.txt
```

### Comparing `wizata-dsapi-0.1.90/LICENSE.txt` & `wizata-dsapi-0.1.91/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.90/setup.py` & `wizata-dsapi-0.1.91/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='wizata-dsapi',
-    version='0.1.90',
+    version='0.1.91',
     description='Wizata Data Science Toolkit',
     author='Wizata S.A.',
     author_email='info@wizata.com',
     packages=['wizata_dsapi'],
     install_requires=[
         'dill==0.3.6',
         'pandas==1.5.3',
```

### Comparing `wizata-dsapi-0.1.90/wizata_dsapi/__init__.py` & `wizata-dsapi-0.1.91/wizata_dsapi/__init__.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.90/wizata_dsapi/api_dto.py` & `wizata-dsapi-0.1.91/wizata_dsapi/api_dto.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.90/wizata_dsapi/dataframe_toolkit.py` & `wizata-dsapi-0.1.91/wizata_dsapi/dataframe_toolkit.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.90/wizata_dsapi/datapoint.py` & `wizata-dsapi-0.1.91/wizata_dsapi/datapoint.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.90/wizata_dsapi/ds_dataframe.py` & `wizata-dsapi-0.1.91/wizata_dsapi/ds_dataframe.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.90/wizata_dsapi/dsapi_json_encoder.py` & `wizata-dsapi-0.1.91/wizata_dsapi/dsapi_json_encoder.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.90/wizata_dsapi/execution.py` & `wizata-dsapi-0.1.91/wizata_dsapi/execution.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,14 +97,15 @@
         self.updatedById = None
         self.updatedDate = None
 
         # Outputs Properties (generated by Execution)
         self.models = []
         self.anomalies = []
         self.plots = []
+        self.dataframes = []
         self.output_ds_dataframe = None
         self.warnings = None
 
     def _get_dataframe(self):
         if self.input_ds_dataframe is None:
             return None
         else:
```

### Comparing `wizata-dsapi-0.1.90/wizata_dsapi/experiment.py` & `wizata-dsapi-0.1.91/wizata_dsapi/experiment.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.90/wizata_dsapi/mlmodel.py` & `wizata-dsapi-0.1.91/wizata_dsapi/mlmodel.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.90/wizata_dsapi/model_toolkit.py` & `wizata-dsapi-0.1.91/wizata_dsapi/model_toolkit.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.90/wizata_dsapi/pipeline.py` & `wizata-dsapi-0.1.91/wizata_dsapi/pipeline.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.90/wizata_dsapi/plot.py` & `wizata-dsapi-0.1.91/wizata_dsapi/plot.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.90/wizata_dsapi/request.py` & `wizata-dsapi-0.1.91/wizata_dsapi/request.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.90/wizata_dsapi/script.py` & `wizata-dsapi-0.1.91/wizata_dsapi/script.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.90/wizata_dsapi/template.py` & `wizata-dsapi-0.1.91/wizata_dsapi/template.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.90/wizata_dsapi/twin.py` & `wizata-dsapi-0.1.91/wizata_dsapi/twin.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.90/wizata_dsapi/twinregistration.py` & `wizata-dsapi-0.1.91/wizata_dsapi/twinregistration.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.90/wizata_dsapi/wizata_dsapi_client.py` & `wizata-dsapi-0.1.91/wizata_dsapi/wizata_dsapi_client.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.90/wizata_dsapi.egg-info/SOURCES.txt` & `wizata-dsapi-0.1.91/wizata_dsapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.1.90/wizata_dsapi.egg-info/requires.txt` & `wizata-dsapi-0.1.91/wizata_dsapi.egg-info/requires.txt`

 * *Files identical despite different names*

