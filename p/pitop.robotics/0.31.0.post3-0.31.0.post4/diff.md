# Comparing `tmp/pitop.robotics-0.31.0.post3.tar.gz` & `tmp/pitop.robotics-0.31.0.post4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pitop.robotics-0.31.0.post3.tar", last modified: Tue Jun 13 16:41:55 2023, max compression
+gzip compressed data, was "dist/pitop.robotics-0.31.0.post4.tar", last modified: Tue Jun 13 18:30:09 2023, max compression
```

## Comparing `pitop.robotics-0.31.0.post3.tar` & `pitop.robotics-0.31.0.post4.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 16:41:55.000000 pitop.robotics-0.31.0.post3/
--rw-r--r--   0 runner    (1001) docker     (122)       36 2023-06-13 16:41:37.000000 pitop.robotics-0.31.0.post3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      977 2023-06-13 16:41:55.000000 pitop.robotics-0.31.0.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      141 2023-06-13 16:41:37.000000 pitop.robotics-0.31.0.post3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 16:41:55.000000 pitop.robotics-0.31.0.post3/pitop/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 16:41:55.000000 pitop.robotics-0.31.0.post3/pitop/robotics/
--rw-r--r--   0 runner    (1001) docker     (122)      384 2023-06-13 16:41:37.000000 pitop.robotics-0.31.0.post3/pitop/robotics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1096 2023-06-13 16:41:37.000000 pitop.robotics-0.31.0.post3/pitop/robotics/blockpi_rover.py
--rw-r--r--   0 runner    (1001) docker     (122)     2181 2023-06-13 16:41:37.000000 pitop.robotics-0.31.0.post3/pitop/robotics/configurations.py
--rw-r--r--   0 runner    (1001) docker     (122)     8112 2023-06-13 16:41:37.000000 pitop.robotics-0.31.0.post3/pitop/robotics/drive_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 16:41:55.000000 pitop.robotics-0.31.0.post3/pitop/robotics/filterpy/
--rw-r--r--   0 runner    (1001) docker     (122)     1084 2023-06-13 16:41:37.000000 pitop.robotics-0.31.0.post3/pitop/robotics/filterpy/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-13 16:41:37.000000 pitop.robotics-0.31.0.post3/pitop/robotics/filterpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1529 2023-06-13 16:41:37.000000 pitop.robotics-0.31.0.post3/pitop/robotics/filterpy/common.py
--rw-r--r--   0 runner    (1001) docker     (122)    40171 2023-06-13 16:41:37.000000 pitop.robotics-0.31.0.post3/pitop/robotics/filterpy/kalman.py
--rw-r--r--   0 runner    (1001) docker     (122)     1521 2023-06-13 16:41:37.000000 pitop.robotics-0.31.0.post3/pitop/robotics/filterpy/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 16:41:55.000000 pitop.robotics-0.31.0.post3/pitop/robotics/json/
--rw-r--r--   0 runner    (1001) docker     (122)      130 2023-06-13 16:41:37.000000 pitop.robotics-0.31.0.post3/pitop/robotics/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1262 2023-06-13 16:41:37.000000 pitop.robotics-0.31.0.post3/pitop/robotics/json/alex.json
--rw-r--r--   0 runner    (1001) docker     (122)     1567 2023-06-13 16:41:37.000000 pitop.robotics-0.31.0.post3/pitop/robotics/json/bobbie.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 16:41:55.000000 pitop.robotics-0.31.0.post3/pitop/robotics/navigation/
--rw-r--r--   0 runner    (1001) docker     (122)       56 2023-06-13 16:41:37.000000 pitop.robotics-0.31.0.post3/pitop/robotics/navigation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 16:41:55.000000 pitop.robotics-0.31.0.post3/pitop/robotics/navigation/core/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-13 16:41:37.000000 pitop.robotics-0.31.0.post3/pitop/robotics/navigation/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2690 2023-06-13 16:41:37.000000 pitop.robotics-0.31.0.post3/pitop/robotics/navigation/core/driving_manager.py
--rw-r--r--   0 runner    (1001) docker     (122)     1860 2023-06-13 16:41:37.000000 pitop.robotics-0.31.0.post3/pitop/robotics/navigation/core/goal_criteria.py
--rw-r--r--   0 runner    (1001) docker     (122)     1853 2023-06-13 16:41:37.000000 pitop.robotics-0.31.0.post3/pitop/robotics/navigation/core/measurement_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (122)     9443 2023-06-13 16:41:37.000000 pitop.robotics-0.31.0.post3/pitop/robotics/navigation/core/robot_state.py
--rw-r--r--   0 runner    (1001) docker     (122)     1111 2023-06-13 16:41:37.000000 pitop.robotics-0.31.0.post3/pitop/robotics/navigation/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     9014 2023-06-13 16:41:37.000000 pitop.robotics-0.31.0.post3/pitop/robotics/navigation/navigation_controller.py
--rw-r--r--   0 runner    (1001) docker     (122)     6937 2023-06-13 16:41:37.000000 pitop.robotics-0.31.0.post3/pitop/robotics/navigation/navigator.py
--rw-r--r--   0 runner    (1001) docker     (122)     2464 2023-06-13 16:41:37.000000 pitop.robotics-0.31.0.post3/pitop/robotics/pan_tilt_controller.py
--rw-r--r--   0 runner    (1001) docker     (122)     2131 2023-06-13 16:41:37.000000 pitop.robotics-0.31.0.post3/pitop/robotics/pan_tilt_object_tracker.py
--rw-r--r--   0 runner    (1001) docker     (122)     3313 2023-06-13 16:41:37.000000 pitop.robotics-0.31.0.post3/pitop/robotics/pincer_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 16:41:55.000000 pitop.robotics-0.31.0.post3/pitop/robotics/simple_pid/
--rw-r--r--   0 runner    (1001) docker     (122)     1077 2023-06-13 16:41:37.000000 pitop.robotics-0.31.0.post3/pitop/robotics/simple_pid/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (122)     9360 2023-06-13 16:41:37.000000 pitop.robotics-0.31.0.post3/pitop/robotics/simple_pid/PID.py
--rw-r--r--   0 runner    (1001) docker     (122)     1614 2023-06-13 16:41:37.000000 pitop.robotics-0.31.0.post3/pitop/robotics/simple_pid/PID.pyi
--rw-r--r--   0 runner    (1001) docker     (122)      107 2023-06-13 16:41:37.000000 pitop.robotics-0.31.0.post3/pitop/robotics/simple_pid/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       21 2023-06-13 16:41:37.000000 pitop.robotics-0.31.0.post3/pitop/robotics/simple_pid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-13 16:41:37.000000 pitop.robotics-0.31.0.post3/pitop/robotics/simple_pid/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)     7933 2023-06-13 16:41:37.000000 pitop.robotics-0.31.0.post3/pitop/robotics/tilt_roll_head_controller.py
--rw-r--r--   0 runner    (1001) docker     (122)     4550 2023-06-13 16:41:37.000000 pitop.robotics-0.31.0.post3/pitop/robotics/two_servo_assembly_calibrator.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 16:41:55.000000 pitop.robotics-0.31.0.post3/pitop.robotics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      977 2023-06-13 16:41:55.000000 pitop.robotics-0.31.0.post3/pitop.robotics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1445 2023-06-13 16:41:55.000000 pitop.robotics-0.31.0.post3/pitop.robotics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-13 16:41:55.000000 pitop.robotics-0.31.0.post3/pitop.robotics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      104 2023-06-13 16:41:55.000000 pitop.robotics-0.31.0.post3/pitop.robotics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-06-13 16:41:55.000000 pitop.robotics-0.31.0.post3/pitop.robotics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-13 16:41:55.000000 pitop.robotics-0.31.0.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2058 2023-06-13 16:41:37.000000 pitop.robotics-0.31.0.post3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 18:30:09.000000 pitop.robotics-0.31.0.post4/
+-rw-r--r--   0 runner    (1001) docker     (122)       36 2023-06-13 18:29:45.000000 pitop.robotics-0.31.0.post4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      977 2023-06-13 18:30:09.000000 pitop.robotics-0.31.0.post4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      141 2023-06-13 18:29:45.000000 pitop.robotics-0.31.0.post4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 18:30:09.000000 pitop.robotics-0.31.0.post4/pitop/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 18:30:09.000000 pitop.robotics-0.31.0.post4/pitop/robotics/
+-rw-r--r--   0 runner    (1001) docker     (122)      384 2023-06-13 18:29:45.000000 pitop.robotics-0.31.0.post4/pitop/robotics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1096 2023-06-13 18:29:45.000000 pitop.robotics-0.31.0.post4/pitop/robotics/blockpi_rover.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2181 2023-06-13 18:29:45.000000 pitop.robotics-0.31.0.post4/pitop/robotics/configurations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8112 2023-06-13 18:29:45.000000 pitop.robotics-0.31.0.post4/pitop/robotics/drive_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 18:30:09.000000 pitop.robotics-0.31.0.post4/pitop/robotics/filterpy/
+-rw-r--r--   0 runner    (1001) docker     (122)     1084 2023-06-13 18:29:45.000000 pitop.robotics-0.31.0.post4/pitop/robotics/filterpy/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-13 18:29:45.000000 pitop.robotics-0.31.0.post4/pitop/robotics/filterpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1529 2023-06-13 18:29:45.000000 pitop.robotics-0.31.0.post4/pitop/robotics/filterpy/common.py
+-rw-r--r--   0 runner    (1001) docker     (122)    40171 2023-06-13 18:29:45.000000 pitop.robotics-0.31.0.post4/pitop/robotics/filterpy/kalman.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1521 2023-06-13 18:29:45.000000 pitop.robotics-0.31.0.post4/pitop/robotics/filterpy/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 18:30:09.000000 pitop.robotics-0.31.0.post4/pitop/robotics/json/
+-rw-r--r--   0 runner    (1001) docker     (122)      130 2023-06-13 18:29:45.000000 pitop.robotics-0.31.0.post4/pitop/robotics/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1262 2023-06-13 18:29:45.000000 pitop.robotics-0.31.0.post4/pitop/robotics/json/alex.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1567 2023-06-13 18:29:45.000000 pitop.robotics-0.31.0.post4/pitop/robotics/json/bobbie.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 18:30:09.000000 pitop.robotics-0.31.0.post4/pitop/robotics/navigation/
+-rw-r--r--   0 runner    (1001) docker     (122)       56 2023-06-13 18:29:45.000000 pitop.robotics-0.31.0.post4/pitop/robotics/navigation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 18:30:09.000000 pitop.robotics-0.31.0.post4/pitop/robotics/navigation/core/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-13 18:29:45.000000 pitop.robotics-0.31.0.post4/pitop/robotics/navigation/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2690 2023-06-13 18:29:45.000000 pitop.robotics-0.31.0.post4/pitop/robotics/navigation/core/driving_manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1860 2023-06-13 18:29:45.000000 pitop.robotics-0.31.0.post4/pitop/robotics/navigation/core/goal_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1853 2023-06-13 18:29:45.000000 pitop.robotics-0.31.0.post4/pitop/robotics/navigation/core/measurement_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9443 2023-06-13 18:29:45.000000 pitop.robotics-0.31.0.post4/pitop/robotics/navigation/core/robot_state.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1111 2023-06-13 18:29:45.000000 pitop.robotics-0.31.0.post4/pitop/robotics/navigation/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9014 2023-06-13 18:29:45.000000 pitop.robotics-0.31.0.post4/pitop/robotics/navigation/navigation_controller.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6937 2023-06-13 18:29:45.000000 pitop.robotics-0.31.0.post4/pitop/robotics/navigation/navigator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2464 2023-06-13 18:29:45.000000 pitop.robotics-0.31.0.post4/pitop/robotics/pan_tilt_controller.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2131 2023-06-13 18:29:45.000000 pitop.robotics-0.31.0.post4/pitop/robotics/pan_tilt_object_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3313 2023-06-13 18:29:45.000000 pitop.robotics-0.31.0.post4/pitop/robotics/pincer_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 18:30:09.000000 pitop.robotics-0.31.0.post4/pitop/robotics/simple_pid/
+-rw-r--r--   0 runner    (1001) docker     (122)     1077 2023-06-13 18:29:45.000000 pitop.robotics-0.31.0.post4/pitop/robotics/simple_pid/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (122)     9360 2023-06-13 18:29:45.000000 pitop.robotics-0.31.0.post4/pitop/robotics/simple_pid/PID.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1614 2023-06-13 18:29:45.000000 pitop.robotics-0.31.0.post4/pitop/robotics/simple_pid/PID.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)      107 2023-06-13 18:29:45.000000 pitop.robotics-0.31.0.post4/pitop/robotics/simple_pid/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       21 2023-06-13 18:29:45.000000 pitop.robotics-0.31.0.post4/pitop/robotics/simple_pid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-13 18:29:45.000000 pitop.robotics-0.31.0.post4/pitop/robotics/simple_pid/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)     7933 2023-06-13 18:29:45.000000 pitop.robotics-0.31.0.post4/pitop/robotics/tilt_roll_head_controller.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4550 2023-06-13 18:29:45.000000 pitop.robotics-0.31.0.post4/pitop/robotics/two_servo_assembly_calibrator.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 18:30:09.000000 pitop.robotics-0.31.0.post4/pitop.robotics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      977 2023-06-13 18:30:09.000000 pitop.robotics-0.31.0.post4/pitop.robotics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1445 2023-06-13 18:30:09.000000 pitop.robotics-0.31.0.post4/pitop.robotics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-13 18:30:09.000000 pitop.robotics-0.31.0.post4/pitop.robotics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      104 2023-06-13 18:30:09.000000 pitop.robotics-0.31.0.post4/pitop.robotics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-06-13 18:30:09.000000 pitop.robotics-0.31.0.post4/pitop.robotics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-13 18:30:09.000000 pitop.robotics-0.31.0.post4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2075 2023-06-13 18:29:45.000000 pitop.robotics-0.31.0.post4/setup.py
```

### Comparing `pitop.robotics-0.31.0.post3/PKG-INFO` & `pitop.robotics-0.31.0.post4/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pitop.robotics
-Version: 0.31.0.post3
+Version: 0.31.0.post4
 Summary: pi-top Python SDK.
 Home-page: https://github.com/pi-top/pi-top-Python-SDK
 Author: pi-top
 Author-email: deb-maintainers@pi-top.com
 License: Apache Software License
 Description: ===========================
         pi-top Python Robotics
