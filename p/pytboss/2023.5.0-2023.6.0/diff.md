# Comparing `tmp/pytboss-2023.5.0.tar.gz` & `tmp/pytboss-2023.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytboss-2023.5.0.tar", last modified: Wed May 17 12:57:37 2023, max compression
+gzip compressed data, was "pytboss-2023.6.0.tar", last modified: Tue Jun 13 02:33:51 2023, max compression
```

## Comparing `pytboss-2023.5.0.tar` & `pytboss-2023.6.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:57:37.813426 pytboss-2023.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-17 12:57:11.000000 pytboss-2023.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-17 12:57:11.000000 pytboss-2023.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8897 2023-05-17 12:57:37.813426 pytboss-2023.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8237 2023-05-17 12:57:11.000000 pytboss-2023.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-05-17 12:57:11.000000 pytboss-2023.5.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:57:37.809426 pytboss-2023.5.0/pytboss/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-17 12:57:11.000000 pytboss-2023.5.0/pytboss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-17 12:57:37.000000 pytboss-2023.5.0/pytboss/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     9359 2023-05-17 12:57:11.000000 pytboss-2023.5.0/pytboss/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7798 2023-05-17 12:57:11.000000 pytboss-2023.5.0/pytboss/ble.py
--rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-05-17 12:57:11.000000 pytboss-2023.5.0/pytboss/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-17 12:57:11.000000 pytboss-2023.5.0/pytboss/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-05-17 12:57:11.000000 pytboss-2023.5.0/pytboss/fs.py
--rw-r--r--   0 runner    (1001) docker     (123)   537876 2023-05-17 12:57:11.000000 pytboss-2023.5.0/pytboss/grills.json
--rw-r--r--   0 runner    (1001) docker     (123)     6089 2023-05-17 12:57:11.000000 pytboss-2023.5.0/pytboss/grills.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:57:37.813426 pytboss-2023.5.0/pytboss.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8897 2023-05-17 12:57:37.000000 pytboss-2023.5.0/pytboss.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-17 12:57:37.000000 pytboss-2023.5.0/pytboss.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 12:57:37.000000 pytboss-2023.5.0/pytboss.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-17 12:57:37.000000 pytboss-2023.5.0/pytboss.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-17 12:57:37.000000 pytboss-2023.5.0/pytboss.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 12:57:37.000000 pytboss-2023.5.0/pytboss.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-17 12:57:11.000000 pytboss-2023.5.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-17 12:57:11.000000 pytboss-2023.5.0/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-17 12:57:11.000000 pytboss-2023.5.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 12:57:37.813426 pytboss-2023.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:33:51.903314 pytboss-2023.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-13 02:33:33.000000 pytboss-2023.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-13 02:33:33.000000 pytboss-2023.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8897 2023-06-13 02:33:51.903314 pytboss-2023.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8237 2023-06-13 02:33:33.000000 pytboss-2023.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-06-13 02:33:33.000000 pytboss-2023.6.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:33:51.899314 pytboss-2023.6.0/pytboss/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-13 02:33:33.000000 pytboss-2023.6.0/pytboss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-13 02:33:51.000000 pytboss-2023.6.0/pytboss/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9720 2023-06-13 02:33:33.000000 pytboss-2023.6.0/pytboss/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8093 2023-06-13 02:33:33.000000 pytboss-2023.6.0/pytboss/ble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-06-13 02:33:33.000000 pytboss-2023.6.0/pytboss/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-13 02:33:33.000000 pytboss-2023.6.0/pytboss/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-13 02:33:33.000000 pytboss-2023.6.0/pytboss/fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   537876 2023-06-13 02:33:33.000000 pytboss-2023.6.0/pytboss/grills.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6089 2023-06-13 02:33:33.000000 pytboss-2023.6.0/pytboss/grills.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:33:51.903314 pytboss-2023.6.0/pytboss.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8897 2023-06-13 02:33:51.000000 pytboss-2023.6.0/pytboss.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-13 02:33:51.000000 pytboss-2023.6.0/pytboss.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 02:33:51.000000 pytboss-2023.6.0/pytboss.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-13 02:33:51.000000 pytboss-2023.6.0/pytboss.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-13 02:33:51.000000 pytboss-2023.6.0/pytboss.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 02:33:51.000000 pytboss-2023.6.0/pytboss.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-13 02:33:33.000000 pytboss-2023.6.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-13 02:33:33.000000 pytboss-2023.6.0/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-13 02:33:33.000000 pytboss-2023.6.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 02:33:51.903314 pytboss-2023.6.0/setup.cfg
```

### Comparing `pytboss-2023.5.0/LICENSE` & `pytboss-2023.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytboss-2023.5.0/PKG-INFO` & `pytboss-2023.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytboss
-Version: 2023.5.0
+Version: 2023.6.0
 Summary: Python library for interacting with Pitboss grills and smokers.
 Author-email: David Knowles <dknowles2@gmail.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/dknowles2/pyschlage
 Project-URL: Source Code, https://github.com/dknowles2/pyschlage
 Project-URL: Bug Reports, https://github.com/dknowles2/pyschlage/issues
 Keywords: pitboss,api,iot,ble
