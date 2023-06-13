# Comparing `tmp/robomotion-1.7.4rc0.tar.gz` & `tmp/robomotion-1.7.5rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robomotion-1.7.4rc0.tar", last modified: Tue Jun 13 10:30:16 2023, max compression
+gzip compressed data, was "robomotion-1.7.5rc0.tar", last modified: Tue Jun 13 14:58:16 2023, max compression
```

## Comparing `robomotion-1.7.4rc0.tar` & `robomotion-1.7.5rc0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 hasan     (1000) hasan     (1000)        0 2023-06-13 10:30:16.584328 robomotion-1.7.4rc0/
--rw-rw-r--   0 hasan     (1000) hasan     (1000)      513 2023-06-13 10:30:16.584328 robomotion-1.7.4rc0/PKG-INFO
-drwxrwxr-x   0 hasan     (1000) hasan     (1000)        0 2023-06-13 10:30:16.584328 robomotion-1.7.4rc0/robomotion/
--rw-rw-r--   0 hasan     (1000) hasan     (1000)        0 2022-08-24 12:32:15.000000 robomotion-1.7.4rc0/robomotion/__init__.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)     3855 2023-06-08 09:30:16.000000 robomotion-1.7.4rc0/robomotion/debug.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)      660 2023-05-10 13:07:28.000000 robomotion-1.7.4rc0/robomotion/decorators.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)      338 2023-06-08 09:30:16.000000 robomotion-1.7.4rc0/robomotion/error.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)     1877 2023-06-08 09:30:16.000000 robomotion-1.7.4rc0/robomotion/event.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)      264 2022-08-24 12:32:15.000000 robomotion-1.7.4rc0/robomotion/factory.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)      800 2022-08-24 12:32:15.000000 robomotion-1.7.4rc0/robomotion/health.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)     1601 2023-06-08 09:30:16.000000 robomotion-1.7.4rc0/robomotion/health_pb2.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)     2457 2023-06-08 09:30:16.000000 robomotion-1.7.4rc0/robomotion/health_pb2_grpc.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)  1674682 2023-06-08 09:30:16.000000 robomotion-1.7.4rc0/robomotion/icons.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)     1183 2023-06-08 09:30:16.000000 robomotion-1.7.4rc0/robomotion/message.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)     3392 2022-09-21 11:29:46.000000 robomotion-1.7.4rc0/robomotion/node.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)     2116 2022-08-24 12:32:15.000000 robomotion-1.7.4rc0/robomotion/plugin.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)     7359 2023-06-13 10:29:47.000000 robomotion-1.7.4rc0/robomotion/plugin_pb2.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)    27555 2023-06-13 10:13:54.000000 robomotion-1.7.4rc0/robomotion/plugin_pb2_grpc.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)     2735 2023-06-08 09:30:16.000000 robomotion-1.7.4rc0/robomotion/runner_pb2.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)    11076 2023-06-08 09:30:16.000000 robomotion-1.7.4rc0/robomotion/runner_pb2_grpc.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)     4525 2023-06-13 09:47:09.000000 robomotion-1.7.4rc0/robomotion/runtime.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)    21852 2023-06-13 09:47:09.000000 robomotion-1.7.4rc0/robomotion/spec.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)     2436 2023-06-08 09:30:16.000000 robomotion-1.7.4rc0/robomotion/struct_pb2.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)      159 2023-06-08 09:30:16.000000 robomotion-1.7.4rc0/robomotion/struct_pb2_grpc.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)      507 2023-06-08 09:30:16.000000 robomotion-1.7.4rc0/robomotion/utils.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)     7035 2023-06-13 09:47:09.000000 robomotion-1.7.4rc0/robomotion/variable.py
-drwxrwxr-x   0 hasan     (1000) hasan     (1000)        0 2023-06-13 10:30:16.584328 robomotion-1.7.4rc0/robomotion.egg-info/
--rw-rw-r--   0 hasan     (1000) hasan     (1000)      513 2023-06-13 10:30:16.000000 robomotion-1.7.4rc0/robomotion.egg-info/PKG-INFO
--rw-rw-r--   0 hasan     (1000) hasan     (1000)      747 2023-06-13 10:30:16.000000 robomotion-1.7.4rc0/robomotion.egg-info/SOURCES.txt
--rw-rw-r--   0 hasan     (1000) hasan     (1000)        1 2023-06-13 10:30:16.000000 robomotion-1.7.4rc0/robomotion.egg-info/dependency_links.txt
--rw-rw-r--   0 hasan     (1000) hasan     (1000)        1 2023-06-13 10:30:16.000000 robomotion-1.7.4rc0/robomotion.egg-info/not-zip-safe
--rw-rw-r--   0 hasan     (1000) hasan     (1000)      100 2023-06-13 10:30:16.000000 robomotion-1.7.4rc0/robomotion.egg-info/requires.txt
--rw-rw-r--   0 hasan     (1000) hasan     (1000)       11 2023-06-13 10:30:16.000000 robomotion-1.7.4rc0/robomotion.egg-info/top_level.txt
--rw-rw-r--   0 hasan     (1000) hasan     (1000)       38 2023-06-13 10:30:16.584328 robomotion-1.7.4rc0/setup.cfg
--rw-rw-r--   0 hasan     (1000) hasan     (1000)     1423 2023-06-13 10:30:06.000000 robomotion-1.7.4rc0/setup.py
+drwxrwxr-x   0 hasan     (1000) hasan     (1000)        0 2023-06-13 14:58:16.375707 robomotion-1.7.5rc0/
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)      513 2023-06-13 14:58:16.375707 robomotion-1.7.5rc0/PKG-INFO
+drwxrwxr-x   0 hasan     (1000) hasan     (1000)        0 2023-06-13 14:58:16.371707 robomotion-1.7.5rc0/robomotion/
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)        0 2022-08-24 12:32:15.000000 robomotion-1.7.5rc0/robomotion/__init__.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)     3855 2023-06-08 09:30:16.000000 robomotion-1.7.5rc0/robomotion/debug.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)      660 2023-05-10 13:07:28.000000 robomotion-1.7.5rc0/robomotion/decorators.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)      338 2023-06-08 09:30:16.000000 robomotion-1.7.5rc0/robomotion/error.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)     1868 2023-06-13 14:57:51.000000 robomotion-1.7.5rc0/robomotion/event.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)      264 2022-08-24 12:32:15.000000 robomotion-1.7.5rc0/robomotion/factory.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)      800 2022-08-24 12:32:15.000000 robomotion-1.7.5rc0/robomotion/health.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)     1601 2023-06-08 09:30:16.000000 robomotion-1.7.5rc0/robomotion/health_pb2.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)     2457 2023-06-08 09:30:16.000000 robomotion-1.7.5rc0/robomotion/health_pb2_grpc.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)  1674682 2023-06-08 09:30:16.000000 robomotion-1.7.5rc0/robomotion/icons.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)     1183 2023-06-08 09:30:16.000000 robomotion-1.7.5rc0/robomotion/message.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)     3392 2022-09-21 11:29:46.000000 robomotion-1.7.5rc0/robomotion/node.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)     2116 2022-08-24 12:32:15.000000 robomotion-1.7.5rc0/robomotion/plugin.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)     7359 2023-06-13 14:54:50.000000 robomotion-1.7.5rc0/robomotion/plugin_pb2.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)    27555 2023-06-13 14:54:50.000000 robomotion-1.7.5rc0/robomotion/plugin_pb2_grpc.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)     2735 2023-06-08 09:30:16.000000 robomotion-1.7.5rc0/robomotion/runner_pb2.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)    11076 2023-06-08 09:30:16.000000 robomotion-1.7.5rc0/robomotion/runner_pb2_grpc.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)     4525 2023-06-13 09:47:09.000000 robomotion-1.7.5rc0/robomotion/runtime.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)    21852 2023-06-13 09:47:09.000000 robomotion-1.7.5rc0/robomotion/spec.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)     2436 2023-06-08 09:30:16.000000 robomotion-1.7.5rc0/robomotion/struct_pb2.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)      159 2023-06-08 09:30:16.000000 robomotion-1.7.5rc0/robomotion/struct_pb2_grpc.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)      507 2023-06-08 09:30:16.000000 robomotion-1.7.5rc0/robomotion/utils.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)     7035 2023-06-13 09:47:09.000000 robomotion-1.7.5rc0/robomotion/variable.py
+drwxrwxr-x   0 hasan     (1000) hasan     (1000)        0 2023-06-13 14:58:16.371707 robomotion-1.7.5rc0/robomotion.egg-info/
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)      513 2023-06-13 14:58:16.000000 robomotion-1.7.5rc0/robomotion.egg-info/PKG-INFO
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)      747 2023-06-13 14:58:16.000000 robomotion-1.7.5rc0/robomotion.egg-info/SOURCES.txt
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)        1 2023-06-13 14:58:16.000000 robomotion-1.7.5rc0/robomotion.egg-info/dependency_links.txt
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)        1 2023-06-13 14:58:16.000000 robomotion-1.7.5rc0/robomotion.egg-info/not-zip-safe
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)       84 2023-06-13 14:58:16.000000 robomotion-1.7.5rc0/robomotion.egg-info/requires.txt
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)       11 2023-06-13 14:58:16.000000 robomotion-1.7.5rc0/robomotion.egg-info/top_level.txt
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)       38 2023-06-13 14:58:16.375707 robomotion-1.7.5rc0/setup.cfg
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)     1400 2023-06-13 14:58:11.000000 robomotion-1.7.5rc0/setup.py
```

### Comparing `robomotion-1.7.4rc0/PKG-INFO` & `robomotion-1.7.5rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robomotion
-Version: 1.7.4rc0
+Version: 1.7.5rc0
 Summary: UNKNOWN
 Home-page: https://robomotion.io/
 Author: Robomotion IO
 Author-email: support@robomotion.io
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/robomotionio/python-lib/issues
 Project-URL: Dev Docs, https://docs.robomotion.io/
