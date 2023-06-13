# Comparing `tmp/mlcvzoo_util-0.3.0.tar.gz` & `tmp/mlcvzoo_util-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlcvzoo_util-0.3.0.tar", max compression
+gzip compressed data, was "mlcvzoo_util-0.3.1.tar", max compression
```

## Comparing `mlcvzoo_util-0.3.0.tar` & `mlcvzoo_util-0.3.1.tar`

### file list

```diff
@@ -1,33 +1,34 @@
--rw-r--r--   0        0        0      411 2023-02-14 09:35:53.978926 mlcvzoo_util-0.3.0/README.md
--rw-r--r--   0        0        0      177 2023-02-15 07:23:22.367520 mlcvzoo_util-0.3.0/mlcvzoo_util/__init__.py
--rw-r--r--   0        0        0      154 2023-02-14 09:35:53.978926 mlcvzoo_util-0.3.0/mlcvzoo_util/cvat_annotation_handler/__init__.py
--rw-r--r--   0        0        0     7306 2023-02-14 09:35:53.978926 mlcvzoo_util-0.3.0/mlcvzoo_util/cvat_annotation_handler/configuration.py
--rw-r--r--   0        0        0     6068 2023-02-14 09:35:53.978926 mlcvzoo_util-0.3.0/mlcvzoo_util/cvat_annotation_handler/cvat_annotation_handler.py
--rw-r--r--   0        0        0     8356 2023-02-14 09:35:53.978926 mlcvzoo_util-0.3.0/mlcvzoo_util/cvat_annotation_handler/cvat_dumper.py
--rw-r--r--   0        0        0     9792 2023-02-14 09:35:53.978926 mlcvzoo_util-0.3.0/mlcvzoo_util/cvat_annotation_handler/cvat_uploader.py
--rw-r--r--   0        0        0     1081 2023-02-14 09:35:53.978926 mlcvzoo_util-0.3.0/mlcvzoo_util/cvat_annotation_handler/utils.py
--rw-r--r--   0        0        0    12903 2023-02-14 09:35:53.978926 mlcvzoo_util-0.3.0/mlcvzoo_util/image_io_utils.py
--rw-r--r--   0        0        0      204 2023-02-14 09:35:53.978926 mlcvzoo_util-0.3.0/mlcvzoo_util/logger/__init__.py
--rw-r--r--   0        0        0     3881 2023-02-15 07:23:22.367520 mlcvzoo_util-0.3.0/mlcvzoo_util/logger/logger.py
--rw-r--r--   0        0        0     4178 2023-02-15 07:23:22.367520 mlcvzoo_util-0.3.0/mlcvzoo_util/mlcvzoo_cli_tool.py
--rw-r--r--   0        0        0      154 2023-02-14 09:35:53.978926 mlcvzoo_util-0.3.0/mlcvzoo_util/model_evaluator/__init__.py
--rw-r--r--   0        0        0     2990 2023-02-15 07:23:22.367520 mlcvzoo_util-0.3.0/mlcvzoo_util/model_evaluator/configuration.py
--rw-r--r--   0        0        0     8515 2023-02-15 07:23:22.367520 mlcvzoo_util-0.3.0/mlcvzoo_util/model_evaluator/metric_factory.py
--rw-r--r--   0        0        0    16818 2023-02-15 07:23:22.367520 mlcvzoo_util-0.3.0/mlcvzoo_util/model_evaluator/model_evaluator.py
--rw-r--r--   0        0        0      573 2023-02-14 09:35:53.978926 mlcvzoo_util-0.3.0/mlcvzoo_util/model_evaluator/structs.py
--rw-r--r--   0        0        0      154 2023-02-14 09:35:53.978926 mlcvzoo_util-0.3.0/mlcvzoo_util/model_timer/__init__.py
--rw-r--r--   0        0        0     1143 2023-02-14 09:35:53.978926 mlcvzoo_util-0.3.0/mlcvzoo_util/model_timer/configuration.py
--rw-r--r--   0        0        0     9658 2023-02-15 07:23:22.367520 mlcvzoo_util-0.3.0/mlcvzoo_util/model_timer/model_timer.py
--rw-r--r--   0        0        0      154 2023-02-14 09:35:53.978926 mlcvzoo_util-0.3.0/mlcvzoo_util/model_trainer/__init__.py
--rw-r--r--   0        0        0      699 2023-02-15 07:23:22.367520 mlcvzoo_util-0.3.0/mlcvzoo_util/model_trainer/configuration.py
--rw-r--r--   0        0        0     6586 2023-02-15 07:23:22.367520 mlcvzoo_util-0.3.0/mlcvzoo_util/model_trainer/model_trainer.py
--rw-r--r--   0        0        0      154 2023-02-14 09:35:53.978926 mlcvzoo_util-0.3.0/mlcvzoo_util/pre_annotation_tool/__init__.py
--rw-r--r--   0        0        0     1338 2023-02-14 09:35:53.982926 mlcvzoo_util-0.3.0/mlcvzoo_util/pre_annotation_tool/configuration.py
--rw-r--r--   0        0        0    12598 2023-02-15 07:23:22.367520 mlcvzoo_util-0.3.0/mlcvzoo_util/pre_annotation_tool/pre_annotation_tool.py
--rw-r--r--   0        0        0      154 2023-02-14 09:35:53.982926 mlcvzoo_util-0.3.0/mlcvzoo_util/py.typed
--rw-r--r--   0        0        0      154 2023-02-14 09:35:53.982926 mlcvzoo_util-0.3.0/mlcvzoo_util/video_image_creator/__init__.py
--rw-r--r--   0        0        0     1231 2023-02-14 09:35:53.982926 mlcvzoo_util-0.3.0/mlcvzoo_util/video_image_creator/configuration.py
--rw-r--r--   0        0        0    14405 2023-02-15 07:23:22.367520 mlcvzoo_util-0.3.0/mlcvzoo_util/video_image_creator/video_image_creator.py
--rw-r--r--   0        0        0     4031 2023-02-15 07:23:22.367520 mlcvzoo_util-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2443 1970-01-01 00:00:00.000000 mlcvzoo_util-0.3.0/setup.py
--rw-r--r--   0        0        0     1898 1970-01-01 00:00:00.000000 mlcvzoo_util-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11412 2023-06-13 11:38:09.059835 mlcvzoo_util-0.3.1/LICENSE
+-rw-r--r--   0        0        0      411 2023-06-13 11:38:09.059835 mlcvzoo_util-0.3.1/README.md
+-rw-r--r--   0        0        0      244 2023-06-13 11:38:09.059835 mlcvzoo_util-0.3.1/mlcvzoo_util/__init__.py
+-rw-r--r--   0        0        0      196 2023-06-13 11:38:09.059835 mlcvzoo_util-0.3.1/mlcvzoo_util/cvat_annotation_handler/__init__.py
+-rw-r--r--   0        0        0     7348 2023-06-13 11:38:09.059835 mlcvzoo_util-0.3.1/mlcvzoo_util/cvat_annotation_handler/configuration.py
+-rw-r--r--   0        0        0     6110 2023-06-13 11:38:09.059835 mlcvzoo_util-0.3.1/mlcvzoo_util/cvat_annotation_handler/cvat_annotation_handler.py
+-rw-r--r--   0        0        0     8392 2023-06-13 11:38:09.059835 mlcvzoo_util-0.3.1/mlcvzoo_util/cvat_annotation_handler/cvat_dumper.py
+-rw-r--r--   0        0        0     9831 2023-06-13 11:38:09.059835 mlcvzoo_util-0.3.1/mlcvzoo_util/cvat_annotation_handler/cvat_uploader.py
+-rw-r--r--   0        0        0     1123 2023-06-13 11:38:09.059835 mlcvzoo_util-0.3.1/mlcvzoo_util/cvat_annotation_handler/utils.py
+-rw-r--r--   0        0        0    12943 2023-06-13 11:38:09.059835 mlcvzoo_util-0.3.1/mlcvzoo_util/image_io_utils.py
+-rw-r--r--   0        0        0      246 2023-06-13 11:38:09.059835 mlcvzoo_util-0.3.1/mlcvzoo_util/logger/__init__.py
+-rw-r--r--   0        0        0     3923 2023-06-13 11:38:09.059835 mlcvzoo_util-0.3.1/mlcvzoo_util/logger/logger.py
+-rw-r--r--   0        0        0     4220 2023-06-13 11:38:09.059835 mlcvzoo_util-0.3.1/mlcvzoo_util/mlcvzoo_cli_tool.py
+-rw-r--r--   0        0        0      196 2023-06-13 11:38:09.063835 mlcvzoo_util-0.3.1/mlcvzoo_util/model_evaluator/__init__.py
+-rw-r--r--   0        0        0     3032 2023-06-13 11:38:09.063835 mlcvzoo_util-0.3.1/mlcvzoo_util/model_evaluator/configuration.py
+-rw-r--r--   0        0        0     8556 2023-06-13 11:38:09.063835 mlcvzoo_util-0.3.1/mlcvzoo_util/model_evaluator/metric_factory.py
+-rw-r--r--   0        0        0    16860 2023-06-13 11:38:09.063835 mlcvzoo_util-0.3.1/mlcvzoo_util/model_evaluator/model_evaluator.py
+-rw-r--r--   0        0        0      615 2023-06-13 11:38:09.063835 mlcvzoo_util-0.3.1/mlcvzoo_util/model_evaluator/structs.py
+-rw-r--r--   0        0        0      196 2023-06-13 11:38:09.063835 mlcvzoo_util-0.3.1/mlcvzoo_util/model_timer/__init__.py
+-rw-r--r--   0        0        0     1185 2023-06-13 11:38:09.063835 mlcvzoo_util-0.3.1/mlcvzoo_util/model_timer/configuration.py
+-rw-r--r--   0        0        0     9776 2023-06-13 11:38:09.063835 mlcvzoo_util-0.3.1/mlcvzoo_util/model_timer/model_timer.py
+-rw-r--r--   0        0        0      196 2023-06-13 11:38:09.063835 mlcvzoo_util-0.3.1/mlcvzoo_util/model_trainer/__init__.py
+-rw-r--r--   0        0        0      741 2023-06-13 11:38:09.063835 mlcvzoo_util-0.3.1/mlcvzoo_util/model_trainer/configuration.py
+-rw-r--r--   0        0        0     6628 2023-06-13 11:38:09.063835 mlcvzoo_util-0.3.1/mlcvzoo_util/model_trainer/model_trainer.py
+-rw-r--r--   0        0        0      196 2023-06-13 11:38:09.063835 mlcvzoo_util-0.3.1/mlcvzoo_util/pre_annotation_tool/__init__.py
+-rw-r--r--   0        0        0     1380 2023-06-13 11:38:09.063835 mlcvzoo_util-0.3.1/mlcvzoo_util/pre_annotation_tool/configuration.py
+-rw-r--r--   0        0        0    12686 2023-06-13 11:38:09.063835 mlcvzoo_util-0.3.1/mlcvzoo_util/pre_annotation_tool/pre_annotation_tool.py
+-rw-r--r--   0        0        0        0 2023-06-13 11:38:09.063835 mlcvzoo_util-0.3.1/mlcvzoo_util/py.typed
+-rw-r--r--   0        0        0      196 2023-06-13 11:38:09.063835 mlcvzoo_util-0.3.1/mlcvzoo_util/video_image_creator/__init__.py
+-rw-r--r--   0        0        0     1273 2023-06-13 11:38:09.063835 mlcvzoo_util-0.3.1/mlcvzoo_util/video_image_creator/configuration.py
+-rw-r--r--   0        0        0    14447 2023-06-13 11:38:09.063835 mlcvzoo_util-0.3.1/mlcvzoo_util/video_image_creator/video_image_creator.py
+-rw-r--r--   0        0        0     4230 2023-06-13 11:38:09.063835 mlcvzoo_util-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2416 1970-01-01 00:00:00.000000 mlcvzoo_util-0.3.1/setup.py
+-rw-r--r--   0        0        0     1875 1970-01-01 00:00:00.000000 mlcvzoo_util-0.3.1/PKG-INFO
```

### Comparing `mlcvzoo_util-0.3.0/mlcvzoo_util/cvat_annotation_handler/configuration.py` & `mlcvzoo_util-0.3.1/mlcvzoo_util/cvat_annotation_handler/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright 2022 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """
 Module for defining all configuration classes that
 are used in the context of the CVATAnnotationHandler
 """
 
 import logging
