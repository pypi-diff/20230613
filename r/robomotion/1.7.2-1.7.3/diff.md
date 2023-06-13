# Comparing `tmp/robomotion-1.7.2.tar.gz` & `tmp/robomotion-1.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robomotion-1.7.2.tar", last modified: Tue Jun 13 09:48:11 2023, max compression
+gzip compressed data, was "robomotion-1.7.3.tar", last modified: Tue Jun 13 10:14:24 2023, max compression
```

## Comparing `robomotion-1.7.2.tar` & `robomotion-1.7.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 hasan     (1000) hasan     (1000)        0 2023-06-13 09:48:11.652544 robomotion-1.7.2/
--rw-rw-r--   0 hasan     (1000) hasan     (1000)      510 2023-06-13 09:48:11.652544 robomotion-1.7.2/PKG-INFO
-drwxrwxr-x   0 hasan     (1000) hasan     (1000)        0 2023-06-13 09:48:11.652544 robomotion-1.7.2/robomotion/
--rw-rw-r--   0 hasan     (1000) hasan     (1000)        0 2022-08-24 12:32:15.000000 robomotion-1.7.2/robomotion/__init__.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)     3855 2023-06-08 09:30:16.000000 robomotion-1.7.2/robomotion/debug.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)      660 2023-05-10 13:07:28.000000 robomotion-1.7.2/robomotion/decorators.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)      338 2023-06-08 09:30:16.000000 robomotion-1.7.2/robomotion/error.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)     1877 2023-06-08 09:30:16.000000 robomotion-1.7.2/robomotion/event.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)      264 2022-08-24 12:32:15.000000 robomotion-1.7.2/robomotion/factory.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)      800 2022-08-24 12:32:15.000000 robomotion-1.7.2/robomotion/health.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)     1601 2023-06-08 09:30:16.000000 robomotion-1.7.2/robomotion/health_pb2.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)     2457 2023-06-08 09:30:16.000000 robomotion-1.7.2/robomotion/health_pb2_grpc.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)  1674682 2023-06-08 09:30:16.000000 robomotion-1.7.2/robomotion/icons.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)     1183 2023-06-08 09:30:16.000000 robomotion-1.7.2/robomotion/message.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)     3392 2022-09-21 11:29:46.000000 robomotion-1.7.2/robomotion/node.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)     2116 2022-08-24 12:32:15.000000 robomotion-1.7.2/robomotion/plugin.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)     7084 2023-06-08 09:30:16.000000 robomotion-1.7.2/robomotion/plugin_pb2.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)    26015 2023-06-08 09:30:16.000000 robomotion-1.7.2/robomotion/plugin_pb2_grpc.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)     2735 2023-06-08 09:30:16.000000 robomotion-1.7.2/robomotion/runner_pb2.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)    11076 2023-06-08 09:30:16.000000 robomotion-1.7.2/robomotion/runner_pb2_grpc.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)     4525 2023-06-13 09:47:09.000000 robomotion-1.7.2/robomotion/runtime.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)    21852 2023-06-13 09:47:09.000000 robomotion-1.7.2/robomotion/spec.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)     2436 2023-06-08 09:30:16.000000 robomotion-1.7.2/robomotion/struct_pb2.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)      159 2023-06-08 09:30:16.000000 robomotion-1.7.2/robomotion/struct_pb2_grpc.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)      507 2023-06-08 09:30:16.000000 robomotion-1.7.2/robomotion/utils.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)     7035 2023-06-13 09:47:09.000000 robomotion-1.7.2/robomotion/variable.py
-drwxrwxr-x   0 hasan     (1000) hasan     (1000)        0 2023-06-13 09:48:11.652544 robomotion-1.7.2/robomotion.egg-info/
--rw-rw-r--   0 hasan     (1000) hasan     (1000)      510 2023-06-13 09:48:11.000000 robomotion-1.7.2/robomotion.egg-info/PKG-INFO
--rw-rw-r--   0 hasan     (1000) hasan     (1000)      747 2023-06-13 09:48:11.000000 robomotion-1.7.2/robomotion.egg-info/SOURCES.txt
--rw-rw-r--   0 hasan     (1000) hasan     (1000)        1 2023-06-13 09:48:11.000000 robomotion-1.7.2/robomotion.egg-info/dependency_links.txt
--rw-rw-r--   0 hasan     (1000) hasan     (1000)        1 2023-06-13 09:48:11.000000 robomotion-1.7.2/robomotion.egg-info/not-zip-safe
--rw-rw-r--   0 hasan     (1000) hasan     (1000)      100 2023-06-13 09:48:11.000000 robomotion-1.7.2/robomotion.egg-info/requires.txt
--rw-rw-r--   0 hasan     (1000) hasan     (1000)       11 2023-06-13 09:48:11.000000 robomotion-1.7.2/robomotion.egg-info/top_level.txt
--rw-rw-r--   0 hasan     (1000) hasan     (1000)       38 2023-06-13 09:48:11.652544 robomotion-1.7.2/setup.cfg
--rw-rw-r--   0 hasan     (1000) hasan     (1000)     1420 2023-06-13 09:47:09.000000 robomotion-1.7.2/setup.py
+drwxrwxr-x   0 hasan     (1000) hasan     (1000)        0 2023-06-13 10:14:24.342220 robomotion-1.7.3/
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)      510 2023-06-13 10:14:24.342220 robomotion-1.7.3/PKG-INFO
+drwxrwxr-x   0 hasan     (1000) hasan     (1000)        0 2023-06-13 10:14:24.342220 robomotion-1.7.3/robomotion/
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)        0 2022-08-24 12:32:15.000000 robomotion-1.7.3/robomotion/__init__.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)     3855 2023-06-08 09:30:16.000000 robomotion-1.7.3/robomotion/debug.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)      660 2023-05-10 13:07:28.000000 robomotion-1.7.3/robomotion/decorators.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)      338 2023-06-08 09:30:16.000000 robomotion-1.7.3/robomotion/error.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)     1877 2023-06-08 09:30:16.000000 robomotion-1.7.3/robomotion/event.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)      264 2022-08-24 12:32:15.000000 robomotion-1.7.3/robomotion/factory.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)      800 2022-08-24 12:32:15.000000 robomotion-1.7.3/robomotion/health.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)     1601 2023-06-08 09:30:16.000000 robomotion-1.7.3/robomotion/health_pb2.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)     2457 2023-06-08 09:30:16.000000 robomotion-1.7.3/robomotion/health_pb2_grpc.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)  1674682 2023-06-08 09:30:16.000000 robomotion-1.7.3/robomotion/icons.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)     1183 2023-06-08 09:30:16.000000 robomotion-1.7.3/robomotion/message.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)     3392 2022-09-21 11:29:46.000000 robomotion-1.7.3/robomotion/node.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)     2116 2022-08-24 12:32:15.000000 robomotion-1.7.3/robomotion/plugin.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)     7137 2023-06-13 10:13:23.000000 robomotion-1.7.3/robomotion/plugin_pb2.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)    27555 2023-06-13 10:13:54.000000 robomotion-1.7.3/robomotion/plugin_pb2_grpc.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)     2735 2023-06-08 09:30:16.000000 robomotion-1.7.3/robomotion/runner_pb2.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)    11076 2023-06-08 09:30:16.000000 robomotion-1.7.3/robomotion/runner_pb2_grpc.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)     4525 2023-06-13 09:47:09.000000 robomotion-1.7.3/robomotion/runtime.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)    21852 2023-06-13 09:47:09.000000 robomotion-1.7.3/robomotion/spec.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)     2436 2023-06-08 09:30:16.000000 robomotion-1.7.3/robomotion/struct_pb2.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)      159 2023-06-08 09:30:16.000000 robomotion-1.7.3/robomotion/struct_pb2_grpc.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)      507 2023-06-08 09:30:16.000000 robomotion-1.7.3/robomotion/utils.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)     7035 2023-06-13 09:47:09.000000 robomotion-1.7.3/robomotion/variable.py
+drwxrwxr-x   0 hasan     (1000) hasan     (1000)        0 2023-06-13 10:14:24.342220 robomotion-1.7.3/robomotion.egg-info/
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)      510 2023-06-13 10:14:24.000000 robomotion-1.7.3/robomotion.egg-info/PKG-INFO
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)      747 2023-06-13 10:14:24.000000 robomotion-1.7.3/robomotion.egg-info/SOURCES.txt
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)        1 2023-06-13 10:14:24.000000 robomotion-1.7.3/robomotion.egg-info/dependency_links.txt
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)        1 2023-06-13 10:14:24.000000 robomotion-1.7.3/robomotion.egg-info/not-zip-safe
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)      100 2023-06-13 10:14:24.000000 robomotion-1.7.3/robomotion.egg-info/requires.txt
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)       11 2023-06-13 10:14:24.000000 robomotion-1.7.3/robomotion.egg-info/top_level.txt
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)       38 2023-06-13 10:14:24.346220 robomotion-1.7.3/setup.cfg
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)     1420 2023-06-13 10:14:11.000000 robomotion-1.7.3/setup.py
```

### Comparing `robomotion-1.7.2/robomotion/debug.py` & `robomotion-1.7.3/robomotion/debug.py`

 * *Files identical despite different names*

### Comparing `robomotion-1.7.2/robomotion/decorators.py` & `robomotion-1.7.3/robomotion/decorators.py`

 * *Files identical despite different names*

### Comparing `robomotion-1.7.2/robomotion/event.py` & `robomotion-1.7.3/robomotion/event.py`

 * *Files identical despite different names*

### Comparing `robomotion-1.7.2/robomotion/health.py` & `robomotion-1.7.3/robomotion/health.py`

 * *Files identical despite different names*

### Comparing `robomotion-1.7.2/robomotion/health_pb2.py` & `robomotion-1.7.3/robomotion/health_pb2.py`

 * *Files identical despite different names*

### Comparing `robomotion-1.7.2/robomotion/health_pb2_grpc.py` & `robomotion-1.7.3/robomotion/health_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `robomotion-1.7.2/robomotion/icons.py` & `robomotion-1.7.3/robomotion/icons.py`

 * *Files identical despite different names*

