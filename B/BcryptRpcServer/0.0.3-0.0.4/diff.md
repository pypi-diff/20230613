# Comparing `tmp/BcryptRpcServer-0.0.3.tar.gz` & `tmp/BcryptRpcServer-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BcryptRpcServer-0.0.3.tar", last modified: Tue Jun 13 06:21:21 2023, max compression
+gzip compressed data, was "BcryptRpcServer-0.0.4.tar", last modified: Tue Jun 13 06:43:04 2023, max compression
```

## Comparing `BcryptRpcServer-0.0.3.tar` & `BcryptRpcServer-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,14 @@
-drwxr-xr-x   0 cyal1      (501) wheel        (0)        0 2023-06-13 06:21:21.804143 BcryptRpcServer-0.0.3/
-drwxr-xr-x   0 cyal1      (501) wheel        (0)        0 2023-06-13 06:21:21.803094 BcryptRpcServer-0.0.3/BcryptRpcServer/
--rw-r--r--   0 cyal1      (501) wheel        (0)     3449 2023-06-13 06:19:38.000000 BcryptRpcServer-0.0.3/BcryptRpcServer/BcryptRpcServer.py
--rw-r--r--   0 cyal1      (501) wheel        (0)        1 2023-06-13 06:20:57.000000 BcryptRpcServer-0.0.3/BcryptRpcServer/__init__.py
--rw-r--r--   0 cyal1      (501) wheel        (0)     1427 2023-06-13 06:19:38.000000 BcryptRpcServer-0.0.3/BcryptRpcServer/burpextender_pb2.py
--rw-r--r--   0 cyal1      (501) wheel        (0)     2416 2023-06-13 06:19:38.000000 BcryptRpcServer-0.0.3/BcryptRpcServer/burpextender_pb2_grpc.py
-drwxr-xr-x   0 cyal1      (501) wheel        (0)        0 2023-06-13 06:21:21.803821 BcryptRpcServer-0.0.3/BcryptRpcServer.egg-info/
--rw-r--r--   0 cyal1      (501) wheel        (0)     1587 2023-06-13 06:21:21.000000 BcryptRpcServer-0.0.3/BcryptRpcServer.egg-info/PKG-INFO
--rw-r--r--   0 cyal1      (501) wheel        (0)      352 2023-06-13 06:21:21.000000 BcryptRpcServer-0.0.3/BcryptRpcServer.egg-info/SOURCES.txt
--rw-r--r--   0 cyal1      (501) wheel        (0)        1 2023-06-13 06:21:21.000000 BcryptRpcServer-0.0.3/BcryptRpcServer.egg-info/dependency_links.txt
--rw-r--r--   0 cyal1      (501) wheel        (0)       53 2023-06-13 06:21:21.000000 BcryptRpcServer-0.0.3/BcryptRpcServer.egg-info/requires.txt
--rw-r--r--   0 cyal1      (501) wheel        (0)       16 2023-06-13 06:21:21.000000 BcryptRpcServer-0.0.3/BcryptRpcServer.egg-info/top_level.txt
--rw-r--r--   0 cyal1      (501) wheel        (0)     1587 2023-06-13 06:21:21.803998 BcryptRpcServer-0.0.3/PKG-INFO
--rw-r--r--   0 cyal1      (501) wheel        (0)     1302 2023-06-13 06:19:38.000000 BcryptRpcServer-0.0.3/README.md
--rw-r--r--   0 cyal1      (501) wheel        (0)       38 2023-06-13 06:21:21.804182 BcryptRpcServer-0.0.3/setup.cfg
--rw-r--r--   0 cyal1      (501) wheel        (0)     1389 2023-06-13 06:21:18.000000 BcryptRpcServer-0.0.3/setup.py
+drwxr-xr-x   0 cyal1      (501) wheel        (0)        0 2023-06-13 06:43:04.185930 BcryptRpcServer-0.0.4/
+drwxr-xr-x   0 cyal1      (501) wheel        (0)        0 2023-06-13 06:43:04.185642 BcryptRpcServer-0.0.4/BcryptRpcServer.egg-info/
+-rw-r--r--   0 cyal1      (501) wheel        (0)     1628 2023-06-13 06:43:04.000000 BcryptRpcServer-0.0.4/BcryptRpcServer.egg-info/PKG-INFO
+-rw-r--r--   0 cyal1      (501) wheel        (0)      276 2023-06-13 06:43:04.000000 BcryptRpcServer-0.0.4/BcryptRpcServer.egg-info/SOURCES.txt
+-rw-r--r--   0 cyal1      (501) wheel        (0)        1 2023-06-13 06:43:04.000000 BcryptRpcServer-0.0.4/BcryptRpcServer.egg-info/dependency_links.txt
+-rw-r--r--   0 cyal1      (501) wheel        (0)       53 2023-06-13 06:43:04.000000 BcryptRpcServer-0.0.4/BcryptRpcServer.egg-info/requires.txt
+-rw-r--r--   0 cyal1      (501) wheel        (0)       55 2023-06-13 06:43:04.000000 BcryptRpcServer-0.0.4/BcryptRpcServer.egg-info/top_level.txt
+-rw-r--r--   0 cyal1      (501) wheel        (0)     3449 2023-06-13 06:19:38.000000 BcryptRpcServer-0.0.4/BcryptRpcServer.py
+-rw-r--r--   0 cyal1      (501) wheel        (0)     1628 2023-06-13 06:43:04.185799 BcryptRpcServer-0.0.4/PKG-INFO
+-rw-r--r--   0 cyal1      (501) wheel        (0)     1343 2023-06-13 06:41:56.000000 BcryptRpcServer-0.0.4/README.md
+-rw-r--r--   0 cyal1      (501) wheel        (0)     1427 2023-06-13 06:19:38.000000 BcryptRpcServer-0.0.4/burpextender_pb2.py
+-rw-r--r--   0 cyal1      (501) wheel        (0)     2416 2023-06-13 06:19:38.000000 BcryptRpcServer-0.0.4/burpextender_pb2_grpc.py
+-rw-r--r--   0 cyal1      (501) wheel        (0)       38 2023-06-13 06:43:04.185966 BcryptRpcServer-0.0.4/setup.cfg
+-rw-r--r--   0 cyal1      (501) wheel        (0)      834 2023-06-13 06:42:23.000000 BcryptRpcServer-0.0.4/setup.py
```

### Comparing `BcryptRpcServer-0.0.3/BcryptRpcServer/BcryptRpcServer.py` & `BcryptRpcServer-0.0.4/BcryptRpcServer.py`

 * *Files identical despite different names*

### Comparing `BcryptRpcServer-0.0.3/BcryptRpcServer/burpextender_pb2.py` & `BcryptRpcServer-0.0.4/burpextender_pb2.py`

 * *Files identical despite different names*

### Comparing `BcryptRpcServer-0.0.3/BcryptRpcServer/burpextender_pb2_grpc.py` & `BcryptRpcServer-0.0.4/burpextender_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `BcryptRpcServer-0.0.3/BcryptRpcServer.egg-info/PKG-INFO` & `BcryptRpcServer-0.0.4/BcryptRpcServer.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 Metadata-Version: 2.1
 Name: BcryptRpcServer
-Version: 0.0.3
+Version: 0.0.4
 Summary: The rpc server api of https://github.com/cyal1/BcryptMontoya
 Home-page: https://github.com/cyal1/BcryptRpcServer/tree/main/python
 Author: cyal1
 Author-email: admin@example.com
 Description-Content-Type: text/markdown
 
 # BcryptRpcServer
 
+## install 
+pip install BcryptRpcServer
+
 ## Basic
 ```python
 import BcryptRpcServer 
 
 def test(a,b,c,d,e):
     print(a,type(a),b,type(b),c,type(c),d,type(d),e,type(e))
     return b'asdf'
```

### Comparing `BcryptRpcServer-0.0.3/PKG-INFO` & `BcryptRpcServer-0.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 Metadata-Version: 2.1
 Name: BcryptRpcServer
-Version: 0.0.3
+Version: 0.0.4
 Summary: The rpc server api of https://github.com/cyal1/BcryptMontoya
 Home-page: https://github.com/cyal1/BcryptRpcServer/tree/main/python
 Author: cyal1
 Author-email: admin@example.com
 Description-Content-Type: text/markdown
 
 # BcryptRpcServer
 
+## install 
+pip install BcryptRpcServer
+
 ## Basic
 ```python
 import BcryptRpcServer 
 
 def test(a,b,c,d,e):
     print(a,type(a),b,type(b),c,type(c),d,type(d),e,type(e))
     return b'asdf'
```

### Comparing `BcryptRpcServer-0.0.3/README.md` & `BcryptRpcServer-0.0.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 # BcryptRpcServer
 
+## install 
+pip install BcryptRpcServer
+
 ## Basic
 ```python
 import BcryptRpcServer 
 
 def test(a,b,c,d,e):
     print(a,type(a),b,type(b),c,type(c),d,type(d),e,type(e))
     return b'asdf'
```