```

### Comparing `mlcvzoo_util-0.3.0/mlcvzoo_util/cvat_annotation_handler/cvat_annotation_handler.py` & `mlcvzoo_util-0.3.1/mlcvzoo_util/cvat_annotation_handler/cvat_annotation_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright 2022 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """
 Central module for handling the download and upload
 of zip files to CVAT via their commandline interface
 """
 
 import argparse
```

### Comparing `mlcvzoo_util-0.3.0/mlcvzoo_util/cvat_annotation_handler/cvat_dumper.py` & `mlcvzoo_util-0.3.1/mlcvzoo_util/cvat_annotation_handler/cvat_dumper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright 2022 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """Module for handling the download of zip files to CVAT via their commandline interface"""
 
 import logging
 import os
 import shutil
 
@@ -138,15 +139,14 @@
         )
 
         if return_code != 0:
             raise IOError(f"CVAT download did not succeed, return-code={return_code}")
 
     @staticmethod
     def __create_target_zip_path(dump_task_config: CVATTaskDumpConfig) -> str:
-
         if dump_task_config.target_zip_path == "":
             target_zip_path: str = os.path.join("tmp", "tmp-task.zip")
             logger.debug(
                 "dump_task_config.target_zip_path is not set, therefore the default '%s' "
                 "will be used to store the downloaded task:",
                 target_zip_path,
             )
