# Comparing `tmp/pictorus-0.0.6.tar.gz` & `tmp/pictorus-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pictorus-0.0.6.tar", last modified: Tue Jun  6 15:53:49 2023, max compression
+gzip compressed data, was "pictorus-0.0.7.tar", last modified: Tue Jun 13 16:19:32 2023, max compression
```

## Comparing `pictorus-0.0.6.tar` & `pictorus-0.0.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      554 2023-04-18 22:31:36.961706 pictorus-0.0.6/.github/workflows/test.yaml
--rw-r--r--   0        0        0      918 2023-02-14 23:52:57.501277 pictorus-0.0.6/.gitignore
--rw-r--r--   0        0        0        6 2023-02-15 19:48:07.053003 pictorus-0.0.6/.python-version
--rw-r--r--   0        0        0    32422 2023-02-15 19:48:07.053335 pictorus-0.0.6/LICENSE
--rw-r--r--   0        0        0      737 2023-02-16 17:48:01.977637 pictorus-0.0.6/PUB_README.md
--rw-r--r--   0        0        0     1433 2023-03-30 22:18:14.564827 pictorus-0.0.6/README.md
--rw-r--r--   0        0        0      828 2023-05-19 20:34:53.614814 pictorus-0.0.6/pyproject.toml
--rwxr-xr-x   0        0        0      340 2023-02-15 19:48:07.054532 pictorus-0.0.6/script/setup
--rw-r--r--   0        0        0       61 2023-06-06 15:53:17.152203 pictorus-0.0.6/src/pictorus/__init__.py
--rw-r--r--   0        0        0    14247 2023-05-19 20:28:20.661444 pictorus-0.0.6/src/pictorus/app_manager.py
--rw-r--r--   0        0        0     3147 2023-06-06 15:52:56.896505 pictorus-0.0.6/src/pictorus/config.py
--rw-r--r--   0        0        0      492 2023-05-09 19:07:56.162364 pictorus-0.0.6/src/pictorus/constants.py
--rw-r--r--   0        0        0      244 2023-02-15 19:48:07.055277 pictorus-0.0.6/src/pictorus/logging.py
--rw-r--r--   0        0        0     4054 2023-05-19 20:28:20.662559 pictorus-0.0.6/src/pictorus/pictorus_cli.py
--rwxr-xr-x   0        0        0     2390 2023-05-19 20:28:20.663228 pictorus-0.0.6/src/pictorus/pictorus_device_manager.py
--rw-r--r--   0        0        0     1476 2023-02-16 17:48:01.978870 pictorus-0.0.6/src/pictorus/systemd.py
--rw-r--r--   0        0        0     4878 2023-05-09 19:07:56.163315 pictorus-0.0.6/src/pictorus/telemetry_manager.py
--rw-r--r--   0        0        0     3316 2023-05-19 20:34:53.615084 pictorus-0.0.6/src/pictorus/version_manager.py
--rw-r--r--   0        0        0     9002 2023-05-09 19:07:56.163796 pictorus-0.0.6/tests/pictorus/test_app_manager.py
--rw-r--r--   0        0        0     2389 2023-05-19 20:34:53.615288 pictorus-0.0.6/tests/pictorus/test_version_manager.py
--rw-r--r--   0        0        0     1345 1970-01-01 00:00:00.000000 pictorus-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      554 2023-04-18 22:31:36.961706 pictorus-0.0.7/.github/workflows/test.yaml
+-rw-r--r--   0        0        0      918 2023-02-14 23:52:57.501277 pictorus-0.0.7/.gitignore
+-rw-r--r--   0        0        0        6 2023-02-15 19:48:07.053003 pictorus-0.0.7/.python-version
+-rw-r--r--   0        0        0    32422 2023-02-15 19:48:07.053335 pictorus-0.0.7/LICENSE
+-rw-r--r--   0        0        0      737 2023-02-16 17:48:01.977637 pictorus-0.0.7/PUB_README.md
+-rw-r--r--   0        0        0     1433 2023-03-30 22:18:14.564827 pictorus-0.0.7/README.md
+-rw-r--r--   0        0        0      828 2023-05-19 20:34:53.614814 pictorus-0.0.7/pyproject.toml
+-rwxr-xr-x   0        0        0      340 2023-02-15 19:48:07.054532 pictorus-0.0.7/script/setup
+-rw-r--r--   0        0        0       61 2023-06-13 16:18:46.133398 pictorus-0.0.7/src/pictorus/__init__.py
+-rw-r--r--   0        0        0    14247 2023-05-19 20:28:20.661444 pictorus-0.0.7/src/pictorus/app_manager.py
+-rw-r--r--   0        0        0     3147 2023-06-06 15:52:56.896505 pictorus-0.0.7/src/pictorus/config.py
+-rw-r--r--   0        0        0      492 2023-05-09 19:07:56.162364 pictorus-0.0.7/src/pictorus/constants.py
+-rw-r--r--   0        0        0      244 2023-02-15 19:48:07.055277 pictorus-0.0.7/src/pictorus/logging.py
+-rw-r--r--   0        0        0     5040 2023-06-13 16:18:36.750543 pictorus-0.0.7/src/pictorus/pictorus_cli.py
+-rwxr-xr-x   0        0        0     2390 2023-05-19 20:28:20.663228 pictorus-0.0.7/src/pictorus/pictorus_device_manager.py
+-rw-r--r--   0        0        0     1476 2023-02-16 17:48:01.978870 pictorus-0.0.7/src/pictorus/systemd.py
+-rw-r--r--   0        0        0     4878 2023-05-09 19:07:56.163315 pictorus-0.0.7/src/pictorus/telemetry_manager.py
+-rw-r--r--   0        0        0     3316 2023-05-19 20:34:53.615084 pictorus-0.0.7/src/pictorus/version_manager.py
+-rw-r--r--   0        0        0     9002 2023-05-09 19:07:56.163796 pictorus-0.0.7/tests/pictorus/test_app_manager.py
+-rw-r--r--   0        0        0     2389 2023-05-19 20:34:53.615288 pictorus-0.0.7/tests/pictorus/test_version_manager.py
+-rw-r--r--   0        0        0     1345 1970-01-01 00:00:00.000000 pictorus-0.0.7/PKG-INFO
```

### Comparing `pictorus-0.0.6/.github/workflows/test.yaml` & `pictorus-0.0.7/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `pictorus-0.0.6/.gitignore` & `pictorus-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `pictorus-0.0.6/LICENSE` & `pictorus-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pictorus-0.0.6/PUB_README.md` & `pictorus-0.0.7/PUB_README.md`

 * *Files identical despite different names*

### Comparing `pictorus-0.0.6/README.md` & `pictorus-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `pictorus-0.0.6/pyproject.toml` & `pictorus-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pictorus-0.0.6/src/pictorus/app_manager.py` & `pictorus-0.0.7/src/pictorus/app_manager.py`

 * *Files identical despite different names*

