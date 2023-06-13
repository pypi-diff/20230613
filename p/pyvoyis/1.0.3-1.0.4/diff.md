# Comparing `tmp/pyvoyis-1.0.3.tar.gz` & `tmp/pyvoyis-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvoyis-1.0.3.tar", last modified: Thu Jun  8 15:05:38 2023, max compression
+gzip compressed data, was "pyvoyis-1.0.4.tar", last modified: Tue Jun 13 08:24:11 2023, max compression
```

## Comparing `pyvoyis-1.0.3.tar` & `pyvoyis-1.0.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:05:38.779862 pyvoyis-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-08 15:05:29.000000 pyvoyis-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-06-08 15:05:38.779862 pyvoyis-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-06-08 15:05:29.000000 pyvoyis-1.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 15:05:38.779862 pyvoyis-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-06-08 15:05:29.000000 pyvoyis-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:05:38.779862 pyvoyis-1.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:05:38.779862 pyvoyis-1.0.3/src/pyvoyis/
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-08 15:05:29.000000 pyvoyis-1.0.3/src/pyvoyis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42832 2023-06-08 15:05:29.000000 pyvoyis-1.0.3/src/pyvoyis/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:05:38.779862 pyvoyis-1.0.3/src/pyvoyis/api500/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-08 15:05:29.000000 pyvoyis-1.0.3/src/pyvoyis/api500/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6343 2023-06-08 15:05:29.000000 pyvoyis-1.0.3/src/pyvoyis/api500/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-08 15:05:29.000000 pyvoyis-1.0.3/src/pyvoyis/api500/command.py
--rw-r--r--   0 runner    (1001) docker     (123)    57923 2023-06-08 15:05:29.000000 pyvoyis-1.0.3/src/pyvoyis/api500/defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-06-08 15:05:29.000000 pyvoyis-1.0.3/src/pyvoyis/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-06-08 15:05:29.000000 pyvoyis-1.0.3/src/pyvoyis/commander.py
--rw-r--r--   0 runner    (1001) docker     (123)     8111 2023-06-08 15:05:29.000000 pyvoyis-1.0.3/src/pyvoyis/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    15669 2023-06-08 15:05:29.000000 pyvoyis-1.0.3/src/pyvoyis/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-06-08 15:05:29.000000 pyvoyis-1.0.3/src/pyvoyis/state_machine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:05:38.779862 pyvoyis-1.0.3/src/pyvoyis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-06-08 15:05:38.000000 pyvoyis-1.0.3/src/pyvoyis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-08 15:05:38.000000 pyvoyis-1.0.3/src/pyvoyis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 15:05:38.000000 pyvoyis-1.0.3/src/pyvoyis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-08 15:05:38.000000 pyvoyis-1.0.3/src/pyvoyis.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-08 15:05:38.000000 pyvoyis-1.0.3/src/pyvoyis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-08 15:05:38.000000 pyvoyis-1.0.3/src/pyvoyis.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 08:24:11.032920 pyvoyis-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-13 08:24:02.000000 pyvoyis-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-06-13 08:24:11.032920 pyvoyis-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-06-13 08:24:02.000000 pyvoyis-1.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 08:24:11.032920 pyvoyis-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-06-13 08:24:02.000000 pyvoyis-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 08:24:11.024920 pyvoyis-1.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 08:24:11.028920 pyvoyis-1.0.4/src/pyvoyis/
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-13 08:24:02.000000 pyvoyis-1.0.4/src/pyvoyis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43532 2023-06-13 08:24:02.000000 pyvoyis-1.0.4/src/pyvoyis/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 08:24:11.032920 pyvoyis-1.0.4/src/pyvoyis/api500/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-13 08:24:02.000000 pyvoyis-1.0.4/src/pyvoyis/api500/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-06-13 08:24:02.000000 pyvoyis-1.0.4/src/pyvoyis/api500/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-13 08:24:02.000000 pyvoyis-1.0.4/src/pyvoyis/api500/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57924 2023-06-13 08:24:02.000000 pyvoyis-1.0.4/src/pyvoyis/api500/defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-13 08:24:02.000000 pyvoyis-1.0.4/src/pyvoyis/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-06-13 08:24:02.000000 pyvoyis-1.0.4/src/pyvoyis/commander.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10073 2023-06-13 08:24:02.000000 pyvoyis-1.0.4/src/pyvoyis/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15669 2023-06-13 08:24:02.000000 pyvoyis-1.0.4/src/pyvoyis/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-06-13 08:24:02.000000 pyvoyis-1.0.4/src/pyvoyis/state_machine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 08:24:11.032920 pyvoyis-1.0.4/src/pyvoyis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-06-13 08:24:11.000000 pyvoyis-1.0.4/src/pyvoyis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-13 08:24:11.000000 pyvoyis-1.0.4/src/pyvoyis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 08:24:11.000000 pyvoyis-1.0.4/src/pyvoyis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-13 08:24:11.000000 pyvoyis-1.0.4/src/pyvoyis.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-13 08:24:11.000000 pyvoyis-1.0.4/src/pyvoyis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-13 08:24:11.000000 pyvoyis-1.0.4/src/pyvoyis.egg-info/top_level.txt
```

### Comparing `pyvoyis-1.0.3/LICENSE` & `pyvoyis-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvoyis-1.0.3/PKG-INFO` & `pyvoyis-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvoyis
-Version: 1.0.3
+Version: 1.0.4
 Summary: Voyis Recon LS python driver
 Home-page: https://github.com/miquelmassot/pyvoyis
 Author: Miquel Massot
 Author-email: miquel.massot@gmail.com
 Maintainer: Miquel Massot
 Maintainer-email: miquel.massot@gmail.com
 License: GPLv3
