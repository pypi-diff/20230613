# Comparing `tmp/yalexs_ble-2.1.8.tar.gz` & `tmp/yalexs_ble-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yalexs_ble-2.1.8.tar", max compression
+gzip compressed data, was "yalexs_ble-2.1.9.tar", max compression
```

## Comparing `yalexs_ble-2.1.8.tar` & `yalexs_ble-2.1.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    35823 2023-03-26 21:08:52.726641 yalexs_ble-2.1.8/LICENSE
--rw-r--r--   0        0        0     3663 2023-03-26 21:08:52.726641 yalexs_ble-2.1.8/README.md
--rw-r--r--   0        0        0     2398 2023-03-26 21:08:53.530651 yalexs_ble-2.1.8/pyproject.toml
--rw-r--r--   0        0        0      871 2023-03-26 21:08:53.482651 yalexs_ble-2.1.8/src/yalexs_ble/__init__.py
--rw-r--r--   0        0        0     2225 2023-03-26 21:08:52.730641 yalexs_ble-2.1.8/src/yalexs_ble/const.py
--rw-r--r--   0        0        0    15048 2023-03-26 21:08:52.730641 yalexs_ble-2.1.8/src/yalexs_ble/lock.py
--rw-r--r--   0        0        0    32249 2023-03-26 21:08:52.730641 yalexs_ble-2.1.8/src/yalexs_ble/push.py
--rw-r--r--   0        0        0        0 2023-03-26 21:08:52.730641 yalexs_ble-2.1.8/src/yalexs_ble/py.typed
--rw-r--r--   0        0        0     2308 2023-03-26 21:08:52.730641 yalexs_ble-2.1.8/src/yalexs_ble/secure_session.py
--rw-r--r--   0        0        0     9415 2023-03-26 21:08:52.730641 yalexs_ble-2.1.8/src/yalexs_ble/session.py
--rw-r--r--   0        0        0     2642 2023-03-26 21:08:52.730641 yalexs_ble-2.1.8/src/yalexs_ble/util.py
--rw-r--r--   0        0        0     5096 1970-01-01 00:00:00.000000 yalexs_ble-2.1.8/PKG-INFO
+-rw-r--r--   0        0        0    35823 2023-03-26 21:19:09.562610 yalexs_ble-2.1.9/LICENSE
+-rw-r--r--   0        0        0     3663 2023-03-26 21:19:09.562610 yalexs_ble-2.1.9/README.md
+-rw-r--r--   0        0        0     2398 2023-03-26 21:19:10.358600 yalexs_ble-2.1.9/pyproject.toml
+-rw-r--r--   0        0        0      871 2023-03-26 21:19:10.310600 yalexs_ble-2.1.9/src/yalexs_ble/__init__.py
+-rw-r--r--   0        0        0     2225 2023-03-26 21:19:09.566610 yalexs_ble-2.1.9/src/yalexs_ble/const.py
+-rw-r--r--   0        0        0    15275 2023-03-26 21:19:09.566610 yalexs_ble-2.1.9/src/yalexs_ble/lock.py
+-rw-r--r--   0        0        0    32249 2023-03-26 21:19:09.566610 yalexs_ble-2.1.9/src/yalexs_ble/push.py
+-rw-r--r--   0        0        0        0 2023-03-26 21:19:09.566610 yalexs_ble-2.1.9/src/yalexs_ble/py.typed
+-rw-r--r--   0        0        0     2308 2023-03-26 21:19:09.566610 yalexs_ble-2.1.9/src/yalexs_ble/secure_session.py
+-rw-r--r--   0        0        0     9539 2023-03-26 21:19:09.566610 yalexs_ble-2.1.9/src/yalexs_ble/session.py
+-rw-r--r--   0        0        0     2642 2023-03-26 21:19:09.566610 yalexs_ble-2.1.9/src/yalexs_ble/util.py
+-rw-r--r--   0        0        0     5096 1970-01-01 00:00:00.000000 yalexs_ble-2.1.9/PKG-INFO
```

### Comparing `yalexs_ble-2.1.8/LICENSE` & `yalexs_ble-2.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `yalexs_ble-2.1.8/README.md` & `yalexs_ble-2.1.9/README.md`

 * *Files identical despite different names*

