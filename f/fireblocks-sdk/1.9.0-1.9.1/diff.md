# Comparing `tmp/fireblocks_sdk-1.9.0.tar.gz` & `tmp/fireblocks_sdk-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fireblocks_sdk-1.9.0.tar", last modified: Wed Nov 24 10:08:12 2021, max compression
+gzip compressed data, was "fireblocks_sdk-1.9.1.tar", last modified: Thu Dec  2 14:59:19 2021, max compression
```

## Comparing `fireblocks_sdk-1.9.0.tar` & `fireblocks_sdk-1.9.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-24 10:08:12.245602 fireblocks_sdk-1.9.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1067 2021-11-24 10:07:57.000000 fireblocks_sdk-1.9.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)      554 2021-11-24 10:08:12.245602 fireblocks_sdk-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      611 2021-11-24 10:07:57.000000 fireblocks_sdk-1.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-24 10:08:12.241602 fireblocks_sdk-1.9.0/fireblocks_sdk/
--rw-r--r--   0 runner    (1001) docker     (121)      146 2021-11-24 10:07:57.000000 fireblocks_sdk-1.9.0/fireblocks_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6766 2021-11-24 10:07:57.000000 fireblocks_sdk-1.9.0/fireblocks_sdk/api_types.py
--rw-r--r--   0 runner    (1001) docker     (121)    49943 2021-11-24 10:07:57.000000 fireblocks_sdk-1.9.0/fireblocks_sdk/sdk.py
--rw-r--r--   0 runner    (1001) docker     (121)      824 2021-11-24 10:07:57.000000 fireblocks_sdk-1.9.0/fireblocks_sdk/sdk_token_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-24 10:08:12.245602 fireblocks_sdk-1.9.0/fireblocks_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      554 2021-11-24 10:08:12.000000 fireblocks_sdk-1.9.0/fireblocks_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      343 2021-11-24 10:08:12.000000 fireblocks_sdk-1.9.0/fireblocks_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-24 10:08:12.000000 fireblocks_sdk-1.9.0/fireblocks_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       48 2021-11-24 10:08:12.000000 fireblocks_sdk-1.9.0/fireblocks_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2021-11-24 10:08:12.000000 fireblocks_sdk-1.9.0/fireblocks_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       79 2021-11-24 10:08:12.245602 fireblocks_sdk-1.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      709 2021-11-24 10:08:03.000000 fireblocks_sdk-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-02 14:59:19.865375 fireblocks_sdk-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (121)     1067 2021-12-02 14:59:05.000000 fireblocks_sdk-1.9.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      554 2021-12-02 14:59:19.865375 fireblocks_sdk-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      611 2021-12-02 14:59:05.000000 fireblocks_sdk-1.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-02 14:59:19.865375 fireblocks_sdk-1.9.1/fireblocks_sdk/
+-rw-r--r--   0 runner    (1001) docker     (121)      146 2021-12-02 14:59:05.000000 fireblocks_sdk-1.9.1/fireblocks_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6766 2021-12-02 14:59:05.000000 fireblocks_sdk-1.9.1/fireblocks_sdk/api_types.py
+-rw-r--r--   0 runner    (1001) docker     (121)    49510 2021-12-02 14:59:05.000000 fireblocks_sdk-1.9.1/fireblocks_sdk/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (121)      824 2021-12-02 14:59:05.000000 fireblocks_sdk-1.9.1/fireblocks_sdk/sdk_token_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-02 14:59:19.865375 fireblocks_sdk-1.9.1/fireblocks_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      554 2021-12-02 14:59:19.000000 fireblocks_sdk-1.9.1/fireblocks_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      343 2021-12-02 14:59:19.000000 fireblocks_sdk-1.9.1/fireblocks_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-02 14:59:19.000000 fireblocks_sdk-1.9.1/fireblocks_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       48 2021-12-02 14:59:19.000000 fireblocks_sdk-1.9.1/fireblocks_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       15 2021-12-02 14:59:19.000000 fireblocks_sdk-1.9.1/fireblocks_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       79 2021-12-02 14:59:19.865375 fireblocks_sdk-1.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      709 2021-12-02 14:59:12.000000 fireblocks_sdk-1.9.1/setup.py
```

### Comparing `fireblocks_sdk-1.9.0/LICENSE.txt` & `fireblocks_sdk-1.9.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fireblocks_sdk-1.9.0/PKG-INFO` & `fireblocks_sdk-1.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: fireblocks_sdk
-Version: 1.9.0
+Version: 1.9.1
 Summary: Fireblocks python SDK
 Home-page: https://github.com/fireblocks/fireblocks-sdk-py
 License: MIT
-Download-URL: https://github.com/fireblocks/fireblocks-sdk-py/archive/v1.9.0.tar.gz
+Download-URL: https://github.com/fireblocks/fireblocks-sdk-py/archive/v1.9.1.tar.gz
 Keywords: Fireblocks,SDK
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `fireblocks_sdk-1.9.0/README.md` & `fireblocks_sdk-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `fireblocks_sdk-1.9.0/fireblocks_sdk/api_types.py` & `fireblocks_sdk-1.9.1/fireblocks_sdk/api_types.py`

 * *Files identical despite different names*

### Comparing `fireblocks_sdk-1.9.0/fireblocks_sdk/sdk.py` & `fireblocks_sdk-1.9.1/fireblocks_sdk/sdk.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,30 @@
 from .sdk_token_provider import SdkTokenProvider
 from .api_types import FireblocksApiException, TRANSACTION_TYPES, TRANSACTION_STATUS_TYPES, PEER_TYPES, \
     TransferPeerPath, DestinationTransferPeerPath, TransferTicketTerm, TRANSACTION_TRANSFER, SIGNING_ALGORITHM, \
     UnsignedMessage, FEE_LEVEL
 from fireblocks_sdk.api_types import TransactionDestination
 
 
