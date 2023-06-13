# Comparing `tmp/openworld-sdk-python-fraudprevention-0.8.0.tar.gz` & `tmp/openworld-sdk-python-fraudprevention-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openworld-sdk-python-fraudprevention-0.8.0.tar", last modified: Tue May 30 14:40:27 2023, max compression
+gzip compressed data, was "openworld-sdk-python-fraudprevention-0.8.1.tar", last modified: Tue Jun 13 16:45:31 2023, max compression
```

## Comparing `openworld-sdk-python-fraudprevention-0.8.0.tar` & `openworld-sdk-python-fraudprevention-0.8.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:40:27.644522 openworld-sdk-python-fraudprevention-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-05-30 14:40:27.644522 openworld-sdk-python-fraudprevention-0.8.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:40:27.644522 openworld-sdk-python-fraudprevention-0.8.0/openworld/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:40:27.644522 openworld-sdk-python-fraudprevention-0.8.0/openworld/sdk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:40:27.644522 openworld-sdk-python-fraudprevention-0.8.0/openworld/sdk/fraudprevention/
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-30 14:40:21.000000 openworld-sdk-python-fraudprevention-0.8.0/openworld/sdk/fraudprevention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-05-30 14:40:21.000000 openworld-sdk-python-fraudprevention-0.8.0/openworld/sdk/fraudprevention/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    68115 2023-05-30 14:40:21.000000 openworld-sdk-python-fraudprevention-0.8.0/openworld/sdk/fraudprevention/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:40:27.644522 openworld-sdk-python-fraudprevention-0.8.0/openworld_sdk_python_fraudprevention.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-05-30 14:40:27.000000 openworld-sdk-python-fraudprevention-0.8.0/openworld_sdk_python_fraudprevention.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-30 14:40:27.000000 openworld-sdk-python-fraudprevention-0.8.0/openworld_sdk_python_fraudprevention.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 14:40:27.000000 openworld-sdk-python-fraudprevention-0.8.0/openworld_sdk_python_fraudprevention.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-30 14:40:27.000000 openworld-sdk-python-fraudprevention-0.8.0/openworld_sdk_python_fraudprevention.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-30 14:40:27.000000 openworld-sdk-python-fraudprevention-0.8.0/openworld_sdk_python_fraudprevention.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 14:40:27.644522 openworld-sdk-python-fraudprevention-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-05-30 14:40:05.000000 openworld-sdk-python-fraudprevention-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:45:31.418360 openworld-sdk-python-fraudprevention-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-06-13 16:45:31.418360 openworld-sdk-python-fraudprevention-0.8.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:45:31.418360 openworld-sdk-python-fraudprevention-0.8.1/openworld/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:45:31.418360 openworld-sdk-python-fraudprevention-0.8.1/openworld/sdk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:45:31.418360 openworld-sdk-python-fraudprevention-0.8.1/openworld/sdk/fraudprevention/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-13 16:45:24.000000 openworld-sdk-python-fraudprevention-0.8.1/openworld/sdk/fraudprevention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-06-13 16:45:24.000000 openworld-sdk-python-fraudprevention-0.8.1/openworld/sdk/fraudprevention/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68115 2023-06-13 16:45:24.000000 openworld-sdk-python-fraudprevention-0.8.1/openworld/sdk/fraudprevention/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:45:31.418360 openworld-sdk-python-fraudprevention-0.8.1/openworld_sdk_python_fraudprevention.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-06-13 16:45:31.000000 openworld-sdk-python-fraudprevention-0.8.1/openworld_sdk_python_fraudprevention.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-13 16:45:31.000000 openworld-sdk-python-fraudprevention-0.8.1/openworld_sdk_python_fraudprevention.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 16:45:31.000000 openworld-sdk-python-fraudprevention-0.8.1/openworld_sdk_python_fraudprevention.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-13 16:45:31.000000 openworld-sdk-python-fraudprevention-0.8.1/openworld_sdk_python_fraudprevention.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-13 16:45:31.000000 openworld-sdk-python-fraudprevention-0.8.1/openworld_sdk_python_fraudprevention.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 16:45:31.418360 openworld-sdk-python-fraudprevention-0.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-06-13 16:45:16.000000 openworld-sdk-python-fraudprevention-0.8.1/setup.py
```

### Comparing `openworld-sdk-python-fraudprevention-0.8.0/PKG-INFO` & `openworld-sdk-python-fraudprevention-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openworld-sdk-python-fraudprevention
-Version: 0.8.0
+Version: 0.8.1
 Summary: Open World Fraud Prevention SDK for Python
 Home-page: https://github.com/ExpediaGroup/openworld-sdk-python
 Author: Expedia Group
 Author-email: oss@expediagroup.com
 License: Apache License, Version 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
