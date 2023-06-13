# Comparing `tmp/pitop.processing-0.31.0.post3.tar.gz` & `tmp/pitop.processing-0.31.0.post4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pitop.processing-0.31.0.post3.tar", last modified: Tue Jun 13 16:41:55 2023, max compression
+gzip compressed data, was "dist/pitop.processing-0.31.0.post4.tar", last modified: Tue Jun 13 18:30:08 2023, max compression
```

## Comparing `pitop.processing-0.31.0.post3.tar` & `pitop.processing-0.31.0.post4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 16:41:55.000000 pitop.processing-0.31.0.post3/
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-13 16:41:37.000000 pitop.processing-0.31.0.post3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      991 2023-06-13 16:41:55.000000 pitop.processing-0.31.0.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      153 2023-06-13 16:41:37.000000 pitop.processing-0.31.0.post3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 16:41:55.000000 pitop.processing-0.31.0.post3/pitop/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 16:41:55.000000 pitop.processing-0.31.0.post3/pitop/processing/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-13 16:41:37.000000 pitop.processing-0.31.0.post3/pitop/processing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 16:41:55.000000 pitop.processing-0.31.0.post3/pitop/processing/algorithms/
--rw-r--r--   0 runner    (1001) docker     (122)       86 2023-06-13 16:41:37.000000 pitop.processing-0.31.0.post3/pitop/processing/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10933 2023-06-13 16:41:37.000000 pitop.processing-0.31.0.post3/pitop/processing/algorithms/ball_detect.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 16:41:55.000000 pitop.processing-0.31.0.post3/pitop/processing/algorithms/faces/
--rw-r--r--   0 runner    (1001) docker     (122)       90 2023-06-13 16:41:37.000000 pitop.processing-0.31.0.post3/pitop/processing/algorithms/faces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 16:41:55.000000 pitop.processing-0.31.0.post3/pitop/processing/algorithms/faces/core/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-13 16:41:37.000000 pitop.processing-0.31.0.post3/pitop/processing/algorithms/faces/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      737 2023-06-13 16:41:37.000000 pitop.processing-0.31.0.post3/pitop/processing/algorithms/faces/core/emotion.py
--rw-r--r--   0 runner    (1001) docker     (122)     3361 2023-06-13 16:41:37.000000 pitop.processing-0.31.0.post3/pitop/processing/algorithms/faces/core/face.py
--rw-r--r--   0 runner    (1001) docker     (122)     7135 2023-06-13 16:41:37.000000 pitop.processing-0.31.0.post3/pitop/processing/algorithms/faces/core/face_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     8777 2023-06-13 16:41:37.000000 pitop.processing-0.31.0.post3/pitop/processing/algorithms/faces/emotion_classifier.py
--rw-r--r--   0 runner    (1001) docker     (122)    10660 2023-06-13 16:41:37.000000 pitop.processing-0.31.0.post3/pitop/processing/algorithms/faces/face_detector.py
--rw-r--r--   0 runner    (1001) docker     (122)     3250 2023-06-13 16:41:37.000000 pitop.processing-0.31.0.post3/pitop/processing/algorithms/line_detect.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 16:41:55.000000 pitop.processing-0.31.0.post3/pitop/processing/core/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-13 16:41:37.000000 pitop.processing-0.31.0.post3/pitop/processing/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3302 2023-06-13 16:41:37.000000 pitop.processing-0.31.0.post3/pitop/processing/core/load_models.py
--rw-r--r--   0 runner    (1001) docker     (122)     1737 2023-06-13 16:41:37.000000 pitop.processing-0.31.0.post3/pitop/processing/core/math_functions.py
--rw-r--r--   0 runner    (1001) docker     (122)     5439 2023-06-13 16:41:37.000000 pitop.processing-0.31.0.post3/pitop/processing/core/vision_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 16:41:55.000000 pitop.processing-0.31.0.post3/pitop.processing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      991 2023-06-13 16:41:55.000000 pitop.processing-0.31.0.post3/pitop.processing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      892 2023-06-13 16:41:55.000000 pitop.processing-0.31.0.post3/pitop.processing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-13 16:41:55.000000 pitop.processing-0.31.0.post3/pitop.processing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      218 2023-06-13 16:41:55.000000 pitop.processing-0.31.0.post3/pitop.processing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-06-13 16:41:55.000000 pitop.processing-0.31.0.post3/pitop.processing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-13 16:41:55.000000 pitop.processing-0.31.0.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2313 2023-06-13 16:41:37.000000 pitop.processing-0.31.0.post3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 18:30:08.000000 pitop.processing-0.31.0.post4/
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-13 18:29:45.000000 pitop.processing-0.31.0.post4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      991 2023-06-13 18:30:08.000000 pitop.processing-0.31.0.post4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      153 2023-06-13 18:29:45.000000 pitop.processing-0.31.0.post4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 18:30:08.000000 pitop.processing-0.31.0.post4/pitop/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 18:30:08.000000 pitop.processing-0.31.0.post4/pitop/processing/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-13 18:29:45.000000 pitop.processing-0.31.0.post4/pitop/processing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 18:30:08.000000 pitop.processing-0.31.0.post4/pitop/processing/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (122)       86 2023-06-13 18:29:45.000000 pitop.processing-0.31.0.post4/pitop/processing/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10933 2023-06-13 18:29:45.000000 pitop.processing-0.31.0.post4/pitop/processing/algorithms/ball_detect.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 18:30:08.000000 pitop.processing-0.31.0.post4/pitop/processing/algorithms/faces/
+-rw-r--r--   0 runner    (1001) docker     (122)       90 2023-06-13 18:29:45.000000 pitop.processing-0.31.0.post4/pitop/processing/algorithms/faces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 18:30:08.000000 pitop.processing-0.31.0.post4/pitop/processing/algorithms/faces/core/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-13 18:29:45.000000 pitop.processing-0.31.0.post4/pitop/processing/algorithms/faces/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      737 2023-06-13 18:29:45.000000 pitop.processing-0.31.0.post4/pitop/processing/algorithms/faces/core/emotion.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3361 2023-06-13 18:29:45.000000 pitop.processing-0.31.0.post4/pitop/processing/algorithms/faces/core/face.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7135 2023-06-13 18:29:45.000000 pitop.processing-0.31.0.post4/pitop/processing/algorithms/faces/core/face_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8777 2023-06-13 18:29:45.000000 pitop.processing-0.31.0.post4/pitop/processing/algorithms/faces/emotion_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10660 2023-06-13 18:29:45.000000 pitop.processing-0.31.0.post4/pitop/processing/algorithms/faces/face_detector.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3250 2023-06-13 18:29:45.000000 pitop.processing-0.31.0.post4/pitop/processing/algorithms/line_detect.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 18:30:08.000000 pitop.processing-0.31.0.post4/pitop/processing/core/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-13 18:29:45.000000 pitop.processing-0.31.0.post4/pitop/processing/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3302 2023-06-13 18:29:45.000000 pitop.processing-0.31.0.post4/pitop/processing/core/load_models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1737 2023-06-13 18:29:45.000000 pitop.processing-0.31.0.post4/pitop/processing/core/math_functions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5439 2023-06-13 18:29:45.000000 pitop.processing-0.31.0.post4/pitop/processing/core/vision_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 18:30:08.000000 pitop.processing-0.31.0.post4/pitop.processing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      991 2023-06-13 18:30:08.000000 pitop.processing-0.31.0.post4/pitop.processing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      892 2023-06-13 18:30:08.000000 pitop.processing-0.31.0.post4/pitop.processing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-13 18:30:08.000000 pitop.processing-0.31.0.post4/pitop.processing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      218 2023-06-13 18:30:08.000000 pitop.processing-0.31.0.post4/pitop.processing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-06-13 18:30:08.000000 pitop.processing-0.31.0.post4/pitop.processing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-13 18:30:08.000000 pitop.processing-0.31.0.post4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2330 2023-06-13 18:29:45.000000 pitop.processing-0.31.0.post4/setup.py
```

### Comparing `pitop.processing-0.31.0.post3/PKG-INFO` & `pitop.processing-0.31.0.post4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pitop.processing
-Version: 0.31.0.post3
+Version: 0.31.0.post4
 Summary: pi-top Python SDK.
 Home-page: https://github.com/pi-top/pi-top-Python-SDK
 Author: pi-top
 Author-email: deb-maintainers@pi-top.com
 License: Apache Software License
 Description: ===========================
         pi-top Python Processing
