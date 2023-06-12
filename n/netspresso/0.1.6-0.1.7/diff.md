# Comparing `tmp/netspresso-0.1.6-py3-none-any.whl.zip` & `tmp/netspresso-0.1.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,25 +1,26 @@
-Zip file size: 19021 bytes, number of entries: 23
--rw-rw-rw-  2.0 fat       23 b- defN 23-Jun-08 04:37 netspresso/__init__.py
--rw-rw-rw-  2.0 fat    23052 b- defN 23-Jun-08 02:23 netspresso/compressor/__init__.py
+Zip file size: 20286 bytes, number of entries: 24
+-rw-rw-rw-  2.0 fat       23 b- defN 23-Jun-12 20:25 netspresso/__init__.py
+-rw-rw-rw-  2.0 fat    23322 b- defN 23-Jun-12 20:25 netspresso/compressor/__init__.py
 -rw-rw-rw-  2.0 fat     8456 b- defN 23-Jun-05 06:16 netspresso/compressor/client/__init__.py
--rw-rw-rw-  2.0 fat      536 b- defN 23-Jun-05 04:34 netspresso/compressor/client/config.py
+-rw-rw-rw-  2.0 fat      535 b- defN 23-Jun-12 20:43 netspresso/compressor/client/config.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-05 02:41 netspresso/compressor/client/schemas/__init__.py
 -rw-rw-rw-  2.0 fat     2644 b- defN 23-Jun-05 02:41 netspresso/compressor/client/schemas/auth.py
 -rw-rw-rw-  2.0 fat      482 b- defN 23-Jun-05 02:41 netspresso/compressor/client/schemas/common.py
--rw-rw-rw-  2.0 fat     4141 b- defN 23-Jun-05 02:41 netspresso/compressor/client/schemas/compression.py
--rw-rw-rw-  2.0 fat     5705 b- defN 23-Jun-08 02:08 netspresso/compressor/client/schemas/model.py
+-rw-rw-rw-  2.0 fat     4108 b- defN 23-Jun-12 20:25 netspresso/compressor/client/schemas/compression.py
+-rw-rw-rw-  2.0 fat     5681 b- defN 23-Jun-12 20:25 netspresso/compressor/client/schemas/model.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-05 02:41 netspresso/compressor/client/utils/__init__.py
 -rw-rw-rw-  2.0 fat      481 b- defN 23-Jun-05 02:41 netspresso/compressor/client/utils/common.py
 -rw-rw-rw-  2.0 fat      840 b- defN 23-Jun-07 07:58 netspresso/compressor/client/utils/enum.py
 -rw-rw-rw-  2.0 fat     3814 b- defN 23-Jun-05 02:41 netspresso/compressor/client/utils/validator.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-05 02:41 netspresso/compressor/core/__init__.py
--rw-rw-rw-  2.0 fat      563 b- defN 23-Jun-05 02:41 netspresso/compressor/core/compression.py
--rw-rw-rw-  2.0 fat      521 b- defN 23-Jun-05 02:41 netspresso/compressor/core/model.py
+-rw-rw-rw-  2.0 fat     1900 b- defN 23-Jun-12 20:25 netspresso/compressor/core/compression.py
+-rw-rw-rw-  2.0 fat     2966 b- defN 23-Jun-12 20:25 netspresso/compressor/core/model.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-05 02:41 netspresso/compressor/utils/__init__.py
+-rw-rw-rw-  2.0 fat     2035 b- defN 23-Jun-12 20:25 netspresso/compressor/utils/model.py
 -rw-rw-rw-  2.0 fat      236 b- defN 23-Jun-05 02:41 netspresso/compressor/utils/token.py
--rw-rw-rw-  2.0 fat    11558 b- defN 23-Jun-08 04:44 netspresso-0.1.6.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      872 b- defN 23-Jun-08 04:44 netspresso-0.1.6.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-08 04:44 netspresso-0.1.6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 23-Jun-08 04:44 netspresso-0.1.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     2142 b- defN 23-Jun-08 04:44 netspresso-0.1.6.dist-info/RECORD
-23 files, 66169 bytes uncompressed, 15433 bytes compressed:  76.7%
+-rw-rw-rw-  2.0 fat    11558 b- defN 23-Jun-12 20:44 netspresso-0.1.7.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      769 b- defN 23-Jun-12 20:44 netspresso-0.1.7.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-12 20:44 netspresso-0.1.7.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 23-Jun-12 20:44 netspresso-0.1.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     2237 b- defN 23-Jun-12 20:44 netspresso-0.1.7.dist-info/RECORD
+24 files, 72190 bytes uncompressed, 16550 bytes compressed:  77.1%
```

## zipnote {}

```diff
@@ -45,26 +45,29 @@
 
 Filename: netspresso/compressor/core/model.py
 Comment: 
 
 Filename: netspresso/compressor/utils/__init__.py
 Comment: 
 
