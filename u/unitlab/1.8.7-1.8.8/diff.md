# Comparing `tmp/unitlab-1.8.7.tar.gz` & `tmp/unitlab-1.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unitlab-1.8.7.tar", last modified: Wed May 24 10:40:14 2023, max compression
+gzip compressed data, was "unitlab-1.8.8.tar", last modified: Tue Jun 13 12:52:23 2023, max compression
```

## Comparing `unitlab-1.8.7.tar` & `unitlab-1.8.8.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-05-24 10:40:14.097626 unitlab-1.8.7/
--rw-rw-r--   0 me        (1000) me        (1000)     1060 2022-11-07 13:04:44.000000 unitlab-1.8.7/LICENSE.md
--rw-rw-r--   0 me        (1000) me        (1000)       84 2023-02-15 09:26:00.000000 unitlab-1.8.7/MANIFEST.in
--rw-rw-r--   0 me        (1000) me        (1000)      654 2023-05-24 10:40:14.097626 unitlab-1.8.7/PKG-INFO
--rw-rw-r--   0 me        (1000) me        (1000)     1439 2023-05-23 07:41:41.000000 unitlab-1.8.7/README.md
--rw-rw-r--   0 me        (1000) me        (1000)      106 2023-05-24 10:40:14.097626 unitlab-1.8.7/setup.cfg
--rw-rw-r--   0 me        (1000) me        (1000)     1108 2023-05-24 10:39:59.000000 unitlab-1.8.7/setup.py
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-05-24 10:40:14.093626 unitlab-1.8.7/src/
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-05-24 10:40:14.097626 unitlab-1.8.7/src/unitlab/
--rw-rw-r--   0 me        (1000) me        (1000)      214 2023-05-23 13:05:07.000000 unitlab-1.8.7/src/unitlab/__init__.py
--rw-rw-r--   0 me        (1000) me        (1000)     2084 2023-05-24 10:17:52.000000 unitlab-1.8.7/src/unitlab/cli.py
--rw-rw-r--   0 me        (1000) me        (1000)    11524 2023-05-24 10:17:52.000000 unitlab-1.8.7/src/unitlab/client.py
--rw-rw-r--   0 me        (1000) me        (1000)      656 2023-05-23 07:35:04.000000 unitlab-1.8.7/src/unitlab/exceptions.py
--rw-rw-r--   0 me        (1000) me        (1000)     1785 2023-05-24 10:17:52.000000 unitlab-1.8.7/src/unitlab/run.py
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-05-24 10:40:14.097626 unitlab-1.8.7/src/unitlab.egg-info/
--rw-rw-r--   0 me        (1000) me        (1000)      654 2023-05-24 10:40:14.000000 unitlab-1.8.7/src/unitlab.egg-info/PKG-INFO
--rw-rw-r--   0 me        (1000) me        (1000)      373 2023-05-24 10:40:14.000000 unitlab-1.8.7/src/unitlab.egg-info/SOURCES.txt
--rw-rw-r--   0 me        (1000) me        (1000)        1 2023-05-24 10:40:14.000000 unitlab-1.8.7/src/unitlab.egg-info/dependency_links.txt
--rw-rw-r--   0 me        (1000) me        (1000)       44 2023-05-24 10:40:14.000000 unitlab-1.8.7/src/unitlab.egg-info/entry_points.txt
--rw-rw-r--   0 me        (1000) me        (1000)       55 2023-05-24 10:40:14.000000 unitlab-1.8.7/src/unitlab.egg-info/requires.txt
--rw-rw-r--   0 me        (1000) me        (1000)        8 2023-05-24 10:40:14.000000 unitlab-1.8.7/src/unitlab.egg-info/top_level.txt
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-13 12:52:23.083466 unitlab-1.8.8/
+-rw-rw-r--   0 me        (1000) me        (1000)     1060 2022-11-07 13:04:44.000000 unitlab-1.8.8/LICENSE.md
+-rw-rw-r--   0 me        (1000) me        (1000)       84 2023-02-15 09:26:00.000000 unitlab-1.8.8/MANIFEST.in
+-rw-rw-r--   0 me        (1000) me        (1000)      654 2023-06-13 12:52:23.083466 unitlab-1.8.8/PKG-INFO
+-rw-rw-r--   0 me        (1000) me        (1000)     1431 2023-06-13 08:13:23.000000 unitlab-1.8.8/README.md
+-rw-rw-r--   0 me        (1000) me        (1000)      106 2023-06-13 12:52:23.083466 unitlab-1.8.8/setup.cfg
+-rw-rw-r--   0 me        (1000) me        (1000)     1108 2023-06-13 11:16:56.000000 unitlab-1.8.8/setup.py
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-13 12:52:23.083466 unitlab-1.8.8/src/
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-13 12:52:23.083466 unitlab-1.8.8/src/unitlab/
+-rw-rw-r--   0 me        (1000) me        (1000)      214 2023-05-23 13:05:07.000000 unitlab-1.8.8/src/unitlab/__init__.py
+-rw-rw-r--   0 me        (1000) me        (1000)     2112 2023-06-13 12:01:49.000000 unitlab-1.8.8/src/unitlab/cli.py
+-rw-rw-r--   0 me        (1000) me        (1000)    12257 2023-06-13 12:34:06.000000 unitlab-1.8.8/src/unitlab/client.py
+-rw-rw-r--   0 me        (1000) me        (1000)      656 2023-06-13 10:04:19.000000 unitlab-1.8.8/src/unitlab/exceptions.py
+-rw-rw-r--   0 me        (1000) me        (1000)     1785 2023-06-13 12:01:36.000000 unitlab-1.8.8/src/unitlab/run.py
+-rw-rw-r--   0 me        (1000) me        (1000)     2089 2023-06-13 12:43:07.000000 unitlab-1.8.8/src/unitlab/utils.py
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-13 12:52:23.083466 unitlab-1.8.8/src/unitlab.egg-info/
+-rw-rw-r--   0 me        (1000) me        (1000)      654 2023-06-13 12:52:23.000000 unitlab-1.8.8/src/unitlab.egg-info/PKG-INFO
+-rw-rw-r--   0 me        (1000) me        (1000)      394 2023-06-13 12:52:23.000000 unitlab-1.8.8/src/unitlab.egg-info/SOURCES.txt
+-rw-rw-r--   0 me        (1000) me        (1000)        1 2023-06-13 12:52:23.000000 unitlab-1.8.8/src/unitlab.egg-info/dependency_links.txt
+-rw-rw-r--   0 me        (1000) me        (1000)       44 2023-06-13 12:52:23.000000 unitlab-1.8.8/src/unitlab.egg-info/entry_points.txt
+-rw-rw-r--   0 me        (1000) me        (1000)       55 2023-06-13 12:52:23.000000 unitlab-1.8.8/src/unitlab.egg-info/requires.txt
+-rw-rw-r--   0 me        (1000) me        (1000)        8 2023-06-13 12:52:23.000000 unitlab-1.8.8/src/unitlab.egg-info/top_level.txt
```

### Comparing `unitlab-1.8.7/LICENSE.md` & `unitlab-1.8.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `unitlab-1.8.7/PKG-INFO` & `unitlab-1.8.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitlab
-Version: 1.8.7
+Version: 1.8.8
 Home-page: https://github.com/teamunitlab/unitlab-sdk
 Author: Unitlab Inc.
 Author-email: team@unitlab.ai
 License: MIT
 Keywords: unitlab-sdk
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `unitlab-1.8.7/README.md` & `unitlab-1.8.8/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 <p align="center"> 
     <br>