```

### Comparing `robomotion-1.7.4rc0/robomotion/debug.py` & `robomotion-1.7.5rc0/robomotion/debug.py`

 * *Files identical despite different names*

### Comparing `robomotion-1.7.4rc0/robomotion/decorators.py` & `robomotion-1.7.5rc0/robomotion/decorators.py`

 * *Files identical despite different names*

### Comparing `robomotion-1.7.4rc0/robomotion/event.py` & `robomotion-1.7.5rc0/robomotion/event.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,15 @@
     DebugRequest,
     EmitOutputRequest,
     EmitInputRequest,
     EmitErrorRequest,
     EmitFlowEventRequest,
     AppRequestRequest,
 )
-from pickle5 import *
-
+import pickle
 
 class Event:
     @staticmethod
     def emit_debug(guid: str, name: str, message: object):
         if Runtime.client == None:
             raise RuntimeNotInitializedError
```

### Comparing `robomotion-1.7.4rc0/robomotion/health.py` & `robomotion-1.7.5rc0/robomotion/health.py`

 * *Files identical despite different names*

### Comparing `robomotion-1.7.4rc0/robomotion/health_pb2.py` & `robomotion-1.7.5rc0/robomotion/health_pb2.py`

 * *Files identical despite different names*

### Comparing `robomotion-1.7.4rc0/robomotion/health_pb2_grpc.py` & `robomotion-1.7.5rc0/robomotion/health_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `robomotion-1.7.4rc0/robomotion/icons.py` & `robomotion-1.7.5rc0/robomotion/icons.py`

 * *Files identical despite different names*