+Filename: netspresso/compressor/utils/model.py
+Comment: 
+
 Filename: netspresso/compressor/utils/token.py
 Comment: 
 
-Filename: netspresso-0.1.6.dist-info/LICENSE
+Filename: netspresso-0.1.7.dist-info/LICENSE
 Comment: 
 
-Filename: netspresso-0.1.6.dist-info/METADATA
+Filename: netspresso-0.1.7.dist-info/METADATA
 Comment: 
 
-Filename: netspresso-0.1.6.dist-info/WHEEL
+Filename: netspresso-0.1.7.dist-info/WHEEL
 Comment: 
 
-Filename: netspresso-0.1.6.dist-info/top_level.txt
+Filename: netspresso-0.1.7.dist-info/top_level.txt
 Comment: 
 
-Filename: netspresso-0.1.6.dist-info/RECORD
+Filename: netspresso-0.1.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## netspresso/__init__.py

```diff
@@ -1 +1 @@
-__version__ = "0.1.6"
+__version__ = "0.1.7"
```

## netspresso/compressor/__init__.py

```diff
@@ -17,27 +17,33 @@
     AutoCompressionRequest,
     CompressionRequest,
     GetAvailableLayersRequest,
     CreateCompressionRequest,
     RecommendationRequest,
     UploadDatasetRequest,
 )
-from netspresso.compressor.core.model import CompressedModel, Model
-from netspresso.compressor.core.compression import CompressionBase, CompressionInfo
+from netspresso.compressor.core.model import CompressedModel, Model, ModelCollection
+from netspresso.compressor.core.compression import CompressionInfo
+from netspresso.compressor.utils.model import (
+    get_compressed_model_object,
+    get_model_collection_object,
+    get_model_object,
+)
 from netspresso.compressor.utils.token import check_jwt_exp
 
 
 class ModelCompressor:
     def __init__(self, email: str, password: str):
         """Initialize the Model Compressor.
 
         Args:
             email (str): The email address for a user account.
             password (str): The password for a user account.
         """
+
         self.email = email
         self.password = password
         self.client = ModelCompressorAPIClient()
         self.__login()
 
     def __login(self) -> None:
         try:
@@ -76,141 +82,148 @@
 
         Raises:
             e: If an error occurs while getting credit information.
 
         Returns:
             int: The total amount of available NetsPresso credits.
         """
+
         try:
             credit = self.client.get_credit(access_token=self.access_token)
             logger.info(f"Get Credit successful. Credit: {credit.total}")
 
             return credit.total
 
         except Exception as e:
             logger.error(f"Get Credit failed. Error: {e}")
             raise e
 
     @validate_token
     def upload_model(
-        self, model_name: str, task: Task, framework: Framework, file_path: str, input_shapes: List = []
+        self, model_name: str, task: Task, framework: Framework, file_path: str, input_shapes: List[Dict[str, int]] = []
     ) -> Model:
         """Upload a model for compression.
 
         Args:
             model_name (str): The name of the model.
             task (Task): The task of the model.
             framework (Framework): The framework of the model.
             file_path (str): The file path where the model is located.
-            input_shapes (List[str], optional): Input shapes of the model. Defaults to [].
-
-        Note:
-            * Currently, only single input models are supported.
-            * If the model's `input_shapes` are **dynamic**, it must be provided as a required input.
-            * If the model's `input_shapes` are **static**, it must be set to the same shape as the model's input tensor.
+            input_shapes (List[Dict[str, int]], optional): Input shapes of the model. Defaults to [].
 
         Raises:
             e: If an error occurs while uploading the model.
 
         Returns:
             Model: Uploaded model object.
         """
+
         try:
             logger.info("Uploading Model...")
             data = UploadModelRequest(
                 model_name=model_name,
                 task=task.value,
                 framework=framework.value,
                 file_path=file_path,
                 input_layers=input_shapes,
             )
             model_info = self.client.upload_model(data=data, access_token=self.access_token)
-            model = Model(model_info)
+            model = get_model_object(model_info=model_info)
+
             logger.info(f"Upload model successful. Model ID: {model.model_id}")
 
             return model
 
         except Exception as e:
             logger.error(f"Upload model failed. Error: {e}")
             raise e
 
     @validate_token
-    def get_models(self) -> List[Dict[str, Any]]:
+    def get_models(self) -> List[ModelCollection]:
         """Get the list of uploaded & compressed models.
 
         Raises:
             e: If an error occurs while getting the model list.
 
         Returns:
-            List[Dict[str, Any]]: The list of uploaded & compressed models.
+            List[ModelCollection]: The list of uploaded & compressed models.
         """
+
         try:
             logger.info("Getting model list...")
             models = []
             parent_models = self.client.get_parent_models(is_simple=True, access_token=self.access_token)
-            uploaded_models = [
-                vars(Model(parent_model)) for parent_model in parent_models if parent_model.origin_from == "custom"
-            ]
-            for uploaded_model in uploaded_models:
-                children_models = self.client.get_children_models(
-                    model_id=uploaded_model["model_id"], access_token=self.access_token
-                )
-                uploaded_model["compressed_models"] = [
-                    vars(CompressedModel(children_model)) for children_model in children_models
-                ]
-                models.append(uploaded_model)
+
+            for parent_model_info in parent_models:
+                if parent_model_info.origin_from == "custom":
+                    model = get_model_collection_object(model_info=parent_model_info)
+
+                    children_models = self.client.get_children_models(
+                        model_id=model.model_id, access_token=self.access_token
+                    )
+                    model.compressed_models = [
+                        get_compressed_model_object(children_model) for children_model in children_models
+                    ]
+
+                models.append(model)
             logger.info("Get model list successful.")
 
             return models
 
         except Exception as e:
             logger.error(f"Get model list failed. Error: {e}")
             raise e
 
     @validate_token
-    def get_uploaded_models(self) -> List[Dict[str, Any]]:
+    def get_uploaded_models(self) -> List[Model]:
         """Get the list of uploaded models.
 
         Raises:
             e: If an error occurs while getting the uploaded model list.
 
         Returns:
-            List[Dict[str, Any]]: The list of uploaded models.
+            List[Model]: The list of uploaded models.
         """
+
         try:
             logger.info("Getting uploaded model list...")
             parent_models = self.client.get_parent_models(is_simple=True, access_token=self.access_token)
             uploaded_models = [
-                vars(Model(parent_model)) for parent_model in parent_models if parent_model.origin_from == "custom"
+                get_model_object(model_info=parent_model_info)
+                for parent_model_info in parent_models
+                if parent_model_info.origin_from == "custom"
             ]
             logger.info("Get uploaded model list successful.")
 
             return uploaded_models
 
         except Exception as e:
             logger.error(f"Get uploaded model list failed. Error: {e}")
             raise e
 
     @validate_token
-    def get_compressed_models(self, model_id: str) -> List[Dict[str, Any]]:
+    def get_compressed_models(self, model_id: str) -> List[CompressedModel]:
         """Get the list of compressed models for a given model ID.
 
         Args:
             model_id (str): The ID of the model.
 
         Raises:
             e: If an error occurs while getting the compressed model list.
 
         Returns:
-            List[Dict[str, Any]]: The list of compressed models for a given model ID.
+            List[CompressedModel]: The list of compressed models for a given model ID.
         """
+
         try:
             logger.info("Getting compressed model list...")
             children_models = self.client.get_children_models(model_id=model_id, access_token=self.access_token)
-            compressed_models = [vars(CompressedModel(children_model)) for children_model in children_models]
+            compressed_models = [
+                get_compressed_model_object(model_info=children_model_info) for children_model_info in children_models
+            ]
             logger.info("Get compressed model list successful.")
 
             return compressed_models
 
         except Exception as e:
             logger.error(f"Get compressed model list failed. Error: {e}")
             raise e
@@ -225,21 +238,22 @@
         Raises:
             e: If an error occurs while getting the model.
 
         Returns:
             Union[Model, CompressedModel]: The retrieved model. If the model is compressed,
             `CompressedModel` will be returned. Otherwise, `Model` will be returned.
         """
+
         try:
             logger.info("Getting model...")
             model_info = self.client.get_model_info(model_id=model_id, access_token=self.access_token)
             if model_info.status.is_compressed:
-                model = CompressedModel(model_info)
+                model = get_compressed_model_object(model_info=model_info)
             else:
-                model = Model(model_info)
+                model = get_model_object(model_info=model_info)
             logger.info("Get model successful.")
 
             return model
 
         except Exception as e:
             logger.error(f"Get model failed. Error: {e}")
             raise e
@@ -251,14 +265,15 @@
         Args:
             model_id (str): The ID of the model.
             local_path (str): The local path to save the downloaded model.
 
         Raises:
             e: If an error occurs while downloading the model.
         """
+
         try:
             logger.info("Downloading model...")
             download_link = self.client.get_download_model_link(model_id=model_id, access_token=self.access_token)
             request.urlretrieve(download_link.url, local_path)
             logger.info(f"Download model successful. Local Path: {local_path}")
 
         except Exception as e:
@@ -272,14 +287,15 @@
         Args:
             model_id (str): The ID of the model.
             recursive (bool, optional): Whether to also delete the compressed model for that model. Defaults to False.
 
         Raises:
             e: If an error occurs while deleting the model.
         """
+
         try:
             logger.info("Deleting model...")
             children_models = self.client.get_children_models(model_id=model_id, access_token=self.access_token)
             if len(children_models) != 0:
                 if not recursive:
                     logger.warning(
                         "Deleting the model will also delete its compressed models. To proceed with the deletion, set the `recursive` parameter to True."
@@ -294,32 +310,36 @@
                 logger.info("Delete model successful.")
 
         except Exception as e:
             logger.error(f"Delete model failed. Error: {e}")
             raise e
 
     @validate_token
-    def select_compression_method(self, model_id: str, compression_method: CompressionMethod) -> CompressionBase:
+    def select_compression_method(self, model_id: str, compression_method: CompressionMethod) -> CompressionInfo:
         """Select a compression method for a model.
 
         Args:
             model_id (str): The ID of the model.
             compression_method (CompressionMethod): The selected compression method.
 
         Raises:
             e: If an error occurs while selecting the compression method.
 
         Returns:
-            CompressionBase: The compression information for the selected compression method.
+            CompressionInfo: The compression information for the selected compression method.
         """
         try:
             logger.info("Selecting compression method...")
             data = GetAvailableLayersRequest(model_id=model_id, compression_method=compression_method.value)
             response = self.client.get_available_layers(data=data, access_token=self.access_token)
-            compression_info = CompressionBase(compression_method.value, response.available_layers, model_id)
+            compression_info = CompressionInfo(
+                original_model_id=model_id,
+                compression_method=compression_method.value,
+                available_layers=response.available_layers,
+            )
             logger.info("Select compression method successful.")
 
             return compression_info
 
         except Exception as e:
             logger.error(f"Select compression method failed. Error: {e}")
             raise e
@@ -335,16 +355,22 @@
             e: If an error occurs while getting the compression information.
 
         Returns:
             CompressionInfo: The information about the compression.
         """
         try:
             logger.info("Getting compression...")
+            compression_info = self.client.get_compression_info(
+                compression_id=compression_id, access_token=self.access_token
+            )
             compression_info = CompressionInfo(
-                self.client.get_compression_info(compression_id=compression_id, access_token=self.access_token)
+                compressed_model_id=compression_info.new_model_id,
+                compression_id=compression_info.compression_id,
+                compression_method=compression_info.compression_method,
+                available_layers=compression_info.available_layers,
             )
             logger.info("Get compression successful.")
 
             return compression_info
 
         except Exception as e:
             logger.error(f"Get compression failed. Error: {e}")
@@ -388,22 +414,22 @@
 
         Returns:
             CompressedModel: The compressed model.
         """
         try:
             logger.info("Compressing model...")
             data = CreateCompressionRequest(
-                model_id=compression.model_id,
+                model_id=compression.original_model_id,
                 model_name=model_name,
                 compression_method=compression.compression_method,
             )
             compression_info = self.client.create_compression(data=data, access_token=self.access_token)
 
             if dataset_path and compression.compression_method == CompressionMethod.PR_NN.value:
-                self.__upload_dataset(model_id=compression.model_id, dataset_path=dataset_path)
+                self.__upload_dataset(model_id=compression.original_model_id, dataset_path=dataset_path)
 
             for available_layers in compression.available_layers:
                 if available_layers.values != [""]:
                     available_layers.use = True
 
             data = CompressionRequest(
                 compression_id=compression_info.compression_id,
@@ -441,33 +467,29 @@
             model_name (str): The name of the compressed model.
             compression_method (CompressionMethod): The selected compression method.
             recommendation_method (RecommendationMethod): The selected recommendation method.
             recommendation_ratio (float): The compression ratio recommended by the recommendation method.
             output_path (str): The local path to save the compressed model.
             dataset_path (str, optional): The path of the dataset used for nuclear norm compression method. Default is None.
 
-        Note:
-            - recommendation_method
-                - If you selected PR_L2, PR_GM, PR_NN for compression_method
-                    - The recommended_method available is **SLAMP**.
-                - If you selected FD_TK, FD_SVD for compression_method
-                    - The recommended_method available is **VBMF**.
-            - recommendation_ratio:
-                - SLAMP: 0 < ratio <= 1
-                - VBMF: -1 <= ratio <= 1
-
         Raises:
             e: If an error occurs while performing recommendation compression.
 
         Returns:
             CompressedModel: The compressed model.
         """
+
         try:
             logger.info("Compressing recommendation-based model...")
 
+            if compression_method in [CompressionMethod.PR_ID, CompressionMethod.FD_CP]:
+                raise Exception(
+                    f"The {compression_method.value} compression method you choose doesn't provide a recommendation."
+                )
+
             if (
                 compression_method in [CompressionMethod.PR_L2, CompressionMethod.PR_GM, CompressionMethod.PR_NN]
                 and recommendation_method != RecommendationMethod.SLAMP
             ):
                 raise Exception(
                     f"The {compression_method.value} compression method is only available the SLAMP recommendation method."
                 )
@@ -530,34 +552,32 @@
 
         Args:
             model_id (str): The ID of the model.
             model_name (str): The name of the compressed model.
             output_path (str): The local path to save the compressed model.
             compression_ratio (float): The compression ratio for automatic compression. Defaults to 0.5.
 
-        Note:
-            - compression_ratio: 0 < ratio <= 1
-
         Raises:
             e: If an error occurs while performing automatic compression.
 
         Returns:
             CompressedModel: The compressed model.
         """
+
         try:
             logger.info("Compressing automatic-based model...")
             data = AutoCompressionRequest(
                 model_id=model_id,
                 model_name=model_name,
                 recommendation_ratio=compression_ratio,
                 save_path=output_path,
             )
             model_info = self.client.auto_compression(data=data, access_token=self.access_token)
             self.download_model(model_id=model_info.model_id, local_path=output_path)
-            compressed_model = CompressedModel(model_info)
+            compressed_model = get_compressed_model_object(model_info=model_info)
             logger.info(f"Automatic compression successful. Compressed Model ID: {compressed_model.model_id}")
             logger.info("25 credits have been consumed.")
 
             return compressed_model
 
         except Exception as e:
             logger.error(f"Automatic compression failed. Error: {e}")
```

