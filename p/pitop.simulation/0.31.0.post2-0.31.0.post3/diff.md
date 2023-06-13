# Comparing `tmp/pitop.simulation-0.31.0.post2.tar.gz` & `tmp/pitop.simulation-0.31.0.post3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pitop.simulation-0.31.0.post2.tar", last modified: Mon May 22 19:13:14 2023, max compression
+gzip compressed data, was "dist/pitop.simulation-0.31.0.post3.tar", last modified: Tue Jun 13 16:41:55 2023, max compression
```

## Comparing `pitop.simulation-0.31.0.post2.tar` & `pitop.simulation-0.31.0.post3.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:13:14.000000 pitop.simulation-0.31.0.post2/
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-22 19:12:55.000000 pitop.simulation-0.31.0.post2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1027 2023-05-22 19:13:14.000000 pitop.simulation-0.31.0.post2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      181 2023-05-22 19:12:55.000000 pitop.simulation-0.31.0.post2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:13:14.000000 pitop.simulation-0.31.0.post2/pitop/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:13:14.000000 pitop.simulation-0.31.0.post2/pitop/simulation/
--rw-r--r--   0 runner    (1001) docker     (122)      195 2023-05-22 19:12:55.000000 pitop.simulation-0.31.0.post2/pitop/simulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      160 2023-05-22 19:12:55.000000 pitop.simulation-0.31.0.post2/pitop/simulation/color.py
--rw-r--r--   0 runner    (1001) docker     (122)      310 2023-05-22 19:12:55.000000 pitop.simulation-0.31.0.post2/pitop/simulation/events.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:13:14.000000 pitop.simulation-0.31.0.post2/pitop/simulation/images/
--rw-r--r--   0 runner    (1001) docker     (122)     6176 2023-05-22 19:12:55.000000 pitop.simulation-0.31.0.post2/pitop/simulation/images/Button.png
--rw-r--r--   0 runner    (1001) docker     (122)     6304 2023-05-22 19:12:55.000000 pitop.simulation-0.31.0.post2/pitop/simulation/images/Button_pressed.png
--rw-r--r--   0 runner    (1001) docker     (122)     6353 2023-05-22 19:12:55.000000 pitop.simulation-0.31.0.post2/pitop/simulation/images/Buzzer.png
--rw-r--r--   0 runner    (1001) docker     (122)     5809 2023-05-22 19:12:55.000000 pitop.simulation-0.31.0.post2/pitop/simulation/images/LED_green_off.png
--rw-r--r--   0 runner    (1001) docker     (122)     6237 2023-05-22 19:12:55.000000 pitop.simulation-0.31.0.post2/pitop/simulation/images/LED_green_on.png
--rw-r--r--   0 runner    (1001) docker     (122)     5669 2023-05-22 19:12:55.000000 pitop.simulation-0.31.0.post2/pitop/simulation/images/LED_red_off.png
--rw-r--r--   0 runner    (1001) docker     (122)     5115 2023-05-22 19:12:55.000000 pitop.simulation-0.31.0.post2/pitop/simulation/images/LED_red_on.png
--rw-r--r--   0 runner    (1001) docker     (122)     5749 2023-05-22 19:12:55.000000 pitop.simulation-0.31.0.post2/pitop/simulation/images/LED_yellow_off.png
--rw-r--r--   0 runner    (1001) docker     (122)     5172 2023-05-22 19:12:55.000000 pitop.simulation-0.31.0.post2/pitop/simulation/images/LED_yellow_on.png
--rw-r--r--   0 runner    (1001) docker     (122)     7143 2023-05-22 19:12:55.000000 pitop.simulation-0.31.0.post2/pitop/simulation/images/LightSensor.png
--rw-r--r--   0 runner    (1001) docker     (122)   121264 2023-05-22 19:12:55.000000 pitop.simulation-0.31.0.post2/pitop/simulation/images/Pitop.png
--rw-r--r--   0 runner    (1001) docker     (122)     7857 2023-05-22 19:12:55.000000 pitop.simulation-0.31.0.post2/pitop/simulation/images/Potentiometer.png
--rw-r--r--   0 runner    (1001) docker     (122)     1866 2023-05-22 19:12:55.000000 pitop.simulation-0.31.0.post2/pitop/simulation/images/Readme.md
--rw-r--r--   0 runner    (1001) docker     (122)     9412 2023-05-22 19:12:55.000000 pitop.simulation-0.31.0.post2/pitop/simulation/images/SoundSensor.png
--rw-r--r--   0 runner    (1001) docker     (122)    14445 2023-05-22 19:12:56.000000 pitop.simulation-0.31.0.post2/pitop/simulation/images/UltrasonicSensor.png
--rw-r--r--   0 runner    (1001) docker     (122)      936 2023-05-22 19:12:56.000000 pitop.simulation-0.31.0.post2/pitop/simulation/images/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      566 2023-05-22 19:12:56.000000 pitop.simulation-0.31.0.post2/pitop/simulation/images/angle_icon.png
--rw-r--r--   0 runner    (1001) docker     (122)     2352 2023-05-22 19:12:56.000000 pitop.simulation-0.31.0.post2/pitop/simulation/images/buzzer_sound_icon.png
--rw-r--r--   0 runner    (1001) docker     (122)      655 2023-05-22 19:12:56.000000 pitop.simulation-0.31.0.post2/pitop/simulation/images/distance_icon.png
--rw-r--r--   0 runner    (1001) docker     (122)     1128 2023-05-22 19:12:56.000000 pitop.simulation-0.31.0.post2/pitop/simulation/images/lightbulb_icon.png
--rw-r--r--   0 runner    (1001) docker     (122)      685 2023-05-22 19:12:56.000000 pitop.simulation-0.31.0.post2/pitop/simulation/images/speaker_icon.png
--rw-r--r--   0 runner    (1001) docker     (122)     1714 2023-05-22 19:12:56.000000 pitop.simulation-0.31.0.post2/pitop/simulation/port_label.py
--rw-r--r--   0 runner    (1001) docker     (122)     4685 2023-05-22 19:12:56.000000 pitop.simulation-0.31.0.post2/pitop/simulation/simsprite.py
--rw-r--r--   0 runner    (1001) docker     (122)     9453 2023-05-22 19:12:56.000000 pitop.simulation-0.31.0.post2/pitop/simulation/simulation.py
--rw-r--r--   0 runner    (1001) docker     (122)    12342 2023-05-22 19:12:56.000000 pitop.simulation-0.31.0.post2/pitop/simulation/sprites.py
--rw-r--r--   0 runner    (1001) docker     (122)       80 2023-05-22 19:12:56.000000 pitop.simulation-0.31.0.post2/pitop/simulation/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:13:14.000000 pitop.simulation-0.31.0.post2/pitop/simulation/virtual_hardware/
--rw-r--r--   0 runner    (1001) docker     (122)      497 2023-05-22 19:12:56.000000 pitop.simulation-0.31.0.post2/pitop/simulation/virtual_hardware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      863 2023-05-22 19:12:56.000000 pitop.simulation-0.31.0.post2/pitop/simulation/virtual_hardware/fonts.py
--rw-r--r--   0 runner    (1001) docker     (122)     2610 2023-05-22 19:12:56.000000 pitop.simulation-0.31.0.post2/pitop/simulation/virtual_hardware/pitop.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:13:14.000000 pitop.simulation-0.31.0.post2/pitop/simulation/virtual_hardware/vendor/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:13:14.000000 pitop.simulation-0.31.0.post2/pitop/simulation/virtual_hardware/vendor/Mock/
--rw-r--r--   0 runner    (1001) docker     (122)     8181 2023-05-22 19:12:56.000000 pitop.simulation-0.31.0.post2/pitop/simulation/virtual_hardware/vendor/Mock/GPIO.py
--rw-r--r--   0 runner    (1001) docker     (122)       22 2023-05-22 19:12:56.000000 pitop.simulation-0.31.0.post2/pitop/simulation/virtual_hardware/vendor/Mock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-22 19:12:56.000000 pitop.simulation-0.31.0.post2/pitop/simulation/virtual_hardware/vendor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:13:14.000000 pitop.simulation-0.31.0.post2/pitop/simulation/widgets/
--rw-r--r--   0 runner    (1001) docker     (122)       77 2023-05-22 19:12:56.000000 pitop.simulation-0.31.0.post2/pitop/simulation/widgets/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     4969 2023-05-22 19:12:56.000000 pitop.simulation-0.31.0.post2/pitop/simulation/widgets/slider.py
--rw-r--r--   0 runner    (1001) docker     (122)     2123 2023-05-22 19:12:56.000000 pitop.simulation-0.31.0.post2/pitop/simulation/widgets/widget.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:13:14.000000 pitop.simulation-0.31.0.post2/pitop.simulation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1027 2023-05-22 19:13:14.000000 pitop.simulation-0.31.0.post2/pitop.simulation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1702 2023-05-22 19:13:14.000000 pitop.simulation-0.31.0.post2/pitop.simulation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-22 19:13:14.000000 pitop.simulation-0.31.0.post2/pitop.simulation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       57 2023-05-22 19:13:14.000000 pitop.simulation-0.31.0.post2/pitop.simulation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-05-22 19:13:14.000000 pitop.simulation-0.31.0.post2/pitop.simulation.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-22 19:13:14.000000 pitop.simulation-0.31.0.post2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1989 2023-05-22 19:12:56.000000 pitop.simulation-0.31.0.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 16:41:55.000000 pitop.simulation-0.31.0.post3/
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-13 16:41:37.000000 pitop.simulation-0.31.0.post3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1027 2023-06-13 16:41:55.000000 pitop.simulation-0.31.0.post3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      181 2023-06-13 16:41:37.000000 pitop.simulation-0.31.0.post3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 16:41:55.000000 pitop.simulation-0.31.0.post3/pitop/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 16:41:55.000000 pitop.simulation-0.31.0.post3/pitop/simulation/
+-rw-r--r--   0 runner    (1001) docker     (122)      195 2023-06-13 16:41:37.000000 pitop.simulation-0.31.0.post3/pitop/simulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      160 2023-06-13 16:41:37.000000 pitop.simulation-0.31.0.post3/pitop/simulation/color.py
+-rw-r--r--   0 runner    (1001) docker     (122)      310 2023-06-13 16:41:37.000000 pitop.simulation-0.31.0.post3/pitop/simulation/events.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 16:41:55.000000 pitop.simulation-0.31.0.post3/pitop/simulation/images/
+-rw-r--r--   0 runner    (1001) docker     (122)     6176 2023-06-13 16:41:37.000000 pitop.simulation-0.31.0.post3/pitop/simulation/images/Button.png
+-rw-r--r--   0 runner    (1001) docker     (122)     6304 2023-06-13 16:41:37.000000 pitop.simulation-0.31.0.post3/pitop/simulation/images/Button_pressed.png
+-rw-r--r--   0 runner    (1001) docker     (122)     6353 2023-06-13 16:41:37.000000 pitop.simulation-0.31.0.post3/pitop/simulation/images/Buzzer.png
+-rw-r--r--   0 runner    (1001) docker     (122)     5809 2023-06-13 16:41:37.000000 pitop.simulation-0.31.0.post3/pitop/simulation/images/LED_green_off.png
+-rw-r--r--   0 runner    (1001) docker     (122)     6237 2023-06-13 16:41:37.000000 pitop.simulation-0.31.0.post3/pitop/simulation/images/LED_green_on.png
+-rw-r--r--   0 runner    (1001) docker     (122)     5669 2023-06-13 16:41:37.000000 pitop.simulation-0.31.0.post3/pitop/simulation/images/LED_red_off.png
+-rw-r--r--   0 runner    (1001) docker     (122)     5115 2023-06-13 16:41:37.000000 pitop.simulation-0.31.0.post3/pitop/simulation/images/LED_red_on.png
+-rw-r--r--   0 runner    (1001) docker     (122)     5749 2023-06-13 16:41:37.000000 pitop.simulation-0.31.0.post3/pitop/simulation/images/LED_yellow_off.png
+-rw-r--r--   0 runner    (1001) docker     (122)     5172 2023-06-13 16:41:37.000000 pitop.simulation-0.31.0.post3/pitop/simulation/images/LED_yellow_on.png
+-rw-r--r--   0 runner    (1001) docker     (122)     7143 2023-06-13 16:41:37.000000 pitop.simulation-0.31.0.post3/pitop/simulation/images/LightSensor.png
+-rw-r--r--   0 runner    (1001) docker     (122)   121264 2023-06-13 16:41:37.000000 pitop.simulation-0.31.0.post3/pitop/simulation/images/Pitop.png
+-rw-r--r--   0 runner    (1001) docker     (122)     7857 2023-06-13 16:41:37.000000 pitop.simulation-0.31.0.post3/pitop/simulation/images/Potentiometer.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1866 2023-06-13 16:41:37.000000 pitop.simulation-0.31.0.post3/pitop/simulation/images/Readme.md
+-rw-r--r--   0 runner    (1001) docker     (122)     9412 2023-06-13 16:41:37.000000 pitop.simulation-0.31.0.post3/pitop/simulation/images/SoundSensor.png
+-rw-r--r--   0 runner    (1001) docker     (122)    14445 2023-06-13 16:41:37.000000 pitop.simulation-0.31.0.post3/pitop/simulation/images/UltrasonicSensor.png
+-rw-r--r--   0 runner    (1001) docker     (122)      936 2023-06-13 16:41:37.000000 pitop.simulation-0.31.0.post3/pitop/simulation/images/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      566 2023-06-13 16:41:37.000000 pitop.simulation-0.31.0.post3/pitop/simulation/images/angle_icon.png
+-rw-r--r--   0 runner    (1001) docker     (122)     2352 2023-06-13 16:41:37.000000 pitop.simulation-0.31.0.post3/pitop/simulation/images/buzzer_sound_icon.png
+-rw-r--r--   0 runner    (1001) docker     (122)      655 2023-06-13 16:41:37.000000 pitop.simulation-0.31.0.post3/pitop/simulation/images/distance_icon.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1128 2023-06-13 16:41:37.000000 pitop.simulation-0.31.0.post3/pitop/simulation/images/lightbulb_icon.png
+-rw-r--r--   0 runner    (1001) docker     (122)      685 2023-06-13 16:41:37.000000 pitop.simulation-0.31.0.post3/pitop/simulation/images/speaker_icon.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1714 2023-06-13 16:41:37.000000 pitop.simulation-0.31.0.post3/pitop/simulation/port_label.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4685 2023-06-13 16:41:37.000000 pitop.simulation-0.31.0.post3/pitop/simulation/simsprite.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9453 2023-06-13 16:41:37.000000 pitop.simulation-0.31.0.post3/pitop/simulation/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12342 2023-06-13 16:41:37.000000 pitop.simulation-0.31.0.post3/pitop/simulation/sprites.py
+-rw-r--r--   0 runner    (1001) docker     (122)       80 2023-06-13 16:41:37.000000 pitop.simulation-0.31.0.post3/pitop/simulation/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 16:41:55.000000 pitop.simulation-0.31.0.post3/pitop/simulation/virtual_hardware/
+-rw-r--r--   0 runner    (1001) docker     (122)      497 2023-06-13 16:41:37.000000 pitop.simulation-0.31.0.post3/pitop/simulation/virtual_hardware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      863 2023-06-13 16:41:37.000000 pitop.simulation-0.31.0.post3/pitop/simulation/virtual_hardware/fonts.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2610 2023-06-13 16:41:37.000000 pitop.simulation-0.31.0.post3/pitop/simulation/virtual_hardware/pitop.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 16:41:55.000000 pitop.simulation-0.31.0.post3/pitop/simulation/virtual_hardware/vendor/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 16:41:55.000000 pitop.simulation-0.31.0.post3/pitop/simulation/virtual_hardware/vendor/Mock/
+-rw-r--r--   0 runner    (1001) docker     (122)     8181 2023-06-13 16:41:37.000000 pitop.simulation-0.31.0.post3/pitop/simulation/virtual_hardware/vendor/Mock/GPIO.py
+-rw-r--r--   0 runner    (1001) docker     (122)       22 2023-06-13 16:41:37.000000 pitop.simulation-0.31.0.post3/pitop/simulation/virtual_hardware/vendor/Mock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-13 16:41:37.000000 pitop.simulation-0.31.0.post3/pitop/simulation/virtual_hardware/vendor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 16:41:55.000000 pitop.simulation-0.31.0.post3/pitop/simulation/widgets/
+-rw-r--r--   0 runner    (1001) docker     (122)       77 2023-06-13 16:41:37.000000 pitop.simulation-0.31.0.post3/pitop/simulation/widgets/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     4969 2023-06-13 16:41:37.000000 pitop.simulation-0.31.0.post3/pitop/simulation/widgets/slider.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2123 2023-06-13 16:41:37.000000 pitop.simulation-0.31.0.post3/pitop/simulation/widgets/widget.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 16:41:55.000000 pitop.simulation-0.31.0.post3/pitop.simulation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1027 2023-06-13 16:41:55.000000 pitop.simulation-0.31.0.post3/pitop.simulation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1702 2023-06-13 16:41:55.000000 pitop.simulation-0.31.0.post3/pitop.simulation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-13 16:41:55.000000 pitop.simulation-0.31.0.post3/pitop.simulation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       57 2023-06-13 16:41:55.000000 pitop.simulation-0.31.0.post3/pitop.simulation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-06-13 16:41:55.000000 pitop.simulation-0.31.0.post3/pitop.simulation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-13 16:41:55.000000 pitop.simulation-0.31.0.post3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1989 2023-06-13 16:41:37.000000 pitop.simulation-0.31.0.post3/setup.py
```

### Comparing `pitop.simulation-0.31.0.post2/PKG-INFO` & `pitop.simulation-0.31.0.post3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pitop.simulation
-Version: 0.31.0.post2
+Version: 0.31.0.post3
 Summary: pi-top Python SDK.
 Home-page: https://github.com/pi-top/pi-top-Python-SDK
 Author: pi-top
 Author-email: deb-maintainers@pi-top.com
 License: Apache Software License
 Description: ===========================
         pi-top Python Simulation
