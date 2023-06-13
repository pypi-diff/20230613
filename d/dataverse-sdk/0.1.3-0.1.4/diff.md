# Comparing `tmp/dataverse-sdk-0.1.3.tar.gz` & `tmp/dataverse-sdk-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataverse-sdk-0.1.3.tar", last modified: Wed May 24 06:43:24 2023, max compression
+gzip compressed data, was "dataverse-sdk-0.1.4.tar", last modified: Tue Jun 13 10:18:31 2023, max compression
```

## Comparing `dataverse-sdk-0.1.3.tar` & `dataverse-sdk-0.1.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2023-05-24 06:43:24.047591 dataverse-sdk-0.1.3/
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     5983 2023-05-24 06:43:24.047472 dataverse-sdk-0.1.3/PKG-INFO
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     5743 2023-05-24 06:41:33.000000 dataverse-sdk-0.1.3/README.md
-drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2023-05-24 06:43:24.044969 dataverse-sdk-0.1.3/dataverse_sdk/
--rw-r--r--   0 yihsuanchen   (501) staff       (20)      825 2023-05-12 08:24:04.000000 dataverse-sdk-0.1.3/dataverse_sdk/__init__.py
-drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2023-05-24 06:43:24.045980 dataverse-sdk-0.1.3/dataverse_sdk/apis/
--rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-05-12 08:24:04.000000 dataverse-sdk-0.1.3/dataverse_sdk/apis/__init__.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)    10150 2023-05-24 06:41:33.000000 dataverse-sdk-0.1.3/dataverse_sdk/apis/backend.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)    19626 2023-05-24 06:41:33.000000 dataverse-sdk-0.1.3/dataverse_sdk/client.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     1550 2023-05-12 08:24:04.000000 dataverse-sdk-0.1.3/dataverse_sdk/connections.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)      587 2023-05-12 08:24:04.000000 dataverse-sdk-0.1.3/dataverse_sdk/constants.py
-drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2023-05-24 06:43:24.046311 dataverse-sdk-0.1.3/dataverse_sdk/exceptions/
--rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-05-12 08:24:04.000000 dataverse-sdk-0.1.3/dataverse_sdk/exceptions/__init__.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)       49 2023-05-12 08:24:04.000000 dataverse-sdk-0.1.3/dataverse_sdk/exceptions/client.py
-drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2023-05-24 06:43:24.047047 dataverse-sdk-0.1.3/dataverse_sdk/schemas/
--rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-05-12 08:24:04.000000 dataverse-sdk-0.1.3/dataverse_sdk/schemas/__init__.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     3036 2023-05-17 07:09:24.000000 dataverse-sdk-0.1.3/dataverse_sdk/schemas/api.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     8689 2023-05-24 06:41:33.000000 dataverse-sdk-0.1.3/dataverse_sdk/schemas/client.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     1164 2023-05-12 08:24:04.000000 dataverse-sdk-0.1.3/dataverse_sdk/schemas/common.py
-drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2023-05-24 06:43:24.047288 dataverse-sdk-0.1.3/dataverse_sdk/utils/
--rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-05-12 08:24:04.000000 dataverse-sdk-0.1.3/dataverse_sdk/utils/__init__.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)      371 2023-05-12 08:24:04.000000 dataverse-sdk-0.1.3/dataverse_sdk/utils/utils.py
-drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2023-05-24 06:43:24.045739 dataverse-sdk-0.1.3/dataverse_sdk.egg-info/
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     5983 2023-05-24 06:43:24.000000 dataverse-sdk-0.1.3/dataverse_sdk.egg-info/PKG-INFO
--rw-r--r--   0 yihsuanchen   (501) staff       (20)      629 2023-05-24 06:43:24.000000 dataverse-sdk-0.1.3/dataverse_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 yihsuanchen   (501) staff       (20)        1 2023-05-24 06:43:24.000000 dataverse-sdk-0.1.3/dataverse_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 yihsuanchen   (501) staff       (20)       18 2023-05-24 06:43:24.000000 dataverse-sdk-0.1.3/dataverse_sdk.egg-info/requires.txt
--rw-r--r--   0 yihsuanchen   (501) staff       (20)       14 2023-05-24 06:43:24.000000 dataverse-sdk-0.1.3/dataverse_sdk.egg-info/top_level.txt
--rw-r--r--   0 yihsuanchen   (501) staff       (20)       38 2023-05-24 06:43:24.047627 dataverse-sdk-0.1.3/setup.cfg
--rw-r--r--   0 yihsuanchen   (501) staff       (20)      613 2023-05-24 06:41:33.000000 dataverse-sdk-0.1.3/setup.py
+drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2023-06-13 10:18:31.396193 dataverse-sdk-0.1.4/
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     5983 2023-06-13 10:18:31.396077 dataverse-sdk-0.1.4/PKG-INFO
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     5743 2023-05-24 06:41:33.000000 dataverse-sdk-0.1.4/README.md
+drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2023-06-13 10:18:31.393017 dataverse-sdk-0.1.4/dataverse_sdk/
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)      825 2023-05-12 08:24:04.000000 dataverse-sdk-0.1.4/dataverse_sdk/__init__.py
+drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2023-06-13 10:18:31.394163 dataverse-sdk-0.1.4/dataverse_sdk/apis/
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-05-12 08:24:04.000000 dataverse-sdk-0.1.4/dataverse_sdk/apis/__init__.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)    10144 2023-06-13 10:15:56.000000 dataverse-sdk-0.1.4/dataverse_sdk/apis/backend.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)    20188 2023-06-13 10:15:56.000000 dataverse-sdk-0.1.4/dataverse_sdk/client.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     1550 2023-05-12 08:24:04.000000 dataverse-sdk-0.1.4/dataverse_sdk/connections.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)      587 2023-06-09 02:47:03.000000 dataverse-sdk-0.1.4/dataverse_sdk/constants.py
+drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2023-06-13 10:18:31.394389 dataverse-sdk-0.1.4/dataverse_sdk/exceptions/
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-05-12 08:24:04.000000 dataverse-sdk-0.1.4/dataverse_sdk/exceptions/__init__.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)       49 2023-05-12 08:24:04.000000 dataverse-sdk-0.1.4/dataverse_sdk/exceptions/client.py
+drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2023-06-13 10:18:31.395465 dataverse-sdk-0.1.4/dataverse_sdk/schemas/
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-05-12 08:24:04.000000 dataverse-sdk-0.1.4/dataverse_sdk/schemas/__init__.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     3036 2023-05-17 07:09:24.000000 dataverse-sdk-0.1.4/dataverse_sdk/schemas/api.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     9954 2023-06-13 10:15:56.000000 dataverse-sdk-0.1.4/dataverse_sdk/schemas/client.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     1164 2023-05-12 08:24:04.000000 dataverse-sdk-0.1.4/dataverse_sdk/schemas/common.py
+drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2023-06-13 10:18:31.395857 dataverse-sdk-0.1.4/dataverse_sdk/utils/
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-05-12 08:24:04.000000 dataverse-sdk-0.1.4/dataverse_sdk/utils/__init__.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)      371 2023-05-12 08:24:04.000000 dataverse-sdk-0.1.4/dataverse_sdk/utils/utils.py
+drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2023-06-13 10:18:31.393952 dataverse-sdk-0.1.4/dataverse_sdk.egg-info/
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     5983 2023-06-13 10:18:31.000000 dataverse-sdk-0.1.4/dataverse_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)      629 2023-06-13 10:18:31.000000 dataverse-sdk-0.1.4/dataverse_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)        1 2023-06-13 10:18:31.000000 dataverse-sdk-0.1.4/dataverse_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)       18 2023-06-13 10:18:31.000000 dataverse-sdk-0.1.4/dataverse_sdk.egg-info/requires.txt
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)       14 2023-06-13 10:18:31.000000 dataverse-sdk-0.1.4/dataverse_sdk.egg-info/top_level.txt
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)       38 2023-06-13 10:18:31.396228 dataverse-sdk-0.1.4/setup.cfg
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)      613 2023-06-13 10:15:56.000000 dataverse-sdk-0.1.4/setup.py
```

### Comparing `dataverse-sdk-0.1.3/PKG-INFO` & `dataverse-sdk-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataverse-sdk
-Version: 0.1.3
+Version: 0.1.4
 Summary: Dataverse SDK For Python
 Home-page: 
 Author: LinkerVision
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9, <4
 Description-Content-Type: text/markdown