## netspresso/compressor/client/config.py

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 
 from loguru import logger
 from pydantic import BaseSettings
 
 BASE_DIR = Path(__file__).resolve().parent
 config = configparser.ConfigParser()
-DEPLOYMENT_MODE = os.getenv("DEPLOYMENT_MODE", "LOCAL")
+DEPLOYMENT_MODE = os.getenv("DEPLOYMENT_MODE", "PROD")
 logger.info(f"Read {DEPLOYMENT_MODE} config")
 config.read(f"{BASE_DIR}/configs/config-{DEPLOYMENT_MODE.lower()}.ini")
 
 
 class Config(BaseSettings):
     API_PREFIX: str = "/api/v2"
     IP: str = config["GENERAL"]["IP"]
```

## netspresso/compressor/client/schemas/compression.py

```diff
@@ -1,18 +1,17 @@
 from typing import Dict, List, Any
-from uuid import UUID
 
 from pydantic import BaseModel, Field, root_validator
 
 from .common import COMPRESSION_METHOD, RECOMMENDATION_METHOD
 from ..utils.validator import CompressionParamsValidator
 
 
 class CreateCompressionRequest(BaseModel):
-    model_id: UUID = Field(..., description="Model ID")
+    model_id: str = Field(..., description="Model ID")
     model_name: str = Field(..., description="Model Name")
     description: str = Field("", description="Description")
     compression_method: COMPRESSION_METHOD = Field(..., description="Compression Method")
 
 
 class AvailableLayerBase(BaseModel):
     name: str = Field(..., description="Layer Name")
