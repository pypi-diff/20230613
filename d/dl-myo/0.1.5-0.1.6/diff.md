# Comparing `tmp/dl_myo-0.1.5.tar.gz` & `tmp/dl_myo-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "dl_myo-0.1.6.tar", max compression
```

## Comparing `dl_myo-0.1.5.tar` & `dl_myo-0.1.6.tar`

### file list

```diff
@@ -1,12 +1,9 @@
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 dl_myo-0.1.5/Dockerfile
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 dl_myo-0.1.5/docker-compose.yml
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 dl_myo-0.1.5/myo/__init__.py
--rw-r--r--   0        0        0     3226 2020-02-02 00:00:00.000000 dl_myo-0.1.5/myo/commands.py
--rw-r--r--   0        0        0     6625 2020-02-02 00:00:00.000000 dl_myo-0.1.5/myo/device.py
--rw-r--r--   0        0        0     6131 2020-02-02 00:00:00.000000 dl_myo-0.1.5/myo/handle.py
--rw-r--r--   0        0        0     5891 2020-02-02 00:00:00.000000 dl_myo-0.1.5/myo/types.py
--rw-r--r--   0        0        0     2741 2020-02-02 00:00:00.000000 dl_myo-0.1.5/.gitignore
--rw-r--r--   0        0        0    35131 2020-02-02 00:00:00.000000 dl_myo-0.1.5/LICENSE
--rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 dl_myo-0.1.5/README.md
--rw-r--r--   0        0        0     3237 2020-02-02 00:00:00.000000 dl_myo-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     3391 2020-02-02 00:00:00.000000 dl_myo-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    35131 2023-06-13 18:39:07.020525 dl_myo-0.1.6/LICENSE
+-rw-r--r--   0        0        0     2514 2023-06-13 18:39:07.020525 dl_myo-0.1.6/README.md
+-rw-r--r--   0        0        0      455 2023-06-13 18:39:07.020525 dl_myo-0.1.6/myo/__init__.py
+-rw-r--r--   0        0        0     3226 2023-06-13 18:39:07.020525 dl_myo-0.1.6/myo/commands.py
+-rw-r--r--   0        0        0     6562 2023-06-13 18:39:07.020525 dl_myo-0.1.6/myo/device.py
+-rw-r--r--   0        0        0     6485 2023-06-13 18:39:07.024525 dl_myo-0.1.6/myo/handle.py
+-rw-r--r--   0        0        0     9457 2023-06-13 18:39:07.024525 dl_myo-0.1.6/myo/types.py
+-rw-r--r--   0        0        0     3140 2023-06-13 18:39:28.676804 dl_myo-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     3052 1970-01-01 00:00:00.000000 dl_myo-0.1.6/PKG-INFO
```

### Comparing `dl_myo-0.1.5/myo/commands.py` & `dl_myo-0.1.6/myo/commands.py`

 * *Files identical despite different names*

### Comparing `dl_myo-0.1.5/myo/device.py` & `dl_myo-0.1.6/myo/device.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from __future__ import annotations
 
 import binascii
 import json
 import logging
 
 from bleak import BleakClient, BleakScanner
