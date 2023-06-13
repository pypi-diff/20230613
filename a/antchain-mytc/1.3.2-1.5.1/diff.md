# Comparing `tmp/antchain_mytc-1.3.2.tar.gz` & `tmp/antchain_mytc-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_mytc-1.3.2.tar", last modified: Mon May 22 08:53:55 2023, max compression
+gzip compressed data, was "dist/antchain_mytc-1.5.1.tar", last modified: Tue Jun 13 02:09:28 2023, max compression
```

## Comparing `antchain_mytc-1.3.2.tar` & `antchain_mytc-1.5.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 08:53:55.000000 antchain_mytc-1.3.2/
--rw-r--r--   0 root         (0) root         (0)      600 2023-05-22 08:53:55.000000 antchain_mytc-1.3.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-22 08:53:55.000000 antchain_mytc-1.3.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2168 2023-05-22 08:53:55.000000 antchain_mytc-1.3.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      807 2023-05-22 08:53:55.000000 antchain_mytc-1.3.2/README-CN.md
--rw-r--r--   0 root         (0) root         (0)      993 2023-05-22 08:53:55.000000 antchain_mytc-1.3.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 08:53:55.000000 antchain_mytc-1.3.2/antchain_mytc.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2168 2023-05-22 08:53:55.000000 antchain_mytc-1.3.2/antchain_mytc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      331 2023-05-22 08:53:55.000000 antchain_mytc-1.3.2/antchain_mytc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 08:53:55.000000 antchain_mytc-1.3.2/antchain_mytc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-05-22 08:53:55.000000 antchain_mytc-1.3.2/antchain_mytc.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-05-22 08:53:55.000000 antchain_mytc-1.3.2/antchain_mytc.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 08:53:55.000000 antchain_mytc-1.3.2/antchain_sdk_mytc/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-22 08:53:55.000000 antchain_mytc-1.3.2/antchain_sdk_mytc/__init__.py
--rw-r--r--   0 root         (0) root         (0)    76005 2023-05-22 08:53:55.000000 antchain_mytc-1.3.2/antchain_sdk_mytc/client.py
--rw-r--r--   0 root         (0) root         (0)   144991 2023-05-22 08:53:55.000000 antchain_mytc-1.3.2/antchain_sdk_mytc/models.py
--rw-r--r--   0 root         (0) root         (0)       73 2023-05-22 08:53:55.000000 antchain_mytc-1.3.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2493 2023-05-22 08:53:55.000000 antchain_mytc-1.3.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:09:28.000000 antchain_mytc-1.5.1/
+-rw-r--r--   0 root         (0) root         (0)      600 2023-06-13 02:09:27.000000 antchain_mytc-1.5.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-13 02:09:27.000000 antchain_mytc-1.5.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2168 2023-06-13 02:09:28.000000 antchain_mytc-1.5.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      807 2023-06-13 02:09:27.000000 antchain_mytc-1.5.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)      993 2023-06-13 02:09:27.000000 antchain_mytc-1.5.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:09:28.000000 antchain_mytc-1.5.1/antchain_mytc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2168 2023-06-13 02:09:28.000000 antchain_mytc-1.5.1/antchain_mytc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      331 2023-06-13 02:09:28.000000 antchain_mytc-1.5.1/antchain_mytc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 02:09:28.000000 antchain_mytc-1.5.1/antchain_mytc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-06-13 02:09:28.000000 antchain_mytc-1.5.1/antchain_mytc.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-06-13 02:09:28.000000 antchain_mytc-1.5.1/antchain_mytc.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 02:09:28.000000 antchain_mytc-1.5.1/antchain_sdk_mytc/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-13 02:09:27.000000 antchain_mytc-1.5.1/antchain_sdk_mytc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    80369 2023-06-13 02:09:27.000000 antchain_mytc-1.5.1/antchain_sdk_mytc/client.py
+-rw-r--r--   0 root         (0) root         (0)   150064 2023-06-13 02:09:27.000000 antchain_mytc-1.5.1/antchain_sdk_mytc/models.py
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-13 02:09:28.000000 antchain_mytc-1.5.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2493 2023-06-13 02:09:27.000000 antchain_mytc-1.5.1/setup.py
```

### Comparing `antchain_mytc-1.3.2/LICENSE` & `antchain_mytc-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_mytc-1.3.2/PKG-INFO` & `antchain_mytc-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain_mytc
-Version: 1.3.2
+Version: 1.5.1
 Summary: Ant Chain MYTC SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_mytc-1.3.2/README-CN.md` & `antchain_mytc-1.5.1/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_mytc-1.3.2/README.md` & `antchain_mytc-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `antchain_mytc-1.3.2/antchain_mytc.egg-info/PKG-INFO` & `antchain_mytc-1.5.1/antchain_mytc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain-mytc
-Version: 1.3.2
+Version: 1.5.1
 Summary: Ant Chain MYTC SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_mytc-1.3.2/antchain_sdk_mytc/client.py` & `antchain_mytc-1.5.1/antchain_sdk_mytc/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,15 +131,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.3.2',
+                    'sdk_version': '1.5.1',
                     '_prod_code': 'MYTC',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -235,15 +235,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.3.2',
+                    'sdk_version': '1.5.1',
                     '_prod_code': 'MYTC',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -451,14 +451,104 @@
             request.file_id = upload_resp.file_id
         UtilClient.validate_model(request)
         return TeaCore.from_map(
             mytc_models.CheckCodeFakeResponse(),
             await self.do_request_async('1.0', 'antchain.mytc.code.fake.check', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
+    def check_code_fakescreen(
+        self,
+        request: mytc_models.CheckCodeFakescreenRequest,
+    ) -> mytc_models.CheckCodeFakescreenResponse:
+        """
+        Description: 二维码防伪防屏拍图片验证
+        Summary: 二维码防伪防屏拍图片验证
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.check_code_fakescreen_ex(request, headers, runtime)
+
+    async def check_code_fakescreen_async(
+        self,
+        request: mytc_models.CheckCodeFakescreenRequest,
+    ) -> mytc_models.CheckCodeFakescreenResponse:
+        """
+        Description: 二维码防伪防屏拍图片验证
+        Summary: 二维码防伪防屏拍图片验证
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.check_code_fakescreen_ex_async(request, headers, runtime)
+
+    def check_code_fakescreen_ex(
+        self,
+        request: mytc_models.CheckCodeFakescreenRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> mytc_models.CheckCodeFakescreenResponse:
+        """
+        Description: 二维码防伪防屏拍图片验证
+        Summary: 二维码防伪防屏拍图片验证
+        """
+        if not UtilClient.is_unset(request.file_object):
+            upload_req = mytc_models.CreateAntcloudGatewayxFileUploadRequest(
+                auth_token=request.auth_token,
+                api_code='antchain.mytc.code.fakescreen.check',
+                file_name=request.file_object_name
+            )
+            upload_resp = self.create_antcloud_gatewayx_file_upload_ex(upload_req, headers, runtime)
+            if not AntchainUtils.is_success(upload_resp.result_code, 'ok'):
+                check_code_fakescreen_response = mytc_models.CheckCodeFakescreenResponse(
+                    req_msg_id=upload_resp.req_msg_id,
+                    result_code=upload_resp.result_code,
+                    result_msg=upload_resp.result_msg
+                )
+                return check_code_fakescreen_response
+            upload_headers = AntchainUtils.parse_upload_headers(upload_resp.upload_headers)
+            AntchainUtils.put_object(request.file_object, upload_headers, upload_resp.upload_url)
+            request.file_id = upload_resp.file_id
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            mytc_models.CheckCodeFakescreenResponse(),
+            self.do_request('1.0', 'antchain.mytc.code.fakescreen.check', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def check_code_fakescreen_ex_async(
+        self,
+        request: mytc_models.CheckCodeFakescreenRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> mytc_models.CheckCodeFakescreenResponse:
+        """
+        Description: 二维码防伪防屏拍图片验证
+        Summary: 二维码防伪防屏拍图片验证
+        """
+        if not UtilClient.is_unset(request.file_object):
+            upload_req = mytc_models.CreateAntcloudGatewayxFileUploadRequest(
+                auth_token=request.auth_token,
+                api_code='antchain.mytc.code.fakescreen.check',
+                file_name=request.file_object_name
+            )
+            upload_resp = await self.create_antcloud_gatewayx_file_upload_ex_async(upload_req, headers, runtime)
+            if not AntchainUtils.is_success(upload_resp.result_code, 'ok'):
+                check_code_fakescreen_response = mytc_models.CheckCodeFakescreenResponse(
+                    req_msg_id=upload_resp.req_msg_id,
+                    result_code=upload_resp.result_code,
+                    result_msg=upload_resp.result_msg
+                )
+                return check_code_fakescreen_response
+            upload_headers = AntchainUtils.parse_upload_headers(upload_resp.upload_headers)
+            await AntchainUtils.put_object_async(request.file_object, upload_headers, upload_resp.upload_url)
+            request.file_id = upload_resp.file_id
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            mytc_models.CheckCodeFakescreenResponse(),
+            await self.do_request_async('1.0', 'antchain.mytc.code.fakescreen.check', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
     def init_anti_imagesync(
         self,
         request: mytc_models.InitAntiImagesyncRequest,
     ) -> mytc_models.InitAntiImagesyncResponse:
         """
         Description: 防伪码平台防伪底图上传，初始化上传记录
         Summary: 防伪码平台防伪底图上传初始化
```

