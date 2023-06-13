# Comparing `tmp/BcryptRpcServer-0.0.1.tar.gz` & `tmp/BcryptRpcServer-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BcryptRpcServer-0.0.1.tar", last modified: Tue Jun 13 05:09:31 2023, max compression
+gzip compressed data, was "BcryptRpcServer-0.0.2.tar", last modified: Tue Jun 13 05:54:27 2023, max compression
```

## Comparing `BcryptRpcServer-0.0.1.tar` & `BcryptRpcServer-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,12 @@
-drwxr-xr-x   0 cyal1      (501) wheel        (0)        0 2023-06-13 05:09:31.824647 BcryptRpcServer-0.0.1/
-drwxr-xr-x   0 cyal1      (501) wheel        (0)        0 2023-06-13 05:09:31.824312 BcryptRpcServer-0.0.1/BcryptRpcServer.egg-info/
--rw-r--r--   0 cyal1      (501) wheel        (0)     1723 2023-06-13 05:09:31.000000 BcryptRpcServer-0.0.1/BcryptRpcServer.egg-info/PKG-INFO
--rw-r--r--   0 cyal1      (501) wheel        (0)      246 2023-06-13 05:09:31.000000 BcryptRpcServer-0.0.1/BcryptRpcServer.egg-info/SOURCES.txt
--rw-r--r--   0 cyal1      (501) wheel        (0)        1 2023-06-13 05:09:31.000000 BcryptRpcServer-0.0.1/BcryptRpcServer.egg-info/dependency_links.txt
--rw-r--r--   0 cyal1      (501) wheel        (0)       44 2023-06-13 05:09:31.000000 BcryptRpcServer-0.0.1/BcryptRpcServer.egg-info/requires.txt
--rw-r--r--   0 cyal1      (501) wheel        (0)       16 2023-06-13 05:09:31.000000 BcryptRpcServer-0.0.1/BcryptRpcServer.egg-info/top_level.txt
--rw-r--r--   0 cyal1      (501) wheel        (0)     3470 2023-06-13 05:05:39.000000 BcryptRpcServer-0.0.1/BcryptRpcServer.py
--rw-r--r--   0 cyal1      (501) wheel        (0)     1723 2023-06-13 05:09:31.824508 BcryptRpcServer-0.0.1/PKG-INFO
--rw-r--r--   0 cyal1      (501) wheel        (0)     1401 2023-06-13 04:52:23.000000 BcryptRpcServer-0.0.1/README.md
--rw-r--r--   0 cyal1      (501) wheel        (0)      513 2023-06-13 04:55:09.000000 BcryptRpcServer-0.0.1/pyproject.toml
--rw-r--r--   0 cyal1      (501) wheel        (0)       38 2023-06-13 05:09:31.824707 BcryptRpcServer-0.0.1/setup.cfg
--rw-r--r--   0 cyal1      (501) wheel        (0)     1369 2023-06-13 05:09:17.000000 BcryptRpcServer-0.0.1/setup.py
+drwxr-xr-x   0 cyal1      (501) wheel        (0)        0 2023-06-13 05:54:27.040069 BcryptRpcServer-0.0.2/
+drwxr-xr-x   0 cyal1      (501) wheel        (0)        0 2023-06-13 05:54:27.039762 BcryptRpcServer-0.0.2/BcryptRpcServer.egg-info/
+-rw-r--r--   0 cyal1      (501) wheel        (0)     1686 2023-06-13 05:54:27.000000 BcryptRpcServer-0.0.2/BcryptRpcServer.egg-info/PKG-INFO
+-rw-r--r--   0 cyal1      (501) wheel        (0)      231 2023-06-13 05:54:27.000000 BcryptRpcServer-0.0.2/BcryptRpcServer.egg-info/SOURCES.txt
+-rw-r--r--   0 cyal1      (501) wheel        (0)        1 2023-06-13 05:54:27.000000 BcryptRpcServer-0.0.2/BcryptRpcServer.egg-info/dependency_links.txt
+-rw-r--r--   0 cyal1      (501) wheel        (0)       53 2023-06-13 05:54:27.000000 BcryptRpcServer-0.0.2/BcryptRpcServer.egg-info/requires.txt
+-rw-r--r--   0 cyal1      (501) wheel        (0)       16 2023-06-13 05:54:27.000000 BcryptRpcServer-0.0.2/BcryptRpcServer.egg-info/top_level.txt
+-rw-r--r--   0 cyal1      (501) wheel        (0)     3470 2023-06-13 05:54:16.000000 BcryptRpcServer-0.0.2/BcryptRpcServer.py
+-rw-r--r--   0 cyal1      (501) wheel        (0)     1686 2023-06-13 05:54:27.039933 BcryptRpcServer-0.0.2/PKG-INFO
+-rw-r--r--   0 cyal1      (501) wheel        (0)     1401 2023-06-13 04:52:23.000000 BcryptRpcServer-0.0.2/README.md
+-rw-r--r--   0 cyal1      (501) wheel        (0)       38 2023-06-13 05:54:27.040109 BcryptRpcServer-0.0.2/setup.cfg
+-rw-r--r--   0 cyal1      (501) wheel        (0)     1378 2023-06-13 05:50:23.000000 BcryptRpcServer-0.0.2/setup.py
```

### Comparing `BcryptRpcServer-0.0.1/BcryptRpcServer.egg-info/PKG-INFO` & `BcryptRpcServer-0.0.2/BcryptRpcServer.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: BcryptRpcServer
-Version: 0.0.1
+Version: 0.0.2
 Summary: The rpc server api of https://github.com/cyal1/BcryptMontoya
 Home-page: https://github.com/cyal1/BcryptRpcServer/tree/main/python
 Author: cyal1
 Author-email: admin@example.com
