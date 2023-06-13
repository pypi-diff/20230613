# Comparing `tmp/pitop-0.7.0.tar.gz` & `tmp/pitop-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pitop-0.7.0.tar", last modified: Wed Dec 23 13:18:55 2020, max compression
+gzip compressed data, was "pitop-0.8.1.tar", last modified: Mon Jan  4 14:16:56 2021, max compression
```

## Comparing `pitop-0.7.0.tar` & `pitop-0.8.1.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxr-xr-x   0 jorge      (501) staff       (20)        0 2020-12-23 13:18:55.890612 pitop-0.7.0/
--rw-r--r--   0 jorge      (501) staff       (20)     7439 2020-12-23 13:18:55.890437 pitop-0.7.0/PKG-INFO
--rw-r--r--   0 jorge      (501) staff       (20)     5238 2020-12-17 22:10:46.000000 pitop-0.7.0/README.rst
-drwxr-xr-x   0 jorge      (501) staff       (20)        0 2020-12-23 13:18:55.880363 pitop-0.7.0/pitop/
--rw-r--r--   0 jorge      (501) staff       (20)        0 2020-12-14 16:34:56.000000 pitop-0.7.0/pitop/__init__.py
-drwxr-xr-x   0 jorge      (501) staff       (20)        0 2020-12-23 13:18:55.881369 pitop-0.7.0/pitop/battery/
--rw-r--r--   0 jorge      (501) staff       (20)       29 2020-12-17 22:10:46.000000 pitop-0.7.0/pitop/battery/__init__.py
--rw-r--r--   0 jorge      (501) staff       (20)     2726 2020-12-17 13:02:52.000000 pitop-0.7.0/pitop/battery/battery.py
-drwxr-xr-x   0 jorge      (501) staff       (20)        0 2020-12-23 13:18:55.881757 pitop-0.7.0/pitop/camera/
--rw-r--r--   0 jorge      (501) staff       (20)       91 2020-12-17 22:10:46.000000 pitop-0.7.0/pitop/camera/__init__.py
--rw-r--r--   0 jorge      (501) staff       (20)     9226 2020-12-14 16:34:56.000000 pitop-0.7.0/pitop/camera/camera.py
-drwxr-xr-x   0 jorge      (501) staff       (20)        0 2020-12-23 13:18:55.881995 pitop-0.7.0/pitop/camera/core/
--rw-r--r--   0 jorge      (501) staff       (20)      325 2020-12-17 22:10:46.000000 pitop-0.7.0/pitop/camera/core/__init__.py
-drwxr-xr-x   0 jorge      (501) staff       (20)        0 2020-12-23 13:18:55.882475 pitop-0.7.0/pitop/camera/core/cameras/
--rw-r--r--   0 jorge      (501) staff       (20)      151 2020-12-17 22:10:46.000000 pitop-0.7.0/pitop/camera/core/cameras/__init__.py
--rw-r--r--   0 jorge      (501) staff       (20)      202 2020-12-14 16:34:56.000000 pitop-0.7.0/pitop/camera/core/cameras/camera_types.py
--rw-r--r--   0 jorge      (501) staff       (20)     2479 2020-12-14 16:34:56.000000 pitop-0.7.0/pitop/camera/core/cameras/file_system_camera.py
--rw-r--r--   0 jorge      (501) staff       (20)      794 2020-12-14 16:34:56.000000 pitop-0.7.0/pitop/camera/core/cameras/usb_camera.py
-drwxr-xr-x   0 jorge      (501) staff       (20)        0 2020-12-23 13:18:55.883306 pitop-0.7.0/pitop/camera/core/capture_actions/
--rw-r--r--   0 jorge      (501) staff       (20)      336 2020-12-17 22:10:46.000000 pitop-0.7.0/pitop/camera/core/capture_actions/__init__.py
--rw-r--r--   0 jorge      (501) staff       (20)      734 2020-12-14 16:34:56.000000 pitop-0.7.0/pitop/camera/core/capture_actions/capture_action_base.py
--rw-r--r--   0 jorge      (501) staff       (20)      362 2020-12-14 16:34:56.000000 pitop-0.7.0/pitop/camera/core/capture_actions/capture_actions.py
--rw-r--r--   0 jorge      (501) staff       (20)     1692 2020-12-14 16:34:56.000000 pitop-0.7.0/pitop/camera/core/capture_actions/generic_action.py
--rw-r--r--   0 jorge      (501) staff       (20)     2956 2020-12-14 16:34:56.000000 pitop-0.7.0/pitop/camera/core/capture_actions/motion_detector.py
--rw-r--r--   0 jorge      (501) staff       (20)      622 2020-12-17 16:55:09.000000 pitop-0.7.0/pitop/camera/core/capture_actions/store_frame.py
--rw-r--r--   0 jorge      (501) staff       (20)     2116 2020-12-14 16:34:56.000000 pitop-0.7.0/pitop/camera/core/capture_actions/video_capture.py
--rw-r--r--   0 jorge      (501) staff       (20)     3373 2020-12-14 16:34:56.000000 pitop-0.7.0/pitop/camera/core/frame_handler.py
--rw-r--r--   0 jorge      (501) staff       (20)      911 2020-12-14 16:34:56.000000 pitop-0.7.0/pitop/camera/pil_opencv_conversion.py
-drwxr-xr-x   0 jorge      (501) staff       (20)        0 2020-12-23 13:18:55.883542 pitop-0.7.0/pitop/display/
--rw-r--r--   0 jorge      (501) staff       (20)       29 2020-12-17 22:10:46.000000 pitop-0.7.0/pitop/display/__init__.py
--rw-r--r--   0 jorge      (501) staff       (20)     5107 2020-12-17 13:02:52.000000 pitop-0.7.0/pitop/display/display.py
-drwxr-xr-x   0 jorge      (501) staff       (20)        0 2020-12-23 13:18:55.883760 pitop-0.7.0/pitop/keyboard/
--rw-r--r--   0 jorge      (501) staff       (20)       43 2020-12-17 22:10:46.000000 pitop-0.7.0/pitop/keyboard/__init__.py
--rw-r--r--   0 jorge      (501) staff       (20)     2720 2020-12-14 16:34:56.000000 pitop-0.7.0/pitop/keyboard/key_listener.py
-drwxr-xr-x   0 jorge      (501) staff       (20)        0 2020-12-23 13:18:55.883908 pitop-0.7.0/pitop/miniscreen/
--rw-r--r--   0 jorge      (501) staff       (20)      126 2020-12-17 22:10:46.000000 pitop-0.7.0/pitop/miniscreen/__init__.py
-drwxr-xr-x   0 jorge      (501) staff       (20)        0 2020-12-23 13:18:55.884150 pitop-0.7.0/pitop/miniscreen/buttons/
--rw-r--r--   0 jorge      (501) staff       (20)      103 2020-12-17 22:10:46.000000 pitop-0.7.0/pitop/miniscreen/buttons/__init__.py
--rw-r--r--   0 jorge      (501) staff       (20)     4298 2020-12-14 16:34:56.000000 pitop-0.7.0/pitop/miniscreen/buttons/buttons.py
-drwxr-xr-x   0 jorge      (501) staff       (20)        0 2020-12-23 13:18:55.884365 pitop-0.7.0/pitop/miniscreen/oled/
--rw-r--r--   0 jorge      (501) staff       (20)       23 2020-12-17 22:10:46.000000 pitop-0.7.0/pitop/miniscreen/oled/__init__.py
-drwxr-xr-x   0 jorge      (501) staff       (20)        0 2020-12-23 13:18:55.884957 pitop-0.7.0/pitop/miniscreen/oled/core/
--rw-r--r--   0 jorge      (501) staff       (20)        0 2020-12-14 16:34:56.000000 pitop-0.7.0/pitop/miniscreen/oled/core/__init__.py
--rw-r--r--   0 jorge      (501) staff       (20)    17508 2020-12-14 16:34:56.000000 pitop-0.7.0/pitop/miniscreen/oled/core/canvas.py
--rw-r--r--   0 jorge      (501) staff       (20)     2456 2020-12-17 22:10:46.000000 pitop-0.7.0/pitop/miniscreen/oled/core/controls.py
--rw-r--r--   0 jorge      (501) staff       (20)     3420 2020-12-14 16:34:56.000000 pitop-0.7.0/pitop/miniscreen/oled/core/fps_regulator.py
--rw-r--r--   0 jorge      (501) staff       (20)      752 2020-12-14 16:34:56.000000 pitop-0.7.0/pitop/miniscreen/oled/core/image_helper.py
--rw-r--r--   0 jorge      (501) staff       (20)    11049 2020-12-17 22:10:46.000000 pitop-0.7.0/pitop/miniscreen/oled/oled.py
-drwxr-xr-x   0 jorge      (501) staff       (20)        0 2020-12-23 13:18:55.886963 pitop-0.7.0/pitop/pma/
--rw-r--r--   0 jorge      (501) staff       (20)      481 2020-12-17 22:10:46.000000 pitop-0.7.0/pitop/pma/__init__.py
--rw-r--r--   0 jorge      (501) staff       (20)     2164 2020-12-14 16:34:56.000000 pitop-0.7.0/pitop/pma/adc_base.py
--rw-r--r--   0 jorge      (501) staff       (20)     2045 2020-12-14 16:34:56.000000 pitop-0.7.0/pitop/pma/button.py
--rw-r--r--   0 jorge      (501) staff       (20)     1987 2020-12-14 16:34:56.000000 pitop-0.7.0/pitop/pma/buzzer.py
-drwxr-xr-x   0 jorge      (501) staff       (20)        0 2020-12-23 13:18:55.887593 pitop-0.7.0/pitop/pma/common/
--rw-r--r--   0 jorge      (501) staff       (20)       61 2020-12-17 22:10:46.000000 pitop-0.7.0/pitop/pma/common/__init__.py
--rw-r--r--   0 jorge      (501) staff       (20)     1715 2020-12-14 16:34:56.000000 pitop-0.7.0/pitop/pma/common/encoder_motor_registers.py
--rw-r--r--   0 jorge      (501) staff       (20)     2033 2020-12-17 14:05:50.000000 pitop-0.7.0/pitop/pma/common/imu_registers.py
-drwxr-xr-x   0 jorge      (501) staff       (20)        0 2020-12-23 13:18:55.887794 pitop-0.7.0/pitop/pma/common/math_functions/
--rw-r--r--   0 jorge      (501) staff       (20)        0 2020-12-17 22:11:12.000000 pitop-0.7.0/pitop/pma/common/math_functions/__init__.py
--rw-r--r--   0 jorge      (501) staff       (20)     3746 2020-12-17 22:46:58.000000 pitop-0.7.0/pitop/pma/common/math_functions/ellipsoid_functions.py
--rw-r--r--   0 jorge      (501) staff       (20)      169 2020-12-14 16:34:56.000000 pitop-0.7.0/pitop/pma/common/plate_registers.py
--rw-r--r--   0 jorge      (501) staff       (20)      922 2020-12-17 22:10:46.000000 pitop-0.7.0/pitop/pma/common/servo_motor_registers.py
--rw-r--r--   0 jorge      (501) staff       (20)     1784 2020-12-14 16:34:56.000000 pitop-0.7.0/pitop/pma/common/utils.py
--rw-r--r--   0 jorge      (501) staff       (20)      158 2020-12-14 16:34:56.000000 pitop-0.7.0/pitop/pma/components.py
--rw-r--r--   0 jorge      (501) staff       (20)    15659 2020-12-17 22:10:46.000000 pitop-0.7.0/pitop/pma/encoder_motor.py
--rw-r--r--   0 jorge      (501) staff       (20)     5200 2020-12-14 16:34:56.000000 pitop-0.7.0/pitop/pma/encoder_motor_controller.py
--rw-r--r--   0 jorge      (501) staff       (20)     4915 2020-12-17 22:10:46.000000 pitop-0.7.0/pitop/pma/imu.py
--rw-r--r--   0 jorge      (501) staff       (20)     9881 2020-12-17 22:10:46.000000 pitop-0.7.0/pitop/pma/imu_controller.py
--rw-r--r--   0 jorge      (501) staff       (20)     2023 2020-12-14 16:34:56.000000 pitop-0.7.0/pitop/pma/led.py
--rw-r--r--   0 jorge      (501) staff       (20)     1237 2020-12-14 16:34:56.000000 pitop-0.7.0/pitop/pma/light_sensor.py
--rw-r--r--   0 jorge      (501) staff       (20)      325 2020-12-14 16:34:56.000000 pitop-0.7.0/pitop/pma/parameters.py
--rw-r--r--   0 jorge      (501) staff       (20)     2482 2020-12-14 16:34:56.000000 pitop-0.7.0/pitop/pma/plate_interface.py
--rw-r--r--   0 jorge      (501) staff       (20)     1368 2020-12-14 16:34:56.000000 pitop-0.7.0/pitop/pma/potentiometer.py
--rw-r--r--   0 jorge      (501) staff       (20)     4235 2020-12-17 22:10:46.000000 pitop-0.7.0/pitop/pma/servo_controller.py
--rw-r--r--   0 jorge      (501) staff       (20)     8335 2020-12-17 22:10:46.000000 pitop-0.7.0/pitop/pma/servo_motor.py
--rw-r--r--   0 jorge      (501) staff       (20)     1122 2020-12-14 16:34:56.000000 pitop-0.7.0/pitop/pma/sound_sensor.py
--rw-r--r--   0 jorge      (501) staff       (20)     7316 2020-12-14 16:34:56.000000 pitop-0.7.0/pitop/pma/ultrasonic_sensor.py
-drwxr-xr-x   0 jorge      (501) staff       (20)        0 2020-12-23 13:18:55.888100 pitop-0.7.0/pitop/protoplus/
--rw-r--r--   0 jorge      (501) staff       (20)       62 2020-12-17 22:10:46.000000 pitop-0.7.0/pitop/protoplus/__init__.py
--rw-r--r--   0 jorge      (501) staff       (20)     2152 2020-12-14 16:34:56.000000 pitop-0.7.0/pitop/protoplus/adc.py
--rw-r--r--   0 jorge      (501) staff       (20)     2499 2020-12-17 13:02:52.000000 pitop-0.7.0/pitop/protoplus/sensors.py
-drwxr-xr-x   0 jorge      (501) staff       (20)        0 2020-12-23 13:18:55.888507 pitop-0.7.0/pitop/pulse/
--rw-r--r--   0 jorge      (501) staff       (20)        0 2020-12-14 16:34:56.000000 pitop-0.7.0/pitop/pulse/__init__.py
--rw-r--r--   0 jorge      (501) staff       (20)     5842 2020-12-17 13:02:52.000000 pitop-0.7.0/pitop/pulse/configuration.py
--rw-r--r--   0 jorge      (501) staff       (20)    16813 2020-12-17 13:02:52.000000 pitop-0.7.0/pitop/pulse/ledmatrix.py
--rw-r--r--   0 jorge      (501) staff       (20)     8981 2020-12-17 13:02:52.000000 pitop-0.7.0/pitop/pulse/microphone.py
-drwxr-xr-x   0 jorge      (501) staff       (20)        0 2020-12-23 13:18:55.888898 pitop-0.7.0/pitop/system/
--rw-r--r--   0 jorge      (501) staff       (20)      285 2020-12-17 22:10:46.000000 pitop-0.7.0/pitop/system/__init__.py
--rw-r--r--   0 jorge      (501) staff       (20)      265 2020-12-14 16:34:56.000000 pitop-0.7.0/pitop/system/daemon.py
--rw-r--r--   0 jorge      (501) staff       (20)     1693 2020-12-14 16:34:56.000000 pitop-0.7.0/pitop/system/device.py
--rw-r--r--   0 jorge      (501) staff       (20)     3509 2020-12-22 21:47:06.000000 pitop-0.7.0/pitop/system/peripherals.py
-drwxr-xr-x   0 jorge      (501) staff       (20)        0 2020-12-23 13:18:55.881143 pitop-0.7.0/pitop.egg-info/
--rw-r--r--   0 jorge      (501) staff       (20)     7439 2020-12-23 13:18:55.000000 pitop-0.7.0/pitop.egg-info/PKG-INFO
--rw-r--r--   0 jorge      (501) staff       (20)     2697 2020-12-23 13:18:55.000000 pitop-0.7.0/pitop.egg-info/SOURCES.txt
--rw-r--r--   0 jorge      (501) staff       (20)        1 2020-12-23 13:18:55.000000 pitop-0.7.0/pitop.egg-info/dependency_links.txt
--rw-r--r--   0 jorge      (501) staff       (20)      248 2020-12-23 13:18:55.000000 pitop-0.7.0/pitop.egg-info/entry_points.txt
--rw-r--r--   0 jorge      (501) staff       (20)      213 2020-12-23 13:18:55.000000 pitop-0.7.0/pitop.egg-info/requires.txt
--rw-r--r--   0 jorge      (501) staff       (20)       15 2020-12-23 13:18:55.000000 pitop-0.7.0/pitop.egg-info/top_level.txt
-drwxr-xr-x   0 jorge      (501) staff       (20)        0 2020-12-23 13:18:55.890205 pitop-0.7.0/pitopcli/
--rw-r--r--   0 jorge      (501) staff       (20)        0 2020-12-14 16:34:56.000000 pitop-0.7.0/pitopcli/__init__.py
--rw-r--r--   0 jorge      (501) staff       (20)     2983 2020-12-14 16:34:56.000000 pitop-0.7.0/pitopcli/battery.py
--rw-r--r--   0 jorge      (501) staff       (20)     1331 2020-12-14 16:34:56.000000 pitop-0.7.0/pitopcli/cli_base.py
--rw-r--r--   0 jorge      (501) staff       (20)     1904 2020-12-14 16:34:56.000000 pitop-0.7.0/pitopcli/deprecated_cli_runner.py
--rw-r--r--   0 jorge      (501) staff       (20)     4247 2020-12-14 16:34:56.000000 pitop-0.7.0/pitopcli/devices.py
--rw-r--r--   0 jorge      (501) staff       (20)     5166 2020-12-14 16:34:56.000000 pitop-0.7.0/pitopcli/display.py
--rw-r--r--   0 jorge      (501) staff       (20)     4348 2020-12-17 22:10:46.000000 pitop-0.7.0/pitopcli/help.py
--rw-r--r--   0 jorge      (501) staff       (20)     2381 2020-12-17 22:10:46.000000 pitop-0.7.0/pitopcli/imu.py
--rw-r--r--   0 jorge      (501) staff       (20)    13281 2020-12-17 22:10:46.000000 pitop-0.7.0/pitopcli/imu_calibration.py
--rw-r--r--   0 jorge      (501) staff       (20)     3490 2020-12-17 13:02:52.000000 pitop-0.7.0/pitopcli/oled.py
--rw-r--r--   0 jorge      (501) staff       (20)     2014 2020-12-17 22:10:46.000000 pitop-0.7.0/pitopcli/pitop.py
--rw-r--r--   0 jorge      (501) staff       (20)       38 2020-12-23 13:18:55.890655 pitop-0.7.0/setup.cfg
--rw-r--r--   0 jorge      (501) staff       (20)     4512 2020-12-17 22:10:46.000000 pitop-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-01-04 14:16:56.236524 pitop-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (121)     7993 2021-01-04 14:16:56.236524 pitop-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     5720 2021-01-04 14:16:45.000000 pitop-0.8.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-01-04 14:16:56.220523 pitop-0.8.1/pitop/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-01-04 14:16:45.000000 pitop-0.8.1/pitop/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-01-04 14:16:56.220523 pitop-0.8.1/pitop/battery/
+-rw-r--r--   0 runner    (1001) docker     (121)       29 2021-01-04 14:16:45.000000 pitop-0.8.1/pitop/battery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2726 2021-01-04 14:16:45.000000 pitop-0.8.1/pitop/battery/battery.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-01-04 14:16:56.220523 pitop-0.8.1/pitop/camera/
+-rw-r--r--   0 runner    (1001) docker     (121)       91 2021-01-04 14:16:45.000000 pitop-0.8.1/pitop/camera/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9226 2021-01-04 14:16:45.000000 pitop-0.8.1/pitop/camera/camera.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-01-04 14:16:56.220523 pitop-0.8.1/pitop/camera/core/
+-rw-r--r--   0 runner    (1001) docker     (121)      325 2021-01-04 14:16:45.000000 pitop-0.8.1/pitop/camera/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-01-04 14:16:56.220523 pitop-0.8.1/pitop/camera/core/cameras/
+-rw-r--r--   0 runner    (1001) docker     (121)      151 2021-01-04 14:16:45.000000 pitop-0.8.1/pitop/camera/core/cameras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      202 2021-01-04 14:16:45.000000 pitop-0.8.1/pitop/camera/core/cameras/camera_types.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2479 2021-01-04 14:16:45.000000 pitop-0.8.1/pitop/camera/core/cameras/file_system_camera.py
+-rw-r--r--   0 runner    (1001) docker     (121)      794 2021-01-04 14:16:45.000000 pitop-0.8.1/pitop/camera/core/cameras/usb_camera.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-01-04 14:16:56.220523 pitop-0.8.1/pitop/camera/core/capture_actions/
+-rw-r--r--   0 runner    (1001) docker     (121)      336 2021-01-04 14:16:45.000000 pitop-0.8.1/pitop/camera/core/capture_actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      734 2021-01-04 14:16:45.000000 pitop-0.8.1/pitop/camera/core/capture_actions/capture_action_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)      362 2021-01-04 14:16:45.000000 pitop-0.8.1/pitop/camera/core/capture_actions/capture_actions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1692 2021-01-04 14:16:45.000000 pitop-0.8.1/pitop/camera/core/capture_actions/generic_action.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2956 2021-01-04 14:16:45.000000 pitop-0.8.1/pitop/camera/core/capture_actions/motion_detector.py
+-rw-r--r--   0 runner    (1001) docker     (121)      622 2021-01-04 14:16:45.000000 pitop-0.8.1/pitop/camera/core/capture_actions/store_frame.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2116 2021-01-04 14:16:45.000000 pitop-0.8.1/pitop/camera/core/capture_actions/video_capture.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3373 2021-01-04 14:16:45.000000 pitop-0.8.1/pitop/camera/core/frame_handler.py
+-rw-r--r--   0 runner    (1001) docker     (121)      911 2021-01-04 14:16:45.000000 pitop-0.8.1/pitop/camera/pil_opencv_conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-01-04 14:16:56.220523 pitop-0.8.1/pitop/display/
+-rw-r--r--   0 runner    (1001) docker     (121)       29 2021-01-04 14:16:45.000000 pitop-0.8.1/pitop/display/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5107 2021-01-04 14:16:45.000000 pitop-0.8.1/pitop/display/display.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-01-04 14:16:56.220523 pitop-0.8.1/pitop/keyboard/
+-rw-r--r--   0 runner    (1001) docker     (121)       43 2021-01-04 14:16:45.000000 pitop-0.8.1/pitop/keyboard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2720 2021-01-04 14:16:45.000000 pitop-0.8.1/pitop/keyboard/key_listener.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-01-04 14:16:56.220523 pitop-0.8.1/pitop/miniscreen/
+-rw-r--r--   0 runner    (1001) docker     (121)      126 2021-01-04 14:16:45.000000 pitop-0.8.1/pitop/miniscreen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-01-04 14:16:56.228523 pitop-0.8.1/pitop/miniscreen/buttons/
+-rw-r--r--   0 runner    (1001) docker     (121)      103 2021-01-04 14:16:45.000000 pitop-0.8.1/pitop/miniscreen/buttons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4298 2021-01-04 14:16:45.000000 pitop-0.8.1/pitop/miniscreen/buttons/buttons.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-01-04 14:16:56.228523 pitop-0.8.1/pitop/miniscreen/oled/
+-rw-r--r--   0 runner    (1001) docker     (121)       23 2021-01-04 14:16:45.000000 pitop-0.8.1/pitop/miniscreen/oled/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-01-04 14:16:56.228523 pitop-0.8.1/pitop/miniscreen/oled/core/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-01-04 14:16:45.000000 pitop-0.8.1/pitop/miniscreen/oled/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17508 2021-01-04 14:16:45.000000 pitop-0.8.1/pitop/miniscreen/oled/core/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2456 2021-01-04 14:16:45.000000 pitop-0.8.1/pitop/miniscreen/oled/core/controls.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3420 2021-01-04 14:16:45.000000 pitop-0.8.1/pitop/miniscreen/oled/core/fps_regulator.py
+-rw-r--r--   0 runner    (1001) docker     (121)      752 2021-01-04 14:16:45.000000 pitop-0.8.1/pitop/miniscreen/oled/core/image_helper.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11049 2021-01-04 14:16:45.000000 pitop-0.8.1/pitop/miniscreen/oled/oled.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-01-04 14:16:56.232524 pitop-0.8.1/pitop/pma/
+-rw-r--r--   0 runner    (1001) docker     (121)      481 2021-01-04 14:16:45.000000 pitop-0.8.1/pitop/pma/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2164 2021-01-04 14:16:45.000000 pitop-0.8.1/pitop/pma/adc_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2045 2021-01-04 14:16:45.000000 pitop-0.8.1/pitop/pma/button.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1987 2021-01-04 14:16:45.000000 pitop-0.8.1/pitop/pma/buzzer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-01-04 14:16:56.232524 pitop-0.8.1/pitop/pma/common/
+-rw-r--r--   0 runner    (1001) docker     (121)       61 2021-01-04 14:16:45.000000 pitop-0.8.1/pitop/pma/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1715 2021-01-04 14:16:45.000000 pitop-0.8.1/pitop/pma/common/encoder_motor_registers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2033 2021-01-04 14:16:45.000000 pitop-0.8.1/pitop/pma/common/imu_registers.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-01-04 14:16:56.232524 pitop-0.8.1/pitop/pma/common/math_functions/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-01-04 14:16:45.000000 pitop-0.8.1/pitop/pma/common/math_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3746 2021-01-04 14:16:45.000000 pitop-0.8.1/pitop/pma/common/math_functions/ellipsoid_functions.py
+-rw-r--r--   0 runner    (1001) docker     (121)      169 2021-01-04 14:16:45.000000 pitop-0.8.1/pitop/pma/common/plate_registers.py
+-rw-r--r--   0 runner    (1001) docker     (121)      922 2021-01-04 14:16:45.000000 pitop-0.8.1/pitop/pma/common/servo_motor_registers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1784 2021-01-04 14:16:45.000000 pitop-0.8.1/pitop/pma/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      158 2021-01-04 14:16:45.000000 pitop-0.8.1/pitop/pma/components.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15659 2021-01-04 14:16:45.000000 pitop-0.8.1/pitop/pma/encoder_motor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5200 2021-01-04 14:16:45.000000 pitop-0.8.1/pitop/pma/encoder_motor_controller.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4915 2021-01-04 14:16:45.000000 pitop-0.8.1/pitop/pma/imu.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9881 2021-01-04 14:16:45.000000 pitop-0.8.1/pitop/pma/imu_controller.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2023 2021-01-04 14:16:45.000000 pitop-0.8.1/pitop/pma/led.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1237 2021-01-04 14:16:45.000000 pitop-0.8.1/pitop/pma/light_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (121)      325 2021-01-04 14:16:45.000000 pitop-0.8.1/pitop/pma/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2482 2021-01-04 14:16:45.000000 pitop-0.8.1/pitop/pma/plate_interface.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1368 2021-01-04 14:16:45.000000 pitop-0.8.1/pitop/pma/potentiometer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4235 2021-01-04 14:16:45.000000 pitop-0.8.1/pitop/pma/servo_controller.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8335 2021-01-04 14:16:45.000000 pitop-0.8.1/pitop/pma/servo_motor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1122 2021-01-04 14:16:45.000000 pitop-0.8.1/pitop/pma/sound_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7316 2021-01-04 14:16:45.000000 pitop-0.8.1/pitop/pma/ultrasonic_sensor.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-01-04 14:16:56.232524 pitop-0.8.1/pitop/protoplus/
+-rw-r--r--   0 runner    (1001) docker     (121)       62 2021-01-04 14:16:45.000000 pitop-0.8.1/pitop/protoplus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2152 2021-01-04 14:16:45.000000 pitop-0.8.1/pitop/protoplus/adc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2499 2021-01-04 14:16:45.000000 pitop-0.8.1/pitop/protoplus/sensors.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-01-04 14:16:56.236524 pitop-0.8.1/pitop/pulse/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-01-04 14:16:45.000000 pitop-0.8.1/pitop/pulse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5842 2021-01-04 14:16:45.000000 pitop-0.8.1/pitop/pulse/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16813 2021-01-04 14:16:45.000000 pitop-0.8.1/pitop/pulse/ledmatrix.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8981 2021-01-04 14:16:45.000000 pitop-0.8.1/pitop/pulse/microphone.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-01-04 14:16:56.236524 pitop-0.8.1/pitop/system/
+-rw-r--r--   0 runner    (1001) docker     (121)      285 2021-01-04 14:16:45.000000 pitop-0.8.1/pitop/system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      265 2021-01-04 14:16:45.000000 pitop-0.8.1/pitop/system/daemon.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1693 2021-01-04 14:16:45.000000 pitop-0.8.1/pitop/system/device.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3509 2021-01-04 14:16:45.000000 pitop-0.8.1/pitop/system/peripherals.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-01-04 14:16:56.220523 pitop-0.8.1/pitop.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     7993 2021-01-04 14:16:56.000000 pitop-0.8.1/pitop.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2700 2021-01-04 14:16:56.000000 pitop-0.8.1/pitop.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-01-04 14:16:56.000000 pitop-0.8.1/pitop.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      248 2021-01-04 14:16:56.000000 pitop-0.8.1/pitop.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      213 2021-01-04 14:16:56.000000 pitop-0.8.1/pitop.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       15 2021-01-04 14:16:56.000000 pitop-0.8.1/pitop.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-01-04 14:16:56.236524 pitop-0.8.1/pitopcli/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-01-04 14:16:45.000000 pitop-0.8.1/pitopcli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2983 2021-01-04 14:16:45.000000 pitop-0.8.1/pitopcli/battery.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1331 2021-01-04 14:16:45.000000 pitop-0.8.1/pitopcli/cli_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1904 2021-01-04 14:16:45.000000 pitop-0.8.1/pitopcli/deprecated_cli_runner.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4247 2021-01-04 14:16:45.000000 pitop-0.8.1/pitopcli/devices.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5166 2021-01-04 14:16:45.000000 pitop-0.8.1/pitopcli/display.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2381 2021-01-04 14:16:45.000000 pitop-0.8.1/pitopcli/imu.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13281 2021-01-04 14:16:45.000000 pitop-0.8.1/pitopcli/imu_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3490 2021-01-04 14:16:45.000000 pitop-0.8.1/pitopcli/oled.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2026 2021-01-04 14:16:45.000000 pitop-0.8.1/pitopcli/pitop.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4402 2021-01-04 14:16:45.000000 pitop-0.8.1/pitopcli/support.py
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-01-04 14:16:56.236524 pitop-0.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     4512 2021-01-04 14:16:45.000000 pitop-0.8.1/setup.py
```

### Comparing `pitop-0.7.0/PKG-INFO` & `pitop-0.8.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,37 @@
 Metadata-Version: 2.1
 Name: pitop