### Comparing `yalexs_ble-2.1.8/pyproject.toml` & `yalexs_ble-2.1.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "yalexs-ble"
-version = "2.1.8"
+version = "2.1.9"
 description = "Bluetooth control of Yale and August locks"
 authors = ["J. Nick Koston <nick@koston.org>"]
 license = "GNU General Public License v3.0"
 readme = "README.md"
 repository = "https://github.com/bdraco/yalexs-ble"
 documentation = "https://yalexs-ble.readthedocs.io"
 classifiers = [
```

### Comparing `yalexs_ble-2.1.8/src/yalexs_ble/__init__.py` & `yalexs_ble-2.1.9/src/yalexs_ble/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     local_name_is_unique,
     local_name_to_serial,
     serial_to_local_name,
     unique_id_from_device_adv,
     unique_id_from_local_name_address,
 )
 
-__version__ = "2.1.8"
+__version__ = "2.1.9"
 
 __all__ = [
     "AuthError",
     "ConnectionInfo",
     "DisconnectedError",
     "DoorStatus",
     "Lock",
```

### Comparing `yalexs_ble-2.1.8/src/yalexs_ble/const.py` & `yalexs_ble-2.1.9/src/yalexs_ble/const.py`

 * *Files identical despite different names*

### Comparing `yalexs_ble-2.1.8/src/yalexs_ble/lock.py` & `yalexs_ble-2.1.9/src/yalexs_ble/lock.py`

 * *Files 2% similar despite different names*

```diff
@@ -228,15 +228,17 @@
         _LOGGER.debug("%s: Setting up the session", self.name)
         self.secure_session.set_key(self.key)
         handshake_keys = os.urandom(16)
 
         # Send SEC_LOCK_TO_MOBILE_KEY_EXCHANGE
         cmd = self.secure_session.build_command(0x01)
         util._copy(cmd, handshake_keys[0x00:0x08], destLocation=0x04)
-        response = await self.secure_session.execute(cmd)
+        response = await self.secure_session.execute(
+            cmd, "SEC_LOCK_TO_MOBILE_KEY_EXCHANGE"
+        )
         if response[0x00] != 0x02:
             raise AuthError(
                 "Authentication error: key or slot (key index) is incorrect: unexpected response to SEC_LOCK_TO_MOBILE_KEY_EXCHANGE: "
                 + response.hex()
             )
 
         self.is_secure = True
@@ -245,15 +247,15 @@
         util._copy(session_key, handshake_keys[0x00:0x08])
         util._copy(session_key, response[0x04:0x0C], destLocation=0x08)
         self.secure_session.set_key(session_key)
 
         # Send SEC_INITIALIZATION_COMMAND
         cmd = self.secure_session.build_command(0x03)
         util._copy(cmd, handshake_keys[0x08:0x10], destLocation=0x04)
-        response = await self.secure_session.execute(cmd)
+        response = await self.secure_session.execute(cmd, "SEC_INITIALIZATION_COMMAND")
         if response[0] != 0x04:
             raise AuthError(
                 "Authentication error: key or slot (key index) is incorrect: unexpected response to SEC_INITIALIZATION_COMMAND: "
                 + response.hex()
             )
         self.session.set_key(session_key)
 
@@ -279,37 +281,41 @@
         return self._lock_info
 
     @raise_if_not_connected
     async def force_lock(self) -> None:
         """Force the lock to lock."""
         _LOGGER.debug("%s: Locking", self.name)
         assert self.session is not None  # nosec
-        await self.session.execute(self.session.build_command(Commands.LOCK.value))
+        await self.session.execute(
+            self.session.build_command(Commands.LOCK.value), "force_lock"
+        )
         _LOGGER.debug("%s: Finished locking", self.name)
 
     @raise_if_not_connected
     async def force_unlock(self) -> None:
         """Force the lock to unlock."""
         _LOGGER.debug("%s: Unlocking", self.name)
         assert self.session is not None  # nosec
-        await self.session.execute(self.session.build_command(Commands.UNLOCK.value))
+        await self.session.execute(
+            self.session.build_command(Commands.UNLOCK.value), "force_unlock"
+        )
         _LOGGER.debug("%s: Finished unlocking", self.name)
 
     async def lock(self) -> None:
         if (await self.status()).lock == LockStatus.UNLOCKED:
             await self.force_lock()
 
     async def unlock(self) -> None:
         if (await self.status()).lock == LockStatus.LOCKED:
             await self.force_unlock()
 
-    async def _execute_command(self, cmd_byte: int) -> bytes:
+    async def _execute_command(self, cmd_byte: int, command_name: str) -> bytes:
         assert self.session is not None  # nosec
         response = await self.session.execute(
-            self.session.build_operation_command(cmd_byte)
+            self.session.build_operation_command(cmd_byte), command_name
         )
         _LOGGER.debug("%s: response: [%s]", self.name, response.hex())
         return response
 
     def _parse_lock_and_door_state(
         self, response: bytes
     ) -> tuple[LockStatus, DoorStatus]:
@@ -329,15 +335,15 @@
             )
         return lock_status_enum, door_status_enum
 
     @raise_if_not_connected
     async def status(self) -> LockState:
         _LOGGER.debug("%s: Executing status", self.name)
         response = await self._execute_command(
-            0x2F if self._lock_info and self._lock_info.door_sense else 0x02
+            0x2F if self._lock_info and self._lock_info.door_sense else 0x02, "status"
         )
         _LOGGER.debug("%s: Finished executing status", self.name)
         return LockState(*self._parse_lock_and_door_state(response), None, None)
 
     def _parse_battery_state(self, response: bytes) -> BatteryState:
         """Parse the battery state from the response."""
         voltage = (response[0x09] * 256 + response[0x08]) / 1000
