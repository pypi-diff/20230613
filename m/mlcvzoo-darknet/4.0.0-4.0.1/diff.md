# Comparing `tmp/mlcvzoo_darknet-4.0.0.tar.gz` & `tmp/mlcvzoo_darknet-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlcvzoo_darknet-4.0.0.tar", max compression
+gzip compressed data, was "mlcvzoo_darknet-4.0.1.tar", max compression
```

## Comparing `mlcvzoo_darknet-4.0.0.tar` & `mlcvzoo_darknet-4.0.1.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0      401 2023-02-14 09:49:28.024275 mlcvzoo_darknet-4.0.0/README.md
--rw-r--r--   0        0        0      177 2023-02-14 16:06:15.782863 mlcvzoo_darknet-4.0.0/mlcvzoo_darknet/__init__.py
--rw-r--r--   0        0        0     2906 2023-02-14 16:06:15.782863 mlcvzoo_darknet-4.0.0/mlcvzoo_darknet/configuration.py
--rw-r--r--   0        0        0     1330 2023-02-14 09:49:28.024275 mlcvzoo_darknet-4.0.0/mlcvzoo_darknet/darknetdatafile.py
--rw-r--r--   0        0        0    13716 2023-02-14 16:06:15.782863 mlcvzoo_darknet-4.0.0/mlcvzoo_darknet/model.py
--rw-r--r--   0        0        0      154 2023-02-14 09:49:28.024275 mlcvzoo_darknet-4.0.0/mlcvzoo_darknet/py.typed
--rw-r--r--   0        0        0     3635 2023-02-14 16:06:15.782863 mlcvzoo_darknet-4.0.0/pyproject.toml
--rw-r--r--   0        0        0     1351 1970-01-01 00:00:00.000000 mlcvzoo_darknet-4.0.0/setup.py
--rw-r--r--   0        0        0     1812 1970-01-01 00:00:00.000000 mlcvzoo_darknet-4.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11412 2023-06-13 11:43:52.159896 mlcvzoo_darknet-4.0.1/LICENSE
+-rw-r--r--   0        0        0      401 2023-06-13 11:43:52.159896 mlcvzoo_darknet-4.0.1/README.md
+-rw-r--r--   0        0        0      244 2023-06-13 11:43:52.159896 mlcvzoo_darknet-4.0.1/mlcvzoo_darknet/__init__.py
+-rw-r--r--   0        0        0     2948 2023-06-13 11:43:52.159896 mlcvzoo_darknet-4.0.1/mlcvzoo_darknet/configuration.py
+-rw-r--r--   0        0        0     1372 2023-06-13 11:43:52.159896 mlcvzoo_darknet-4.0.1/mlcvzoo_darknet/darknetdatafile.py
+-rw-r--r--   0        0        0    13799 2023-06-13 11:43:52.159896 mlcvzoo_darknet-4.0.1/mlcvzoo_darknet/model.py
+-rw-r--r--   0        0        0        0 2023-06-13 11:43:52.159896 mlcvzoo_darknet-4.0.1/mlcvzoo_darknet/py.typed
+-rw-r--r--   0        0        0     3707 2023-06-13 11:43:52.159896 mlcvzoo_darknet-4.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1336 1970-01-01 00:00:00.000000 mlcvzoo_darknet-4.0.1/setup.py
+-rw-r--r--   0        0        0     1801 1970-01-01 00:00:00.000000 mlcvzoo_darknet-4.0.1/PKG-INFO
```

### Comparing `mlcvzoo_darknet-4.0.0/mlcvzoo_darknet/configuration.py` & `mlcvzoo_darknet-4.0.1/mlcvzoo_darknet/configuration.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright 2021 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """
 Definition of the DarknetConfig that is used to configure the DarknetDetectionModel.
 """
 
 from typing import Optional
```

### Comparing `mlcvzoo_darknet-4.0.0/mlcvzoo_darknet/darknetdatafile.py` & `mlcvzoo_darknet-4.0.1/mlcvzoo_darknet/darknetdatafile.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright 2021 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """
 Module for handling the writing of a darknet data file,
 which defines the main information that is needed for training
 a model in the darknet framework.
 """
