# Comparing `tmp/innovationmerge-1.0.5.tar.gz` & `tmp/innovationmerge-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "innovationmerge-1.0.5.tar", max compression
+gzip compressed data, was "innovationmerge-1.0.6.tar", max compression
```

## Comparing `innovationmerge-1.0.5.tar` & `innovationmerge-1.0.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      180 2023-06-11 12:39:59.490310 innovationmerge-1.0.5/innovationmerge/__init__.py
--rw-r--r--   0        0        0      986 2023-06-04 12:33:31.912374 innovationmerge-1.0.5/innovationmerge/app/__init__.py
--rw-r--r--   0        0        0      339 2023-06-04 12:33:31.896708 innovationmerge-1.0.5/innovationmerge/app/exceptions.py
--rw-r--r--   0        0        0      776 2023-06-04 12:33:31.912374 innovationmerge-1.0.5/innovationmerge/app/logger/__init__.py
--rw-r--r--   0        0        0     1342 2023-06-04 12:33:31.912374 innovationmerge-1.0.5/innovationmerge/app/middleware/__init__.py
--rw-r--r--   0        0        0      655 2023-06-04 12:33:31.927958 innovationmerge-1.0.5/innovationmerge/app/routers/__init__.py
--rw-r--r--   0        0        0     1414 2023-06-04 12:33:31.912374 innovationmerge-1.0.5/innovationmerge/app/routers/authenticate.py
--rw-r--r--   0        0        0     1520 2023-06-04 12:33:31.927958 innovationmerge-1.0.5/innovationmerge/app/routers/sample_route.py
--rw-r--r--   0        0        0       46 2023-06-04 12:33:31.896708 innovationmerge-1.0.5/innovationmerge/app/sample.py
--rw-r--r--   0        0        0      104 2023-06-04 12:33:31.927958 innovationmerge-1.0.5/innovationmerge/app/schemas/sample_schema.py
--rw-r--r--   0        0        0      459 2023-06-04 12:33:31.927958 innovationmerge-1.0.5/innovationmerge/app/schemas/user_schema.py
--rw-r--r--   0        0        0     3226 2023-06-04 12:33:31.912374 innovationmerge-1.0.5/innovationmerge/app/security.py
--rw-r--r--   0        0        0     1836 2023-06-04 12:33:31.881091 innovationmerge-1.0.5/innovationmerge/config.py
--rw-r--r--   0        0        0       94 2023-06-11 07:21:11.268905 innovationmerge-1.0.5/innovationmerge/configurations/constants.py
--rw-r--r--   0        0        0     1300 2023-06-04 12:33:31.943618 innovationmerge-1.0.5/innovationmerge/docs/api_doc.py
--rw-r--r--   0        0        0        0 2023-06-04 12:33:31.943618 innovationmerge-1.0.5/innovationmerge/docs/file.md
--rw-r--r--   0        0        0        0 2023-06-04 12:33:31.943618 innovationmerge-1.0.5/innovationmerge/scripts/test.sh
--rw-r--r--   0        0        0        0 2023-06-04 13:48:12.834202 innovationmerge-1.0.5/innovationmerge/src/ai/__init__.py
--rw-r--r--   0        0        0        0 2023-06-04 13:48:12.834202 innovationmerge-1.0.5/innovationmerge/src/ai/cpu/__init__.py
--rw-r--r--   0        0        0     8690 2023-06-11 12:37:12.329152 innovationmerge-1.0.5/innovationmerge/src/ai/cpu/object_detection.py
--rw-r--r--   0        0        0        0 2023-06-04 16:01:26.589721 innovationmerge-1.0.5/innovationmerge/src/ai/edge/__init__.py
--rw-r--r--   0        0        0      148 2023-06-04 14:35:41.131565 innovationmerge-1.0.5/innovationmerge/src/ai/edge/object_detection.py
--rw-r--r--   0        0        0     1576 2023-06-11 08:17:15.382234 innovationmerge-1.0.5/innovationmerge/src/utils/responses.py
--rw-r--r--   0        0        0      153 2023-06-04 12:33:31.943618 innovationmerge-1.0.5/innovationmerge/tests/__init__.py
--rw-r--r--   0        0        0     3188 2023-06-04 12:33:31.943618 innovationmerge-1.0.5/innovationmerge/tests/sample.py
--rw-r--r--   0        0        0     1193 2023-06-11 12:39:40.887778 innovationmerge-1.0.5/innovationmerge/tests/test_object_detection.py
--rw-r--r--   0        0        0     1070 2023-06-11 13:08:46.873762 innovationmerge-1.0.5/pyproject.toml
--rw-r--r--   0        0        0      447 2023-06-04 14:30:02.127230 innovationmerge-1.0.5/README.md
--rw-r--r--   0        0        0     1771 1970-01-01 00:00:00.000000 innovationmerge-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0      180 2023-06-11 12:39:59.490310 innovationmerge-1.0.6/innovationmerge/__init__.py
+-rw-r--r--   0        0        0      986 2023-06-04 12:33:31.912374 innovationmerge-1.0.6/innovationmerge/app/__init__.py
+-rw-r--r--   0        0        0      339 2023-06-04 12:33:31.896708 innovationmerge-1.0.6/innovationmerge/app/exceptions.py
+-rw-r--r--   0        0        0      776 2023-06-04 12:33:31.912374 innovationmerge-1.0.6/innovationmerge/app/logger/__init__.py
+-rw-r--r--   0        0        0     1342 2023-06-04 12:33:31.912374 innovationmerge-1.0.6/innovationmerge/app/middleware/__init__.py
+-rw-r--r--   0        0        0      655 2023-06-04 12:33:31.927958 innovationmerge-1.0.6/innovationmerge/app/routers/__init__.py
+-rw-r--r--   0        0        0     1414 2023-06-04 12:33:31.912374 innovationmerge-1.0.6/innovationmerge/app/routers/authenticate.py
+-rw-r--r--   0        0        0     1520 2023-06-04 12:33:31.927958 innovationmerge-1.0.6/innovationmerge/app/routers/sample_route.py
+-rw-r--r--   0        0        0       46 2023-06-04 12:33:31.896708 innovationmerge-1.0.6/innovationmerge/app/sample.py
+-rw-r--r--   0        0        0      104 2023-06-04 12:33:31.927958 innovationmerge-1.0.6/innovationmerge/app/schemas/sample_schema.py
+-rw-r--r--   0        0        0      459 2023-06-04 12:33:31.927958 innovationmerge-1.0.6/innovationmerge/app/schemas/user_schema.py
+-rw-r--r--   0        0        0     3226 2023-06-04 12:33:31.912374 innovationmerge-1.0.6/innovationmerge/app/security.py
+-rw-r--r--   0        0        0     1836 2023-06-04 12:33:31.881091 innovationmerge-1.0.6/innovationmerge/config.py
+-rw-r--r--   0        0        0       94 2023-06-11 07:21:11.268905 innovationmerge-1.0.6/innovationmerge/configurations/constants.py
+-rw-r--r--   0        0        0     1300 2023-06-04 12:33:31.943618 innovationmerge-1.0.6/innovationmerge/docs/api_doc.py
+-rw-r--r--   0        0        0        0 2023-06-04 12:33:31.943618 innovationmerge-1.0.6/innovationmerge/docs/file.md
+-rw-r--r--   0        0        0        0 2023-06-04 12:33:31.943618 innovationmerge-1.0.6/innovationmerge/scripts/test.sh
+-rw-r--r--   0        0        0        0 2023-06-04 13:48:12.834202 innovationmerge-1.0.6/innovationmerge/src/ai/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-04 13:48:12.834202 innovationmerge-1.0.6/innovationmerge/src/ai/cpu/__init__.py
+-rw-r--r--   0        0        0     8690 2023-06-11 12:37:12.329152 innovationmerge-1.0.6/innovationmerge/src/ai/cpu/object_detection.py
+-rw-r--r--   0        0        0        0 2023-06-04 16:01:26.589721 innovationmerge-1.0.6/innovationmerge/src/ai/edge/__init__.py
+-rw-r--r--   0        0        0      148 2023-06-04 14:35:41.131565 innovationmerge-1.0.6/innovationmerge/src/ai/edge/object_detection.py
+-rw-r--r--   0        0        0     2598 2023-06-13 17:52:52.825884 innovationmerge-1.0.6/innovationmerge/src/utils/responses.py
+-rw-r--r--   0        0        0      153 2023-06-04 12:33:31.943618 innovationmerge-1.0.6/innovationmerge/tests/__init__.py
+-rw-r--r--   0        0        0     3188 2023-06-04 12:33:31.943618 innovationmerge-1.0.6/innovationmerge/tests/sample.py
+-rw-r--r--   0        0        0     1193 2023-06-11 12:39:40.887778 innovationmerge-1.0.6/innovationmerge/tests/test_object_detection.py
+-rw-r--r--   0        0        0      925 2023-06-13 17:56:28.680663 innovationmerge-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0      447 2023-06-04 14:30:02.127230 innovationmerge-1.0.6/README.md
+-rw-r--r--   0        0        0     1500 1970-01-01 00:00:00.000000 innovationmerge-1.0.6/PKG-INFO
```

### Comparing `innovationmerge-1.0.5/innovationmerge/app/__init__.py` & `innovationmerge-1.0.6/innovationmerge/app/__init__.py`

 * *Files identical despite different names*

### Comparing `innovationmerge-1.0.5/innovationmerge/app/logger/__init__.py` & `innovationmerge-1.0.6/innovationmerge/app/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `innovationmerge-1.0.5/innovationmerge/app/middleware/__init__.py` & `innovationmerge-1.0.6/innovationmerge/app/middleware/__init__.py`

 * *Files identical despite different names*