@@ -21,23 +20,23 @@
 
 class AvailableLayer(AvailableLayerBase):
     use: bool = Field(False, description="Compression Selection Status")
     channels: List[int] = Field([], description="Channel Info")
 
 
 class CompressionResponse(BaseModel):
-    new_model_id: UUID = Field(..., description="Model ID")
-    compression_id: UUID = Field(..., description="Compression ID")
+    new_model_id: str = Field(..., description="Model ID")
+    compression_id: str = Field(..., description="Compression ID")
     compression_method: COMPRESSION_METHOD = Field(..., description="Compression Method")
     available_layers: List[AvailableLayer] = Field([], description="Compressible Layers")
 
 
 class RecommendationRequest(BaseModel):
-    model_id: UUID = Field(..., description="Model ID")
-    compression_id: UUID = Field(..., description="Compression ID")
+    model_id: str = Field(..., description="Model ID")
+    compression_id: str = Field(..., description="Compression ID")
     recommendation_method: RECOMMENDATION_METHOD = Field(..., description="Recommendation Method")
     recommendation_ratio: float = Field(..., description="Recommendation Ratio")
 
     @root_validator
     def validate_ratio(cls, values):
         method = values.get("recommendation_method")
         ratio = values.get("recommendation_ratio")
@@ -55,45 +54,45 @@
 
 
 class RecommendationResponse(BaseModel):
     recommended_layers: List[RecommendationInfo] = Field([], description="Recommended Layers")
 
 
 class CompressionRequest(BaseModel):
