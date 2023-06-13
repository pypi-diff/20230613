# Comparing `tmp/py-miraie-ac-0.0.9.tar.gz` & `tmp/py-miraie-ac-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-miraie-ac-0.0.9.tar", last modified: Sat Jun 10 06:47:45 2023, max compression
+gzip compressed data, was "py-miraie-ac-0.1.0.tar", last modified: Tue Jun 13 02:53:38 2023, max compression
```

## Comparing `py-miraie-ac-0.0.9.tar` & `py-miraie-ac-0.1.0.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-06-10 06:47:45.873209 py-miraie-ac-0.0.9/
--rw-rw-rw-   0        0        0    35821 2023-06-09 07:50:41.000000 py-miraie-ac-0.0.9/LICENSE
--rw-rw-rw-   0        0        0     1232 2023-06-10 06:47:45.874328 py-miraie-ac-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0      625 2023-06-09 08:48:49.000000 py-miraie-ac-0.0.9/README.md
--rw-rw-rw-   0        0        0      104 2023-06-09 16:09:32.000000 py-miraie-ac-0.0.9/pyproject.toml
--rw-rw-rw-   0        0        0      801 2023-06-10 06:47:45.875331 py-miraie-ac-0.0.9/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-10 06:47:45.798210 py-miraie-ac-0.0.9/src/
-drwxrwxrwx   0        0        0        0 2023-06-10 06:47:45.866206 py-miraie-ac-0.0.9/src/py_miraie_ac/
--rw-rw-rw-   0        0        0      403 2023-06-09 13:16:33.000000 py-miraie-ac-0.0.9/src/py_miraie_ac/__init__.py
--rw-rw-rw-   0        0        0     6359 2023-06-10 06:47:06.000000 py-miraie-ac-0.0.9/src/py_miraie_ac/api.py
--rw-rw-rw-   0        0        0     6252 2023-06-09 17:07:32.000000 py-miraie-ac-0.0.9/src/py_miraie_ac/broker.py
--rw-rw-rw-   0        0        0      421 2023-06-05 03:33:43.000000 py-miraie-ac-0.0.9/src/py_miraie_ac/constants.py
--rw-rw-rw-   0        0        0     4604 2023-06-10 06:43:16.000000 py-miraie-ac-0.0.9/src/py_miraie_ac/device.py
--rw-rw-rw-   0        0        0      857 2023-06-09 13:29:04.000000 py-miraie-ac-0.0.9/src/py_miraie_ac/deviceStatus.py
--rw-rw-rw-   0        0        0      917 2023-06-05 03:55:22.000000 py-miraie-ac-0.0.9/src/py_miraie_ac/enums.py
--rw-rw-rw-   0        0        0      121 2023-06-05 03:55:32.000000 py-miraie-ac-0.0.9/src/py_miraie_ac/exceptions.py
--rw-rw-rw-   0        0        0      483 2023-06-09 13:29:18.000000 py-miraie-ac-0.0.9/src/py_miraie_ac/home.py
--rw-rw-rw-   0        0        0      460 2023-06-05 03:57:35.000000 py-miraie-ac-0.0.9/src/py_miraie_ac/user.py
--rw-rw-rw-   0        0        0      236 2023-06-09 13:29:27.000000 py-miraie-ac-0.0.9/src/py_miraie_ac/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-10 06:47:45.872205 py-miraie-ac-0.0.9/src/py_miraie_ac.egg-info/
--rw-rw-rw-   0        0        0     1232 2023-06-10 06:47:45.000000 py-miraie-ac-0.0.9/src/py_miraie_ac.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      544 2023-06-10 06:47:45.000000 py-miraie-ac-0.0.9/src/py_miraie_ac.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 06:47:45.000000 py-miraie-ac-0.0.9/src/py_miraie_ac.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-06-10 06:47:45.000000 py-miraie-ac-0.0.9/src/py_miraie_ac.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-10 06:47:45.000000 py-miraie-ac-0.0.9/src/py_miraie_ac.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-13 02:53:38.575922 py-miraie-ac-0.1.0/
+-rw-rw-rw-   0        0        0    35821 2023-06-09 07:50:41.000000 py-miraie-ac-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0     1273 2023-06-13 02:53:38.575922 py-miraie-ac-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      666 2023-06-13 02:52:22.000000 py-miraie-ac-0.1.0/README.md
+-rw-rw-rw-   0        0        0      104 2023-06-09 16:09:32.000000 py-miraie-ac-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0      801 2023-06-13 02:53:38.576921 py-miraie-ac-0.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-13 02:53:38.458475 py-miraie-ac-0.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-13 02:53:38.566714 py-miraie-ac-0.1.0/src/py_miraie_ac/
+-rw-rw-rw-   0        0        0      403 2023-06-09 13:16:33.000000 py-miraie-ac-0.1.0/src/py_miraie_ac/__init__.py
+-rw-rw-rw-   0        0        0     6645 2023-06-12 15:09:04.000000 py-miraie-ac-0.1.0/src/py_miraie_ac/api.py
+-rw-rw-rw-   0        0        0     6900 2023-06-12 15:07:29.000000 py-miraie-ac-0.1.0/src/py_miraie_ac/broker.py
+-rw-rw-rw-   0        0        0      421 2023-06-05 03:33:43.000000 py-miraie-ac-0.1.0/src/py_miraie_ac/constants.py
+-rw-rw-rw-   0        0        0     4928 2023-06-11 14:23:54.000000 py-miraie-ac-0.1.0/src/py_miraie_ac/device.py
+-rw-rw-rw-   0        0        0      995 2023-06-10 12:09:13.000000 py-miraie-ac-0.1.0/src/py_miraie_ac/deviceStatus.py
+-rw-rw-rw-   0        0        0      917 2023-06-05 03:55:22.000000 py-miraie-ac-0.1.0/src/py_miraie_ac/enums.py
+-rw-rw-rw-   0        0        0      121 2023-06-05 03:55:32.000000 py-miraie-ac-0.1.0/src/py_miraie_ac/exceptions.py
+-rw-rw-rw-   0        0        0      483 2023-06-09 13:29:18.000000 py-miraie-ac-0.1.0/src/py_miraie_ac/home.py
+-rw-rw-rw-   0        0        0     1556 2023-06-12 15:09:49.000000 py-miraie-ac-0.1.0/src/py_miraie_ac/test.py
+-rw-rw-rw-   0        0        0      460 2023-06-05 03:57:35.000000 py-miraie-ac-0.1.0/src/py_miraie_ac/user.py
+-rw-rw-rw-   0        0        0      236 2023-06-09 13:29:27.000000 py-miraie-ac-0.1.0/src/py_miraie_ac/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-13 02:53:38.574932 py-miraie-ac-0.1.0/src/py_miraie_ac.egg-info/
+-rw-rw-rw-   0        0        0     1273 2023-06-13 02:53:38.000000 py-miraie-ac-0.1.0/src/py_miraie_ac.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      569 2023-06-13 02:53:38.000000 py-miraie-ac-0.1.0/src/py_miraie_ac.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 02:53:38.000000 py-miraie-ac-0.1.0/src/py_miraie_ac.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-06-13 02:53:38.000000 py-miraie-ac-0.1.0/src/py_miraie_ac.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-13 02:53:38.000000 py-miraie-ac-0.1.0/src/py_miraie_ac.egg-info/top_level.txt
```

### Comparing `py-miraie-ac-0.0.9/LICENSE` & `py-miraie-ac-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py-miraie-ac-0.0.9/PKG-INFO` & `py-miraie-ac-0.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-miraie-ac
-Version: 0.0.9
+Version: 0.1.0
 Summary: A package to control and read MirAIe Aircons by Panasonic
 Home-page: https://github.com/milothomas/py-miraie-ac
 Author: Milo Thomas
 Author-email: 20719501+milothomas@users.noreply.github.com
 Project-URL: Bug Tracker, https://github.com/milothomas/py-miraie-ac/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -22,16 +22,22 @@
 pip install py-miraie-ac
 ```
 
 **Usage**
 ```
 import asyncio
 from api import MirAIeAPI
