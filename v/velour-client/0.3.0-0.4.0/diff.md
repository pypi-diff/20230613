# Comparing `tmp/velour-client-0.3.0.tar.gz` & `tmp/velour-client-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "velour-client-0.3.0.tar", last modified: Thu Jun  1 18:29:32 2023, max compression
+gzip compressed data, was "velour-client-0.4.0.tar", last modified: Tue Jun 13 18:45:19 2023, max compression
```

## Comparing `velour-client-0.3.0.tar` & `velour-client-0.4.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:29:32.983302 velour-client-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-01 18:29:23.000000 velour-client-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-06-01 18:29:32.983302 velour-client-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-01 18:29:23.000000 velour-client-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-01 18:29:23.000000 velour-client-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 18:29:32.983302 velour-client-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-01 18:29:23.000000 velour-client-0.3.0/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:29:32.979303 velour-client-0.3.0/unit-tests/
--rw-r--r--   0 runner    (1001) docker     (123)    11733 2023-06-01 18:29:23.000000 velour-client-0.3.0/unit-tests/test_chariot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-06-01 18:29:23.000000 velour-client-0.3.0/unit-tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-01 18:29:23.000000 velour-client-0.3.0/unit-tests/test_coco.py
--rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-06-01 18:29:23.000000 velour-client-0.3.0/unit-tests/test_data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-06-01 18:29:23.000000 velour-client-0.3.0/unit-tests/test_viz.py
--rw-r--r--   0 runner    (1001) docker     (123)     7757 2023-06-01 18:29:23.000000 velour-client-0.3.0/unit-tests/test_yolo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:29:32.979303 velour-client-0.3.0/velour/
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-01 18:29:23.000000 velour-client-0.3.0/velour/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28176 2023-06-01 18:29:23.000000 velour-client-0.3.0/velour/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-06-01 18:29:23.000000 velour-client-0.3.0/velour/data_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:29:32.983302 velour-client-0.3.0/velour/integrations/
--rw-r--r--   0 runner    (1001) docker     (123)    14911 2023-06-01 18:29:23.000000 velour-client-0.3.0/velour/integrations/chariot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-06-01 18:29:23.000000 velour-client-0.3.0/velour/integrations/coco.py
--rw-r--r--   0 runner    (1001) docker     (123)     5015 2023-06-01 18:29:23.000000 velour-client-0.3.0/velour/integrations/yolo.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-01 18:29:23.000000 velour-client-0.3.0/velour/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     6128 2023-06-01 18:29:23.000000 velour-client-0.3.0/velour/viz.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:29:32.983302 velour-client-0.3.0/velour_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-06-01 18:29:32.000000 velour-client-0.3.0/velour_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-01 18:29:32.000000 velour-client-0.3.0/velour_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 18:29:32.000000 velour-client-0.3.0/velour_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-01 18:29:32.000000 velour-client-0.3.0/velour_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-01 18:29:32.000000 velour-client-0.3.0/velour_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:45:19.660563 velour-client-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-13 18:45:10.000000 velour-client-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-06-13 18:45:19.660563 velour-client-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-13 18:45:10.000000 velour-client-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-13 18:45:10.000000 velour-client-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 18:45:19.660563 velour-client-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-13 18:45:10.000000 velour-client-0.4.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:45:19.656563 velour-client-0.4.0/unit-tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    11733 2023-06-13 18:45:10.000000 velour-client-0.4.0/unit-tests/test_chariot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-06-13 18:45:10.000000 velour-client-0.4.0/unit-tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-13 18:45:10.000000 velour-client-0.4.0/unit-tests/test_coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-06-13 18:45:10.000000 velour-client-0.4.0/unit-tests/test_data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-06-13 18:45:10.000000 velour-client-0.4.0/unit-tests/test_viz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7838 2023-06-13 18:45:10.000000 velour-client-0.4.0/unit-tests/test_yolo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:45:19.656563 velour-client-0.4.0/velour/
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-13 18:45:10.000000 velour-client-0.4.0/velour/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28267 2023-06-13 18:45:10.000000 velour-client-0.4.0/velour/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-06-13 18:45:10.000000 velour-client-0.4.0/velour/data_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:45:19.656563 velour-client-0.4.0/velour/integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)    14911 2023-06-13 18:45:10.000000 velour-client-0.4.0/velour/integrations/chariot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-06-13 18:45:10.000000 velour-client-0.4.0/velour/integrations/coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5305 2023-06-13 18:45:10.000000 velour-client-0.4.0/velour/integrations/yolo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-13 18:45:10.000000 velour-client-0.4.0/velour/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6128 2023-06-13 18:45:10.000000 velour-client-0.4.0/velour/viz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:45:19.660563 velour-client-0.4.0/velour_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-06-13 18:45:19.000000 velour-client-0.4.0/velour_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-13 18:45:19.000000 velour-client-0.4.0/velour_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 18:45:19.000000 velour-client-0.4.0/velour_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-13 18:45:19.000000 velour-client-0.4.0/velour_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-13 18:45:19.000000 velour-client-0.4.0/velour_client.egg-info/top_level.txt
```

### Comparing `velour-client-0.3.0/LICENSE` & `velour-client-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `velour-client-0.3.0/PKG-INFO` & `velour-client-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: velour-client
-Version: 0.3.0
+Version: 0.4.0
 Summary: Python client for the Velour evaluation store
 License: Copyright 2023 Striveworks
         
         Permission is hereby granted, free of charge, to any person obtaining
         a copy of this software and associated documentation files (the
         "Software"), to deal in the Software without restriction, including
         without limitation the rights to use, copy, modify, merge, publish,
```