```

### Comparing `pitop.simulation-0.31.0.post2/pitop/simulation/images/Button.png` & `pitop.simulation-0.31.0.post3/pitop/simulation/images/Button.png`

 * *Files identical despite different names*

### Comparing `pitop.simulation-0.31.0.post2/pitop/simulation/images/Button_pressed.png` & `pitop.simulation-0.31.0.post3/pitop/simulation/images/Button_pressed.png`

 * *Files identical despite different names*

### Comparing `pitop.simulation-0.31.0.post2/pitop/simulation/images/Buzzer.png` & `pitop.simulation-0.31.0.post3/pitop/simulation/images/Buzzer.png`

 * *Files identical despite different names*

### Comparing `pitop.simulation-0.31.0.post2/pitop/simulation/images/LED_green_off.png` & `pitop.simulation-0.31.0.post3/pitop/simulation/images/LED_green_off.png`

 * *Files identical despite different names*

### Comparing `pitop.simulation-0.31.0.post2/pitop/simulation/images/LED_green_on.png` & `pitop.simulation-0.31.0.post3/pitop/simulation/images/LED_green_on.png`

 * *Files identical despite different names*

### Comparing `pitop.simulation-0.31.0.post2/pitop/simulation/images/LED_red_off.png` & `pitop.simulation-0.31.0.post3/pitop/simulation/images/LED_red_off.png`

 * *Files identical despite different names*

### Comparing `pitop.simulation-0.31.0.post2/pitop/simulation/images/LED_red_on.png` & `pitop.simulation-0.31.0.post3/pitop/simulation/images/LED_red_on.png`

 * *Files identical despite different names*

### Comparing `pitop.simulation-0.31.0.post2/pitop/simulation/images/LED_yellow_off.png` & `pitop.simulation-0.31.0.post3/pitop/simulation/images/LED_yellow_off.png`

 * *Files identical despite different names*

### Comparing `pitop.simulation-0.31.0.post2/pitop/simulation/images/LED_yellow_on.png` & `pitop.simulation-0.31.0.post3/pitop/simulation/images/LED_yellow_on.png`

 * *Files identical despite different names*

### Comparing `pitop.simulation-0.31.0.post2/pitop/simulation/images/LightSensor.png` & `pitop.simulation-0.31.0.post3/pitop/simulation/images/LightSensor.png`

 * *Files identical despite different names*

### Comparing `pitop.simulation-0.31.0.post2/pitop/simulation/images/Pitop.png` & `pitop.simulation-0.31.0.post3/pitop/simulation/images/Pitop.png`

 * *Files identical despite different names*

### Comparing `pitop.simulation-0.31.0.post2/pitop/simulation/images/Potentiometer.png` & `pitop.simulation-0.31.0.post3/pitop/simulation/images/Potentiometer.png`

 * *Files identical despite different names*

### Comparing `pitop.simulation-0.31.0.post2/pitop/simulation/images/Readme.md` & `pitop.simulation-0.31.0.post3/pitop/simulation/images/Readme.md`

 * *Files identical despite different names*

### Comparing `pitop.simulation-0.31.0.post2/pitop/simulation/images/SoundSensor.png` & `pitop.simulation-0.31.0.post3/pitop/simulation/images/SoundSensor.png`

 * *Files identical despite different names*

### Comparing `pitop.simulation-0.31.0.post2/pitop/simulation/images/UltrasonicSensor.png` & `pitop.simulation-0.31.0.post3/pitop/simulation/images/UltrasonicSensor.png`

 * *Files identical despite different names*

### Comparing `pitop.simulation-0.31.0.post2/pitop/simulation/images/__init__.py` & `pitop.simulation-0.31.0.post3/pitop/simulation/images/__init__.py`

 * *Files identical despite different names*

### Comparing `pitop.simulation-0.31.0.post2/pitop/simulation/images/angle_icon.png` & `pitop.simulation-0.31.0.post3/pitop/simulation/images/angle_icon.png`

 * *Files identical despite different names*

### Comparing `pitop.simulation-0.31.0.post2/pitop/simulation/images/buzzer_sound_icon.png` & `pitop.simulation-0.31.0.post3/pitop/simulation/images/buzzer_sound_icon.png`

 * *Files identical despite different names*

### Comparing `pitop.simulation-0.31.0.post2/pitop/simulation/images/distance_icon.png` & `pitop.simulation-0.31.0.post3/pitop/simulation/images/distance_icon.png`

 * *Files identical despite different names*

### Comparing `pitop.simulation-0.31.0.post2/pitop/simulation/images/lightbulb_icon.png` & `pitop.simulation-0.31.0.post3/pitop/simulation/images/lightbulb_icon.png`

 * *Files identical despite different names*

### Comparing `pitop.simulation-0.31.0.post2/pitop/simulation/images/speaker_icon.png` & `pitop.simulation-0.31.0.post3/pitop/simulation/images/speaker_icon.png`

 * *Files identical despite different names*

### Comparing `pitop.simulation-0.31.0.post2/pitop/simulation/port_label.py` & `pitop.simulation-0.31.0.post3/pitop/simulation/port_label.py`

 * *Files identical despite different names*

### Comparing `pitop.simulation-0.31.0.post2/pitop/simulation/simsprite.py` & `pitop.simulation-0.31.0.post3/pitop/simulation/simsprite.py`

 * *Files identical despite different names*

### Comparing `pitop.simulation-0.31.0.post2/pitop/simulation/simulation.py` & `pitop.simulation-0.31.0.post3/pitop/simulation/simulation.py`

 * *Files identical despite different names*

### Comparing `pitop.simulation-0.31.0.post2/pitop/simulation/sprites.py` & `pitop.simulation-0.31.0.post3/pitop/simulation/sprites.py`

 * *Files identical despite different names*

### Comparing `pitop.simulation-0.31.0.post2/pitop/simulation/virtual_hardware/fonts.py` & `pitop.simulation-0.31.0.post3/pitop/simulation/virtual_hardware/fonts.py`

 * *Files identical despite different names*

### Comparing `pitop.simulation-0.31.0.post2/pitop/simulation/virtual_hardware/pitop.py` & `pitop.simulation-0.31.0.post3/pitop/simulation/virtual_hardware/pitop.py`

 * *Files identical despite different names*

### Comparing `pitop.simulation-0.31.0.post2/pitop/simulation/virtual_hardware/vendor/Mock/GPIO.py` & `pitop.simulation-0.31.0.post3/pitop/simulation/virtual_hardware/vendor/Mock/GPIO.py`

 * *Files identical despite different names*

### Comparing `pitop.simulation-0.31.0.post2/pitop/simulation/widgets/slider.py` & `pitop.simulation-0.31.0.post3/pitop/simulation/widgets/slider.py`

 * *Files identical despite different names*

### Comparing `pitop.simulation-0.31.0.post2/pitop/simulation/widgets/widget.py` & `pitop.simulation-0.31.0.post3/pitop/simulation/widgets/widget.py`

 * *Files identical despite different names*

### Comparing `pitop.simulation-0.31.0.post2/pitop.simulation.egg-info/PKG-INFO` & `pitop.simulation-0.31.0.post3/pitop.simulation.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pitop.simulation
-Version: 0.31.0.post2
+Version: 0.31.0.post3
 Summary: pi-top Python SDK.
 Home-page: https://github.com/pi-top/pi-top-Python-SDK
 Author: pi-top
 Author-email: deb-maintainers@pi-top.com
 License: Apache Software License
 Description: ===========================
         pi-top Python Simulation
```

### Comparing `pitop.simulation-0.31.0.post2/pitop.simulation.egg-info/SOURCES.txt` & `pitop.simulation-0.31.0.post3/pitop.simulation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pitop.simulation-0.31.0.post2/setup.py` & `pitop.simulation-0.31.0.post3/setup.py`

 * *Files identical despite different names*