-from enums import AuthType, SwingMode
+from enums import AuthType
 from device import Device
 
-async with MirAIeAPI(auth_type=AuthType.MOBILE, login_id=mobile_number, password=password) as api:
-        home:Home = await api.initialize()
-        for deviceId, device in home.devices.items():
-            print("Found device: ", device.friendly_name)
-            officeAc.set_temperature(24)
-            officeAc.turnOn()
+async with MirAIeAPI(
+        auth_type=AuthType.MOBILE, 
+        login_id="YOUR_MOBILE_NUMBER", 
+        password="YOUR_PASSWORD"
+    ) as api:
+    await api.initialize()
+    for device in api.devices:
+        print("Found device: ", device.friendly_name)
+        device.set_temperature(24)
+        device.turn_on()
+
+asyncio.get_event_loop().run_until_complete(start())
```

### Comparing `py-miraie-ac-0.0.9/setup.cfg` & `py-miraie-ac-0.1.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 792d 6d69 7261 6965 2d61 630d   = py-miraie-ac.
-00000020: 0a76 6572 7369 6f6e 203d 2030 2e30 2e39  .version = 0.0.9
+00000020: 0a76 6572 7369 6f6e 203d 2030 2e31 2e30  .version = 0.1.0
 00000030: 0d0a 6175 7468 6f72 203d 204d 696c 6f20  ..author = Milo 
 00000040: 5468 6f6d 6173 0d0a 6175 7468 6f72 5f65  Thomas..author_e
 00000050: 6d61 696c 203d 2032 3037 3139 3530 312b  mail = 20719501+
 00000060: 6d69 6c6f 7468 6f6d 6173 4075 7365 7273  milothomas@users
 00000070: 2e6e 6f72 6570 6c79 2e67 6974 6875 622e  .noreply.github.
 00000080: 636f 6d0d 0a64 6573 6372 6970 7469 6f6e  com..description
 00000090: 203d 2041 2070 6163 6b61 6765 2074 6f20   = A package to
