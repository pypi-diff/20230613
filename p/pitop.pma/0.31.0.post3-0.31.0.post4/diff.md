# Comparing `tmp/pitop.pma-0.31.0.post3.tar.gz` & `tmp/pitop.pma-0.31.0.post4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pitop.pma-0.31.0.post3.tar", last modified: Tue Jun 13 16:41:54 2023, max compression
+gzip compressed data, was "dist/pitop.pma-0.31.0.post4.tar", last modified: Tue Jun 13 18:30:08 2023, max compression
```

## Comparing `pitop.pma-0.31.0.post3.tar` & `pitop.pma-0.31.0.post4.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 16:41:54.000000 pitop.pma-0.31.0.post3/
--rw-r--r--   0 runner    (1001) docker     (122)       31 2023-06-13 16:41:37.000000 pitop.pma-0.31.0.post3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1014 2023-06-13 16:41:54.000000 pitop.pma-0.31.0.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      175 2023-06-13 16:41:37.000000 pitop.pma-0.31.0.post3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 16:41:54.000000 pitop.pma-0.31.0.post3/pitop/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 16:41:54.000000 pitop.pma-0.31.0.post3/pitop/pma/
--rw-r--r--   0 runner    (1001) docker     (122)      540 2023-06-13 16:41:37.000000 pitop.pma-0.31.0.post3/pitop/pma/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2953 2023-06-13 16:41:37.000000 pitop.pma-0.31.0.post3/pitop/pma/adc_base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2551 2023-06-13 16:41:37.000000 pitop.pma-0.31.0.post3/pitop/pma/button.py
--rw-r--r--   0 runner    (1001) docker     (122)     2458 2023-06-13 16:41:37.000000 pitop.pma-0.31.0.post3/pitop/pma/buzzer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 16:41:54.000000 pitop.pma-0.31.0.post3/pitop/pma/common/
--rw-r--r--   0 runner    (1001) docker     (122)       48 2023-06-13 16:41:37.000000 pitop.pma-0.31.0.post3/pitop/pma/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1893 2023-06-13 16:41:37.000000 pitop.pma-0.31.0.post3/pitop/pma/common/encoder_motor_registers.py
--rw-r--r--   0 runner    (1001) docker     (122)     1954 2023-06-13 16:41:37.000000 pitop.pma-0.31.0.post3/pitop/pma/common/imu_registers.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 16:41:54.000000 pitop.pma-0.31.0.post3/pitop/pma/common/math_functions/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-13 16:41:37.000000 pitop.pma-0.31.0.post3/pitop/pma/common/math_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3746 2023-06-13 16:41:37.000000 pitop.pma-0.31.0.post3/pitop/pma/common/math_functions/ellipsoid_functions.py
--rw-r--r--   0 runner    (1001) docker     (122)      169 2023-06-13 16:41:37.000000 pitop.pma-0.31.0.post3/pitop/pma/common/plate_registers.py
--rw-r--r--   0 runner    (1001) docker     (122)      926 2023-06-13 16:41:37.000000 pitop.pma-0.31.0.post3/pitop/pma/common/servo_motor_registers.py
--rw-r--r--   0 runner    (1001) docker     (122)      404 2023-06-13 16:41:37.000000 pitop.pma-0.31.0.post3/pitop/pma/common/ultrasonic_registers.py
--rw-r--r--   0 runner    (1001) docker     (122)     1781 2023-06-13 16:41:37.000000 pitop.pma-0.31.0.post3/pitop/pma/common/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    17224 2023-06-13 16:41:37.000000 pitop.pma-0.31.0.post3/pitop/pma/encoder_motor.py
--rw-r--r--   0 runner    (1001) docker     (122)     6086 2023-06-13 16:41:37.000000 pitop.pma-0.31.0.post3/pitop/pma/encoder_motor_controller.py
--rw-r--r--   0 runner    (1001) docker     (122)     4934 2023-06-13 16:41:37.000000 pitop.pma-0.31.0.post3/pitop/pma/imu.py
--rw-r--r--   0 runner    (1001) docker     (122)    10278 2023-06-13 16:41:37.000000 pitop.pma-0.31.0.post3/pitop/pma/imu_controller.py
--rw-r--r--   0 runner    (1001) docker     (122)     2643 2023-06-13 16:41:37.000000 pitop.pma-0.31.0.post3/pitop/pma/led.py
--rw-r--r--   0 runner    (1001) docker     (122)     2134 2023-06-13 16:41:37.000000 pitop.pma-0.31.0.post3/pitop/pma/light_sensor.py
--rw-r--r--   0 runner    (1001) docker     (122)      301 2023-06-13 16:41:37.000000 pitop.pma-0.31.0.post3/pitop/pma/parameters.py
--rw-r--r--   0 runner    (1001) docker     (122)     2586 2023-06-13 16:41:37.000000 pitop.pma-0.31.0.post3/pitop/pma/plate_interface.py
--rw-r--r--   0 runner    (1001) docker     (122)     2028 2023-06-13 16:41:37.000000 pitop.pma-0.31.0.post3/pitop/pma/potentiometer.py
--rw-r--r--   0 runner    (1001) docker     (122)     4953 2023-06-13 16:41:37.000000 pitop.pma-0.31.0.post3/pitop/pma/servo_controller.py
--rw-r--r--   0 runner    (1001) docker     (122)    10704 2023-06-13 16:41:37.000000 pitop.pma-0.31.0.post3/pitop/pma/servo_motor.py
--rw-r--r--   0 runner    (1001) docker     (122)     1888 2023-06-13 16:41:37.000000 pitop.pma-0.31.0.post3/pitop/pma/sound_sensor.py
--rw-r--r--   0 runner    (1001) docker     (122)     6078 2023-06-13 16:41:37.000000 pitop.pma-0.31.0.post3/pitop/pma/ultrasonic_sensor.py
--rw-r--r--   0 runner    (1001) docker     (122)    12048 2023-06-13 16:41:37.000000 pitop.pma-0.31.0.post3/pitop/pma/ultrasonic_sensor_base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 16:41:54.000000 pitop.pma-0.31.0.post3/pitop.pma.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1014 2023-06-13 16:41:54.000000 pitop.pma-0.31.0.post3/pitop.pma.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1011 2023-06-13 16:41:54.000000 pitop.pma-0.31.0.post3/pitop.pma.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-13 16:41:54.000000 pitop.pma-0.31.0.post3/pitop.pma.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      110 2023-06-13 16:41:54.000000 pitop.pma-0.31.0.post3/pitop.pma.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-06-13 16:41:54.000000 pitop.pma-0.31.0.post3/pitop.pma.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-13 16:41:54.000000 pitop.pma-0.31.0.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2054 2023-06-13 16:41:37.000000 pitop.pma-0.31.0.post3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 18:30:08.000000 pitop.pma-0.31.0.post4/
+-rw-r--r--   0 runner    (1001) docker     (122)       31 2023-06-13 18:29:44.000000 pitop.pma-0.31.0.post4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1014 2023-06-13 18:30:08.000000 pitop.pma-0.31.0.post4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      175 2023-06-13 18:29:44.000000 pitop.pma-0.31.0.post4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 18:30:08.000000 pitop.pma-0.31.0.post4/pitop/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 18:30:08.000000 pitop.pma-0.31.0.post4/pitop/pma/
+-rw-r--r--   0 runner    (1001) docker     (122)      540 2023-06-13 18:29:44.000000 pitop.pma-0.31.0.post4/pitop/pma/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2953 2023-06-13 18:29:44.000000 pitop.pma-0.31.0.post4/pitop/pma/adc_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2551 2023-06-13 18:29:44.000000 pitop.pma-0.31.0.post4/pitop/pma/button.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2458 2023-06-13 18:29:44.000000 pitop.pma-0.31.0.post4/pitop/pma/buzzer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 18:30:08.000000 pitop.pma-0.31.0.post4/pitop/pma/common/
+-rw-r--r--   0 runner    (1001) docker     (122)       48 2023-06-13 18:29:44.000000 pitop.pma-0.31.0.post4/pitop/pma/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1893 2023-06-13 18:29:44.000000 pitop.pma-0.31.0.post4/pitop/pma/common/encoder_motor_registers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1954 2023-06-13 18:29:44.000000 pitop.pma-0.31.0.post4/pitop/pma/common/imu_registers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 18:30:08.000000 pitop.pma-0.31.0.post4/pitop/pma/common/math_functions/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-13 18:29:44.000000 pitop.pma-0.31.0.post4/pitop/pma/common/math_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3746 2023-06-13 18:29:44.000000 pitop.pma-0.31.0.post4/pitop/pma/common/math_functions/ellipsoid_functions.py
+-rw-r--r--   0 runner    (1001) docker     (122)      169 2023-06-13 18:29:44.000000 pitop.pma-0.31.0.post4/pitop/pma/common/plate_registers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      926 2023-06-13 18:29:44.000000 pitop.pma-0.31.0.post4/pitop/pma/common/servo_motor_registers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      404 2023-06-13 18:29:44.000000 pitop.pma-0.31.0.post4/pitop/pma/common/ultrasonic_registers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1781 2023-06-13 18:29:44.000000 pitop.pma-0.31.0.post4/pitop/pma/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17224 2023-06-13 18:29:45.000000 pitop.pma-0.31.0.post4/pitop/pma/encoder_motor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6086 2023-06-13 18:29:45.000000 pitop.pma-0.31.0.post4/pitop/pma/encoder_motor_controller.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4934 2023-06-13 18:29:45.000000 pitop.pma-0.31.0.post4/pitop/pma/imu.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10278 2023-06-13 18:29:45.000000 pitop.pma-0.31.0.post4/pitop/pma/imu_controller.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2643 2023-06-13 18:29:45.000000 pitop.pma-0.31.0.post4/pitop/pma/led.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2134 2023-06-13 18:29:45.000000 pitop.pma-0.31.0.post4/pitop/pma/light_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (122)      301 2023-06-13 18:29:45.000000 pitop.pma-0.31.0.post4/pitop/pma/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2586 2023-06-13 18:29:45.000000 pitop.pma-0.31.0.post4/pitop/pma/plate_interface.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2028 2023-06-13 18:29:45.000000 pitop.pma-0.31.0.post4/pitop/pma/potentiometer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4953 2023-06-13 18:29:45.000000 pitop.pma-0.31.0.post4/pitop/pma/servo_controller.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10704 2023-06-13 18:29:45.000000 pitop.pma-0.31.0.post4/pitop/pma/servo_motor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1888 2023-06-13 18:29:45.000000 pitop.pma-0.31.0.post4/pitop/pma/sound_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6078 2023-06-13 18:29:45.000000 pitop.pma-0.31.0.post4/pitop/pma/ultrasonic_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12048 2023-06-13 18:29:45.000000 pitop.pma-0.31.0.post4/pitop/pma/ultrasonic_sensor_base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 18:30:08.000000 pitop.pma-0.31.0.post4/pitop.pma.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1014 2023-06-13 18:30:08.000000 pitop.pma-0.31.0.post4/pitop.pma.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1011 2023-06-13 18:30:08.000000 pitop.pma-0.31.0.post4/pitop.pma.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-13 18:30:08.000000 pitop.pma-0.31.0.post4/pitop.pma.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      110 2023-06-13 18:30:08.000000 pitop.pma-0.31.0.post4/pitop.pma.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-06-13 18:30:08.000000 pitop.pma-0.31.0.post4/pitop.pma.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-13 18:30:08.000000 pitop.pma-0.31.0.post4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2071 2023-06-13 18:29:45.000000 pitop.pma-0.31.0.post4/setup.py
```

### Comparing `pitop.pma-0.31.0.post3/PKG-INFO` & `pitop.pma-0.31.0.post4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pitop.pma
-Version: 0.31.0.post3
+Version: 0.31.0.post4
 Summary: pi-top Python SDK.
 Home-page: https://github.com/pi-top/pi-top-Python-SDK
 Author: pi-top
 Author-email: deb-maintainers@pi-top.com
 License: Apache Software License
 Description: ===========================
         pi-top Python PMA