### Comparing `velour-client-0.3.0/pyproject.toml` & `velour-client-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `velour-client-0.3.0/unit-tests/test_chariot.py` & `velour-client-0.4.0/unit-tests/test_chariot.py`

 * *Files identical despite different names*

### Comparing `velour-client-0.3.0/unit-tests/test_client.py` & `velour-client-0.4.0/unit-tests/test_client.py`

 * *Files identical despite different names*

### Comparing `velour-client-0.3.0/unit-tests/test_coco.py` & `velour-client-0.4.0/unit-tests/test_coco.py`

 * *Files identical despite different names*

### Comparing `velour-client-0.3.0/unit-tests/test_data_types.py` & `velour-client-0.4.0/unit-tests/test_data_types.py`

 * *Files identical despite different names*

### Comparing `velour-client-0.3.0/unit-tests/test_viz.py` & `velour-client-0.4.0/unit-tests/test_viz.py`

 * *Files identical despite different names*

### Comparing `velour-client-0.3.0/unit-tests/test_yolo.py` & `velour-client-0.4.0/unit-tests/test_yolo.py`

 * *Files 3% similar despite different names*

```diff
@@ -208,29 +208,31 @@
     results = Results(
         orig_img=numpy.random.rand(image["height"], image["width"], 3),
         path=image["path"],
         names=names,
         probs=probs,
     )
 
-    predictions = parse_yolo_image_classification(results, image["uid"])
+    predictions = parse_yolo_image_classification(
+        results, image["uid"], label_key="class"
+    )
 
     assert len(predictions) == 1
 
     prediction = predictions[0]
 
     assert isinstance(prediction, PredictedImageClassification)
 
     assert prediction.image.uid == image["uid"]
     assert prediction.image.height == image["height"]
     assert prediction.image.width == image["width"]
     assert prediction.image.frame is None
 
     for i in range(len(prediction.scored_labels)):
-        assert prediction.scored_labels[i].label.key == "class_label"
+        assert prediction.scored_labels[i].label.key == "class"
         assert prediction.scored_labels[i].label.value == names[i]
         assert prediction.scored_labels[i].score == probs[i]
 
 
 def test__convert_yolo_segmentation(image, yolo_mask, velour_mask):
     yolo_mask = MaskOnGPU(yolo_mask)
     output = _convert_yolo_segmentation(
@@ -250,46 +252,50 @@
         orig_img=img,
         path=image["path"],
         names=names,
         boxes=bboxes,
         masks=masks,
     )
 
-    predictions = parse_yolo_image_segmentation(results, image["uid"])
+    predictions = parse_yolo_image_segmentation(
+        results, image["uid"], label_key="class"
+    )
 
     assert len(predictions) == bboxes.shape[0]
     for i in range(len(predictions)):
         assert isinstance(predictions[i], PredictedInstanceSegmentation)
         assert predictions[i].image.uid == image["uid"]
         assert predictions[i].image.height == image["height"]
         assert predictions[i].image.width == image["width"]
         assert predictions[i].image.frame is None
-        assert predictions[i].scored_labels[0].label.key == "class_label"
+        assert predictions[i].scored_labels[0].label.key == "class"
         assert predictions[i].scored_labels[0].label.value == names[i]
         assert predictions[i].scored_labels[0].score == bboxes[i][4]
         assert predictions[i].mask.shape == velour_mask.shape
         assert (predictions[i].mask == velour_mask).all()
 
 
 def test_parse_yolo_object_detection(image, bboxes, names):
     img = numpy.random.rand(image["height"], image["width"], 3)
 
     results = Results(
         orig_img=img, path=image["path"], names=names, boxes=bboxes
     )
 
-    predictions = parse_yolo_object_detection(results, image["uid"])
+    predictions = parse_yolo_object_detection(
+        results, image["uid"], label_key="class"
+    )
 
     assert len(predictions) == bboxes.shape[0]
     for i in range(len(predictions)):
         assert isinstance(predictions[i], PredictedDetection)
         assert predictions[i].image.uid == image["uid"]
         assert predictions[i].image.height == image["height"]
         assert predictions[i].image.width == image["width"]
         assert predictions[i].image.frame is None
-        assert predictions[i].scored_labels[0].label.key == "class_label"
+        assert predictions[i].scored_labels[0].label.key == "class"
         assert predictions[i].scored_labels[0].label.value == names[i]
         assert predictions[i].scored_labels[0].score == bboxes[i][4]
         assert predictions[i].bbox.xmin == bboxes[i][0]
         assert predictions[i].bbox.ymin == bboxes[i][1]
         assert predictions[i].bbox.xmax == bboxes[i][2]
         assert predictions[i].bbox.ymax == bboxes[i][3]
```