```

### Comparing `pitop.processing-0.31.0.post3/pitop/processing/algorithms/ball_detect.py` & `pitop.processing-0.31.0.post4/pitop/processing/algorithms/ball_detect.py`

 * *Files identical despite different names*

### Comparing `pitop.processing-0.31.0.post3/pitop/processing/algorithms/faces/core/emotion.py` & `pitop.processing-0.31.0.post4/pitop/processing/algorithms/faces/core/emotion.py`

 * *Files identical despite different names*

### Comparing `pitop.processing-0.31.0.post3/pitop/processing/algorithms/faces/core/face.py` & `pitop.processing-0.31.0.post4/pitop/processing/algorithms/faces/core/face.py`

 * *Files identical despite different names*

### Comparing `pitop.processing-0.31.0.post3/pitop/processing/algorithms/faces/core/face_utils.py` & `pitop.processing-0.31.0.post4/pitop/processing/algorithms/faces/core/face_utils.py`

 * *Files identical despite different names*

### Comparing `pitop.processing-0.31.0.post3/pitop/processing/algorithms/faces/emotion_classifier.py` & `pitop.processing-0.31.0.post4/pitop/processing/algorithms/faces/emotion_classifier.py`

 * *Files identical despite different names*

### Comparing `pitop.processing-0.31.0.post3/pitop/processing/algorithms/faces/face_detector.py` & `pitop.processing-0.31.0.post4/pitop/processing/algorithms/faces/face_detector.py`

 * *Files identical despite different names*

### Comparing `pitop.processing-0.31.0.post3/pitop/processing/algorithms/line_detect.py` & `pitop.processing-0.31.0.post4/pitop/processing/algorithms/line_detect.py`

 * *Files identical despite different names*

### Comparing `pitop.processing-0.31.0.post3/pitop/processing/core/load_models.py` & `pitop.processing-0.31.0.post4/pitop/processing/core/load_models.py`

 * *Files identical despite different names*

### Comparing `pitop.processing-0.31.0.post3/pitop/processing/core/math_functions.py` & `pitop.processing-0.31.0.post4/pitop/processing/core/math_functions.py`

 * *Files identical despite different names*

### Comparing `pitop.processing-0.31.0.post3/pitop/processing/core/vision_functions.py` & `pitop.processing-0.31.0.post4/pitop/processing/core/vision_functions.py`

 * *Files identical despite different names*

### Comparing `pitop.processing-0.31.0.post3/pitop.processing.egg-info/PKG-INFO` & `pitop.processing-0.31.0.post4/pitop.processing.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pitop.processing
-Version: 0.31.0.post3
+Version: 0.31.0.post4
 Summary: pi-top Python SDK.
 Home-page: https://github.com/pi-top/pi-top-Python-SDK
 Author: pi-top
 Author-email: deb-maintainers@pi-top.com
 License: Apache Software License
 Description: ===========================
         pi-top Python Processing
```

### Comparing `pitop.processing-0.31.0.post3/pitop.processing.egg-info/SOURCES.txt` & `pitop.processing-0.31.0.post4/pitop.processing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pitop.processing-0.31.0.post3/setup.py` & `pitop.processing-0.31.0.post4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 if not sys.version_info >= (3, 7):
     raise ValueError("This package requires Python 3.7 or above")
 
 HERE = os.path.abspath(os.path.dirname(__file__))
 
-__version__ = os.environ.get("PYTHON_PACKAGE_VERSION", "0.0.1.dev1")
+__version__ = os.environ.get("PYTHON_PACKAGE_VERSION", "0.0.1.dev1").replace('"', "")
 assert __version__ != ""
 
 __project__ = "pitop.processing"
 __author__ = "pi-top"
 __author_email__ = "deb-maintainers@pi-top.com"
 
 __url__ = "https://github.com/pi-top/pi-top-Python-SDK"
```

