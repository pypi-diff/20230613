# Comparing `tmp/meili_ros_lib-0.1.7.tar.gz` & `tmp/meili_ros_lib-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meili_ros_lib-0.1.7.tar", last modified: Tue Jun 13 10:24:57 2023, max compression
+gzip compressed data, was "meili_ros_lib-0.1.8.tar", last modified: Tue Jun 13 12:36:55 2023, max compression
```

## Comparing `meili_ros_lib-0.1.7.tar` & `meili_ros_lib-0.1.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 10:24:57.269917 meili_ros_lib-0.1.7/
--rw-rw-rw-   0 root         (0) root         (0)     1085 2023-06-13 10:24:47.000000 meili_ros_lib-0.1.7/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      297 2023-06-13 10:24:57.269917 meili_ros_lib-0.1.7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       14 2023-06-13 10:24:47.000000 meili_ros_lib-0.1.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 10:24:57.269002 meili_ros_lib-0.1.7/meili_ros_lib/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-13 10:24:47.000000 meili_ros_lib-0.1.7/meili_ros_lib/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    20850 2023-06-13 10:24:47.000000 meili_ros_lib-0.1.7/meili_ros_lib/agent.py
--rw-rw-rw-   0 root         (0) root         (0)     2208 2023-06-13 10:24:47.000000 meili_ros_lib-0.1.7/meili_ros_lib/agent_setup.py
--rw-rw-rw-   0 root         (0) root         (0)     4521 2023-06-13 10:24:47.000000 meili_ros_lib-0.1.7/meili_ros_lib/config_agent.py
--rw-rw-rw-   0 root         (0) root         (0)     3274 2023-06-13 10:24:47.000000 meili_ros_lib-0.1.7/meili_ros_lib/connection.py
--rw-rw-rw-   0 root         (0) root         (0)     1450 2023-06-13 10:24:47.000000 meili_ros_lib-0.1.7/meili_ros_lib/docking.py
--rw-rw-rw-   0 root         (0) root         (0)     1649 2023-06-13 10:24:47.000000 meili_ros_lib-0.1.7/meili_ros_lib/maths.py
--rw-rw-rw-   0 root         (0) root         (0)    11990 2023-06-13 10:24:47.000000 meili_ros_lib-0.1.7/meili_ros_lib/offline.py
--rw-rw-rw-   0 root         (0) root         (0)     2620 2023-06-13 10:24:47.000000 meili_ros_lib-0.1.7/meili_ros_lib/parse_data.py
--rw-rw-rw-   0 root         (0) root         (0)     9864 2023-06-13 10:24:47.000000 meili_ros_lib-0.1.7/meili_ros_lib/sdk_handlers.py
--rw-rw-rw-   0 root         (0) root         (0)      881 2023-06-13 10:24:47.000000 meili_ros_lib-0.1.7/meili_ros_lib/sentry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 10:24:57.269917 meili_ros_lib-0.1.7/meili_ros_lib.egg-info/
--rw-r--r--   0 root         (0) root         (0)      297 2023-06-13 10:24:57.000000 meili_ros_lib-0.1.7/meili_ros_lib.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      479 2023-06-13 10:24:57.000000 meili_ros_lib-0.1.7/meili_ros_lib.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 10:24:57.000000 meili_ros_lib-0.1.7/meili_ros_lib.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-06-13 10:24:57.000000 meili_ros_lib-0.1.7/meili_ros_lib.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      353 2023-06-13 10:24:57.269917 meili_ros_lib-0.1.7/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      131 2023-06-13 10:24:47.000000 meili_ros_lib-0.1.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 12:36:55.096264 meili_ros_lib-0.1.8/
+-rw-rw-rw-   0 root         (0) root         (0)     1085 2023-06-13 12:36:45.000000 meili_ros_lib-0.1.8/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      297 2023-06-13 12:36:55.097264 meili_ros_lib-0.1.8/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       14 2023-06-13 12:36:45.000000 meili_ros_lib-0.1.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 12:36:55.096264 meili_ros_lib-0.1.8/meili_ros_lib/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-13 12:36:45.000000 meili_ros_lib-0.1.8/meili_ros_lib/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    21298 2023-06-13 12:36:45.000000 meili_ros_lib-0.1.8/meili_ros_lib/agent.py
+-rw-rw-rw-   0 root         (0) root         (0)     2208 2023-06-13 12:36:45.000000 meili_ros_lib-0.1.8/meili_ros_lib/agent_setup.py
+-rw-rw-rw-   0 root         (0) root         (0)     4521 2023-06-13 12:36:45.000000 meili_ros_lib-0.1.8/meili_ros_lib/config_agent.py
+-rw-rw-rw-   0 root         (0) root         (0)     3284 2023-06-13 12:36:45.000000 meili_ros_lib-0.1.8/meili_ros_lib/connection.py
+-rw-rw-rw-   0 root         (0) root         (0)     1450 2023-06-13 12:36:45.000000 meili_ros_lib-0.1.8/meili_ros_lib/docking.py
+-rw-rw-rw-   0 root         (0) root         (0)     1649 2023-06-13 12:36:45.000000 meili_ros_lib-0.1.8/meili_ros_lib/maths.py
+-rw-rw-rw-   0 root         (0) root         (0)    11990 2023-06-13 12:36:45.000000 meili_ros_lib-0.1.8/meili_ros_lib/offline.py
+-rw-rw-rw-   0 root         (0) root         (0)     2620 2023-06-13 12:36:45.000000 meili_ros_lib-0.1.8/meili_ros_lib/parse_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     9864 2023-06-13 12:36:45.000000 meili_ros_lib-0.1.8/meili_ros_lib/sdk_handlers.py
+-rw-rw-rw-   0 root         (0) root         (0)      881 2023-06-13 12:36:45.000000 meili_ros_lib-0.1.8/meili_ros_lib/sentry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 12:36:55.096264 meili_ros_lib-0.1.8/meili_ros_lib.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      297 2023-06-13 12:36:55.000000 meili_ros_lib-0.1.8/meili_ros_lib.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      479 2023-06-13 12:36:55.000000 meili_ros_lib-0.1.8/meili_ros_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 12:36:55.000000 meili_ros_lib-0.1.8/meili_ros_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-06-13 12:36:55.000000 meili_ros_lib-0.1.8/meili_ros_lib.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      353 2023-06-13 12:36:55.097264 meili_ros_lib-0.1.8/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      131 2023-06-13 12:36:45.000000 meili_ros_lib-0.1.8/setup.py
```

### Comparing `meili_ros_lib-0.1.7/LICENSE.txt` & `meili_ros_lib-0.1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `meili_ros_lib-0.1.7/meili_ros_lib/agent.py` & `meili_ros_lib-0.1.8/meili_ros_lib/agent.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import math
 import sys
 import datetime
+import threading
 from math import sqrt
 
 from meili_sdk.websockets.models.message import Message
 from meili_sdk.websockets import constants
 
 from geometry_msgs.msg import PoseWithCovarianceStamped, Pose, Twist
 from sensor_msgs.msg import NavSatFix
@@ -25,14 +26,19 @@
     capacity = 47.6 * voltage - 500
     return capacity
 
 
 class Agent:
     def __init__(self, node, file_name_vehicles, file_name_topics):
         # Logging functions
+
+        # Threads
+        self.thread1 = None
+        self.thread2 = None
+
         self.log_info = node.log_info
         self.log_error = node.log_error
         self.file_name_vehicles = file_name_vehicles
         self.file_name_topics = file_name_topics
 
         # Initial instances
         self.node = node
@@ -167,16 +173,16 @@
         try:
             message = Message(event=event, value=value, vehicle=vehicle)
             message.validate()
             self.client.send(message)
         except Exception as e:
             self.log_info(f"SEND MESSAGE ERROR{e} {event} {vehicle}")
 
-    def ping_filtering_mode(self, pub_rate):
-        pub_rate.sleep()
+    def ping_filtering_mode(self):
+
         self.ping_speed()
 
         if self.node.outdoor:
             self.ping_gps()
         else:
             self.ping_location()
 
@@ -351,26 +357,24 @@
             for vehicle in self.vehicles:
                 if (vehicle['prefix']) == name:
                     vehicle = self.vehicle_list[count]
                 count += 1
         else:
             vehicle = self.vehicle_list[0]
 
-        if self.ws_open & (type_msg == "error" or type_msg == "warning"):
+        if self.ws_open and self.node.logging==type_msg:
+            type_msg="warning"
             try:
-                if type_msg == "error":
-                    type_msg = "warning"
-                # This is a fix until BE is fixed!
                 self.send_message_client(
                     constants.EVENT_NOTIFICATION,
-                    {"vehicle": vehicle,
-                     "message": rosout_message, "level": type_msg,
-                     "meta": {"file": msg.file, "function": msg.function, "line": msg.line}},
-                    vehicle,
-                )
+                            {"vehicle": vehicle,
+                             "message": rosout_message, "level": type_msg,
+                             "meta": {"file": msg.file, "function": msg.function, "line": msg.line}},
+                            vehicle,
+                        )
             except Exception as e:
                 self.log_error(f"[ROSAgent] Sending notification error {e}")
 
     def task_in_progress(self, goal_id, status_id, vehicle_uuid):
         if self.ws_open:
             vehicle_position = self.return_vehicle_position(vehicle_uuid)
             if self.waypoints_goal_id[vehicle_position] is not None:
@@ -529,26 +533,39 @@
         vehicle_position = self.return_vehicle_position(vehicle_uuid)
         self.msg_speed[vehicle_position] = msg
         # Parse current robot pose and sent to FMS task_msg_server
         if self.node.topic_streaming_mode == "REALTIME" and self.ws_open:
             self.ping_speed()
 
     ################################################
-    def run(self, rate, pub_rate):
+    def run(self, conn_rate, pub_rate):
         """Running the agent"""
         # When Mode is filtering, all data is sent to the FMS task_msg_server at specific frequency
         self.check_topic_streaming_mode()
 
         while True:
             try:
                 # Check internet connection
-                if not self.connection.offline_agent.task_offline_started:
-                    self.check_internet()
-                    rate.sleep()
-                if self.node.topic_streaming_mode == "FILTERING" and self.ws_open:
-                    self.ping_filtering_mode(pub_rate)
+                if not (self.thread1 and self.thread1.is_alive()):
+                    self.thread1 = threading.Thread(target=self.connecting, args=(conn_rate,))
+                    self.thread1.start()
+
+                if not (self.thread2 and self.thread2.is_alive()):
+                    self.thread2 = threading.Thread(target=self.pinging, args=(pub_rate,))
+                    self.thread2.start()
+
 
             except Exception as error:
                 capture_exception(error)
                 self.log_error(
                     f"[ROSAgent] Run Error: {type(error).__name__}, {error}"
                 )
+
+    def connecting(self, conn_rate):
+        if not self.connection.offline_agent.task_offline_started:
+            self.check_internet()
+            conn_rate.sleep()
+
+    def pinging(self, pub_rate):
+        if self.node.topic_streaming_mode == "FILTERING" and self.ws_open:
+            self.ping_filtering_mode()
+            pub_rate.sleep()
```