### Comparing `velour-client-0.3.0/velour/client.py` & `velour-client-0.4.0/velour/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import io
 import json
 import math
 import os
 from base64 import b64decode, b64encode
 from dataclasses import asdict
 from enum import Enum
-from typing import Dict, List, Union
+from typing import Dict, List, Optional, Union
 from urllib.parse import urljoin
 
 import numpy as np
 import PIL.Image
 import requests
 from tqdm.auto import tqdm
 
@@ -589,27 +589,29 @@
         dataset: ImageDataset,
         model_pred_task_type: Task = None,
         dataset_gt_task_type: Task = None,
         iou_thresholds: List[float] = None,
         ious_to_keep: List[float] = None,
         min_area: float = None,
         max_area: float = None,
+        label_key: Optional[str] = None,
     ) -> "EvalJob":
         payload = {
             "settings": {
                 "model_name": self.name,
                 "dataset_name": dataset.name,
                 "model_pred_task_type": model_pred_task_type.value
                 if model_pred_task_type is not None
                 else None,
                 "dataset_gt_task_type": dataset_gt_task_type.value
                 if dataset_gt_task_type is not None
                 else None,
                 "min_area": min_area,
                 "max_area": max_area,
+                "label_key": label_key,
             }
         }
 
         if iou_thresholds is not None:
             payload["iou_thresholds"] = iou_thresholds
         if ious_to_keep is not None:
             payload["ious_to_keep"] = ious_to_keep
```

### Comparing `velour-client-0.3.0/velour/data_types.py` & `velour-client-0.4.0/velour/data_types.py`

 * *Files identical despite different names*

### Comparing `velour-client-0.3.0/velour/integrations/chariot.py` & `velour-client-0.4.0/velour/integrations/chariot.py`

 * *Files identical despite different names*

### Comparing `velour-client-0.3.0/velour/integrations/coco.py` & `velour-client-0.4.0/velour/integrations/coco.py`

 * *Files identical despite different names*

### Comparing `velour-client-0.3.0/velour/integrations/yolo.py` & `velour-client-0.4.0/velour/integrations/yolo.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,28 +11,30 @@
     PredictedDetection,
     PredictedImageClassification,
     PredictedInstanceSegmentation,
     ScoredLabel,
 )
 
 
