# Comparing `tmp/bohrium-sdk-0.2.1.tar.gz` & `tmp/bohrium-sdk-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bohrium-sdk-0.2.1.tar", last modified: Tue Jun 13 02:16:55 2023, max compression
+gzip compressed data, was "bohrium-sdk-0.2.2.tar", last modified: Tue Jun 13 03:50:37 2023, max compression
```

## Comparing `bohrium-sdk-0.2.1.tar` & `bohrium-sdk-0.2.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-06-13 02:16:55.973595 bohrium-sdk-0.2.1/
--rw-r--r--   0 dingzhaohan   (501) staff       (20)      205 2023-06-13 02:16:55.973389 bohrium-sdk-0.2.1/PKG-INFO
--rw-r--r--   0 dingzhaohan   (501) staff       (20)       56 2023-05-16 07:10:39.000000 bohrium-sdk-0.2.1/README.md
-drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-06-13 02:16:55.965277 bohrium-sdk-0.2.1/bohrium_sdk.egg-info/
--rw-r--r--   0 dingzhaohan   (501) staff       (20)      205 2023-06-13 02:16:55.000000 bohrium-sdk-0.2.1/bohrium_sdk.egg-info/PKG-INFO
--rw-r--r--   0 dingzhaohan   (501) staff       (20)      444 2023-06-13 02:16:55.000000 bohrium-sdk-0.2.1/bohrium_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 dingzhaohan   (501) staff       (20)        1 2023-06-13 02:16:55.000000 bohrium-sdk-0.2.1/bohrium_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 dingzhaohan   (501) staff       (20)       11 2023-06-13 02:16:55.000000 bohrium-sdk-0.2.1/bohrium_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-06-13 02:16:55.971691 bohrium-sdk-0.2.1/bohriumsdk/
--rw-r--r--   0 dingzhaohan   (501) staff       (20)      123 2023-05-16 07:22:01.000000 bohrium-sdk-0.2.1/bohriumsdk/__init__.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)        0 2023-05-29 08:11:22.000000 bohrium-sdk-0.2.1/bohriumsdk/__main__.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     6809 2023-06-13 02:16:30.000000 bohrium-sdk-0.2.1/bohriumsdk/client.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     1737 2023-06-08 02:50:49.000000 bohrium-sdk-0.2.1/bohriumsdk/database.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     1965 2023-06-12 09:26:10.000000 bohrium-sdk-0.2.1/bohriumsdk/image.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     4119 2023-06-12 09:25:17.000000 bohrium-sdk-0.2.1/bohriumsdk/job.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     2159 2023-05-30 07:06:38.000000 bohrium-sdk-0.2.1/bohriumsdk/node.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     2213 2023-06-12 09:26:00.000000 bohrium-sdk-0.2.1/bohriumsdk/project.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     7809 2023-06-13 01:39:50.000000 bohrium-sdk-0.2.1/bohriumsdk/storage.py
-drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-06-13 02:16:55.972922 bohrium-sdk-0.2.1/bohriumsdk/test/
--rw-r--r--   0 dingzhaohan   (501) staff       (20)        0 2023-05-29 08:09:08.000000 bohrium-sdk-0.2.1/bohriumsdk/test/__init__.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)       80 2023-05-29 08:13:02.000000 bohrium-sdk-0.2.1/bohriumsdk/test/test_node.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     4467 2023-06-13 01:43:50.000000 bohrium-sdk-0.2.1/bohriumsdk/test.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     4751 2023-06-07 01:28:13.000000 bohrium-sdk-0.2.1/bohriumsdk/util.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)       38 2023-06-13 02:16:55.973641 bohrium-sdk-0.2.1/setup.cfg
--rw-r--r--   0 dingzhaohan   (501) staff       (20)      366 2023-06-13 02:16:50.000000 bohrium-sdk-0.2.1/setup.py
+drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-06-13 03:50:37.492877 bohrium-sdk-0.2.2/
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)      205 2023-06-13 03:50:37.491337 bohrium-sdk-0.2.2/PKG-INFO
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)       56 2023-05-16 07:10:39.000000 bohrium-sdk-0.2.2/README.md
+drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-06-13 03:50:37.473142 bohrium-sdk-0.2.2/bohrium_sdk.egg-info/
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)      205 2023-06-13 03:50:37.000000 bohrium-sdk-0.2.2/bohrium_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)      444 2023-06-13 03:50:37.000000 bohrium-sdk-0.2.2/bohrium_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)        1 2023-06-13 03:50:37.000000 bohrium-sdk-0.2.2/bohrium_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)       11 2023-06-13 03:50:37.000000 bohrium-sdk-0.2.2/bohrium_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-06-13 03:50:37.486495 bohrium-sdk-0.2.2/bohriumsdk/
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)      123 2023-05-16 07:22:01.000000 bohrium-sdk-0.2.2/bohriumsdk/__init__.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)        0 2023-05-29 08:11:22.000000 bohrium-sdk-0.2.2/bohriumsdk/__main__.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     6887 2023-06-13 03:47:27.000000 bohrium-sdk-0.2.2/bohriumsdk/client.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     1737 2023-06-08 02:50:49.000000 bohrium-sdk-0.2.2/bohriumsdk/database.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     1965 2023-06-12 09:26:10.000000 bohrium-sdk-0.2.2/bohriumsdk/image.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     4119 2023-06-12 09:25:17.000000 bohrium-sdk-0.2.2/bohriumsdk/job.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     2159 2023-05-30 07:06:38.000000 bohrium-sdk-0.2.2/bohriumsdk/node.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     2213 2023-06-12 09:26:00.000000 bohrium-sdk-0.2.2/bohriumsdk/project.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     7809 2023-06-13 01:39:50.000000 bohrium-sdk-0.2.2/bohriumsdk/storage.py
+drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-06-13 03:50:37.490027 bohrium-sdk-0.2.2/bohriumsdk/test/
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)        0 2023-05-29 08:09:08.000000 bohrium-sdk-0.2.2/bohriumsdk/test/__init__.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)       80 2023-05-29 08:13:02.000000 bohrium-sdk-0.2.2/bohriumsdk/test/test_node.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     4467 2023-06-13 01:43:50.000000 bohrium-sdk-0.2.2/bohriumsdk/test.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     4751 2023-06-07 01:28:13.000000 bohrium-sdk-0.2.2/bohriumsdk/util.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)       38 2023-06-13 03:50:37.492981 bohrium-sdk-0.2.2/setup.cfg
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)      366 2023-06-13 03:48:26.000000 bohrium-sdk-0.2.2/setup.py
```

### Comparing `bohrium-sdk-0.2.1/bohriumsdk/client.py` & `bohrium-sdk-0.2.2/bohriumsdk/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import os
 import json
 import urllib
 import getpass
 import time
 import configparser
 import re