```

### Comparing `pyvoyis-1.0.3/README.md` & `pyvoyis-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pyvoyis-1.0.3/setup.py` & `pyvoyis-1.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 # read the contents of README file
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="pyvoyis",
-    version="1.0.3",
+    version="1.0.4",
     description="Voyis Recon LS python driver",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Miquel Massot",
     author_email="miquel.massot@gmail.com",
     maintainer="Miquel Massot",
     maintainer_email="miquel.massot@gmail.com",
```

### Comparing `pyvoyis-1.0.3/src/pyvoyis/__init__.py` & `pyvoyis-1.0.4/src/pyvoyis/__init__.py`

 * *Files identical despite different names*

### Comparing `pyvoyis-1.0.3/src/pyvoyis/api.py` & `pyvoyis-1.0.4/src/pyvoyis/api.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,72 +2,73 @@
 Copyright (c) 2023, Miquel Massot
 All rights reserved.
 Licensed under the GPLv3 License.
 See LICENSE.md file in the project root for full license information.
 """
 
 import asyncio
+import datetime
 import logging
+import os
 import threading
 import time
 from pathlib import Path
 
 import nest_asyncio
+import yaml
 
-from pyvoyis.tools.custom_logger import setup_logging
 from pyvoyis.api500 import API500Client
 from pyvoyis.api500.defs import (
+    API_PARAM_STILLS_ADVANCED_ADAPTIVE_LIGHTING,
+    API_PARAM_STILLS_ADVANCED_BRIGHTNESS,
+    API_PARAM_STILLS_ADVANCED_COLOUR_ENHANCEMENT_LVL,
+    API_PARAM_STILLS_ADVANCED_COLOUR_MODE,
+    API_PARAM_STILLS_ADVANCED_CONTRAST,
+    API_PARAM_STILLS_ADVANCED_CONTRAST_LVL,
+    API_PARAM_STILLS_ADVANCED_CONTRAST_MODE,
+    API_PARAM_STILLS_ADVANCED_WHITE_BALANCE,
+    API_PARAM_STILLS_IMAGE_LEVEL,
     API_PARAM_STILLS_IMAGE_SAVE_ORIGINAL,
     API_PARAM_STILLS_IMAGE_UNDISTORT,
     API_PARAM_STILLS_PROCESSED_IMAGE_FORMAT,
     ENDPOINT_ID_LOG,
     ENDPOINT_ID_SENSOR_LASER,
     ENDPOINT_ID_SENSOR_STILLS_PROCESSED,
     ENDPOINT_ID_SENSOR_STILLS_RAW,
     ENDPOINT_ID_STREAM,
     ENDPOINT_ID_XYZ_LASER,
-    NAVPROTO_PSONNAV,
-    SCANNER_NOT_READY,
     SCANNER_CONNECTED_TO_THIS_API,
+    SCANNER_NOT_READY,
     SCANNER_PARAM_INDEX_OF_REFRACTION,
     SCANNER_PARAM_LASER_FREQ,
     SCANNER_PARAM_LASER_MAX_RANGE,
     SCANNER_PARAM_LASER_MIN_RANGE,
     SCANNER_PARAM_LASER_OUTPUT_GAIN,
     SCANNER_PARAM_LED_PANEL_INTENSITY,
     SCANNER_PARAM_MEMS_OUTPUT_ENABLE,
     SCANNER_PARAM_OUTPUT_LASER_DATA,
     SCANNER_PARAM_PROFILE_STILLS_EXP,
     SCANNER_PARAM_STILL_FREQ,
-    SCANNER_PARAM_STILLS_IMAGE_LEVEL,
     SCANNER_STATUS_CONNECTED,
     SCANNER_STATUS_CPU_TEMP_CH,
-    SCANNER_STATUS_CPU_TEMP_LASER,
-    SCANNER_STATUS_CPU_TEMP_STILLS,
-    SCANNER_STATUS_INTERNAL_TEMP_CH,
-    SCANNER_STATUS_INTERNAL_TEMP_LASER_SENSOR,
-    SCANNER_STATUS_INTERNAL_TEMP_STILLS_SENSOR,
     SCANNER_STATUS_LASER_CAMERA_CONNECTED,
     SCANNER_STATUS_LASER_CAMERA_READY,
     SCANNER_STATUS_LASER_CONNECTED,
     SCANNER_STATUS_LASER_DONGLE_AT_CH,
     SCANNER_STATUS_LASER_INHIBIT_ENABLED,
     SCANNER_STATUS_LASER_READY,
     SCANNER_STATUS_LASER_SAFETY_DISABLED,
     SCANNER_STATUS_LED_PANEL_CONNECTED,
     SCANNER_STATUS_LED_PANEL_READY,
     SCANNER_STATUS_READY,
     SCANNER_STATUS_SCAN_IN_PROGRESS,
-    SCANNER_STATUS_SENSOR_TEMP_LASER_SENSOR,
-    SCANNER_STATUS_SENSOR_TEMP_STILLS_SENSOR,
     SCANNER_STATUS_STILLS_CAMERA_CONNECTED,
     SCANNER_STATUS_STILLS_CAMERA_READY,
-    SOURCE_TCP_CLIENT,
-    SOURCE_TCP_SERVER,
     VALUE_TYPE_BOOL,
+    VALUE_TYPE_FLOAT,
     VALUE_TYPE_UINT,
     scanner_connection_to_str,
     str_to_navproto,
     str_to_network_source,
 )
 from pyvoyis.commander import VoyisCommander
 from pyvoyis.messages import (
@@ -88,40 +89,39 @@
     ScannerParameter,
     ScannerParametersNot,
     ScannerStatus,
     ScannerStatusNot,
 )
 from pyvoyis.state_machine import VoyisAPIStateMachine
 from pyvoyis.tools.bool2str import bool2str
-from pyvoyis.tools.str2bool import str2bool
+from pyvoyis.tools.custom_logger import setup_logging
 from pyvoyis.tools.rate import Rate
 from pyvoyis.tools.safe_get import safe_get
+from pyvoyis.tools.str2bool import str2bool
 
 nest_asyncio.apply()
 
 
 class VoyisAPI:
     def __init__(self, config):
         """Class to handle the Voyis API"""
         self.config = config
-        setup_logging(config.log_path)
+        self.ip = self.config.ip_address
+        self.port = self.config.port
 
-        print(self.config)
+        self.start_logging()
 
-        self.ip = config.ip_address
-        self.port = config.port
-        self.log = logging.getLogger("VoyisAPI")
         self.event = threading.Event()
         self.task_set = set()
 
         # Handle RuntimeError: There is no current event loop in thread 'Thread-1'.
         try:
             self.loop = asyncio.get_event_loop()
         except RuntimeError as e:
-            if str(e).startswith('There is no current event loop in thread'):
+            if str(e).startswith("There is no current event loop in thread"):
                 self.loop = asyncio.new_event_loop()
                 asyncio.set_event_loop(self.loop)
             else:
                 raise
 
         self.client = API500Client(self.ip, self.port, self.loop, self.task_set)
         self.state = VoyisAPIStateMachine()
@@ -144,14 +144,34 @@
         self.correction_model_list_not_list = []
         self.pending_cmd_status_not_list = []
         self.ack_rsp_list = []
 
         self._request_acquisition = False
         self._request_stop = False
 
+    def start_logging(self):
+        # Set default path and logging
+        bp = self.config.endpoint_id.base_path
+        current_date = datetime.datetime.now().strftime("%Y%m%d_%H%M%S")
+        mp = current_date + "_" + self.config.endpoint_id.mission_postfix
+        self.default_path = os.path.join(bp, mp)
+        logging_folder = os.path.join(self.config.log_path, mp, "pyvoyis_logs")
+
+        print("Setting up logging in: ", logging_folder)
+        setup_logging(logging_folder)
+
+        # Copy configuration file to logging folder
+        new_file = os.path.join(logging_folder, "pyvoyis.yaml")
+        with open(new_file, "w") as f:
+            yaml.dump(self.config.dict(), f, default_flow_style=False)
+        print(self.config)
+
+        self.log = logging.getLogger("VoyisAPI")
+        self.log.info("Saving results to %s", self.default_path)
+
     def request_acquisition(self):
         """Request acquisition"""
         self._request_acquisition = True
 
     def request_stop(self):
         """Request stop"""
         self._request_stop = True
@@ -171,15 +191,15 @@
         bool
             True if the command was accepted, False otherwise
         """
         if retries <= 0:
             return False
         len_ack_before = len(self.ack_rsp_list)
         self.loop.run_until_complete(self.client.send_message(cmd.to_str()))
