# Comparing `tmp/bohrium-sdk-0.2.0.tar.gz` & `tmp/bohrium-sdk-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bohrium-sdk-0.2.0.tar", last modified: Tue Jun 13 02:14:56 2023, max compression
+gzip compressed data, was "bohrium-sdk-0.2.1.tar", last modified: Tue Jun 13 02:16:55 2023, max compression
```

## Comparing `bohrium-sdk-0.2.0.tar` & `bohrium-sdk-0.2.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-06-13 02:14:56.967407 bohrium-sdk-0.2.0/
--rw-r--r--   0 dingzhaohan   (501) staff       (20)      205 2023-06-13 02:14:56.967013 bohrium-sdk-0.2.0/PKG-INFO
--rw-r--r--   0 dingzhaohan   (501) staff       (20)       56 2023-05-16 07:10:39.000000 bohrium-sdk-0.2.0/README.md
-drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-06-13 02:14:56.950762 bohrium-sdk-0.2.0/bohrium_sdk.egg-info/
--rw-r--r--   0 dingzhaohan   (501) staff       (20)      205 2023-06-13 02:14:56.000000 bohrium-sdk-0.2.0/bohrium_sdk.egg-info/PKG-INFO
--rw-r--r--   0 dingzhaohan   (501) staff       (20)      444 2023-06-13 02:14:56.000000 bohrium-sdk-0.2.0/bohrium_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 dingzhaohan   (501) staff       (20)        1 2023-06-13 02:14:56.000000 bohrium-sdk-0.2.0/bohrium_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 dingzhaohan   (501) staff       (20)       11 2023-06-13 02:14:56.000000 bohrium-sdk-0.2.0/bohrium_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-06-13 02:14:56.963894 bohrium-sdk-0.2.0/bohriumsdk/
--rw-r--r--   0 dingzhaohan   (501) staff       (20)      123 2023-05-16 07:22:01.000000 bohrium-sdk-0.2.0/bohriumsdk/__init__.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)        0 2023-05-29 08:11:22.000000 bohrium-sdk-0.2.0/bohriumsdk/__main__.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     6955 2023-06-13 01:50:05.000000 bohrium-sdk-0.2.0/bohriumsdk/client.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     1737 2023-06-08 02:50:49.000000 bohrium-sdk-0.2.0/bohriumsdk/database.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     1965 2023-06-12 09:26:10.000000 bohrium-sdk-0.2.0/bohriumsdk/image.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     4119 2023-06-12 09:25:17.000000 bohrium-sdk-0.2.0/bohriumsdk/job.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     2159 2023-05-30 07:06:38.000000 bohrium-sdk-0.2.0/bohriumsdk/node.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     2213 2023-06-12 09:26:00.000000 bohrium-sdk-0.2.0/bohriumsdk/project.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     7809 2023-06-13 01:39:50.000000 bohrium-sdk-0.2.0/bohriumsdk/storage.py
-drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-06-13 02:14:56.966450 bohrium-sdk-0.2.0/bohriumsdk/test/
--rw-r--r--   0 dingzhaohan   (501) staff       (20)        0 2023-05-29 08:09:08.000000 bohrium-sdk-0.2.0/bohriumsdk/test/__init__.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)       80 2023-05-29 08:13:02.000000 bohrium-sdk-0.2.0/bohriumsdk/test/test_node.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     4467 2023-06-13 01:43:50.000000 bohrium-sdk-0.2.0/bohriumsdk/test.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     4751 2023-06-07 01:28:13.000000 bohrium-sdk-0.2.0/bohriumsdk/util.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)       38 2023-06-13 02:14:56.967690 bohrium-sdk-0.2.0/setup.cfg
--rw-r--r--   0 dingzhaohan   (501) staff       (20)      366 2023-06-13 02:14:48.000000 bohrium-sdk-0.2.0/setup.py
+drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-06-13 02:16:55.973595 bohrium-sdk-0.2.1/
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)      205 2023-06-13 02:16:55.973389 bohrium-sdk-0.2.1/PKG-INFO
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)       56 2023-05-16 07:10:39.000000 bohrium-sdk-0.2.1/README.md
+drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-06-13 02:16:55.965277 bohrium-sdk-0.2.1/bohrium_sdk.egg-info/
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)      205 2023-06-13 02:16:55.000000 bohrium-sdk-0.2.1/bohrium_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)      444 2023-06-13 02:16:55.000000 bohrium-sdk-0.2.1/bohrium_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)        1 2023-06-13 02:16:55.000000 bohrium-sdk-0.2.1/bohrium_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)       11 2023-06-13 02:16:55.000000 bohrium-sdk-0.2.1/bohrium_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-06-13 02:16:55.971691 bohrium-sdk-0.2.1/bohriumsdk/
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)      123 2023-05-16 07:22:01.000000 bohrium-sdk-0.2.1/bohriumsdk/__init__.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)        0 2023-05-29 08:11:22.000000 bohrium-sdk-0.2.1/bohriumsdk/__main__.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     6809 2023-06-13 02:16:30.000000 bohrium-sdk-0.2.1/bohriumsdk/client.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     1737 2023-06-08 02:50:49.000000 bohrium-sdk-0.2.1/bohriumsdk/database.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     1965 2023-06-12 09:26:10.000000 bohrium-sdk-0.2.1/bohriumsdk/image.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     4119 2023-06-12 09:25:17.000000 bohrium-sdk-0.2.1/bohriumsdk/job.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     2159 2023-05-30 07:06:38.000000 bohrium-sdk-0.2.1/bohriumsdk/node.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     2213 2023-06-12 09:26:00.000000 bohrium-sdk-0.2.1/bohriumsdk/project.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     7809 2023-06-13 01:39:50.000000 bohrium-sdk-0.2.1/bohriumsdk/storage.py
+drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-06-13 02:16:55.972922 bohrium-sdk-0.2.1/bohriumsdk/test/
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)        0 2023-05-29 08:09:08.000000 bohrium-sdk-0.2.1/bohriumsdk/test/__init__.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)       80 2023-05-29 08:13:02.000000 bohrium-sdk-0.2.1/bohriumsdk/test/test_node.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     4467 2023-06-13 01:43:50.000000 bohrium-sdk-0.2.1/bohriumsdk/test.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     4751 2023-06-07 01:28:13.000000 bohrium-sdk-0.2.1/bohriumsdk/util.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)       38 2023-06-13 02:16:55.973641 bohrium-sdk-0.2.1/setup.cfg
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)      366 2023-06-13 02:16:50.000000 bohrium-sdk-0.2.1/setup.py
```

### Comparing `bohrium-sdk-0.2.0/bohriumsdk/client.py` & `bohrium-sdk-0.2.1/bohriumsdk/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 class Client:
     def __init__(
             self, 
             api_version: str = 'v2',
             email: str = "",
             password: str = "",
             base_url_v1: str = 'https://bohrium.dp.tech',
-            base_url_v2: str = "https://openapi.dp.tech",
             token: str = "",
             debug: bool = False,
             use_config_file: bool = False,
             config_file_location_v1: str = '~/.lebesgue_config.json',
             config_file_location_v2: str ='~/.brmconfig'
         ) -> None:
         if api_version == "v1":