@@ -155,30 +155,28 @@
 
         return target_zip_path
 
     @staticmethod
     def __create_zip_extract_dir_path(
         target_zip_path: str, zip_extract_dir: str
     ) -> str:
-
         if not os.path.isdir(zip_extract_dir):
             zip_extract_dir = target_zip_path.replace(".zip", "")
             logger.debug(
                 "dump_task_config.target_zip_path is not set, therefore the default '%s' "
                 "will be used to store the downloaded task:",
                 zip_extract_dir,
             )
 
         return zip_extract_dir
 
     @staticmethod
     def __pre_clean_up_and_determine_skip(
         overwrite_existing_zip: bool, target_zip_path: str
     ) -> bool:
-
         if os.path.isfile(target_zip_path):
             if overwrite_existing_zip:
                 logger.info("Clean up old dump data, remove '%s'", target_zip_path)
                 os.remove(target_zip_path)
             else:
                 logger.info(
                     "Skip download since zip-file '%s' exists and should not be overwritten",
@@ -200,29 +198,27 @@
             )
             shutil.rmtree(zip_extract_dir)
 
     @staticmethod
     def __create_cvat_dump_cli_command(
         base_command: str, target_zip_path: str, task_info: CVATTaskInfoConfig
     ) -> str:
-
         return (
             f"{base_command} dump "
             f"{task_info.task_ID} "
             f"{target_zip_path} "
             f"--format '{task_info.annotation_format}'"
         )
 
     @staticmethod
     def __extract_and_copy_annotations_to_data_dir(
         target_zip_path: str,
         zip_extract_dir: str,
         dataset_dir: str,
     ) -> None:
