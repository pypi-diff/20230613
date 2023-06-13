# Comparing `tmp/yly-python-sdk-1.2.1.tar.gz` & `tmp/yly-python-sdk-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/yly-python-sdk-1.2.1.tar", last modified: Wed May 12 06:15:41 2021, max compression
+gzip compressed data, was "yly-python-sdk-2.0.tar", last modified: Tue Jun 13 09:43:48 2023, max compression
```

## Comparing `yly-python-sdk-1.2.1.tar` & `yly-python-sdk-2.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 lwy       (1000) lwy       (1000)        0 2021-05-12 06:15:41.278904 yly-python-sdk-1.2.1/
-drwxrwxr-x   0 lwy       (1000) lwy       (1000)        0 2021-05-12 06:15:41.274904 yly-python-sdk-1.2.1/Lib/
-drwxrwxr-x   0 lwy       (1000) lwy       (1000)        0 2021-05-12 06:15:41.274904 yly-python-sdk-1.2.1/Lib/Api/
--rw-rw-r--   0 lwy       (1000) lwy       (1000)        0 2021-05-12 06:01:33.000000 yly-python-sdk-1.2.1/Lib/Api/__init__.py
--rw-rw-r--   0 lwy       (1000) lwy       (1000)      852 2021-05-12 06:12:54.000000 yly-python-sdk-1.2.1/Lib/Api/yly_express_print.py
--rw-rw-r--   0 lwy       (1000) lwy       (1000)      546 2021-05-12 06:01:33.000000 yly-python-sdk-1.2.1/Lib/Api/yly_oauth.py
--rw-rw-r--   0 lwy       (1000) lwy       (1000)      700 2021-05-12 06:01:33.000000 yly-python-sdk-1.2.1/Lib/Api/yly_picture_print.py
--rw-rw-r--   0 lwy       (1000) lwy       (1000)      646 2021-05-12 06:01:33.000000 yly-python-sdk-1.2.1/Lib/Api/yly_print.py
--rw-rw-r--   0 lwy       (1000) lwy       (1000)      527 2021-05-12 06:01:33.000000 yly-python-sdk-1.2.1/Lib/Api/yly_print_menu.py
--rw-rw-r--   0 lwy       (1000) lwy       (1000)     6682 2021-05-12 06:01:33.000000 yly-python-sdk-1.2.1/Lib/Api/yly_printer.py
-drwxrwxr-x   0 lwy       (1000) lwy       (1000)        0 2021-05-12 06:15:41.274904 yly-python-sdk-1.2.1/Lib/Config/
--rw-rw-r--   0 lwy       (1000) lwy       (1000)        0 2021-05-12 06:01:33.000000 yly-python-sdk-1.2.1/Lib/Config/__init__.py
--rw-rw-r--   0 lwy       (1000) lwy       (1000)      551 2021-05-12 06:01:33.000000 yly-python-sdk-1.2.1/Lib/Config/config.py
-drwxrwxr-x   0 lwy       (1000) lwy       (1000)        0 2021-05-12 06:15:41.274904 yly-python-sdk-1.2.1/Lib/Oauth/
--rw-rw-r--   0 lwy       (1000) lwy       (1000)        0 2021-05-12 06:01:33.000000 yly-python-sdk-1.2.1/Lib/Oauth/__init__.py
--rw-rw-r--   0 lwy       (1000) lwy       (1000)     1874 2021-05-12 06:01:33.000000 yly-python-sdk-1.2.1/Lib/Oauth/oauth.py
-drwxrwxr-x   0 lwy       (1000) lwy       (1000)        0 2021-05-12 06:15:41.274904 yly-python-sdk-1.2.1/Lib/Protocol/
--rw-rw-r--   0 lwy       (1000) lwy       (1000)        0 2021-05-12 06:01:33.000000 yly-python-sdk-1.2.1/Lib/Protocol/__init__.py
--rw-rw-r--   0 lwy       (1000) lwy       (1000)     1256 2021-05-12 06:01:33.000000 yly-python-sdk-1.2.1/Lib/Protocol/rpc_client.py
--rw-rw-r--   0 lwy       (1000) lwy       (1000)        0 2021-05-12 06:01:33.000000 yly-python-sdk-1.2.1/Lib/__init__.py
--rw-rw-r--   0 lwy       (1000) lwy       (1000)      244 2021-05-12 06:15:41.278904 yly-python-sdk-1.2.1/PKG-INFO
--rw-rw-r--   0 lwy       (1000) lwy       (1000)     2100 2021-05-12 06:01:33.000000 yly-python-sdk-1.2.1/README.md
--rw-rw-r--   0 lwy       (1000) lwy       (1000)       38 2021-05-12 06:15:41.278904 yly-python-sdk-1.2.1/setup.cfg
--rw-rw-r--   0 lwy       (1000) lwy       (1000)      341 2021-05-12 06:11:55.000000 yly-python-sdk-1.2.1/setup.py
-drwxrwxr-x   0 lwy       (1000) lwy       (1000)        0 2021-05-12 06:15:41.278904 yly-python-sdk-1.2.1/yly_python_sdk.egg-info/
--rw-rw-r--   0 lwy       (1000) lwy       (1000)      244 2021-05-12 06:15:41.000000 yly-python-sdk-1.2.1/yly_python_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 lwy       (1000) lwy       (1000)      492 2021-05-12 06:15:41.000000 yly-python-sdk-1.2.1/yly_python_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 lwy       (1000) lwy       (1000)        1 2021-05-12 06:15:41.000000 yly-python-sdk-1.2.1/yly_python_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 lwy       (1000) lwy       (1000)        4 2021-05-12 06:15:41.000000 yly-python-sdk-1.2.1/yly_python_sdk.egg-info/top_level.txt
+drwxrwxr-x   0 lwy       (1000) lwy       (1000)        0 2023-06-13 09:43:48.087800 yly-python-sdk-2.0/
+drwxrwxr-x   0 lwy       (1000) lwy       (1000)        0 2023-06-13 09:43:48.083800 yly-python-sdk-2.0/Lib/
+drwxrwxr-x   0 lwy       (1000) lwy       (1000)        0 2023-06-13 09:43:48.083800 yly-python-sdk-2.0/Lib/Api/
+-rw-rw-r--   0 lwy       (1000) lwy       (1000)        0 2021-05-12 06:01:33.000000 yly-python-sdk-2.0/Lib/Api/__init__.py
+-rw-rw-r--   0 lwy       (1000) lwy       (1000)     1200 2023-06-13 09:19:49.000000 yly-python-sdk-2.0/Lib/Api/yly_express_print.py
+-rw-rw-r--   0 lwy       (1000) lwy       (1000)      546 2021-05-12 06:01:33.000000 yly-python-sdk-2.0/Lib/Api/yly_oauth.py
+-rw-rw-r--   0 lwy       (1000) lwy       (1000)      794 2023-06-13 09:20:20.000000 yly-python-sdk-2.0/Lib/Api/yly_picture_print.py
+-rw-rw-r--   0 lwy       (1000) lwy       (1000)      887 2023-06-13 09:19:49.000000 yly-python-sdk-2.0/Lib/Api/yly_print.py
+-rw-rw-r--   0 lwy       (1000) lwy       (1000)      527 2021-05-12 06:01:33.000000 yly-python-sdk-2.0/Lib/Api/yly_print_menu.py
+-rw-rw-r--   0 lwy       (1000) lwy       (1000)     7056 2023-06-13 09:16:23.000000 yly-python-sdk-2.0/Lib/Api/yly_printer.py
+drwxrwxr-x   0 lwy       (1000) lwy       (1000)        0 2023-06-13 09:43:48.083800 yly-python-sdk-2.0/Lib/Config/
+-rw-rw-r--   0 lwy       (1000) lwy       (1000)        0 2021-05-12 06:01:33.000000 yly-python-sdk-2.0/Lib/Config/__init__.py
+-rw-rw-r--   0 lwy       (1000) lwy       (1000)      635 2023-06-13 09:00:02.000000 yly-python-sdk-2.0/Lib/Config/config.py
+drwxrwxr-x   0 lwy       (1000) lwy       (1000)        0 2023-06-13 09:43:48.083800 yly-python-sdk-2.0/Lib/Oauth/
+-rw-rw-r--   0 lwy       (1000) lwy       (1000)        0 2021-05-12 06:01:33.000000 yly-python-sdk-2.0/Lib/Oauth/__init__.py
+-rw-rw-r--   0 lwy       (1000) lwy       (1000)     1879 2023-06-13 09:02:12.000000 yly-python-sdk-2.0/Lib/Oauth/oauth.py
+drwxrwxr-x   0 lwy       (1000) lwy       (1000)        0 2023-06-13 09:43:48.087800 yly-python-sdk-2.0/Lib/Protocol/
+-rw-rw-r--   0 lwy       (1000) lwy       (1000)        0 2021-05-12 06:01:33.000000 yly-python-sdk-2.0/Lib/Protocol/__init__.py
+-rw-rw-r--   0 lwy       (1000) lwy       (1000)     1267 2023-06-13 09:06:45.000000 yly-python-sdk-2.0/Lib/Protocol/rpc_client.py
+-rw-rw-r--   0 lwy       (1000) lwy       (1000)        0 2021-05-12 06:01:33.000000 yly-python-sdk-2.0/Lib/__init__.py
+-rw-rw-r--   0 lwy       (1000) lwy       (1000)      242 2023-06-13 09:43:48.087800 yly-python-sdk-2.0/PKG-INFO
+-rw-rw-r--   0 lwy       (1000) lwy       (1000)     2442 2023-06-13 09:23:27.000000 yly-python-sdk-2.0/README.md
+-rw-rw-r--   0 lwy       (1000) lwy       (1000)       38 2023-06-13 09:43:48.087800 yly-python-sdk-2.0/setup.cfg
+-rw-rw-r--   0 lwy       (1000) lwy       (1000)      339 2023-06-13 09:36:59.000000 yly-python-sdk-2.0/setup.py
+drwxrwxr-x   0 lwy       (1000) lwy       (1000)        0 2023-06-13 09:43:48.087800 yly-python-sdk-2.0/yly_python_sdk.egg-info/
+-rw-rw-r--   0 lwy       (1000) lwy       (1000)      242 2023-06-13 09:43:47.000000 yly-python-sdk-2.0/yly_python_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 lwy       (1000) lwy       (1000)      492 2023-06-13 09:43:47.000000 yly-python-sdk-2.0/yly_python_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 lwy       (1000) lwy       (1000)        1 2023-06-13 09:43:47.000000 yly-python-sdk-2.0/yly_python_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 lwy       (1000) lwy       (1000)        4 2023-06-13 09:43:47.000000 yly-python-sdk-2.0/yly_python_sdk.egg-info/top_level.txt
```

### Comparing `yly-python-sdk-1.2.1/Lib/Api/yly_express_print.py` & `yly-python-sdk-2.0/Lib/Api/yly_print_menu.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,22 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 
-class YlyExpressPrint:
+class YlyPrintMenu:
 
     __client = None
 
     def __init__(self, client):
         self.__client = client
 