```

### Comparing `mlcvzoo_darknet-4.0.0/mlcvzoo_darknet/model.py` & `mlcvzoo_darknet-4.0.1/mlcvzoo_darknet/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright 2021 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """
 Module for defining the DarknetDetectionModel. It is a ObjectDetectionModel
 which can be trained on custom data.
 """
 
 import importlib.util
@@ -129,19 +130,22 @@
     def get_training_output_dir(self) -> str:
         return self.configuration.train_config.work_dir
 
     def store(self, checkpoint_path: str) -> None:
         logger.warning("The store method is currently not implemented")
 
     def restore(self, checkpoint_path: str) -> None:
-
         if self.darknet_module is None:
             raise ValueError("Model is not initialized for ...")
 
-        (self.net, _, _,) = self.darknet_module.load_network(
+        (
+            self.net,
+            _,
+            _,
+        ) = self.darknet_module.load_network(
             self.configuration.inference_config.config_path,
             self.configuration.inference_config.data_path,
             checkpoint_path,
         )
 
     def _init_inference_model(self) -> None:
         df = DarknetDataFile(**self.configuration.inference_config.data_file.to_dict())
@@ -159,15 +163,14 @@
 
         if self.configuration.inference_config.checkpoint_path != "":
             self.restore(
                 checkpoint_path=self.configuration.inference_config.checkpoint_path
             )
 
     def _init_training_model(self) -> None:
-
         self.annotation_handler = AnnotationHandler(
             configuration=self.configuration.train_config.train_annotation_handler_config
         )
 
     def _numpy_to_darknet_image(self, img: ImageType) -> Tuple[ImageType, Any]:
         """
         NOTE: the output image "dk_image" is of type "self.darknet_module.IMAGE".
@@ -200,15 +203,14 @@
     def _write_darknet_config(
         self,
         train_work_dir: str,
         train_txt_path: str,
         test_txt_path: str,
         model_specifier: str,
     ) -> Tuple[str, str]:
-
         cfg_in_path = self.configuration.train_config.config_path
 
         data_path = os.path.join(train_work_dir, f"{model_specifier}.data")
         cfg_out_path = os.path.join(train_work_dir, f"{model_specifier}.cfg")
 
         # TODO: differentiate between valid and eval paths
         df = DarknetDataFile(
@@ -227,15 +229,14 @@
             cfg_out_path,
         )
         shutil.copy(cfg_in_path, cfg_out_path)
 
         return data_path, cfg_out_path
 
     def train(self) -> None:
-
         train_annotation_handler_config = (
             self.configuration.train_config.train_annotation_handler_config
         )
 
         if (
             train_annotation_handler_config is None
             or train_annotation_handler_config.write_output is None
@@ -314,15 +315,14 @@
 
                 if line == "" and darknet_process.poll() is not None:
                     break
 
     def predict(
         self, data_item: Union[ImageType, str]
     ) -> Tuple[Union[ImageType, str], List[BoundingBox]]:
-
         """
         Predicts objects in given data_item
         Args:
             data_item: N-dimensional array or string containing the image path
 
         Returns:
             Data_item which served as input
```

### Comparing `mlcvzoo_darknet-4.0.0/pyproject.toml` & `mlcvzoo_darknet-4.0.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "mlcvzoo_darknet"
-version = "4.0.0"
-license = "Open Logistics License Version 1.0"
 description = "MLCVZoo Darknet Package"
+version = "4.0.1"
+license = "Open Logistics Foundation License v1.3"
 readme = "README.md"
 homepage = "https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo"
 repository = "https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo"
 documentation = "https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo/-/blob/main/documentation/index.adoc"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
@@ -35,27 +35,28 @@
 yaml-config-builder = { version = "^8" }
 related-mltoolbox = { version = "^1.0" }
 mlcvzoo_base = { version = "^5.0" }
 attrs = { version = ">=20" }
 
 # 1.19.2 is oldest available on aarch64 but 1.19.5 leads to unbuildable pytorch there, all is well on amd64
 numpy = { version = ">=1.19.2,!=1.19.5" }
-nptyping = { version = "^2.0" }
-opencv-python = { version = "^4.5,!=4.5.5.64" }
-opencv-contrib-python = { version = "^4.5,!=4.5.5.64" }
+nptyping = { version = ">=2.0" }
+opencv-python = { version = ">=4.5,!=4.5.5.64"}
+opencv-contrib-python = { version = ">=4.5,!=4.5.5.64" }
 
 [tool.poetry.dev-dependencies]
-mock = { version = "^4.0" }
-pytest = { version = "^7.0" }
-pytest-cov = { version = "^3.0.0" }
-black = { version = "^22" }
+mock = { version = ">=4.0" }
+pytest = { version = ">=7.0" }
+pytest-cov = { version = ">=3.0.0" }
+black = { version = ">=22" }
 mypy = { version = ">=0.961" }
-pylint = { version = "^2.9.6" }
-isort = { version = "^5.9" }
-pytest-mock = "^3.7"
+pylint = { version = ">=2.9.6" }
+# Isort guarantees formatting results for 5.X
+isort = { version = "^5.0" }
+pytest-mock = { version = ">=3.7" }
 
 [build-system]
 # NOTE: Don't remove setuptools, therefore require it from the build system
 requires = ["setuptools", "poetry_core>=1.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
```

### Comparing `mlcvzoo_darknet-4.0.0/setup.py` & `mlcvzoo_darknet-4.0.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['attrs>=20',
  'mlcvzoo_base>=5.0,<6.0',
- 'nptyping>=2.0,<3.0',
+ 'nptyping>=2.0',
  'numpy>=1.19.2,!=1.19.5',
- 'opencv-contrib-python>=4.5,<5.0,!=4.5.5.64',
- 'opencv-python>=4.5,<5.0,!=4.5.5.64',
+ 'opencv-contrib-python>=4.5,!=4.5.5.64',
+ 'opencv-python>=4.5,!=4.5.5.64',
  'related-mltoolbox>=1.0,<2.0',
  'yaml-config-builder>=8,<9']
 
 setup_kwargs = {
     'name': 'mlcvzoo-darknet',
-    'version': '4.0.0',
+    'version': '4.0.1',
     'description': 'MLCVZoo Darknet Package',
     'long_description': '# MLCVZoo Darknet\n\nThe MLCVZoo is an SDK for simplifying the usage of various (machine learning driven)\ncomputer vision algorithms. The package **mlcvzoo_darknet** is the wrapper module for the\n[darknet framework](https://github.com/AlexeyAB/darknet).\n\nFurther information about the MLCVZoo can be found [here](../README.md).\n\n## Install\n`\npip install mlcvzoo-darknet\n`\n\n## Technology stack\n\n- Python\n',
     'author': 'Maximilian Otten',
     'author_email': 'maximilian.otten@iml.fraunhofer.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo',
```

### Comparing `mlcvzoo_darknet-4.0.0/PKG-INFO` & `mlcvzoo_darknet-4.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: mlcvzoo-darknet
-Version: 4.0.0
+Version: 4.0.1
 Summary: MLCVZoo Darknet Package
 Home-page: https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo
-License: Open Logistics License Version 1.0
+License: Open Logistics Foundation License v1.3
 Author: Maximilian Otten
 Author-email: maximilian.otten@iml.fraunhofer.de
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: Other/Proprietary License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: attrs (>=20)
 Requires-Dist: mlcvzoo_base (>=5.0,<6.0)
-Requires-Dist: nptyping (>=2.0,<3.0)
+Requires-Dist: nptyping (>=2.0)
 Requires-Dist: numpy (>=1.19.2,!=1.19.5)
-Requires-Dist: opencv-contrib-python (>=4.5,<5.0,!=4.5.5.64)
-Requires-Dist: opencv-python (>=4.5,<5.0,!=4.5.5.64)
+Requires-Dist: opencv-contrib-python (>=4.5,!=4.5.5.64)
+Requires-Dist: opencv-python (>=4.5,!=4.5.5.64)
 Requires-Dist: related-mltoolbox (>=1.0,<2.0)
 Requires-Dist: yaml-config-builder (>=8,<9)
 Project-URL: Documentation, https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo/-/blob/main/documentation/index.adoc
 Project-URL: Repository, https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo
 Description-Content-Type: text/markdown
 
 # MLCVZoo Darknet
```