### Comparing `innovationmerge-1.0.5/innovationmerge/app/routers/__init__.py` & `innovationmerge-1.0.6/innovationmerge/app/routers/__init__.py`

 * *Files identical despite different names*

### Comparing `innovationmerge-1.0.5/innovationmerge/app/routers/authenticate.py` & `innovationmerge-1.0.6/innovationmerge/app/routers/authenticate.py`

 * *Files identical despite different names*

### Comparing `innovationmerge-1.0.5/innovationmerge/app/routers/sample_route.py` & `innovationmerge-1.0.6/innovationmerge/app/routers/sample_route.py`

 * *Files identical despite different names*

### Comparing `innovationmerge-1.0.5/innovationmerge/app/security.py` & `innovationmerge-1.0.6/innovationmerge/app/security.py`

 * *Files identical despite different names*

### Comparing `innovationmerge-1.0.5/innovationmerge/config.py` & `innovationmerge-1.0.6/innovationmerge/config.py`

 * *Files identical despite different names*

### Comparing `innovationmerge-1.0.5/innovationmerge/docs/api_doc.py` & `innovationmerge-1.0.6/innovationmerge/docs/api_doc.py`

 * *Files identical despite different names*

### Comparing `innovationmerge-1.0.5/innovationmerge/src/ai/cpu/object_detection.py` & `innovationmerge-1.0.6/innovationmerge/src/ai/cpu/object_detection.py`

 * *Files identical despite different names*