-    def index(self, machine_code, content, origin_id, sandbox):
+    def add_print_menu(self, machine_code, content):
         """
-        面单打印接口
-        不支持机型: k4-wh, k4-wa, m1 (k4系列机型不建议使用不干胶热敏纸)
+        添加应用菜单接口
         :param machine_code: 机器码
-        :param content: 面单数据
-        :param origin_id: 商户系统内部订单号，要求32个字符内，只能是数字、大小写字母
-        :param sandbox: 沙箱环境1  正式环境0
+        :param content: 菜单详情(json)
         :return:
         """
         params = {
             'machine_code': machine_code,
-            'content': content,
-            'origin_id': origin_id,
-            'sandbox': sandbox
+            'content': content
         }
-        return self.__client.call('expressprint/index', params)
+        return self.__client.call('printmenu/addprintmenu', params)
```

### Comparing `yly-python-sdk-1.2.1/Lib/Api/yly_oauth.py` & `yly-python-sdk-2.0/Lib/Api/yly_oauth.py`

 * *Files identical despite different names*

### Comparing `yly-python-sdk-1.2.1/Lib/Api/yly_printer.py` & `yly-python-sdk-2.0/Lib/Api/yly_printer.py`

 * *Files 1% similar despite different names*

```diff
@@ -215,14 +215,27 @@
         params = {
             'machine_code': machine_code,
             'page_index': page_index,
             'page_size': page_size
         }
         return self.__client.call('printer/getorderpaginglist', params)
 