-    compression_id: UUID = Field(..., description="Compression ID")
+    compression_id: str = Field(..., description="Compression ID")
     compression_method: COMPRESSION_METHOD = Field(..., description="Compression Method")
     layers: List[AvailableLayer] = Field([], description="Compressible Layers")
     options: Dict[str, str] = Field({"policy": "average"}, description="Compression Options")
-    compressed_model_id: UUID = Field(..., description="Compressed Model ID")
+    compressed_model_id: str = Field(..., description="Compressed Model ID")
 
     @root_validator
     def validate_compression_params(cls, values):
         compression_method = values.get("compression_method")
         layers = values.get("layers")
 
         compression_params_validator = CompressionParamsValidator(compression_method, layers)
         compression_params_validator.validate()
 
         return values
 
 
 class AutoCompressionRequest(BaseModel):
-    model_id: UUID = Field(..., description="Model ID")
+    model_id: str = Field(..., description="Model ID")
     model_name: str = Field(..., description="Model Name")
     description: str = Field("", description="Description")
     recommendation_ratio: float = Field(..., gt=0, le=1, description="Recommendation Ratio")
     save_path: str = Field(..., description="Compressed Model Save Path")
 
 
 class UploadDatasetRequest(BaseModel):
-    model_id: UUID = Field(..., description="Model ID")
+    model_id: str = Field(..., description="Model ID")
     file_path: str = Field(..., description="Model Path")
 
 
 class GetAvailableLayersRequest(BaseModel):
