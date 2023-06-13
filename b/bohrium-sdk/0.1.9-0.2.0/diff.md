# Comparing `tmp/bohrium-sdk-0.1.9.tar.gz` & `tmp/bohrium-sdk-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bohrium-sdk-0.1.9.tar", last modified: Fri Jun  2 08:11:57 2023, max compression
+gzip compressed data, was "bohrium-sdk-0.2.0.tar", last modified: Tue Jun 13 02:14:56 2023, max compression
```

## Comparing `bohrium-sdk-0.1.9.tar` & `bohrium-sdk-0.2.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-06-02 08:11:57.332857 bohrium-sdk-0.1.9/
--rw-r--r--   0 dingzhaohan   (501) staff       (20)      205 2023-06-02 08:11:57.332654 bohrium-sdk-0.1.9/PKG-INFO
--rw-r--r--   0 dingzhaohan   (501) staff       (20)       56 2023-05-16 07:10:39.000000 bohrium-sdk-0.1.9/README.md
-drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-06-02 08:11:57.327827 bohrium-sdk-0.1.9/bohrium_sdk.egg-info/
--rw-r--r--   0 dingzhaohan   (501) staff       (20)      205 2023-06-02 08:11:57.000000 bohrium-sdk-0.1.9/bohrium_sdk.egg-info/PKG-INFO
--rw-r--r--   0 dingzhaohan   (501) staff       (20)      459 2023-06-02 08:11:57.000000 bohrium-sdk-0.1.9/bohrium_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 dingzhaohan   (501) staff       (20)        1 2023-06-02 08:11:57.000000 bohrium-sdk-0.1.9/bohrium_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 dingzhaohan   (501) staff       (20)       84 2023-06-02 08:11:57.000000 bohrium-sdk-0.1.9/bohrium_sdk.egg-info/entry_points.txt
--rw-r--r--   0 dingzhaohan   (501) staff       (20)       11 2023-06-02 08:11:57.000000 bohrium-sdk-0.1.9/bohrium_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-06-02 08:11:57.331425 bohrium-sdk-0.1.9/bohriumsdk/
--rw-r--r--   0 dingzhaohan   (501) staff       (20)      123 2023-05-16 07:22:01.000000 bohrium-sdk-0.1.9/bohriumsdk/__init__.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)        0 2023-05-29 08:11:22.000000 bohrium-sdk-0.1.9/bohriumsdk/__main__.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     6137 2023-06-02 08:11:36.000000 bohrium-sdk-0.1.9/bohriumsdk/client.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     1970 2023-05-30 07:06:19.000000 bohrium-sdk-0.1.9/bohriumsdk/image.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     3766 2023-05-30 07:06:03.000000 bohrium-sdk-0.1.9/bohriumsdk/job.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     2159 2023-05-30 07:06:38.000000 bohrium-sdk-0.1.9/bohriumsdk/node.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     2223 2023-05-30 07:25:30.000000 bohrium-sdk-0.1.9/bohriumsdk/project.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     2835 2023-05-30 07:06:55.000000 bohrium-sdk-0.1.9/bohriumsdk/storage.py
-drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-06-02 08:11:57.332215 bohrium-sdk-0.1.9/bohriumsdk/test/
--rw-r--r--   0 dingzhaohan   (501) staff       (20)        0 2023-05-29 08:09:08.000000 bohrium-sdk-0.1.9/bohriumsdk/test/__init__.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)       80 2023-05-29 08:13:02.000000 bohrium-sdk-0.1.9/bohriumsdk/test/test_node.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     2369 2023-05-30 01:45:00.000000 bohrium-sdk-0.1.9/bohriumsdk/test.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)     4730 2023-06-02 07:31:47.000000 bohrium-sdk-0.1.9/bohriumsdk/util.py
--rw-r--r--   0 dingzhaohan   (501) staff       (20)       38 2023-06-02 08:11:57.333020 bohrium-sdk-0.1.9/setup.cfg
--rw-r--r--   0 dingzhaohan   (501) staff       (20)      501 2023-06-02 08:11:41.000000 bohrium-sdk-0.1.9/setup.py
+drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-06-13 02:14:56.967407 bohrium-sdk-0.2.0/
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)      205 2023-06-13 02:14:56.967013 bohrium-sdk-0.2.0/PKG-INFO
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)       56 2023-05-16 07:10:39.000000 bohrium-sdk-0.2.0/README.md
+drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-06-13 02:14:56.950762 bohrium-sdk-0.2.0/bohrium_sdk.egg-info/
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)      205 2023-06-13 02:14:56.000000 bohrium-sdk-0.2.0/bohrium_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)      444 2023-06-13 02:14:56.000000 bohrium-sdk-0.2.0/bohrium_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)        1 2023-06-13 02:14:56.000000 bohrium-sdk-0.2.0/bohrium_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)       11 2023-06-13 02:14:56.000000 bohrium-sdk-0.2.0/bohrium_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-06-13 02:14:56.963894 bohrium-sdk-0.2.0/bohriumsdk/
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)      123 2023-05-16 07:22:01.000000 bohrium-sdk-0.2.0/bohriumsdk/__init__.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)        0 2023-05-29 08:11:22.000000 bohrium-sdk-0.2.0/bohriumsdk/__main__.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     6955 2023-06-13 01:50:05.000000 bohrium-sdk-0.2.0/bohriumsdk/client.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     1737 2023-06-08 02:50:49.000000 bohrium-sdk-0.2.0/bohriumsdk/database.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     1965 2023-06-12 09:26:10.000000 bohrium-sdk-0.2.0/bohriumsdk/image.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     4119 2023-06-12 09:25:17.000000 bohrium-sdk-0.2.0/bohriumsdk/job.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     2159 2023-05-30 07:06:38.000000 bohrium-sdk-0.2.0/bohriumsdk/node.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     2213 2023-06-12 09:26:00.000000 bohrium-sdk-0.2.0/bohriumsdk/project.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     7809 2023-06-13 01:39:50.000000 bohrium-sdk-0.2.0/bohriumsdk/storage.py
+drwxr-xr-x   0 dingzhaohan   (501) staff       (20)        0 2023-06-13 02:14:56.966450 bohrium-sdk-0.2.0/bohriumsdk/test/
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)        0 2023-05-29 08:09:08.000000 bohrium-sdk-0.2.0/bohriumsdk/test/__init__.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)       80 2023-05-29 08:13:02.000000 bohrium-sdk-0.2.0/bohriumsdk/test/test_node.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     4467 2023-06-13 01:43:50.000000 bohrium-sdk-0.2.0/bohriumsdk/test.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)     4751 2023-06-07 01:28:13.000000 bohrium-sdk-0.2.0/bohriumsdk/util.py
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)       38 2023-06-13 02:14:56.967690 bohrium-sdk-0.2.0/setup.cfg
+-rw-r--r--   0 dingzhaohan   (501) staff       (20)      366 2023-06-13 02:14:48.000000 bohrium-sdk-0.2.0/setup.py
```

### Comparing `bohrium-sdk-0.1.9/bohriumsdk/client.py` & `bohrium-sdk-0.2.0/bohriumsdk/client.py`

 * *Files 17% similar despite different names*

```diff
@@ -46,32 +46,39 @@
             if token is not None:
                 self.token = token
             else:
                 self._login()
         elif api_version == "v2":
             self.config_file_location_expand = os.path.expanduser(config_file_location_v2)
             if not os.path.exists(self.config_file_location_expand):