### Comparing `innovationmerge-1.0.5/innovationmerge/src/utils/responses.py` & `innovationmerge-1.0.6/innovationmerge/src/utils/responses.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,39 @@
 import cv2
 import time
 
+
 def read_image(input_image_path):
     cv2_image = cv2.imread(input_image_path)
     return cv2_image
 
 
 def load_labels(filename):
   with open(filename, 'r') as f:
     return [line.strip() for line in f.readlines()]
 
 
+def draw_detections(detections, cv2_image):
+    for detection in detections.get("detection"):
+       xmin = detection.get("label_bounding_box")[0].get("x")
+       ymin = detection.get("label_bounding_box")[0].get("y")
+       xmax = detection.get("label_bounding_box")[1].get("x")
+       ymax = detection.get("label_bounding_box")[1].get("y")
+       cv2.rectangle(cv2_image, (xmin, ymin), (xmax, ymax), (10, 255, 0), 2)
+        # Draw label
+       object_name = detection["label_class_name"]
+       confidence = detection["confidence"]
+       label = '%s: %d%%' % (object_name, int(confidence*100))
+       labelSize, baseLine = cv2.getTextSize(label, cv2.FONT_HERSHEY_SIMPLEX, 0.7, 2)
+       label_ymin = max(ymin, labelSize[1] + 10)
+       cv2.rectangle(cv2_image, (xmin, label_ymin-labelSize[1]-10), (xmin+labelSize[0], label_ymin+baseLine-10), (255, 255, 255), cv2.FILLED)
+       cv2.putText(cv2_image, label, (xmin, label_ymin-7), cv2.FONT_HERSHEY_SIMPLEX, 0.7, (0, 0, 0), 2)
+    return cv2_image
+
+
 def save_detection_image(detections, cv2_image, output_image_path):
     for detection in detections.get("detection"):
        xmin = detection.get("label_bounding_box")[0].get("x")
        ymin = detection.get("label_bounding_box")[0].get("y")
        xmax = detection.get("label_bounding_box")[1].get("x")
        ymax = detection.get("label_bounding_box")[1].get("y")
        cv2.rectangle(cv2_image, (xmin, ymin), (xmax, ymax), (10, 255, 0), 2)
