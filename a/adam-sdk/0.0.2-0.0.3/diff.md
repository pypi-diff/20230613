# Comparing `tmp/adam-sdk-0.0.2.tar.gz` & `tmp/adam-sdk-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adam-sdk-0.0.2.tar", last modified: Tue Jun  6 10:54:44 2023, max compression
+gzip compressed data, was "adam-sdk-0.0.3.tar", last modified: Tue Jun 13 02:39:57 2023, max compression
```

## Comparing `adam-sdk-0.0.2.tar` & `adam-sdk-0.0.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 10:54:44.680461 adam-sdk-0.0.2/
--rw-rw-rw-   0        0        0     1091 2023-06-06 00:09:38.000000 adam-sdk-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      491 2023-06-06 10:54:44.680461 adam-sdk-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       23 2023-06-05 22:18:33.000000 adam-sdk-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 10:54:44.672460 adam-sdk-0.0.2/adam_sdk/
--rw-rw-rw-   0        0        0     4175 2023-06-05 22:31:29.000000 adam-sdk-0.0.2/adam_sdk/AdamManager.py
-drwxrwxrwx   0        0        0        0 2023-06-06 10:54:44.676459 adam-sdk-0.0.2/adam_sdk/Controllers/
--rw-rw-rw-   0        0        0     1551 2023-06-05 22:18:51.000000 adam-sdk-0.0.2/adam_sdk/Controllers/JointController.py
--rw-rw-rw-   0        0        0     2453 2023-06-06 05:40:02.000000 adam-sdk-0.0.2/adam_sdk/Controllers/MecanumMoveController.py
--rw-rw-rw-   0        0        0     3719 2023-06-06 10:43:34.000000 adam-sdk-0.0.2/adam_sdk/Controllers/MotorController.py
--rw-rw-rw-   0        0        0     1721 2023-06-06 01:37:42.000000 adam-sdk-0.0.2/adam_sdk/JsonParser.py
-drwxrwxrwx   0        0        0        0 2023-06-06 10:54:44.679458 adam-sdk-0.0.2/adam_sdk/Models/
--rw-rw-rw-   0        0        0      247 2023-06-05 22:31:09.000000 adam-sdk-0.0.2/adam_sdk/Models/IMoveController.py
--rw-rw-rw-   0        0        0      332 2023-06-05 22:18:51.000000 adam-sdk-0.0.2/adam_sdk/Models/Joint.py
--rw-rw-rw-   0        0        0      452 2023-06-05 22:18:51.000000 adam-sdk-0.0.2/adam_sdk/Models/Motor.py
--rw-rw-rw-   0        0        0      260 2023-06-05 22:18:51.000000 adam-sdk-0.0.2/adam_sdk/Models/MotorCommand.py
--rw-rw-rw-   0        0        0       77 2023-06-05 22:18:51.000000 adam-sdk-0.0.2/adam_sdk/Models/MotorEnum.py
--rw-rw-rw-   0        0        0      225 2023-06-05 22:25:49.000000 adam-sdk-0.0.2/adam_sdk/Models/SerializableCommands.py
--rw-rw-rw-   0        0        0     2404 2023-06-05 22:30:22.000000 adam-sdk-0.0.2/adam_sdk/ServoConnection.py
--rw-rw-rw-   0        0        0      582 2023-06-06 05:40:02.000000 adam-sdk-0.0.2/adam_sdk/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-06 10:54:44.675460 adam-sdk-0.0.2/adam_sdk.egg-info/
--rw-rw-rw-   0        0        0      491 2023-06-06 10:54:44.000000 adam-sdk-0.0.2/adam_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      593 2023-06-06 10:54:44.000000 adam-sdk-0.0.2/adam_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 10:54:44.000000 adam-sdk-0.0.2/adam_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-06-06 10:54:44.000000 adam-sdk-0.0.2/adam_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-06 10:54:44.000000 adam-sdk-0.0.2/adam_sdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-06 10:54:44.680461 adam-sdk-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      807 2023-06-06 10:54:44.000000 adam-sdk-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 02:39:57.779216 adam-sdk-0.0.3/
+-rw-rw-rw-   0        0        0     1091 2023-06-06 00:09:38.000000 adam-sdk-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     5284 2023-06-13 02:39:57.779216 adam-sdk-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4818 2023-06-13 01:16:00.000000 adam-sdk-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-13 02:39:57.768215 adam-sdk-0.0.3/adam_sdk/
+-rw-rw-rw-   0        0        0     4175 2023-06-05 22:31:29.000000 adam-sdk-0.0.3/adam_sdk/AdamManager.py
+drwxrwxrwx   0        0        0        0 2023-06-13 02:39:57.774213 adam-sdk-0.0.3/adam_sdk/Controllers/
+-rw-rw-rw-   0        0        0     1551 2023-06-05 22:18:51.000000 adam-sdk-0.0.3/adam_sdk/Controllers/JointController.py
+-rw-rw-rw-   0        0        0     2454 2023-06-13 01:16:00.000000 adam-sdk-0.0.3/adam_sdk/Controllers/MecanumMoveController.py
+-rw-rw-rw-   0        0        0     3719 2023-06-06 10:43:34.000000 adam-sdk-0.0.3/adam_sdk/Controllers/MotorController.py
+-rw-rw-rw-   0        0        0     1720 2023-06-13 02:31:51.000000 adam-sdk-0.0.3/adam_sdk/JsonParser.py
+drwxrwxrwx   0        0        0        0 2023-06-13 02:39:57.778213 adam-sdk-0.0.3/adam_sdk/Models/
+-rw-rw-rw-   0        0        0      247 2023-06-05 22:31:09.000000 adam-sdk-0.0.3/adam_sdk/Models/IMoveController.py
+-rw-rw-rw-   0        0        0      332 2023-06-05 22:18:51.000000 adam-sdk-0.0.3/adam_sdk/Models/Joint.py
+-rw-rw-rw-   0        0        0      452 2023-06-05 22:18:51.000000 adam-sdk-0.0.3/adam_sdk/Models/Motor.py
+-rw-rw-rw-   0        0        0      260 2023-06-05 22:18:51.000000 adam-sdk-0.0.3/adam_sdk/Models/MotorCommand.py
+-rw-rw-rw-   0        0        0       77 2023-06-05 22:18:51.000000 adam-sdk-0.0.3/adam_sdk/Models/MotorEnum.py
+-rw-rw-rw-   0        0        0      225 2023-06-05 22:25:49.000000 adam-sdk-0.0.3/adam_sdk/Models/SerializableCommands.py
+-rw-rw-rw-   0        0        0     2404 2023-06-05 22:30:22.000000 adam-sdk-0.0.3/adam_sdk/ServoConnection.py
+-rw-rw-rw-   0        0        0      582 2023-06-06 05:40:02.000000 adam-sdk-0.0.3/adam_sdk/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 02:39:57.772214 adam-sdk-0.0.3/adam_sdk.egg-info/
+-rw-rw-rw-   0        0        0     5284 2023-06-13 02:39:57.000000 adam-sdk-0.0.3/adam_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      593 2023-06-13 02:39:57.000000 adam-sdk-0.0.3/adam_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 02:39:57.000000 adam-sdk-0.0.3/adam_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-06-13 02:39:57.000000 adam-sdk-0.0.3/adam_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-13 02:39:57.000000 adam-sdk-0.0.3/adam_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-13 02:39:57.779216 adam-sdk-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      807 2023-06-13 02:34:14.000000 adam-sdk-0.0.3/setup.py
```

### Comparing `adam-sdk-0.0.2/LICENSE` & `adam-sdk-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `adam-sdk-0.0.2/adam_sdk/AdamManager.py` & `adam-sdk-0.0.3/adam_sdk/AdamManager.py`

 * *Files identical despite different names*