-Version: 0.7.0
+Version: 0.8.1
 Summary: pi-top Python SDK
 Home-page: https://github.com/pi-top/pi-top-Python-SDK
 Author: pi-top
 Author-email: deb-maintainers@pi-top.com
 License: Apache Software License
 Description: ===========================
         pi-top Python SDK (Preview)
         ===========================
         
         A simple, modular interface for interacting with a pi-top and its related accessories and components.
         
+        .. ###############################################
+        .. # NOTE: THESE ARE EXTERNAL LINKS, AS THEY ARE #
+        .. # REQUIRED FOR THE IMAGES TO SHOW ON PYPI     #
+        .. ###############################################
+        
         Supports all pi-top devices:
         
-        .. image:: docs/_static/overview/devices.jpg
+        .. image:: https://github.com/pi-top/pi-top-Python-SDK/raw/master/docs/_static/overview/devices.jpg
         
         Supports pi-top Maker Architecture (PMA):
         
-        .. image:: docs/_static/overview/pma.jpg
+        .. image:: https://github.com/pi-top/pi-top-Python-SDK/raw/master/docs/_static/overview/pma.jpg
         
         Supports all pi-top peripherals:
         
-        .. image:: docs/_static/overview/peripherals.jpg
+        .. image:: https://github.com/pi-top/pi-top-Python-SDK/raw/master/docs/_static/overview/peripherals.jpg
         
         --------------------------
         Status: Active Development
         --------------------------
         
         This SDK is currently in active development. Please be patient while we work towards v1.0.0!
         