### Comparing `robomotion-1.7.2/robomotion/message.py` & `robomotion-1.7.3/robomotion/message.py`

 * *Files identical despite different names*

### Comparing `robomotion-1.7.2/robomotion/node.py` & `robomotion-1.7.3/robomotion/node.py`

 * *Files identical despite different names*

### Comparing `robomotion-1.7.2/robomotion/plugin.py` & `robomotion-1.7.3/robomotion/plugin.py`

 * *Files identical despite different names*

### Comparing `robomotion-1.7.2/robomotion/plugin_pb2.py` & `robomotion-1.7.3/robomotion/plugin_pb2.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,79 +2,79 @@
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: plugin.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
-
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from robomotion import struct_pb2 as struct__pb2
+import struct_pb2 as struct__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x0cplugin.proto\x12\x05proto\x1a\x0cstruct.proto"2\n\x05\x45rror\x12\n\n\x02OK\x18\x02 \x01(\x08\x12\x0c\n\x04\x63ode\x18\x03 \x01(\t\x12\x0f\n\x07message\x18\x04 \x01(\t"1\n\x0bInitRequest\x12\x14\n\x0c\x65vent_server\x18\x01 \x01(\r\x12\x0c\n\x04port\x18\x02 \x01(\r"/\n\x0fOnCreateRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0e\n\x06\x63onfig\x18\x02 \x01(\x0c"/\n\x10OnCreateResponse\x12\x1b\n\x05\x65rror\x18\x01 \x01(\x0b\x32\x0c.proto.Error"3\n\x10OnMessageRequest\x12\x0c\n\x04guid\x18\x01 \x01(\t\x12\x11\n\tinMessage\x18\x02 \x01(\x0c"D\n\x11OnMessageResponse\x12\x12\n\noutMessage\x18\x01 \x01(\x0c\x12\x1b\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x0c.proto.Error"\x1e\n\x0eOnCloseRequest\x12\x0c\n\x04guid\x18\x01 \x01(\t".\n\x0fOnCloseResponse\x12\x1b\n\x05\x65rror\x18\x01 \x01(\x0b\x32\x0c.proto.Error"\x07\n\x05\x45mpty";\n\x0c\x44\x65\x62ugRequest\x12\x0c\n\x04guid\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0f\n\x07message\x18\x03 \x01(\x0c"2\n\x14\x45mitFlowEventRequest\x12\x0c\n\x04guid\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t"/\n\x10\x45mitInputRequest\x12\x0c\n\x04guid\x18\x01 \x01(\t\x12\r\n\x05input\x18\x02 \x01(\x0c"?\n\x11\x45mitOutputRequest\x12\x0c\n\x04guid\x18\x01 \x01(\t\x12\x0e\n\x06output\x18\x02 \x01(\x0c\x12\x0c\n\x04port\x18\x03 \x01(\x05"?\n\x10\x45mitErrorRequest\x12\x0c\n\x04guid\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0f\n\x07message\x18\x03 \x01(\t"6\n\x13GetVaultItemRequest\x12\x0f\n\x07vaultId\x18\x01 \x01(\t\x12\x0e\n\x06ItemId\x18\x02 \x01(\t"=\n\x14GetVaultItemResponse\x12%\n\x04item\x18\x01 \x01(\x0b\x32\x17.google.protobuf.Struct"D\n\x13SetVaultItemRequest\x12\x0f\n\x07vaultId\x18\x01 \x01(\t\x12\x0e\n\x06ItemId\x18\x02 \x01(\t\x12\x0c\n\x04\x44\x61ta\x18\x03 \x01(\x0c"=\n\x14SetVaultItemResponse\x12%\n\x04item\x18\x01 \x01(\x0b\x32\x17.google.protobuf.Struct"\'\n\x08Variable\x12\r\n\x05scope\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t"7\n\x12GetVariableRequest\x12!\n\x08variable\x18\x01 \x01(\x0b\x32\x0f.proto.Variable"=\n\x13GetVariableResponse\x12&\n\x05value\x18\x01 \x01(\x0b\x32\x17.google.protobuf.Struct"_\n\x12SetVariableRequest\x12!\n\x08variable\x18\x01 \x01(\x0b\x32\x0f.proto.Variable\x12&\n\x05value\x18\x02 \x01(\x0b\x32\x17.google.protobuf.Struct">\n\x14GetRobotInfoResponse\x12&\n\x05robot\x18\x01 \x01(\x0b\x32\x17.google.protobuf.Struct"5\n\x11\x41ppRequestRequest\x12\x0f\n\x07request\x18\x01 \x01(\x0c\x12\x0f\n\x07timeout\x18\x02 \x01(\x05"&\n\x12\x41ppRequestResponse\x12\x10\n\x08response\x18\x01 \x01(\x0c\x32\xe7\x01\n\x04Node\x12(\n\x04Init\x12\x12.proto.InitRequest\x1a\x0c.proto.Empty\x12;\n\x08OnCreate\x12\x16.proto.OnCreateRequest\x1a\x17.proto.OnCreateResponse\x12>\n\tOnMessage\x12\x17.proto.OnMessageRequest\x1a\x18.proto.OnMessageResponse\x12\x38\n\x07OnClose\x12\x15.proto.OnCloseRequest\x1a\x16.proto.OnCloseResponse2\xc8\x05\n\rRuntimeHelper\x12#\n\x05\x43lose\x12\x0c.proto.Empty\x1a\x0c.proto.Empty\x12*\n\x05\x44\x65\x62ug\x12\x13.proto.DebugRequest\x1a\x0c.proto.Empty\x12:\n\rEmitFlowEvent\x12\x1b.proto.EmitFlowEventRequest\x1a\x0c.proto.Empty\x12\x32\n\tEmitInput\x12\x17.proto.EmitInputRequest\x1a\x0c.proto.Empty\x12\x34\n\nEmitOutput\x12\x18.proto.EmitOutputRequest\x1a\x0c.proto.Empty\x12\x32\n\tEmitError\x12\x17.proto.EmitErrorRequest\x1a\x0c.proto.Empty\x12G\n\x0cGetVaultItem\x12\x1a.proto.GetVaultItemRequest\x1a\x1b.proto.GetVaultItemResponse\x12G\n\x0cSetVaultItem\x12\x1a.proto.SetVaultItemRequest\x1a\x1b.proto.SetVaultItemResponse\x12\x44\n\x0bGetVariable\x12\x19.proto.GetVariableRequest\x1a\x1a.proto.GetVariableResponse\x12\x36\n\x0bSetVariable\x12\x19.proto.SetVariableRequest\x1a\x0c.proto.Empty\x12\x39\n\x0cGetRobotInfo\x12\x0c.proto.Empty\x1a\x1b.proto.GetRobotInfoResponse\x12\x41\n\nAppRequest\x12\x18.proto.AppRequestRequest\x1a\x19.proto.AppRequestResponseb\x06proto3'
-)
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0cplugin.proto\x12\x05proto\x1a\x0cstruct.proto\"2\n\x05\x45rror\x12\n\n\x02OK\x18\x02 \x01(\x08\x12\x0c\n\x04\x63ode\x18\x03 \x01(\t\x12\x0f\n\x07message\x18\x04 \x01(\t\"1\n\x0bInitRequest\x12\x14\n\x0c\x65vent_server\x18\x01 \x01(\r\x12\x0c\n\x04port\x18\x02 \x01(\r\"/\n\x0fOnCreateRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0e\n\x06\x63onfig\x18\x02 \x01(\x0c\"/\n\x10OnCreateResponse\x12\x1b\n\x05\x65rror\x18\x01 \x01(\x0b\x32\x0c.proto.Error\"3\n\x10OnMessageRequest\x12\x0c\n\x04guid\x18\x01 \x01(\t\x12\x11\n\tinMessage\x18\x02 \x01(\x0c\"D\n\x11OnMessageResponse\x12\x12\n\noutMessage\x18\x01 \x01(\x0c\x12\x1b\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x0c.proto.Error\"\x1e\n\x0eOnCloseRequest\x12\x0c\n\x04guid\x18\x01 \x01(\t\".\n\x0fOnCloseResponse\x12\x1b\n\x05\x65rror\x18\x01 \x01(\x0b\x32\x0c.proto.Error\"\x07\n\x05\x45mpty\";\n\x0c\x44\x65\x62ugRequest\x12\x0c\n\x04guid\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0f\n\x07message\x18\x03 \x01(\x0c\"2\n\x14\x45mitFlowEventRequest\x12\x0c\n\x04guid\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"/\n\x10\x45mitInputRequest\x12\x0c\n\x04guid\x18\x01 \x01(\t\x12\r\n\x05input\x18\x02 \x01(\x0c\"?\n\x11\x45mitOutputRequest\x12\x0c\n\x04guid\x18\x01 \x01(\t\x12\x0e\n\x06output\x18\x02 \x01(\x0c\x12\x0c\n\x04port\x18\x03 \x01(\x05\"?\n\x10\x45mitErrorRequest\x12\x0c\n\x04guid\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0f\n\x07message\x18\x03 \x01(\t\"6\n\x13GetVaultItemRequest\x12\x0f\n\x07vaultId\x18\x01 \x01(\t\x12\x0e\n\x06ItemId\x18\x02 \x01(\t\"=\n\x14GetVaultItemResponse\x12%\n\x04item\x18\x01 \x01(\x0b\x32\x17.google.protobuf.Struct\"D\n\x13SetVaultItemRequest\x12\x0f\n\x07vaultId\x18\x01 \x01(\t\x12\x0e\n\x06ItemId\x18\x02 \x01(\t\x12\x0c\n\x04\x44\x61ta\x18\x03 \x01(\x0c\"=\n\x14SetVaultItemResponse\x12%\n\x04item\x18\x01 \x01(\x0b\x32\x17.google.protobuf.Struct\"\'\n\x08Variable\x12\r\n\x05scope\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"7\n\x12GetVariableRequest\x12!\n\x08variable\x18\x01 \x01(\x0b\x32\x0f.proto.Variable\"=\n\x13GetVariableResponse\x12&\n\x05value\x18\x01 \x01(\x0b\x32\x17.google.protobuf.Struct\"_\n\x12SetVariableRequest\x12!\n\x08variable\x18\x01 \x01(\x0b\x32\x0f.proto.Variable\x12&\n\x05value\x18\x02 \x01(\x0b\x32\x17.google.protobuf.Struct\">\n\x14GetRobotInfoResponse\x12&\n\x05robot\x18\x01 \x01(\x0b\x32\x17.google.protobuf.Struct\"5\n\x11\x41ppRequestRequest\x12\x0f\n\x07request\x18\x01 \x01(\x0c\x12\x0f\n\x07timeout\x18\x02 \x01(\x05\"&\n\x12\x41ppRequestResponse\x12\x10\n\x08response\x18\x01 \x01(\x0c\"0\n\x13\x44ownloadFileRequest\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t2\xe7\x01\n\x04Node\x12(\n\x04Init\x12\x12.proto.InitRequest\x1a\x0c.proto.Empty\x12;\n\x08OnCreate\x12\x16.proto.OnCreateRequest\x1a\x17.proto.OnCreateResponse\x12>\n\tOnMessage\x12\x17.proto.OnMessageRequest\x1a\x18.proto.OnMessageResponse\x12\x38\n\x07OnClose\x12\x15.proto.OnCloseRequest\x1a\x16.proto.OnCloseResponse2\x82\x06\n\rRuntimeHelper\x12#\n\x05\x43lose\x12\x0c.proto.Empty\x1a\x0c.proto.Empty\x12*\n\x05\x44\x65\x62ug\x12\x13.proto.DebugRequest\x1a\x0c.proto.Empty\x12:\n\rEmitFlowEvent\x12\x1b.proto.EmitFlowEventRequest\x1a\x0c.proto.Empty\x12\x32\n\tEmitInput\x12\x17.proto.EmitInputRequest\x1a\x0c.proto.Empty\x12\x34\n\nEmitOutput\x12\x18.proto.EmitOutputRequest\x1a\x0c.proto.Empty\x12\x32\n\tEmitError\x12\x17.proto.EmitErrorRequest\x1a\x0c.proto.Empty\x12G\n\x0cGetVaultItem\x12\x1a.proto.GetVaultItemRequest\x1a\x1b.proto.GetVaultItemResponse\x12G\n\x0cSetVaultItem\x12\x1a.proto.SetVaultItemRequest\x1a\x1b.proto.SetVaultItemResponse\x12\x44\n\x0bGetVariable\x12\x19.proto.GetVariableRequest\x1a\x1a.proto.GetVariableResponse\x12\x36\n\x0bSetVariable\x12\x19.proto.SetVariableRequest\x1a\x0c.proto.Empty\x12\x39\n\x0cGetRobotInfo\x12\x0c.proto.Empty\x1a\x1b.proto.GetRobotInfoResponse\x12\x41\n\nAppRequest\x12\x18.proto.AppRequestRequest\x1a\x19.proto.AppRequestResponse\x12\x38\n\x0c\x44ownloadFile\x12\x1a.proto.DownloadFileRequest\x1a\x0c.proto.Emptyb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "plugin_pb2", globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'plugin_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
-    DESCRIPTOR._options = None
-    _ERROR._serialized_start = 37
-    _ERROR._serialized_end = 87
-    _INITREQUEST._serialized_start = 89
-    _INITREQUEST._serialized_end = 138
-    _ONCREATEREQUEST._serialized_start = 140
-    _ONCREATEREQUEST._serialized_end = 187
-    _ONCREATERESPONSE._serialized_start = 189
-    _ONCREATERESPONSE._serialized_end = 236
-    _ONMESSAGEREQUEST._serialized_start = 238
-    _ONMESSAGEREQUEST._serialized_end = 289
-    _ONMESSAGERESPONSE._serialized_start = 291
-    _ONMESSAGERESPONSE._serialized_end = 359
-    _ONCLOSEREQUEST._serialized_start = 361
-    _ONCLOSEREQUEST._serialized_end = 391
-    _ONCLOSERESPONSE._serialized_start = 393
-    _ONCLOSERESPONSE._serialized_end = 439
-    _EMPTY._serialized_start = 441
-    _EMPTY._serialized_end = 448
-    _DEBUGREQUEST._serialized_start = 450
-    _DEBUGREQUEST._serialized_end = 509
-    _EMITFLOWEVENTREQUEST._serialized_start = 511
-    _EMITFLOWEVENTREQUEST._serialized_end = 561
-    _EMITINPUTREQUEST._serialized_start = 563
-    _EMITINPUTREQUEST._serialized_end = 610
-    _EMITOUTPUTREQUEST._serialized_start = 612
-    _EMITOUTPUTREQUEST._serialized_end = 675
-    _EMITERRORREQUEST._serialized_start = 677
-    _EMITERRORREQUEST._serialized_end = 740
-    _GETVAULTITEMREQUEST._serialized_start = 742
-    _GETVAULTITEMREQUEST._serialized_end = 796
-    _GETVAULTITEMRESPONSE._serialized_start = 798
-    _GETVAULTITEMRESPONSE._serialized_end = 859
-    _SETVAULTITEMREQUEST._serialized_start = 861
-    _SETVAULTITEMREQUEST._serialized_end = 929
-    _SETVAULTITEMRESPONSE._serialized_start = 931
-    _SETVAULTITEMRESPONSE._serialized_end = 992
-    _VARIABLE._serialized_start = 994
-    _VARIABLE._serialized_end = 1033
-    _GETVARIABLEREQUEST._serialized_start = 1035
-    _GETVARIABLEREQUEST._serialized_end = 1090
-    _GETVARIABLERESPONSE._serialized_start = 1092
-    _GETVARIABLERESPONSE._serialized_end = 1153
-    _SETVARIABLEREQUEST._serialized_start = 1155
-    _SETVARIABLEREQUEST._serialized_end = 1250
-    _GETROBOTINFORESPONSE._serialized_start = 1252
-    _GETROBOTINFORESPONSE._serialized_end = 1314
-    _APPREQUESTREQUEST._serialized_start = 1316
-    _APPREQUESTREQUEST._serialized_end = 1369
-    _APPREQUESTRESPONSE._serialized_start = 1371
-    _APPREQUESTRESPONSE._serialized_end = 1409
-    _NODE._serialized_start = 1412
-    _NODE._serialized_end = 1643
-    _RUNTIMEHELPER._serialized_start = 1646
-    _RUNTIMEHELPER._serialized_end = 2358
+
+  DESCRIPTOR._options = None
+  _ERROR._serialized_start=37
+  _ERROR._serialized_end=87
+  _INITREQUEST._serialized_start=89
+  _INITREQUEST._serialized_end=138
+  _ONCREATEREQUEST._serialized_start=140
+  _ONCREATEREQUEST._serialized_end=187
+  _ONCREATERESPONSE._serialized_start=189
+  _ONCREATERESPONSE._serialized_end=236
+  _ONMESSAGEREQUEST._serialized_start=238
+  _ONMESSAGEREQUEST._serialized_end=289
+  _ONMESSAGERESPONSE._serialized_start=291
+  _ONMESSAGERESPONSE._serialized_end=359
+  _ONCLOSEREQUEST._serialized_start=361
+  _ONCLOSEREQUEST._serialized_end=391
+  _ONCLOSERESPONSE._serialized_start=393
+  _ONCLOSERESPONSE._serialized_end=439
+  _EMPTY._serialized_start=441
+  _EMPTY._serialized_end=448
+  _DEBUGREQUEST._serialized_start=450
+  _DEBUGREQUEST._serialized_end=509
+  _EMITFLOWEVENTREQUEST._serialized_start=511
+  _EMITFLOWEVENTREQUEST._serialized_end=561
+  _EMITINPUTREQUEST._serialized_start=563
+  _EMITINPUTREQUEST._serialized_end=610
+  _EMITOUTPUTREQUEST._serialized_start=612
+  _EMITOUTPUTREQUEST._serialized_end=675
+  _EMITERRORREQUEST._serialized_start=677
+  _EMITERRORREQUEST._serialized_end=740
+  _GETVAULTITEMREQUEST._serialized_start=742
+  _GETVAULTITEMREQUEST._serialized_end=796
+  _GETVAULTITEMRESPONSE._serialized_start=798
+  _GETVAULTITEMRESPONSE._serialized_end=859
+  _SETVAULTITEMREQUEST._serialized_start=861
+  _SETVAULTITEMREQUEST._serialized_end=929
+  _SETVAULTITEMRESPONSE._serialized_start=931
+  _SETVAULTITEMRESPONSE._serialized_end=992
+  _VARIABLE._serialized_start=994
+  _VARIABLE._serialized_end=1033
+  _GETVARIABLEREQUEST._serialized_start=1035
+  _GETVARIABLEREQUEST._serialized_end=1090
+  _GETVARIABLERESPONSE._serialized_start=1092
+  _GETVARIABLERESPONSE._serialized_end=1153
+  _SETVARIABLEREQUEST._serialized_start=1155
+  _SETVARIABLEREQUEST._serialized_end=1250
+  _GETROBOTINFORESPONSE._serialized_start=1252
+  _GETROBOTINFORESPONSE._serialized_end=1314
+  _APPREQUESTREQUEST._serialized_start=1316
+  _APPREQUESTREQUEST._serialized_end=1369
+  _APPREQUESTRESPONSE._serialized_start=1371
+  _APPREQUESTRESPONSE._serialized_end=1409
+  _DOWNLOADFILEREQUEST._serialized_start=1411
+  _DOWNLOADFILEREQUEST._serialized_end=1459
+  _NODE._serialized_start=1462
+  _NODE._serialized_end=1693
+  _RUNTIMEHELPER._serialized_start=1696
+  _RUNTIMEHELPER._serialized_end=2466
 # @@protoc_insertion_point(module_scope)
```

### Comparing `robomotion-1.7.2/robomotion/plugin_pb2_grpc.py` & `robomotion-1.7.3/robomotion/plugin_pb2_grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -279,14 +279,19 @@
             response_deserializer=plugin__pb2.GetRobotInfoResponse.FromString,
         )
         self.AppRequest = channel.unary_unary(
             "/proto.RuntimeHelper/AppRequest",
             request_serializer=plugin__pb2.AppRequestRequest.SerializeToString,
             response_deserializer=plugin__pb2.AppRequestResponse.FromString,
         )
+        self.DownloadFile = channel.unary_unary(
+            "/proto.RuntimeHelper/DownloadFile",
+            request_serializer=plugin__pb2.DownloadFileRequest.SerializeToString,
+            response_deserializer=plugin__pb2.Empty.FromString,
+        )
 
 
 class RuntimeHelperServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def Close(self, request, context):
         """Missing associated documentation comment in .proto file."""
@@ -356,14 +361,20 @@
 
     def AppRequest(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
+    def DownloadFile(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details("Method not implemented!")
+        raise NotImplementedError("Method not implemented!")
+
 
 def add_RuntimeHelperServicer_to_server(servicer, server):
     rpc_method_handlers = {
         "Close": grpc.unary_unary_rpc_method_handler(
             servicer.Close,
             request_deserializer=plugin__pb2.Empty.FromString,
             response_serializer=plugin__pb2.Empty.SerializeToString,
@@ -419,14 +430,19 @@
             response_serializer=plugin__pb2.GetRobotInfoResponse.SerializeToString,
         ),
         "AppRequest": grpc.unary_unary_rpc_method_handler(
             servicer.AppRequest,
             request_deserializer=plugin__pb2.AppRequestRequest.FromString,
             response_serializer=plugin__pb2.AppRequestResponse.SerializeToString,
         ),
+        "DownloadFile": grpc.unary_unary_rpc_method_handler(
+            servicer.DownloadFile,
+            request_deserializer=plugin__pb2.DownloadFileRequest.FromString,
+            response_serializer=plugin__pb2.Empty.SerializeToString,
+        ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
         "proto.RuntimeHelper", rpc_method_handlers
     )
     server.add_generic_rpc_handlers((generic_handler,))
 
 
@@ -775,9 +791,38 @@
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
+            metadata,
+        )
+
+    @staticmethod
+    def DownloadFile(
+        request,
+        target,
+        options=(),
+        channel_credentials=None,
+        call_credentials=None,
+        insecure=False,
+        compression=None,
+        wait_for_ready=None,
+        timeout=None,
+        metadata=None,
+    ):
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            "/proto.RuntimeHelper/DownloadFile",
+            plugin__pb2.DownloadFileRequest.SerializeToString,
+            plugin__pb2.Empty.FromString,
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
             metadata,
         )
```

### Comparing `robomotion-1.7.2/robomotion/runner_pb2.py` & `robomotion-1.7.3/robomotion/runner_pb2.py`

 * *Files identical despite different names*

### Comparing `robomotion-1.7.2/robomotion/runner_pb2_grpc.py` & `robomotion-1.7.3/robomotion/runner_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `robomotion-1.7.2/robomotion/runtime.py` & `robomotion-1.7.3/robomotion/runtime.py`

 * *Files identical despite different names*

### Comparing `robomotion-1.7.2/robomotion/spec.py` & `robomotion-1.7.3/robomotion/spec.py`

 * *Files identical despite different names*

### Comparing `robomotion-1.7.2/robomotion/struct_pb2.py` & `robomotion-1.7.3/robomotion/struct_pb2.py`

 * *Files identical despite different names*

### Comparing `robomotion-1.7.2/robomotion/variable.py` & `robomotion-1.7.3/robomotion/variable.py`

 * *Files identical despite different names*

### Comparing `robomotion-1.7.2/robomotion.egg-info/SOURCES.txt` & `robomotion-1.7.3/robomotion.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `robomotion-1.7.2/setup.py` & `robomotion-1.7.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     "jsonpath-ng==1.5.3",
     "pickle5==0.0.11",
     "zipp==3.1.0",
 ]
 
 setup(
     name=PROJECT_PACKAGE_NAME,
-    version="1.7.2",
+    version="1.7.3",
     url=PROJECT_URL,
     project_urls=PROJECT_URLS,
     author=PROJECT_AUTHOR,
     author_email=PROJECT_EMAIL,
     packages=PACKAGES,
     include_package_data=True,
     zip_safe=False,
```

