# Comparing `tmp/async-http-requests-0.0.2.tar.gz` & `tmp/async-http-requests-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async-http-requests-0.0.2.tar", last modified: Thu Jun  1 14:24:08 2023, max compression
+gzip compressed data, was "async-http-requests-0.0.3.tar", last modified: Tue Jun 13 19:56:40 2023, max compression
```

## Comparing `async-http-requests-0.0.2.tar` & `async-http-requests-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 andreasergi  (1000) andreasergi  (1000)        0 2023-06-01 14:24:08.582024 async-http-requests-0.0.2/
--rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)     1078 2023-04-13 10:12:28.000000 async-http-requests-0.0.2/LICENSE
--rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)       17 2023-04-14 15:28:46.000000 async-http-requests-0.0.2/MANIFEST.in
--rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)     5148 2023-06-01 14:24:08.582024 async-http-requests-0.0.2/PKG-INFO
--rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)     3413 2023-04-16 16:58:44.000000 async-http-requests-0.0.2/README.md
--rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)      858 2023-05-31 11:31:14.000000 async-http-requests-0.0.2/pyproject.toml
--rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)       38 2023-06-01 14:24:08.582024 async-http-requests-0.0.2/setup.cfg
--rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)       38 2023-04-13 22:04:33.000000 async-http-requests-0.0.2/setup.py
-drwxrwxr-x   0 andreasergi  (1000) andreasergi  (1000)        0 2023-06-01 14:24:08.578024 async-http-requests-0.0.2/src/
--rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)     5741 2023-06-01 13:29:55.000000 async-http-requests-0.0.2/src/AsyncRequests.py
--rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)      608 2023-04-14 09:22:32.000000 async-http-requests-0.0.2/src/RequestObject.py
--rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)      476 2023-04-14 10:05:37.000000 async-http-requests-0.0.2/src/RequestsType.py
-drwxrwxr-x   0 andreasergi  (1000) andreasergi  (1000)        0 2023-06-01 14:24:08.582024 async-http-requests-0.0.2/src/async_http_requests.egg-info/
--rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)     5148 2023-06-01 14:24:08.000000 async-http-requests-0.0.2/src/async_http_requests.egg-info/PKG-INFO
--rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)      376 2023-06-01 14:24:08.000000 async-http-requests-0.0.2/src/async_http_requests.egg-info/SOURCES.txt
--rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)        1 2023-06-01 14:24:08.000000 async-http-requests-0.0.2/src/async_http_requests.egg-info/dependency_links.txt
--rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)      100 2023-06-01 14:24:08.000000 async-http-requests-0.0.2/src/async_http_requests.egg-info/requires.txt
--rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)       48 2023-06-01 14:24:08.000000 async-http-requests-0.0.2/src/async_http_requests.egg-info/top_level.txt
--rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)      459 2023-04-13 16:22:15.000000 async-http-requests-0.0.2/src/helper.py
-drwxrwxr-x   0 andreasergi  (1000) andreasergi  (1000)        0 2023-06-01 14:24:08.582024 async-http-requests-0.0.2/test/
--rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)     1625 2023-06-01 13:32:21.000000 async-http-requests-0.0.2/test/test.py
+drwxrwxr-x   0 andreasergi  (1000) andreasergi  (1000)        0 2023-06-13 19:56:40.077345 async-http-requests-0.0.3/
+-rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)     1078 2023-04-13 10:12:28.000000 async-http-requests-0.0.3/LICENSE
+-rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)       17 2023-04-14 15:28:46.000000 async-http-requests-0.0.3/MANIFEST.in
+-rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)     5148 2023-06-13 19:56:40.077345 async-http-requests-0.0.3/PKG-INFO
+-rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)     3413 2023-04-16 16:58:44.000000 async-http-requests-0.0.3/README.md
+-rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)      858 2023-06-13 19:55:59.000000 async-http-requests-0.0.3/pyproject.toml
+-rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)       38 2023-06-13 19:56:40.077345 async-http-requests-0.0.3/setup.cfg
+-rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)       38 2023-04-13 22:04:33.000000 async-http-requests-0.0.3/setup.py
+drwxrwxr-x   0 andreasergi  (1000) andreasergi  (1000)        0 2023-06-13 19:56:40.077345 async-http-requests-0.0.3/src/
+-rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)     5772 2023-06-13 19:52:26.000000 async-http-requests-0.0.3/src/AsyncRequests.py
+-rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)      608 2023-04-14 09:22:32.000000 async-http-requests-0.0.3/src/RequestObject.py
+-rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)      476 2023-04-14 10:05:37.000000 async-http-requests-0.0.3/src/RequestsType.py
+drwxrwxr-x   0 andreasergi  (1000) andreasergi  (1000)        0 2023-06-13 19:56:40.077345 async-http-requests-0.0.3/src/async_http_requests.egg-info/
+-rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)     5148 2023-06-13 19:56:40.000000 async-http-requests-0.0.3/src/async_http_requests.egg-info/PKG-INFO
+-rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)      376 2023-06-13 19:56:40.000000 async-http-requests-0.0.3/src/async_http_requests.egg-info/SOURCES.txt
+-rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)        1 2023-06-13 19:56:40.000000 async-http-requests-0.0.3/src/async_http_requests.egg-info/dependency_links.txt
+-rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)      100 2023-06-13 19:56:40.000000 async-http-requests-0.0.3/src/async_http_requests.egg-info/requires.txt
+-rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)       48 2023-06-13 19:56:40.000000 async-http-requests-0.0.3/src/async_http_requests.egg-info/top_level.txt
+-rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)      459 2023-04-13 16:22:15.000000 async-http-requests-0.0.3/src/helper.py
+drwxrwxr-x   0 andreasergi  (1000) andreasergi  (1000)        0 2023-06-13 19:56:40.077345 async-http-requests-0.0.3/test/
+-rw-rw-r--   0 andreasergi  (1000) andreasergi  (1000)     1701 2023-06-11 16:58:44.000000 async-http-requests-0.0.3/test/test.py
```

### Comparing `async-http-requests-0.0.2/LICENSE` & `async-http-requests-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `async-http-requests-0.0.2/PKG-INFO` & `async-http-requests-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async-http-requests
-Version: 0.0.2
+Version: 0.0.3
 Summary: Asynchronous HTTP requests
 Author-email: Andrea Sergi <andrea.serg1@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 sclash - Andrea Sergi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `async-http-requests-0.0.2/README.md` & `async-http-requests-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `async-http-requests-0.0.2/pyproject.toml` & `async-http-requests-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "async-http-requests"
-version = "0.0.2"
+version = "0.0.3"
 description = "Asynchronous HTTP requests"
 readme = "README.md"
 authors = [{ name = "Andrea Sergi", email = "andrea.serg1@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `async-http-requests-0.0.2/src/AsyncRequests.py` & `async-http-requests-0.0.3/src/AsyncRequests.py`

 * *Files 4% similar despite different names*

```diff
@@ -99,16 +99,16 @@
         
         await self.queue.join()
         for c in consumers:
             c.cancel()
 
         if len(self.error_response) > 0:
             self.error_data = pd.DataFrame()