@@ -38,14 +43,18 @@
         --------------------
         Build Status: Latest
         --------------------
         
         .. image:: https://img.shields.io/github/workflow/status/pi-top/pi-top-Python-SDK/Build,%20Test%20and%20Publish
            :alt: GitHub Workflow Status
         
+        
+        .. image:: https://img.shields.io/github/v/tag/pi-top/pi-top-Python-SDK
+            :alt: GitHub tag (latest by date)
+        
         .. image:: https://img.shields.io/github/v/release/pi-top/pi-top-Python-SDK
             :alt: GitHub release (latest by date)
         
         .. image:: https://img.shields.io/pypi/v/pitop
            :alt: PyPI release
         
         .. image:: https://readthedocs.com/projects/pi-top-pi-top-python-sdk/badge/?version=latest&token=13589f150cf192dcfc6ebfd53aae33164450aafd181c5e49018a21fd93149127
```

### Comparing `pitop-0.7.0/README.rst` & `pitop-0.8.1/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 ===========================
 pi-top Python SDK (Preview)
 ===========================
 
 A simple, modular interface for interacting with a pi-top and its related accessories and components.
 
+.. ###############################################
+.. # NOTE: THESE ARE EXTERNAL LINKS, AS THEY ARE #
+.. # REQUIRED FOR THE IMAGES TO SHOW ON PYPI     #
+.. ###############################################
+
 Supports all pi-top devices:
 