```

### Comparing `pitop.pma-0.31.0.post3/pitop/pma/__init__.py` & `pitop.pma-0.31.0.post4/pitop/pma/__init__.py`

 * *Files identical despite different names*

### Comparing `pitop.pma-0.31.0.post3/pitop/pma/adc_base.py` & `pitop.pma-0.31.0.post4/pitop/pma/adc_base.py`

 * *Files identical despite different names*

### Comparing `pitop.pma-0.31.0.post3/pitop/pma/button.py` & `pitop.pma-0.31.0.post4/pitop/pma/button.py`

 * *Files identical despite different names*

### Comparing `pitop.pma-0.31.0.post3/pitop/pma/buzzer.py` & `pitop.pma-0.31.0.post4/pitop/pma/buzzer.py`

 * *Files identical despite different names*

### Comparing `pitop.pma-0.31.0.post3/pitop/pma/common/encoder_motor_registers.py` & `pitop.pma-0.31.0.post4/pitop/pma/common/encoder_motor_registers.py`

 * *Files identical despite different names*

### Comparing `pitop.pma-0.31.0.post3/pitop/pma/common/imu_registers.py` & `pitop.pma-0.31.0.post4/pitop/pma/common/imu_registers.py`

 * *Files identical despite different names*

### Comparing `pitop.pma-0.31.0.post3/pitop/pma/common/math_functions/ellipsoid_functions.py` & `pitop.pma-0.31.0.post4/pitop/pma/common/math_functions/ellipsoid_functions.py`

 * *Files identical despite different names*

### Comparing `pitop.pma-0.31.0.post3/pitop/pma/common/servo_motor_registers.py` & `pitop.pma-0.31.0.post4/pitop/pma/common/servo_motor_registers.py`

 * *Files identical despite different names*

### Comparing `pitop.pma-0.31.0.post3/pitop/pma/common/utils.py` & `pitop.pma-0.31.0.post4/pitop/pma/common/utils.py`

 * *Files identical despite different names*

### Comparing `pitop.pma-0.31.0.post3/pitop/pma/encoder_motor.py` & `pitop.pma-0.31.0.post4/pitop/pma/encoder_motor.py`

 * *Files identical despite different names*

### Comparing `pitop.pma-0.31.0.post3/pitop/pma/encoder_motor_controller.py` & `pitop.pma-0.31.0.post4/pitop/pma/encoder_motor_controller.py`

 * *Files identical despite different names*

### Comparing `pitop.pma-0.31.0.post3/pitop/pma/imu.py` & `pitop.pma-0.31.0.post4/pitop/pma/imu.py`

 * *Files identical despite different names*

### Comparing `pitop.pma-0.31.0.post3/pitop/pma/imu_controller.py` & `pitop.pma-0.31.0.post4/pitop/pma/imu_controller.py`

 * *Files identical despite different names*

### Comparing `pitop.pma-0.31.0.post3/pitop/pma/led.py` & `pitop.pma-0.31.0.post4/pitop/pma/led.py`

 * *Files identical despite different names*

### Comparing `pitop.pma-0.31.0.post3/pitop/pma/light_sensor.py` & `pitop.pma-0.31.0.post4/pitop/pma/light_sensor.py`

 * *Files identical despite different names*

### Comparing `pitop.pma-0.31.0.post3/pitop/pma/plate_interface.py` & `pitop.pma-0.31.0.post4/pitop/pma/plate_interface.py`

 * *Files identical despite different names*

### Comparing `pitop.pma-0.31.0.post3/pitop/pma/potentiometer.py` & `pitop.pma-0.31.0.post4/pitop/pma/potentiometer.py`

 * *Files identical despite different names*

### Comparing `pitop.pma-0.31.0.post3/pitop/pma/servo_controller.py` & `pitop.pma-0.31.0.post4/pitop/pma/servo_controller.py`

 * *Files identical despite different names*

### Comparing `pitop.pma-0.31.0.post3/pitop/pma/servo_motor.py` & `pitop.pma-0.31.0.post4/pitop/pma/servo_motor.py`

 * *Files identical despite different names*

### Comparing `pitop.pma-0.31.0.post3/pitop/pma/sound_sensor.py` & `pitop.pma-0.31.0.post4/pitop/pma/sound_sensor.py`

 * *Files identical despite different names*

### Comparing `pitop.pma-0.31.0.post3/pitop/pma/ultrasonic_sensor.py` & `pitop.pma-0.31.0.post4/pitop/pma/ultrasonic_sensor.py`

 * *Files identical despite different names*

### Comparing `pitop.pma-0.31.0.post3/pitop/pma/ultrasonic_sensor_base.py` & `pitop.pma-0.31.0.post4/pitop/pma/ultrasonic_sensor_base.py`

 * *Files identical despite different names*

### Comparing `pitop.pma-0.31.0.post3/pitop.pma.egg-info/PKG-INFO` & `pitop.pma-0.31.0.post4/pitop.pma.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pitop.pma
-Version: 0.31.0.post3
+Version: 0.31.0.post4
 Summary: pi-top Python SDK.
 Home-page: https://github.com/pi-top/pi-top-Python-SDK
 Author: pi-top
 Author-email: deb-maintainers@pi-top.com
 License: Apache Software License
 Description: ===========================
         pi-top Python PMA
```

### Comparing `pitop.pma-0.31.0.post3/pitop.pma.egg-info/SOURCES.txt` & `pitop.pma-0.31.0.post4/pitop.pma.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pitop.pma-0.31.0.post3/setup.py` & `pitop.pma-0.31.0.post4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 if not sys.version_info >= (3, 7):
     raise ValueError("This package requires Python 3.7 or above")
 
 HERE = os.path.abspath(os.path.dirname(__file__))
 
-__version__ = os.environ.get("PYTHON_PACKAGE_VERSION", "0.0.1.dev1")
+__version__ = os.environ.get("PYTHON_PACKAGE_VERSION", "0.0.1.dev1").replace('"', "")
 assert __version__ != ""
 
 __project__ = "pitop.pma"
 __author__ = "pi-top"
 __author_email__ = "deb-maintainers@pi-top.com"
 
 __url__ = "https://github.com/pi-top/pi-top-Python-SDK"
```