### Comparing `antchain_mytc-1.3.2/antchain_sdk_mytc/models.py` & `antchain_mytc-1.5.1/antchain_sdk_mytc/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -956,33 +956,29 @@
         self,
         auth_token: str = None,
         product_instance_id: str = None,
         device_type: str = None,
         file_object: BinaryIO = None,
         file_object_name: str = None,
         file_id: str = None,
-        image_str: str = None,
     ):
         # OAuth模式下的授权token
         self.auth_token = auth_token
         self.product_instance_id = product_instance_id
         # 设备型号
         self.device_type = device_type
         # 图片文件id，通过小程序拍照，上传的二维码图片信息。
         # 待上传文件
         self.file_object = file_object
         # 待上传文件名
         self.file_object_name = file_object_name
         self.file_id = file_id
-        # Base64格式的图片数据
-        # 
-        self.image_str = image_str
 
     def validate(self):
-        pass
+        self.validate_required(self.file_id, 'file_id')
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -994,16 +990,14 @@
             result['device_type'] = self.device_type
         if self.file_object is not None:
             result['fileObject'] = self.file_object
         if self.file_object_name is not None:
             result['fileObjectName'] = self.file_object_name
         if self.file_id is not None:
             result['file_id'] = self.file_id
-        if self.image_str is not None:
-            result['image_str'] = self.image_str
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('auth_token') is not None:
             self.auth_token = m.get('auth_token')
         if m.get('product_instance_id') is not None:
@@ -1012,16 +1006,14 @@
             self.device_type = m.get('device_type')
         if m.get('fileObject') is not None:
             self.file_object = m.get('fileObject')
         if m.get('fileObjectName') is not None:
             self.file_object_name = m.get('fileObjectName')
         if m.get('file_id') is not None:
             self.file_id = m.get('file_id')
-        if m.get('image_str') is not None:
-            self.image_str = m.get('image_str')
         return self
 
 
 class CheckCodeFakeResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
@@ -1080,14 +1072,157 @@
         if m.get('detect_code') is not None:
             self.detect_code = m.get('detect_code')
         if m.get('detect_message') is not None:
             self.detect_message = m.get('detect_message')
         return self
 
 
+class CheckCodeFakescreenRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        device_type: str = None,
+        file_object: BinaryIO = None,
+        file_object_name: str = None,
+        file_id: str = None,
+        pair_id: str = None,
+        file_type: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 设备型号
+        self.device_type = device_type
+        # 闪光前图片
+        # 待上传文件
+        self.file_object = file_object
+        # 待上传文件名
+        self.file_object_name = file_object_name
+        self.file_id = file_id
+        # 配对标识，闪光前后需要用同一个配对标识。
+        self.pair_id = pair_id
+        # 文件类型.
+        # unflashed: 未闪光图片
+        # flashed: 闪光后图片
+        self.file_type = file_type
+
+    def validate(self):
+        self.validate_required(self.file_id, 'file_id')
+        self.validate_required(self.pair_id, 'pair_id')
+        self.validate_required(self.file_type, 'file_type')
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
+        if self.device_type is not None:
+            result['device_type'] = self.device_type
+        if self.file_object is not None:
+            result['fileObject'] = self.file_object
+        if self.file_object_name is not None:
+            result['fileObjectName'] = self.file_object_name
+        if self.file_id is not None:
+            result['file_id'] = self.file_id
+        if self.pair_id is not None:
+            result['pair_id'] = self.pair_id
+        if self.file_type is not None:
+            result['file_type'] = self.file_type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('device_type') is not None:
+            self.device_type = m.get('device_type')
+        if m.get('fileObject') is not None:
+            self.file_object = m.get('fileObject')
+        if m.get('fileObjectName') is not None:
+            self.file_object_name = m.get('fileObjectName')
+        if m.get('file_id') is not None:
+            self.file_id = m.get('file_id')
+        if m.get('pair_id') is not None:
+            self.pair_id = m.get('pair_id')
+        if m.get('file_type') is not None:
+            self.file_type = m.get('file_type')
+        return self
+
+
+class CheckCodeFakescreenResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        detect_success: bool = None,
+        detect_code: str = None,
+        detect_message: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 验真是否成功
+        self.detect_success = detect_success
+        # 返回编码
+        self.detect_code = detect_code
+        # 调用返回信息
+        self.detect_message = detect_message
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
+        if self.detect_success is not None:
+            result['detect_success'] = self.detect_success
+        if self.detect_code is not None:
+            result['detect_code'] = self.detect_code
+        if self.detect_message is not None:
+            result['detect_message'] = self.detect_message
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
+        if m.get('detect_success') is not None:
+            self.detect_success = m.get('detect_success')
+        if m.get('detect_code') is not None:
+            self.detect_code = m.get('detect_code')
+        if m.get('detect_message') is not None:
+            self.detect_message = m.get('detect_message')
+        return self
+
+
 class InitAntiImagesyncRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
         code_type: str = None,
         batch_no: str = None,