### Comparing `adam-sdk-0.0.2/adam_sdk/Controllers/JointController.py` & `adam-sdk-0.0.3/adam_sdk/Controllers/JointController.py`

 * *Files identical despite different names*

### Comparing `adam-sdk-0.0.2/adam_sdk/Controllers/MecanumMoveController.py` & `adam-sdk-0.0.3/adam_sdk/Controllers/MecanumMoveController.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Tuple
 from .MotorController import MotorController
 from pymodbus.client.serial import ModbusSerialClient as ModbusClient
 
 class MecanumMoveController:
     def __init__(self):
         client = ModbusClient(
-            method="rtu", port="/dev/ttyUSB1", stopbits=1, bytesize=8, parity='N', baudrate=9600
+            method="rtu", port="/dev/ttyS0", stopbits=1, bytesize=8, parity='N', baudrate=76800
         )
         client.connect()
         
         self.front_left = MotorController(client, 22, 2, 3)  # Создание объекта мотора для переднего левого колеса
         self.front_right = MotorController(client, 23, 0, 1, True)  # Создание объекта мотора для переднего правого колеса с инверсией
         self.rear_left = MotorController(client, 22, 0, 1)  # Создание объекта мотора для заднего левого колеса
         self.rear_right = MotorController(client, 23, 2, 3, True)  # Создание объекта мотора для заднего правого колеса с инверсией