-    model_id: UUID = Field(..., description="Model ID")
+    model_id: str = Field(..., description="Model ID")
     compression_method: COMPRESSION_METHOD = Field(..., description="Compression Method")
 
 
 class GetAvailableLayersReponse(BaseModel):
     compression_method: COMPRESSION_METHOD = Field(..., description="Compression Method")
     available_layers: List[AvailableLayer] = Field([], description="Compressible Layers")
```

## netspresso/compressor/client/schemas/model.py

```diff
@@ -1,10 +1,9 @@
 import json
 from typing import List, Any
-from uuid import UUID
 from os.path import basename
 
 from pydantic import BaseModel, Field, validator, root_validator, HttpUrl
 
 from netspresso.compressor.client.schemas.common import TASK, FRAMEWORK, ORIGIN_FROM
 from netspresso.compressor.client.utils.enum import Framework, Extension
 
@@ -99,15 +98,15 @@
     total_latency: float = Field(0, description="Total Latency of Model")
     performance: List = Field([], description="Metric Value")
     spec: List = Field([], description="Metric Value")
     layers: List = Field([], description="Metric Value")
 
 
 class ModelResponse(BaseModel):
-    model_id: UUID = Field(..., description="Model ID")
+    model_id: str = Field(..., description="Model ID")
     model_name: str = Field(..., description="Model Name")
     description: str = Field("", description="Description")
     original_model_id: str = Field(..., description="Original Model ID")
     original_compression_id: str = Field("", description="Compression ID")
     task: TASK = Field(..., description="Task")
     framework: FRAMEWORK = Field(..., description="Framework")
     origin_from: ORIGIN_FROM = Field(..., description="Origin From(Model Source)")