-.. image:: docs/_static/overview/devices.jpg
+.. image:: https://github.com/pi-top/pi-top-Python-SDK/raw/master/docs/_static/overview/devices.jpg
 
 Supports pi-top Maker Architecture (PMA):
 
-.. image:: docs/_static/overview/pma.jpg
+.. image:: https://github.com/pi-top/pi-top-Python-SDK/raw/master/docs/_static/overview/pma.jpg
 
 Supports all pi-top peripherals:
 
-.. image:: docs/_static/overview/peripherals.jpg
+.. image:: https://github.com/pi-top/pi-top-Python-SDK/raw/master/docs/_static/overview/peripherals.jpg
 
 --------------------------
 Status: Active Development
 --------------------------
 
 This SDK is currently in active development. Please be patient while we work towards v1.0.0!
 
@@ -30,14 +35,18 @@
 --------------------
 Build Status: Latest
 --------------------
 
 .. image:: https://img.shields.io/github/workflow/status/pi-top/pi-top-Python-SDK/Build,%20Test%20and%20Publish
    :alt: GitHub Workflow Status
 
+
+.. image:: https://img.shields.io/github/v/tag/pi-top/pi-top-Python-SDK
+    :alt: GitHub tag (latest by date)
+
 .. image:: https://img.shields.io/github/v/release/pi-top/pi-top-Python-SDK
     :alt: GitHub release (latest by date)
 
 .. image:: https://img.shields.io/pypi/v/pitop
    :alt: PyPI release
 
 .. image:: https://readthedocs.com/projects/pi-top-pi-top-python-sdk/badge/?version=latest&token=13589f150cf192dcfc6ebfd53aae33164450aafd181c5e49018a21fd93149127