### Comparing `meili_ros_lib-0.1.7/meili_ros_lib/agent_setup.py` & `meili_ros_lib-0.1.8/meili_ros_lib/agent_setup.py`

 * *Files identical despite different names*

### Comparing `meili_ros_lib-0.1.7/meili_ros_lib/config_agent.py` & `meili_ros_lib-0.1.8/meili_ros_lib/config_agent.py`

 * *Files identical despite different names*

### Comparing `meili_ros_lib-0.1.7/meili_ros_lib/connection.py` & `meili_ros_lib-0.1.8/meili_ros_lib/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
                         self.offline_agent.offline_tasks = self.offline_agent.config_offlinetasks()
                     else:
                         self.offline_agent.activate_offline_agent()
         except Exception as e:
             self.log_info(f"ERROR >> {e}")
         return ws_open
 
-    def check_internet_connection(self, ws_open, host="https://google.com"):
+    def check_internet_connection(self, ws_open, host='https://demo.meilirobots.com'):
 
         try:
             # CHECK FOR INTERNET CONNECTION
             urllib.request.urlopen(host, timeout=5)  # nosec
             self.offline_agent.offline = False
             self.internet_down = 0
```

### Comparing `meili_ros_lib-0.1.7/meili_ros_lib/docking.py` & `meili_ros_lib-0.1.8/meili_ros_lib/docking.py`

 * *Files identical despite different names*

### Comparing `meili_ros_lib-0.1.7/meili_ros_lib/maths.py` & `meili_ros_lib-0.1.8/meili_ros_lib/maths.py`

 * *Files identical despite different names*

### Comparing `meili_ros_lib-0.1.7/meili_ros_lib/offline.py` & `meili_ros_lib-0.1.8/meili_ros_lib/offline.py`

 * *Files identical despite different names*

### Comparing `meili_ros_lib-0.1.7/meili_ros_lib/parse_data.py` & `meili_ros_lib-0.1.8/meili_ros_lib/parse_data.py`

 * *Files identical despite different names*

### Comparing `meili_ros_lib-0.1.7/meili_ros_lib/sdk_handlers.py` & `meili_ros_lib-0.1.8/meili_ros_lib/sdk_handlers.py`

 * *Files identical despite different names*

### Comparing `meili_ros_lib-0.1.7/meili_ros_lib/sentry.py` & `meili_ros_lib-0.1.8/meili_ros_lib/sentry.py`

 * *Files identical despite different names*

