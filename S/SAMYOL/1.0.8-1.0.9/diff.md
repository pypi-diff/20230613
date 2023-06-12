# Comparing `tmp/SAMYOL-1.0.8.tar.gz` & `tmp/SAMYOL-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SAMYOL-1.0.8.tar", last modified: Mon Jun 12 13:56:28 2023, max compression
+gzip compressed data, was "SAMYOL-1.0.9.tar", last modified: Mon Jun 12 22:00:12 2023, max compression
```

## Comparing `SAMYOL-1.0.8.tar` & `SAMYOL-1.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:56:28.523151 SAMYOL-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-12 13:56:18.000000 SAMYOL-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-06-12 13:56:28.523151 SAMYOL-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-06-12 13:56:18.000000 SAMYOL-1.0.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:56:28.519151 SAMYOL-1.0.8/SAMYOL/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-12 13:56:18.000000 SAMYOL-1.0.8/SAMYOL/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-06-12 13:56:18.000000 SAMYOL-1.0.8/SAMYOL/prediction_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-06-12 13:56:18.000000 SAMYOL-1.0.8/SAMYOL/predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-06-12 13:56:18.000000 SAMYOL-1.0.8/SAMYOL/sam_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     7035 2023-06-12 13:56:18.000000 SAMYOL-1.0.8/SAMYOL/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-06-12 13:56:18.000000 SAMYOL-1.0.8/SAMYOL/yolo_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-06-12 13:56:18.000000 SAMYOL-1.0.8/SAMYOL/yolo_postprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-06-12 13:56:18.000000 SAMYOL-1.0.8/SAMYOL/yolo_preprocessing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:56:28.523151 SAMYOL-1.0.8/SAMYOL.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-06-12 13:56:28.000000 SAMYOL-1.0.8/SAMYOL.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-12 13:56:28.000000 SAMYOL-1.0.8/SAMYOL.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 13:56:28.000000 SAMYOL-1.0.8/SAMYOL.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-12 13:56:28.000000 SAMYOL-1.0.8/SAMYOL.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-12 13:56:28.000000 SAMYOL-1.0.8/SAMYOL.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 13:56:28.523151 SAMYOL-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-06-12 13:56:18.000000 SAMYOL-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 22:00:12.841010 SAMYOL-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-12 22:00:01.000000 SAMYOL-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-06-12 22:00:12.841010 SAMYOL-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-06-12 22:00:01.000000 SAMYOL-1.0.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 22:00:12.841010 SAMYOL-1.0.9/SAMYOL/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-12 22:00:01.000000 SAMYOL-1.0.9/SAMYOL/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4323 2023-06-12 22:00:01.000000 SAMYOL-1.0.9/SAMYOL/prediction_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-06-12 22:00:01.000000 SAMYOL-1.0.9/SAMYOL/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6079 2023-06-12 22:00:01.000000 SAMYOL-1.0.9/SAMYOL/sam_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7035 2023-06-12 22:00:01.000000 SAMYOL-1.0.9/SAMYOL/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-06-12 22:00:01.000000 SAMYOL-1.0.9/SAMYOL/yolo_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-06-12 22:00:01.000000 SAMYOL-1.0.9/SAMYOL/yolo_postprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-06-12 22:00:01.000000 SAMYOL-1.0.9/SAMYOL/yolo_preprocessing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 22:00:12.841010 SAMYOL-1.0.9/SAMYOL.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-06-12 22:00:12.000000 SAMYOL-1.0.9/SAMYOL.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-12 22:00:12.000000 SAMYOL-1.0.9/SAMYOL.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 22:00:12.000000 SAMYOL-1.0.9/SAMYOL.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-12 22:00:12.000000 SAMYOL-1.0.9/SAMYOL.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-12 22:00:12.000000 SAMYOL-1.0.9/SAMYOL.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 22:00:12.841010 SAMYOL-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-06-12 22:00:01.000000 SAMYOL-1.0.9/setup.py
```

### Comparing `SAMYOL-1.0.8/LICENSE` & `SAMYOL-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `SAMYOL-1.0.8/PKG-INFO` & `SAMYOL-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SAMYOL
-Version: 1.0.8
+Version: 1.0.9
 Summary: Combines YOLO models and SAM
 Author: Jawher Ben Abdallah
 Author-email: jawher.b.abdallah@gmail.com
 Maintainer: Rim Sleimi
 Maintainer-email: sleimi.rim1996@gmail.com
 License: Apache License 2.0
 Project-URL: Source, https://github.com/Jawher-Ben-Abdallah/SAMYOL
```