```

### Comparing `pitop-0.7.0/pitop/battery/battery.py` & `pitop-0.8.1/pitop/battery/battery.py`

 * *Files identical despite different names*

### Comparing `pitop-0.7.0/pitop/camera/camera.py` & `pitop-0.8.1/pitop/camera/camera.py`

 * *Files identical despite different names*

### Comparing `pitop-0.7.0/pitop/camera/core/cameras/file_system_camera.py` & `pitop-0.8.1/pitop/camera/core/cameras/file_system_camera.py`

 * *Files identical despite different names*

### Comparing `pitop-0.7.0/pitop/camera/core/cameras/usb_camera.py` & `pitop-0.8.1/pitop/camera/core/cameras/usb_camera.py`

 * *Files identical despite different names*

### Comparing `pitop-0.7.0/pitop/camera/core/capture_actions/capture_action_base.py` & `pitop-0.8.1/pitop/camera/core/capture_actions/capture_action_base.py`

 * *Files identical despite different names*

### Comparing `pitop-0.7.0/pitop/camera/core/capture_actions/generic_action.py` & `pitop-0.8.1/pitop/camera/core/capture_actions/generic_action.py`

 * *Files identical despite different names*

### Comparing `pitop-0.7.0/pitop/camera/core/capture_actions/motion_detector.py` & `pitop-0.8.1/pitop/camera/core/capture_actions/motion_detector.py`

 * *Files identical despite different names*

### Comparing `pitop-0.7.0/pitop/camera/core/capture_actions/store_frame.py` & `pitop-0.8.1/pitop/camera/core/capture_actions/store_frame.py`

 * *Files identical despite different names*

### Comparing `pitop-0.7.0/pitop/camera/core/capture_actions/video_capture.py` & `pitop-0.8.1/pitop/camera/core/capture_actions/video_capture.py`

 * *Files identical despite different names*

### Comparing `pitop-0.7.0/pitop/camera/core/frame_handler.py` & `pitop-0.8.1/pitop/camera/core/frame_handler.py`

 * *Files identical despite different names*

### Comparing `pitop-0.7.0/pitop/camera/pil_opencv_conversion.py` & `pitop-0.8.1/pitop/camera/pil_opencv_conversion.py`

 * *Files identical despite different names*

### Comparing `pitop-0.7.0/pitop/display/display.py` & `pitop-0.8.1/pitop/display/display.py`

 * *Files identical despite different names*

### Comparing `pitop-0.7.0/pitop/keyboard/key_listener.py` & `pitop-0.8.1/pitop/keyboard/key_listener.py`

 * *Files identical despite different names*

### Comparing `pitop-0.7.0/pitop/miniscreen/buttons/buttons.py` & `pitop-0.8.1/pitop/miniscreen/buttons/buttons.py`

 * *Files identical despite different names*

### Comparing `pitop-0.7.0/pitop/miniscreen/oled/core/canvas.py` & `pitop-0.8.1/pitop/miniscreen/oled/core/canvas.py`

 * *Files identical despite different names*

### Comparing `pitop-0.7.0/pitop/miniscreen/oled/core/controls.py` & `pitop-0.8.1/pitop/miniscreen/oled/core/controls.py`

 * *Files identical despite different names*

### Comparing `pitop-0.7.0/pitop/miniscreen/oled/core/fps_regulator.py` & `pitop-0.8.1/pitop/miniscreen/oled/core/fps_regulator.py`

 * *Files identical despite different names*

### Comparing `pitop-0.7.0/pitop/miniscreen/oled/core/image_helper.py` & `pitop-0.8.1/pitop/miniscreen/oled/core/image_helper.py`

 * *Files identical despite different names*

### Comparing `pitop-0.7.0/pitop/miniscreen/oled/oled.py` & `pitop-0.8.1/pitop/miniscreen/oled/oled.py`

 * *Files identical despite different names*

### Comparing `pitop-0.7.0/pitop/pma/adc_base.py` & `pitop-0.8.1/pitop/pma/adc_base.py`

 * *Files identical despite different names*

### Comparing `pitop-0.7.0/pitop/pma/button.py` & `pitop-0.8.1/pitop/pma/button.py`

 * *Files identical despite different names*

### Comparing `pitop-0.7.0/pitop/pma/buzzer.py` & `pitop-0.8.1/pitop/pma/buzzer.py`

 * *Files identical despite different names*

### Comparing `pitop-0.7.0/pitop/pma/common/encoder_motor_registers.py` & `pitop-0.8.1/pitop/pma/common/encoder_motor_registers.py`

 * *Files identical despite different names*

### Comparing `pitop-0.7.0/pitop/pma/common/imu_registers.py` & `pitop-0.8.1/pitop/pma/common/imu_registers.py`

 * *Files identical despite different names*

### Comparing `pitop-0.7.0/pitop/pma/common/math_functions/ellipsoid_functions.py` & `pitop-0.8.1/pitop/pma/common/math_functions/ellipsoid_functions.py`

 * *Files identical despite different names*

### Comparing `pitop-0.7.0/pitop/pma/common/servo_motor_registers.py` & `pitop-0.8.1/pitop/pma/common/servo_motor_registers.py`

 * *Files identical despite different names*

### Comparing `pitop-0.7.0/pitop/pma/common/utils.py` & `pitop-0.8.1/pitop/pma/common/utils.py`

 * *Files identical despite different names*

### Comparing `pitop-0.7.0/pitop/pma/encoder_motor.py` & `pitop-0.8.1/pitop/pma/encoder_motor.py`

 * *Files identical despite different names*

### Comparing `pitop-0.7.0/pitop/pma/encoder_motor_controller.py` & `pitop-0.8.1/pitop/pma/encoder_motor_controller.py`

 * *Files identical despite different names*

### Comparing `pitop-0.7.0/pitop/pma/imu.py` & `pitop-0.8.1/pitop/pma/imu.py`

 * *Files identical despite different names*

### Comparing `pitop-0.7.0/pitop/pma/imu_controller.py` & `pitop-0.8.1/pitop/pma/imu_controller.py`

 * *Files identical despite different names*

### Comparing `pitop-0.7.0/pitop/pma/led.py` & `pitop-0.8.1/pitop/pma/led.py`

 * *Files identical despite different names*

### Comparing `pitop-0.7.0/pitop/pma/light_sensor.py` & `pitop-0.8.1/pitop/pma/light_sensor.py`

 * *Files identical despite different names*

### Comparing `pitop-0.7.0/pitop/pma/plate_interface.py` & `pitop-0.8.1/pitop/pma/plate_interface.py`

 * *Files identical despite different names*

### Comparing `pitop-0.7.0/pitop/pma/potentiometer.py` & `pitop-0.8.1/pitop/pma/potentiometer.py`

 * *Files identical despite different names*

### Comparing `pitop-0.7.0/pitop/pma/servo_controller.py` & `pitop-0.8.1/pitop/pma/servo_controller.py`

 * *Files identical despite different names*

### Comparing `pitop-0.7.0/pitop/pma/servo_motor.py` & `pitop-0.8.1/pitop/pma/servo_motor.py`

 * *Files identical despite different names*

### Comparing `pitop-0.7.0/pitop/pma/sound_sensor.py` & `pitop-0.8.1/pitop/pma/sound_sensor.py`

 * *Files identical despite different names*

### Comparing `pitop-0.7.0/pitop/pma/ultrasonic_sensor.py` & `pitop-0.8.1/pitop/pma/ultrasonic_sensor.py`

 * *Files identical despite different names*

### Comparing `pitop-0.7.0/pitop/protoplus/adc.py` & `pitop-0.8.1/pitop/protoplus/adc.py`

 * *Files identical despite different names*

### Comparing `pitop-0.7.0/pitop/protoplus/sensors.py` & `pitop-0.8.1/pitop/protoplus/sensors.py`

 * *Files identical despite different names*

### Comparing `pitop-0.7.0/pitop/pulse/configuration.py` & `pitop-0.8.1/pitop/pulse/configuration.py`

 * *Files identical despite different names*

### Comparing `pitop-0.7.0/pitop/pulse/ledmatrix.py` & `pitop-0.8.1/pitop/pulse/ledmatrix.py`

 * *Files identical despite different names*

### Comparing `pitop-0.7.0/pitop/pulse/microphone.py` & `pitop-0.8.1/pitop/pulse/microphone.py`

 * *Files identical despite different names*

### Comparing `pitop-0.7.0/pitop/system/device.py` & `pitop-0.8.1/pitop/system/device.py`

 * *Files identical despite different names*

### Comparing `pitop-0.7.0/pitop/system/peripherals.py` & `pitop-0.8.1/pitop/system/peripherals.py`

 * *Files identical despite different names*

### Comparing `pitop-0.7.0/pitop.egg-info/PKG-INFO` & `pitop-0.8.1/pitop.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,37 @@
 Metadata-Version: 2.1
 Name: pitop