-
         if not os.path.isdir(dataset_dir):
             logger.warning(
                 "Path to dataset_dir='%s' does not exist! "
                 "Skip the extraction and move of annotation data.",
                 dataset_dir,
             )
             return
@@ -232,15 +228,14 @@
         zip_annotation_dir = os.path.join(zip_extract_dir, "Annotations")
 
         annotation_file_paths = get_file_list(
             input_dir=zip_extract_dir, search_subfolders=True, file_extension=".xml"
         )
 
         for annotation_path in annotation_file_paths:
-
             dataset_annotation_path = annotation_path.replace(
                 zip_annotation_dir, dataset_dir
             )
 
             ensure_dir(file_path=dataset_annotation_path, verbose=True)
 
             logger.debug(
```

### Comparing `mlcvzoo_util-0.3.0/mlcvzoo_util/cvat_annotation_handler/cvat_uploader.py` & `mlcvzoo_util-0.3.1/mlcvzoo_util/cvat_annotation_handler/cvat_uploader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright 2022 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """Module for handling the upload of zip files to CVAT via their commandline interface"""
 
 import logging
 import os
 import zipfile
 from typing import Dict
@@ -129,15 +130,14 @@
         if return_code != 0:
             raise ValueError(f"Upload did not succeed, return-code={return_code}")
 
     @staticmethod
     def __create_cvat_upload_cli_command(
         base_command: str, target_zip_path: str, task_info: CVATTaskInfoConfig
     ) -> str:
-
         return (
             f"{base_command} upload "
             f"{task_info.task_ID} "
             f"{target_zip_path} "
             f"--format '{task_info.annotation_format}'"
         )
 
@@ -174,15 +174,14 @@
             prediction_data_dir=upload_task_config.prediction_data_dir,
         )
 
     @staticmethod
     def __write_prediction_data_to_zip(
         source_zip_path: str, target_zip_path: str, prediction_data_dir: str
     ) -> str:
-
         if not os.path.isdir(prediction_data_dir):
             raise ValueError(
                 f"prediction_data_dir='{prediction_data_dir}' does not exist! "
                 "Please specify a directory in order to generate"
                 "a prediction zip file for the upload to CVAT!"
             )
 
@@ -240,15 +239,14 @@
         )
 
         # Write annotation data to zip-file
         for annotation_xml_path in annotation_xml_files:
             annotation_file_name = os.path.basename(annotation_xml_path)
 
             if annotation_file_name in predicted_xml_paths_map:
-
                 logger.debug(
                     "Add xml file to upload zip-file: '%s'",
                     predicted_xml_paths_map[annotation_file_name],
                 )
                 with open(
                     file=predicted_xml_paths_map[annotation_file_name], encoding="utf8"
                 ) as prediction_file:
```

### Comparing `mlcvzoo_util-0.3.0/mlcvzoo_util/cvat_annotation_handler/utils.py` & `mlcvzoo_util-0.3.1/mlcvzoo_util/cvat_annotation_handler/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright 2022 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """Module for storing utility functions that are needed for the cvat_annotation_handler package"""
 
 import logging
 import os
 import shlex
 import subprocess
```

### Comparing `mlcvzoo_util-0.3.0/mlcvzoo_util/image_io_utils.py` & `mlcvzoo_util-0.3.1/mlcvzoo_util/image_io_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright 2021 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """Module for different utility operations regarding image (picture) objects"""
 
 from __future__ import annotations
 
 import copy
 import logging
@@ -120,15 +121,14 @@
             img_info: String, any information that should be printed on the image
 
         Returns: None
 
         """
 
         if self.mode != VideoLiveOutput.MODE_TERMINATE:
-
             self.end = time.time() - self.start
 
             # will only be executed once
             if not self.resized_window:
                 scale_factor = frame.shape[1] / frame.shape[0]
 
                 if self.resize_window is True:
@@ -211,15 +211,14 @@
         return self.mode == VideoLiveOutput.MODE_TERMINATE
 
 
 class VideoFileInput:
     """Class for handling a video and navigating through its frames"""
 
     def __init__(self, path: str):
-
         logger.debug("Init VideoFileInput for video '%s'", path)
 
         self.cap = cv2.VideoCapture(path)
 
         self.current_frame: Optional[np.ndarray] = None  # type: ignore[type-arg]
 
     def goto_frame(self, num: int) -> None:
```

### Comparing `mlcvzoo_util-0.3.0/mlcvzoo_util/logger/logger.py` & `mlcvzoo_util-0.3.1/mlcvzoo_util/logger/logger.py`

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
 
 """Module for handling python logging"""
 
 import logging
 import os
 import re
 import sys
```

### Comparing `mlcvzoo_util-0.3.0/mlcvzoo_util/mlcvzoo_cli_tool.py` & `mlcvzoo_util-0.3.1/mlcvzoo_util/mlcvzoo_cli_tool.py`

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
 Module for the definition of a super class for any mlcvzoo module that is
 providing a commandline interface.
 """
 
 import argparse
```

### Comparing `mlcvzoo_util-0.3.0/mlcvzoo_util/model_evaluator/configuration.py` & `mlcvzoo_util-0.3.1/mlcvzoo_util/model_evaluator/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright 2022 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """
 Module for configuring the parsing of information from yaml in python
 accessible attributes for the Evaluation Runner (ER) class
 """
 
 from typing import List, Optional