```

### Comparing `innovationmerge-1.0.5/innovationmerge/tests/sample.py` & `innovationmerge-1.0.6/innovationmerge/tests/sample.py`

 * *Files identical despite different names*

### Comparing `innovationmerge-1.0.5/innovationmerge/tests/test_object_detection.py` & `innovationmerge-1.0.6/innovationmerge/tests/test_object_detection.py`

 * *Files identical despite different names*

### Comparing `innovationmerge-1.0.5/pyproject.toml` & `innovationmerge-1.0.6/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "innovationmerge"
-version = "1.0.5"
+version = "1.0.6"
 description = "innovationmerge core components"
 authors = ["innovationmerge"]
 readme = "README.md"
 packages = [{include = "innovationmerge"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
@@ -16,20 +16,15 @@
 uvicorn = "^0.18.3"
 python-dotenv = "^0.21.0"
 python-json-logger = "^2.0.4"
 requests = "^2.28.1"
 python-jose = "^3.3.0"
 passlib = "^1.7.4"
 bcrypt = "^4.0.0"
-numpy = ">=1.22,<1.24"
-tensorflow-io-gcs-filesystem = "0.31.0"
 opencv-python = "^4.7.0.72"
-tensorflow-cpu = "2.12.0"
-tensorflow = "2.12.0"
-tensorflow-intel = "^2.12.0"
 
 
 [tool.poetry.dev-dependencies]
 pytest = "7.1.3"
 pytest-cov = "3.0.0"
 black = "^22.8.0"
 flake8 = "^5.0.4"
```

### Comparing `innovationmerge-1.0.5/PKG-INFO` & `innovationmerge-1.0.6/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: innovationmerge
-Version: 1.0.5
+Version: 1.0.6
 Summary: innovationmerge core components
 Author: innovationmerge
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -12,26 +12,21 @@
 Provides-Extra: cpu
 Provides-Extra: edge
 Provides-Extra: gpu
 Requires-Dist: aiofiles (>=22.1.0,<23.0.0)
 Requires-Dist: bcrypt (>=4.0.0,<5.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: fastapi (>=0.85.0,<0.86.0)
-Requires-Dist: numpy (>=1.22,<1.24)
 Requires-Dist: opencv-python (>=4.7.0.72,<5.0.0.0)
 Requires-Dist: passlib (>=1.7.4,<2.0.0)
 Requires-Dist: python-dotenv (>=0.21.0,<0.22.0)
 Requires-Dist: python-jose (>=3.3.0,<4.0.0)
 Requires-Dist: python-json-logger (>=2.0.4,<3.0.0)
 Requires-Dist: python-multipart (>=0.0.5,<0.0.6)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
-Requires-Dist: tensorflow (==2.12.0) ; extra == "edge"
-Requires-Dist: tensorflow-cpu (==2.12.0) ; extra == "cpu"
-Requires-Dist: tensorflow-intel (>=2.12.0,<3.0.0) ; extra == "cpu"
-Requires-Dist: tensorflow-io-gcs-filesystem (==0.31.0)
 Requires-Dist: tox (>=3.26.0,<4.0.0)
 Requires-Dist: uvicorn (>=0.18.3,<0.19.0)
 Description-Content-Type: text/markdown
 
 ## About
 - `Author` : innovationmerge
 - `Version`: 1.0
```