```

### Comparing `pytboss-2023.5.0/README.md` & `pytboss-2023.6.0/README.md`

 * *Files identical despite different names*

### Comparing `pytboss-2023.5.0/pyproject.toml` & `pytboss-2023.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytboss-2023.5.0/pytboss/api.py` & `pytboss-2023.6.0/pytboss/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 """Client library for interacting with PitBoss grills over Bluetooth LE."""
 
 import asyncio
 import inspect
 import json
+import logging
 from typing import Awaitable, Callable, TypedDict
 
 from . import grills
 from .ble import BleConnection
 from .config import Config
 from .fs import FileSystem
 
+_LOGGER = logging.getLogger("pytboss")
+
 
 class StateDict(TypedDict, total=False):
     """State of the grill."""
 
     p1Target: int
     """Target temperature for meat probe 1."""
 
@@ -123,14 +126,18 @@
         self._spec: grills.Grill = grills.get_grill(grill_model)
         self._conn = conn
         self._lock = asyncio.Lock()  # protects callbacks and state.
         self._state_callbacks = []
         self._vdata_callbacks = []
         self._state = StateDict()
 
+    def is_connected(self) -> bool:
+        """Returns whether we are actively connected to the grill."""
+        return self._conn.is_connected()
+
     async def start(self):
         """Sets up the API for use.
 
         Required to be called before the API can be used.
         """
         # TODO: Add support for stop()
         await self._conn.connect()
@@ -153,14 +160,15 @@
         :type callback: VDataCallback
         """
         # TODO: Return a handle for unsubscribe.
         async with self._lock:
             self._vdata_callbacks.append(callback)
 
     async def _on_debug_log_received(self, data: bytearray):
+        _LOGGER.debug("Debug log received: %s", data)
         parts = data.decode("utf-8").split()
         if len(parts) != 3:
             # Unknown payload; ignore.
             return
 
         head, payload, tail = parts
         checksum = int(tail[1 : len(tail) - 1])  # noqa: E203
@@ -169,14 +177,15 @@
             return
         if head == "<==PB:":
             await self._on_state_received(payload)
         elif head == "<==PBD:":
             await self._on_vdata_received(payload)
 
     async def _on_state_received(self, payload: str):
+        _LOGGER.debug("State received: %s", payload)
         state = None
         match payload[:4]:
             case "FE0B":
                 state = self._spec.control_board.parse_status(payload)
             case "FE0C":
                 state = self._spec.control_board.parse_temperatures(payload)
 
@@ -192,14 +201,15 @@
                 if inspect.iscoroutinefunction(callback):
                     await callback(self._state)
                 else:
                     callback(self._state)
 
     async def _on_vdata_received(self, payload: bytearray):
         vdata = json.loads(payload)
+        _LOGGER.debug("VData received: %s", vdata)
         async with self._lock:
             # TODO: Run callbacks concurrently
             # TODO: Send copies of state so subscribers can't modify it
             for callback in self._vdata_callbacks:
                 if inspect.iscoroutinefunction(callback):
                     await callback(vdata)
                 else:
```

### Comparing `pytboss-2023.5.0/pytboss/ble.py` & `pytboss-2023.6.0/pytboss/ble.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,23 +5,26 @@
   https://mongoose-os.com/docs/mongoose-os/api/net/bt-service-debug.md
 """
 
 from __future__ import annotations
 
 import asyncio
 import json