### Comparing `robomotion-1.7.4rc0/robomotion/message.py` & `robomotion-1.7.5rc0/robomotion/message.py`

 * *Files identical despite different names*

### Comparing `robomotion-1.7.4rc0/robomotion/node.py` & `robomotion-1.7.5rc0/robomotion/node.py`

 * *Files identical despite different names*

### Comparing `robomotion-1.7.4rc0/robomotion/plugin.py` & `robomotion-1.7.5rc0/robomotion/plugin.py`

 * *Files identical despite different names*

### Comparing `robomotion-1.7.4rc0/robomotion/plugin_pb2.py` & `robomotion-1.7.5rc0/robomotion/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `robomotion-1.7.4rc0/robomotion/plugin_pb2_grpc.py` & `robomotion-1.7.5rc0/robomotion/plugin_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `robomotion-1.7.4rc0/robomotion/runner_pb2.py` & `robomotion-1.7.5rc0/robomotion/runner_pb2.py`

 * *Files identical despite different names*

### Comparing `robomotion-1.7.4rc0/robomotion/runner_pb2_grpc.py` & `robomotion-1.7.5rc0/robomotion/runner_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `robomotion-1.7.4rc0/robomotion/runtime.py` & `robomotion-1.7.5rc0/robomotion/runtime.py`

 * *Files identical despite different names*

### Comparing `robomotion-1.7.4rc0/robomotion/spec.py` & `robomotion-1.7.5rc0/robomotion/spec.py`

 * *Files identical despite different names*

### Comparing `robomotion-1.7.4rc0/robomotion/struct_pb2.py` & `robomotion-1.7.5rc0/robomotion/struct_pb2.py`

 * *Files identical despite different names*

### Comparing `robomotion-1.7.4rc0/robomotion/variable.py` & `robomotion-1.7.5rc0/robomotion/variable.py`

 * *Files identical despite different names*

### Comparing `robomotion-1.7.4rc0/robomotion.egg-info/PKG-INFO` & `robomotion-1.7.5rc0/robomotion.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robomotion
-Version: 1.7.4rc0
+Version: 1.7.5rc0
 Summary: UNKNOWN
 Home-page: https://robomotion.io/
 Author: Robomotion IO
 Author-email: support@robomotion.io
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/robomotionio/python-lib/issues
 Project-URL: Dev Docs, https://docs.robomotion.io/
```

### Comparing `robomotion-1.7.4rc0/robomotion.egg-info/SOURCES.txt` & `robomotion-1.7.5rc0/robomotion.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `robomotion-1.7.4rc0/setup.py` & `robomotion-1.7.5rc0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,21 +27,20 @@
 PACKAGES = find_packages(exclude=["tests", "tests.*"])
 
 REQUIRES = [
     "protobuf==4.23.0",
     "grpcio==1.54.0",
     "grpcio-tools==1.54.0",
     "jsonpath-ng==1.5.3",
-    "pickle5==0.0.11",
     "zipp==3.1.0",
 ]
 
 setup(
     name=PROJECT_PACKAGE_NAME,
-    version="1.7.4-rc",
+    version="1.7.5-rc",
     url=PROJECT_URL,
     project_urls=PROJECT_URLS,
     author=PROJECT_AUTHOR,
     author_email=PROJECT_EMAIL,
     packages=PACKAGES,
     include_package_data=True,
     zip_safe=False,
```