-        if not expect_ack: 
+        if not expect_ack:
             return True
         # Wait for AckRsp to be received
         timeout_start = time.time()
         while time.time() < timeout_start + timeout_s:
             if len(self.ack_rsp_list) == len_ack_before + 1:
                 break
             time.sleep(0.1)
@@ -191,15 +211,15 @@
                         cmd.command, ack_rsp.nack_error_string
                     )
                 )
             elif ack_rsp.accepted:
                 self.log.info("Command {} accepted!".format(cmd.command))
             return ack_rsp.accepted
         else:
-            self.send_message(cmd, timeout_s=timeout_s, retries=retries-1)
+            self.send_message(cmd, timeout_s=timeout_s, retries=retries - 1)
             return False
 
     def get_received_messages(self):
         """Get the received messages from the API500Client
 
         Returns
         -------
@@ -251,14 +271,29 @@
                 return
             success = self.check_connection_status()
             if not success:
                 self.log.error("Could not check connection status")
                 return
             self.state.configure()
         elif self.state.is_configuring:
+            success = self.configure_time_source()
+            if not success:
+                self.log.error(
+                    "Could not configure time source.",
+                    "Check that the IP address provided for time sync is accessible",
+                    "from the Voyis API PC network.",
+                )
+                return
+            success = self.configure_nav()
+            if not success:
+                self.log.error(
+                    "Could not configure nav. Check that the IP address provided for",
+                    "nav updates is accessible from the Voyis PC network.",
+                )
+                return
             success = self.set_data_options()
             if not success:
                 self.log.error("Could not set data options")
                 return
             # Necessary to be able to read armed / temperatures
             success = self.get_scanner_status()
             if not success:
@@ -267,46 +302,26 @@
             success = self.perform_system_checks()
             if not success:
                 self.log.error("Could not perform system checks or some checks failed")
                 return
             success = self.stop_scanning_if_running()
             if not success:
                 self.log.error("Could not stop scanning")
-            success = self.configure_time_source()
-            if not success:
-                self.log.error('Could not configure time source. Check that the IP address provided for time sync is accessible from the Voyis API PC network.')
-                return
-            success = self.configure_nav()
-            if not success:
-                self.log.error('Could not configure nav. Check that the IP address provided for nav updates is accessible from the Voyis PC network.')
-                return
             success = self.set_scan_parameters()
             if not success:
                 self.log.error("Could not set scan parameters")
                 return
             success = self.check_laser_is_armed()
             if not success:
                 self.log.error("Could not check laser is armed")
                 return
             success = self.check_temperatures()
             if not success:
                 self.log.error("Could not check temperatures")
                 return
-            
-            """
-            # Do a network time sync
-            self.cmd.network_time_sync.payload = {
-                "microseconds_since_epoch": int(time.time()*1e6)
-            }
-            success = self.send_message(self.cmd.network_time_sync)
-            if not success:
-                self.log.error("Could not sync network time")
-                return
-            """
-
             self.state.ready()
         if self.state.is_readying and self._request_acquisition:
             self._request_acquisition = False
             self.state.request_acquisition()
         elif self.state.is_requesting_acquisition:
             success = self.start_scanning()
             if not success:
@@ -329,15 +344,15 @@
         elif self.state.is_stopping:
             self.state.disconnect()
         elif self.state.is_disconnecting:
             success = self.disconnect()
             if not success:
                 self.log.error("Could not disconnect")
                 return
-            self.state.idling()
+            self.state.reset()
 
     def run(self):
         """Main function to run the API client"""
         self.asyncio_thread = threading.Thread(target=self.asyncio_thread_fn)
         self.asyncio_thread.start()
 
         # Prepare a background thread to listen to the API and keep it alive
@@ -389,47 +404,32 @@
             True if the connection was successful, False otherwise
         """
         self.log.info("[VoyisAPI]: Connecting to scanner...")
         success = self.send_message(self.cmd.list_scanners)
         if not success:
             self.log.warn("Command list_scanners was not successful")
             return False