-Version: 0.7.0
+Version: 0.8.1
 Summary: pi-top Python SDK
 Home-page: https://github.com/pi-top/pi-top-Python-SDK
 Author: pi-top
 Author-email: deb-maintainers@pi-top.com
 License: Apache Software License
 Description: ===========================
         pi-top Python SDK (Preview)
         ===========================
         
         A simple, modular interface for interacting with a pi-top and its related accessories and components.
         
+        .. ###############################################
+        .. # NOTE: THESE ARE EXTERNAL LINKS, AS THEY ARE #
+        .. # REQUIRED FOR THE IMAGES TO SHOW ON PYPI     #
+        .. ###############################################
+        
         Supports all pi-top devices:
         
-        .. image:: docs/_static/overview/devices.jpg
+        .. image:: https://github.com/pi-top/pi-top-Python-SDK/raw/master/docs/_static/overview/devices.jpg
         
         Supports pi-top Maker Architecture (PMA):
         
-        .. image:: docs/_static/overview/pma.jpg
+        .. image:: https://github.com/pi-top/pi-top-Python-SDK/raw/master/docs/_static/overview/pma.jpg
         
         Supports all pi-top peripherals:
         
-        .. image:: docs/_static/overview/peripherals.jpg
+        .. image:: https://github.com/pi-top/pi-top-Python-SDK/raw/master/docs/_static/overview/peripherals.jpg
         
         --------------------------
         Status: Active Development
         --------------------------
         
         This SDK is currently in active development. Please be patient while we work towards v1.0.0!
         
