# Comparing `tmp/algokit-1.1.0-py3-none-any.whl.zip` & `tmp/algokit-1.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 43198 bytes, number of entries: 31
+Zip file size: 43495 bytes, number of entries: 31
 -rw-r--r--  2.0 unx     1168 b- defN 80-Jan-01 00:00 algokit/__init__.py
 -rw-r--r--  2.0 unx       43 b- defN 80-Jan-01 00:00 algokit/__main__.py
 -rw-r--r--  2.0 unx     1511 b- defN 80-Jan-01 00:00 algokit/cli/__init__.py
 -rw-r--r--  2.0 unx     1778 b- defN 80-Jan-01 00:00 algokit/cli/bootstrap.py
 -rw-r--r--  2.0 unx     6065 b- defN 80-Jan-01 00:00 algokit/cli/completions.py
 -rw-r--r--  2.0 unx      296 b- defN 80-Jan-01 00:00 algokit/cli/config.py
 -rw-r--r--  2.0 unx     5802 b- defN 80-Jan-01 00:00 algokit/cli/doctor.py
@@ -16,18 +16,18 @@
 -rw-r--r--  2.0 unx    10801 b- defN 80-Jan-01 00:00 algokit/core/bootstrap.py
 -rw-r--r--  2.0 unx     1380 b- defN 80-Jan-01 00:00 algokit/core/conf.py
 -rw-r--r--  2.0 unx     4711 b- defN 80-Jan-01 00:00 algokit/core/doctor.py
 -rw-r--r--  2.0 unx     1159 b- defN 80-Jan-01 00:00 algokit/core/init.py
 -rw-r--r--  2.0 unx     5128 b- defN 80-Jan-01 00:00 algokit/core/log_handlers.py
 -rw-r--r--  2.0 unx     3520 b- defN 80-Jan-01 00:00 algokit/core/proc.py
 -rw-r--r--  2.0 unx     1970 b- defN 80-Jan-01 00:00 algokit/core/questionary_extensions.py
--rw-r--r--  2.0 unx     9294 b- defN 80-Jan-01 00:00 algokit/core/sandbox.py
+-rw-r--r--  2.0 unx    10420 b- defN 80-Jan-01 00:00 algokit/core/sandbox.py
 -rw-r--r--  2.0 unx     4025 b- defN 80-Jan-01 00:00 algokit/core/typed_client_generation.py
 -rw-r--r--  2.0 unx      508 b- defN 80-Jan-01 00:00 algokit/core/utils.py
 -rw-r--r--  2.0 unx     4174 b- defN 80-Jan-01 00:00 algokit/core/version_prompt.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 algokit/py.typed
--rw-r--r--  2.0 unx     1081 b- defN 80-Jan-01 00:00 algokit-1.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx    13733 b- defN 80-Jan-01 00:00 algokit-1.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 algokit-1.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       47 b- defN 80-Jan-01 00:00 algokit-1.1.0.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     2477 b- defN 16-Jan-01 00:00 algokit-1.1.0.dist-info/RECORD
-31 files, 114454 bytes uncompressed, 39270 bytes compressed:  65.7%
+-rw-r--r--  2.0 unx     1081 b- defN 80-Jan-01 00:00 algokit-1.1.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx    13733 b- defN 80-Jan-01 00:00 algokit-1.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 algokit-1.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       47 b- defN 80-Jan-01 00:00 algokit-1.1.1.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     2478 b- defN 16-Jan-01 00:00 algokit-1.1.1.dist-info/RECORD
+31 files, 115581 bytes uncompressed, 39567 bytes compressed:  65.8%
```

## zipnote {}

```diff
@@ -72,23 +72,23 @@
 
 Filename: algokit/core/version_prompt.py
 Comment: 
 
 Filename: algokit/py.typed
 Comment: 
 
-Filename: algokit-1.1.0.dist-info/LICENSE
+Filename: algokit-1.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: algokit-1.1.0.dist-info/METADATA
+Filename: algokit-1.1.1.dist-info/METADATA
 Comment: 
 
-Filename: algokit-1.1.0.dist-info/WHEEL
+Filename: algokit-1.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: algokit-1.1.0.dist-info/entry_points.txt
+Filename: algokit-1.1.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: algokit-1.1.0.dist-info/RECORD
+Filename: algokit-1.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## algokit/core/sandbox.py