-        
+
         self.cmd.check_for_scanner.payload = {"ip_address": self.ip}
         success = self.send_message(self.cmd.check_for_scanner)
 
         if not success:
             self.log.warn("Command check_for_scanner was not successful")
             return False
 
         while not self.is_scanner_connected():
             self.cmd.connect_scanner.payload = {"ip_address": self.ip}
-            success =  self.send_message(self.cmd.connect_scanner)
+            success = self.send_message(self.cmd.connect_scanner)
             if not success:
                 self.log.warn("Command connect_scanner was not successful")
                 return False
             if self.last_connection_state == 5:
                 break
             self.log.info("Waiting 5 seconds before requesting for a connection")
             time.sleep(5)
-
-        """
-        scanner_connected = False
-        retries = 0
-        while not scanner_connected and retries < 5:
-            if SCANNER_STATUS_CONNECTED in self.scanner_status_not_dict:
-                scanner_connected = str2bool(self.scanner_status_not_dict[SCANNER_STATUS_CONNECTED].value.get())
-            retries += 1
-            time.sleep(1)
-        
-        if not scanner_connected:
-            self.log.warn("The state SCANNER_STATUS_CONNECTED was never set.")
-
-        return scanner_connected
-        """
         return True
 
     def check_connection_status(self):
         """Check connection status
 
         Returns
         -------
@@ -454,55 +454,67 @@
 
         self.cmd.set_endpoints.payload = [
             {
                 "endpoint_id": ENDPOINT_ID_LOG,
                 "net_enabled": False,
                 "net_connection": "",
                 "file_enabled": True,
-                "file_name": self.config.endpoint_id.log,
+                "file_name": os.path.join(
+                    self.default_path, self.config.endpoint_id.log
+                ),
                 "file_max_bytes": 1024 * 1024 * 1024,
             },
             {
                 "endpoint_id": ENDPOINT_ID_STREAM,
                 "net_enabled": False,
                 "net_connection": "",
                 "file_enabled": True,
-                "file_name": self.config.endpoint_id.stream,
+                "file_name": os.path.join(
+                    self.default_path, self.config.endpoint_id.stream
+                ),
                 "file_max_bytes": 1024 * 1024 * 1024,
             },
             {
                 "endpoint_id": ENDPOINT_ID_XYZ_LASER,
                 "net_enabled": False,
                 "net_connection": "",
                 "file_enabled": True,
-                "file_name": self.config.endpoint_id.xyz_laser,
+                "file_name": os.path.join(
+                    self.default_path, self.config.endpoint_id.xyz_laser
+                ),
                 "file_max_bytes": 1024 * 1024 * 1024,
             },
             {
                 "endpoint_id": ENDPOINT_ID_SENSOR_LASER,
                 "net_enabled": False,
                 "net_connection": "",
                 "file_enabled": True,
-                "file_name": self.config.endpoint_id.sensor_laser,
+                "file_name": os.path.join(
+                    self.default_path, self.config.endpoint_id.sensor_laser
+                ),
                 "file_max_bytes": 0,
             },
             {
                 "endpoint_id": ENDPOINT_ID_SENSOR_STILLS_RAW,
                 "net_enabled": False,
                 "net_connection": "",
                 "file_enabled": True,
-                "file_name": self.config.endpoint_id.sensor_stills_raw,
+                "file_name": os.path.join(
+                    self.default_path, self.config.endpoint_id.sensor_stills_raw
+                ),
                 "file_max_bytes": 0,
             },
             {
                 "endpoint_id": ENDPOINT_ID_SENSOR_STILLS_PROCESSED,
                 "net_enabled": False,
                 "net_connection": "",
                 "file_enabled": True,
-                "file_name": self.config.endpoint_id.sensor_stills_processed,
+                "file_name": os.path.join(
+                    self.default_path, self.config.endpoint_id.sensor_stills_processed
+                ),
                 "file_max_bytes": 0,
             },
         ]
 
         success = self.send_message(self.cmd.set_endpoints)
         if not success:
             return False
@@ -518,25 +530,25 @@
         respectively.
 
         Returns
         -------
         bool
             True if the scanner is connected to this API, False otherwise
         """
-        #self.send_message(self.cmd.list_scanners)
+        # self.send_message(self.cmd.list_scanners)
 