@@ -1100,15 +1235,14 @@
         self.code_type = code_type
         # 防伪码批次号
         self.batch_no = batch_no
         # 批次下要上传的防伪码总数
         self.total = total
 
     def validate(self):
-        self.validate_required(self.code_type, 'code_type')
         self.validate_required(self.batch_no, 'batch_no')
         self.validate_required(self.total, 'total')
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -1198,103 +1332,101 @@
 
 
 class UploadAntiImagesyncRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
-        code_type: str = None,
         code: str = None,
-        batch_no: str = None,
         file_object: BinaryIO = None,
         file_object_name: str = None,
         file_id: str = None,
+        batch_no: str = None,
     ):
         # OAuth模式下的授权token
         self.auth_token = auth_token
         self.product_instance_id = product_instance_id
-        # 防伪码类型
-        self.code_type = code_type
         # 防伪码码值
         self.code = code
-        # 批次号码
-        self.batch_no = batch_no
         # 文件id
         # 待上传文件
         self.file_object = file_object
         # 待上传文件名
         self.file_object_name = file_object_name
         self.file_id = file_id
+        # 防伪码批次号，若不填写，则会获取当天最新批次号。若批次不存在，则创建一个新的批次。
+        self.batch_no = batch_no
 
     def validate(self):
-        self.validate_required(self.code_type, 'code_type')
         self.validate_required(self.code, 'code')
-        self.validate_required(self.batch_no, 'batch_no')
+        self.validate_required(self.file_id, 'file_id')
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.product_instance_id is not None:
             result['product_instance_id'] = self.product_instance_id
-        if self.code_type is not None:
-            result['code_type'] = self.code_type
         if self.code is not None:
             result['code'] = self.code
-        if self.batch_no is not None:
-            result['batch_no'] = self.batch_no
         if self.file_object is not None:
             result['fileObject'] = self.file_object
         if self.file_object_name is not None:
             result['fileObjectName'] = self.file_object_name
         if self.file_id is not None:
             result['file_id'] = self.file_id
+        if self.batch_no is not None:
+            result['batch_no'] = self.batch_no
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('auth_token') is not None:
             self.auth_token = m.get('auth_token')
         if m.get('product_instance_id') is not None:
             self.product_instance_id = m.get('product_instance_id')
-        if m.get('code_type') is not None:
-            self.code_type = m.get('code_type')
         if m.get('code') is not None:
             self.code = m.get('code')