```diff
@@ -1,10 +1,11 @@
 import enum
 import json
 import logging
+import time
 from pathlib import Path
 from typing import Any, cast
 
 import httpx
 
 from algokit.core.conf import get_app_config_dir
 from algokit.core.proc import RunResult, run, run_interactive
@@ -72,15 +73,19 @@
         )
 
     def up(self) -> None:
         logger.info("Starting AlgoKit LocalNet now...")
         self._run_compose_command(
             "up --detach --quiet-pull --wait", bad_return_code_error_message="Failed to start LocalNet"
         )
-        logger.info("Started; execute `algokit explore` to explore LocalNet in a web user interface.")
+        logger.debug("AlgoKit LocalNet started, waiting for health check")
+        if _wait_for_algod():
+            logger.info("Started; execute `algokit explore` to explore LocalNet in a web user interface.")
+        else:
+            logger.warning("AlgoKit LocalNet failed to return a successful health check")
 
     def stop(self) -> None:
         logger.info("Stopping AlgoKit LocalNet now...")
         self._run_compose_command("stop", bad_return_code_error_message="Failed to stop LocalNet")
         logger.info("Sandbox Stopped; execute `algokit localnet start` to start it again.")
 
     def down(self) -> None:
@@ -116,14 +121,36 @@
         return cast(list[dict[str, Any]], data)
 
 
 DEFAULT_ALGOD_SERVER = "http://localhost"
 DEFAULT_ALGOD_TOKEN = "a" * 64
 DEFAULT_ALGOD_PORT = 4001
 DEFAULT_INDEXER_PORT = 8980
+DEFAULT_WAIT_FOR_ALGOD = 30
+DEFAULT_HEALTH_TIMEOUT = 1
+ALGOD_HEALTH_URL = f"{DEFAULT_ALGOD_SERVER}:{DEFAULT_ALGOD_PORT}/health"
+
+
+def _wait_for_algod() -> bool:
+    end_time = time.time() + DEFAULT_WAIT_FOR_ALGOD
+    last_exception: httpx.RequestError | None = None
+    while time.time() < end_time:
+        try:
+            health = httpx.get(ALGOD_HEALTH_URL, timeout=DEFAULT_HEALTH_TIMEOUT)
+        except httpx.RequestError as ex:
+            last_exception = ex
+        else:
+            if health.is_success:
+                logger.debug("AlgoKit LocalNet health check successful, algod is ready")
+                return True
+            logger.debug(f"AlgoKit LocalNet health check returned {health.status_code}, waiting")
+        time.sleep(DEFAULT_HEALTH_TIMEOUT)
+    if last_exception:
+        logger.debug("AlgoKit LocalNet health request failed", exc_info=last_exception)
+    return False
 
 
 def get_config_json() -> str:
     return (
         '{ "Version": 12, "GossipFanout": 1, "EndpointAddress": "0.0.0.0:8080", "DNSBootstrapID": "",'
         ' "IncomingConnectionsLimit": 0, "Archival":false, "isIndexerActive":false, "EnableDeveloperAPI":true}"'
     )
```

## Comparing `algokit-1.1.0.dist-info/LICENSE` & `algokit-1.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `algokit-1.1.0.dist-info/METADATA` & `algokit-1.1.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: algokit
-Version: 1.1.0
+Version: 1.1.1
 Summary: Algorand development kit command-line interface
 License: MIT
 Author: Algorand Foundation
 Author-email: contact@algorand.foundation
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

## Comparing `algokit-1.1.0.dist-info/RECORD` & `algokit-1.1.1.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 algokit/core/bootstrap.py,sha256=HQxSNCoNhD8wQAcdUPrO6vG8nZjGziZ7TDUYlf7eZ8U,10801
 algokit/core/conf.py,sha256=oWSlSAvTUviSK_AdS-H_G6DMqVOvBe_jCC-vJfgrkBI,1380
 algokit/core/doctor.py,sha256=I2BKoupBPot26Y-4OTMFJp0mATLfp9Nlz8XXv1N7i8Y,4711
 algokit/core/init.py,sha256=7y_EwVtuMfqZG_CGDR08K0f2SOOeFq6y1d8ihZgG3Uo,1159
 algokit/core/log_handlers.py,sha256=IT9mo8NhiLl2rzH6t6F9kEflmmFbOfOhKaPzRp7CVTM,5128
 algokit/core/proc.py,sha256=aJ3BGyXmI0oguOE1WbAyirCW2_IIBYuPOFutCX7cXnE,3520
 algokit/core/questionary_extensions.py,sha256=QvUGXL_GxcPvdGemy_5-Fza4d1PSJ2ml7aZAS3r4M20,1970
-algokit/core/sandbox.py,sha256=w4Q6AKP6fp8l1UiMOuZVxtU0c32eZtbu9BiHRe0mPww,9294
+algokit/core/sandbox.py,sha256=isOHDCO805_m3FoPBYHjK_1SIFN0flYWhCoeI72M8lw,10420
 algokit/core/typed_client_generation.py,sha256=ITKs3FyJT_XMln9ssPkyBFtJ66favkgYu0zY_cBGqSg,4025
 algokit/core/utils.py,sha256=hgemlB8znOsGCO090BQOydnbq4ZRAsD9CzMbApEMGY8,508
 algokit/core/version_prompt.py,sha256=yf63811ilKPoJfusxKBmxoZetrCKMKvGoSODI1-kaek,4174
 algokit/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-algokit-1.1.0.dist-info/LICENSE,sha256=CPjn5HTZL3VUJ8E1lxtdBx6SLzNnQlOoezdFYom9R24,1081
-algokit-1.1.0.dist-info/METADATA,sha256=Nb-l9F6NuOut5VZn6ZoyBgoLMvzsz0nRJVOX21EX2Tg,13733
-algokit-1.1.0.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
-algokit-1.1.0.dist-info/entry_points.txt,sha256=JJtH-iaVJa6YUrN69B7AMycsg9-q6OwV52olGIU65rc,47
-algokit-1.1.0.dist-info/RECORD,,
+algokit-1.1.1.dist-info/LICENSE,sha256=CPjn5HTZL3VUJ8E1lxtdBx6SLzNnQlOoezdFYom9R24,1081
+algokit-1.1.1.dist-info/METADATA,sha256=MSfb7zDNCJgzEtsgVxPfyizl0Zu5HQUp_DjFVi7jHfw,13733
+algokit-1.1.1.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
+algokit-1.1.1.dist-info/entry_points.txt,sha256=JJtH-iaVJa6YUrN69B7AMycsg9-q6OwV52olGIU65rc,47
+algokit-1.1.1.dist-info/RECORD,,
```