+    def reprint(self, machine_code, order_no):
+        """
+        获取订单状态接口
+        :param machine_code: 机器码
+        :param order_no: 易联云订单id
+        :return:
+        """
+        params = {
+            'machine_code': machine_code,
+            'order_id': order_no
+        }
+        return self.__client.call('printer/reprintorder', params)
+
     def get_print_status(self, machine_code):
         """
         获取终端状态接口
         :param machine_code: 机器码
         :return:
         """
         params = {
```

### Comparing `yly-python-sdk-1.2.1/Lib/Config/config.py` & `yly-python-sdk-2.0/Lib/Config/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/python
 class Config:
 
     __client_id = None
     __client_secret = None
-    __request_url = 'https://open-api.10ss.net/'
+    __request_url = 'https://open-api.10ss.net'
 
     def __init__(self, id, secret):
         if (id == None or secret == None):
             raise Exception('ClientId and clientSecret cannot be empty')
         self.__client_id = id
         self.__client_secret = secret
 
@@ -15,7 +15,10 @@
         return self.__client_id
 
     def get_client_secret(self):
         return self.__client_secret
 
     def get_request_url(self):
         return self.__request_url
+
+    def set_request_url(self, request_url):
+        self.__request_url = request_url
```

### Comparing `yly-python-sdk-1.2.1/Lib/Oauth/oauth.py` & `yly-python-sdk-2.0/Lib/Oauth/oauth.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,12 +45,12 @@
         return self.post(params)
 
     def post(self, req_params):
         try:
             header = {
                 'Content-Type': 'application/x-www-form-urlencoded;charset=utf-8'
             }
-            req_url = self.url + 'oauth/oauth'
+            req_url = self.url + '/' +'oauth/oauth'
             res = requests.post(req_url, data=req_params, headers=header)
             return json.loads(res.text)
         except Exception as e:
             raise Exception('yly api response:{}'.format(e))
```

### Comparing `yly-python-sdk-1.2.1/Lib/Protocol/rpc_client.py` & `yly-python-sdk-2.0/Lib/Protocol/rpc_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,20 +14,20 @@
         self.client_secret = config.get_client_secret()
         self.url = config.get_request_url()
         self.md5 = hashlib.md5()
 
     def call(self, action, params):
         params['client_id'] = self.client_id
         params['access_token'] = self.access_token
-        params['timestamp'] = time.time()
+        params['timestamp'] = int(time.time())
         params['id'] = uuid.uuid4()
         sign_str = str(self.client_id) + str(params['timestamp']) + self.client_secret
         self.md5.update(sign_str.encode('utf-8'))
         params['sign'] = self.md5.hexdigest()
-        request_url = self.url + action
+        request_url = self.url + '/' + action
         request_data = params
         return self.post(request_url, request_data)
 
     def post(self, req_url, req_params):
         try:
             header = {
                 'Content-Type': 'application/x-www-form-urlencoded;charset=utf-8',
```