-                print("Config File ~/.brmconfig not found! Now login to bohrium and generate it!")
-                self.login()
-                access_key_name = input("Please enter access_key name: ")
-                self.generate_access_key(access_key_name)
+                print("Config File ~/.brmconfig not found! Please visit https://bohrium.dp.tech/personal/setting and click AccessKey create button to generate it !")
+                self.access_key = input("Please enter AccessKey: ")
+                
+                # data = f"[Credentials]\nbaseUrl=https://openapi.dp.tech\naccessKey={self.access_key}"
+                data = f"[Credentials]\nbaseUrl=http://localhost:8087\naccessKey={self.access_key}"
+                with open(self.config_file_location_expand, 'w') as f:
+                    f.write(data)
+            
             config = configparser.ConfigParser()
             config.read(self.config_file_location_expand)
             self.base_url = config.get('Credentials', 'baseUrl')
             self.access_key = config.get('Credentials', 'accessKey')
+            # print(self.access_key)
             self.params = {"accessKey": self.access_key}
             self.token = ""
+            self.check_ak()
+            
 
-    def post(self, url, host="", data=None, headers=None, params=None, stream=False, retry=5):
-        return self._req('POST', url, host=host, data=data, headers=headers, params=params, stream=stream, retry=retry)
+    def post(self, url, host="", json=None, data=None, headers=None, params=None, stream=False, retry=5):
+        return self._req('POST', url, host=host, json=json, data=data, headers=headers, params=params, stream=stream, retry=retry)
 
