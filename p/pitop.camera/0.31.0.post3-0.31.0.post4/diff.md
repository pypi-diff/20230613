# Comparing `tmp/pitop.camera-0.31.0.post3.tar.gz` & `tmp/pitop.camera-0.31.0.post4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pitop.camera-0.31.0.post3.tar", last modified: Tue Jun 13 16:41:51 2023, max compression
+gzip compressed data, was "dist/pitop.camera-0.31.0.post4.tar", last modified: Tue Jun 13 18:30:05 2023, max compression
```

## Comparing `pitop.camera-0.31.0.post3.tar` & `pitop.camera-0.31.0.post4.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 16:41:51.000000 pitop.camera-0.31.0.post3/
--rw-r--r--   0 runner    (1001) docker     (122)       34 2023-06-13 16:41:37.000000 pitop.camera-0.31.0.post3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      964 2023-06-13 16:41:51.000000 pitop.camera-0.31.0.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      130 2023-06-13 16:41:37.000000 pitop.camera-0.31.0.post3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 16:41:51.000000 pitop.camera-0.31.0.post3/pitop/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 16:41:51.000000 pitop.camera-0.31.0.post3/pitop/camera/
--rw-r--r--   0 runner    (1001) docker     (122)       27 2023-06-13 16:41:37.000000 pitop.camera-0.31.0.post3/pitop/camera/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12221 2023-06-13 16:41:37.000000 pitop.camera-0.31.0.post3/pitop/camera/camera.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 16:41:51.000000 pitop.camera-0.31.0.post3/pitop/camera/camera_calibration/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-13 16:41:37.000000 pitop.camera-0.31.0.post3/pitop/camera/camera_calibration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      331 2023-06-13 16:41:37.000000 pitop.camera-0.31.0.post3/pitop/camera/camera_calibration/camera_cal_dist_pickle_640-480.p
--rw-r--r--   0 runner    (1001) docker     (122)     1184 2023-06-13 16:41:37.000000 pitop.camera-0.31.0.post3/pitop/camera/camera_calibration/load_parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 16:41:51.000000 pitop.camera-0.31.0.post3/pitop/camera/core/
--rw-r--r--   0 runner    (1001) docker     (122)      310 2023-06-13 16:41:37.000000 pitop.camera-0.31.0.post3/pitop/camera/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 16:41:51.000000 pitop.camera-0.31.0.post3/pitop/camera/core/cameras/
--rw-r--r--   0 runner    (1001) docker     (122)      151 2023-06-13 16:41:37.000000 pitop.camera-0.31.0.post3/pitop/camera/core/cameras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      101 2023-06-13 16:41:37.000000 pitop.camera-0.31.0.post3/pitop/camera/core/cameras/camera_types.py
--rw-r--r--   0 runner    (1001) docker     (122)     2623 2023-06-13 16:41:37.000000 pitop.camera-0.31.0.post3/pitop/camera/core/cameras/file_system_camera.py
--rw-r--r--   0 runner    (1001) docker     (122)     3683 2023-06-13 16:41:37.000000 pitop.camera-0.31.0.post3/pitop/camera/core/cameras/usb_camera.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 16:41:51.000000 pitop.camera-0.31.0.post3/pitop/camera/core/capture_actions/
--rw-r--r--   0 runner    (1001) docker     (122)      337 2023-06-13 16:41:37.000000 pitop.camera-0.31.0.post3/pitop/camera/core/capture_actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      750 2023-06-13 16:41:37.000000 pitop.camera-0.31.0.post3/pitop/camera/core/capture_actions/capture_action_base.py
--rw-r--r--   0 runner    (1001) docker     (122)      362 2023-06-13 16:41:37.000000 pitop.camera-0.31.0.post3/pitop/camera/core/capture_actions/capture_actions.py
--rw-r--r--   0 runner    (1001) docker     (122)     1745 2023-06-13 16:41:37.000000 pitop.camera-0.31.0.post3/pitop/camera/core/capture_actions/generic_action.py
--rw-r--r--   0 runner    (1001) docker     (122)     2928 2023-06-13 16:41:37.000000 pitop.camera-0.31.0.post3/pitop/camera/core/capture_actions/motion_detector.py
--rw-r--r--   0 runner    (1001) docker     (122)      619 2023-06-13 16:41:37.000000 pitop.camera-0.31.0.post3/pitop/camera/core/capture_actions/store_frame.py
--rw-r--r--   0 runner    (1001) docker     (122)     1901 2023-06-13 16:41:37.000000 pitop.camera-0.31.0.post3/pitop/camera/core/capture_actions/video_capture.py
--rw-r--r--   0 runner    (1001) docker     (122)     3477 2023-06-13 16:41:37.000000 pitop.camera-0.31.0.post3/pitop/camera/core/frame_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 16:41:51.000000 pitop.camera-0.31.0.post3/pitop.camera.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      964 2023-06-13 16:41:51.000000 pitop.camera-0.31.0.post3/pitop.camera.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1012 2023-06-13 16:41:51.000000 pitop.camera-0.31.0.post3/pitop.camera.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-13 16:41:51.000000 pitop.camera-0.31.0.post3/pitop.camera.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      182 2023-06-13 16:41:51.000000 pitop.camera-0.31.0.post3/pitop.camera.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-06-13 16:41:51.000000 pitop.camera-0.31.0.post3/pitop.camera.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-13 16:41:51.000000 pitop.camera-0.31.0.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2159 2023-06-13 16:41:37.000000 pitop.camera-0.31.0.post3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 18:30:05.000000 pitop.camera-0.31.0.post4/
+-rw-r--r--   0 runner    (1001) docker     (122)       34 2023-06-13 18:29:44.000000 pitop.camera-0.31.0.post4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      964 2023-06-13 18:30:05.000000 pitop.camera-0.31.0.post4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      130 2023-06-13 18:29:44.000000 pitop.camera-0.31.0.post4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 18:30:05.000000 pitop.camera-0.31.0.post4/pitop/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 18:30:05.000000 pitop.camera-0.31.0.post4/pitop/camera/
+-rw-r--r--   0 runner    (1001) docker     (122)       27 2023-06-13 18:29:44.000000 pitop.camera-0.31.0.post4/pitop/camera/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12221 2023-06-13 18:29:44.000000 pitop.camera-0.31.0.post4/pitop/camera/camera.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 18:30:05.000000 pitop.camera-0.31.0.post4/pitop/camera/camera_calibration/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-13 18:29:44.000000 pitop.camera-0.31.0.post4/pitop/camera/camera_calibration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      331 2023-06-13 18:29:44.000000 pitop.camera-0.31.0.post4/pitop/camera/camera_calibration/camera_cal_dist_pickle_640-480.p
+-rw-r--r--   0 runner    (1001) docker     (122)     1184 2023-06-13 18:29:44.000000 pitop.camera-0.31.0.post4/pitop/camera/camera_calibration/load_parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 18:30:05.000000 pitop.camera-0.31.0.post4/pitop/camera/core/
+-rw-r--r--   0 runner    (1001) docker     (122)      310 2023-06-13 18:29:44.000000 pitop.camera-0.31.0.post4/pitop/camera/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 18:30:05.000000 pitop.camera-0.31.0.post4/pitop/camera/core/cameras/
+-rw-r--r--   0 runner    (1001) docker     (122)      151 2023-06-13 18:29:44.000000 pitop.camera-0.31.0.post4/pitop/camera/core/cameras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      101 2023-06-13 18:29:44.000000 pitop.camera-0.31.0.post4/pitop/camera/core/cameras/camera_types.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2623 2023-06-13 18:29:44.000000 pitop.camera-0.31.0.post4/pitop/camera/core/cameras/file_system_camera.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3683 2023-06-13 18:29:44.000000 pitop.camera-0.31.0.post4/pitop/camera/core/cameras/usb_camera.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 18:30:05.000000 pitop.camera-0.31.0.post4/pitop/camera/core/capture_actions/
+-rw-r--r--   0 runner    (1001) docker     (122)      337 2023-06-13 18:29:44.000000 pitop.camera-0.31.0.post4/pitop/camera/core/capture_actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      750 2023-06-13 18:29:44.000000 pitop.camera-0.31.0.post4/pitop/camera/core/capture_actions/capture_action_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)      362 2023-06-13 18:29:44.000000 pitop.camera-0.31.0.post4/pitop/camera/core/capture_actions/capture_actions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1745 2023-06-13 18:29:44.000000 pitop.camera-0.31.0.post4/pitop/camera/core/capture_actions/generic_action.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2928 2023-06-13 18:29:44.000000 pitop.camera-0.31.0.post4/pitop/camera/core/capture_actions/motion_detector.py
+-rw-r--r--   0 runner    (1001) docker     (122)      619 2023-06-13 18:29:44.000000 pitop.camera-0.31.0.post4/pitop/camera/core/capture_actions/store_frame.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1901 2023-06-13 18:29:44.000000 pitop.camera-0.31.0.post4/pitop/camera/core/capture_actions/video_capture.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3477 2023-06-13 18:29:44.000000 pitop.camera-0.31.0.post4/pitop/camera/core/frame_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 18:30:05.000000 pitop.camera-0.31.0.post4/pitop.camera.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      964 2023-06-13 18:30:05.000000 pitop.camera-0.31.0.post4/pitop.camera.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1012 2023-06-13 18:30:05.000000 pitop.camera-0.31.0.post4/pitop.camera.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-13 18:30:05.000000 pitop.camera-0.31.0.post4/pitop.camera.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      182 2023-06-13 18:30:05.000000 pitop.camera-0.31.0.post4/pitop.camera.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-06-13 18:30:05.000000 pitop.camera-0.31.0.post4/pitop.camera.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-13 18:30:05.000000 pitop.camera-0.31.0.post4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2176 2023-06-13 18:29:44.000000 pitop.camera-0.31.0.post4/setup.py
```

### Comparing `pitop.camera-0.31.0.post3/PKG-INFO` & `pitop.camera-0.31.0.post4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pitop.camera
-Version: 0.31.0.post3
+Version: 0.31.0.post4
 Summary: pi-top Python SDK.
 Home-page: https://github.com/pi-top/pi-top-Python-SDK
 Author: pi-top
 Author-email: deb-maintainers@pi-top.com
 License: Apache Software License
 Description: ===========================
         pi-top Python Camera