```

### Comparing `mlcvzoo_util-0.3.0/mlcvzoo_util/model_evaluator/metric_factory.py` & `mlcvzoo_util-0.3.1/mlcvzoo_util/model_evaluator/metric_factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright 2022 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """
 Module for the definition of a generic MetricFactory which provides
 interface methods. These interfaces are consumed by the ModelEvaluator
 in order to implement a generic metric computation functionally.
 """
 
@@ -92,15 +93,14 @@
 
     @staticmethod
     def compute_metrics(
         inference_model: ObjectDetectionModel,  # type: ignore[type-arg]
         gt_annotations: List[BaseAnnotation],
         model_evaluator_config: ModelEvaluatorConfig,
     ) -> ODModelEvaluationMetrics:
-
         return evaluate_with_model(
             model=inference_model,
             gt_annotations=gt_annotations,
             iou_thresholds=model_evaluator_config.iou_thresholds,
         )
 
     @staticmethod
```

### Comparing `mlcvzoo_util-0.3.0/mlcvzoo_util/model_evaluator/model_evaluator.py` & `mlcvzoo_util-0.3.1/mlcvzoo_util/model_evaluator/model_evaluator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright 2021 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """Module for evaluating mlcvzoo models"""
 
 import argparse
 import logging
 import os.path
 from abc import ABC
```

### Comparing `mlcvzoo_util-0.3.0/mlcvzoo_util/model_evaluator/structs.py` & `mlcvzoo_util-0.3.1/mlcvzoo_util/model_evaluator/structs.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright 2022 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """
 Module for defining enums and structs that are used across the
 model_evaluator package.
 """
 from dataclasses import dataclass
 from enum import Enum, auto
```

### Comparing `mlcvzoo_util-0.3.0/mlcvzoo_util/model_timer/configuration.py` & `mlcvzoo_util-0.3.1/mlcvzoo_util/model_timer/configuration.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright 2022 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 from typing import List, Optional
 
 import related
 from config_builder import BaseConfigClass
 from mlcvzoo_base.configuration.device_query import ModelTimerDeviceQueryConfig
 from mlcvzoo_base.configuration.mlfow_config import MLFlowConfig
```

### Comparing `mlcvzoo_util-0.3.0/mlcvzoo_util/model_timer/model_timer.py` & `mlcvzoo_util-0.3.1/mlcvzoo_util/model_timer/model_timer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,26 @@
-# Copyright 2022 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """Module that provides a generic component for measuring runtimes of mlcvzoo models"""
 
 import argparse
 import logging
 import time
 from typing import Any, Dict, List, Optional, Type, cast
 
 import cv2
 import mlflow
 from config_builder import ConfigBuilder
 from mlcvzoo_base.api.model import Model
 from mlcvzoo_base.configuration.model_config import ModelConfig
+from mlcvzoo_base.configuration.replacement_config import ReplacementConfig
 from mlcvzoo_base.configuration.structs import MLFlowExperimentTypes
 from mlcvzoo_base.metrics.mlflow.mlflow_runner import MLFLowRunner
 from mlcvzoo_base.models.model_registry import ModelRegistry
 from mlcvzoo_base.utils.gpu_util import GpuInfo, get_device_info
 
 from mlcvzoo_util.logger import Logger
 from mlcvzoo_util.mlcvzoo_cli_tool import MLCVZooCLITool, configure_model_argparse
```

### Comparing `mlcvzoo_util-0.3.0/mlcvzoo_util/model_trainer/configuration.py` & `mlcvzoo_util-0.3.1/mlcvzoo_util/model_trainer/configuration.py`

 * *Files 15% similar despite different names*

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
 Module for parsing information from yaml in python accessible attributes for the ModelSuite class.
 """
 
 import related
 from attr import define
```

### Comparing `mlcvzoo_util-0.3.0/mlcvzoo_util/model_trainer/model_trainer.py` & `mlcvzoo_util-0.3.1/mlcvzoo_util/model_trainer/model_trainer.py`

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
 
 """Module for handling the training of mlcvzoo models"""
 
 import argparse
 import logging
 from typing import Any, Dict, Optional, Type, cast