@@ -38,14 +43,18 @@
         --------------------
         Build Status: Latest
         --------------------
         
         .. image:: https://img.shields.io/github/workflow/status/pi-top/pi-top-Python-SDK/Build,%20Test%20and%20Publish
            :alt: GitHub Workflow Status
         
+        
+        .. image:: https://img.shields.io/github/v/tag/pi-top/pi-top-Python-SDK
+            :alt: GitHub tag (latest by date)
+        
         .. image:: https://img.shields.io/github/v/release/pi-top/pi-top-Python-SDK
             :alt: GitHub release (latest by date)
         
         .. image:: https://img.shields.io/pypi/v/pitop
            :alt: PyPI release
         
         .. image:: https://readthedocs.com/projects/pi-top-pi-top-python-sdk/badge/?version=latest&token=13589f150cf192dcfc6ebfd53aae33164450aafd181c5e49018a21fd93149127
```

### Comparing `pitop-0.7.0/pitop.egg-info/SOURCES.txt` & `pitop-0.8.1/pitop.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -78,12 +78,12 @@
 pitop/system/peripherals.py
 pitopcli/__init__.py
 pitopcli/battery.py
 pitopcli/cli_base.py
 pitopcli/deprecated_cli_runner.py
 pitopcli/devices.py
 pitopcli/display.py
