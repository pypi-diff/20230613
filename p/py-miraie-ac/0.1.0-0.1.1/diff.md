# Comparing `tmp/py-miraie-ac-0.1.0.tar.gz` & `tmp/py-miraie-ac-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-miraie-ac-0.1.0.tar", last modified: Tue Jun 13 02:53:38 2023, max compression
+gzip compressed data, was "py-miraie-ac-0.1.1.tar", last modified: Tue Jun 13 07:06:14 2023, max compression
```

## Comparing `py-miraie-ac-0.1.0.tar` & `py-miraie-ac-0.1.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 02:53:38.575922 py-miraie-ac-0.1.0/
--rw-rw-rw-   0        0        0    35821 2023-06-09 07:50:41.000000 py-miraie-ac-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     1273 2023-06-13 02:53:38.575922 py-miraie-ac-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      666 2023-06-13 02:52:22.000000 py-miraie-ac-0.1.0/README.md
--rw-rw-rw-   0        0        0      104 2023-06-09 16:09:32.000000 py-miraie-ac-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0      801 2023-06-13 02:53:38.576921 py-miraie-ac-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-13 02:53:38.458475 py-miraie-ac-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-13 02:53:38.566714 py-miraie-ac-0.1.0/src/py_miraie_ac/
--rw-rw-rw-   0        0        0      403 2023-06-09 13:16:33.000000 py-miraie-ac-0.1.0/src/py_miraie_ac/__init__.py
--rw-rw-rw-   0        0        0     6645 2023-06-12 15:09:04.000000 py-miraie-ac-0.1.0/src/py_miraie_ac/api.py
--rw-rw-rw-   0        0        0     6900 2023-06-12 15:07:29.000000 py-miraie-ac-0.1.0/src/py_miraie_ac/broker.py
--rw-rw-rw-   0        0        0      421 2023-06-05 03:33:43.000000 py-miraie-ac-0.1.0/src/py_miraie_ac/constants.py
--rw-rw-rw-   0        0        0     4928 2023-06-11 14:23:54.000000 py-miraie-ac-0.1.0/src/py_miraie_ac/device.py
--rw-rw-rw-   0        0        0      995 2023-06-10 12:09:13.000000 py-miraie-ac-0.1.0/src/py_miraie_ac/deviceStatus.py
--rw-rw-rw-   0        0        0      917 2023-06-05 03:55:22.000000 py-miraie-ac-0.1.0/src/py_miraie_ac/enums.py
--rw-rw-rw-   0        0        0      121 2023-06-05 03:55:32.000000 py-miraie-ac-0.1.0/src/py_miraie_ac/exceptions.py
--rw-rw-rw-   0        0        0      483 2023-06-09 13:29:18.000000 py-miraie-ac-0.1.0/src/py_miraie_ac/home.py
--rw-rw-rw-   0        0        0     1556 2023-06-12 15:09:49.000000 py-miraie-ac-0.1.0/src/py_miraie_ac/test.py
--rw-rw-rw-   0        0        0      460 2023-06-05 03:57:35.000000 py-miraie-ac-0.1.0/src/py_miraie_ac/user.py
--rw-rw-rw-   0        0        0      236 2023-06-09 13:29:27.000000 py-miraie-ac-0.1.0/src/py_miraie_ac/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-13 02:53:38.574932 py-miraie-ac-0.1.0/src/py_miraie_ac.egg-info/
--rw-rw-rw-   0        0        0     1273 2023-06-13 02:53:38.000000 py-miraie-ac-0.1.0/src/py_miraie_ac.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      569 2023-06-13 02:53:38.000000 py-miraie-ac-0.1.0/src/py_miraie_ac.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 02:53:38.000000 py-miraie-ac-0.1.0/src/py_miraie_ac.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-06-13 02:53:38.000000 py-miraie-ac-0.1.0/src/py_miraie_ac.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-13 02:53:38.000000 py-miraie-ac-0.1.0/src/py_miraie_ac.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-13 07:06:14.057970 py-miraie-ac-0.1.1/
+-rw-rw-rw-   0        0        0    35821 2023-06-09 07:50:41.000000 py-miraie-ac-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     1273 2023-06-13 07:06:14.057970 py-miraie-ac-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      666 2023-06-13 02:52:22.000000 py-miraie-ac-0.1.1/README.md
+-rw-rw-rw-   0        0        0      104 2023-06-09 16:09:32.000000 py-miraie-ac-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0      801 2023-06-13 07:06:14.059338 py-miraie-ac-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-13 07:06:14.010952 py-miraie-ac-0.1.1/src/
+drwxrwxrwx   0        0        0        0 2023-06-13 07:06:14.052980 py-miraie-ac-0.1.1/src/py_miraie_ac/
+-rw-rw-rw-   0        0        0      403 2023-06-09 13:16:33.000000 py-miraie-ac-0.1.1/src/py_miraie_ac/__init__.py
+-rw-rw-rw-   0        0        0     6764 2023-06-13 07:05:06.000000 py-miraie-ac-0.1.1/src/py_miraie_ac/api.py
+-rw-rw-rw-   0        0        0     6944 2023-06-13 07:04:03.000000 py-miraie-ac-0.1.1/src/py_miraie_ac/broker.py
+-rw-rw-rw-   0        0        0      421 2023-06-05 03:33:43.000000 py-miraie-ac-0.1.1/src/py_miraie_ac/constants.py
+-rw-rw-rw-   0        0        0     4928 2023-06-11 14:23:54.000000 py-miraie-ac-0.1.1/src/py_miraie_ac/device.py
+-rw-rw-rw-   0        0        0      995 2023-06-10 12:09:13.000000 py-miraie-ac-0.1.1/src/py_miraie_ac/deviceStatus.py
+-rw-rw-rw-   0        0        0      917 2023-06-05 03:55:22.000000 py-miraie-ac-0.1.1/src/py_miraie_ac/enums.py
+-rw-rw-rw-   0        0        0      121 2023-06-05 03:55:32.000000 py-miraie-ac-0.1.1/src/py_miraie_ac/exceptions.py
+-rw-rw-rw-   0        0        0      483 2023-06-09 13:29:18.000000 py-miraie-ac-0.1.1/src/py_miraie_ac/home.py
+-rw-rw-rw-   0        0        0     1585 2023-06-13 07:04:26.000000 py-miraie-ac-0.1.1/src/py_miraie_ac/test.py
+-rw-rw-rw-   0        0        0      460 2023-06-05 03:57:35.000000 py-miraie-ac-0.1.1/src/py_miraie_ac/user.py
+-rw-rw-rw-   0        0        0      236 2023-06-09 13:29:27.000000 py-miraie-ac-0.1.1/src/py_miraie_ac/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-13 07:06:14.057970 py-miraie-ac-0.1.1/src/py_miraie_ac.egg-info/
+-rw-rw-rw-   0        0        0     1273 2023-06-13 07:06:13.000000 py-miraie-ac-0.1.1/src/py_miraie_ac.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      569 2023-06-13 07:06:13.000000 py-miraie-ac-0.1.1/src/py_miraie_ac.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 07:06:13.000000 py-miraie-ac-0.1.1/src/py_miraie_ac.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-06-13 07:06:13.000000 py-miraie-ac-0.1.1/src/py_miraie_ac.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-13 07:06:13.000000 py-miraie-ac-0.1.1/src/py_miraie_ac.egg-info/top_level.txt
```

### Comparing `py-miraie-ac-0.1.0/LICENSE` & `py-miraie-ac-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `py-miraie-ac-0.1.0/PKG-INFO` & `py-miraie-ac-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-miraie-ac
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package to control and read MirAIe Aircons by Panasonic
 Home-page: https://github.com/milothomas/py-miraie-ac
 Author: Milo Thomas
 Author-email: 20719501+milothomas@users.noreply.github.com
 Project-URL: Bug Tracker, https://github.com/milothomas/py-miraie-ac/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `py-miraie-ac-0.1.0/README.md` & `py-miraie-ac-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `py-miraie-ac-0.1.0/setup.cfg` & `py-miraie-ac-0.1.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 792d 6d69 7261 6965 2d61 630d   = py-miraie-ac.
-00000020: 0a76 6572 7369 6f6e 203d 2030 2e31 2e30  .version = 0.1.0
+00000020: 0a76 6572 7369 6f6e 203d 2030 2e31 2e31  .version = 0.1.1
 00000030: 0d0a 6175 7468 6f72 203d 204d 696c 6f20  ..author = Milo 
 00000040: 5468 6f6d 6173 0d0a 6175 7468 6f72 5f65  Thomas..author_e
 00000050: 6d61 696c 203d 2032 3037 3139 3530 312b  mail = 20719501+
 00000060: 6d69 6c6f 7468 6f6d 6173 4075 7365 7273  milothomas@users
 00000070: 2e6e 6f72 6570 6c79 2e67 6974 6875 622e  .noreply.github.
 00000080: 636f 6d0d 0a64 6573 6372 6970 7469 6f6e  com..description
 00000090: 203d 2041 2070 6163 6b61 6765 2074 6f20   = A package to
```

