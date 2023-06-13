# Comparing `tmp/antchain_bot-1.8.70.tar.gz` & `tmp/antchain_bot-1.8.76.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_bot-1.8.70.tar", last modified: Wed May 17 06:30:00 2023, max compression
+gzip compressed data, was "dist/antchain_bot-1.8.76.tar", last modified: Tue Jun 13 05:41:26 2023, max compression
```

## Comparing `antchain_bot-1.8.70.tar` & `antchain_bot-1.8.76.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:30:00.000000 antchain_bot-1.8.70/
--rw-r--r--   0 root         (0) root         (0)      600 2023-05-17 06:30:00.000000 antchain_bot-1.8.70/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-17 06:30:00.000000 antchain_bot-1.8.70/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2163 2023-05-17 06:30:00.000000 antchain_bot-1.8.70/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      804 2023-05-17 06:30:00.000000 antchain_bot-1.8.70/README-CN.md
--rw-r--r--   0 root         (0) root         (0)      990 2023-05-17 06:30:00.000000 antchain_bot-1.8.70/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:30:00.000000 antchain_bot-1.8.70/antchain_bot.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2163 2023-05-17 06:30:00.000000 antchain_bot-1.8.70/antchain_bot.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      323 2023-05-17 06:30:00.000000 antchain_bot-1.8.70/antchain_bot.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 06:30:00.000000 antchain_bot-1.8.70/antchain_bot.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-05-17 06:30:00.000000 antchain_bot-1.8.70/antchain_bot.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-05-17 06:30:00.000000 antchain_bot-1.8.70/antchain_bot.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 06:30:00.000000 antchain_bot-1.8.70/antchain_sdk_bot/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-17 06:30:00.000000 antchain_bot-1.8.70/antchain_sdk_bot/__init__.py
--rw-r--r--   0 root         (0) root         (0)   423032 2023-05-17 06:30:00.000000 antchain_bot-1.8.70/antchain_sdk_bot/client.py
--rw-r--r--   0 root         (0) root         (0)  1124816 2023-05-17 06:30:00.000000 antchain_bot-1.8.70/antchain_sdk_bot/models.py
--rw-r--r--   0 root         (0) root         (0)       73 2023-05-17 06:30:00.000000 antchain_bot-1.8.70/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2488 2023-05-17 06:30:00.000000 antchain_bot-1.8.70/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 05:41:26.000000 antchain_bot-1.8.76/
+-rw-r--r--   0 root         (0) root         (0)      600 2023-06-13 05:41:26.000000 antchain_bot-1.8.76/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-13 05:41:26.000000 antchain_bot-1.8.76/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2163 2023-06-13 05:41:26.000000 antchain_bot-1.8.76/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      804 2023-06-13 05:41:26.000000 antchain_bot-1.8.76/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)      990 2023-06-13 05:41:26.000000 antchain_bot-1.8.76/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 05:41:26.000000 antchain_bot-1.8.76/antchain_bot.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2163 2023-06-13 05:41:26.000000 antchain_bot-1.8.76/antchain_bot.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      323 2023-06-13 05:41:26.000000 antchain_bot-1.8.76/antchain_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 05:41:26.000000 antchain_bot-1.8.76/antchain_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-06-13 05:41:26.000000 antchain_bot-1.8.76/antchain_bot.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-06-13 05:41:26.000000 antchain_bot-1.8.76/antchain_bot.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 05:41:26.000000 antchain_bot-1.8.76/antchain_sdk_bot/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 05:41:26.000000 antchain_bot-1.8.76/antchain_sdk_bot/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   425326 2023-06-13 05:41:26.000000 antchain_bot-1.8.76/antchain_sdk_bot/client.py
+-rw-r--r--   0 root         (0) root         (0)  1132219 2023-06-13 05:41:26.000000 antchain_bot-1.8.76/antchain_sdk_bot/models.py
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-13 05:41:26.000000 antchain_bot-1.8.76/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2488 2023-06-13 05:41:26.000000 antchain_bot-1.8.76/setup.py
```

### Comparing `antchain_bot-1.8.70/LICENSE` & `antchain_bot-1.8.76/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_bot-1.8.70/PKG-INFO` & `antchain_bot-1.8.76/antchain_bot.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: antchain_bot
-Version: 1.8.70
+Name: antchain-bot
+Version: 1.8.76
 Summary: Ant Chain BOT SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_bot-1.8.70/README-CN.md` & `antchain_bot-1.8.76/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_bot-1.8.70/README.md` & `antchain_bot-1.8.76/README.md`

 * *Files identical despite different names*

### Comparing `antchain_bot-1.8.70/antchain_bot.egg-info/PKG-INFO` & `antchain_bot-1.8.76/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: antchain-bot
-Version: 1.8.70
+Name: antchain_bot
+Version: 1.8.76
 Summary: Ant Chain BOT SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_bot-1.8.70/antchain_sdk_bot/client.py` & `antchain_bot-1.8.76/antchain_sdk_bot/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.8.70',
