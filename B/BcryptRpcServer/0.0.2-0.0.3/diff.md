# Comparing `tmp/BcryptRpcServer-0.0.2.tar.gz` & `tmp/BcryptRpcServer-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BcryptRpcServer-0.0.2.tar", last modified: Tue Jun 13 05:54:27 2023, max compression
+gzip compressed data, was "BcryptRpcServer-0.0.3.tar", last modified: Tue Jun 13 06:21:21 2023, max compression
```

## Comparing `BcryptRpcServer-0.0.2.tar` & `BcryptRpcServer-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,16 @@
-drwxr-xr-x   0 cyal1      (501) wheel        (0)        0 2023-06-13 05:54:27.040069 BcryptRpcServer-0.0.2/
-drwxr-xr-x   0 cyal1      (501) wheel        (0)        0 2023-06-13 05:54:27.039762 BcryptRpcServer-0.0.2/BcryptRpcServer.egg-info/
--rw-r--r--   0 cyal1      (501) wheel        (0)     1686 2023-06-13 05:54:27.000000 BcryptRpcServer-0.0.2/BcryptRpcServer.egg-info/PKG-INFO
--rw-r--r--   0 cyal1      (501) wheel        (0)      231 2023-06-13 05:54:27.000000 BcryptRpcServer-0.0.2/BcryptRpcServer.egg-info/SOURCES.txt
--rw-r--r--   0 cyal1      (501) wheel        (0)        1 2023-06-13 05:54:27.000000 BcryptRpcServer-0.0.2/BcryptRpcServer.egg-info/dependency_links.txt
--rw-r--r--   0 cyal1      (501) wheel        (0)       53 2023-06-13 05:54:27.000000 BcryptRpcServer-0.0.2/BcryptRpcServer.egg-info/requires.txt
--rw-r--r--   0 cyal1      (501) wheel        (0)       16 2023-06-13 05:54:27.000000 BcryptRpcServer-0.0.2/BcryptRpcServer.egg-info/top_level.txt
--rw-r--r--   0 cyal1      (501) wheel        (0)     3470 2023-06-13 05:54:16.000000 BcryptRpcServer-0.0.2/BcryptRpcServer.py
--rw-r--r--   0 cyal1      (501) wheel        (0)     1686 2023-06-13 05:54:27.039933 BcryptRpcServer-0.0.2/PKG-INFO
--rw-r--r--   0 cyal1      (501) wheel        (0)     1401 2023-06-13 04:52:23.000000 BcryptRpcServer-0.0.2/README.md
--rw-r--r--   0 cyal1      (501) wheel        (0)       38 2023-06-13 05:54:27.040109 BcryptRpcServer-0.0.2/setup.cfg
--rw-r--r--   0 cyal1      (501) wheel        (0)     1378 2023-06-13 05:50:23.000000 BcryptRpcServer-0.0.2/setup.py
+drwxr-xr-x   0 cyal1      (501) wheel        (0)        0 2023-06-13 06:21:21.804143 BcryptRpcServer-0.0.3/
+drwxr-xr-x   0 cyal1      (501) wheel        (0)        0 2023-06-13 06:21:21.803094 BcryptRpcServer-0.0.3/BcryptRpcServer/
+-rw-r--r--   0 cyal1      (501) wheel        (0)     3449 2023-06-13 06:19:38.000000 BcryptRpcServer-0.0.3/BcryptRpcServer/BcryptRpcServer.py
+-rw-r--r--   0 cyal1      (501) wheel        (0)        1 2023-06-13 06:20:57.000000 BcryptRpcServer-0.0.3/BcryptRpcServer/__init__.py
+-rw-r--r--   0 cyal1      (501) wheel        (0)     1427 2023-06-13 06:19:38.000000 BcryptRpcServer-0.0.3/BcryptRpcServer/burpextender_pb2.py
+-rw-r--r--   0 cyal1      (501) wheel        (0)     2416 2023-06-13 06:19:38.000000 BcryptRpcServer-0.0.3/BcryptRpcServer/burpextender_pb2_grpc.py
+drwxr-xr-x   0 cyal1      (501) wheel        (0)        0 2023-06-13 06:21:21.803821 BcryptRpcServer-0.0.3/BcryptRpcServer.egg-info/
+-rw-r--r--   0 cyal1      (501) wheel        (0)     1587 2023-06-13 06:21:21.000000 BcryptRpcServer-0.0.3/BcryptRpcServer.egg-info/PKG-INFO
+-rw-r--r--   0 cyal1      (501) wheel        (0)      352 2023-06-13 06:21:21.000000 BcryptRpcServer-0.0.3/BcryptRpcServer.egg-info/SOURCES.txt
+-rw-r--r--   0 cyal1      (501) wheel        (0)        1 2023-06-13 06:21:21.000000 BcryptRpcServer-0.0.3/BcryptRpcServer.egg-info/dependency_links.txt
+-rw-r--r--   0 cyal1      (501) wheel        (0)       53 2023-06-13 06:21:21.000000 BcryptRpcServer-0.0.3/BcryptRpcServer.egg-info/requires.txt
+-rw-r--r--   0 cyal1      (501) wheel        (0)       16 2023-06-13 06:21:21.000000 BcryptRpcServer-0.0.3/BcryptRpcServer.egg-info/top_level.txt
+-rw-r--r--   0 cyal1      (501) wheel        (0)     1587 2023-06-13 06:21:21.803998 BcryptRpcServer-0.0.3/PKG-INFO
+-rw-r--r--   0 cyal1      (501) wheel        (0)     1302 2023-06-13 06:19:38.000000 BcryptRpcServer-0.0.3/README.md
+-rw-r--r--   0 cyal1      (501) wheel        (0)       38 2023-06-13 06:21:21.804182 BcryptRpcServer-0.0.3/setup.cfg
+-rw-r--r--   0 cyal1      (501) wheel        (0)     1389 2023-06-13 06:21:18.000000 BcryptRpcServer-0.0.3/setup.py
```

### Comparing `BcryptRpcServer-0.0.2/BcryptRpcServer.egg-info/PKG-INFO` & `BcryptRpcServer-0.0.3/BcryptRpcServer.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 Metadata-Version: 2.1
 Name: BcryptRpcServer