```

### Comparing `dataverse-sdk-0.1.3/README.md` & `dataverse-sdk-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `dataverse-sdk-0.1.3/dataverse_sdk/__init__.py` & `dataverse-sdk-0.1.4/dataverse_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `dataverse-sdk-0.1.3/dataverse_sdk/apis/backend.py` & `dataverse-sdk-0.1.4/dataverse_sdk/apis/backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -178,15 +178,15 @@
         if current_user:
             kwargs["current_user"] = current_user
         if exclude_sensor_type is not None:
             kwargs["exclude_sensor_type"] = exclude_sensor_type.value
         if image_type is not None:
             kwargs["ontology__image_type"] = image_type.value
         resp = self.send_request(
-            url=f"{self.host}/api/projects/basic/?{urlencode(kwargs)}",
+            url=f"{self.host}/api/projects/?{urlencode(kwargs)}",
             method="get",
             headers=self.headers,
         )
         return resp.json()["results"]
 
     def list_ml_models(self, project_id: int, **kwargs) -> list:
         kwargs["project"] = project_id
```

### Comparing `dataverse-sdk-0.1.3/dataverse_sdk/client.py` & `dataverse-sdk-0.1.4/dataverse_sdk/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -184,30 +184,30 @@
         return Project.create(project_data)
 
     def list_projects(
         self,
         current_user: bool = True,
         exclude_sensor_type: Optional[SensorType] = None,
         image_type: Optional[OntologyImageType] = None,
-    ) -> list:
+    ) -> list[Project]:
         """list projects in dataverse (with given filter query params)
 
         Parameters
         ----------
         current_user : bool, optional
             only show the projects of current user, by default True
         exclude_sensor_type : Optional[SensorType], optional
             exclude the projects with the given sensor type, by default None
         image_type : Optional[OntologyImageType], optional
             only include the projects with the given image type, by default None
 
         Returns
         -------
-        list
-            list of projects [{'id': 5, 'name': 'Kitti Sequential Project'}, {'id': 6, 'name': 'project2'}]
+        list[Projects]
+            list of project items
 
         Raises
         ------
         ClientConnectionError
             raise error if there is any error occurs when calling backend APIs.
         """
 