+import sys
 
 class RequestInfoException(Exception):
     pass
 
 class Client:
     def __init__(
             self, 
@@ -54,15 +55,14 @@
                 data = f"[Credentials]\nbaseUrl=https://openapi.dp.tech\naccessKey={self.access_key}"
                 with open(self.config_file_location_expand, 'w') as f:
                     f.write(data)
             config = configparser.ConfigParser()
             config.read(self.config_file_location_expand)
             self.base_url = config.get('Credentials', 'baseUrl')
             self.access_key = config.get('Credentials', 'accessKey')
-            # print(self.access_key)
             self.params = {"accessKey": self.access_key}
             self.token = ""
             self.check_ak()
             
 
     def post(self, url, host="", json=None, data=None, headers=None, params=None, stream=False, retry=5):
         return self._req('POST', url, host=host, json=json, data=data, headers=headers, params=params, stream=stream, retry=retry)
@@ -91,15 +91,15 @@
                 resp = requests.get(url=url, params=params, headers=headers, stream=stream)
             if method == 'POST':
                 resp = requests.post(url=url, json=json, data=data, params=params, headers=headers, stream=stream)
             resp_code = resp.status_code
             if resp_code == 401:
                 os.remove(self.config_file_location_expand)
                 print("Config file(~/.brmconfig) AccessKey invalid! Visit https://bohrium.dp.tech/personal/setting to generate it! ")
-                exit()
+                sys.exit()
             if not resp.ok:
                 try:
                     result = resp.json()
                     err = result.get("error")
                 except:
                     pass
                 time.sleep(0.1 * i)
@@ -112,21 +112,23 @@
             elif result['code'] == 0:
                 return result.get('data', {})
             else:
                 err = result.get("message") or result.get("error")
                 break
         raise RequestInfoException(resp_code, url, err)
 
-    def get_token(self):
-        self.login()
-        return self.token
+    # def get_token(self):
+    #     self.login()
+    #     return self.token
 
     def check_ak(self):
         url = f"/openapi/v1/ak/get"
         resp = self.get(url=url, params=self.params)
+        if resp.get("user_id", 0) != 0:
+            print("AccessKey authorization passed! ")
         return resp
 
     # def login(self):
     #     email = input("Please enter Bohrium Account Email: ")
     #     password = getpass.getpass(prompt="Please enter password: ")
     #     post_data = {
     #         'username': email,
```

### Comparing `bohrium-sdk-0.2.1/bohriumsdk/database.py` & `bohrium-sdk-0.2.2/bohriumsdk/database.py`

 * *Files identical despite different names*

### Comparing `bohrium-sdk-0.2.1/bohriumsdk/image.py` & `bohrium-sdk-0.2.2/bohriumsdk/image.py`

 * *Files identical despite different names*

### Comparing `bohrium-sdk-0.2.1/bohriumsdk/job.py` & `bohrium-sdk-0.2.2/bohriumsdk/job.py`

 * *Files identical despite different names*

### Comparing `bohrium-sdk-0.2.1/bohriumsdk/node.py` & `bohrium-sdk-0.2.2/bohriumsdk/node.py`

 * *Files identical despite different names*

### Comparing `bohrium-sdk-0.2.1/bohriumsdk/project.py` & `bohrium-sdk-0.2.2/bohriumsdk/project.py`

 * *Files identical despite different names*

### Comparing `bohrium-sdk-0.2.1/bohriumsdk/storage.py` & `bohrium-sdk-0.2.2/bohriumsdk/storage.py`

 * *Files identical despite different names*

### Comparing `bohrium-sdk-0.2.1/bohriumsdk/test.py` & `bohrium-sdk-0.2.2/bohriumsdk/test.py`

 * *Files identical despite different names*

### Comparing `bohrium-sdk-0.2.1/bohriumsdk/util.py` & `bohrium-sdk-0.2.2/bohriumsdk/util.py`

 * *Files identical despite different names*

