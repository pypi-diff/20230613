# Comparing `tmp/lodestone-python-sdk-1.0.3.tar.gz` & `tmp/lodestone-python-sdk-1.0.3.post999.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lodestone-python-sdk-1.0.3.tar", last modified: Tue Jun 13 08:04:26 2023, max compression
+gzip compressed data, was "lodestone-python-sdk-1.0.3.post999.tar", last modified: Tue Jun 13 09:34:25 2023, max compression
```

## Comparing `lodestone-python-sdk-1.0.3.tar` & `lodestone-python-sdk-1.0.3.post999.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 bocai      (501) staff       (20)        0 2023-06-13 08:04:26.893163 lodestone-python-sdk-1.0.3/
--rw-r--r--   0 bocai      (501) staff       (20)      524 2023-06-13 08:04:26.893042 lodestone-python-sdk-1.0.3/PKG-INFO
--rw-r--r--   0 bocai      (501) staff       (20)      254 2023-06-13 08:03:14.000000 lodestone-python-sdk-1.0.3/README.md
-drwxr-xr-x   0 bocai      (501) staff       (20)        0 2023-06-13 08:04:26.892305 lodestone-python-sdk-1.0.3/lodestone_python_sdk/
--rw-r--r--   0 bocai      (501) staff       (20)        0 2023-06-13 06:22:56.000000 lodestone-python-sdk-1.0.3/lodestone_python_sdk/__init__.py
--rw-r--r--   0 bocai      (501) staff       (20)      735 2023-06-13 07:47:08.000000 lodestone-python-sdk-1.0.3/lodestone_python_sdk/client.py
--rw-r--r--   0 bocai      (501) staff       (20)       42 2023-06-13 03:03:25.000000 lodestone-python-sdk-1.0.3/lodestone_python_sdk/exceptions.py
-drwxr-xr-x   0 bocai      (501) staff       (20)        0 2023-06-13 08:04:26.892873 lodestone-python-sdk-1.0.3/lodestone_python_sdk.egg-info/
--rw-r--r--   0 bocai      (501) staff       (20)      524 2023-06-13 08:04:26.000000 lodestone-python-sdk-1.0.3/lodestone_python_sdk.egg-info/PKG-INFO
--rw-r--r--   0 bocai      (501) staff       (20)      293 2023-06-13 08:04:26.000000 lodestone-python-sdk-1.0.3/lodestone_python_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 bocai      (501) staff       (20)        1 2023-06-13 08:04:26.000000 lodestone-python-sdk-1.0.3/lodestone_python_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 bocai      (501) staff       (20)       21 2023-06-13 08:04:26.000000 lodestone-python-sdk-1.0.3/lodestone_python_sdk.egg-info/top_level.txt
--rw-r--r--   0 bocai      (501) staff       (20)       38 2023-06-13 08:04:26.893212 lodestone-python-sdk-1.0.3/setup.cfg
--rw-r--r--   0 bocai      (501) staff       (20)      477 2023-06-13 08:04:23.000000 lodestone-python-sdk-1.0.3/setup.py
+drwxr-xr-x   0 bocai      (501) staff       (20)        0 2023-06-13 09:34:25.820268 lodestone-python-sdk-1.0.3.post999/
+-rw-r--r--   0 bocai      (501) staff       (20)      526 2023-06-13 09:34:25.820150 lodestone-python-sdk-1.0.3.post999/PKG-INFO
+-rw-r--r--   0 bocai      (501) staff       (20)      248 2023-06-13 08:22:58.000000 lodestone-python-sdk-1.0.3.post999/README.md
+drwxr-xr-x   0 bocai      (501) staff       (20)        0 2023-06-13 09:34:25.819200 lodestone-python-sdk-1.0.3.post999/lodestone_python_sdk/
+-rw-r--r--   0 bocai      (501) staff       (20)        0 2023-06-13 06:22:56.000000 lodestone-python-sdk-1.0.3.post999/lodestone_python_sdk/__init__.py
+-rw-r--r--   0 bocai      (501) staff       (20)      697 2023-06-13 09:13:28.000000 lodestone-python-sdk-1.0.3.post999/lodestone_python_sdk/client.py
+-rw-r--r--   0 bocai      (501) staff       (20)       42 2023-06-13 03:03:25.000000 lodestone-python-sdk-1.0.3.post999/lodestone_python_sdk/exceptions.py
+drwxr-xr-x   0 bocai      (501) staff       (20)        0 2023-06-13 09:34:25.819967 lodestone-python-sdk-1.0.3.post999/lodestone_python_sdk.egg-info/
+-rw-r--r--   0 bocai      (501) staff       (20)      526 2023-06-13 09:34:25.000000 lodestone-python-sdk-1.0.3.post999/lodestone_python_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 bocai      (501) staff       (20)      336 2023-06-13 09:34:25.000000 lodestone-python-sdk-1.0.3.post999/lodestone_python_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 bocai      (501) staff       (20)        1 2023-06-13 09:34:25.000000 lodestone-python-sdk-1.0.3.post999/lodestone_python_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 bocai      (501) staff       (20)       21 2023-06-13 09:34:25.000000 lodestone-python-sdk-1.0.3.post999/lodestone_python_sdk.egg-info/requires.txt
+-rw-r--r--   0 bocai      (501) staff       (20)       21 2023-06-13 09:34:25.000000 lodestone-python-sdk-1.0.3.post999/lodestone_python_sdk.egg-info/top_level.txt
+-rw-r--r--   0 bocai      (501) staff       (20)       38 2023-06-13 09:34:25.820313 lodestone-python-sdk-1.0.3.post999/setup.cfg
+-rw-r--r--   0 bocai      (501) staff       (20)      506 2023-06-13 09:34:20.000000 lodestone-python-sdk-1.0.3.post999/setup.py
```

### Comparing `lodestone-python-sdk-1.0.3/PKG-INFO` & `lodestone-python-sdk-1.0.3.post999/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lodestone-python-sdk
-Version: 1.0.3
+Version: 1.0.3.post999
 Summary: Auth to tuyoo's Lodestone
 Home-page: UNKNOWN
 Author: bocai
 Author-email: peijianbo@tuyoogame.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >3.2