-pitopcli/help.py
 pitopcli/imu.py
 pitopcli/imu_calibration.py
 pitopcli/oled.py
-pitopcli/pitop.py
+pitopcli/pitop.py
+pitopcli/support.py
```

### Comparing `pitop-0.7.0/pitopcli/battery.py` & `pitop-0.8.1/pitopcli/battery.py`

 * *Files identical despite different names*

### Comparing `pitop-0.7.0/pitopcli/cli_base.py` & `pitop-0.8.1/pitopcli/cli_base.py`

 * *Files identical despite different names*

### Comparing `pitop-0.7.0/pitopcli/deprecated_cli_runner.py` & `pitop-0.8.1/pitopcli/deprecated_cli_runner.py`

 * *Files identical despite different names*

### Comparing `pitop-0.7.0/pitopcli/devices.py` & `pitop-0.8.1/pitopcli/devices.py`

 * *Files identical despite different names*

### Comparing `pitop-0.7.0/pitopcli/display.py` & `pitop-0.8.1/pitopcli/display.py`

 * *Files identical despite different names*

### Comparing `pitop-0.7.0/pitopcli/help.py` & `pitop-0.8.1/pitopcli/support.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 
 class StdoutFormat:
     BOLD = '\033[1m'
     ENDC = '\033[0m'
     GREEN = '\033[92m'
 
 
-class HelpCLI(CliBaseClass):
-    parser_help = "Find help for your device"
-    cli_name = 'docs'
+class SupportCLI(CliBaseClass):
+    parser_help = "Find resources to learn how to use your device and get help if needed."
+    cli_name = 'support'
 
     ONLINE_URI = "https://docs.pi-top.com/python-sdk/"
     LOCAL_URI = "/usr/share/doc/python3-pitop/html/index.html"
     KNOWLEDGE_BASE_URI = "https://knowledgebase.pi-top.com/"
     FORUM_URI = "https://forum.pi-top.com/"
 
     def __init__(self, args) -> None:
@@ -88,15 +88,15 @@
         else:
             print_docs()
             print_other()
         return 0
 
     @classmethod
     def add_parser_arguments(cls, parser) -> None:
-        subparser = parser.add_subparsers(title="pi-top help",
+        subparser = parser.add_subparsers(title="pi-top support",
                                           description=cls.parser_help,
                                           dest="help_subcommand")
 
         docs_parser = subparser.add_parser("docs", help="Find documentation")
         docs_parser.add_argument("--open", "-o",
                                  help="Open a browser with the documentation page",
                                  action="store_true"
```

### Comparing `pitop-0.7.0/pitopcli/imu.py` & `pitop-0.8.1/pitopcli/imu.py`

 * *Files identical despite different names*

### Comparing `pitop-0.7.0/pitopcli/imu_calibration.py` & `pitop-0.8.1/pitopcli/imu_calibration.py`

 * *Files identical despite different names*

### Comparing `pitop-0.7.0/pitopcli/oled.py` & `pitop-0.8.1/pitopcli/oled.py`

 * *Files identical despite different names*

### Comparing `pitop-0.7.0/pitopcli/pitop.py` & `pitop-0.8.1/pitopcli/pitop.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 from argparse import ArgumentParser
 from sys import exit
 
 from .battery import BatteryCLI
 from .cli_base import PitopCliException, PitopCliInvalidArgument
 from .display import DisplayCLI
 from .devices import DeviceCLI
-from .help import HelpCLI
+from .support import SupportCLI
 from .imu import ImuCLI
 from .oled import OledCLI
 
 
 lookup_dict = {
     "battery": BatteryCLI,
     "devices": DeviceCLI,
     "display": DisplayCLI,
-    "help": HelpCLI,
+    "support": SupportCLI,
     "imu": ImuCLI,
     "oled": OledCLI
 }
 
 
 def get_parser():
     """Configures the argument parser according to the CLI classes
```

### Comparing `pitop-0.7.0/setup.py` & `pitop-0.8.1/setup.py`

 * *Files identical despite different names*