-        #self.cmd.check_for_scanner.payload = {"ip_address": self.ip}
-        #self.send_message(self.cmd.check_for_scanner)
+        # self.cmd.check_for_scanner.payload = {"ip_address": self.ip}
+        # self.send_message(self.cmd.check_for_scanner)
 
         while len(self.scanner_list_not_dict) == 0:
             time.sleep(1)
             self.log.info("Waiting for ScannerListNot")
             if not self.client.connected:
                 return False
-            
+
         scanner_connection_state = int(safe_get(self.scanner_list_not_dict, self.ip))
         if scanner_connection_state is None:
             self.log.warning("Scanner not found in ScannerListNot")
             return False
 
         self.log.debug("[VoyisAPI]: Scanner found in ScannerListNot")
         self.log.info(
@@ -546,25 +558,33 @@
         )
 
         if scanner_connection_state < SCANNER_NOT_READY:
             self.log.warn("Scanner is not ready, resetting comms...")
             self.state.reset()
 
         return scanner_connection_state == SCANNER_CONNECTED_TO_THIS_API
-    
+
     def wait_for_scanning_status(self, expected_value):
         status_achieved = False
         while not status_achieved:
-            success = self.get_scanner_status()
+            self.get_scanner_status()
             if SCANNER_STATUS_SCAN_IN_PROGRESS not in self.scanner_status_not_dict:
                 continue
-            res = str2bool(self.scanner_status_not_dict[SCANNER_STATUS_SCAN_IN_PROGRESS].value.get())
+            res = str2bool(
+                self.scanner_status_not_dict[
+                    SCANNER_STATUS_SCAN_IN_PROGRESS
+                ].value.get()
+            )
             if res == expected_value:
                 break
-            self.log.info("Waiting for SCANNER_STATUS_SCAN_IN_PROGRESS to become {}".format(expected_value))
+            self.log.info(
+                "Waiting for SCANNER_STATUS_SCAN_IN_PROGRESS to become {}".format(
+                    expected_value
+                )
+            )
             time.sleep(5)
 
     def stop_scanning_if_running(self):
         """Helper function to stop scanning if it is running
 
         Returns
         -------
@@ -658,33 +678,41 @@
             "  * API: {} {}".format(
                 "Connected" if str2bool(api_connected.value.get()) else "NOT Connected",
                 "Ready" if str2bool(api_ready.value.get()) else "NOT Ready",
             )
         )
         self.log.info(
             "  * Stills camera: {} {}".format(
-                "Connected" if str2bool(stills_cam_connected.value.get()) else "NOT Connected",
+                "Connected"
+                if str2bool(stills_cam_connected.value.get())
+                else "NOT Connected",
                 "Ready" if str2bool(stills_cam_ready.value.get()) else "NOT Ready",
             )
         )
         self.log.info(
             "  * Laser camera: {} {}".format(
-                "Connected" if str2bool(laser_cam_connected.value.get()) else "NOT Connected",
+                "Connected"
+                if str2bool(laser_cam_connected.value.get())
+                else "NOT Connected",
                 "Ready" if str2bool(laser_cam_ready.value.get()) else "NOT Ready",
             )
         )
         self.log.info(
             "  * Laser: {} {}".format(
-                "Connected" if str2bool(laser_connected.value.get()) else "NOT Connected",
+                "Connected"
+                if str2bool(laser_connected.value.get())
+                else "NOT Connected",
                 "Ready" if str2bool(laser_ready.value.get()) else "NOT Ready",
             )
         )
         self.log.info(
             "  * LED panel: {} {}".format(
-                "Connected" if str2bool(led_panel_connected.value.get()) else "NOT Connected",
+                "Connected"
+                if str2bool(led_panel_connected.value.get())
+                else "NOT Connected",
                 "Ready" if str2bool(led_panel_ready.value.get()) else "NOT Ready",
             )
         )
 
         return (
             api_ready
             and stills_cam_ready
@@ -721,26 +749,38 @@
         self.log.info("[VoyisAPI]: Configuring nav...")
 
         self.cmd.set_nav_data_source.payload = {
             "network": str_to_network_source(self.config.navigation_input.mode),
             "protocol": str_to_navproto(self.config.navigation_input.driver),
             "connection": self.config.navigation_input.ip_address,
         }
-        return self.send_message(self.cmd.set_nav_data_source)
+        success = self.send_message(self.cmd.set_nav_data_source)
+
+        if not success:
+            self.log.warn("Could not set Navigation data source")
+            return False
+
+        self.cmd.set_range_data_source.payload = {
+            "network": str_to_network_source(self.config.range_input.mode),
+            "protocol": str_to_navproto(self.config.range_input.driver),
+            "connection": self.config.range_input.ip_address,
+        }
+
+        return self.send_message(self.cmd.set_range_data_source)
 
     def set_scan_parameters(self):
         """Sets the scan parameters
 
         Returns
         -------
         bool
             True if the command was successful, False otherwise
         """
         self.log.info("[VoyisAPI]: Setting scan parameters...")
-        cfg = self.config.scanner_param
+        cfg = self.config.parameters
         self.cmd.set_local_scanner_parameters.payload = [
             {
                 "parameter_id": SCANNER_PARAM_PROFILE_STILLS_EXP,
                 "value": str(cfg.stills_exp_us),
                 "type": VALUE_TYPE_UINT,
             },
             {
@@ -784,61 +824,99 @@
                 "type": VALUE_TYPE_UINT,
             },
             {
                 "parameter_id": SCANNER_PARAM_LASER_OUTPUT_GAIN,
                 "value": str(cfg.laser_gain_percentage),
                 "type": VALUE_TYPE_UINT,
             },
-            {
-                "parameter_id": SCANNER_PARAM_STILLS_IMAGE_LEVEL,
-                "value": str(cfg.stills_image_level),
-                "type": VALUE_TYPE_UINT,
-            },
         ]
 
         success = self.send_message(self.cmd.set_local_scanner_parameters)
         if not success:
             return False
 
         success = self.send_message(self.cmd.apply_local_scanner_parameters)
         if not success:
             return False
-        
-        """
+
         success = self.send_message(self.cmd.query_api_configuration)
         if not success:
             return False
 