### Comparing `SAMYOL-1.0.8/README.rst` & `SAMYOL-1.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `SAMYOL-1.0.8/SAMYOL/prediction_results.py` & `SAMYOL-1.0.9/SAMYOL/prediction_results.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,14 +26,17 @@
     def display(self, index: int) -> None:
         """
         Display the bounding boxes and masks for a specific image.
 
         Args:
             index (int): Index of the image to display.
         """
+        if not index in self.predictions.keys():
+            raise Exception(f"No predictions found for image of id: {index}.")
+        
         image = self.images[index]
         target_predictions = self.predictions[index]
 
         # Create a subplot for displaying the image, bounding boxes, and masks
         fig, ax = plt.subplots(figsize=(6, 6))
 
         # Plot the image
@@ -78,15 +81,17 @@
             save_dir (str): Directory to save the images.
             filename (str): Filename for the saved images.
             fuse_masks (bool): Whether to merge all masks or save them separately.
             save_metadata (bool): Whether to save metadata as a JSON file.
             image_id (int): Index of the image to save.
             mask_format (str): Image format to save.
         """
-
+        if not image_id in self.predictions.keys():
+            raise Exception(f"No predictions found for image of id: {image_id}.")
+        
         filtered_data = self.predictions[image_id]
         masks = filtered_data['masks']
         if fuse_masks:
             # Merge all masks
             masks = np.logical_or.reduce(np.array(masks))
             cv2.imwrite(f"{save_dir}/{filename}.{mask_format}", masks * 255)
         else:
```

### Comparing `SAMYOL-1.0.8/SAMYOL/predictor.py` & `SAMYOL-1.0.9/SAMYOL/predictor.py`

 * *Files identical despite different names*

### Comparing `SAMYOL-1.0.8/SAMYOL/sam_inference.py` & `SAMYOL-1.0.9/SAMYOL/sam_inference.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         check_and_install_library('segment_anything')
         from segment_anything import SamPredictor, sam_model_registry
         model_type, model_path = download_model_weights(sam_model_type)
         sam = sam_model_registry[model_type](checkpoint=model_path).to(device)
         predictor = SamPredictor(sam)
 
         # Get predictions from SAM
-        object_segmentation_predictions = []
+        object_segmentation_predictions = {}
 
         image_ids = list(set([d['image_id'] for d in obj_det_predictions]))
 
         for image_id in image_ids:
             # Filter the data based on the current image_id
             filtered_data = [d for d in obj_det_predictions if d['image_id'] == image_id]
 
@@ -62,21 +62,22 @@
                 point_coords=None,
                 point_labels=None,
                 boxes=transformed_boxes,
                 multimask_output=True
             )
             idx_max_iou = torch.argmax(scores.view(-1, 3), dim=1).tolist()
 
-            object_segmentation_predictions.append({
-                'image_id': image_id,
-                'class_id': class_ids,
-                'class_label': class_labels,
-                'score': [scores.squeeze()[i, j, ...].item() for i, j in enumerate(idx_max_iou)],
-                'bbox': bboxes,
-                'masks': [masks[i, j, ...].cpu().numpy() for i, j in enumerate(idx_max_iou)]
+            object_segmentation_predictions.update({
+                image_id : {
+                    'class_id': class_ids,
+                    'class_label': class_labels,
+                    'score': [scores.squeeze()[i, j, ...].item() for i, j in enumerate(idx_max_iou)],
+                    'bbox': bboxes,
+                    'masks': [masks[i, j, ...].cpu().numpy() for i, j in enumerate(idx_max_iou)]
+                }
             })
 
         return object_segmentation_predictions
 
     @staticmethod
     def predict_from_HuggingFace(
         sam_model_type: str,
@@ -100,15 +101,15 @@
         check_and_install_library('transformers')
         from transformers import SamModel, SamProcessor
 
         sam_model = SamModel.from_pretrained(f"facebook/sam-vit-{sam_model_type}").to(device)
         sam_processor = SamProcessor.from_pretrained(f"facebook/sam-vit-{sam_model_type}")
 
         # Get predictions from SAM
-        object_segmentation_predictions = []
+        object_segmentation_predictions = {}
 
         image_ids = list(set([d['image_id'] for d in obj_det_predictions]))
 
         for image_id in image_ids:
             # Filter the data based on the current image_id
             filtered_data = [d for d in obj_det_predictions if d['image_id'] == image_id]
 
@@ -132,17 +133,18 @@
             masks = sam_processor.image_processor.post_process_masks(outputs.pred_masks.cpu(), inputs["original_sizes"].cpu(), inputs["reshaped_input_sizes"].cpu())
             scores = outputs.iou_scores
 
             # Reshape the tensor to have size (N, 3)
             reshaped_iou_scores = outputs.iou_scores.squeeze()
             idx_max_iou = torch.argmax(reshaped_iou_scores.view(-1, 3), dim=1).tolist()
 
-            object_segmentation_predictions.append({
-                'image_id': image_id,
-                'class_id': class_ids,
-                'class_label': class_labels,
-                'score': [outputs.iou_scores.squeeze()[i, j, ...].item() for i, j in enumerate(idx_max_iou)],
-                'bbox': bboxes,
-                'masks': [masks[0][i, j, ...].cpu().numpy() for i, j in enumerate(idx_max_iou)]
+            object_segmentation_predictions.update({
+                image_id : {
+                    'class_id': class_ids,
+                    'class_label': class_labels,
+                    'score': [outputs.iou_scores.squeeze()[i, j, ...].item() for i, j in enumerate(idx_max_iou)],
+                    'bbox': bboxes,
+                    'masks': [masks[0][i, j, ...].cpu().numpy() for i, j in enumerate(idx_max_iou)]
+                }
             })
 
         return object_segmentation_predictions
```

### Comparing `SAMYOL-1.0.8/SAMYOL/utils.py` & `SAMYOL-1.0.9/SAMYOL/utils.py`

 * *Files identical despite different names*

### Comparing `SAMYOL-1.0.8/SAMYOL/yolo_inference.py` & `SAMYOL-1.0.9/SAMYOL/yolo_inference.py`

 * *Files identical despite different names*

### Comparing `SAMYOL-1.0.8/SAMYOL/yolo_postprocessing.py` & `SAMYOL-1.0.9/SAMYOL/yolo_postprocessing.py`

 * *Files identical despite different names*

### Comparing `SAMYOL-1.0.8/SAMYOL/yolo_preprocessing.py` & `SAMYOL-1.0.9/SAMYOL/yolo_preprocessing.py`

 * *Files identical despite different names*

### Comparing `SAMYOL-1.0.8/SAMYOL.egg-info/PKG-INFO` & `SAMYOL-1.0.9/SAMYOL.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SAMYOL
-Version: 1.0.8
+Version: 1.0.9
 Summary: Combines YOLO models and SAM
 Author: Jawher Ben Abdallah
 Author-email: jawher.b.abdallah@gmail.com
 Maintainer: Rim Sleimi
 Maintainer-email: sleimi.rim1996@gmail.com
 License: Apache License 2.0
 Project-URL: Source, https://github.com/Jawher-Ben-Abdallah/SAMYOL
```

### Comparing `SAMYOL-1.0.8/setup.py` & `SAMYOL-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 long_description = 'SAMYOL is a Python library that combines an object detection model (YOLOv6, YOLOv7, YOLOv8, or YOLO-NAS) and the Segment Anything Model (SAM).'
 setup(
   name="SAMYOL",
-  version="1.0.8",
+  version="1.0.9",
   description="Combines YOLO models and SAM",
   packages=find_packages(),
   long_description=long_description,
   long_description_content_type="text/x-rst",
   project_urls={
         'Source': 'https://github.com/Jawher-Ben-Abdallah/SAMYOL',
     },
```

