# Comparing `tmp/robomotion-1.7.1.tar.gz` & `tmp/robomotion-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robomotion-1.7.1.tar", last modified: Thu Jun  8 09:47:23 2023, max compression
+gzip compressed data, was "robomotion-1.7.2.tar", last modified: Tue Jun 13 09:48:11 2023, max compression
```

## Comparing `robomotion-1.7.1.tar` & `robomotion-1.7.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 hasan     (1000) hasan     (1000)        0 2023-06-08 09:47:23.291285 robomotion-1.7.1/
--rw-rw-r--   0 hasan     (1000) hasan     (1000)      510 2023-06-08 09:47:23.287285 robomotion-1.7.1/PKG-INFO
-drwxrwxr-x   0 hasan     (1000) hasan     (1000)        0 2023-06-08 09:47:23.287285 robomotion-1.7.1/robomotion/
--rw-rw-r--   0 hasan     (1000) hasan     (1000)        0 2022-08-24 12:32:15.000000 robomotion-1.7.1/robomotion/__init__.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)     3855 2023-06-08 09:30:16.000000 robomotion-1.7.1/robomotion/debug.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)      660 2023-05-10 13:07:28.000000 robomotion-1.7.1/robomotion/decorators.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)      338 2023-06-08 09:30:16.000000 robomotion-1.7.1/robomotion/error.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)     1877 2023-06-08 09:30:16.000000 robomotion-1.7.1/robomotion/event.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)      264 2022-08-24 12:32:15.000000 robomotion-1.7.1/robomotion/factory.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)      800 2022-08-24 12:32:15.000000 robomotion-1.7.1/robomotion/health.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)     1601 2023-06-08 09:30:16.000000 robomotion-1.7.1/robomotion/health_pb2.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)     2457 2023-06-08 09:30:16.000000 robomotion-1.7.1/robomotion/health_pb2_grpc.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)  1674682 2023-06-08 09:30:16.000000 robomotion-1.7.1/robomotion/icons.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)     1183 2023-06-08 09:30:16.000000 robomotion-1.7.1/robomotion/message.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)     3392 2022-09-21 11:29:46.000000 robomotion-1.7.1/robomotion/node.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)     2116 2022-08-24 12:32:15.000000 robomotion-1.7.1/robomotion/plugin.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)     7084 2023-06-08 09:30:16.000000 robomotion-1.7.1/robomotion/plugin_pb2.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)    26015 2023-06-08 09:30:16.000000 robomotion-1.7.1/robomotion/plugin_pb2_grpc.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)     2735 2023-06-08 09:30:16.000000 robomotion-1.7.1/robomotion/runner_pb2.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)    11076 2023-06-08 09:30:16.000000 robomotion-1.7.1/robomotion/runner_pb2_grpc.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)     4268 2023-06-08 09:30:16.000000 robomotion-1.7.1/robomotion/runtime.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)    21852 2023-06-08 09:30:51.000000 robomotion-1.7.1/robomotion/spec.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)     2436 2023-06-08 09:30:16.000000 robomotion-1.7.1/robomotion/struct_pb2.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)      159 2023-06-08 09:30:16.000000 robomotion-1.7.1/robomotion/struct_pb2_grpc.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)      507 2023-06-08 09:30:16.000000 robomotion-1.7.1/robomotion/utils.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)     7035 2023-06-08 09:40:11.000000 robomotion-1.7.1/robomotion/variable.py
-drwxrwxr-x   0 hasan     (1000) hasan     (1000)        0 2023-06-08 09:47:23.287285 robomotion-1.7.1/robomotion.egg-info/
--rw-rw-r--   0 hasan     (1000) hasan     (1000)      510 2023-06-08 09:47:23.000000 robomotion-1.7.1/robomotion.egg-info/PKG-INFO
--rw-rw-r--   0 hasan     (1000) hasan     (1000)      747 2023-06-08 09:47:23.000000 robomotion-1.7.1/robomotion.egg-info/SOURCES.txt
--rw-rw-r--   0 hasan     (1000) hasan     (1000)        1 2023-06-08 09:47:23.000000 robomotion-1.7.1/robomotion.egg-info/dependency_links.txt
--rw-rw-r--   0 hasan     (1000) hasan     (1000)        1 2023-05-11 08:16:43.000000 robomotion-1.7.1/robomotion.egg-info/not-zip-safe
--rw-rw-r--   0 hasan     (1000) hasan     (1000)      100 2023-06-08 09:47:23.000000 robomotion-1.7.1/robomotion.egg-info/requires.txt
--rw-rw-r--   0 hasan     (1000) hasan     (1000)       11 2023-06-08 09:47:23.000000 robomotion-1.7.1/robomotion.egg-info/top_level.txt
--rw-rw-r--   0 hasan     (1000) hasan     (1000)       38 2023-06-08 09:47:23.291285 robomotion-1.7.1/setup.cfg
--rw-rw-r--   0 hasan     (1000) hasan     (1000)     1420 2023-06-08 09:44:55.000000 robomotion-1.7.1/setup.py
+drwxrwxr-x   0 hasan     (1000) hasan     (1000)        0 2023-06-13 09:48:11.652544 robomotion-1.7.2/
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)      510 2023-06-13 09:48:11.652544 robomotion-1.7.2/PKG-INFO
+drwxrwxr-x   0 hasan     (1000) hasan     (1000)        0 2023-06-13 09:48:11.652544 robomotion-1.7.2/robomotion/
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)        0 2022-08-24 12:32:15.000000 robomotion-1.7.2/robomotion/__init__.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)     3855 2023-06-08 09:30:16.000000 robomotion-1.7.2/robomotion/debug.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)      660 2023-05-10 13:07:28.000000 robomotion-1.7.2/robomotion/decorators.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)      338 2023-06-08 09:30:16.000000 robomotion-1.7.2/robomotion/error.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)     1877 2023-06-08 09:30:16.000000 robomotion-1.7.2/robomotion/event.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)      264 2022-08-24 12:32:15.000000 robomotion-1.7.2/robomotion/factory.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)      800 2022-08-24 12:32:15.000000 robomotion-1.7.2/robomotion/health.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)     1601 2023-06-08 09:30:16.000000 robomotion-1.7.2/robomotion/health_pb2.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)     2457 2023-06-08 09:30:16.000000 robomotion-1.7.2/robomotion/health_pb2_grpc.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)  1674682 2023-06-08 09:30:16.000000 robomotion-1.7.2/robomotion/icons.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)     1183 2023-06-08 09:30:16.000000 robomotion-1.7.2/robomotion/message.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)     3392 2022-09-21 11:29:46.000000 robomotion-1.7.2/robomotion/node.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)     2116 2022-08-24 12:32:15.000000 robomotion-1.7.2/robomotion/plugin.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)     7084 2023-06-08 09:30:16.000000 robomotion-1.7.2/robomotion/plugin_pb2.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)    26015 2023-06-08 09:30:16.000000 robomotion-1.7.2/robomotion/plugin_pb2_grpc.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)     2735 2023-06-08 09:30:16.000000 robomotion-1.7.2/robomotion/runner_pb2.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)    11076 2023-06-08 09:30:16.000000 robomotion-1.7.2/robomotion/runner_pb2_grpc.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)     4525 2023-06-13 09:47:09.000000 robomotion-1.7.2/robomotion/runtime.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)    21852 2023-06-13 09:47:09.000000 robomotion-1.7.2/robomotion/spec.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)     2436 2023-06-08 09:30:16.000000 robomotion-1.7.2/robomotion/struct_pb2.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)      159 2023-06-08 09:30:16.000000 robomotion-1.7.2/robomotion/struct_pb2_grpc.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)      507 2023-06-08 09:30:16.000000 robomotion-1.7.2/robomotion/utils.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)     7035 2023-06-13 09:47:09.000000 robomotion-1.7.2/robomotion/variable.py
+drwxrwxr-x   0 hasan     (1000) hasan     (1000)        0 2023-06-13 09:48:11.652544 robomotion-1.7.2/robomotion.egg-info/
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)      510 2023-06-13 09:48:11.000000 robomotion-1.7.2/robomotion.egg-info/PKG-INFO
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)      747 2023-06-13 09:48:11.000000 robomotion-1.7.2/robomotion.egg-info/SOURCES.txt
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)        1 2023-06-13 09:48:11.000000 robomotion-1.7.2/robomotion.egg-info/dependency_links.txt
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)        1 2023-06-13 09:48:11.000000 robomotion-1.7.2/robomotion.egg-info/not-zip-safe
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)      100 2023-06-13 09:48:11.000000 robomotion-1.7.2/robomotion.egg-info/requires.txt
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)       11 2023-06-13 09:48:11.000000 robomotion-1.7.2/robomotion.egg-info/top_level.txt
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)       38 2023-06-13 09:48:11.652544 robomotion-1.7.2/setup.cfg
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)     1420 2023-06-13 09:47:09.000000 robomotion-1.7.2/setup.py
```

### Comparing `robomotion-1.7.1/robomotion/debug.py` & `robomotion-1.7.2/robomotion/debug.py`

 * *Files identical despite different names*

### Comparing `robomotion-1.7.1/robomotion/decorators.py` & `robomotion-1.7.2/robomotion/decorators.py`

 * *Files identical despite different names*

### Comparing `robomotion-1.7.1/robomotion/event.py` & `robomotion-1.7.2/robomotion/event.py`

 * *Files identical despite different names*

### Comparing `robomotion-1.7.1/robomotion/health.py` & `robomotion-1.7.2/robomotion/health.py`

 * *Files identical despite different names*

### Comparing `robomotion-1.7.1/robomotion/health_pb2.py` & `robomotion-1.7.2/robomotion/health_pb2.py`

 * *Files identical despite different names*

### Comparing `robomotion-1.7.1/robomotion/health_pb2_grpc.py` & `robomotion-1.7.2/robomotion/health_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `robomotion-1.7.1/robomotion/icons.py` & `robomotion-1.7.2/robomotion/icons.py`

 * *Files identical despite different names*