### Comparing `pictorus-0.0.6/src/pictorus/config.py` & `pictorus-0.0.7/src/pictorus/config.py`

 * *Files identical despite different names*

### Comparing `pictorus-0.0.6/src/pictorus/pictorus_cli.py` & `pictorus-0.0.7/src/pictorus/pictorus_cli.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,39 +6,48 @@
 import platform
 import socket
 import sys
 from urllib.parse import urljoin
 import shutil
 import os
 from enum import Enum
+import json
+from typing import Tuple
 
 import requests
 
 from pictorus.config import API_PREFIX, Config
 from pictorus.constants import PICTORUS_SERVICE_NAME
 from pictorus.systemd import create_service, SYSTEMD_DIR
 
 config = Config()
 
+DEFAULT_AUTH_ERROR = "Unable to authenticate with pictorus"
+
 
 class TextFormat(Enum):
     OKCYAN = "\033[96m"
     OKGREEN = "\033[92m"
     WARNING = "\033[93m"
     FAIL = "\033[91m"
     ENDC = "\033[0m"
 
 
 def printf(message: str, fmt: TextFormat):
     print(f"{fmt.value}{message}{TextFormat.ENDC.value}")
 
 
-def get_credentials():
+def get_credentials(username: str = None):
     """Prompt user for username and password"""