+def handle_response(response, page_mode=False):
+    response_data = response.json()
+    if response.status_code >= 300:
+        if type(response_data) is dict:
+            error_code = response_data.get("code")
+            raise FireblocksApiException("Got an error from fireblocks server: " + response.text, error_code)
+        else:
+            raise FireblocksApiException("Got an error from fireblocks server: " + response.text)
+    else:
+        if page_mode:
+            return {'transactions': response_data,
+                    'pageDetails': {'prevPage': response.headers.get('prev-page', ''),
+                                    'nextPage': response.headers.get('next-page', '')}}
+        return response_data
+
+
 class FireblocksSDK(object):
 
     def __init__(self, private_key, api_key, api_base_url="https://api.fireblocks.io", timeout=None):
         """Creates a new Fireblocks API Client.
 
         Args:
             private_key (str): A string representation of your private key (in PEM format)
@@ -1138,39 +1154,25 @@
         token = self.token_provider.sign_jwt(path)
         headers = {
             "X-API-Key": self.api_key,
             "Authorization": f"Bearer {token}"
         }
 
         response = requests.get(self.base_url + path, headers=headers, timeout=self.timeout)
-        response_data = response.json()
-        if response.status_code >= 300:
-            error_code = response_data.get('code')
-            raise FireblocksApiException("Got an error from fireblocks server: " + response.text, error_code)
-        else:
-            if page_mode:
-                return {'transactions': response_data,
-                        'pageDetails': {'prevPage': response.headers.get('prev-page', ''),
-                                        'nextPage': response.headers.get('next-page', '')}}
-            else:
-                return response_data
+        return handle_response(response, page_mode)
 
     def _delete_request(self, path):
         token = self.token_provider.sign_jwt(path)
         headers = {
             "X-API-Key": self.api_key,
             "Authorization": f"Bearer {token}"
         }
 
         response = requests.delete(self.base_url + path, headers=headers, timeout=self.timeout)
-        if response.status_code >= 300:
-            error_code = response.json().get("code")
-            raise FireblocksApiException("Got an error from fireblocks server: " + response.text, error_code)
-        else:
-            return response.json()
+        return handle_response(response)
 
     def _post_request(self, path, body={}, idempotency_key=None):
         token = self.token_provider.sign_jwt(path, body)
         if idempotency_key is None:
             headers = {
                 "X-API-Key": self.api_key,
                 "Authorization": f"Bearer {token}"
@@ -1179,27 +1181,19 @@
             headers = {
                 "X-API-Key": self.api_key,
                 "Authorization": f"Bearer {token}",
                 "Idempotency-Key": idempotency_key
             }
 
         response = requests.post(self.base_url + path, headers=headers, json=body, timeout=self.timeout)
-        if response.status_code >= 300:
-            error_code = response.json().get("code")
-            raise FireblocksApiException("Got an error from fireblocks server: " + response.text, error_code)
-        else:
-            return response.json()
+        return handle_response(response)
 
     def _put_request(self, path, body={}):
         token = self.token_provider.sign_jwt(path, body)
         headers = {
             "X-API-Key": self.api_key,
             "Authorization": f"Bearer {token}",
             "Content-Type": "application/json"
         }
 
         response = requests.put(self.base_url + path, headers=headers, data=json.dumps(body), timeout=self.timeout)
-        if response.status_code >= 300:
-            error_code = response.json().get("code")
-            raise FireblocksApiException("Got an error from fireblocks server: " + response.text, error_code)
-        else:
-            return response.json()
+        return handle_response(response)
```

### Comparing `fireblocks_sdk-1.9.0/fireblocks_sdk/sdk_token_provider.py` & `fireblocks_sdk-1.9.1/fireblocks_sdk/sdk_token_provider.py`

 * *Files identical despite different names*

### Comparing `fireblocks_sdk-1.9.0/fireblocks_sdk.egg-info/PKG-INFO` & `fireblocks_sdk-1.9.1/fireblocks_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: fireblocks-sdk
-Version: 1.9.0
+Version: 1.9.1
 Summary: Fireblocks python SDK
 Home-page: https://github.com/fireblocks/fireblocks-sdk-py
 License: MIT
-Download-URL: https://github.com/fireblocks/fireblocks-sdk-py/archive/v1.9.0.tar.gz
+Download-URL: https://github.com/fireblocks/fireblocks-sdk-py/archive/v1.9.1.tar.gz
 Keywords: Fireblocks,SDK
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `fireblocks_sdk-1.9.0/setup.py` & `fireblocks_sdk-1.9.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from distutils.core import setup
 setup(
   name = 'fireblocks_sdk',
   packages = ['fireblocks_sdk'],
-  version = '1.9.0',
+  version = '1.9.1',
   license='MIT',
   description = 'Fireblocks python SDK',
   url = 'https://github.com/fireblocks/fireblocks-sdk-py',
-  download_url = 'https://github.com/fireblocks/fireblocks-sdk-py/archive/v1.9.0.tar.gz',
+  download_url = 'https://github.com/fireblocks/fireblocks-sdk-py/archive/v1.9.1.tar.gz',
   keywords = ['Fireblocks', 'SDK'],
   install_requires=[
           'PyJWT>=2.3.0',
           'cryptography>=2.7',
           'requests>=2.22.0',
       ],
   classifiers=[
```