```

### Comparing `mlcvzoo_util-0.3.0/mlcvzoo_util/pre_annotation_tool/configuration.py` & `mlcvzoo_util-0.3.1/mlcvzoo_util/pre_annotation_tool/configuration.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright 2022 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """
 Module for configuring the parsing of information from yaml in python
 accessible attributes for the PreAnnotationTool class
 """
 
 import related
```

### Comparing `mlcvzoo_util-0.3.0/mlcvzoo_util/pre_annotation_tool/pre_annotation_tool.py` & `mlcvzoo_util-0.3.1/mlcvzoo_util/pre_annotation_tool/pre_annotation_tool.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-# Copyright 2022 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """
 Module for handling the generation and uploading of annotations to CVAT, which realizes that
 the feature of pre-annotating annotation tasks
 """
 
 import argparse
 import logging
 import os
 import zipfile
+from pathlib import Path
 from typing import Any, Dict, List, Optional, Tuple, Type, cast
 
 import cv2
 from config_builder import ConfigBuilder
 from mlcvzoo_base.api.data.annotation import BaseAnnotation
 from mlcvzoo_base.api.model import Model, ObjectDetectionModel
 from mlcvzoo_base.configuration.model_config import ModelConfig
@@ -249,15 +251,15 @@
             if not os.path.isfile(predicted_annotation.annotation_path) or (
                 os.path.isfile(predicted_annotation.annotation_path)
                 and self.configuration.overwrite_existing_annotations
             ):
                 # TODO: When ReadFromFile model is supporting images, then switch
                 #       to predict on image and not image-path
                 _, predicted_bounding_boxes = object_detection_model.predict(
-                    data_item=image_path
+                    data_item=str(Path(image_path).resolve())
                 )
 
                 logger.info("Predicted bounding boxes: %s" % predicted_bounding_boxes)
 
                 if self.video_live_output is not None:
                     self.video_live_output.output_frame(
                         draw_on_image(
```

### Comparing `mlcvzoo_util-0.3.0/mlcvzoo_util/video_image_creator/configuration.py` & `mlcvzoo_util-0.3.1/mlcvzoo_util/video_image_creator/configuration.py`

 * *Files 13% similar despite different names*

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
 Module for configuring the parsing of information from yaml in python
 accessible attributes for extracting frames from videos
 """
 from typing import Dict
```

### Comparing `mlcvzoo_util-0.3.0/mlcvzoo_util/video_image_creator/video_image_creator.py` & `mlcvzoo_util-0.3.1/mlcvzoo_util/video_image_creator/video_image_creator.py`

 * *Files 3% similar despite different names*

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
 Module for extracting frames from videos. In the context of the mlcvzoo, this
 is used to build training datasets.
 """
 
 import argparse
```

### Comparing `mlcvzoo_util-0.3.0/pyproject.toml` & `mlcvzoo_util-0.3.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "mlcvzoo_util"
-version = "0.3.0"
-license = "Open Logistics License Version 1.0"
 description = "MLCVZoo Util Package"
+version = "0.3.1"
+license = "Open Logistics Foundation License v1.3"
 readme = "README.md"
 homepage = "https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo"
 repository = "https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo"
 documentation = "https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo/-/blob/main/documentation/index.adoc"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
@@ -43,30 +43,33 @@
 
 yaml-config-builder = { version = "^8.0" }
 related-mltoolbox = { version = "^1.0" }
 mlcvzoo_base = { version = "^5.0" }
 
 # 1.19.2 is oldest available on aarch64 but 1.19.5 leads to unbuildable pytorch there, all is well on amd64
 numpy = { version = ">=1.19.2,!=1.19.5" }
-opencv-python = { version = "^4.5,!=4.5.5.64" }
-opencv-contrib-python = { version = "^4.5,!=4.5.5.64" }
-tqdm = { version = "^4.61" }
-imageio = { version = "^2.9" }
-mlflow = { version = "^1.22" }
-nptyping = { version="^2.0" }
+opencv-python = { version = ">=4.5,!=4.5.5.64"}
+opencv-contrib-python = { version = ">=4.5,!=4.5.5.64" }
+tqdm = { version = ">=4.61" }
+imageio = { version = ">=2.9" }
+# TODO: Newer mlflow pulls in llvmlite which is not _just_
+#       installable currently so defer upgrading this for now
+mlflow = { version = ">=1.22,<2" }
+nptyping = { version=">=2.0" }
 
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