### Comparing `robomotion-1.7.1/robomotion/message.py` & `robomotion-1.7.2/robomotion/message.py`

 * *Files identical despite different names*

### Comparing `robomotion-1.7.1/robomotion/node.py` & `robomotion-1.7.2/robomotion/node.py`

 * *Files identical despite different names*

### Comparing `robomotion-1.7.1/robomotion/plugin.py` & `robomotion-1.7.2/robomotion/plugin.py`

 * *Files identical despite different names*

### Comparing `robomotion-1.7.1/robomotion/plugin_pb2.py` & `robomotion-1.7.2/robomotion/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `robomotion-1.7.1/robomotion/plugin_pb2_grpc.py` & `robomotion-1.7.2/robomotion/plugin_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `robomotion-1.7.1/robomotion/runner_pb2.py` & `robomotion-1.7.2/robomotion/runner_pb2.py`

 * *Files identical despite different names*

### Comparing `robomotion-1.7.1/robomotion/runner_pb2_grpc.py` & `robomotion-1.7.2/robomotion/runner_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `robomotion-1.7.1/robomotion/runtime.py` & `robomotion-1.7.2/robomotion/runtime.py`

 * *Files 4% similar despite different names*

```diff
@@ -148,7 +148,15 @@
         response = Runtime.client.GetRobotInfo(request)
         return json_format.MessageToDict(response.robot)["value"]
 
     @staticmethod
     def get_robot_version() -> str:
         info = Runtime.get_robot_info()
         return str(info.get("version"))
+
+    @staticmethod
+    def download_file(url: str, path: str):
+        if Runtime.client == None:
+            raise RuntimeNotInitializedError
+
+        request = plugin_pb2.DownloadFileRequest(url=url, path=path)
+        Runtime.client.DownloadFile(request)
```

### Comparing `robomotion-1.7.1/robomotion/spec.py` & `robomotion-1.7.2/robomotion/spec.py`

 * *Files identical despite different names*

### Comparing `robomotion-1.7.1/robomotion/struct_pb2.py` & `robomotion-1.7.2/robomotion/struct_pb2.py`

 * *Files identical despite different names*

### Comparing `robomotion-1.7.1/robomotion/variable.py` & `robomotion-1.7.2/robomotion/variable.py`

 * *Files identical despite different names*

### Comparing `robomotion-1.7.1/robomotion.egg-info/SOURCES.txt` & `robomotion-1.7.2/robomotion.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `robomotion-1.7.1/setup.py` & `robomotion-1.7.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     "jsonpath-ng==1.5.3",
     "pickle5==0.0.11",
     "zipp==3.1.0",
 ]
 
 setup(
     name=PROJECT_PACKAGE_NAME,
-    version="1.7.1",
+    version="1.7.2",
     url=PROJECT_URL,
     project_urls=PROJECT_URLS,
     author=PROJECT_AUTHOR,
     author_email=PROJECT_EMAIL,
     packages=PACKAGES,
     include_package_data=True,
     zip_safe=False,
```