-License: UNKNOWN
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # BcryptRpcServer
 The rpc server of https://github.com/cyal1/BcryptMontoya
 
 ## install
 `pip install BcryptRpcServer`
@@ -75,9 +73,7 @@
 
 BcryptRpcServer.run("127.0.0.1:30051")
 
 ```
 
 
 
-
-
```

### Comparing `BcryptRpcServer-0.0.1/BcryptRpcServer.py` & `BcryptRpcServer-0.0.2/BcryptRpcServer.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import google.protobuf.any_pb2 as any_pb2
 from google.protobuf.wrappers_pb2 import *
 import burpextender_pb2 as pb2
 from concurrent import futures
 import burpextender_pb2_grpc as pb2_grpc
 
 
-__version__ = '0.0.1'
+__version__ = '0.0.2'
 function_registry = {}
 
 def expose(func):
     function_registry[func.__name__] = func
 
 class CallFuncServicer(pb2_grpc.CallFuncServiceServicer):
     def CallFunc(self, request, context):
```

### Comparing `BcryptRpcServer-0.0.1/PKG-INFO` & `BcryptRpcServer-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: BcryptRpcServer
-Version: 0.0.1
+Version: 0.0.2
 Summary: The rpc server api of https://github.com/cyal1/BcryptMontoya
 Home-page: https://github.com/cyal1/BcryptRpcServer/tree/main/python
 Author: cyal1
 Author-email: admin@example.com
-License: UNKNOWN
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # BcryptRpcServer
 The rpc server of https://github.com/cyal1/BcryptMontoya
 
 ## install
 `pip install BcryptRpcServer`
@@ -75,9 +73,7 @@
 
 BcryptRpcServer.run("127.0.0.1:30051")
 
 ```
 
 
 
-
-
```

### Comparing `BcryptRpcServer-0.0.1/README.md` & `BcryptRpcServer-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `BcryptRpcServer-0.0.1/setup.py` & `BcryptRpcServer-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     author_email="admin@example.com",
     description="The rpc server api of https://github.com/cyal1/BcryptMontoya",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/cyal1/BcryptRpcServer/tree/main/python",
     py_modules=['BcryptRpcServer'],
     install_requires=[
-        "grpc==1.0.0",
+        "grpcio-tools==1.54.2",
         "grpcio==1.54.2",
         "protobuf==4.23.2"
         ],
     classifiers=[
         # "Topic :: Software Development :: Libraries :: Python Modules",
         # "Programming Language :: Python",
         # "Programming Language :: Python :: 3",
```

