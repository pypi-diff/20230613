# Comparing `tmp/censius-1.7.0.tar.gz` & `tmp/censius-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "censius-1.7.0.tar", last modified: Mon Jun 12 16:51:54 2023, max compression
+gzip compressed data, was "censius-1.7.1.tar", last modified: Tue Jun 13 09:21:13 2023, max compression
```

## Comparing `censius-1.7.0.tar` & `censius-1.7.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:51:54.729897 censius-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-12 16:51:54.729897 censius-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-12 16:51:52.000000 censius-1.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-12 16:51:52.000000 censius-1.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 16:51:54.729897 censius-1.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-06-12 16:51:52.000000 censius-1.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:51:54.725897 censius-1.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:51:54.725897 censius-1.7.0/src/censius/
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-12 16:51:52.000000 censius-1.7.0/src/censius/CensiusParent.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-12 16:51:52.000000 censius-1.7.0/src/censius/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-12 16:51:52.000000 censius-1.7.0/src/censius/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-12 16:51:52.000000 censius-1.7.0/src/censius/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:51:54.729897 censius-1.7.0/src/censius/ml/
--rw-r--r--   0 runner    (1001) docker     (123)    33575 2023-06-12 16:51:52.000000 censius-1.7.0/src/censius/ml/CensiusClient.py
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-12 16:51:52.000000 censius-1.7.0/src/censius/ml/Dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-12 16:51:52.000000 censius-1.7.0/src/censius/ml/DatasetType.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-12 16:51:52.000000 censius-1.7.0/src/censius/ml/Explanation.py
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-12 16:51:52.000000 censius-1.7.0/src/censius/ml/ExplanationType.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-12 16:51:52.000000 censius-1.7.0/src/censius/ml/ModelType.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-12 16:51:52.000000 censius-1.7.0/src/censius/ml/Prediction.py
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-12 16:51:52.000000 censius-1.7.0/src/censius/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-06-12 16:51:52.000000 censius-1.7.0/src/censius/ml/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    14033 2023-06-12 16:51:52.000000 censius-1.7.0/src/censius/ml/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)    21301 2023-06-12 16:51:52.000000 censius-1.7.0/src/censius/ml/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:51:54.729897 censius-1.7.0/src/censius/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-06-12 16:51:52.000000 censius-1.7.0/src/censius/nlp/CensiusClient.py
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-12 16:51:52.000000 censius-1.7.0/src/censius/nlp/DatasetType.py
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-12 16:51:52.000000 censius-1.7.0/src/censius/nlp/ModelType.py
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-12 16:51:52.000000 censius-1.7.0/src/censius/nlp/UseCase.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-12 16:51:52.000000 censius-1.7.0/src/censius/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-12 16:51:52.000000 censius-1.7.0/src/censius/nlp/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-06-12 16:51:52.000000 censius-1.7.0/src/censius/nlp/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 16:51:54.725897 censius-1.7.0/src/censius.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-12 16:51:54.000000 censius-1.7.0/src/censius.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-06-12 16:51:54.000000 censius-1.7.0/src/censius.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 16:51:54.000000 censius-1.7.0/src/censius.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-12 16:51:54.000000 censius-1.7.0/src/censius.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-12 16:51:54.000000 censius-1.7.0/src/censius.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:21:13.710478 censius-1.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-13 09:21:13.710478 censius-1.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-13 09:21:10.000000 censius-1.7.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-13 09:21:10.000000 censius-1.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 09:21:13.710478 censius-1.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-06-13 09:21:10.000000 censius-1.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:21:13.706478 censius-1.7.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:21:13.710478 censius-1.7.1/src/censius/
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-13 09:21:10.000000 censius-1.7.1/src/censius/CensiusParent.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-13 09:21:10.000000 censius-1.7.1/src/censius/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-13 09:21:10.000000 censius-1.7.1/src/censius/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-13 09:21:10.000000 censius-1.7.1/src/censius/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:21:13.710478 censius-1.7.1/src/censius/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)    33575 2023-06-13 09:21:10.000000 censius-1.7.1/src/censius/ml/CensiusClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-13 09:21:10.000000 censius-1.7.1/src/censius/ml/Dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-13 09:21:10.000000 censius-1.7.1/src/censius/ml/DatasetType.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-13 09:21:10.000000 censius-1.7.1/src/censius/ml/Explanation.py
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-13 09:21:10.000000 censius-1.7.1/src/censius/ml/ExplanationType.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-13 09:21:10.000000 censius-1.7.1/src/censius/ml/ModelType.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-13 09:21:10.000000 censius-1.7.1/src/censius/ml/Prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-13 09:21:10.000000 censius-1.7.1/src/censius/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-06-13 09:21:10.000000 censius-1.7.1/src/censius/ml/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14033 2023-06-13 09:21:10.000000 censius-1.7.1/src/censius/ml/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21301 2023-06-13 09:21:10.000000 censius-1.7.1/src/censius/ml/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:21:13.710478 censius-1.7.1/src/censius/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-06-13 09:21:10.000000 censius-1.7.1/src/censius/nlp/CensiusClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-13 09:21:10.000000 censius-1.7.1/src/censius/nlp/DatasetType.py
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-13 09:21:10.000000 censius-1.7.1/src/censius/nlp/ModelType.py
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-13 09:21:10.000000 censius-1.7.1/src/censius/nlp/UseCase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-13 09:21:10.000000 censius-1.7.1/src/censius/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-13 09:21:10.000000 censius-1.7.1/src/censius/nlp/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-06-13 09:21:10.000000 censius-1.7.1/src/censius/nlp/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:21:13.710478 censius-1.7.1/src/censius.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-13 09:21:13.000000 censius-1.7.1/src/censius.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-06-13 09:21:13.000000 censius-1.7.1/src/censius.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 09:21:13.000000 censius-1.7.1/src/censius.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-13 09:21:13.000000 censius-1.7.1/src/censius.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-13 09:21:13.000000 censius-1.7.1/src/censius.egg-info/top_level.txt
```

### Comparing `censius-1.7.0/PKG-INFO` & `censius-1.7.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: censius
-Version: 1.7.0
+Version: 1.7.1
 Summary: API for Censius
 Home-page: https://github.com/Censius/censius-logs-python-sdk
 Author: Censius
 Author-email: dev@censius.ai
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `censius-1.7.0/setup.py` & `censius-1.7.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="censius",
-    version="1.7.0",
+    version="1.7.1",
     description="API for Censius",
     long_description=long_description,
     long_description_content_type="text/markdown",
     py_modules=["censius/client"],
     package_dir={"": "src"},
     packages=["censius", "censius.nlp", "censius.ml"],
     install_requires=["requests", "jsonschema", "pandas", "numpy"],
```