```

### Comparing `pitop.robotics-0.31.0.post3/pitop/robotics/blockpi_rover.py` & `pitop.robotics-0.31.0.post4/pitop/robotics/blockpi_rover.py`

 * *Files identical despite different names*

### Comparing `pitop.robotics-0.31.0.post3/pitop/robotics/configurations.py` & `pitop.robotics-0.31.0.post4/pitop/robotics/configurations.py`

 * *Files identical despite different names*

### Comparing `pitop.robotics-0.31.0.post3/pitop/robotics/drive_controller.py` & `pitop.robotics-0.31.0.post4/pitop/robotics/drive_controller.py`

 * *Files identical despite different names*

### Comparing `pitop.robotics-0.31.0.post3/pitop/robotics/filterpy/LICENSE.md` & `pitop.robotics-0.31.0.post4/pitop/robotics/filterpy/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pitop.robotics-0.31.0.post3/pitop/robotics/filterpy/common.py` & `pitop.robotics-0.31.0.post4/pitop/robotics/filterpy/common.py`

 * *Files identical despite different names*

### Comparing `pitop.robotics-0.31.0.post3/pitop/robotics/filterpy/kalman.py` & `pitop.robotics-0.31.0.post4/pitop/robotics/filterpy/kalman.py`

 * *Files identical despite different names*

### Comparing `pitop.robotics-0.31.0.post3/pitop/robotics/filterpy/stats.py` & `pitop.robotics-0.31.0.post4/pitop/robotics/filterpy/stats.py`

 * *Files identical despite different names*

### Comparing `pitop.robotics-0.31.0.post3/pitop/robotics/json/alex.json` & `pitop.robotics-0.31.0.post4/pitop/robotics/json/alex.json`

 * *Files identical despite different names*

### Comparing `pitop.robotics-0.31.0.post3/pitop/robotics/json/bobbie.json` & `pitop.robotics-0.31.0.post4/pitop/robotics/json/bobbie.json`

 * *Files identical despite different names*

### Comparing `pitop.robotics-0.31.0.post3/pitop/robotics/navigation/core/driving_manager.py` & `pitop.robotics-0.31.0.post4/pitop/robotics/navigation/core/driving_manager.py`

 * *Files identical despite different names*

### Comparing `pitop.robotics-0.31.0.post3/pitop/robotics/navigation/core/goal_criteria.py` & `pitop.robotics-0.31.0.post4/pitop/robotics/navigation/core/goal_criteria.py`

 * *Files identical despite different names*

### Comparing `pitop.robotics-0.31.0.post3/pitop/robotics/navigation/core/measurement_scheduler.py` & `pitop.robotics-0.31.0.post4/pitop/robotics/navigation/core/measurement_scheduler.py`

 * *Files identical despite different names*

### Comparing `pitop.robotics-0.31.0.post3/pitop/robotics/navigation/core/robot_state.py` & `pitop.robotics-0.31.0.post4/pitop/robotics/navigation/core/robot_state.py`

 * *Files identical despite different names*

### Comparing `pitop.robotics-0.31.0.post3/pitop/robotics/navigation/core/utils.py` & `pitop.robotics-0.31.0.post4/pitop/robotics/navigation/core/utils.py`

 * *Files identical despite different names*

### Comparing `pitop.robotics-0.31.0.post3/pitop/robotics/navigation/navigation_controller.py` & `pitop.robotics-0.31.0.post4/pitop/robotics/navigation/navigation_controller.py`

 * *Files identical despite different names*

### Comparing `pitop.robotics-0.31.0.post3/pitop/robotics/navigation/navigator.py` & `pitop.robotics-0.31.0.post4/pitop/robotics/navigation/navigator.py`

 * *Files identical despite different names*

### Comparing `pitop.robotics-0.31.0.post3/pitop/robotics/pan_tilt_controller.py` & `pitop.robotics-0.31.0.post4/pitop/robotics/pan_tilt_controller.py`

 * *Files identical despite different names*

### Comparing `pitop.robotics-0.31.0.post3/pitop/robotics/pan_tilt_object_tracker.py` & `pitop.robotics-0.31.0.post4/pitop/robotics/pan_tilt_object_tracker.py`

 * *Files identical despite different names*

### Comparing `pitop.robotics-0.31.0.post3/pitop/robotics/pincer_controller.py` & `pitop.robotics-0.31.0.post4/pitop/robotics/pincer_controller.py`

 * *Files identical despite different names*

### Comparing `pitop.robotics-0.31.0.post3/pitop/robotics/simple_pid/LICENSE.md` & `pitop.robotics-0.31.0.post4/pitop/robotics/simple_pid/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pitop.robotics-0.31.0.post3/pitop/robotics/simple_pid/PID.py` & `pitop.robotics-0.31.0.post4/pitop/robotics/simple_pid/PID.py`

 * *Files identical despite different names*

### Comparing `pitop.robotics-0.31.0.post3/pitop/robotics/simple_pid/PID.pyi` & `pitop.robotics-0.31.0.post4/pitop/robotics/simple_pid/PID.pyi`

 * *Files identical despite different names*

### Comparing `pitop.robotics-0.31.0.post3/pitop/robotics/tilt_roll_head_controller.py` & `pitop.robotics-0.31.0.post4/pitop/robotics/tilt_roll_head_controller.py`

 * *Files identical despite different names*

### Comparing `pitop.robotics-0.31.0.post3/pitop/robotics/two_servo_assembly_calibrator.py` & `pitop.robotics-0.31.0.post4/pitop/robotics/two_servo_assembly_calibrator.py`

 * *Files identical despite different names*

### Comparing `pitop.robotics-0.31.0.post3/pitop.robotics.egg-info/PKG-INFO` & `pitop.robotics-0.31.0.post4/pitop.robotics.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pitop.robotics
-Version: 0.31.0.post3
+Version: 0.31.0.post4
 Summary: pi-top Python SDK.
 Home-page: https://github.com/pi-top/pi-top-Python-SDK
 Author: pi-top
 Author-email: deb-maintainers@pi-top.com
 License: Apache Software License
 Description: ===========================
         pi-top Python Robotics
```

### Comparing `pitop.robotics-0.31.0.post3/pitop.robotics.egg-info/SOURCES.txt` & `pitop.robotics-0.31.0.post4/pitop.robotics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pitop.robotics-0.31.0.post3/setup.py` & `pitop.robotics-0.31.0.post4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 if not sys.version_info >= (3, 7):
     raise ValueError("This package requires Python 3.7 or above")
 
 HERE = os.path.abspath(os.path.dirname(__file__))
 
-__version__ = os.environ.get("PYTHON_PACKAGE_VERSION", "0.0.1.dev1")
+__version__ = os.environ.get("PYTHON_PACKAGE_VERSION", "0.0.1.dev1").replace('"', "")
 assert __version__ != ""
 
 __project__ = "pitop.robotics"
 __author__ = "pi-top"
 __author_email__ = "deb-maintainers@pi-top.com"
 
 __url__ = "https://github.com/pi-top/pi-top-Python-SDK"
```