```

### Comparing `py-miraie-ac-0.0.9/src/py_miraie_ac/api.py` & `py-miraie-ac-0.1.0/src/py_miraie_ac/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """The MirAIe API module"""
 
 import math
 import random
+import asyncio
 import aiohttp
-from py_miraie_ac.constants import DEVICE_DETAILS_URL, HOMES_URL,HTTP_CLIENT_ID,LOGIN_URL,STATUS_URL
 from py_miraie_ac.broker import MirAIeBroker
 from py_miraie_ac.device import Device
+from py_miraie_ac.constants import DEVICE_DETAILS_URL, HOMES_URL,HTTP_CLIENT_ID,LOGIN_URL,STATUS_URL
 from py_miraie_ac.deviceStatus import DeviceStatus
 from py_miraie_ac.enums import (
     AuthType,
     DisplayState,
     FanMode,
     HVACMode,
     PowerMode,
@@ -32,15 +33,15 @@
     __topics: list[str] = []
     __broker: MirAIeBroker
 
     @property
     def devices(self) -> list[Device]:
         """Returns a list of available devices."""
         return list(self.__home.devices.values())
-    
+
     def __init__(self, auth_type: AuthType, login_id: str, password: str):
         self.__auth_type = str(auth_type.value)
         self.__login_id = login_id
         self.__password = password
         self.__http_session = aiohttp.ClientSession()
 
     async def __aenter__(self):
@@ -54,21 +55,24 @@
         """Initializes the MirAIe API"""
 
         self.__user = await self.__login()
         self.__broker = MirAIeBroker()
 
         self.__home = await self.__get_home_details()
         self.__broker.set_topics(self.__topics)
-        self.__broker.init_broker(self.__home.home_id, self.__user.access_token)
+        self.__broker.init_broker(self.__home.home_id, self.__user.access_token, self.reconnect_broker)
         self.__broker.connect()
 
-    async def reconnect_broker(self):
+    def reconnect_broker(self, reconnect_callback: callable):
         """Authenticates with MirAIe and reconnects to MQTT server with the new credentials"""
-        self.__user = await self.__login()
-        self.__broker.reconnect(self.__user.access_token)
+        loop = self.__http_session.loop
+        fut = asyncio.run_coroutine_threadsafe(self.__login(), loop)
+
+        self.__user = fut.result()
+        reconnect_callback(self.__home.home_id, self.__user.access_token)
 
     async def __login(self):
         data = {
             "clientId": HTTP_CLIENT_ID,
             "password": self.__password,
             "scope": self.__get_scope(),
         }
@@ -94,14 +98,15 @@
         resp = await response.json()
         return await self.__parse_home_details(resp[0])
 
     async def __parse_home_details(self, json_response):
         devices: list[Device] = []
 
         for space in json_response["spaces"]:
+            space_name = space["spaceName"]
             for device in space["devices"]:
                 device_id = device["deviceId"]
                 topic = str(device["topic"][0])
                 device_details = await self.__get_device_details(device_id)
                 device_status = await self.__get_device_status(device_id)
 
                 device = Device(
@@ -115,17 +120,17 @@
                     mac_address=device_details["macAddress"],
                     category=device_details["category"],
                     brand=device_details["brand"],
                     firmware_version=device_details["firmwareVersion"],
                     serial_number=device_details["serialNumber"],
                     model_number=device_details["modelNumber"],
                     product_serial_number=device_details["productSerialNumber"],
-                    area_name=space["spaceName"],
                     status=device_status,
                     broker=self.__broker,
+                    area_name=space_name,
                 )
 
                 self.__topics.append(device.status_topic)
                 self.__topics.append(device.connection_status_topic)
                 devices.append(device)
 
         return Home(home_id=json_response["homeId"], devices=devices)
@@ -152,22 +157,23 @@
         json = await response.json()
         status = DeviceStatus(
             is_online=json["onlineStatus"] == "true",
             temperature=to_float(json["actmp"]),
             room_temp=to_float(json["rmtmp"]),
             power_mode=PowerMode(json["ps"]),
             fan_mode=FanMode(json["acfs"]),
-            swing_mode=SwingMode(json["acvs"]),
             display_state=DisplayState(json["acdc"]),
             hvac_mode=HVACMode(json["acmd"]),
             preset_mode=PresetMode.BOOST
             if json["acpm"] == "on"
             else PresetMode.ECO
             if json["acem"] == "on"
             else PresetMode.NONE,
+            vertical_swing_mode=SwingMode(json["acvs"]),
+            horizontal_swing_mode=SwingMode(json["achs"]),
         )
 
         return status
 
     def __build_http_headers(self):
         return {
             "Authorization": f"Bearer {self.__user.access_token}"
```

### Comparing `py-miraie-ac-0.0.9/src/py_miraie_ac/broker.py` & `py-miraie-ac-0.1.0/src/py_miraie_ac/broker.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 """The MQTT broker implemetation"""
 
 import json
 import math
 import random
 import ssl
+from typing import Callable
 from paho.mqtt import client as paho
-
 from py_miraie_ac.enums import FanMode, HVACMode, PowerMode, PresetMode, SwingMode
 
 class MirAIeBroker:
     """The MirAIe Broker class"""
 
     __host: str = "mqtt.miraie.in"
     __port: int = 8883
+    __useSsl: bool = True
     __username: str
     __password: str
     __topics: list[str] = []
-    __callbacks: dict[str, list[callable]] = {}
+    __callbacks: dict[str, list[Callable]] = {}
     __client: paho.Client
-    
-    def init_broker(self, username: str, password: str):
+    __get_access_token_callback: Callable
+
+    def init_broker(self, username: str, password: str, get_access_token_callback: Callable):
         """Initializes the MQTT client"""
         self.__username = username
         self.__password = password
+        self.__get_access_token_callback = get_access_token_callback
         self.__init_mqtt_client()
 
     def set_topics(self, topics: list[str]):
         """Sets the topics to subscribe to"""
         self.__topics = topics
 
-    def register_callback(self, topic: str, callback):
+    def register_callback(self, topic: str, callback: Callable):
         """Registers callbacks for a given topic"""
         self.__callbacks[topic] = callback
 
     def remove_callback(self, topic: str):
         """Removes an existing callback"""
         self.__callbacks.pop(topic, None)
 
@@ -53,15 +56,15 @@
     def disconnect(self):
         """Disconnects from MirAIe"""
         self.__client.loop_stop()
         self.__client.disconnect()
 
     def set_temperature(self, topic: str, value: float):
         """Sets the Temperature to the given value"""
-        message = self.__build_temp_essage(value)
+        message = self.__build_temp_message(value)
         self.__client.publish(topic, message)
 
     def set_power(self, topic: str, value: PowerMode):
         """Sets the Power to the given value"""
         message = self.__build_power_message(value)
         self.__client.publish(topic, message)
 
@@ -76,17 +79,22 @@
         self.__client.publish(topic, message)
 
     def set_preset_mode(self, topic: str, value: PresetMode):
         """Sets the Preset to the given value"""
         message = self.__build_preset_mode_message(value)
         self.__client.publish(topic, message)
 
-    def set_swing_mode(self, topic: str, value: SwingMode):
-        """Sets the Swing to the given value"""
-        message = self.__build_swing_mode_message(value)
+    def set_vertical_swing_mode(self, topic: str, value: SwingMode):
+        """Sets the Vertical Swing to the given value"""
+        message = self.__build_vertical_swing_mode_message(value)
+        self.__client.publish(topic, message)
+
+    def set_horizontal_swing_mode(self, topic: str, value: SwingMode):
+        """Sets the Horizontal Swing to the given value"""
+        message = self.__build_horizontal_swing_mode_message(value)
         self.__client.publish(topic, message)
 
     def __generate_client_id(self):
         return (
             f"an{self.__generate_random_number(16)}{self.__generate_random_number(5)}"
         )
 
@@ -101,44 +109,43 @@
             protocol=paho.MQTTv31,
             clean_session=False,
         )
         self.__client.username_pw_set(
             username=self.__username, password=self.__password
         )
         self.__client.on_connect = self.__on_mqtt_connected
-        self.__client.on_message = self.__on_mqtt_message_received
         self.__client.on_disconnect = self.__on_mqtt_disconnected
-        self.__client.on_log = self.__on_mqtt_log
-        self.__client.tls_set(certfile=None, keyfile=None, cert_reqs=ssl.CERT_REQUIRED)
+        self.__client.on_message = self.__on_mqtt_message_received
 
-    def __on_mqtt_log(self, client, userdata, level, buff):
-        print("==========")
-        print("MQTT LOG:", buff)
-        print("level:", level)
-        print("userData", userdata)
-        print("==========")
+        if self.__useSsl:
+            self.__client.tls_set(certfile=None, keyfile=None, cert_reqs=ssl.CERT_REQUIRED)
 
     def __on_mqtt_connected(self, client: paho.Client, user_data, flags, rc):
         for topic in self.__topics:
             client.subscribe(topic, qos=1)
 
+    def __on_mqtt_disconnected(self, client: paho.Client, user_data, rc):
+        def callback(username: str, password: str):
+            self.__client.username_pw_set(username, password)
+            self.__client.reconnect()
+
+        if rc != 0:
+            self.__get_access_token_callback(callback)
+
     def __on_mqtt_message_received(self, client: paho.Client, user_data, message):
         parsed = json.loads(message.payload.decode("utf-8"))
         callback_func = self.__callbacks.get(message.topic)
         callback_func(parsed)
 
-    def __on_mqtt_disconnected(self, client: paho.Client, user_data, rc):
-        print("mqtt disconnected")
-
     def __build_power_message(self, mode: PowerMode):
         message = self.__build_base_message()
         message["ps"] = str(mode.value)
         return json.dumps(message)
 
-    def __build_temp_essage(self, temp: float):
+    def __build_temp_message(self, temp: float):
         message = self.__build_base_message()
         message["actmp"] = str(temp)
         return json.dumps(message)
 
     def __build_hvac_mode_message(self, mode: HVACMode):
         message = self.__build_base_message()
         message["acmd"] = str(mode.value)
@@ -160,18 +167,23 @@
             message["acpm"] = "off"
             message["actmp"] = 26.0
         elif mode == PresetMode.BOOST:
             message["acem"] = "off"
             message["acpm"] = "on"
         return json.dumps(message)
 
-    def __build_swing_mode_message(self, mode: SwingMode):
+    def __build_vertical_swing_mode_message(self, mode: SwingMode):
         message = self.__build_base_message()
         message["acvs"] = mode.value
         return json.dumps(message)
 
+    def __build_horizontal_swing_mode_message(self, mode: SwingMode):
+        message = self.__build_base_message()
+        message["achs"] = mode.value
+        return json.dumps(message)
+
     def __build_base_message(self):
         return {
             "ki": 1,
             "cnt": "an",
             "sid": "1",
         }
```

### Comparing `py-miraie-ac-0.0.9/src/py_miraie_ac/device.py` & `py-miraie-ac-0.1.0/src/py_miraie_ac/device.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 """The MirAIe device"""
+from __future__ import annotations
 from typing import Callable
 from py_miraie_ac.broker import MirAIeBroker
 from py_miraie_ac.deviceStatus import DeviceStatus
 from py_miraie_ac.enums import DisplayState, FanMode, HVACMode, PowerMode, PresetMode, SwingMode
 from py_miraie_ac.utils import to_float
 
 class Device:
     """The MirAIe device class"""
 
     __broker: MirAIeBroker
+    __callbacks: list[Callable]
 
     def __init__(
         self,
         device_id: str,
         name: str,
         friendly_name: str,
         control_topic: str,
@@ -22,17 +24,17 @@
         mac_address: str,
         category: str,
         brand: str,
         firmware_version: str,
         serial_number: str,
         model_number: str,
         product_serial_number: str,
-        area_name: str,
         status: DeviceStatus,
         broker: MirAIeBroker,
+        area_name: str
     ):
         self.device_id = device_id
         self.name = name
         self.friendly_name = friendly_name
         self.control_topic = control_topic
         self.status_topic = status_topic
         self.connection_status_topic = connection_status_topic
@@ -40,19 +42,19 @@
         self.mac_address = mac_address
         self.category = category
         self.brand = brand
         self.firmware_version = firmware_version
         self.serial_number = serial_number
         self.model_number = model_number
         self.product_serial_number = product_serial_number
-        self.area_name = area_name,
         self.status = status
+        self.area_name = area_name
 
         self.__broker = broker
-        self.__callbacks = set()
+        self.__callbacks = []
         self.__broker.register_callback(self.status_topic, self.status_callback_handler)
         self.__broker.register_callback(
             self.connection_status_topic, self.connection_callback_handler
         )
 
     def __publish_state(self):
         for callback in self.__callbacks:
@@ -71,22 +73,23 @@
 
         device_status = DeviceStatus(
             is_online=is_online,
             temperature=to_float(json["actmp"]),
             room_temp=to_float(json["rmtmp"]),
             power_mode=PowerMode(json["ps"]),
             fan_mode=FanMode(json["acfs"]),
-            swing_mode=SwingMode(json["acvs"]),
             display_state=DisplayState(json["acdc"]),
             hvac_mode=HVACMode(json["acmd"]),
             preset_mode=PresetMode.BOOST
             if json["acpm"] == "on"
             else PresetMode.ECO
             if json["acem"] == "on"
             else PresetMode.NONE,
+            vertical_swing_mode=SwingMode(json["acvs"]),
+            horizontal_swing_mode=SwingMode(json["achs"]),
         )
 
         return device_status
 
     def connection_callback_handler(self, status: dict):
         """Handles MQTT messages received on the connection status topic"""
 
@@ -114,18 +117,22 @@
         """Sets the fan mode"""
         self.__broker.set_fan_mode(self.control_topic, mode)
 
     def set_preset_mode(self, mode: PresetMode):
         """Sets the preset mode"""
         self.__broker.set_preset_mode(self.control_topic, mode)
 
-    def set_swing_mode(self, mode: SwingMode):
+    def set_vertical_swing_mode(self, mode: SwingMode):
         """Sets the swing mode"""
-        self.__broker.set_swing_mode(self.control_topic, mode)
+        self.__broker.set_vertical_swing_mode(self.control_topic, mode)
+
+    def set_horizontal_swing_mode(self, mode: SwingMode):
+        """Sets the swing mode"""
+        self.__broker.set_horizontal_swing_mode(self.control_topic, mode)
 
     def register_callback(self, callback: Callable[[], None]) -> None:
         """Registers a callback function"""
-        self.__callbacks.add(callback)
+        self.__callbacks.append(callback)
 
     def remove_callback(self, callback: Callable[[], None]) -> None:
         """Removes a callback function"""
-        self.__callbacks.discard(callback)
+        self.__callbacks.remove(callback)
```

### Comparing `py-miraie-ac-0.0.9/src/py_miraie_ac/enums.py` & `py-miraie-ac-0.1.0/src/py_miraie_ac/enums.py`

 * *Files identical despite different names*

### Comparing `py-miraie-ac-0.0.9/src/py_miraie_ac.egg-info/PKG-INFO` & `py-miraie-ac-0.1.0/src/py_miraie_ac.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-miraie-ac
-Version: 0.0.9
+Version: 0.1.0
 Summary: A package to control and read MirAIe Aircons by Panasonic
 Home-page: https://github.com/milothomas/py-miraie-ac
 Author: Milo Thomas
 Author-email: 20719501+milothomas@users.noreply.github.com
 Project-URL: Bug Tracker, https://github.com/milothomas/py-miraie-ac/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -22,16 +22,22 @@
 pip install py-miraie-ac
 ```
 
 **Usage**
 ```
 import asyncio
 from api import MirAIeAPI
-from enums import AuthType, SwingMode
+from enums import AuthType
 from device import Device
 
-async with MirAIeAPI(auth_type=AuthType.MOBILE, login_id=mobile_number, password=password) as api:
-        home:Home = await api.initialize()
-        for deviceId, device in home.devices.items():
-            print("Found device: ", device.friendly_name)
-            officeAc.set_temperature(24)
-            officeAc.turnOn()
+async with MirAIeAPI(
+        auth_type=AuthType.MOBILE, 
+        login_id="YOUR_MOBILE_NUMBER", 
+        password="YOUR_PASSWORD"
+    ) as api:
+    await api.initialize()
+    for device in api.devices:
+        print("Found device: ", device.friendly_name)
+        device.set_temperature(24)
+        device.turn_on()
+
+asyncio.get_event_loop().run_until_complete(start())
```

### Comparing `py-miraie-ac-0.0.9/src/py_miraie_ac.egg-info/SOURCES.txt` & `py-miraie-ac-0.1.0/src/py_miraie_ac.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 src/py_miraie_ac/broker.py
 src/py_miraie_ac/constants.py
 src/py_miraie_ac/device.py
 src/py_miraie_ac/deviceStatus.py
 src/py_miraie_ac/enums.py
 src/py_miraie_ac/exceptions.py
 src/py_miraie_ac/home.py
+src/py_miraie_ac/test.py
 src/py_miraie_ac/user.py
 src/py_miraie_ac/utils.py
 src/py_miraie_ac.egg-info/PKG-INFO
 src/py_miraie_ac.egg-info/SOURCES.txt
 src/py_miraie_ac.egg-info/dependency_links.txt
 src/py_miraie_ac.egg-info/requires.txt
 src/py_miraie_ac.egg-info/top_level.txt
```

