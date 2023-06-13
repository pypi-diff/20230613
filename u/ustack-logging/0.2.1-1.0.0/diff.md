# Comparing `tmp/ustack-logging-0.2.1.tar.gz` & `tmp/ustack_logging-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ustack-logging-0.2.1.tar", last modified: Thu Apr  6 14:12:48 2017, max compression
+gzip compressed data, was "ustack_logging-1.0.0.tar", max compression
```

## Comparing `ustack-logging-0.2.1.tar` & `ustack_logging-1.0.0.tar`

### file list

```diff
@@ -1,13 +1,6 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2017-04-06 14:12:48.000000 ustack-logging-0.2.1/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2017-04-06 14:12:48.000000 ustack-logging-0.2.1/ustack_logging/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2017-04-06 14:11:10.000000 ustack-logging-0.2.1/ustack_logging/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1267 2017-04-06 14:11:10.000000 ustack-logging-0.2.1/ustack_logging/logging_configuration.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2017-04-06 14:12:48.000000 ustack-logging-0.2.1/ustack_logging.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      282 2017-04-06 14:12:48.000000 ustack-logging-0.2.1/ustack_logging.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      264 2017-04-06 14:12:48.000000 ustack-logging-0.2.1/ustack_logging.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2017-04-06 14:12:48.000000 ustack-logging-0.2.1/ustack_logging.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       34 2017-04-06 14:12:48.000000 ustack-logging-0.2.1/ustack_logging.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       15 2017-04-06 14:12:48.000000 ustack-logging-0.2.1/ustack_logging.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      447 2017-04-06 14:11:10.000000 ustack-logging-0.2.1/setup.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      282 2017-04-06 14:12:48.000000 ustack-logging-0.2.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2017-04-06 14:12:48.000000 ustack-logging-0.2.1/setup.cfg
+-rw-r--r--   0        0        0     1601 2023-06-13 14:24:11.409247 ustack_logging-1.0.0/README.md
+-rw-r--r--   0        0        0      558 2023-06-13 14:24:11.409247 ustack_logging-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-13 14:24:11.409247 ustack_logging-1.0.0/ustack_logging/__init__.py
+-rw-r--r--   0        0        0     1310 2023-06-13 14:24:11.409247 ustack_logging-1.0.0/ustack_logging/logging_configuration.py
+-rw-r--r--   0        0        0        0 2023-06-13 14:24:11.409247 ustack_logging-1.0.0/ustack_logging/py.typed
+-rw-r--r--   0        0        0     2261 1970-01-01 00:00:00.000000 ustack_logging-1.0.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ustack-logging-0.2.1/ustack_logging/logging_configuration.py` & `ustack_logging-1.0.0/ustack_logging/logging_configuration.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import base64
 import datadog
 from datadog_logger import log_error_events
 import kubernetes.client
+import kubernetes.config
 import logging
 import socket
 
 
-def configure_logging():
+def configure_logging() -> None:
     logging.basicConfig(
         format="%(asctime)s %(levelname)s:%(module)s:%(message)s",
         datefmt="%Y-%m-%d %H:%M:%S%z", level=logging.INFO)
 
     try:
         kubernetes.config.load_incluster_config()
 
@@ -29,9 +30,9 @@
 
         log_error_events(tags=[
             "environment:{0}".format(
                 base64.b64decode(environment_info.data["environment"]).decode("utf8")),
             "service:{0}".format(namespace),
             "role:{0}".format(pod_info.metadata.labels["role"])
         ])
-    except:
+    except Exception:
         logging.warning("Could not initialize DataDog error logging, with error:", exc_info=True)
```