-        cfg = self.config.api_param_stills
+        self.log.info("[VoyisAPI]: Setting stills parameters...")
         self.cmd.set_api_configuration.payload = [
             {
                 "parameter_id": API_PARAM_STILLS_IMAGE_UNDISTORT,
-                "value": bool2str(cfg.undistort, "1", "0"),
+                "value": bool2str(cfg.stills_undistort, "1", "0"),
                 "type": VALUE_TYPE_UINT,
             },
             {
                 "parameter_id": API_PARAM_STILLS_IMAGE_SAVE_ORIGINAL,
-                "value": bool2str(cfg.save_original, "1", "0"),
+                "value": bool2str(cfg.stills_save_original, "true", "false"),
                 "type": VALUE_TYPE_BOOL,
             },
             {
                 "parameter_id": API_PARAM_STILLS_PROCESSED_IMAGE_FORMAT,
-                "value": cfg.processed_image_format_uint,
+                "value": str(cfg.stills_processed_image_format_uint),
+                "type": VALUE_TYPE_UINT,
+            },
+            {
+                "parameter_id": API_PARAM_STILLS_IMAGE_LEVEL,
+                "value": str(cfg.stills_image_level),
+                "type": VALUE_TYPE_UINT,
+            },
+            {
+                "parameter_id": API_PARAM_STILLS_ADVANCED_COLOUR_MODE,
+                "value": str(cfg.stills_advanced_colour_mode),
+                "type": VALUE_TYPE_UINT,
+            },
+            {
+                "parameter_id": API_PARAM_STILLS_ADVANCED_COLOUR_ENHANCEMENT_LVL,
+                "value": str(cfg.stills_advanced_colour_enhancement_lvl),
+                "type": VALUE_TYPE_UINT,
+            },
+            {
+                "parameter_id": API_PARAM_STILLS_ADVANCED_CONTRAST_MODE,
+                "value": str(cfg.stills_advanced_contrast_mode),
+                "type": VALUE_TYPE_UINT,
+            },
+            {
+                "parameter_id": API_PARAM_STILLS_ADVANCED_CONTRAST_LVL,
+                "value": str(cfg.stills_advanced_contrast_lvl),
+                "type": VALUE_TYPE_UINT,
+            },
+            {
+                "parameter_id": API_PARAM_STILLS_ADVANCED_BRIGHTNESS,
+                "value": "{:.2f}".format(cfg.stills_advanced_brightness),
+                "type": VALUE_TYPE_FLOAT,
+            },
+            {
+                "parameter_id": API_PARAM_STILLS_ADVANCED_CONTRAST,
+                "value": "{:.2f}".format(cfg.stills_advanced_contrast),
+                "type": VALUE_TYPE_FLOAT,
+            },
+            {
+                "parameter_id": API_PARAM_STILLS_ADVANCED_WHITE_BALANCE,
+                "value": str(cfg.stills_advanced_white_balance),
+                "type": VALUE_TYPE_UINT,
+            },
+            {
+                "parameter_id": API_PARAM_STILLS_ADVANCED_ADAPTIVE_LIGHTING,
+                "value": str(cfg.stills_advanced_adaptive_lighting),
                 "type": VALUE_TYPE_UINT,
             },
         ]
-        success =  self.send_message(self.cmd.set_api_configuration, expect_ack=False)
+        success = self.send_message(self.cmd.set_api_configuration)
         if not success:
             return False
-    
+
         success = self.send_message(self.cmd.query_api_configuration)
         if not success:
             return False
-        """
-        
+
         return True
 
     def check_laser_is_armed(self):
         """Helper function to check if the laser is armed
 
         Returns
         -------