-        <img src="assets/logo.aac4681.png" width="400"/>
+        <img src="assets/logo.png" width="400"/>
     <br>
 <p>
 <br>
 <p align="center">
     <a href="https://github.com/teamunitlab/unitlab-sdk">
         <img alt="Downloads" src="https://img.shields.io/pypi/dm/unitlab">
     </a>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 
-                          [assets/logo.aac4681.png]
+                              [assets/logo.png]
 
                                   [Downloads]
 [Unitlab.ai](https://unitlab.ai/) is an AI-driven data annotation platform that
 automates the collection of raw data, facilitating collaboration with human
 annotators to produce highly accurate labels for your machine learning models.
 With our service, you can optimize work efficiency, improve data quality, and
 reduce costs. ![](https://github.com/teamunitlab/unitlab-sdk/blob/main/assets/
```

### Comparing `unitlab-1.8.7/setup.py` & `unitlab-1.8.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="unitlab",
-    version="1.8.7",
+    version="1.8.8",
     license="MIT",
     author="Unitlab Inc.",
     author_email="team@unitlab.ai",
     packages=find_packages("src"),
     include_package_data=True,
     package_data={"static": ["*"], "Potato": ["*.so"]},
     classifiers=[
```

### Comparing `unitlab-1.8.7/src/unitlab/client.py` & `unitlab-1.8.8/src/unitlab/client.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,32 +5,15 @@
 import re
 
 import aiohttp
 import requests
 import tqdm
 
 from .exceptions import AuthenticationError
-
-BASE_URL = os.environ.get("UNITLAB_BASE_URL", "https://api.unitlab.ai")
-SDK_URL = BASE_URL + "/api/sdk/"
-
-
-SDK_ENPOINTS = {
-    "ai_models": SDK_URL + "ai-models/",
-    "ai_model": SDK_URL + "ai-model/{}/",
-    "tasks": SDK_URL + "tasks/",
-    "task": SDK_URL + "tasks/{}/",
-    "task_datasources": SDK_URL + "tasks/{}/datasources/",
-    "task_workers": SDK_URL + "tasks/{}/workers/",
-    "task_statistics": SDK_URL + "tasks/{}/statistics/",
-    "upload_data": SDK_URL + "upload-data/",
-    "download_data": SDK_URL + "tasks/{}/download-data/",
-    "datasets": SDK_URL + "datasets/",
-    "dataset": SDK_URL + "datasets/{}/",
-}
+from .utils import ENDPOINTS, send_request
 
 
 class UnitlabClient:
     """A client with a connection to the Unitlab.ai platform.
 
     Note:
         Please refer to the `Python SDK quickstart <https://docs.unitlab.ai/tutorials/python-sdk-quickstart>`__ for a full example of working with the Python SDK.
@@ -112,77 +95,95 @@
 
     def tasks(self):
         """Get a list of all tasks.
 
         Returns:
             A list of all tasks.
         """
-        r = self.api_session.get(SDK_ENPOINTS["tasks"], headers=self._get_headers())
-        r.raise_for_status()
-        return r.json()
+        response = send_request(
+            {
+                "method": "GET",
+                "endpoint": ENDPOINTS["tasks"],
+                "headers": self._get_headers(),
+            },
+            session=self.api_session,
+        )
+        return response.json()
 
     def task(self, task_id):
         """Get a task by id.
 
         Args:
             task_id: The id of the task.
         Returns:
             A task.
         """
-        r = self.api_session.get(
-            SDK_ENPOINTS["task"].format(task_id),
-            headers=self._get_headers(),
+        response = send_request(
+            {
+                "method": "GET",
+                "endpoint": ENDPOINTS["task"].format(task_id),
+                "headers": self._get_headers(),
+            },
+            session=self.api_session,
         )
-        r.raise_for_status()
-        return r.json()
+        return response.json()
 
     def task_data(self, task_id):
         """Get the data of a task by id.
 
         Args:
             task_id: The id of the task.
         Returns:
             The data of a task.
         """
-        r = self.api_session.get(
-            SDK_ENPOINTS["task_datasources"].format(task_id),
-            headers=self._get_headers(),
+        response = send_request(
+            {
+                "method": "GET",
+                "endpoint": ENDPOINTS["task_datasources"].format(task_id),
+                "headers": self._get_headers(),
+            },
+            session=self.api_session,
         )
-        r.raise_for_status()
-        return r.json()
+        return response.json()
 
     def task_workers(self, task_id):
         """Get the workers of a task by id.
 
         Args:
             task_id: The id of the task.
         Returns:
             The workers of a task.
         """
-        r = self.api_session.get(
-            SDK_ENPOINTS["task_workers"].format(task_id),
-            headers=self._get_headers(),
+        response = send_request(
+            {
+                "method": "GET",
+                "endpoint": ENDPOINTS["task_workers"].format(task_id),
+                "headers": self._get_headers(),
+            },
+            session=self.api_session,
         )
-        r.raise_for_status()
-        return r.json()
+        return response.json()
 
     def task_statistics(self, task_id):
         """Get the statistics of a task by id.
 
         Args:
             task_id: The id of the task.
         Returns:
             The statistics of a task.
         """
-        r = self.api_session.get(
-            SDK_ENPOINTS["task_statistics"].format(task_id),
-            headers=self._get_headers(),
+        response = send_request(
+            {
+                "method": "GET",
+                "endpoint": ENDPOINTS["task_statistics"].format(task_id),
+                "headers": self._get_headers(),
+            },
+            session=self.api_session,
         )
-        r.raise_for_status()
-        return r.json()
+        return response.json()
 
     def upload_data(self, task_id, directory, batch_size=100):
         """Upload data to a task by id.
 
         Args:
             task_id: The id of the task.
             directory: The directory of images to upload.
@@ -190,20 +191,31 @@
         Returns:
             The upload status.
         """
 
         if not os.path.isdir(directory):
             raise ValueError(f"Directory {directory} does not exist")
 
+        # set correct host
+        send_request(
+            {
+                "method": "GET",
+                "endpoint": "check",
+                "headers": self._get_headers(),
+            },
+            session=self.api_session,
+        )
+        URL = os.environ["UNITLAB_BASE_URL"] + ENDPOINTS["upload_data"]
+
         async def post_image(session: aiohttp.ClientSession, image: str, task_id: str):
             with open(image, "rb") as img:
                 try:
                     response = await session.request(
                         "POST",
-                        url=SDK_ENPOINTS["upload_data"],
+                        url=URL,
                         data=aiohttp.FormData(fields={"task": task_id, "image": img}),
                     )
                     response.raise_for_status()
                     return 1 if response.status == 201 else 0
                 except Exception as e:
                     logging.error(f"Error uploading image {image} - {e}")
                     return 0
@@ -260,19 +272,22 @@
         """Download data from a task by id.
 
         Args:
             task_id: The id of the task.
         Returns:
             Writes the data to a json file.
         """
-        response = self.api_session.get(
-            url=SDK_ENPOINTS["download_data"].format(task_id),
-            headers=self._get_headers(),
+        response = send_request(
+            {
+                "method": "GET",
+                "endpoint": ENDPOINTS["download_data"].format(task_id),
+                "headers": self._get_headers(),
+            },
+            session=self.api_session,
         )
-        response.raise_for_status()
         with self.api_session.get(
             url=response.json()["file"],
             stream=True,
         ) as r:
             r.raise_for_status()
             if "Content-Disposition" in r.headers.keys():
                 content_disposition = r.headers["Content-Disposition"]
@@ -291,56 +306,74 @@
 
     def ai_models(self):
         """Get a list of all ai models.
 
         Returns:
             A list of all ai models.
         """
-        r = self.api_session.get(SDK_ENPOINTS["ai_models"], headers=self._get_headers())
-        r.raise_for_status()
-        return r.json()
+        response = send_request(
+            {
+                "method": "GET",
+                "endpoint": ENDPOINTS["ai_models"],
+                "headers": self._get_headers(),
+            },
+            session=self.api_session,
+        )
+        return response.json()
 
     def ai_model(self, ai_model_id):
         """Get an ai model by id.
 
         Args:
             ai_model_id: The id of the ai model.
         Returns:
             An ai model.
         """
-        r = self.api_session.get(
-            SDK_ENPOINTS["ai_model"].format(ai_model_id),
-            headers=self._get_headers(),
+        response = send_request(
+            {
+                "method": "GET",
+                "endpoint": ENDPOINTS["ai_model"].format(ai_model_id),
+                "headers": self._get_headers(),
+            },
+            session=self.api_session,
         )
-        r.raise_for_status()
-        return r.json()
+        return response.json()
 
     def datasets(self):
         """Get a list of all datasets.
 
         Returns:
             A list of all datasets.
         """
-        r = self.api_session.get(SDK_ENPOINTS["datasets"], headers=self._get_headers())
-        r.raise_for_status()
-        return r.json()
+        response = send_request(
+            {
+                "method": "GET",
+                "endpoint": ENDPOINTS["datasets"],
+                "headers": self._get_headers(),
+            },
+            session=self.api_session,
+        )
+        return response.json()
 
     def dataset(self, dataset_id):
         """Download a dataset by id.
 
         Args:
             dataset_id: The id of the dataset.
         Returns:
             Writes the data to a json file.
         """
-        response = self.api_session.get(
-            url=SDK_ENPOINTS["dataset"].format(dataset_id),
-            headers=self._get_headers(),
+        response = send_request(
+            {
+                "method": "GET",
+                "endpoint": ENDPOINTS["dataset"].format(dataset_id),
+                "headers": self._get_headers(),
+            },
+            session=self.api_session,
         )
-        response.raise_for_status()
         with self.api_session.get(
             url=response.json()["file"],
             stream=True,
         ) as r:
             r.raise_for_status()
             if "Content-Disposition" in r.headers.keys():
                 content_disposition = r.headers["Content-Disposition"]
```

### Comparing `unitlab-1.8.7/src/unitlab/exceptions.py` & `unitlab-1.8.8/src/unitlab/exceptions.py`

 * *Files identical despite different names*

### Comparing `unitlab-1.8.7/src/unitlab/run.py` & `unitlab-1.8.8/src/unitlab/run.py`

 * *Files identical despite different names*

### Comparing `unitlab-1.8.7/src/unitlab.egg-info/PKG-INFO` & `unitlab-1.8.8/src/unitlab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitlab
-Version: 1.8.7
+Version: 1.8.8
 Home-page: https://github.com/teamunitlab/unitlab-sdk
 Author: Unitlab Inc.
 Author-email: team@unitlab.ai
 License: MIT
 Keywords: unitlab-sdk
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