-Version: 0.0.2
+Version: 0.0.3
 Summary: The rpc server api of https://github.com/cyal1/BcryptMontoya
 Home-page: https://github.com/cyal1/BcryptRpcServer/tree/main/python
 Author: cyal1
 Author-email: admin@example.com
 Description-Content-Type: text/markdown
 
 # BcryptRpcServer
-The rpc server of https://github.com/cyal1/BcryptMontoya
-
-## install
-`pip install BcryptRpcServer`
 
 ## Basic
 ```python
 import BcryptRpcServer 
 
 def test(a,b,c,d,e):
     print(a,type(a),b,type(b),c,type(c),d,type(d),e,type(e))
```

### Comparing `BcryptRpcServer-0.0.2/BcryptRpcServer.py` & `BcryptRpcServer-0.0.3/BcryptRpcServer/BcryptRpcServer.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import google.protobuf.any_pb2 as any_pb2
 from google.protobuf.wrappers_pb2 import *
 import burpextender_pb2 as pb2
 from concurrent import futures
 import burpextender_pb2_grpc as pb2_grpc
 
 
-__version__ = '0.0.2'
+
 function_registry = {}
 
 def expose(func):
     function_registry[func.__name__] = func
 
 class CallFuncServicer(pb2_grpc.CallFuncServiceServicer):
     def CallFunc(self, request, context):
```

### Comparing `BcryptRpcServer-0.0.2/PKG-INFO` & `BcryptRpcServer-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 Metadata-Version: 2.1
 Name: BcryptRpcServer
-Version: 0.0.2
+Version: 0.0.3
 Summary: The rpc server api of https://github.com/cyal1/BcryptMontoya
 Home-page: https://github.com/cyal1/BcryptRpcServer/tree/main/python
 Author: cyal1
 Author-email: admin@example.com
 Description-Content-Type: text/markdown
 
 # BcryptRpcServer
-The rpc server of https://github.com/cyal1/BcryptMontoya
-
-## install
-`pip install BcryptRpcServer`
 
 ## Basic
 ```python
 import BcryptRpcServer 
 
 def test(a,b,c,d,e):
     print(a,type(a),b,type(b),c,type(c),d,type(d),e,type(e))
```

### Comparing `BcryptRpcServer-0.0.2/README.md` & `BcryptRpcServer-0.0.3/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,8 @@
 # BcryptRpcServer
-The rpc server of https://github.com/cyal1/BcryptMontoya
-
-## install
-`pip install BcryptRpcServer`
 
 ## Basic
 ```python
 import BcryptRpcServer 
 
 def test(a,b,c,d,e):
     print(a,type(a),b,type(b),c,type(c),d,type(d),e,type(e))
```

### Comparing `BcryptRpcServer-0.0.2/setup.py` & `BcryptRpcServer-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,17 @@
 import BcryptRpcServer
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name="BcryptRpcServer",
-    version=BcryptRpcServer.__version__,
+    version="0.0.3",
     author="cyal1",
+    packages=find_packages(),
     author_email="admin@example.com",
     description="The rpc server api of https://github.com/cyal1/BcryptMontoya",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/cyal1/BcryptRpcServer/tree/main/python",
     py_modules=['BcryptRpcServer'],
     install_requires=[
@@ -32,7 +33,8 @@
         # "Programming Language :: Python :: 3.7",
         # "Programming Language :: Python :: 3.8",
         # "Programming Language :: Python :: 3.9",
         # "Programming Language :: Python :: 3.10",
         # 'Programming Language :: Python :: Implementation :: CPython',
     ],
 )
+
```