+from bleak.backends.characteristic import BleakGATTCharacteristic
 from bleak.backends.device import BLEDevice
 from bleak.backends.scanner import AdvertisementData
 
 from .commands import (
     Command,
     SetMode,
     Vibrate,
@@ -48,17 +49,15 @@
             if mac.lower() == device.address.lower():
                 return True
             return False
 
         self = cls()
         try:
             # scan the device
-            self.__device = await BleakScanner.find_device_by_filter(
-                match_myo_mac, cb=dict(use_bdaddr=True)
-            )
+            self.__device = await BleakScanner.find_device_by_filter(match_myo_mac, cb=dict(use_bdaddr=True))
             if self.device is None:
                 logger.error(f"could not find device with address {mac}")
                 return self
         except Exception as e:
             logger.error("the mac address may be invalid", e)
             return self
 
@@ -72,17 +71,15 @@
         def match_myo_uuid(_: BLEDevice, adv: AdvertisementData):
             if str(UUID.MYO_SERVICE).lower() in adv.service_uuids:
                 return True
             return False
 
         self = cls()
         # scan the device
-        self.__device = await BleakScanner.find_device_by_filter(
-            match_myo_uuid, cb=dict(use_bdaddr=True)
-        )
+        self.__device = await BleakScanner.find_device_by_filter(match_myo_uuid, cb=dict(use_bdaddr=True))
         if self.device is None:
             logger.error(f"could not find device with service UUID {UUID.MYO_SERVICE}")
             return self
 
         # get the device name
         self.__name = str(self.device.name)
 
@@ -103,67 +100,38 @@
 
     async def deep_sleep(self, client: BleakClient):
         """
         Deep Sleep Command
         """
         await self.command(client, DeepSleep())
 
-    async def emg_service(self, client):
-        """
-        EMG Service
-        """
-        await client.write_gatt_char(Handle.EMG_SERVICE.value, b"\x01\x00", True)
-
     async def get_services(self, client: BleakClient, indent=2) -> str:
         """fetch available services as dict"""
-        sd = {"services": {}}
+        sd = {}
         for service in client.services:  # BleakGATTServiceCollection
             try:
                 service_name = Handle(service.handle).name
             except Exception as e:
                 logger.debug("unknown handle: {}", e)
                 continue
 
-            sd["services"][service.handle] = {
-                "name": service_name,
-                "uuid": service.uuid,
-                "chars": {},
-            }
+            chars = {}
             for char in service.characteristics:  # List[BleakGATTCharacteristic]
-                try:
-                    char_name = Handle(char.handle).name
-                except Exception as e:
-                    logger.debug("unknown handle: {}", e)
-                    continue
-
-                value = None
-                if "read" in char.properties:
-                    blob = await client.read_gatt_char(char.handle)
-                    if char_name == Handle.MANUFACTURER_NAME_STRING.name:
-                        value = blob.decode("utf-8")
-                    elif char_name == Handle.FIRMWARE_INFO.name:
-                        value = FirmwareInfo(blob).to_dict()
-                    elif char_name == Handle.FIRMWARE_VERSION.name:
-                        value = str(FirmwareVersion(blob))
-                    elif char_name == Handle.BATTERY_LEVEL.name:
-                        value = ord(blob)
-                    else:
-                        value = binascii.b2a_hex(blob).decode("utf-8")
-
-                sd["services"][service.handle]["chars"][char.handle] = {
-                    "name": char_name,
-                    "uuid": char.uuid,
-                    "properties": ",".join(char.properties),
-                    "value": value,
-                }
+                cd = await gatt_char_to_dict(client, char)
+                if cd:
+                    chars[hex(char.handle)] = cd
 
             # end char
+            sd[hex(service.handle)] = {
+                "name": service_name,
+                "uuid": service.uuid,
+                "chars": chars,
+            }
         # end service
-
-        return json.dumps(sd, indent=indent)
+        return json.dumps({"services": sd}, indent=indent)
 
     async def led(self, client: BleakClient, *args):
         """
         LED Command
             - set leds color
 
         *args: [logoR, logoG, logoB], [lineR, lineG, lineB]
@@ -210,7 +178,44 @@
         await self.command(client, Vibrate(vibration_type))
 
     async def vibrate2(self, client: BleakClient, duration, strength):
         """
         Vibrate2 Command
         """
         await self.command(client, Vibrate2(duration, strength))
+
+    async def write(self, client, handle, value):
+        """
+        Write characteristic
+        """
+        await client.write_gatt_char(handle, value, True)
+
+
+async def gatt_char_to_dict(client: BleakClient, char: BleakGATTCharacteristic):
+    try:
+        char_name = Handle(char.handle).name
+    except Exception as e:
+        logger.debug("unknown handle: {}", e)
+        return None
+
+    cd = {
+        "name": char_name,
+        "uuid": char.uuid,
+        "properties": ",".join(char.properties),
+    }
+    value = None
+    if "read" in char.properties:
+        blob = await client.read_gatt_char(char.handle)
+        if char_name == Handle.MANUFACTURER_NAME_STRING.name:
+            value = blob.decode("utf-8")
+        elif char_name == Handle.FIRMWARE_INFO.name:
+            value = FirmwareInfo(blob).to_dict()
+        elif char_name == Handle.FIRMWARE_VERSION.name:
+            value = str(FirmwareVersion(blob))
+        elif char_name == Handle.BATTERY_LEVEL.name:
+            value = ord(blob)
+        else:
+            value = binascii.b2a_hex(blob).decode("utf-8")
+
+    if value:
+        cd["value"] = value
+    return cd
```

### Comparing `dl_myo-0.1.5/myo/handle.py` & `dl_myo-0.1.6/myo/handle.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,37 +27,39 @@
     0x2A19: "BatteryLevelCharacteristic",
     0x2A00: "DeviceName",
 }
 """
 import aenum
 
 
+# fmt: off
 class Handle(aenum.Enum):
-    DEVICE_INFORMATION = 12
-    MANUFACTURER_NAME_STRING = 13
-    BATTERY_SERVICE = 15
-    BATTERY_LEVEL = 16
-    CONTROL_SERVICE = 19
-    FIRMWARE_INFO = 20
-    FIRMWARE_VERSION = 22
-    COMMAND = 24
-    IMU_SERVICE = 26
-    IMU_DATA = 27
-    MOTION_EVENT = 30
-    CLASSIFIER_SERVICE = 33
-    CLASSIFIER_EVENT = 34
-    FV_SERVICE = 37
-    FV_DATA = 38
-    EMG_SERVICE = 41
-    EMG0_DATA = 42
-    EMG1_DATA = 45
-    EMG2_DATA = 48
-    EMG3_DATA = 51
-    UNKNOWN_SERVICE = 54
-    UNKNOWN_CHAR = 55
+    DEVICE_INFORMATION = 12 # 0x0c
+    MANUFACTURER_NAME_STRING = 13  # 0x0d
+    BATTERY_SERVICE = 15    # 0x0f
+    BATTERY_LEVEL = 16      # 0x10
+    CONTROL_SERVICE = 19    # 0x13
+    FIRMWARE_INFO = 20      # 0x14
+    FIRMWARE_VERSION = 22   # 0x16
+    COMMAND = 24            # 0x18
+    IMU_SERVICE = 26        # 0x1a
+    IMU_DATA = 27           # 0x1b
+    MOTION_EVENT = 30       # 0x1e
+    CLASSIFIER_SERVICE = 33 # 0x21
+    CLASSIFIER_EVENT = 34   # 0x22
+    FV_SERVICE = 37         # 0x25: EMG Filtered Value Service
+    FV_DATA = 38            # 0x26: EMG Filtered Value Data
+    EMG_SERVICE = 41        # 0x29
+    EMG0_DATA = 42          # 0x2a
+    EMG1_DATA = 45          # 0x2d
+    EMG2_DATA = 48          # 0x30
+    EMG3_DATA = 51          # 0x33
+    UNKNOWN_SERVICE = 54    # 0x36
+    UNKNOWN_CHAR = 55       # 0x37
+# fmt: on
 
 
 class UUID:
     MYO_SERVICE = "d5060001-a904-deb9-4748-2c7f4a124842"
 
     # [Service] (Handle: 12): Device Information
     DEVICE_INFORMATION = "0000180a-0000-1000-8000-00805f9b34fb"
```

### Comparing `dl_myo-0.1.5/LICENSE` & `dl_myo-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dl_myo-0.1.5/README.md` & `dl_myo-0.1.6/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # dl-myo (Dongle-less Myo)
 
-[![Build Status](https://github.com/iomz/dl-myo/workflows/build/badge.svg)](https://github.com/iomz/dl-myo/actions?query=workflow%3Abuild)
-[![Image Size](https://ghcr-badge.egpl.dev/iomz/dl-myo/size?label=image%20size)](https://github.com/iomz/dl-myo/pkgs/container/dl-myo)
-[![Python Versions](https://img.shields.io/pypi/pyversions/dl-myo.svg)](https://pypi.python.org/pypi/dl-myo)
-[![PyPI Version](https://img.shields.io/pypi/v/dl-myo.svg)](https://pypi.python.org/pypi/del-myo)
-[![License](https://img.shields.io/pypi/l/dl-myo.svg)](https://pypi.python.org/pypi/dl-myo)
+[![build status](https://github.com/iomz/dl-myo/workflows/build/badge.svg)](https://github.com/iomz/dl-myo/actions?query=workflow%3Abuild)
+[![image size](https://ghcr-badge.egpl.dev/iomz/dl-myo/size?label=image%20size)](https://github.com/iomz/dl-myo/pkgs/container/dl-myo)
+[![codecov](https://codecov.io/gh/iomz/dl-myo/branch/main/graph/badge.svg?token=7bC3Aa1XNN)](https://codecov.io/gh/iomz/dl-myo)
+[![python Versions](https://img.shields.io/pypi/pyversions/dl-myo.svg)](https://pypi.python.org/pypi/dl-myo)
+[![pypi version](https://img.shields.io/pypi/v/dl-myo.svg)](https://pypi.python.org/pypi/dl-myo)
+[![license](https://img.shields.io/pypi/l/dl-myo.svg)](https://pypi.python.org/pypi/dl-myo)
 
 dl-myo is a replacement to MyoConnect for Myo Armband without an official Myo dongle.
 
 If you are fed up with the dongle and still need to use Myo anyway this is the right stuff to grab.
 
 This project is a reimplementation of [Dongleless-myo](https://github.com/iomz/Dongleless-myo) (originally created by [@mamo91](https://github.com/mamo91) and enhanced by [@MyrikLD](https://github.com/MyrikLD)) using [Bleak](https://github.com/hbldh/bleak) instead of [bluepy](https://github.com/IanHarvey/bluepy), and therefore supports asyncio on multiple platforms.
 
@@ -47,10 +48,17 @@
 ### Try the example with Docker
 
 ```bash
 docker compose pull
 docker compose run --rm dl-myo
 ```
 
+## Build (requires [Poetry](https://python-poetry.org/)
+
+```bash
+poetry install
+poetry build
+```
+
 ## Author
 
 [@iomz](https://github.com/iomz) (Iori Mizutani)
```

### Comparing `dl_myo-0.1.5/pyproject.toml` & `dl_myo-0.1.6/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,61 +1,36 @@
-[build-system]
-requires = ["hatchling>=1.17.1", "hatch-vcs>=0.3.0"]
-build-backend = "hatchling.build"
-
 [project]
 name = "dl-myo"
 authors = [
   { name="Iori Mizutani", email="iori.mizutani@gmail.com" },
 ]
 maintainers = [
   { name="Iori Mizutani", email="iori.mizutani@gmail.com" },
 ]
 description = "A replacement middleware to MyoConnect for Myo Armband"
 readme = "README.md"
-requires-python = ">=3.10"
-dependencies = [
-    "aenum>=3.1.12",
-    "bleak>=0.20.2",
-]
 classifiers = [
     "Environment :: Console",
     "Framework :: AsyncIO",
     "Framework :: Hatch",
     "Intended Audience :: Developers",
     "Intended Audience :: Education",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Operating System :: OS Independent",
     "Topic :: Scientific/Engineering :: Human Machine Interfaces",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
-dynamic = ["version"]
 
 [project.urls]
 "Homepage" = "https://github.com/iomz/dl-myo"
 "Bug Tracker" = "https://github.com/iomz/dl-myo/issues"
 
-[tool.hatch.version]
-source = "vcs"
-
-[tool.hatch.version.raw-options]
-version_scheme = "python-simplified-semver"
-local_scheme = "no-local-version"
-parentdir_prefix_version = "v"
-git_describe_command = ["git", "describe", "--dirty", "--tags", "--long", "--match", "v*"]
-
-[tool.hatch.build.targets.sdist]
-exclude = [
-  "/.github",
-  "/examples",
-]
-
 [tool.black]
 line-length = 120
 skip-string-normalization = true
 target-version = ["py311"]
 
 [tool.ruff]
 # Enable pycodestyle (`E`) and Pyflakes (`F`) codes by default.
@@ -92,34 +67,54 @@
 line-length = 120
 # Allow unused variables when underscore-prefixed.
 dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
 # Assume Python 3.10.
 target-version = "py311"
 
 
-[tool.ruff.isort]
-known-first-party = ["hatch", "hatchling"]
-
 [tool.ruff.mccabe]
 # Unlike Flake8, default to a complexity level of 10.
 max-complexity = 10
 
 [tool.ruff.per-file-ignores]
 # Tests can use magic values, assertions, and relative imports
 "tests/**/*" = ["PLR2004", "S101", "TID252"]
 
 [tool.coverage.run]
 branch = true
-source_pkgs = ["hatch", "hatchling", "tests"]
-omit = [
-  "myo/__init__.py",
-]
 
 [tool.coverage.paths]
-tests = ["tests", "*/myo/tests"]
+tests = ["tests"]
 
 [tool.coverage.report]
 exclude_lines = [
   "no cov",
   "if __name__ == .__main__.:",
   "if TYPE_CHECKING:",
 ]
+
+[tool.poetry]
+name = "dl-myo"
+version = "0.1.6"
+description = "A replacement middleware to MyoConnect for Myo Armband"
+authors = ["Iori Mizutani <iori.mizutani@gmail.com>"]
+license = "GPLv3"
+readme = "README.md"
+packages = [{include = "myo"}]
+
+[tool.poetry.dependencies]
+python = "^3.10"
+aenum = "^3.1.12"
+bleak = "^0.20.2"
+
+[tool.poetry.group.dev.dependencies]
+black = "^23.3.0"
+pytest = "^7.3.2"
+pytest-cov = "^4.1.0"
+
+[tool.poetry-dynamic-versioning]
+enable = false
+format = "{base}"
+
+[build-system]
+requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
+build-backend = "poetry_dynamic_versioning.backend"
```

### Comparing `dl_myo-0.1.5/PKG-INFO` & `dl_myo-0.1.6/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,40 +1,31 @@
 Metadata-Version: 2.1
 Name: dl-myo
-Version: 0.1.5
+Version: 0.1.6
 Summary: A replacement middleware to MyoConnect for Myo Armband
-Project-URL: Homepage, https://github.com/iomz/dl-myo
-Project-URL: Bug Tracker, https://github.com/iomz/dl-myo/issues
-Author-email: Iori Mizutani <iori.mizutani@gmail.com>
-Maintainer-email: Iori Mizutani <iori.mizutani@gmail.com>
-License-File: LICENSE
-Classifier: Environment :: Console
-Classifier: Framework :: AsyncIO
-Classifier: Framework :: Hatch
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3 :: Only
+License: GPLv3
+Author: Iori Mizutani
+Author-email: iori.mizutani@gmail.com
+Requires-Python: >=3.10,<4.0
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.10
-Requires-Dist: aenum>=3.1.12
-Requires-Dist: bleak>=0.20.2
+Requires-Dist: aenum (>=3.1.12,<4.0.0)
+Requires-Dist: bleak (>=0.20.2,<0.21.0)
 Description-Content-Type: text/markdown
 
 # dl-myo (Dongle-less Myo)
 
-[![Build Status](https://github.com/iomz/dl-myo/workflows/build/badge.svg)](https://github.com/iomz/dl-myo/actions?query=workflow%3Abuild)
-[![Image Size](https://ghcr-badge.egpl.dev/iomz/dl-myo/size?label=image%20size)](https://github.com/iomz/dl-myo/pkgs/container/dl-myo)
-[![Python Versions](https://img.shields.io/pypi/pyversions/dl-myo.svg)](https://pypi.python.org/pypi/dl-myo)
-[![PyPI Version](https://img.shields.io/pypi/v/dl-myo.svg)](https://pypi.python.org/pypi/del-myo)
-[![License](https://img.shields.io/pypi/l/dl-myo.svg)](https://pypi.python.org/pypi/dl-myo)
+[![build status](https://github.com/iomz/dl-myo/workflows/build/badge.svg)](https://github.com/iomz/dl-myo/actions?query=workflow%3Abuild)
+[![image size](https://ghcr-badge.egpl.dev/iomz/dl-myo/size?label=image%20size)](https://github.com/iomz/dl-myo/pkgs/container/dl-myo)
+[![codecov](https://codecov.io/gh/iomz/dl-myo/branch/main/graph/badge.svg?token=7bC3Aa1XNN)](https://codecov.io/gh/iomz/dl-myo)
+[![python Versions](https://img.shields.io/pypi/pyversions/dl-myo.svg)](https://pypi.python.org/pypi/dl-myo)
+[![pypi version](https://img.shields.io/pypi/v/dl-myo.svg)](https://pypi.python.org/pypi/dl-myo)
+[![license](https://img.shields.io/pypi/l/dl-myo.svg)](https://pypi.python.org/pypi/dl-myo)
 
 dl-myo is a replacement to MyoConnect for Myo Armband without an official Myo dongle.
 
 If you are fed up with the dongle and still need to use Myo anyway this is the right stuff to grab.
 
 This project is a reimplementation of [Dongleless-myo](https://github.com/iomz/Dongleless-myo) (originally created by [@mamo91](https://github.com/mamo91) and enhanced by [@MyrikLD](https://github.com/MyrikLD)) using [Bleak](https://github.com/hbldh/bleak) instead of [bluepy](https://github.com/IanHarvey/bluepy), and therefore supports asyncio on multiple platforms.
 
@@ -73,10 +64,18 @@
 ### Try the example with Docker
 
 ```bash
 docker compose pull
 docker compose run --rm dl-myo
 ```
 
+## Build (requires [Poetry](https://python-poetry.org/)
+
+```bash
+poetry install
+poetry build
+```
+
 ## Author
 
 [@iomz](https://github.com/iomz) (Iori Mizutani)
+
```