+                    'sdk_version': '1.8.76',
                     '_prod_code': 'BOT',
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
-                    'sdk_version': '1.8.70',
+                    'sdk_version': '1.8.76',
                     '_prod_code': 'BOT',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -4449,14 +4449,70 @@
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
             bot_models.SaveIotbasicCustomerResponse(),
             await self.do_request_async('1.0', 'blockchain.bot.iotbasic.customer.save', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
+    def notify_thirddevice_message(
+        self,
+        request: bot_models.NotifyThirddeviceMessageRequest,
+    ) -> bot_models.NotifyThirddeviceMessageResponse:
+        """
+        Description: IoT设备平台-设备消息同步
+        Summary: IoT设备平台-设备消息同步
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.notify_thirddevice_message_ex(request, headers, runtime)
+
+    async def notify_thirddevice_message_async(
+        self,
+        request: bot_models.NotifyThirddeviceMessageRequest,
+    ) -> bot_models.NotifyThirddeviceMessageResponse:
+        """
+        Description: IoT设备平台-设备消息同步
+        Summary: IoT设备平台-设备消息同步
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.notify_thirddevice_message_ex_async(request, headers, runtime)
+
+    def notify_thirddevice_message_ex(
+        self,
+        request: bot_models.NotifyThirddeviceMessageRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> bot_models.NotifyThirddeviceMessageResponse:
+        """
+        Description: IoT设备平台-设备消息同步
+        Summary: IoT设备平台-设备消息同步
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            bot_models.NotifyThirddeviceMessageResponse(),
+            self.do_request('1.0', 'blockchain.bot.thirddevice.message.notify', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def notify_thirddevice_message_ex_async(
+        self,
+        request: bot_models.NotifyThirddeviceMessageRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> bot_models.NotifyThirddeviceMessageResponse:
+        """
+        Description: IoT设备平台-设备消息同步
+        Summary: IoT设备平台-设备消息同步
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            bot_models.NotifyThirddeviceMessageResponse(),
+            await self.do_request_async('1.0', 'blockchain.bot.thirddevice.message.notify', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
     def query_iotplatform_purchaseorder(
         self,
         request: bot_models.QueryIotplatformPurchaseorderRequest,
     ) -> bot_models.QueryIotplatformPurchaseorderResponse:
         """
         Description: 根据设备串号查询采购设备
         Summary: 根据设备串号查询采购设备
```

### Comparing `antchain_bot-1.8.70/antchain_sdk_bot/models.py` & `antchain_bot-1.8.76/antchain_sdk_bot/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2837,25 +2837,28 @@
     def __init__(
         self,
         data_model_id: str = None,
         data_model_name: str = None,
         data_model: str = None,
         biz_type: str = None,
         customer_version: str = None,
+        data_demo: str = None,
     ):
         # 数据模型Id
         self.data_model_id = data_model_id
         # 数据模型名称
         self.data_model_name = data_model_name
         # 数据模型
         self.data_model = data_model
         # 数据模型类别
         self.biz_type = biz_type
         # 用户自定义版本
         self.customer_version = customer_version
+        # 数据样例
+        self.data_demo = data_demo
 
     def validate(self):
         self.validate_required(self.data_model_id, 'data_model_id')
         self.validate_required(self.data_model, 'data_model')
 
     def to_map(self):
         _map = super().to_map()
@@ -2869,28 +2872,32 @@
             result['data_model_name'] = self.data_model_name
         if self.data_model is not None:
             result['data_model'] = self.data_model
         if self.biz_type is not None:
             result['biz_type'] = self.biz_type
         if self.customer_version is not None:
             result['customer_version'] = self.customer_version
+        if self.data_demo is not None:
+            result['data_demo'] = self.data_demo
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('data_model_id') is not None:
             self.data_model_id = m.get('data_model_id')
         if m.get('data_model_name') is not None:
             self.data_model_name = m.get('data_model_name')
         if m.get('data_model') is not None:
             self.data_model = m.get('data_model')
         if m.get('biz_type') is not None:
             self.biz_type = m.get('biz_type')
         if m.get('customer_version') is not None:
             self.customer_version = m.get('customer_version')
+        if m.get('data_demo') is not None:
+            self.data_demo = m.get('data_demo')
         return self
 
 
 class BaiQrcodeGenerateRespData(TeaModel):
     def __init__(
         self,
         generate_result: str = None,
@@ -5625,35 +5632,43 @@
         return self
 
 
 class SendCollectorResult(TeaModel):
     def __init__(
         self,
         tx_hash: str = None,
+        original_index: int = None,
     ):
         # 数据内容content的上链交易哈希
         self.tx_hash = tx_hash
+        # 原入参的数组索引
+        self.original_index = original_index
 
     def validate(self):
         self.validate_required(self.tx_hash, 'tx_hash')
+        self.validate_required(self.original_index, 'original_index')
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.tx_hash is not None:
             result['tx_hash'] = self.tx_hash
+        if self.original_index is not None:
+            result['original_index'] = self.original_index
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('tx_hash') is not None:
             self.tx_hash = m.get('tx_hash')
+        if m.get('original_index') is not None:
+            self.original_index = m.get('original_index')
         return self
 
 
 class GoodsDigitalFingerprintRegisterResultData(TeaModel):
     def __init__(
         self,
         success: bool = None,
@@ -5992,42 +6007,50 @@
 
 
 class TrustiotDeviceIdMap(TeaModel):
     def __init__(
         self,
         trustiot_device_id: int = None,
         device_id: str = None,
+        chain_device_id: str = None,
     ):
         # 可信设备ID
         self.trustiot_device_id = trustiot_device_id
         # 设备ID
         self.device_id = device_id
+        # 设备注册的上链哈希
+        self.chain_device_id = chain_device_id
 
     def validate(self):
         self.validate_required(self.trustiot_device_id, 'trustiot_device_id')
         self.validate_required(self.device_id, 'device_id')
+        self.validate_required(self.chain_device_id, 'chain_device_id')
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.trustiot_device_id is not None:
             result['trustiot_device_id'] = self.trustiot_device_id
         if self.device_id is not None:
             result['device_id'] = self.device_id
+        if self.chain_device_id is not None:
+            result['chain_device_id'] = self.chain_device_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('trustiot_device_id') is not None:
             self.trustiot_device_id = m.get('trustiot_device_id')
         if m.get('device_id') is not None:
             self.device_id = m.get('device_id')
+        if m.get('chain_device_id') is not None:
+            self.chain_device_id = m.get('chain_device_id')
         return self
 
 
 class ProductKeyPageResponse(TeaModel):
     def __init__(
         self,
         page_index: int = None,
@@ -18063,14 +18086,127 @@
         if m.get('result_msg') is not None:
             self.result_msg = m.get('result_msg')
         if m.get('success') is not None:
             self.success = m.get('success')
         return self
 
 
+class NotifyThirddeviceMessageRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        device_did: str = None,
+        command: str = None,
+        signature: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 设备did
+        self.device_did = device_did
+        # 设备信息同步命令
+        self.command = command
+        # 设备签名，用设备pri_key 进行签名，只对deviceDid加签
+        self.signature = signature
+
+    def validate(self):
+        self.validate_required(self.device_did, 'device_did')
+        self.validate_required(self.command, 'command')
+        self.validate_required(self.signature, 'signature')
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
+        if self.device_did is not None:
+            result['device_did'] = self.device_did
+        if self.command is not None:
+            result['command'] = self.command
+        if self.signature is not None:
+            result['signature'] = self.signature
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('device_did') is not None:
+            self.device_did = m.get('device_did')
+        if m.get('command') is not None:
+            self.command = m.get('command')
+        if m.get('signature') is not None:
+            self.signature = m.get('signature')
+        return self
+
+
+class NotifyThirddeviceMessageResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        success: bool = None,
+        command: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 处理结果
+        self.success = success
+        # 设备信息同步命令
+        self.command = command
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
+        if self.success is not None:
+            result['success'] = self.success
+        if self.command is not None:
+            result['command'] = self.command
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
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        if m.get('command') is not None:
+            self.command = m.get('command')
+        return self
+
+
 class QueryIotplatformPurchaseorderRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
         tenant_id: str = None,
         serial_number: str = None,
@@ -18913,26 +19049,29 @@
         self,
         auth_token: str = None,
         product_instance_id: str = None,
         data_model: str = None,
         data_model_name: str = None,
         biz_type: str = None,
         customer_version: str = None,
+        data_demo: str = None,
     ):
         # OAuth模式下的授权token
         self.auth_token = auth_token
         self.product_instance_id = product_instance_id
         # 数据模型
         self.data_model = data_model
         # 数据模型名称
         self.data_model_name = data_model_name
         # 数据模型类别
         self.biz_type = biz_type
         # 用户自定义版本
         self.customer_version = customer_version
+        # 数据样例
+        self.data_demo = data_demo
 
     def validate(self):
         self.validate_required(self.data_model, 'data_model')
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -18947,14 +19086,16 @@
             result['data_model'] = self.data_model
         if self.data_model_name is not None:
             result['data_model_name'] = self.data_model_name
         if self.biz_type is not None:
             result['biz_type'] = self.biz_type
         if self.customer_version is not None:
             result['customer_version'] = self.customer_version
+        if self.data_demo is not None:
+            result['data_demo'] = self.data_demo
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('auth_token') is not None:
             self.auth_token = m.get('auth_token')
         if m.get('product_instance_id') is not None:
@@ -18963,14 +19104,16 @@
             self.data_model = m.get('data_model')
         if m.get('data_model_name') is not None:
             self.data_model_name = m.get('data_model_name')
         if m.get('biz_type') is not None:
             self.biz_type = m.get('biz_type')
         if m.get('customer_version') is not None:
             self.customer_version = m.get('customer_version')
+        if m.get('data_demo') is not None:
+            self.data_demo = m.get('data_demo')
         return self
 
 
 class CreateDeviceDatamodelResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
@@ -22841,34 +22984,38 @@
 class SendCollectorBychainidmulRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
         content: List[CollectContent] = None,
         nonce: str = None,
+        wait_check_and_hash: bool = None,
     ):
         # OAuth模式下的授权token
         self.auth_token = auth_token
         self.product_instance_id = product_instance_id
         # 上传数据
         # 
         # 
         self.content = content
         # 随机业务号，防重放
         # 
         # 
         self.nonce = nonce
+        # 开启后接口返回值中包含txHash
+        self.wait_check_and_hash = wait_check_and_hash
 
     def validate(self):
         self.validate_required(self.content, 'content')
         if self.content:
             for k in self.content:
                 if k:
                     k.validate()
         self.validate_required(self.nonce, 'nonce')
+        self.validate_required(self.wait_check_and_hash, 'wait_check_and_hash')
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -22878,14 +23025,16 @@
             result['product_instance_id'] = self.product_instance_id
         result['content'] = []
         if self.content is not None:
             for k in self.content:
                 result['content'].append(k.to_map() if k else None)
         if self.nonce is not None:
             result['nonce'] = self.nonce
+        if self.wait_check_and_hash is not None:
+            result['wait_check_and_hash'] = self.wait_check_and_hash
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('auth_token') is not None:
             self.auth_token = m.get('auth_token')
         if m.get('product_instance_id') is not None:
@@ -22893,68 +23042,86 @@
         self.content = []
         if m.get('content') is not None:
             for k in m.get('content'):
                 temp_model = CollectContent()
                 self.content.append(temp_model.from_map(k))
         if m.get('nonce') is not None:
             self.nonce = m.get('nonce')
+        if m.get('wait_check_and_hash') is not None:
+            self.wait_check_and_hash = m.get('wait_check_and_hash')
         return self
 
 
 class SendCollectorBychainidmulResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
+        result_list: List[SendCollectorResult] = None,
     ):
         # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
         # 结果码，一般OK表示调用成功
         self.result_code = result_code
         # 异常信息的文本描述
         self.result_msg = result_msg
+        # 数据上链哈希
+        self.result_list = result_list
 
     def validate(self):
-        pass
+        if self.result_list:
+            for k in self.result_list:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
+        result['result_list'] = []
+        if self.result_list is not None:
+            for k in self.result_list:
+                result['result_list'].append(k.to_map() if k else None)
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('req_msg_id') is not None:
             self.req_msg_id = m.get('req_msg_id')
         if m.get('result_code') is not None:
             self.result_code = m.get('result_code')
         if m.get('result_msg') is not None:
             self.result_msg = m.get('result_msg')
+        self.result_list = []
+        if m.get('result_list') is not None:
+            for k in m.get('result_list'):
+                temp_model = SendCollectorResult()
+                self.result_list.append(temp_model.from_map(k))
         return self
 
 
 class SendCollectorDevicebizdataRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
         data_model_id: str = None,
         nonce: str = None,
         content: List[BizContentGroup] = None,
         scene: str = None,
+        wait_check_and_hash: bool = None,
     ):
         # OAuth模式下的授权token
         self.auth_token = auth_token
         self.product_instance_id = product_instance_id
         # 数据模型Id
         # 
         # 
@@ -22963,23 +23130,26 @@
         # 
         # 
         self.nonce = nonce
         # 上传数据
         self.content = content
         # 场景码，与content中的chainDeviceId至少有一个不为空
         self.scene = scene
+        # 开启后，接口返回值中包含txHash
+        self.wait_check_and_hash = wait_check_and_hash
 
     def validate(self):
         self.validate_required(self.data_model_id, 'data_model_id')
         self.validate_required(self.nonce, 'nonce')
         self.validate_required(self.content, 'content')
         if self.content:
             for k in self.content:
                 if k:
                     k.validate()
+        self.validate_required(self.wait_check_and_hash, 'wait_check_and_hash')
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -22993,14 +23163,16 @@
             result['nonce'] = self.nonce
         result['content'] = []
         if self.content is not None:
             for k in self.content:
                 result['content'].append(k.to_map() if k else None)
         if self.scene is not None:
             result['scene'] = self.scene
+        if self.wait_check_and_hash is not None:
+            result['wait_check_and_hash'] = self.wait_check_and_hash
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('auth_token') is not None:
             self.auth_token = m.get('auth_token')
         if m.get('product_instance_id') is not None:
@@ -23012,56 +23184,73 @@
         self.content = []
         if m.get('content') is not None:
             for k in m.get('content'):
                 temp_model = BizContentGroup()
                 self.content.append(temp_model.from_map(k))
         if m.get('scene') is not None:
             self.scene = m.get('scene')
+        if m.get('wait_check_and_hash') is not None:
+            self.wait_check_and_hash = m.get('wait_check_and_hash')
         return self
 
 
 class SendCollectorDevicebizdataResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
+        result_list: List[SendCollectorResult] = None,
     ):
         # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
         # 结果码，一般OK表示调用成功
         self.result_code = result_code
         # 异常信息的文本描述
         self.result_msg = result_msg
+        # 数据上链哈希
+        self.result_list = result_list
 
     def validate(self):
-        pass
+        if self.result_list:
+            for k in self.result_list:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.req_msg_id is not None:
             result['req_msg_id'] = self.req_msg_id
         if self.result_code is not None:
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
+        result['result_list'] = []
+        if self.result_list is not None:
+            for k in self.result_list:
+                result['result_list'].append(k.to_map() if k else None)
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('req_msg_id') is not None:
             self.req_msg_id = m.get('req_msg_id')
         if m.get('result_code') is not None:
             self.result_code = m.get('result_code')
         if m.get('result_msg') is not None:
             self.result_msg = m.get('result_msg')
+        self.result_list = []
+        if m.get('result_list') is not None:
+            for k in m.get('result_list'):
+                temp_model = SendCollectorResult()
+                self.result_list.append(temp_model.from_map(k))
         return self
 
 
 class UpdateDeviceInfobydeviceRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
```

### Comparing `antchain_bot-1.8.70/setup.py` & `antchain_bot-1.8.76/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for antchain_bot.
 
-Created on 17/05/2023
+Created on 13/06/2023
 
 @author: Ant Chain SDK
 """
 
 PACKAGE = "antchain_sdk_bot"
 NAME = "antchain_bot" or "alibabacloud-package"
 DESCRIPTION = "Ant Chain BOT SDK Library for Python"
```