@@ -215,17 +215,21 @@
             project_list: list = self._api_client.list_projects(
                 current_user=current_user,
                 exclude_sensor_type=exclude_sensor_type,
                 image_type=image_type,
             )
         except Exception as e:
             raise ClientConnectionError(f"Failed to get the projects: {e}")
-        return project_list
+        output_project_list = []
+        for project in project_list:
+            output_project_list.append(Project.create(project))
+        return output_project_list
 
-    def get_project(self, project_id: int):
+    @staticmethod
+    def get_project(project_id: int, client: Optional["DataverseClient"] = None):
         """Get project detail by project-id
 
         Parameters
         ----------
         project_id : int
             project-id in db
 
@@ -235,52 +239,72 @@
             Project basemodel from host response for client usage
 
         Raises
         ------
         ClientConnectionError
             raise exception if there is any error occurs when calling backend APIs.
         """
+        if client is None:
+            client = DataverseClient.get_client()
+        api = client._api_client
 
         try:
-            project_data: dict = self._api_client.get_project(project_id=project_id)
+            project_data: dict = api.get_project(project_id=project_id)
         except Exception as e:
             raise ClientConnectionError(f"Failed to get the project: {e}")
         return Project.create(project_data)
 
     @staticmethod
     def list_models(
         project_id: int,
         client: Optional["DataverseClient"] = None,
-    ) -> list:
+        project: Optional["Project"] = None,
+    ) -> list[MLModel]:
         """Get the model list by project id
 
         Parameters
         ----------
         project_id : int
         client : Optional["DataverseClient"], optional
             clientclass, by default None
+        project: Optional["Project"]
+            project basemodel, by default None
 
         Returns
         -------
         list
-            model list from api response
+            list of model items
 
         Raises
         ------
         ClientConnectionError
             raise exception if there is any error occurs when calling backend APIs.
         """
         if client is None:
             client = DataverseClient.get_client()
         api = client._api_client
         try:
             model_list: list = api.list_ml_models(project_id=project_id)
         except Exception as e:
             raise ClientConnectionError(f"Failed to get the models: {e}")
