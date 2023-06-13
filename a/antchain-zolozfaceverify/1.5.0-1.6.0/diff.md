# Comparing `tmp/antchain_zolozfaceverify-1.5.0.tar.gz` & `tmp/antchain_zolozfaceverify-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_zolozfaceverify-1.5.0.tar", last modified: Wed May 25 05:56:58 2022, max compression
+gzip compressed data, was "dist/antchain_zolozfaceverify-1.6.0.tar", last modified: Tue Jun 13 10:38:07 2023, max compression
```

## Comparing `antchain_zolozfaceverify-1.5.0.tar` & `antchain_zolozfaceverify-1.6.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-25 05:56:58.000000 antchain_zolozfaceverify-1.5.0/
--rw-r--r--   0 root         (0) root         (0)      600 2022-05-25 05:56:57.000000 antchain_zolozfaceverify-1.5.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2022-05-25 05:56:57.000000 antchain_zolozfaceverify-1.5.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2242 2022-05-25 05:56:58.000000 antchain_zolozfaceverify-1.5.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      848 2022-05-25 05:56:57.000000 antchain_zolozfaceverify-1.5.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1034 2022-05-25 05:56:57.000000 antchain_zolozfaceverify-1.5.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-25 05:56:58.000000 antchain_zolozfaceverify-1.5.0/antchain_sdk_zolozfaceverify/
--rw-r--r--   0 root         (0) root         (0)       21 2022-05-25 05:56:57.000000 antchain_zolozfaceverify-1.5.0/antchain_sdk_zolozfaceverify/__init__.py
--rw-r--r--   0 root         (0) root         (0)    60014 2022-05-25 05:56:57.000000 antchain_zolozfaceverify-1.5.0/antchain_sdk_zolozfaceverify/client.py
--rw-r--r--   0 root         (0) root         (0)   108698 2022-05-25 05:56:57.000000 antchain_zolozfaceverify-1.5.0/antchain_sdk_zolozfaceverify/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-25 05:56:58.000000 antchain_zolozfaceverify-1.5.0/antchain_zolozfaceverify.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2242 2022-05-25 05:56:58.000000 antchain_zolozfaceverify-1.5.0/antchain_zolozfaceverify.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      419 2022-05-25 05:56:58.000000 antchain_zolozfaceverify-1.5.0/antchain_zolozfaceverify.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-05-25 05:56:58.000000 antchain_zolozfaceverify-1.5.0/antchain_zolozfaceverify.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2022-05-25 05:56:58.000000 antchain_zolozfaceverify-1.5.0/antchain_zolozfaceverify.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2022-05-25 05:56:58.000000 antchain_zolozfaceverify-1.5.0/antchain_zolozfaceverify.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-05-25 05:56:58.000000 antchain_zolozfaceverify-1.5.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2548 2022-05-25 05:56:57.000000 antchain_zolozfaceverify-1.5.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 10:38:07.000000 antchain_zolozfaceverify-1.6.0/
+-rw-r--r--   0 root         (0) root         (0)      600 2023-06-13 10:38:07.000000 antchain_zolozfaceverify-1.6.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-13 10:38:07.000000 antchain_zolozfaceverify-1.6.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2234 2023-06-13 10:38:07.000000 antchain_zolozfaceverify-1.6.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      840 2023-06-13 10:38:07.000000 antchain_zolozfaceverify-1.6.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1026 2023-06-13 10:38:07.000000 antchain_zolozfaceverify-1.6.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 10:38:07.000000 antchain_zolozfaceverify-1.6.0/antchain_sdk_zolozfaceverify/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-13 10:38:07.000000 antchain_zolozfaceverify-1.6.0/antchain_sdk_zolozfaceverify/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    63246 2023-06-13 10:38:07.000000 antchain_zolozfaceverify-1.6.0/antchain_sdk_zolozfaceverify/client.py
+-rw-r--r--   0 root         (0) root         (0)   117513 2023-06-13 10:38:07.000000 antchain_zolozfaceverify-1.6.0/antchain_sdk_zolozfaceverify/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 10:38:07.000000 antchain_zolozfaceverify-1.6.0/antchain_zolozfaceverify.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2234 2023-06-13 10:38:07.000000 antchain_zolozfaceverify-1.6.0/antchain_zolozfaceverify.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      419 2023-06-13 10:38:07.000000 antchain_zolozfaceverify-1.6.0/antchain_zolozfaceverify.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 10:38:07.000000 antchain_zolozfaceverify-1.6.0/antchain_zolozfaceverify.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-06-13 10:38:07.000000 antchain_zolozfaceverify-1.6.0/antchain_zolozfaceverify.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-13 10:38:07.000000 antchain_zolozfaceverify-1.6.0/antchain_zolozfaceverify.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-13 10:38:07.000000 antchain_zolozfaceverify-1.6.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2548 2023-06-13 10:38:07.000000 antchain_zolozfaceverify-1.6.0/setup.py
```

### Comparing `antchain_zolozfaceverify-1.5.0/LICENSE` & `antchain_zolozfaceverify-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_zolozfaceverify-1.5.0/PKG-INFO` & `antchain_zolozfaceverify-1.6.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain_zolozfaceverify
-Version: 1.5.0
+Version: 1.6.0
 Summary: Ant Chain ZOLOZFACEVERIFY SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         