-    def get(self, url, host="", data=None, headers=None, params=None, stream=False, retry=5):
-        return self._req('GET', url, host=host, data=data, headers=headers, params=params, stream=stream, retry=retry)
+    def get(self, url, host="", json=None, headers=None, params=None, stream=False, retry=5):
+        return self._req('GET', url, host=host, json=json, headers=headers, params=params, stream=stream, retry=retry)
 
-    def _req(self, method, url, host="", data=None, headers=None, params=None, stream=False, retry=5):
+    def _req(self, method, url, host="", json=None, data=None, headers=None, params=None, stream=False, retry=3):
         if host: #in ["https://bohrium.test.dp.tech", "https://tiefblue.test.dp.tech"]:
             url = urllib.parse.urljoin(host, url)
         else:
             url = urllib.parse.urljoin(self.base_url, url)
         
         # Set Headers
         if headers is None: headers = {}
@@ -83,16 +90,20 @@
         resp_code = None
         for i in range(retry):
             resp = None
             err = ""
             if method == 'GET':
                 resp = requests.get(url=url, params=params, headers=headers, stream=stream)
             if method == 'POST':
-                resp = requests.post(url=url, json=data, params=params, headers=headers, stream=stream)
+                resp = requests.post(url=url, json=json, data=data, params=params, headers=headers, stream=stream)
             resp_code = resp.status_code
+            if resp_code == 401:
+                os.remove(self.config_file_location_expand)
+                print("Config file(~/.brmconfig) AccessKey invalid! Visit https://bohrium.dp.tech/personal/setting to generate it! ")
+                exit()
             if not resp.ok:
                 try:
                     result = resp.json()
                     err = result.get("error")
                 except:
                     pass
                 time.sleep(0.1 * i)
@@ -109,14 +120,18 @@
                 break
         raise RequestInfoException(resp_code, url, err)
 
     def get_token(self):
         self.login()
         return self.token
 
+    def check_ak(self):
+        url = f"/openapi/v1/ak/get"
+        resp = self.get(url=url, params=self.params)
+        return resp
 
     def login(self):
         email = input("Please enter Bohrium Account Email: ")
         password = getpass.getpass(prompt="Please enter password: ")
         post_data = {
             'username': email,
             'password': password
@@ -144,9 +159,9 @@
             "messages":[{"role":"user","content":f"{prompt}"}],
             "stream":False,
             "model":"gpt-3.5-turbo",
             "temperature":temperature,
             "presence_penalty":0
         }
 
-        resp = self.post(f"/openapi/v1/chat/complete", data=post_data, params=self.params)
+        resp = self.post(f"/openapi/v1/chat/complete", json=post_data, params=self.params)
         return resp
```

### Comparing `bohrium-sdk-0.1.9/bohriumsdk/image.py` & `bohrium-sdk-0.2.0/bohriumsdk/image.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,15 +40,15 @@
             if page_number > 1:
                 data = self.list_image_by_page(project_id=project_id, kind=kind, page=page_number, per_page=30)
             project_list.extend(data['items'])
         return project_list
 
 
     def delete(self, image_id):
-        host = "https://bohrium.test.dp.tech"
+        host = "https://bohrium.dp.tech"
         url = f'/brm/v1/image/del/{image_id}'
         data = self.client.get(host=host, url=url)
         
         return data
 
     def print_image(
             self,
```

### Comparing `bohrium-sdk-0.1.9/bohriumsdk/job.py` & `bohrium-sdk-0.2.0/bohriumsdk/job.py`

 * *Files 10% similar despite different names*

```diff
@@ -55,29 +55,29 @@
         return data
     
     def log(self, job_id):
         data = self.client.get(f'/openapi/v1/job/{job_id}/log', params=self.client.params)
         return data
 
     def insert(self, **kwargs):
-        must_fill = ['oss_path', 'project_id', 'machine_type', 'command', 'platform', 'image_address', 'job_id', 'bohr_job_group_id']
+        must_fill = ['job_type', 'oss_path', 'project_id', 'scass_type', 'command', 'platform', 'image_address', 'job_id']
         # must_fill = ['job_type', 'oss_path', 'project_id', 'scass_type', 'command', 'platform', 'image_name']
         for each in must_fill:
             if each not in kwargs:
                 raise ValueError(f'{each} is required when submitting job')
         camel_data = {humps.camelize(k): v for k, v in kwargs.items()}
         if not isinstance(camel_data['ossPath'], list):
             camel_data['ossPath'] = [camel_data['ossPath']]
         if 'logFile' in camel_data:
             camel_data['logFiles'] = camel_data['logFile']
         if 'logFiles' in camel_data and not isinstance(camel_data['logFiles'], list):
             camel_data['logFiles'] = [camel_data['logFiles']]
-        if self.client.debug:
-            print(camel_data)
-        data = self.client.post(f"/openapi/v2/job/add", data=camel_data, params=self.client.params)
+        #if self.client.debug:
+        print(camel_data)
+        data = self.client.post(f"/openapi/v2/job/add", json=camel_data, params=self.client.params)
         return data
 
 
     def detail(self, job_id):
         data = self.client.get(f'/openapi/v1/job/{job_id}', params=self.client.params)
         return data
     
@@ -86,19 +86,30 @@
             'projectId': project_id
         }
         if name:
             data['name'] = name
         if group_id:
             data['groupId'] = group_id
         try:
-            data = self.client.post(f'/openapi/v1/job/create', data=data, params=self.client.params)
+            data = self.client.post(f'/openapi/v1/job/create', json=data, params=self.client.params)
         except Exception as e:
             raise e
         return data
     
+    def create_job_group(self, project_id, job_group_name):
+        data = {
+            "name": job_group_name,
+            "projectId": project_id
+        }
+        try:
+            resp = self.client.post(f"/openapi/v1/job_group/add", json=data, params=self.client.params).json()
+        except Exception as e:
+            raise e
+        return resp["data"]
+    
     def get_job_token(self, job_id):
         url = f"/openapi/v1/job/{job_id}/input/token"
 
         data = self.client.get(url=url, params=self.client.params)
         print(data)
```

### Comparing `bohrium-sdk-0.1.9/bohriumsdk/node.py` & `bohrium-sdk-0.2.0/bohriumsdk/node.py`

 * *Files identical despite different names*

### Comparing `bohrium-sdk-0.1.9/bohriumsdk/project.py` & `bohrium-sdk-0.2.0/bohriumsdk/project.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,27 +9,27 @@
         self.client = client
 
     def list_project_by_page(
             self,
             page: int = 1,
             per_page: int = 30
         ) -> None:
-        host = "https://bohrium.test.dp.tech"
+        host = "https://bohrium.dp.tech"
         # host = "https://openapi.dp.tech/"
         url = "/account/programs"
         params = {
             "page": page,
             "per_page": per_page
         }
         #self.client.token = "Bearer eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVCJ9.eyJleHAiOjE2ODc2ODE2MTEsImlkZW50aXR5Ijp7Im9yZ0lkIjoxNTcsInVzZXJJZCI6MTU3fSwib3JpZ19pYXQiOjE2ODUwODk2MTF9.OGASZRsHqAKILDSYqyfd76yVktQ8L_oIHFFvWmY54yl7qFaSXXgx6-9_1KoeZG4S36tZFfk8isZaBPpTSTIX6JMkYqdLtxVBGogr4np3hz_ZV8a3set5uTst47Rwa_7Yk1v2iAU4FrghnKemnVu8e4uJSH2pClLgPQVZKF1CZd3AlG55fAvqnzY0-9uiKyBYmfuvUNM1ZlMJXHmFJ400NKZWkZj4iygJ03wGjKBBeXhyIZ4EyIbGrP7683JN2jOyw4wJJISAvKsv_gTNw_mRkdFsZuYx-u19II2UhqCAvMJtwjwgtIY4ReNfEoQPBUJWVyFBi7vaNbkwk-fghr2L0g"
         data = self.client.get(url=url, host=host, params=params)
         return data
     
     def list_all_project(self):
-        host = "https://bohrium.test.dp.tech"
+        host = "https://bohrium.dp.tech"
         url = "/brm/v1/project/list"
         params = {
             'page': 1,
             'pageSize': 10000,
             'queryType': 'all'
         }
         data = self.client.get(url=url, host=host, params=params)
```

### Comparing `bohrium-sdk-0.1.9/bohriumsdk/util.py` & `bohrium-sdk-0.2.0/bohriumsdk/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,16 +25,16 @@
         # if env == "notebook":
         #     console = JupyterConsole()
         #     console.print(table)
         #     display(console) 
         # else:
         print(table)
 
-
-    def zip_file_list(root_path, zip_filename, file_list=[]):
+    @classmethod
+    def zip_file_list(cls, root_path, zip_filename, file_list=[]):
         out_zip_file = os.path.join(root_path, zip_filename)
         # print('debug: file_list', file_list)
         zip_obj = ZipFile(out_zip_file, "w")
         for f in file_list:
             matched_files = os.path.join(root_path, f)
             for ii in glob.glob(matched_files):
                 # print('debug: matched_files:ii', ii)
```