@@ -884,77 +962,19 @@
         -------
         bool
             True if all checks were successful, False otherwise
         """
         self.log.info("[VoyisAPI]: Checking temperatures")
         # Check temperatures
         cpu_temp_ch = safe_get(self.scanner_status_not_dict, SCANNER_STATUS_CPU_TEMP_CH)
-        internal_temp_ch = safe_get(
-            self.scanner_status_not_dict, SCANNER_STATUS_INTERNAL_TEMP_CH
-        )
-        sensor_temp_laser_sensor = safe_get(
-            self.scanner_status_not_dict, SCANNER_STATUS_SENSOR_TEMP_LASER_SENSOR
-        )
-        cpu_temp_laser = safe_get(
-            self.scanner_status_not_dict, SCANNER_STATUS_CPU_TEMP_LASER
-        )
-        internal_temp_laser_sensor = safe_get(
-            self.scanner_status_not_dict, SCANNER_STATUS_INTERNAL_TEMP_LASER_SENSOR
-        )
-        sensor_temp_stills_sensor = safe_get(
-            self.scanner_status_not_dict, SCANNER_STATUS_SENSOR_TEMP_STILLS_SENSOR
-        )
-        cpu_temp_stills = safe_get(
-            self.scanner_status_not_dict, SCANNER_STATUS_CPU_TEMP_STILLS
-        )
-        internal_temp_stills_sensor = safe_get(
-            self.scanner_status_not_dict, SCANNER_STATUS_INTERNAL_TEMP_STILLS_SENSOR
-        )
 
         self.log.info("Temperature readings:")
         if cpu_temp_ch is not None:
             self.log.info("  * cpu_temp_ch: {} C".format(cpu_temp_ch.value.get()))
-        if internal_temp_ch is not None:
-            self.log.info(
-                "  * internal_temp_ch: {} C".format(internal_temp_ch.value.get())
-            )
-        if sensor_temp_laser_sensor is not None:
-            self.log.info(
-                "  * sensor_temp_laser_sensor: {} C".format(
-                    sensor_temp_laser_sensor.value.get()
-                )
-            )
-        if cpu_temp_laser is not None:
-            self.log.info("  * cpu_temp_laser: {} C".format(cpu_temp_laser.value.get()))
-        if internal_temp_laser_sensor is not None:
-            self.log.info(
-                "  * internal_temp_laser_sensor: {} C".format(
-                    internal_temp_laser_sensor.value.get()
-                )
-            )
-        if sensor_temp_stills_sensor is not None:
-            self.log.info(
-                "  * sensor_temp_stills_sensor: {} C".format(
-                    sensor_temp_stills_sensor.value.get()
-                )
-            )
-        if cpu_temp_stills is not None:
-            self.log.info(
-                "  * cpu_temp_stills: {} C".format(cpu_temp_stills.value.get())
-            )
-        if internal_temp_stills_sensor is not None:
-            self.log.info(
-                "  * internal_temp_stills_sensor: {} C".format(
-                    internal_temp_stills_sensor.value.get()
-                )
-            )
-        if internal_temp_ch is not None:
-            return int(internal_temp_ch.value.get()) < 60
-        else:
-            return True
+        return True
 
     def start_scanning(self):
         """Sends the command to start scanning
 
         Returns
         -------
         bool
@@ -1057,15 +1077,17 @@
                     f.write(val.to_yaml())
         elif message == "ScannerListNot":
             msg_class = ScannerListNot(data)
             for idx in range(msg_class.size()):
                 self.scanner_list_not_dict[
                     msg_class.ip_addresses[idx]
                 ] = msg_class.connection_states[idx]
-            self.last_connection_state = int(safe_get(self.scanner_list_not_dict, self.ip))
+            self.last_connection_state = int(
+                safe_get(self.scanner_list_not_dict, self.ip)
+            )
         elif message == "ConnectionChangeNot":
             msg_class = ConnectionChangeNot(data)
             self.connection_change_not_list.append(msg_class)
         elif message == "ScannerStatus":
             msg_class = ScannerStatus(data)
             self.scanner_status_list.append(msg_class)
         elif message == "ScannerStatusNot":
@@ -1156,7 +1178,13 @@
             self.correction_model_list_not_list.append(msg_class)
         elif message == "PendingCmdStatusNot":
             msg_class = PendingCmdStatusNot(data)
             self.pending_cmd_status_not_list.append(msg_class)
         elif message == "AckRsp":
             msg_class = AckRsp(data)
             self.ack_rsp_list.append(msg_class)
+
+    def sync_time_manually(self):
+        self.cmd.sync_time_manually.payload = {
+            "microseconds_since_epoch": int(time.time() * 1e6)
+        }
+        return self.send_message(self.cmd.sync_time_manually)
```

### Comparing `pyvoyis-1.0.3/src/pyvoyis/api500/client.py` & `pyvoyis-1.0.4/src/pyvoyis/api500/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 Copyright (c) 2023, Miquel Massot
 All rights reserved.
 Licensed under the GPLv3 License.
 See LICENSE.md file in the project root for full license information.
 """
 
 import asyncio
+import copy
 import json
 import logging
 import sys
-import copy
 
 if sys.version_info[:2] >= (3, 7):
     pass
 else:
     pass
 
 
@@ -34,15 +34,15 @@
     async def _process_queue_loop(self):
         """Send messages to the server as they become available."""
         await self._ready.wait()
         self.log.info("API500 client ready!")
         while True:
             message = await self.queue.get()
             self.transport.write(message.encode("utf-8"))
-            self.log.warn("Message sent: \n{}".format(message))
+            self.log.debug("Message sent: \n{}".format(message))
             await asyncio.sleep(0.1)
 
     def connection_made(self, transport):
         """Upon connection send the message to the
         server
 
         A message has to have the following items:
@@ -92,32 +92,35 @@
             whole_data = copy.deepcopy(self.data)
             self.data = ""
             self.log.debug("Whole chunk ready")
         else:
             self.log.debug("Adding chunk to message")
             self.data += chunk
             return
-        
+
         # Split data into JSON strings if "}{" is found
         objects = whole_data.split("}{")
 
         # Add back the missing brackets
         if len(objects) > 1:
             objects[0] = objects[0] + "}"
             objects[-1] = "{" + objects[-1]
             for idx in range(1, len(objects) - 1):
                 objects[idx] = "{" + objects[idx] + "}"
 
         # Process each object
         for idx, obj in enumerate(objects):
             try:
-                self.log.warn(
-                    "Received split object {}: {}".format(idx, json.dumps(json.loads(obj))))
+                self.log.debug(
+                    "Received split object {}: {}".format(
+                        idx, json.dumps(json.loads(obj))
+                    )
+                )
                 asyncio.ensure_future(self.process_data(obj))
-            except json.decoder.JSONDecodeError as e:
+            except json.decoder.JSONDecodeError:
                 self.log.warn("Could not decode: {}".format(obj))
 
     def connection_lost(self, error):
         if error:
             self.log.error("ERROR: {}".format(error))
         else:
             self.log.warning("The server closed the connection")