```

## netspresso/compressor/core/compression.py

```diff
@@ -1,12 +1,43 @@
-class CompressionBase:
-    def __init__(self, compression_method, available_layers, model_id):
-        self.compression_method = compression_method
-        self.available_layers = available_layers
-        self.model_id = model_id
+from typing import Any, List
+from pydantic import BaseModel, Field
 
 
-class CompressionInfo(CompressionBase):
-    def __init__(self, compression_info, model_id):
-        super().__init__(compression_info.compression_method, compression_info.available_layers, model_id)
-        self.new_model_id = compression_info.new_model_id
-        self.compression_id = compression_info.compression_id
+class AvailableLayer(BaseModel):
+    """Represents an available layer for compression.
+
+    Attributes:
+        name (str): The name of the layer.
+        values (List[Any]): The compression parameters for the layer.
+        use (bool): The compression selection status for the layer.
+        channels (List[int]): The channel information for the layer.
+    """
+
+    name: str = Field(..., description="Layer Name")
+    values: List[Any] = Field([], description="Compression Parameters")
+    use: bool = Field(False, description="Compression Selection Status")
+    channels: List[int] = Field([], description="Channel Info")
+
+
+class CompressionInfo(BaseModel):
+    """Represents compression information for a model.
+
+    Attributes:
+        compressed_model_id (str): The ID of the compressed model.
+        compression_id (str): The ID of the compression.
+        compression_method (str): The compression method used.
+        available_layers (List[AvailableLayer]): The compressible layers information.
+
+            AvailableLayer Attributes:
+                - name (str): The name of the layer.
+                - values (List[Any]): The compression parameters for the layer.
+                - use (bool): The compression selection status for the layer.
+                - channels (List[int]): The channel information for the layer.
+
+        original_model_id (str): The ID of the original model.
+    """
+
+    compressed_model_id: str = Field("", description="Compressed Model ID")
+    compression_id: str = Field("", description="Compression ID")
+    compression_method: str = Field(..., description="Compression Method")
+    available_layers: List[AvailableLayer] = Field([], description="Compressible Layers")
+    original_model_id: str = Field("", description="Original Model ID")
```

## netspresso/compressor/core/model.py

```diff
@@ -1,14 +1,72 @@
-class Model:
-    def __init__(self, model_info) -> None:
-        self.model_id = model_info.model_id
-        self.model_name = model_info.model_name
-        self.framework = model_info.framework
-        self.task = model_info.task
-        self.spec = model_info.spec
+from typing import Any, List
+from pydantic import BaseModel, Field
+
+
+class InputShape(BaseModel):
+    """Represents the shape of an input tensor.
+
+    Attributes:
+        batch (int): The batch size of the input tensor.
+        channel (int): The number of channels in the input tensor.
+        dimension (List[int]): The dimensions of the input tensor.
+    """
+
+    batch: Any = Field(None, description="Input Batch")
+    channel: int = Field(0, description="Input Channel")
+    dimension: List[int] = Field([0], description="Input Diemension ex) [height, width]")
+
+
+class Model(BaseModel):
+    """Represents a uploaded model.
+
+    Attributes:
+        model_id (str): The ID of the model.
+        model_name (str): The name of the model.
+        task (Task): The task of the model.
+        framework (Framework): The framework of the model.
+        input_shapes (List[InputShape]): The input shapes of the model.
+
+            InputShape Attributes:
+                - batch (int): The batch size of the input tensor.
+                - channel (int): The number of channels in the input tensor.
+                - dimension (List[int]): The dimensions of the input tensor.
+
+        model_size (float): The size of the model.
+        flops (float): The FLOPs (floating point operations) of the model.
+        trainable_parameters (float): The number of trainable parameters in the model.
+        non_trainable_parameters (float): The number of non-trainable parameters in the model.
+        number_of_layers (float): The number of layers in the model.
+    """
+
+    model_id: str = Field(..., description="Model ID")
+    model_name: str = Field(..., description="Model Name")
+    task: str = Field(..., description="Task")
+    framework: str = Field(..., description="Framework")
+    input_shapes: List[InputShape] = Field([], description="Input Shapes")
+    model_size: float = Field(0, description="Model Size")
+    flops: float = Field(0, description="FLOPs")
+    trainable_parameters: float = Field(0, description="Trainable Parameters")
+    non_trainable_parameters: float = Field(0, description="Non Trainable Parameters")
+    number_of_layers: int = Field(0, description="Number of Layers")
 
 
 class CompressedModel(Model):
-    def __init__(self, model_info) -> None:
-        super().__init__(model_info)
-        self.compression_id = model_info.original_compression_id
-        self.original_model_id = model_info.original_model_id
+    """Represents a compressed model.
+
+    Attributes:
+        compression_id (str): The ID of the compression.
+        original_model_id (str): The ID of the uploaded model.
+    """
+
+    compression_id: str = Field("", description="Compression ID")
+    original_model_id: str = Field(..., description="Original Model ID")
+
+
+class ModelCollection(Model):
+    """A collection of models that includes the uploaded model and its compressed models.
+
+    Attributes:
+        compressed_models (List[CompressedModel]): A list of compressed models compressed from this model.
+    """
+
+    compressed_models: List[CompressedModel] = Field([], description="Compressed Models")
```

## Comparing `netspresso-0.1.6.dist-info/LICENSE` & `netspresso-0.1.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `netspresso-0.1.6.dist-info/METADATA` & `netspresso-0.1.7.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: netspresso
-Version: 0.1.6
-Summary: python client for the NetsPresso
-Home-page: https://github.com/nota-github/netspresso-python
+Version: 0.1.7
+Summary: NetsPresso Python Package
+Home-page: https://github.com/Nota-NetsPresso/netspresso-python
 Author: NetsPresso
 Author-email: bmlee@nota.ai
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -14,13 +14,10 @@
 Requires-Dist: loguru (==0.7.0)
 Requires-Dist: urllib3 (==2.0.2)
 Requires-Dist: PyJWT (==2.7.0)
 Requires-Dist: pydantic (==1.10.4)
 Requires-Dist: requests (==2.30.0)
 Requires-Dist: email-validator (==2.0.0)
 Requires-Dist: pytz (==2023.3)
-Requires-Dist: sphinx (==6.2.1)
-Requires-Dist: sphinx-rtd-theme (==1.2.1)
-Requires-Dist: recommonmark (==0.7.1)
 Requires-Dist: typing-extensions (==4.5.0)
 
-# NetsPresso
+# NetsPresso Python Package
```