```

### Comparing `pitop.camera-0.31.0.post3/pitop/camera/camera.py` & `pitop.camera-0.31.0.post4/pitop/camera/camera.py`

 * *Files identical despite different names*

### Comparing `pitop.camera-0.31.0.post3/pitop/camera/camera_calibration/load_parameters.py` & `pitop.camera-0.31.0.post4/pitop/camera/camera_calibration/load_parameters.py`

 * *Files identical despite different names*

### Comparing `pitop.camera-0.31.0.post3/pitop/camera/core/cameras/file_system_camera.py` & `pitop.camera-0.31.0.post4/pitop/camera/core/cameras/file_system_camera.py`

 * *Files identical despite different names*

### Comparing `pitop.camera-0.31.0.post3/pitop/camera/core/cameras/usb_camera.py` & `pitop.camera-0.31.0.post4/pitop/camera/core/cameras/usb_camera.py`

 * *Files identical despite different names*

### Comparing `pitop.camera-0.31.0.post3/pitop/camera/core/capture_actions/capture_action_base.py` & `pitop.camera-0.31.0.post4/pitop/camera/core/capture_actions/capture_action_base.py`

 * *Files identical despite different names*

### Comparing `pitop.camera-0.31.0.post3/pitop/camera/core/capture_actions/generic_action.py` & `pitop.camera-0.31.0.post4/pitop/camera/core/capture_actions/generic_action.py`

 * *Files identical despite different names*

### Comparing `pitop.camera-0.31.0.post3/pitop/camera/core/capture_actions/motion_detector.py` & `pitop.camera-0.31.0.post4/pitop/camera/core/capture_actions/motion_detector.py`

 * *Files identical despite different names*

### Comparing `pitop.camera-0.31.0.post3/pitop/camera/core/capture_actions/store_frame.py` & `pitop.camera-0.31.0.post4/pitop/camera/core/capture_actions/store_frame.py`

 * *Files identical despite different names*

### Comparing `pitop.camera-0.31.0.post3/pitop/camera/core/capture_actions/video_capture.py` & `pitop.camera-0.31.0.post4/pitop/camera/core/capture_actions/video_capture.py`

 * *Files identical despite different names*

### Comparing `pitop.camera-0.31.0.post3/pitop/camera/core/frame_handler.py` & `pitop.camera-0.31.0.post4/pitop/camera/core/frame_handler.py`

 * *Files identical despite different names*

### Comparing `pitop.camera-0.31.0.post3/pitop.camera.egg-info/PKG-INFO` & `pitop.camera-0.31.0.post4/pitop.camera.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pitop.camera
-Version: 0.31.0.post3
+Version: 0.31.0.post4
 Summary: pi-top Python SDK.
 Home-page: https://github.com/pi-top/pi-top-Python-SDK
 Author: pi-top
 Author-email: deb-maintainers@pi-top.com
 License: Apache Software License
 Description: ===========================
         pi-top Python Camera
```

### Comparing `pitop.camera-0.31.0.post3/pitop.camera.egg-info/SOURCES.txt` & `pitop.camera-0.31.0.post4/pitop.camera.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pitop.camera-0.31.0.post3/setup.py` & `pitop.camera-0.31.0.post4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 if not sys.version_info >= (3, 7):
     raise ValueError("This package requires Python 3.7 or above")
 
 HERE = os.path.abspath(os.path.dirname(__file__))
 
-__version__ = os.environ.get("PYTHON_PACKAGE_VERSION", "0.0.1.dev1")
+__version__ = os.environ.get("PYTHON_PACKAGE_VERSION", "0.0.1.dev1").replace('"', "")
 assert __version__ != ""
 
 __project__ = "pitop.camera"
 __author__ = "pi-top"
 __author_email__ = "deb-maintainers@pi-top.com"
 
 __url__ = "https://github.com/pi-top/pi-top-Python-SDK"
```