@@ -32,8 +32,8 @@
         
         for motor, speed in zip([self.front_left, self.front_right, self.rear_left, self.rear_right], speeds):
             motor.set_speed(speed)
         
         # self.front_left.set_speed(speeds[0])  # Установка скорости для переднего левого колеса
         # self.front_right.set_speed(speeds[1])  # Установка скорости для переднего правого колеса
         # self.rear_left.set_speed(speeds[2])  # Установка скорости для заднего левого колеса
-        # self.rear_right.set_speed(speeds[3])  # Установка скорости для заднего правого колеса
+        # self.rear_right.set_speed(speeds[3])  # Установка скорости для заднего правого колеса
```

### Comparing `adam-sdk-0.0.2/adam_sdk/Controllers/MotorController.py` & `adam-sdk-0.0.3/adam_sdk/Controllers/MotorController.py`

 * *Files identical despite different names*

### Comparing `adam-sdk-0.0.2/adam_sdk/JsonParser.py` & `adam-sdk-0.0.3/adam_sdk/JsonParser.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 class JsonParser:
 
     @staticmethod
     def _read_config():
         config_file_path = "/etc/adam_configs/servo_range.config"
         
         if os.path.isfile(config_file_path) is False:
-            config_file_path = f'{current}/../examples/position_range.json'
+            config_file_path = f'{current}/../examples/servo_range.config'
         file = open(config_file_path)
         data = json.load(file)
         file.close()
 
         return data
 
     @staticmethod
```

### Comparing `adam-sdk-0.0.2/adam_sdk/ServoConnection.py` & `adam-sdk-0.0.3/adam_sdk/ServoConnection.py`

 * *Files identical despite different names*

### Comparing `adam-sdk-0.0.2/adam_sdk/__init__.py` & `adam-sdk-0.0.3/adam_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `adam-sdk-0.0.2/adam_sdk.egg-info/SOURCES.txt` & `adam-sdk-0.0.3/adam_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adam-sdk-0.0.2/setup.py` & `adam-sdk-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='adam-sdk',
-    version='0.0.2',
+    version='0.0.3',
     packages=['adam_sdk', 'adam_sdk.Controllers', 'adam_sdk.Models'],
     url='https://github.com/Adam-Software/Adam-SDK',
     license='MIT',
     author='Adam Software',
     author_email='a@nesterof.com',
     description='SDK for robot Adam',
     long_description_content_type="text/markdown",
```