```

### Comparing `pyvoyis-1.0.3/src/pyvoyis/api500/command.py` & `pyvoyis-1.0.4/src/pyvoyis/api500/command.py`

 * *Files identical despite different names*

### Comparing `pyvoyis-1.0.3/src/pyvoyis/api500/defs.py` & `pyvoyis-1.0.4/src/pyvoyis/api500/defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -342,15 +342,15 @@
     elif value == API_PARAM_STILLS_ADVANCED_BRIGHTNESS:
         return "API_PARAM_STILLS_ADVANCED_BRIGHTNESS"
     elif value == API_PARAM_STILLS_ADVANCED_CONTRAST:
         return "API_PARAM_STILLS_ADVANCED_CONTRAST"
     elif value == API_PARAM_STILLS_ADVANCED_WHITE_BALANCE:
         return "API_PARAM_STILLS_ADVANCED_WHITE_BALANCE"
     elif value == API_PARAM_STILLS_ADVANCED_ADAPTIVE_LIGHTING:
-        return "API_PARAM_STILLS_ADVANCED_ADAPTIVE_LIGHTING" 
+        return "API_PARAM_STILLS_ADVANCED_ADAPTIVE_LIGHTING"
     elif value == API_PARAM_DUMMY_0:
         return "API_PARAM_DUMMY_0"
     elif value == API_PARAM_DUMMY_1:
         return "API_PARAM_DUMMY_1"
     elif value == API_PARAM_ENABLE_RAM_BUFF_MONITOR:
         return "API_PARAM_ENABLE_RAM_BUFF_MONITOR"
     else:
@@ -1206,15 +1206,16 @@
 
 SOURCE_COM = 0
 SOURCE_UDP = 1
 SOURCE_TCP_CLIENT = 2
 SOURCE_TCP_SERVER = 3
 SOURCE_MULTICAST = 4
 
-def str_to_network_source(value:str):
+
+def str_to_network_source(value: str):
     if value.lower() == "com":
         return SOURCE_COM
     elif value.lower() == "udp":
         return SOURCE_UDP
     elif value.lower() == "tcp_client":
         return SOURCE_TCP_CLIENT
     elif value.lower() == "tcp_server":
@@ -1243,26 +1244,26 @@
 def timeproto_to_str(value):
     if value == TIMEPROTO_ZDA:
         return "TIMEPROTO_ZDA"
 
 
 # Supported Nav data protocols
 NAVPROTO_RAW = 0  # (not currently implemented)
-NAVPROTO_LNAV = 10  # Sonardyne LNAV format supports range
+NAVPROTO_LNAV = 1  # Sonardyne LNAV format supports range
 NAVPROTO_DELPHINS = 20  # DelphINS format
 NAVPROTO_ISE = 30  # ISE navigation format
 NAVPROTO_KONGSBERG = 40  # Kongsberg navigation format
 NAVPROTO_ROVINS = 50  # ROVINS INS format
 NAVPROTO_NAVLAB = 60  # NAVLAB format
 NAVPROTO_IXBLUESTD = 70  # IXBlue Std format
 NAVPROTO_PHINSSTD = 80  # PHINS Std format supports range
 NAVPROTO_PSONNAV = 1  # Sonardyne PSONNAV format
 
 
-def str_to_navproto(value:str):
+def str_to_navproto(value: str):
     if value.lower() == "raw":
         return NAVPROTO_RAW
     if value.lower() == "lnav":
         return NAVPROTO_LNAV
     if value.lower() == "delphins":
         return NAVPROTO_DELPHINS
     if value.lower() == "ise":
```

### Comparing `pyvoyis-1.0.3/src/pyvoyis/cli.py` & `pyvoyis-1.0.4/src/pyvoyis/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 """
 
 import argparse
 
 from pyvoyis import Configuration, VoyisAPI
 
 
-
 def main():
     parser = argparse.ArgumentParser(
         description="Run a TCP client to send messages to Voyis API"
     )
     parser.add_argument("--ip", type=str, help="IP address of the Voyis API")
     parser.add_argument("--port", type=int, help="Port of the Voyis API")
     parser.add_argument("--log_path", type=str, help="Path to save the log file")
@@ -26,15 +25,14 @@
     args = parser.parse_args()
 
     config = Configuration(args.config)
 
     if args.log_path:
         config.log_path = args.log_path
 
-    
     print("Starting Voyis API client")
 
     if args.ip:
         print("Using provided IP address: %s", args.ip)
         config.ip_address = args.ip
     if args.port:
         print("Using provided port: %s", args.port)
```

### Comparing `pyvoyis-1.0.3/src/pyvoyis/commander.py` & `pyvoyis-1.0.4/src/pyvoyis/commander.py`

 * *Files identical despite different names*

### Comparing `pyvoyis-1.0.3/src/pyvoyis/messages.py` & `pyvoyis-1.0.4/src/pyvoyis/messages.py`

 * *Files identical despite different names*

### Comparing `pyvoyis-1.0.3/src/pyvoyis/state_machine.py` & `pyvoyis-1.0.4/src/pyvoyis/state_machine.py`

 * *Files identical despite different names*

### Comparing `pyvoyis-1.0.3/src/pyvoyis.egg-info/PKG-INFO` & `pyvoyis-1.0.4/src/pyvoyis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvoyis
-Version: 1.0.3
+Version: 1.0.4
 Summary: Voyis Recon LS python driver
 Home-page: https://github.com/miquelmassot/pyvoyis
 Author: Miquel Massot
 Author-email: miquel.massot@gmail.com
 Maintainer: Miquel Massot
 Maintainer-email: miquel.massot@gmail.com
 License: GPLv3
```

### Comparing `pyvoyis-1.0.3/src/pyvoyis.egg-info/SOURCES.txt` & `pyvoyis-1.0.4/src/pyvoyis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