@@ -17,16 +17,16 @@
         ## Installation
         
         - **Install with pip**
         
         Python SDK uses a common package management tool named `pip`. If pip is not installed, see the [pip user guide](https://pip.pypa.io/en/stable/installing/ "pip User Guide") to install pip.
         
         ```bash
-        # Install the antchain_sdk_zolozfaceverify
-        pip install antchain_sdk_zolozfaceverify
+        # Install the antchain-zolozfaceverify
+        pip install antchain-zolozfaceverify
         ```
         
         ## Issues
         
         [Opening an Issue](https://github.com/alipay/antchain-openapi-prod-sdk/issues/new), Issues not conforming to the guidelines may be closed immediately.
         
         ## Usage
```

### Comparing `antchain_zolozfaceverify-1.5.0/README-CN.md` & `antchain_zolozfaceverify-1.6.0/README-CN.md`

 * *Files 3% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 ## 安装
 
 - **使用 pip 安装(推荐)**
 
 如未安装 `pip`, 请先至pip官网 [pip user guide](https://pip.pypa.io/en/stable/installing/ "pip User Guide") 安装pip .
 
 ```bash
-# 安装 antchain_sdk_zolozfaceverify
-pip install antchain_sdk_zolozfaceverify
+# 安装 antchain-zolozfaceverify
+pip install antchain-zolozfaceverify
 ```
 
 ## 问题
 
 [提交 Issue](https://github.com/alipay/antchain-openapi-prod-sdk/issues/new)，不符合指南的问题可能会立即关闭。
 
 ## 使用说明
```

### Comparing `antchain_zolozfaceverify-1.5.0/README.md` & `antchain_zolozfaceverify-1.6.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 ## Installation
 
 - **Install with pip**
 
 Python SDK uses a common package management tool named `pip`. If pip is not installed, see the [pip user guide](https://pip.pypa.io/en/stable/installing/ "pip User Guide") to install pip.
 
 ```bash
-# Install the antchain_sdk_zolozfaceverify
-pip install antchain_sdk_zolozfaceverify
+# Install the antchain-zolozfaceverify
+pip install antchain-zolozfaceverify
 ```
 
 ## Issues
 
 [Opening an Issue](https://github.com/alipay/antchain-openapi-prod-sdk/issues/new), Issues not conforming to the guidelines may be closed immediately.
 
 ## Usage
```

### Comparing `antchain_zolozfaceverify-1.5.0/antchain_sdk_zolozfaceverify/client.py` & `antchain_zolozfaceverify-1.6.0/antchain_sdk_zolozfaceverify/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -94,15 +94,15 @@
             'readTimeout': UtilClient.default_number(runtime.read_timeout, self._read_timeout),
             'connectTimeout': UtilClient.default_number(runtime.connect_timeout, self._connect_timeout),
             'httpProxy': UtilClient.default_string(runtime.http_proxy, self._http_proxy),
             'httpsProxy': UtilClient.default_string(runtime.https_proxy, self._https_proxy),
             'noProxy': UtilClient.default_string(runtime.no_proxy, self._no_proxy),
             'maxIdleConns': UtilClient.default_number(runtime.max_idle_conns, self._max_idle_conns),
             'maxIdleTimeMillis': self._max_idle_time_millis,
-            'keepAliveDurationMillis': self._keep_alive_duration_millis,
+            'keepAliveDuration': self._keep_alive_duration_millis,
             'maxRequests': self._max_requests,
             'maxRequestsPerHost': self._max_requests_per_host,
             'retry': {
                 'retryable': runtime.autoretry,
                 'maxAttempts': UtilClient.default_number(runtime.max_attempts, 3)
             },
             'backoff': {
@@ -131,15 +131,17 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.5.0'
+                    'sdk_version': '1.6.0',
+                    '_prod_code': 'ZOLOZFACEVERIFY',
+                    '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
                     'user-agent': UtilClient.get_user_agent(self._user_agent)
                 }, headers)
@@ -196,15 +198,15 @@
             'readTimeout': UtilClient.default_number(runtime.read_timeout, self._read_timeout),
             'connectTimeout': UtilClient.default_number(runtime.connect_timeout, self._connect_timeout),
             'httpProxy': UtilClient.default_string(runtime.http_proxy, self._http_proxy),
             'httpsProxy': UtilClient.default_string(runtime.https_proxy, self._https_proxy),
             'noProxy': UtilClient.default_string(runtime.no_proxy, self._no_proxy),
             'maxIdleConns': UtilClient.default_number(runtime.max_idle_conns, self._max_idle_conns),
             'maxIdleTimeMillis': self._max_idle_time_millis,
-            'keepAliveDurationMillis': self._keep_alive_duration_millis,
+            'keepAliveDuration': self._keep_alive_duration_millis,
             'maxRequests': self._max_requests,
             'maxRequestsPerHost': self._max_requests_per_host,
             'retry': {
                 'retryable': runtime.autoretry,
                 'maxAttempts': UtilClient.default_number(runtime.max_attempts, 3)
             },
             'backoff': {
@@ -233,15 +235,17 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.5.0'
+                    'sdk_version': '1.6.0',
+                    '_prod_code': 'ZOLOZFACEVERIFY',
+                    '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
                     'user-agent': UtilClient.get_user_agent(self._user_agent)
                 }, headers)
@@ -302,30 +306,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> zolozfaceverify_models.ExecFaceauthAlgorithmResponse:
         """
         Description: 金融云计算能力输出给主站使用
         Summary: 金融云计算能力输出给主站使用
         """
         UtilClient.validate_model(request)
-        return zolozfaceverify_models.ExecFaceauthAlgorithmResponse().from_map(
+        return TeaCore.from_map(
+            zolozfaceverify_models.ExecFaceauthAlgorithmResponse(),
             self.do_request('1.0', 'faceverifyzoloz.faceauth.algorithm.exec', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def exec_faceauth_algorithm_ex_async(
         self,
         request: zolozfaceverify_models.ExecFaceauthAlgorithmRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> zolozfaceverify_models.ExecFaceauthAlgorithmResponse:
         """
         Description: 金融云计算能力输出给主站使用
         Summary: 金融云计算能力输出给主站使用
         """
         UtilClient.validate_model(request)
-        return zolozfaceverify_models.ExecFaceauthAlgorithmResponse().from_map(
+        return TeaCore.from_map(
+            zolozfaceverify_models.ExecFaceauthAlgorithmResponse(),
             await self.do_request_async('1.0', 'faceverifyzoloz.faceauth.algorithm.exec', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def face_faceauth_initialize(
         self,
         request: zolozfaceverify_models.FaceFaceauthInitializeRequest,
     ) -> zolozfaceverify_models.FaceFaceauthInitializeResponse:
@@ -356,30 +362,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> zolozfaceverify_models.FaceFaceauthInitializeResponse:
         """
         Description: 调用“实人认证初始化”接口初始化认证服务并得到zimId，zimId用于唯一标识一次认证请求，后续通过zimId可以查询本次实人认证的结果
         Summary: 实人认证初始化
         """
         UtilClient.validate_model(request)
-        return zolozfaceverify_models.FaceFaceauthInitializeResponse().from_map(
+        return TeaCore.from_map(
+            zolozfaceverify_models.FaceFaceauthInitializeResponse(),
             self.do_request('1.0', 'faceverifyzoloz.faceauth.initialize.face', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def face_faceauth_initialize_ex_async(
         self,
         request: zolozfaceverify_models.FaceFaceauthInitializeRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> zolozfaceverify_models.FaceFaceauthInitializeResponse:
         """
         Description: 调用“实人认证初始化”接口初始化认证服务并得到zimId，zimId用于唯一标识一次认证请求，后续通过zimId可以查询本次实人认证的结果
         Summary: 实人认证初始化
         """
         UtilClient.validate_model(request)
-        return zolozfaceverify_models.FaceFaceauthInitializeResponse().from_map(
+        return TeaCore.from_map(
+            zolozfaceverify_models.FaceFaceauthInitializeResponse(),
             await self.do_request_async('1.0', 'faceverifyzoloz.faceauth.initialize.face', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def face_faceauth_query(
         self,
         request: zolozfaceverify_models.FaceFaceauthQueryRequest,
     ) -> zolozfaceverify_models.FaceFaceauthQueryResponse:
@@ -410,30 +418,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> zolozfaceverify_models.FaceFaceauthQueryResponse:
         """
         Description: 调用“实人认证结果查询”接口可以通过zimId查询当次认证的结果
         Summary: 实人认证查询
         """
         UtilClient.validate_model(request)
-        return zolozfaceverify_models.FaceFaceauthQueryResponse().from_map(
+        return TeaCore.from_map(
+            zolozfaceverify_models.FaceFaceauthQueryResponse(),
             self.do_request('1.0', 'faceverifyzoloz.faceauth.query.face', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def face_faceauth_query_ex_async(
         self,
         request: zolozfaceverify_models.FaceFaceauthQueryRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> zolozfaceverify_models.FaceFaceauthQueryResponse:
         """
         Description: 调用“实人认证结果查询”接口可以通过zimId查询当次认证的结果
         Summary: 实人认证查询
         """
         UtilClient.validate_model(request)
-        return zolozfaceverify_models.FaceFaceauthQueryResponse().from_map(
+        return TeaCore.from_map(
+            zolozfaceverify_models.FaceFaceauthQueryResponse(),
             await self.do_request_async('1.0', 'faceverifyzoloz.faceauth.query.face', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def identity_faceauth_servermode(
         self,
         request: zolozfaceverify_models.IdentityFaceauthServermodeRequest,
     ) -> zolozfaceverify_models.IdentityFaceauthServermodeResponse:
@@ -464,30 +474,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> zolozfaceverify_models.IdentityFaceauthServermodeResponse:
         """
         Description: 人脸纯服务端模式比对
         Summary: 人脸纯服务端模式比对
         """
         UtilClient.validate_model(request)
-        return zolozfaceverify_models.IdentityFaceauthServermodeResponse().from_map(
+        return TeaCore.from_map(
+            zolozfaceverify_models.IdentityFaceauthServermodeResponse(),
             self.do_request('1.0', 'faceverifyzoloz.faceauth.servermode.identity', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def identity_faceauth_servermode_ex_async(
         self,
         request: zolozfaceverify_models.IdentityFaceauthServermodeRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> zolozfaceverify_models.IdentityFaceauthServermodeResponse:
         """
         Description: 人脸纯服务端模式比对
         Summary: 人脸纯服务端模式比对
         """
         UtilClient.validate_model(request)
-        return zolozfaceverify_models.IdentityFaceauthServermodeResponse().from_map(
+        return TeaCore.from_map(
+            zolozfaceverify_models.IdentityFaceauthServermodeResponse(),
             await self.do_request_async('1.0', 'faceverifyzoloz.faceauth.servermode.identity', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def initialize_faceauth_web(
         self,
         request: zolozfaceverify_models.InitializeFaceauthWebRequest,
     ) -> zolozfaceverify_models.InitializeFaceauthWebResponse:
@@ -518,30 +530,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> zolozfaceverify_models.InitializeFaceauthWebResponse:
         """
         Description: 调用“H5实人认证初始化”接口初始化认证服务并得到zimId，zimId用于唯一标识一次认证请求，后续通过zimId可以查询本次实人认证的结果
         Summary: H5实人认证初始化
         """
         UtilClient.validate_model(request)
-        return zolozfaceverify_models.InitializeFaceauthWebResponse().from_map(
+        return TeaCore.from_map(
+            zolozfaceverify_models.InitializeFaceauthWebResponse(),
             self.do_request('1.0', 'faceverifyzoloz.faceauth.web.initialize', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def initialize_faceauth_web_ex_async(
         self,
         request: zolozfaceverify_models.InitializeFaceauthWebRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> zolozfaceverify_models.InitializeFaceauthWebResponse:
         """
         Description: 调用“H5实人认证初始化”接口初始化认证服务并得到zimId，zimId用于唯一标识一次认证请求，后续通过zimId可以查询本次实人认证的结果
         Summary: H5实人认证初始化
         """
         UtilClient.validate_model(request)
-        return zolozfaceverify_models.InitializeFaceauthWebResponse().from_map(
+        return TeaCore.from_map(
+            zolozfaceverify_models.InitializeFaceauthWebResponse(),
             await self.do_request_async('1.0', 'faceverifyzoloz.faceauth.web.initialize', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def query_faceauth_web(
         self,
         request: zolozfaceverify_models.QueryFaceauthWebRequest,
     ) -> zolozfaceverify_models.QueryFaceauthWebResponse:
@@ -572,30 +586,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> zolozfaceverify_models.QueryFaceauthWebResponse:
         """
         Description: H5实人认证查询
         Summary: H5实人认证查询
         """
         UtilClient.validate_model(request)
-        return zolozfaceverify_models.QueryFaceauthWebResponse().from_map(
+        return TeaCore.from_map(
+            zolozfaceverify_models.QueryFaceauthWebResponse(),
             self.do_request('1.0', 'faceverifyzoloz.faceauth.web.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def query_faceauth_web_ex_async(
         self,
         request: zolozfaceverify_models.QueryFaceauthWebRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> zolozfaceverify_models.QueryFaceauthWebResponse:
         """
         Description: H5实人认证查询
         Summary: H5实人认证查询
         """
         UtilClient.validate_model(request)
-        return zolozfaceverify_models.QueryFaceauthWebResponse().from_map(
+        return TeaCore.from_map(
+            zolozfaceverify_models.QueryFaceauthWebResponse(),
             await self.do_request_async('1.0', 'faceverifyzoloz.faceauth.web.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def query_faceauth_metering(
         self,
         request: zolozfaceverify_models.QueryFaceauthMeteringRequest,
     ) -> zolozfaceverify_models.QueryFaceauthMeteringResponse:
@@ -626,30 +642,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> zolozfaceverify_models.QueryFaceauthMeteringResponse:
         """
         Description: 提供给业务方刷脸认证计量查询接口
         Summary: 提供给业务方刷脸认证计量查询接口
         """
         UtilClient.validate_model(request)
-        return zolozfaceverify_models.QueryFaceauthMeteringResponse().from_map(
+        return TeaCore.from_map(
+            zolozfaceverify_models.QueryFaceauthMeteringResponse(),
             self.do_request('1.0', 'faceverifyzoloz.faceauth.metering.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def query_faceauth_metering_ex_async(
         self,
         request: zolozfaceverify_models.QueryFaceauthMeteringRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> zolozfaceverify_models.QueryFaceauthMeteringResponse:
         """
         Description: 提供给业务方刷脸认证计量查询接口
         Summary: 提供给业务方刷脸认证计量查询接口
         """
         UtilClient.validate_model(request)
-        return zolozfaceverify_models.QueryFaceauthMeteringResponse().from_map(
+        return TeaCore.from_map(
+            zolozfaceverify_models.QueryFaceauthMeteringResponse(),
             await self.do_request_async('1.0', 'faceverifyzoloz.faceauth.metering.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def init_faceauth_face_lite(
         self,
         request: zolozfaceverify_models.InitFaceauthFaceLiteRequest,
     ) -> zolozfaceverify_models.InitFaceauthFaceLiteResponse:
@@ -680,30 +698,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> zolozfaceverify_models.InitFaceauthFaceLiteResponse:
         """
         Description: 极简模式初始化接口，返回zimId和协议
         Summary: 极简模式初始化接口
         """
         UtilClient.validate_model(request)
-        return zolozfaceverify_models.InitFaceauthFaceLiteResponse().from_map(
+        return TeaCore.from_map(
+            zolozfaceverify_models.InitFaceauthFaceLiteResponse(),
             self.do_request('1.0', 'faceverifyzoloz.faceauth.face.lite.init', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def init_faceauth_face_lite_ex_async(
         self,
         request: zolozfaceverify_models.InitFaceauthFaceLiteRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> zolozfaceverify_models.InitFaceauthFaceLiteResponse:
         """
         Description: 极简模式初始化接口，返回zimId和协议
         Summary: 极简模式初始化接口
         """
         UtilClient.validate_model(request)
-        return zolozfaceverify_models.InitFaceauthFaceLiteResponse().from_map(
+        return TeaCore.from_map(
+            zolozfaceverify_models.InitFaceauthFaceLiteResponse(),
             await self.do_request_async('1.0', 'faceverifyzoloz.faceauth.face.lite.init', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def query_faceauth_data(
         self,
         request: zolozfaceverify_models.QueryFaceauthDataRequest,
     ) -> zolozfaceverify_models.QueryFaceauthDataResponse:
@@ -734,30 +754,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> zolozfaceverify_models.QueryFaceauthDataResponse:
         """
         Description: 数据查询，排查case
         Summary: 数据查询，排查case
         """
         UtilClient.validate_model(request)
-        return zolozfaceverify_models.QueryFaceauthDataResponse().from_map(
+        return TeaCore.from_map(
+            zolozfaceverify_models.QueryFaceauthDataResponse(),
             self.do_request('1.0', 'faceverifyzoloz.faceauth.data.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def query_faceauth_data_ex_async(
         self,
         request: zolozfaceverify_models.QueryFaceauthDataRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> zolozfaceverify_models.QueryFaceauthDataResponse:
         """
         Description: 数据查询，排查case
         Summary: 数据查询，排查case
         """
         UtilClient.validate_model(request)
-        return zolozfaceverify_models.QueryFaceauthDataResponse().from_map(
+        return TeaCore.from_map(
+            zolozfaceverify_models.QueryFaceauthDataResponse(),
             await self.do_request_async('1.0', 'faceverifyzoloz.faceauth.data.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def exec_authentication_customer_faceability(
         self,
         request: zolozfaceverify_models.ExecAuthenticationCustomerFaceabilityRequest,
     ) -> zolozfaceverify_models.ExecAuthenticationCustomerFaceabilityResponse:
@@ -788,30 +810,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> zolozfaceverify_models.ExecAuthenticationCustomerFaceabilityResponse:
         """
         Description: 提供人脸特征提取、人脸区域识别等能力接口
         Summary: 提供人脸特征提取、人脸区域识别等能力接口
         """
         UtilClient.validate_model(request)
-        return zolozfaceverify_models.ExecAuthenticationCustomerFaceabilityResponse().from_map(
+        return TeaCore.from_map(
+            zolozfaceverify_models.ExecAuthenticationCustomerFaceabilityResponse(),
             self.do_request('1.0', 'faceverifyzoloz.authentication.customer.faceability.exec', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def exec_authentication_customer_faceability_ex_async(
         self,
         request: zolozfaceverify_models.ExecAuthenticationCustomerFaceabilityRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> zolozfaceverify_models.ExecAuthenticationCustomerFaceabilityResponse:
         """
         Description: 提供人脸特征提取、人脸区域识别等能力接口
         Summary: 提供人脸特征提取、人脸区域识别等能力接口
         """
         UtilClient.validate_model(request)
-        return zolozfaceverify_models.ExecAuthenticationCustomerFaceabilityResponse().from_map(
+        return TeaCore.from_map(
+            zolozfaceverify_models.ExecAuthenticationCustomerFaceabilityResponse(),
             await self.do_request_async('1.0', 'faceverifyzoloz.authentication.customer.faceability.exec', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def init_faceauth_zim(
         self,
         request: zolozfaceverify_models.InitFaceauthZimRequest,
     ) -> zolozfaceverify_models.InitFaceauthZimResponse:
@@ -842,30 +866,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> zolozfaceverify_models.InitFaceauthZimResponse:
         """
         Description: 客户端接口初始化认证
         Summary: 客户端初始化
         """
         UtilClient.validate_model(request)
-        return zolozfaceverify_models.InitFaceauthZimResponse().from_map(
+        return TeaCore.from_map(
+            zolozfaceverify_models.InitFaceauthZimResponse(),
             self.do_request('1.0', 'faceverifyzoloz.faceauth.zim.init', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def init_faceauth_zim_ex_async(
         self,
         request: zolozfaceverify_models.InitFaceauthZimRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> zolozfaceverify_models.InitFaceauthZimResponse:
         """
         Description: 客户端接口初始化认证
         Summary: 客户端初始化
         """
         UtilClient.validate_model(request)
-        return zolozfaceverify_models.InitFaceauthZimResponse().from_map(
+        return TeaCore.from_map(
+            zolozfaceverify_models.InitFaceauthZimResponse(),
             await self.do_request_async('1.0', 'faceverifyzoloz.faceauth.zim.init', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def verify_faceauth_zim(
         self,
         request: zolozfaceverify_models.VerifyFaceauthZimRequest,
     ) -> zolozfaceverify_models.VerifyFaceauthZimResponse:
@@ -896,30 +922,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> zolozfaceverify_models.VerifyFaceauthZimResponse:
         """
         Description: 提供客户端活体检测与人脸比对服务
         Summary: 客户端人脸验证
         """
         UtilClient.validate_model(request)
-        return zolozfaceverify_models.VerifyFaceauthZimResponse().from_map(
+        return TeaCore.from_map(
+            zolozfaceverify_models.VerifyFaceauthZimResponse(),
             self.do_request('1.0', 'faceverifyzoloz.faceauth.zim.verify', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def verify_faceauth_zim_ex_async(
         self,
         request: zolozfaceverify_models.VerifyFaceauthZimRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> zolozfaceverify_models.VerifyFaceauthZimResponse:
         """
         Description: 提供客户端活体检测与人脸比对服务
         Summary: 客户端人脸验证
         """
         UtilClient.validate_model(request)
-        return zolozfaceverify_models.VerifyFaceauthZimResponse().from_map(
+        return TeaCore.from_map(
+            zolozfaceverify_models.VerifyFaceauthZimResponse(),
             await self.do_request_async('1.0', 'faceverifyzoloz.faceauth.zim.verify', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def recognize_faceauth_ocr(
         self,
         request: zolozfaceverify_models.RecognizeFaceauthOcrRequest,
     ) -> zolozfaceverify_models.RecognizeFaceauthOcrResponse:
@@ -950,30 +978,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> zolozfaceverify_models.RecognizeFaceauthOcrResponse:
         """
         Description: OCR识别接口，开放给阿里云场景
         Summary: OCR识别接口
         """
         UtilClient.validate_model(request)
-        return zolozfaceverify_models.RecognizeFaceauthOcrResponse().from_map(
+        return TeaCore.from_map(
+            zolozfaceverify_models.RecognizeFaceauthOcrResponse(),
             self.do_request('1.0', 'faceverifyzoloz.faceauth.ocr.recognize', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def recognize_faceauth_ocr_ex_async(
         self,
         request: zolozfaceverify_models.RecognizeFaceauthOcrRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> zolozfaceverify_models.RecognizeFaceauthOcrResponse:
         """
         Description: OCR识别接口，开放给阿里云场景
         Summary: OCR识别接口
         """
         UtilClient.validate_model(request)
-        return zolozfaceverify_models.RecognizeFaceauthOcrResponse().from_map(
+        return TeaCore.from_map(
+            zolozfaceverify_models.RecognizeFaceauthOcrResponse(),
             await self.do_request_async('1.0', 'faceverifyzoloz.faceauth.ocr.recognize', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def init_faceauth_websdk(
         self,
         request: zolozfaceverify_models.InitFaceauthWebsdkRequest,
     ) -> zolozfaceverify_models.InitFaceauthWebsdkResponse:
@@ -1004,30 +1034,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> zolozfaceverify_models.InitFaceauthWebsdkResponse:
         """
         Description: Web实人认证初始化
         Summary: Web实人认证初始化
         """
         UtilClient.validate_model(request)
-        return zolozfaceverify_models.InitFaceauthWebsdkResponse().from_map(
+        return TeaCore.from_map(
+            zolozfaceverify_models.InitFaceauthWebsdkResponse(),
             self.do_request('1.0', 'faceverifyzoloz.faceauth.websdk.init', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def init_faceauth_websdk_ex_async(
         self,
         request: zolozfaceverify_models.InitFaceauthWebsdkRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> zolozfaceverify_models.InitFaceauthWebsdkResponse:
         """
         Description: Web实人认证初始化
         Summary: Web实人认证初始化
         """
         UtilClient.validate_model(request)
-        return zolozfaceverify_models.InitFaceauthWebsdkResponse().from_map(
+        return TeaCore.from_map(
+            zolozfaceverify_models.InitFaceauthWebsdkResponse(),
             await self.do_request_async('1.0', 'faceverifyzoloz.faceauth.websdk.init', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def query_faceauth_websdk(
         self,
         request: zolozfaceverify_models.QueryFaceauthWebsdkRequest,
     ) -> zolozfaceverify_models.QueryFaceauthWebsdkResponse:
@@ -1058,30 +1090,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> zolozfaceverify_models.QueryFaceauthWebsdkResponse:
         """
         Description: Web实人认证查询
         Summary: Web实人认证查询
         """
         UtilClient.validate_model(request)
-        return zolozfaceverify_models.QueryFaceauthWebsdkResponse().from_map(
+        return TeaCore.from_map(
+            zolozfaceverify_models.QueryFaceauthWebsdkResponse(),
             self.do_request('1.0', 'faceverifyzoloz.faceauth.websdk.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def query_faceauth_websdk_ex_async(
         self,
         request: zolozfaceverify_models.QueryFaceauthWebsdkRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> zolozfaceverify_models.QueryFaceauthWebsdkResponse:
         """
         Description: Web实人认证查询
         Summary: Web实人认证查询
         """
         UtilClient.validate_model(request)
-        return zolozfaceverify_models.QueryFaceauthWebsdkResponse().from_map(
+        return TeaCore.from_map(
+            zolozfaceverify_models.QueryFaceauthWebsdkResponse(),
             await self.do_request_async('1.0', 'faceverifyzoloz.faceauth.websdk.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def query_faceauth_file(
         self,
         request: zolozfaceverify_models.QueryFaceauthFileRequest,
     ) -> zolozfaceverify_models.QueryFaceauthFileResponse:
@@ -1112,30 +1146,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> zolozfaceverify_models.QueryFaceauthFileResponse:
         """
         Description: zoloz提供具备权限控制的人脸图片获取接口，提供于支付宝会员等上游，控制数据风险
         Summary: 获取认证资料
         """
         UtilClient.validate_model(request)
-        return zolozfaceverify_models.QueryFaceauthFileResponse().from_map(
+        return TeaCore.from_map(
+            zolozfaceverify_models.QueryFaceauthFileResponse(),
             self.do_request('1.0', 'faceverifyzoloz.faceauth.file.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def query_faceauth_file_ex_async(
         self,
         request: zolozfaceverify_models.QueryFaceauthFileRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> zolozfaceverify_models.QueryFaceauthFileResponse:
         """
         Description: zoloz提供具备权限控制的人脸图片获取接口，提供于支付宝会员等上游，控制数据风险
         Summary: 获取认证资料
         """
         UtilClient.validate_model(request)
-        return zolozfaceverify_models.QueryFaceauthFileResponse().from_map(
+        return TeaCore.from_map(
+            zolozfaceverify_models.QueryFaceauthFileResponse(),
             await self.do_request_async('1.0', 'faceverifyzoloz.faceauth.file.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def init_faceauth_faceplus(
         self,
         request: zolozfaceverify_models.InitFaceauthFaceplusRequest,
     ) -> zolozfaceverify_models.InitFaceauthFaceplusResponse:
@@ -1166,30 +1202,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> zolozfaceverify_models.InitFaceauthFaceplusResponse:
         """
         Description: 人脸双因子认证服务端初始化
         Summary: 人脸双因子认证服务端初始化
         """
         UtilClient.validate_model(request)
-        return zolozfaceverify_models.InitFaceauthFaceplusResponse().from_map(
+        return TeaCore.from_map(
+            zolozfaceverify_models.InitFaceauthFaceplusResponse(),
             self.do_request('1.0', 'faceverifyzoloz.faceauth.faceplus.init', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def init_faceauth_faceplus_ex_async(
         self,
         request: zolozfaceverify_models.InitFaceauthFaceplusRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> zolozfaceverify_models.InitFaceauthFaceplusResponse:
         """
         Description: 人脸双因子认证服务端初始化
         Summary: 人脸双因子认证服务端初始化
         """
         UtilClient.validate_model(request)
-        return zolozfaceverify_models.InitFaceauthFaceplusResponse().from_map(
+        return TeaCore.from_map(
+            zolozfaceverify_models.InitFaceauthFaceplusResponse(),
             await self.do_request_async('1.0', 'faceverifyzoloz.faceauth.faceplus.init', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def query_faceauth_faceplus(
         self,
         request: zolozfaceverify_models.QueryFaceauthFaceplusRequest,
     ) -> zolozfaceverify_models.QueryFaceauthFaceplusResponse:
@@ -1220,30 +1258,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> zolozfaceverify_models.QueryFaceauthFaceplusResponse:
         """
         Description: 人脸双因子认证服务端查询
         Summary: 人脸双因子认证服务端查询
         """
         UtilClient.validate_model(request)
-        return zolozfaceverify_models.QueryFaceauthFaceplusResponse().from_map(
+        return TeaCore.from_map(
+            zolozfaceverify_models.QueryFaceauthFaceplusResponse(),
             self.do_request('1.0', 'faceverifyzoloz.faceauth.faceplus.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def query_faceauth_faceplus_ex_async(
         self,
         request: zolozfaceverify_models.QueryFaceauthFaceplusRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> zolozfaceverify_models.QueryFaceauthFaceplusResponse:
         """
         Description: 人脸双因子认证服务端查询
         Summary: 人脸双因子认证服务端查询
         """
         UtilClient.validate_model(request)
-        return zolozfaceverify_models.QueryFaceauthFaceplusResponse().from_map(
+        return TeaCore.from_map(
+            zolozfaceverify_models.QueryFaceauthFaceplusResponse(),
             await self.do_request_async('1.0', 'faceverifyzoloz.faceauth.faceplus.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def init_faceauth_face_wish(
         self,
         request: zolozfaceverify_models.InitFaceauthFaceWishRequest,
     ) -> zolozfaceverify_models.InitFaceauthFaceWishResponse:
@@ -1274,30 +1314,32 @@
         runtime: util_models.RuntimeOptions,
     ) -> zolozfaceverify_models.InitFaceauthFaceWishResponse:
         """
         Description: 意愿核身认证服务端初始化
         Summary: 意愿核身认证服务端初始化
         """
         UtilClient.validate_model(request)
-        return zolozfaceverify_models.InitFaceauthFaceWishResponse().from_map(
+        return TeaCore.from_map(
+            zolozfaceverify_models.InitFaceauthFaceWishResponse(),
             self.do_request('1.0', 'faceverifyzoloz.faceauth.face.wish.init', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def init_faceauth_face_wish_ex_async(
         self,
         request: zolozfaceverify_models.InitFaceauthFaceWishRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> zolozfaceverify_models.InitFaceauthFaceWishResponse:
         """
         Description: 意愿核身认证服务端初始化
         Summary: 意愿核身认证服务端初始化
         """
         UtilClient.validate_model(request)
-        return zolozfaceverify_models.InitFaceauthFaceWishResponse().from_map(
+        return TeaCore.from_map(
+            zolozfaceverify_models.InitFaceauthFaceWishResponse(),
             await self.do_request_async('1.0', 'faceverifyzoloz.faceauth.face.wish.init', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     def verify_faceauth_video(
         self,
         request: zolozfaceverify_models.VerifyFaceauthVideoRequest,
     ) -> zolozfaceverify_models.VerifyFaceauthVideoResponse:
@@ -1328,25 +1370,83 @@
         runtime: util_models.RuntimeOptions,
     ) -> zolozfaceverify_models.VerifyFaceauthVideoResponse:
         """
         Description: 人脸视频认证
         Summary: 人脸视频认证
         """
         UtilClient.validate_model(request)
-        return zolozfaceverify_models.VerifyFaceauthVideoResponse().from_map(
+        return TeaCore.from_map(
+            zolozfaceverify_models.VerifyFaceauthVideoResponse(),
             self.do_request('1.0', 'faceverifyzoloz.faceauth.video.verify', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
     async def verify_faceauth_video_ex_async(
         self,
         request: zolozfaceverify_models.VerifyFaceauthVideoRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> zolozfaceverify_models.VerifyFaceauthVideoResponse:
         """
         Description: 人脸视频认证
         Summary: 人脸视频认证
         """
         UtilClient.validate_model(request)
-        return zolozfaceverify_models.VerifyFaceauthVideoResponse().from_map(
+        return TeaCore.from_map(
+            zolozfaceverify_models.VerifyFaceauthVideoResponse(),
             await self.do_request_async('1.0', 'faceverifyzoloz.faceauth.video.verify', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
+
+    def init_faceauth_nfc(
+        self,
+        request: zolozfaceverify_models.InitFaceauthNfcRequest,
+    ) -> zolozfaceverify_models.InitFaceauthNfcResponse:
+        """
+        Description: 实证NFC服务端初始化
+        Summary: 实证NFC服务端初始化
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.init_faceauth_nfc_ex(request, headers, runtime)
+
+    async def init_faceauth_nfc_async(
+        self,
+        request: zolozfaceverify_models.InitFaceauthNfcRequest,
+    ) -> zolozfaceverify_models.InitFaceauthNfcResponse:
+        """
+        Description: 实证NFC服务端初始化
+        Summary: 实证NFC服务端初始化
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.init_faceauth_nfc_ex_async(request, headers, runtime)
+
+    def init_faceauth_nfc_ex(
+        self,
+        request: zolozfaceverify_models.InitFaceauthNfcRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> zolozfaceverify_models.InitFaceauthNfcResponse:
+        """
+        Description: 实证NFC服务端初始化
+        Summary: 实证NFC服务端初始化
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            zolozfaceverify_models.InitFaceauthNfcResponse(),
+            self.do_request('1.0', 'faceverifyzoloz.faceauth.nfc.init', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def init_faceauth_nfc_ex_async(
+        self,
+        request: zolozfaceverify_models.InitFaceauthNfcRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> zolozfaceverify_models.InitFaceauthNfcResponse:
+        """
+        Description: 实证NFC服务端初始化
+        Summary: 实证NFC服务端初始化
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            zolozfaceverify_models.InitFaceauthNfcResponse(),
+            await self.do_request_async('1.0', 'faceverifyzoloz.faceauth.nfc.init', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
```

### Comparing `antchain_zolozfaceverify-1.5.0/antchain_sdk_zolozfaceverify/models.py` & `antchain_zolozfaceverify-1.6.0/antchain_sdk_zolozfaceverify/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,14 +66,18 @@
         # 每个目标主机的最大连接数（分主机域名的长链接最大总数
         self.max_requests_per_host = max_requests_per_host
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.access_key_id is not None:
             result['accessKeyId'] = self.access_key_id
         if self.access_key_secret is not None:
             result['accessKeySecret'] = self.access_key_secret
         if self.security_token is not None:
             result['securityToken'] = self.security_token
@@ -179,14 +183,18 @@
         # 可用性检查开始
         self.usable_start_pv = usable_start_pv
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.identify_passed_pv is not None:
             result['identify_passed_pv'] = self.identify_passed_pv
         if self.identify_succeed_pv is not None:
             result['identify_succeed_pv'] = self.identify_succeed_pv
         if self.metering_type is not None:
             result['metering_type'] = self.metering_type
@@ -244,14 +252,18 @@
             for k in self.metering_data_detail_list:
                 if k:
                     k.validate()
         if self.start_time is not None:
             self.validate_pattern(self.start_time, 'start_time', '\\d{4}[-]\\d{1,2}[-]\\d{1,2}[T]\\d{2}:\\d{2}:\\d{2}([Z]|([\\.]\\d{1,9})?[\\+]\\d{2}[\\:]?\\d{2})')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.end_time is not None:
             result['end_time'] = self.end_time
         result['metering_data_detail_list'] = []
         if self.metering_data_detail_list is not None:
             for k in self.metering_data_detail_list:
                 result['metering_data_detail_list'].append(k.to_map() if k else None)
@@ -301,14 +313,18 @@
     def validate(self):
         self.validate_required(self.biz_id, 'biz_id')
         self.validate_required(self.channel, 'channel')
         self.validate_required(self.img_str, 'img_str')
         self.validate_required(self.img_type, 'img_type')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.product_instance_id is not None:
             result['product_instance_id'] = self.product_instance_id
         if self.biz_id is not None:
             result['biz_id'] = self.biz_id
@@ -358,14 +374,18 @@
         # 算法结果，json格式
         self.algo_result = algo_result
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -420,14 +440,18 @@
     def validate(self):
         self.validate_required(self.biz_id, 'biz_id')
         self.validate_required(self.identity_param, 'identity_param')
         self.validate_required(self.metainfo, 'metainfo')
         self.validate_required(self.ref_img_oss_obj, 'ref_img_oss_obj')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.product_instance_id is not None:
             result['product_instance_id'] = self.product_instance_id
         if self.biz_id is not None:
             result['biz_id'] = self.biz_id
@@ -497,14 +521,18 @@
     def validate(self):
         self.validate_required(self.extern_info, 'extern_info')
         self.validate_required(self.result_code_sub, 'result_code_sub')
         self.validate_required(self.result_msg_sub, 'result_msg_sub')
         self.validate_required(self.zim_id, 'zim_id')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -557,14 +585,18 @@
         self.zim_id = zim_id
 
     def validate(self):
         self.validate_required(self.biz_id, 'biz_id')
         self.validate_required(self.zim_id, 'zim_id')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.product_instance_id is not None:
             result['product_instance_id'] = self.product_instance_id
         if self.biz_id is not None:
             result['biz_id'] = self.biz_id
@@ -614,14 +646,18 @@
 
     def validate(self):
         self.validate_required(self.extern_info, 'extern_info')
         self.validate_required(self.result_code_sub, 'result_code_sub')
         self.validate_required(self.result_msg_sub, 'result_msg_sub')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -688,14 +724,18 @@
         # 比对源照片oss中转方式上传
         self.ref_img_oss_obj = ref_img_oss_obj
 
     def validate(self):
         self.validate_required(self.biz_id, 'biz_id')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.product_instance_id is not None:
             result['product_instance_id'] = self.product_instance_id
         if self.auth_img is not None:
             result['auth_img'] = self.auth_img
@@ -767,14 +807,18 @@
         # 明细返回码对应的文案
         self.result_msg_sub = result_msg_sub
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -831,14 +875,18 @@
         # 比对源图片
         self.ref_img = ref_img
 
     def validate(self):
         self.validate_required(self.biz_id, 'biz_id')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.product_instance_id is not None:
             result['product_instance_id'] = self.product_instance_id
         if self.biz_id is not None:
             result['biz_id'] = self.biz_id
@@ -901,14 +949,18 @@
         # 实人认证id
         self.zim_id = zim_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -961,14 +1013,18 @@
         self.zim_id = zim_id
 
     def validate(self):
         self.validate_required(self.biz_id, 'biz_id')
         self.validate_required(self.zim_id, 'zim_id')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.product_instance_id is not None:
             result['product_instance_id'] = self.product_instance_id
         if self.biz_id is not None:
             result['biz_id'] = self.biz_id
@@ -1016,14 +1072,18 @@
         # result_code_sub对应的文案
         self.result_msg_sub = result_msg_sub
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -1088,14 +1148,18 @@
         if self.end_time is not None:
             self.validate_pattern(self.end_time, 'end_time', '\\d{4}[-]\\d{1,2}[-]\\d{1,2}[T]\\d{2}:\\d{2}:\\d{2}([Z]|([\\.]\\d{1,9})?[\\+]\\d{2}[\\:]?\\d{2})')
         self.validate_required(self.start_time, 'start_time')
         if self.start_time is not None:
             self.validate_pattern(self.start_time, 'start_time', '\\d{4}[-]\\d{1,2}[-]\\d{1,2}[T]\\d{2}:\\d{2}:\\d{2}([Z]|([\\.]\\d{1,9})?[\\+]\\d{2}[\\:]?\\d{2})')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.product_instance_id is not None:
             result['product_instance_id'] = self.product_instance_id
         if self.biz_id is not None:
             result['biz_id'] = self.biz_id
@@ -1146,14 +1210,18 @@
         self.metering_data = metering_data
 
     def validate(self):
         if self.metering_data:
             self.metering_data.validate()
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -1205,14 +1273,18 @@
 
     def validate(self):
         self.validate_required(self.biz_id, 'biz_id')
         self.validate_required(self.identity_param, 'identity_param')
         self.validate_required(self.metainfo, 'metainfo')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.product_instance_id is not None:
             result['product_instance_id'] = self.product_instance_id
         if self.biz_id is not None:
             result['biz_id'] = self.biz_id
@@ -1278,14 +1350,18 @@
         # 刷脸认证唯一标识。如果初始化失败则为空，可通过返回码分析具体原因
         self.zim_id = zim_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -1339,14 +1415,18 @@
         self.data_url = data_url
 
     def validate(self):
         self.validate_required(self.biz_id, 'biz_id')
         self.validate_required(self.data_url, 'data_url')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.product_instance_id is not None:
             result['product_instance_id'] = self.product_instance_id
         if self.biz_id is not None:
             result['biz_id'] = self.biz_id
@@ -1384,14 +1464,18 @@
         # 查询结果详情
         self.data = data
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -1441,14 +1525,18 @@
         self.validate_required(self.ability, 'ability')
         self.validate_required(self.alg_ver, 'alg_ver')
         self.validate_required(self.auth_img, 'auth_img')
         self.validate_required(self.biz_id, 'biz_id')
         self.validate_required(self.scene_code, 'scene_code')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.product_instance_id is not None:
             result['product_instance_id'] = self.product_instance_id
         if self.ability is not None:
             result['ability'] = self.ability
@@ -1495,14 +1583,18 @@
         # 异常信息的文本描述
         self.result_msg = result_msg
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -1554,14 +1646,18 @@
         self.zim_principal = zim_principal
 
     def validate(self):
         self.validate_required(self.meta_info, 'meta_info')
         self.validate_required(self.zim_id, 'zim_id')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.product_instance_id is not None:
             result['product_instance_id'] = self.product_instance_id
         if self.biz_data is not None:
             result['biz_data'] = self.biz_data
@@ -1641,14 +1737,18 @@
         # 实人认证id
         self.zimi_id = zimi_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -1716,14 +1816,18 @@
         self.zim_data_oss_obj = zim_data_oss_obj
 
     def validate(self):
         self.validate_required(self.zim_data, 'zim_data')
         self.validate_required(self.zim_id, 'zim_id')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.product_instance_id is not None:
             result['product_instance_id'] = self.product_instance_id
         if self.extern_param is not None:
             result['extern_param'] = self.extern_param
@@ -1787,14 +1891,18 @@
         # 验证返回明细码
         self.validation_ret_code = validation_ret_code
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -1868,14 +1976,18 @@
     def validate(self):
         self.validate_required(self.data_context, 'data_context')
         self.validate_required(self.data_type, 'data_type')
         self.validate_required(self.side, 'side')
         self.validate_required(self.zim_id, 'zim_id')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.product_instance_id is not None:
             result['product_instance_id'] = self.product_instance_id
         if self.data_context is not None:
             result['data_context'] = self.data_context
@@ -1964,14 +2076,18 @@
         # zimid
         self.zim_id = zim_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -2047,14 +2163,18 @@
         # 比对源照片oss方式中转
         self.ref_img_oss_obj = ref_img_oss_obj
 
     def validate(self):
         self.validate_required(self.biz_id, 'biz_id')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.product_instance_id is not None:
             result['product_instance_id'] = self.product_instance_id
         if self.biz_id is not None:
             result['biz_id'] = self.biz_id
@@ -2121,14 +2241,18 @@
         # 实人认证id
         self.zim_id = zim_id
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -2181,14 +2305,18 @@
         self.zim_id = zim_id
 
     def validate(self):
         self.validate_required(self.biz_id, 'biz_id')
         self.validate_required(self.zim_id, 'zim_id')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.product_instance_id is not None:
             result['product_instance_id'] = self.product_instance_id
         if self.biz_id is not None:
             result['biz_id'] = self.biz_id
@@ -2236,14 +2364,18 @@
         # result_code_sub对应的文案
         self.result_msg_sub = result_msg_sub
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -2288,14 +2420,18 @@
         # 预留扩展业务参数
         self.extern_param = extern_param
 
     def validate(self):
         self.validate_required(self.zim_id, 'zim_id')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.product_instance_id is not None:
             result['product_instance_id'] = self.product_instance_id
         if self.zim_id is not None:
             result['zim_id'] = self.zim_id
@@ -2339,14 +2475,18 @@
         # result_code_sub对应的文案
         self.result_msg_sub = result_msg_sub
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -2405,14 +2545,18 @@
 
     def validate(self):
         self.validate_required(self.biz_id, 'biz_id')
         self.validate_required(self.identity_param, 'identity_param')
         self.validate_required(self.metainfo, 'metainfo')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.product_instance_id is not None:
             result['product_instance_id'] = self.product_instance_id
         if self.biz_id is not None:
             result['biz_id'] = self.biz_id
@@ -2475,14 +2619,18 @@
         # 外部参数
         self.extern_info = extern_info
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -2535,14 +2683,18 @@
         self.extern_param = extern_param
 
     def validate(self):
         self.validate_required(self.zim_id, 'zim_id')
         self.validate_required(self.biz_id, 'biz_id')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.product_instance_id is not None:
             result['product_instance_id'] = self.product_instance_id
         if self.zim_id is not None:
             result['zim_id'] = self.zim_id
@@ -2590,14 +2742,18 @@
         # 外部参数
         self.extern_info = extern_info
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -2656,14 +2812,18 @@
 
     def validate(self):
         self.validate_required(self.biz_id, 'biz_id')
         self.validate_required(self.identity_param, 'identity_param')
         self.validate_required(self.metainfo, 'metainfo')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.product_instance_id is not None:
             result['product_instance_id'] = self.product_instance_id
         if self.biz_id is not None:
             result['biz_id'] = self.biz_id
@@ -2726,14 +2886,18 @@
         # 结果信息
         self.result_msg_sub = result_msg_sub
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -2803,14 +2967,18 @@
         # 比对源照片oss中转方式上传
         self.ref_img_oss_obj = ref_img_oss_obj
 
     def validate(self):
         self.validate_required(self.biz_id, 'biz_id')
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.product_instance_id is not None:
             result['product_instance_id'] = self.product_instance_id
         if self.auth_img is not None:
             result['auth_img'] = self.auth_img
@@ -2882,14 +3050,18 @@
         # 明细返回码对应的文案
         self.result_msg_sub = result_msg_sub
 
     def validate(self):
         pass
 
     def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
@@ -2912,9 +3084,150 @@
         if m.get('extern_info') is not None:
             self.extern_info = m.get('extern_info')
         if m.get('result_code_sub') is not None:
             self.result_code_sub = m.get('result_code_sub')
         if m.get('result_msg_sub') is not None:
             self.result_msg_sub = m.get('result_msg_sub')
         return self
+
+
+class InitFaceauthNfcRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        biz_id: str = None,
+        identity_param: str = None,
+        metainfo: str = None,
+        extern_param: str = None,
+        operation_type: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 租户请求的唯一标志，该标识作为对账的关键信息，商户要保证其唯一性
+        self.biz_id = biz_id
+        # 身份，需要公钥加密
+        self.identity_param = identity_param
+        # 客户端采集
+        self.metainfo = metainfo
+        # 外部参数
+        self.extern_param = extern_param
+        # 操作类型
+        self.operation_type = operation_type
+
+    def validate(self):
+        self.validate_required(self.biz_id, 'biz_id')
+        self.validate_required(self.identity_param, 'identity_param')
+        self.validate_required(self.metainfo, 'metainfo')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.biz_id is not None:
+            result['biz_id'] = self.biz_id
+        if self.identity_param is not None:
+            result['identity_param'] = self.identity_param
+        if self.metainfo is not None:
+            result['metainfo'] = self.metainfo
+        if self.extern_param is not None:
+            result['extern_param'] = self.extern_param
+        if self.operation_type is not None:
+            result['operation_type'] = self.operation_type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('biz_id') is not None:
+            self.biz_id = m.get('biz_id')
+        if m.get('identity_param') is not None:
+            self.identity_param = m.get('identity_param')
+        if m.get('metainfo') is not None:
+            self.metainfo = m.get('metainfo')
+        if m.get('extern_param') is not None:
+            self.extern_param = m.get('extern_param')
+        if m.get('operation_type') is not None:
+            self.operation_type = m.get('operation_type')
+        return self
+
+
+class InitFaceauthNfcResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        zim_id: str = None,
+        extern_info: str = None,
+        result_code_sub: str = None,
+        result_msg_sub: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # z-abcd
+        self.zim_id = zim_id
+        # 预留扩展结果
+        self.extern_info = extern_info
+        # 结果码
+        self.result_code_sub = result_code_sub
+        # 结果信息
+        self.result_msg_sub = result_msg_sub
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.zim_id is not None:
+            result['zim_id'] = self.zim_id
+        if self.extern_info is not None:
+            result['extern_info'] = self.extern_info
+        if self.result_code_sub is not None:
+            result['result_code_sub'] = self.result_code_sub
+        if self.result_msg_sub is not None:
+            result['result_msg_sub'] = self.result_msg_sub
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('zim_id') is not None:
+            self.zim_id = m.get('zim_id')
+        if m.get('extern_info') is not None:
+            self.extern_info = m.get('extern_info')
+        if m.get('result_code_sub') is not None:
+            self.result_code_sub = m.get('result_code_sub')
+        if m.get('result_msg_sub') is not None:
+            self.result_msg_sub = m.get('result_msg_sub')
+        return self
```

### Comparing `antchain_zolozfaceverify-1.5.0/antchain_zolozfaceverify.egg-info/PKG-INFO` & `antchain_zolozfaceverify-1.6.0/antchain_zolozfaceverify.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain-zolozfaceverify
-Version: 1.5.0
+Version: 1.6.0
 Summary: Ant Chain ZOLOZFACEVERIFY SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         
@@ -17,16 +17,16 @@
         ## Installation
         
         - **Install with pip**
         
         Python SDK uses a common package management tool named `pip`. If pip is not installed, see the [pip user guide](https://pip.pypa.io/en/stable/installing/ "pip User Guide") to install pip.
         
         ```bash
-        # Install the antchain_sdk_zolozfaceverify
-        pip install antchain_sdk_zolozfaceverify
+        # Install the antchain-zolozfaceverify
+        pip install antchain-zolozfaceverify
         ```
         
         ## Issues
         
         [Opening an Issue](https://github.com/alipay/antchain-openapi-prod-sdk/issues/new), Issues not conforming to the guidelines may be closed immediately.
         
         ## Usage
```

### Comparing `antchain_zolozfaceverify-1.5.0/setup.py` & `antchain_zolozfaceverify-1.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,29 +20,29 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for antchain_zolozfaceverify.
 
-Created on 25/05/2022
+Created on 13/06/2023
 
 @author: Ant Chain SDK
 """
 
 PACKAGE = "antchain_sdk_zolozfaceverify"
 NAME = "antchain_zolozfaceverify" or "alibabacloud-package"
 DESCRIPTION = "Ant Chain ZOLOZFACEVERIFY SDK Library for Python"
 AUTHOR = "Ant Chain SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/alipay/antchain-openapi-prod-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
     "antchain_alipay_util>=1.0.1, <2.0.0",
-    "alibabacloud_tea_util>=0.3.5, <1.0.0",
+    "alibabacloud_tea_util>=0.3.8, <1.0.0",
     "alibabacloud_rpc_util>=0.0.4, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
```