@@ -16,15 +16,15 @@
 
 ```
 pip install lodestone-python-sdk
 ```
 
 ### Usages
 
-```python
+```
 client = AuthClient(auth_host, your_app_key, your_app_secret)
 token = client.get_token()
 ```
 
 ### Tips
 
 ```
```

### Comparing `lodestone-python-sdk-1.0.3/lodestone_python_sdk/client.py` & `lodestone-python-sdk-1.0.3.post999/lodestone_python_sdk/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 
 
 class AuthClient:
     def __init__(self, auth_host, app_key, app_secret, auth_path='account/api/v1/access-token'):
         self.auth_url = urljoin(auth_host, auth_path)
         self.app_key = app_key
         self.app_secret = app_secret
-        self.token = self.get_token()
 
     def get_token(self):
         response = request(
             method='post',
             url=self.auth_url,
             data={'app_key': self.app_key, 'app_secret': self.app_secret}
         )
```

### Comparing `lodestone-python-sdk-1.0.3/lodestone_python_sdk.egg-info/PKG-INFO` & `lodestone-python-sdk-1.0.3.post999/lodestone_python_sdk.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lodestone-python-sdk
-Version: 1.0.3
+Version: 1.0.3.post999
 Summary: Auth to tuyoo's Lodestone
 Home-page: UNKNOWN
 Author: bocai
 Author-email: peijianbo@tuyoogame.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >3.2
@@ -16,15 +16,15 @@
 
 ```
 pip install lodestone-python-sdk
 ```
 
 ### Usages
 
-```python
+```
 client = AuthClient(auth_host, your_app_key, your_app_secret)
 token = client.get_token()
 ```
 
 ### Tips
 
 ```
```