@@ -348,15 +354,15 @@
         # this is the best we can do for now.
         percentage = convert_voltage_to_percentage(voltage / 4)
         return BatteryState(voltage, percentage)
 
     @raise_if_not_connected
     async def battery(self) -> BatteryState:
         _LOGGER.debug("%s: Executing battery", self.name)
-        response = await self._execute_command(0x0F)
+        response = await self._execute_command(0x0F, "battery")
         _LOGGER.debug("%s: Finished executing battery", self.name)
         return self._parse_battery_state(response)
 
     async def disconnect(self) -> None:
         """Disconnect from the lock."""
         _LOGGER.debug("%s: Disconnecting from the lock", self.name)
         if not self.client or not self.client.is_connected:
@@ -376,15 +382,15 @@
             or self._disconnected_event is None
         ):
             return
         cmd = self.secure_session.build_command(0x05)
         cmd[0x11] = 0x00
         response = None
         try:
-            response = await self.secure_session.execute(cmd)
+            response = await self.secure_session.execute(cmd, "shutdown")
         except (AuthError, DisconnectedError):
             # Lock already disconnected us
             return
         except (BleakError, asyncio.TimeoutError, EOFError) as err:
             if not util.is_disconnected_error(err):
                 _LOGGER.debug(
                     "%s: Failed to cleanly disconnect from lock: %s", self.name, err
```

### Comparing `yalexs_ble-2.1.8/src/yalexs_ble/push.py` & `yalexs_ble-2.1.9/src/yalexs_ble/push.py`

 * *Files identical despite different names*

### Comparing `yalexs_ble-2.1.8/src/yalexs_ble/secure_session.py` & `yalexs_ble-2.1.9/src/yalexs_ble/secure_session.py`

 * *Files identical despite different names*

### Comparing `yalexs_ble-2.1.8/src/yalexs_ble/session.py` & `yalexs_ble-2.1.9/src/yalexs_ble/session.py`

 * *Files 3% similar despite different names*

```diff
@@ -118,18 +118,18 @@
         )
         if util._simple_checksum(response) != 0:
             raise ResponseError(f"Simple checksum mismatch {response!r}")
 
         if response[0x00] != 0xBB and response[0x00] != 0xAA:
             raise ResponseError(f"Incorrect flag in response: {response[0x00]}")
 