-        return model_list
+        if project is None:
+            project = DataverseClient.get_project(project_id=project_id)
+        output_model_list = []
+        for model_data in model_list:
+            model_data.update(
+                {
+                    "project": project,
+                    "triton_model_name": model_data["configuration"][
+                        "triton_model_name"
+                    ],
+                }
+            )
+            ml_model = MLModel.create(model_data)
+            output_model_list.append(ml_model)
+        return output_model_list
 
     @staticmethod
     def get_model(
         model_id: int,
         client: Optional["DataverseClient"] = None,
         project: Optional["Project"] = None,
     ) -> MLModel:
@@ -308,27 +332,18 @@
             client = DataverseClient.get_client()
         api = client._api_client
         try:
             model_data: dict = api.get_ml_model(model_id=model_id)
         except Exception as e:
             raise ClientConnectionError(f"Failed to get the dataset: {e}")
 
-        target_class_id = {
-            ontology_class["id"] for ontology_class in model_data["classes"]
-        }
         if project is None:
             project = client.get_project(project_id=model_data["project"]["id"])
-        # get classes used in the model
-        classes = [
-            ontology_class
-            for ontology_class in project.ontology.classes
-            if ontology_class.id in target_class_id
-        ]
-        model_data.update({"id": model_id, "project": project, "classes": classes})
-        return MLModel(**model_data)
+        model_data.update({"id": model_id, "project": project})
+        return MLModel.create(model_data)
 
     @staticmethod
     def get_label_file(
         model_id: int, client: Optional["DataverseClient"] = None
     ) -> Optional[BytesIO]:
         if client is None:
             client = DataverseClient.get_client()
```

### Comparing `dataverse-sdk-0.1.3/dataverse_sdk/connections.py` & `dataverse-sdk-0.1.4/dataverse_sdk/connections.py`

 * *Files identical despite different names*

### Comparing `dataverse-sdk-0.1.3/dataverse_sdk/constants.py` & `dataverse-sdk-0.1.4/dataverse_sdk/constants.py`

 * *Files identical despite different names*

### Comparing `dataverse-sdk-0.1.3/dataverse_sdk/schemas/api.py` & `dataverse-sdk-0.1.4/dataverse_sdk/schemas/api.py`

 * *Files identical despite different names*

### Comparing `dataverse-sdk-0.1.3/dataverse_sdk/schemas/client.py` & `dataverse-sdk-0.1.4/dataverse_sdk/schemas/client.py`

 * *Files 13% similar despite different names*

```diff
@@ -124,29 +124,33 @@
     annotation_format: str
 
     class Config:
         extra = "allow"
 
 
 class Project(BaseModel):
-    id: Optional[int] = None
+    id: int
     name: str
     description: Optional[str] = None
     ego_car: Optional[str] = None
     ontology: Ontology