+import logging
 from typing import Awaitable, Callable
 from uuid import UUID
 
 from bleak import BleakClient, BleakGATTCharacteristic, BLEDevice
 import bleak_retry_connector
 from bleak_retry_connector import BleakClientWithServiceCache
 
 from .exceptions import RPCError
 
+_LOGGER = logging.getLogger("pytboss")
+
 
 def _uuid(s: str) -> str:
     return str(UUID(bytes=s.encode()))
 
 
 # See: https://mongoose-os.com/docs/mongoose-os/api/net/bt-service-debug.md
 SERVICE_DEBUG = _uuid("_mOS_DBG_SVC_ID_")
@@ -64,44 +67,48 @@
         self._last_command_id = 0
         self._rpc_futures = {}
         self._debug_log_callback: DebugLogCallback | None = None
 
     async def connect(self) -> None:
         """Starts the connection to the device."""
         if self._is_connected:
+            _LOGGER.warning("Already connected. Ignoring call to connect().")
             return
         self._ble_client = await bleak_retry_connector.establish_connection(
             client_class=BleakClientWithServiceCache,
             device=self._ble_device,
             name=self._ble_device.name,
             disconnected_callback=self._on_disconnected,
         )
         self._is_connected = True
         await self._ble_client.start_notify(CHAR_RPC_RX_CTL, self._on_rpc_data_received)
 
     def _on_disconnected(self, unused_client):
         """Called when our Bluetooth client is disconnected."""
+        _LOGGER.debug("Bluetooth disconnected.")
         self._is_connected = False
 
     async def disconnect(self) -> None:
         """Stops the connection to the device."""
+        _LOGGER.debug("Disconnecting from device.")
         if self._ble_client:
             try:
                 await self._ble_client.disconnect()
             except:
                 # Bluetooth is awful. Sometimes even disconnects fail.
                 pass
         self._is_connected = False
 
     async def reset_device(self, ble_device: BLEDevice):
         """Resets the BLE device used for transport.
 
         :param ble_device: BLE device to use for transport.
         :type ble_device: bleak.BLEDevice
         """
+        _LOGGER.debug("Resetting device to: %s", ble_device)
         await self.disconnect()
         self._is_connected = False
         self._ble_device = ble_device
         await self.connect()
         async with self._lock:
             if self._debug_log_callback:
                 await self._ble_client.start_notify(
```

### Comparing `pytboss-2023.5.0/pytboss/config.py` & `pytboss-2023.6.0/pytboss/config.py`

 * *Files identical despite different names*

### Comparing `pytboss-2023.5.0/pytboss/fs.py` & `pytboss-2023.6.0/pytboss/fs.py`

 * *Files identical despite different names*

### Comparing `pytboss-2023.5.0/pytboss/grills.json` & `pytboss-2023.6.0/pytboss/grills.json`

 * *Files identical despite different names*

### Comparing `pytboss-2023.5.0/pytboss/grills.py` & `pytboss-2023.6.0/pytboss/grills.py`

 * *Files identical despite different names*

### Comparing `pytboss-2023.5.0/pytboss.egg-info/PKG-INFO` & `pytboss-2023.6.0/pytboss.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytboss
-Version: 2023.5.0
+Version: 2023.6.0
 Summary: Python library for interacting with Pitboss grills and smokers.
 Author-email: David Knowles <dknowles2@gmail.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/dknowles2/pyschlage
 Project-URL: Source Code, https://github.com/dknowles2/pyschlage
 Project-URL: Bug Reports, https://github.com/dknowles2/pyschlage/issues
 Keywords: pitboss,api,iot,ble
```