-        if m.get('batch_no') is not None:
-            self.batch_no = m.get('batch_no')
         if m.get('fileObject') is not None:
             self.file_object = m.get('fileObject')
         if m.get('fileObjectName') is not None:
             self.file_object_name = m.get('fileObjectName')
         if m.get('file_id') is not None:
             self.file_id = m.get('file_id')
+        if m.get('batch_no') is not None:
+            self.batch_no = m.get('batch_no')
         return self
 
 
 class UploadAntiImagesyncResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
         code: str = None,
+        batch_no: str = None,
+        count: int = None,
     ):
         # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
         # 结果码，一般OK表示调用成功
         self.result_code = result_code
         # 异常信息的文本描述
         self.result_msg = result_msg
         # 防伪码码值
         self.code = code
+        # 批次号
+        self.batch_no = batch_no
+        # 该批次号，已上传底图次数
+        self.count = count
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -1305,94 +1437,98 @@
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
         if self.code is not None:
             result['code'] = self.code
+        if self.batch_no is not None:
+            result['batch_no'] = self.batch_no
+        if self.count is not None:
+            result['count'] = self.count
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('req_msg_id') is not None:
             self.req_msg_id = m.get('req_msg_id')
         if m.get('result_code') is not None:
             self.result_code = m.get('result_code')
         if m.get('result_msg') is not None:
             self.result_msg = m.get('result_msg')
         if m.get('code') is not None:
             self.code = m.get('code')
+        if m.get('batch_no') is not None:
+            self.batch_no = m.get('batch_no')
+        if m.get('count') is not None:
+            self.count = m.get('count')
         return self
 
 
 class FinishAntiImagesyncRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
         batch_no: str = None,
-        code_type: str = None,
     ):
         # OAuth模式下的授权token
         self.auth_token = auth_token
         self.product_instance_id = product_instance_id
         # 批次号
         self.batch_no = batch_no
-        # 防伪码类型
-        self.code_type = code_type
 
     def validate(self):
         self.validate_required(self.batch_no, 'batch_no')
-        self.validate_required(self.code_type, 'code_type')
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.product_instance_id is not None:
             result['product_instance_id'] = self.product_instance_id
         if self.batch_no is not None:
             result['batch_no'] = self.batch_no
-        if self.code_type is not None:
-            result['code_type'] = self.code_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('auth_token') is not None:
             self.auth_token = m.get('auth_token')
         if m.get('product_instance_id') is not None:
             self.product_instance_id = m.get('product_instance_id')
         if m.get('batch_no') is not None:
             self.batch_no = m.get('batch_no')
-        if m.get('code_type') is not None:
-            self.code_type = m.get('code_type')
         return self
 
 
 class FinishAntiImagesyncResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
         batch_no: str = None,
+        count: int = None,
     ):
         # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
         # 结果码，一般OK表示调用成功
         self.result_code = result_code
         # 异常信息的文本描述
         self.result_msg = result_msg
         # 批次号
         self.batch_no = batch_no
+        # 该批次号，已上传底图次数
+        # 
+        self.count = count
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -1403,26 +1539,30 @@
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
         if self.batch_no is not None:
             result['batch_no'] = self.batch_no
+        if self.count is not None:
+            result['count'] = self.count
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('req_msg_id') is not None:
             self.req_msg_id = m.get('req_msg_id')
         if m.get('result_code') is not None:
             self.result_code = m.get('result_code')
         if m.get('result_msg') is not None:
             self.result_msg = m.get('result_msg')
         if m.get('batch_no') is not None:
             self.batch_no = m.get('batch_no')
+        if m.get('count') is not None:
+            self.count = m.get('count')
         return self
 
 
 class CreateAntiQrcodeimageRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
```

### Comparing `antchain_mytc-1.3.2/setup.py` & `antchain_mytc-1.5.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for antchain_mytc.
 
-Created on 22/05/2023
+Created on 13/06/2023
 
 @author: Ant Chain SDK
 """
 
 PACKAGE = "antchain_sdk_mytc"
 NAME = "antchain_mytc" or "alibabacloud-package"
 DESCRIPTION = "Ant Chain MYTC SDK Library for Python"
```