## Comparing `netspresso-0.1.6.dist-info/RECORD` & `netspresso-0.1.7.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,24 @@
-netspresso/__init__.py,sha256=js_m8PQ2W0sqE2u8EbnwOj4Lf2mj4pZf8gFa9fJIYQQ,23
-netspresso/compressor/__init__.py,sha256=tgGJSYtJ-65BuhiWd2WoXd3ouPC0U0ZrP7QNWBVZNPQ,23052
+netspresso/__init__.py,sha256=GhTYFGQ77wbJM35lScp2XZKYnkNHTrdYozPoCZiCVSM,23
+netspresso/compressor/__init__.py,sha256=8nccEoi_l_5HaBse4tqOnHqGtdsRq52FqjlMET2VGeY,23322
 netspresso/compressor/client/__init__.py,sha256=pgYngRDyZBTc3vTDNeZPHpSc86KJ_122J-jdKFArpT0,8456
-netspresso/compressor/client/config.py,sha256=i3EZTWDZJEq527YY1hiyiSN-DIVQyjE7zgOI7_kLY9Y,536
+netspresso/compressor/client/config.py,sha256=CjYFS5hAQ7ZjUTE0utCKNOboT7LV1FiGKk_FcsrjPXY,535
 netspresso/compressor/client/schemas/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 netspresso/compressor/client/schemas/auth.py,sha256=NGudVfx4Q7E8XppeDgcKmQlU_3UwKDu3YjYiIwsii1g,2644
 netspresso/compressor/client/schemas/common.py,sha256=w1rR-jqIvjQ6UqMRZ5KYWW8bQrlXMSrAdWXCzA3tQuk,482
-netspresso/compressor/client/schemas/compression.py,sha256=TT3ycahw4zRKgGot6Fk0y1GcgHkJuNPE1UhSJGpDhVw,4141
-netspresso/compressor/client/schemas/model.py,sha256=hsH7v2qxBbaaWJeZNomWxLzEvM-lFxcm4BstR6sdHFM,5705
+netspresso/compressor/client/schemas/compression.py,sha256=0OwRemHeFQy4wZBWHzwcYuf0T2w8fN7Hb39fHWyPM0k,4108
+netspresso/compressor/client/schemas/model.py,sha256=hprc5AQ3gFe8hjtoHEcyKM8HoQCYn53LJwQJ_QsBUHA,5681
 netspresso/compressor/client/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 netspresso/compressor/client/utils/common.py,sha256=gAHVbvzBGmoYNExaGOEgaqJHTszXuMOSwCFpyH_xEwc,481
 netspresso/compressor/client/utils/enum.py,sha256=RUtiknaDJhfML23sILSHnEvPJ2wBqsLDgId0d_IM0fI,840
 netspresso/compressor/client/utils/validator.py,sha256=0pONKSTlxTWcpSIiUw3P2ItPARoLXvu5YSGGxhUFPNU,3814
 netspresso/compressor/core/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-netspresso/compressor/core/compression.py,sha256=XzLukrfHTYEJQPF0A01iYbVZEjKRfgweIMEmGsfpfXc,563
-netspresso/compressor/core/model.py,sha256=bDK_y5dtUxS3_uFEMhSbmv851hglfsA9w5YSLf9RhZE,521
+netspresso/compressor/core/compression.py,sha256=OMrI-SsDXmwzZdz_1jRmv30KTGRRluRszJPqcXFQOwU,1900
+netspresso/compressor/core/model.py,sha256=kH0VBvcpwyxO9QsUpaQZXLB-IZXfw3T-mp613qX3_mE,2966
 netspresso/compressor/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+netspresso/compressor/utils/model.py,sha256=tPojNWMvvHTNT8EgLIJfq_3EWIOIb0HuZHDbF1ANBc0,2035
 netspresso/compressor/utils/token.py,sha256=zWKx6olb8N2c3nSQhUS22IRG7ILQZYIERScETEFeUXY,236
-netspresso-0.1.6.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
-netspresso-0.1.6.dist-info/METADATA,sha256=qOQQZ5W_bA4aJ5CxsZt_abV28bTripTNTC1BId0b74A,872
-netspresso-0.1.6.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-netspresso-0.1.6.dist-info/top_level.txt,sha256=aHBNCm2tepEeTCUHu2_PVIlFG6iGuQReNl0js5hzjdU,11
-netspresso-0.1.6.dist-info/RECORD,,
+netspresso-0.1.7.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
+netspresso-0.1.7.dist-info/METADATA,sha256=YolgYlVXqKP1Kfn2X28c64qgUTpTKbNzhhAeQN1VYGc,769
+netspresso-0.1.7.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+netspresso-0.1.7.dist-info/top_level.txt,sha256=aHBNCm2tepEeTCUHu2_PVIlFG6iGuQReNl0js5hzjdU,11
+netspresso-0.1.7.dist-info/RECORD,,
```