-    sensors: list[Sensor]
+    sensors: Optional[list[Sensor]] = None
     project_tag: Optional[ProjectTag] = None
 
     @classmethod
     def create(cls, project_data: dict) -> "Project":
         ontology = Ontology.create(project_data["ontology"])
-        sensors = [
-            Sensor.create(sensor_data) for sensor_data in project_data["sensors"]
-        ]
-        if project_data["project_tag"] is None:
+        # TODO modify the condition if list projects results with list fields
+        if project_data.get("sensors") is None:
+            sensors = None
+        else:
+            sensors = [
+                Sensor.create(sensor_data) for sensor_data in project_data["sensors"]
+            ]
+        if project_data.get("project_tag") is None:
             project_data["project_tag"] = {}
         project_tag = ProjectTag.create(project_data["project_tag"])
         return cls(
             id=project_data["id"],
             name=project_data["name"],
             description=project_data["description"],
             ego_car=project_data["ego_car"],
@@ -154,15 +158,15 @@
             sensors=sensors,
             project_tag=project_tag,
         )
 
     def list_models(self) -> list:
         from ..client import DataverseClient
 
-        model_list: list = DataverseClient.list_models(project_id=self.id)
+        model_list: list = DataverseClient.list_models(project_id=self.id, project=self)
         return model_list
 
     def get_model(self, model_id: int):
         from ..client import DataverseClient
 
         model_data = DataverseClient.get_model(model_id=model_id, project=self)
         return model_data
@@ -291,14 +295,46 @@
     classes: list
     triton_model_name: str
     description: Optional[str] = None
 
     class Config:
         extra = "allow"
 
+    @classmethod
+    def create(cls, model_data: dict) -> "MLModel":
+        if isinstance(model_data["classes"][0], dict):
+            target_class_id = {
+                ontology_class["id"] for ontology_class in model_data["classes"]
+            }
+        else:
+            target_class_id = set(model_data["classes"])
+
+        from ..client import DataverseClient
+
+        if model_data["project"] is None:
+            project = DataverseClient.get_project(
+                project_id=model_data["project"]["id"]
+            )
+        else:
+            project = model_data["project"]
+        # get classes used in the model
+        classes = [
+            ontology_class
+            for ontology_class in project.ontology.classes
+            if ontology_class.id in target_class_id
+        ]
+        return cls(
+            id=model_data["id"],
+            name=model_data["name"],
+            project=project,
+            classes=classes,
+            updated_at=model_data["updated_at"],
+            triton_model_name=model_data["triton_model_name"],
+        )
+
     def get_label_file(self) -> dict:
         from ..client import DataverseClient
 
         labels: dict = DataverseClient.get_label_file(model_id=self.id)
         return labels
 
     def get_triton_model_file(self):
```

### Comparing `dataverse-sdk-0.1.3/dataverse_sdk/schemas/common.py` & `dataverse-sdk-0.1.4/dataverse_sdk/schemas/common.py`

 * *Files identical despite different names*

### Comparing `dataverse-sdk-0.1.3/dataverse_sdk.egg-info/PKG-INFO` & `dataverse-sdk-0.1.4/dataverse_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataverse-sdk
-Version: 0.1.3
+Version: 0.1.4
 Summary: Dataverse SDK For Python
 Home-page: 
 Author: LinkerVision
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9, <4
 Description-Content-Type: text/markdown
```

### Comparing `dataverse-sdk-0.1.3/dataverse_sdk.egg-info/SOURCES.txt` & `dataverse-sdk-0.1.4/dataverse_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dataverse-sdk-0.1.3/setup.py` & `dataverse-sdk-0.1.4/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 AUTHOR = "LinkerVision"
 PACKAGE_NAME = "dataverse-sdk"
-PACKAGE_VERSION = "0.1.3"
+PACKAGE_VERSION = "0.1.4"
 DESC = "Dataverse SDK For Python"
 with open("README.md", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name=PACKAGE_NAME,
     version=PACKAGE_VERSION,
```