-def parse_yolo_image_classification(result, uid: str):
+def parse_yolo_image_classification(
+    result, uid: str, label_key: str = "class"
+):
     """Parses Ultralytic's result for an image classification task."""
 
     # Extract data
     image_uid = uid
     image_height = result.orig_shape[0]
     image_width = result.orig_shape[1]
     probabilities = result.probs
     labels = result.names
 
     # Create scored label list
     scored_labels = [
         ScoredLabel(
-            label=Label(key="class_label", value=labels[key]),
+            label=Label(key=label_key, value=labels[key]),
             score=probability.item(),
         )
         for key, probability in list(zip(labels, probabilities))
     ]
 
     return [
         PredictedImageClassification(
@@ -58,30 +60,36 @@
     img = PIL.Image.fromarray(numpy.uint8(mask))
     img = img.resize((width, height), resample=resample)
     mask = numpy.array(img, dtype=numpy.uint8) >= 128
     return mask
 
 
 def parse_yolo_image_segmentation(
-    result, uid: str, resample: Resampling = Resampling.BILINEAR
+    result,
+    uid: str,
+    label_key: str = "class",
+    resample: Resampling = Resampling.BILINEAR,
 ):
     """Parses Ultralytic's result for an image segmentation task."""
 
+    if result.masks.data is None:
+        return []
+
     # Extract data
     image_uid = uid
     image_height = result.orig_shape[0]
     image_width = result.orig_shape[1]
     probabilities = [conf.item() for conf in result.boxes.conf]
     labels = [result.names[int(pred.item())] for pred in result.boxes.cls]
     masks = [mask for mask in result.masks.data]
 
     # Create scored label list
     scored_labels = [
         ScoredLabel(
-            label=Label(key="class_label", value=label),
+            label=Label(key=label_key, value=label),
             score=probability,
         )
         for label, probability in list(zip(labels, probabilities))
     ]
 
     # Extract masks
     masks = [
@@ -101,29 +109,29 @@
                 width=image_width,
             ),
         )
         for mask, scored_label in list(zip(masks, scored_labels))
     ]
 
 
-def parse_yolo_object_detection(result, uid: str):
+def parse_yolo_object_detection(result, uid: str, label_key: str = "class"):
     """Parses Ultralytic's result for an object detection task."""
 
     # Extract data
     image_uid = uid
     image_height = result.orig_shape[0]
     image_width = result.orig_shape[1]
     probabilities = [conf.item() for conf in result.boxes.conf]
     labels = [result.names[int(pred.item())] for pred in result.boxes.cls]
     bboxes = [numpy.asarray(box.cpu()) for box in result.boxes.xyxy]
 
     # Create scored label list
     scored_labels = [
         ScoredLabel(
-            label=Label(key="class_label", value=label),
+            label=Label(key=label_key, value=label),
             score=probability,
         )
         for label, probability in list(zip(labels, probabilities))
     ]
 
     # Extract Bounding Boxes
     bboxes = [
@@ -149,14 +157,15 @@
         for bbox, scored_label in list(zip(bboxes, scored_labels))
     ]
 
 
 def parse_yolo_results(
     results,
     uid: str,
+    label_key: str = "class",
     segmentation_resample: Resampling = Resampling.BILINEAR,
 ) -> Union[
     PredictedDetection,
     PredictedImageClassification,
     PredictedInstanceSegmentation,
 ]:
     """Automatically chooses correct parser for Ultralytic YOLO model inferences.
@@ -171,17 +180,22 @@
     Returns
     -------
     Velour prediction.
     """
 
     if "masks" in results.keys and "boxes" in results.keys:
         return parse_yolo_image_segmentation(
-            results, uid=uid, resample=segmentation_resample
+            results,
+            uid=uid,
+            label_key=label_key,
+            resample=segmentation_resample,
         )
     elif "boxes" in results.keys:
-        return parse_yolo_object_detection(results, uid)
+        return parse_yolo_object_detection(results, uid, label_key=label_key)
     elif "probs" in results.keys:
-        return parse_yolo_image_classification(results, uid)
+        return parse_yolo_image_classification(
+            results, uid, label_key=label_key
+        )
     else:
         raise ValueError(
             "Input arguement 'result' does not contain identifiable information."
         )
```

### Comparing `velour-client-0.3.0/velour/viz.py` & `velour-client-0.4.0/velour/viz.py`

 * *Files identical despite different names*

### Comparing `velour-client-0.3.0/velour_client.egg-info/PKG-INFO` & `velour-client-0.4.0/velour_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: velour-client
-Version: 0.3.0
+Version: 0.4.0
 Summary: Python client for the Velour evaluation store
 License: Copyright 2023 Striveworks
         
         Permission is hereby granted, free of charge, to any person obtaining
         a copy of this software and associated documentation files (the
         "Software"), to deal in the Software without restriction, including
         without limitation the rights to use, copy, modify, merge, publish,
```

### Comparing `velour-client-0.3.0/velour_client.egg-info/SOURCES.txt` & `velour-client-0.4.0/velour_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