### Comparing `censius-1.7.0/src/censius/CensiusParent.py` & `censius-1.7.1/src/censius/CensiusParent.py`

 * *Files identical despite different names*

### Comparing `censius-1.7.0/src/censius/ml/CensiusClient.py` & `censius-1.7.1/src/censius/ml/CensiusClient.py`

 * *Files identical despite different names*

### Comparing `censius-1.7.0/src/censius/ml/constants.py` & `censius-1.7.1/src/censius/ml/constants.py`

 * *Files identical despite different names*

### Comparing `censius-1.7.0/src/censius/ml/schemas.py` & `censius-1.7.1/src/censius/ml/schemas.py`

 * *Files identical despite different names*

### Comparing `censius-1.7.0/src/censius/ml/utils.py` & `censius-1.7.1/src/censius/ml/utils.py`

 * *Files identical despite different names*

### Comparing `censius-1.7.0/src/censius/nlp/CensiusClient.py` & `censius-1.7.1/src/censius/nlp/CensiusClient.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
                     headers=self.get_headers(),
                     data=json.dumps(json_data),
                 )
 
                 if response.status_code == 200:
                     dataset_id = response.json()["details"]["datasetId"]
                 else:
-                    return {"status": "error", "details": "failed to register dataset"}
+                    return response.json()
             else:
                 json_data["dataset_id"] = dataset_id
                 url = LLM_REGISTER_DATASET_URL(
                     project_id=self.project_id
                 )
                 requests.request(
                     "POST",
```

### Comparing `censius-1.7.0/src/censius/nlp/constants.py` & `censius-1.7.1/src/censius/nlp/constants.py`

 * *Files identical despite different names*

### Comparing `censius-1.7.0/src/censius/nlp/schema.py` & `censius-1.7.1/src/censius/nlp/schema.py`

 * *Files identical despite different names*

### Comparing `censius-1.7.0/src/censius.egg-info/PKG-INFO` & `censius-1.7.1/src/censius.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: censius
-Version: 1.7.0
+Version: 1.7.1
 Summary: API for Censius
 Home-page: https://github.com/Censius/censius-logs-python-sdk
 Author: Censius
 Author-email: dev@censius.ai
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `censius-1.7.0/src/censius.egg-info/SOURCES.txt` & `censius-1.7.1/src/censius.egg-info/SOURCES.txt`

 * *Files identical despite different names*