-    async def _write(self, command: bytearray) -> bytes:
+    async def _write(self, command: bytearray, command_name: str) -> bytes:
         """Write under the lock."""
         async with self._lock:
-            return await self._locked_write(command)
+            return await self._locked_write(command, command_name)
 
     def _notify(self, char: int, data: bytes) -> None:
         _LOGGER.debug(
             "%s: Receiving response via notify: %s (waiting=%s)",
             self.name,
             data.hex(),
             bool(self._notify_future),
@@ -148,26 +148,28 @@
             _LOGGER.debug("%s: Invalid response, waiting for next one", self.name)
             self._notify_future.set_exception(ex)
             self._notify_future = None
             return
         self._notify_future.set_result(decrypted_data)
         self._notify_future = None
 
-    async def _locked_write(self, command: bytearray) -> bytes:
+    async def _locked_write(self, command: bytearray, command_name: str) -> bytes:
         # NOTE: The last two bytes are not encrypted
         # General idea seems to be that if the last byte
         # of the command indicates an offline key offset (is non-zero),
         # the command is "secure" and encrypted with the offline key
         if not self.client.is_connected or self._disconnected_event.is_set():
             raise BleakError("disconnected")
         assert self.cipher_encrypt is not None, "Cipher not set"  # nosec
         plainText = command[0x00:0x10]
         cipherText = self.cipher_encrypt.update(plainText)
         util._copy(command, cipherText)
-        _LOGGER.debug("%s: Encrypted command: %s", self.name, command.hex())
+        _LOGGER.debug(
+            "%s: Encrypted command %s: %s", self.name, command_name, command.hex()
+        )
 
         for attempt in range(3):
             future: asyncio.Future[bytes] = asyncio.Future()
             self._notify_future = future
             _LOGGER.debug(
                 "%s: Writing command to %s: %s",
                 self.name,
@@ -227,19 +229,19 @@
         except EOFError as err:
             _LOGGER.debug("%s: D-Bus stopping notify: %s", self.name, err)
             pass
         except BleakError as err:
             _LOGGER.debug("%s: Bleak error stopping notify: %s", self.name, err)
             pass
 
-    async def execute(self, command: bytearray) -> bytes:
+    async def execute(self, command: bytearray, command_name: str) -> bytes:
         """Execute command."""
         assert self.cipher_encrypt is not None, "Cipher not set"  # nosec
         self._write_checksum(command)
-        write_task = asyncio.create_task(self._write(command))
+        write_task = asyncio.create_task(self._write(command, command_name))
         disconnect_task = asyncio.create_task(self._disconnected_event.wait())
         await asyncio.wait(
             (write_task, disconnect_task),
             return_when=asyncio.FIRST_COMPLETED,
         )
         if disconnect_task.done():
             write_task.cancel()
```

### Comparing `yalexs_ble-2.1.8/src/yalexs_ble/util.py` & `yalexs_ble-2.1.9/src/yalexs_ble/util.py`

 * *Files identical despite different names*

### Comparing `yalexs_ble-2.1.8/PKG-INFO` & `yalexs_ble-2.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yalexs-ble
-Version: 2.1.8
+Version: 2.1.9
 Summary: Bluetooth control of Yale and August locks
 Home-page: https://github.com/bdraco/yalexs-ble
 License: GNU General Public License v3.0
 Author: J. Nick Koston
 Author-email: nick@koston.org
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: yalexs-ble Version: 2.1.8 Summary: Bluetooth
+Metadata-Version: 2.1 Name: yalexs-ble Version: 2.1.9 Summary: Bluetooth
 control of Yale and August locks Home-page: https://github.com/bdraco/yalexs-
 ble License: GNU General Public License v3.0 Author: J. Nick Koston Author-
 email: nick@koston.org Requires-Python: >=3.9,<4.0 Classifier: Development
 Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers Classifier:
 License :: Other/Proprietary License Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