@@ -48,20 +47,17 @@
             else:
                 self._login()
         elif api_version == "v2":
             self.config_file_location_expand = os.path.expanduser(config_file_location_v2)
             if not os.path.exists(self.config_file_location_expand):
                 print("Config File ~/.brmconfig not found! Please visit https://bohrium.dp.tech/personal/setting and click AccessKey create button to generate it !")
                 self.access_key = input("Please enter AccessKey: ")
-                
-                # data = f"[Credentials]\nbaseUrl=https://openapi.dp.tech\naccessKey={self.access_key}"
-                data = f"[Credentials]\nbaseUrl=http://localhost:8087\naccessKey={self.access_key}"
+                data = f"[Credentials]\nbaseUrl=https://openapi.dp.tech\naccessKey={self.access_key}"
                 with open(self.config_file_location_expand, 'w') as f:
                     f.write(data)
-            
             config = configparser.ConfigParser()
             config.read(self.config_file_location_expand)
             self.base_url = config.get('Credentials', 'baseUrl')
             self.access_key = config.get('Credentials', 'accessKey')
             # print(self.access_key)
             self.params = {"accessKey": self.access_key}
             self.token = ""
@@ -125,37 +121,37 @@
         return self.token
 
     def check_ak(self):
         url = f"/openapi/v1/ak/get"
         resp = self.get(url=url, params=self.params)
         return resp
 