```

### Comparing `openworld-sdk-python-fraudprevention-0.8.0/openworld/sdk/fraudprevention/__init__.py` & `openworld-sdk-python-fraudprevention-0.8.1/openworld/sdk/fraudprevention/__init__.py`

 * *Files identical despite different names*

### Comparing `openworld-sdk-python-fraudprevention-0.8.0/openworld/sdk/fraudprevention/client.py` & `openworld-sdk-python-fraudprevention-0.8.1/openworld/sdk/fraudprevention/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         r"""Fraud Prevention API Client.
 
         Args:
             client_config(ClientConfig): SDK Client Configurations Holder.
         """
         python_version = platform.python_version()
         os_name, os_version, *_ = platform.platform().split('-')
-        sdk_metadata = f'open-world-sdk-python-fraudprevention/0.8.0'
+        sdk_metadata = f'open-world-sdk-python-fraudprevention/0.8.1'
 
         self.__api_client = ApiClient(client_config, _OpenWorldAuthClient)
 
         self.__user_agent = f'{sdk_metadata} (Python {python_version}; {os_name} {os_version})'
 
     def screen(self, transaction_id: UUID = uuid4(), body: OrderPurchaseScreenRequest = None) -> Union[OrderPurchaseScreenResponse, ExtendedError, Error]:
         r"""The Order Purchase API gives a Fraud recommendation for a transaction. A recommendation can be Accept, Reject, or Review. A transaction is marked as Review whenever there are insufficient signals to recommend Accept or Reject. These incidents are manually reviewed, and a corrected recommendation is made asynchronously.
```

### Comparing `openworld-sdk-python-fraudprevention-0.8.0/openworld/sdk/fraudprevention/model.py` & `openworld-sdk-python-fraudprevention-0.8.1/openworld/sdk/fraudprevention/model.py`

 * *Files identical despite different names*

### Comparing `openworld-sdk-python-fraudprevention-0.8.0/openworld_sdk_python_fraudprevention.egg-info/PKG-INFO` & `openworld-sdk-python-fraudprevention-0.8.1/openworld_sdk_python_fraudprevention.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openworld-sdk-python-fraudprevention
-Version: 0.8.0
+Version: 0.8.1
 Summary: Open World Fraud Prevention SDK for Python
 Home-page: https://github.com/ExpediaGroup/openworld-sdk-python
 Author: Expedia Group
 Author-email: oss@expediagroup.com
 License: Apache License, Version 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
```

### Comparing `openworld-sdk-python-fraudprevention-0.8.0/setup.py` & `openworld-sdk-python-fraudprevention-0.8.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 
 
 from setuptools import setup
 
 setup(
     name='openworld-sdk-python-fraudprevention',
-    version='0.8.0',
+    version='0.8.1',
     packages=['openworld.sdk.fraudprevention'],
     package_dir={'openworld-sdk-python-fraudprevention': '.'},
     license='Apache License, Version 2.0',
     author='Expedia Group',
     author_email='oss@expediagroup.com',
     url='https://github.com/ExpediaGroup/openworld-sdk-python',
     classifiers=[
```