-    username = input("Enter username for pictorus: ")
+    username_prompt = (
+        f"Enter username for pictorus [{username}]: "
+        if username
+        else "Enter username for pictorus: "
+    )
+    username = input(username_prompt) or username
     passwd = getpass("Enter password for pictorus: ")
     return username, passwd
 
 
 def prompt_auto_update() -> bool:
     """Prompt the user to ask if they want to update automatically"""
     auto_update = input("Would you like to update pictorus automatically on this device [Y/n]? ")
@@ -86,47 +95,71 @@
         PICTORUS_SERVICE_NAME,
         "Service to manage Pictorus apps",
         bin_path,
     )
     printf("Configured device manager service", TextFormat.OKGREEN)
 
 
+def try_device_configuration(
+    device_name: str, system_data: dict, credentials: Tuple[str, str]
+) -> bool:
+    """Try to configure the device"""
+    session = requests.Session()
+    session.auth = credentials
+
+    res = session.post(
+        urljoin(API_PREFIX, "v2/devices"),
+        json={
+            "name": device_name,
+            "system": system_data,
+        },
+    )
+
+    if not res.ok:
+        try:
+            message = res.json().get("message", DEFAULT_AUTH_ERROR)
+        except json.JSONDecodeError:
+            message = DEFAULT_AUTH_ERROR
+
+        printf(f"Failed to configure device: {message}", TextFormat.FAIL)
+        return False
+
+    config.store_config(res.json())
+    return True
+
+
 def configure_device():
     """Configure this device to connect to pictorus"""
     print("Configuring new device")
     if not config.is_empty():
         confirm = input(
             "It looks like this device is already configured. Would you like to overwrite it [y/N]? "
         )
         if confirm.lower() != "y":
             printf("Skipping device registration", TextFormat.OKCYAN)
             return
 
-    session = requests.Session()
-    session.auth = get_credentials()
-
     hostname = socket.gethostname()
     device_name = input(f"Device Name [{hostname}]: ")
     device_name = device_name or hostname
 
     system_data = {
         "platform": platform.platform(),
         "system": platform.system(),
         "machine": platform.machine(),
     }
 
-    res = session.post(
-        urljoin(API_PREFIX, "v2/devices"),
-        json={
-            "name": device_name,
-            "system": system_data,
-        },
-    )
-    res.raise_for_status()
-    config.store_config(res.json())
+    configured = False
+    username = None
+    while not configured:
+        credentials = get_credentials(username)
+        # Cache the username so user doesn't have to input again on failure
+        username = credentials[0]
+        configured = try_device_configuration(device_name, system_data, credentials)
+
     printf(f"Successfully configured device: {device_name}", TextFormat.OKGREEN)
 
 
 def main():
     """Main CLI entry point"""
     parser = argparse.ArgumentParser(description="Pictorus device manager")
     subparsers = parser.add_subparsers()
```

### Comparing `pictorus-0.0.6/src/pictorus/pictorus_device_manager.py` & `pictorus-0.0.7/src/pictorus/pictorus_device_manager.py`

 * *Files identical despite different names*

### Comparing `pictorus-0.0.6/src/pictorus/systemd.py` & `pictorus-0.0.7/src/pictorus/systemd.py`

 * *Files identical despite different names*

### Comparing `pictorus-0.0.6/src/pictorus/telemetry_manager.py` & `pictorus-0.0.7/src/pictorus/telemetry_manager.py`

 * *Files identical despite different names*

### Comparing `pictorus-0.0.6/src/pictorus/version_manager.py` & `pictorus-0.0.7/src/pictorus/version_manager.py`

 * *Files identical despite different names*

### Comparing `pictorus-0.0.6/tests/pictorus/test_app_manager.py` & `pictorus-0.0.7/tests/pictorus/test_app_manager.py`

 * *Files identical despite different names*

### Comparing `pictorus-0.0.6/tests/pictorus/test_version_manager.py` & `pictorus-0.0.7/tests/pictorus/test_version_manager.py`

 * *Files identical despite different names*

### Comparing `pictorus-0.0.6/PKG-INFO` & `pictorus-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pictorus
-Version: 0.0.6
+Version: 0.0.7
 Summary: Pictorus device manager package
 Author-email: Pictorus Inc <contact@pictor.us>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Dist: awsiotsdk~=1.11.5
 Requires-Dist: requests~=2.26.0
```