-    def login(self):
-        email = input("Please enter Bohrium Account Email: ")
-        password = getpass.getpass(prompt="Please enter password: ")
-        post_data = {
-            'username': email,
-            'password': password
-        }
-        resp = requests.post('https://bohrium.dp.tech/account_gw/login', json=post_data).json().get("data", {})
-        self.token = resp.get('token', '')
-        if self.token: print("Login successfully!")
-        else: print("Login failed!")
-
-    def generate_access_key(self, name="default"):
-        post_data = { "name": name }
-        headers = { 'Authorization': f'Bearer {self.token}' }
-        resp = requests.post(url="https://bohrium-api.dp.tech/bohrapi/v1/ak/add", json=post_data, headers=headers)
-        print(resp)
-        resp = resp.json().get("data", {})
-        self.access_key = resp.get("accessKey", "")
-        data = f"[Credentials]\nbaseUrl=https://openapi.dp.tech\naccessKey={self.access_key}"
-        with open(self.config_file_location_expand, 'w') as f:
-            f.write(data)
-        return resp
+    # def login(self):
+    #     email = input("Please enter Bohrium Account Email: ")
+    #     password = getpass.getpass(prompt="Please enter password: ")
+    #     post_data = {
+    #         'username': email,
+    #         'password': password
+    #     }
+    #     resp = requests.post('https://bohrium.dp.tech/account_gw/login', json=post_data).json().get("data", {})
+    #     self.token = resp.get('token', '')
+    #     if self.token: print("Login successfully!")
+    #     else: print("Login failed!")
+
+    # def generate_access_key(self, name="default"):
+    #     post_data = { "name": name }
+    #     headers = { 'Authorization': f'Bearer {self.token}' }
+    #     resp = requests.post(url="https://bohrium-api.dp.tech/bohrapi/v1/ak/add", json=post_data, headers=headers)
+    #     print(resp)
+    #     resp = resp.json().get("data", {})
+    #     self.access_key = resp.get("accessKey", "")
+    #     data = f"[Credentials]\nbaseUrl=https://openapi.dp.tech\naccessKey={self.access_key}"
+    #     with open(self.config_file_location_expand, 'w') as f:
+    #         f.write(data)
+    #     return resp
 
 
     def chat(self, prompt, temperature=0):
         post_data = {
             "messages":[{"role":"user","content":f"{prompt}"}],
             "stream":False,
             "model":"gpt-3.5-turbo",
```

### Comparing `bohrium-sdk-0.2.0/bohriumsdk/database.py` & `bohrium-sdk-0.2.1/bohriumsdk/database.py`

 * *Files identical despite different names*

### Comparing `bohrium-sdk-0.2.0/bohriumsdk/image.py` & `bohrium-sdk-0.2.1/bohriumsdk/image.py`

 * *Files identical despite different names*

### Comparing `bohrium-sdk-0.2.0/bohriumsdk/job.py` & `bohrium-sdk-0.2.1/bohriumsdk/job.py`

 * *Files identical despite different names*

### Comparing `bohrium-sdk-0.2.0/bohriumsdk/node.py` & `bohrium-sdk-0.2.1/bohriumsdk/node.py`

 * *Files identical despite different names*

### Comparing `bohrium-sdk-0.2.0/bohriumsdk/project.py` & `bohrium-sdk-0.2.1/bohriumsdk/project.py`

 * *Files identical despite different names*

### Comparing `bohrium-sdk-0.2.0/bohriumsdk/storage.py` & `bohrium-sdk-0.2.1/bohriumsdk/storage.py`

 * *Files identical despite different names*

### Comparing `bohrium-sdk-0.2.0/bohriumsdk/test.py` & `bohrium-sdk-0.2.1/bohriumsdk/test.py`

 * *Files identical despite different names*

### Comparing `bohrium-sdk-0.2.0/bohriumsdk/util.py` & `bohrium-sdk-0.2.1/bohriumsdk/util.py`

 * *Files identical despite different names*