-            for err in self.error_response:
-                self.error_data = pd.concat([self.error_data, pd.DataFrame(asdict(err)) ])
+            for idx, err in enumerate(self.error_response):
+                self.error_data = pd.concat([self.error_data, pd.DataFrame(asdict(err), index = [idx]) ])
                 
 
 class AsyncHTTP(AsyncRequests):
 
     def __init__(self, url: List[RequestObject], N_PRODUCERS, N_CONSUMERS):
         super().__init__(url, N_PRODUCERS, N_CONSUMERS)
```

### Comparing `async-http-requests-0.0.2/src/RequestObject.py` & `async-http-requests-0.0.3/src/RequestObject.py`

 * *Files identical despite different names*

### Comparing `async-http-requests-0.0.2/src/async_http_requests.egg-info/PKG-INFO` & `async-http-requests-0.0.3/src/async_http_requests.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async-http-requests
-Version: 0.0.2
+Version: 0.0.3
 Summary: Asynchronous HTTP requests
 Author-email: Andrea Sergi <andrea.serg1@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 sclash - Andrea Sergi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `async-http-requests-0.0.2/test/test.py` & `async-http-requests-0.0.3/test/test.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 
 api = 'https://api.publicapis.org/entries'
 headers = {'user-agent':'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/110.0.0.0 Safari/537.36'}
 
 
 endpoints = [RequestObject(url = api, params = {"title":"cat"}),
              RequestObject(url = api, params = {"title":"dog"}),
-             RequestObject(url = 'https://fuckweb.com/', params = {"title":"fica"}),
+             RequestObject(url = 'http://fnkudshgjdfjgbfdk.com/', params = {"title":"fkhsudh"}), # should return an error
              RequestObject(url = api, params = {"title":"house"}),
              RequestObject(url = api, params = {"title":"weath"}),
-             RequestObject(url = 'https://fuckweb.com/', params = {"title":"cazzo"}),
+             RequestObject(url = 'http://fnkudshgjdfjgbfdk.com/', params = {"title":"nfusdhif"}), #should return an error
              RequestObject(url = api, params = {"title":"py"})]
              
 
 a = AsyncHTTP(
     url = endpoints,
     N_PRODUCERS=5,
     N_CONSUMERS=5
@@ -49,15 +49,15 @@
 end = perf_counter()
 print(f"Sync EXECUTION TIME: {end-start}")
 
 len(a.response)
 
 
 
-requests.get(url = api , params = {"tile":"cazzo"})
+requests.get(url = api , params = {"tile":"sdvdfssf"})
 
 
 
 # import pandas as pd
 # from dataclasses import asdict
 err = a.error_response
 # df = pd.DataFrame()
```