### Comparing `mlcvzoo_util-0.3.0/setup.py` & `mlcvzoo_util-0.3.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,23 +11,23 @@
  'mlcvzoo_util.pre_annotation_tool',
  'mlcvzoo_util.video_image_creator']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['imageio>=2.9,<3.0',
+['imageio>=2.9',
  'mlcvzoo_base>=5.0,<6.0',
- 'mlflow>=1.22,<2.0',
- 'nptyping>=2.0,<3.0',
+ 'mlflow>=1.22,<2',
+ 'nptyping>=2.0',
  'numpy>=1.19.2,!=1.19.5',
- 'opencv-contrib-python>=4.5,<5.0,!=4.5.5.64',
- 'opencv-python>=4.5,<5.0,!=4.5.5.64',
+ 'opencv-contrib-python>=4.5,!=4.5.5.64',
+ 'opencv-python>=4.5,!=4.5.5.64',
  'related-mltoolbox>=1.0,<2.0',
- 'tqdm>=4.61,<5.0',
+ 'tqdm>=4.61',
  'yaml-config-builder>=8.0,<9.0']
 
 entry_points = \
 {'console_scripts': ['mlcvzoo-cvat-handler = '
                      'mlcvzoo_util.cvat_annotation_handler.cvat_annotation_handler:main',
                      'mlcvzoo-modelevaluator = '
                      'mlcvzoo_util.model_evaluator.model_evaluator:main',
@@ -38,15 +38,15 @@
                      'mlcvzoo-preannotator = '
                      'mlcvzoo_util.pre_annotation_tool.pre_annotation_tool:main',
                      'mlcvzoo-video-image-creator = '
                      'mlcvzoo_util.video_image_creator.video_image_creator:main']}
 
 setup_kwargs = {
     'name': 'mlcvzoo-util',
-    'version': '0.3.0',
+    'version': '0.3.1',
     'description': 'MLCVZoo Util Package',
     'long_description': '# MLCVZoo Util\n\nThe MLCVZoo is an SDK for simplifying the usage of various (machine learning driven)\ncomputer vision algorithms. The package **mlcvzoo_util** provides additional utility functions for downstream developments and tools for convenience and CLI usage.\n\nFurther information about the MLCVZoo can be found [here](../README.md).\n\n## Install\n`\npip install mlcvzoo-util\n`\n\n## Technology stack\n\n- Python\n',
     'author': 'Maximilian Otten',
     'author_email': 'maximilian.otten@iml.fraunhofer.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo',
```

### Comparing `mlcvzoo_util-0.3.0/PKG-INFO` & `mlcvzoo_util-0.3.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: mlcvzoo-util
-Version: 0.3.0
+Version: 0.3.1
 Summary: MLCVZoo Util Package
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
-Requires-Dist: imageio (>=2.9,<3.0)
+Requires-Dist: imageio (>=2.9)
 Requires-Dist: mlcvzoo_base (>=5.0,<6.0)
-Requires-Dist: mlflow (>=1.22,<2.0)
-Requires-Dist: nptyping (>=2.0,<3.0)
+Requires-Dist: mlflow (>=1.22,<2)
+Requires-Dist: nptyping (>=2.0)
 Requires-Dist: numpy (>=1.19.2,!=1.19.5)
-Requires-Dist: opencv-contrib-python (>=4.5,<5.0,!=4.5.5.64)
-Requires-Dist: opencv-python (>=4.5,<5.0,!=4.5.5.64)
+Requires-Dist: opencv-contrib-python (>=4.5,!=4.5.5.64)
+Requires-Dist: opencv-python (>=4.5,!=4.5.5.64)
 Requires-Dist: related-mltoolbox (>=1.0,<2.0)
-Requires-Dist: tqdm (>=4.61,<5.0)
+Requires-Dist: tqdm (>=4.61)
 Requires-Dist: yaml-config-builder (>=8.0,<9.0)
 Project-URL: Documentation, https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo/-/blob/main/documentation/index.adoc
 Project-URL: Repository, https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo
 Description-Content-Type: text/markdown
 
 # MLCVZoo Util
```