### Comparing `py-miraie-ac-0.1.0/src/py_miraie_ac/api.py` & `py-miraie-ac-0.1.1/src/py_miraie_ac/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """The MirAIe API module"""
 
 import math
 import random
 import asyncio
+from typing import Callable
+
 import aiohttp
 from py_miraie_ac.broker import MirAIeBroker
 from py_miraie_ac.device import Device
 from py_miraie_ac.constants import DEVICE_DETAILS_URL, HOMES_URL,HTTP_CLIENT_ID,LOGIN_URL,STATUS_URL
 from py_miraie_ac.deviceStatus import DeviceStatus
 from py_miraie_ac.enums import (
     AuthType,
@@ -44,29 +46,32 @@
         self.__password = password
         self.__http_session = aiohttp.ClientSession()
 
     async def __aenter__(self):
         return self
 
     async def __aexit__(self, *excinfo):
-        await self.__http_session.close()
-        self.__broker.disconnect()
+        if "__http_session" in locals():
+            await self.__http_session.close()
+
+        if "__broker" in locals():
+            self.__broker.disconnect()
 
     async def initialize(self):
         """Initializes the MirAIe API"""
 
         self.__user = await self.__login()
         self.__broker = MirAIeBroker()
 
         self.__home = await self.__get_home_details()
         self.__broker.set_topics(self.__topics)
         self.__broker.init_broker(self.__home.home_id, self.__user.access_token, self.reconnect_broker)
         self.__broker.connect()
 
-    def reconnect_broker(self, reconnect_callback: callable):
+    def reconnect_broker(self, reconnect_callback: Callable):
         """Authenticates with MirAIe and reconnects to MQTT server with the new credentials"""
         loop = self.__http_session.loop
         fut = asyncio.run_coroutine_threadsafe(self.__login(), loop)
 
         self.__user = fut.result()
         reconnect_callback(self.__home.home_id, self.__user.access_token)
```

### Comparing `py-miraie-ac-0.1.0/src/py_miraie_ac/broker.py` & `py-miraie-ac-0.1.1/src/py_miraie_ac/broker.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,16 +51,17 @@
         self.__client.username_pw_set(
             username=self.__username, password=self.__password
         )
         self.connect()
 
     def disconnect(self):
         """Disconnects from MirAIe"""
-        self.__client.loop_stop()
-        self.__client.disconnect()
+        if "__client" in locals():
+            self.__client.loop_stop()
+            self.__client.disconnect()
 
     def set_temperature(self, topic: str, value: float):
         """Sets the Temperature to the given value"""
         message = self.__build_temp_message(value)
         self.__client.publish(topic, message)
 
     def set_power(self, topic: str, value: PowerMode):
```

### Comparing `py-miraie-ac-0.1.0/src/py_miraie_ac/device.py` & `py-miraie-ac-0.1.1/src/py_miraie_ac/device.py`

 * *Files identical despite different names*

### Comparing `py-miraie-ac-0.1.0/src/py_miraie_ac/deviceStatus.py` & `py-miraie-ac-0.1.1/src/py_miraie_ac/deviceStatus.py`

 * *Files identical despite different names*

### Comparing `py-miraie-ac-0.1.0/src/py_miraie_ac/enums.py` & `py-miraie-ac-0.1.1/src/py_miraie_ac/enums.py`

 * *Files identical despite different names*

### Comparing `py-miraie-ac-0.1.0/src/py_miraie_ac/test.py` & `py-miraie-ac-0.1.1/src/py_miraie_ac/test.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 """Test class"""
 import asyncio
 import time
+from typing import Callable
 from broker import MirAIeBroker
 from api import MirAIeAPI
 from enums import AuthType
 
 
 
 class Test:
     """TEST"""
     __test = 1
 
     def __init__(self):
         self.__test = 2
 
-    async def cb1(self, cbbroker: callable):
+    async def cb1(self, cbbroker: Callable):
         """Stuff"""
         await asyncio.sleep(3)
         cbbroker("user", "pwd")
 
     def start(self):
         """Test method"""
```

### Comparing `py-miraie-ac-0.1.0/src/py_miraie_ac.egg-info/PKG-INFO` & `py-miraie-ac-0.1.1/src/py_miraie_ac.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-miraie-ac
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package to control and read MirAIe Aircons by Panasonic
 Home-page: https://github.com/milothomas/py-miraie-ac
 Author: Milo Thomas
 Author-email: 20719501+milothomas@users.noreply.github.com
 Project-URL: Bug Tracker, https://github.com/milothomas/py-miraie-ac/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `py-miraie-ac-0.1.0/src/py_miraie_ac.egg-info/SOURCES.txt` & `py-miraie-ac-0.1.1/src/py_miraie_ac.egg-info/SOURCES.txt`

 * *Files identical despite different names*

