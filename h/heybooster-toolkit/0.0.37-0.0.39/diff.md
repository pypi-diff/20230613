# Comparing `tmp/heybooster-toolkit-0.0.37.tar.gz` & `tmp/heybooster-toolkit-0.0.39.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heybooster-toolkit-0.0.37.tar", last modified: Wed Jan 11 10:58:44 2023, max compression
+gzip compressed data, was "/Users/abdullahkulcu/Desktop/heybooster/heybooster-toolkit/dist/.tmp-sebpjsf5/heybooster-toolkit-0.0.39.tar", last modified: Tue Jun 13 09:22:36 2023, max compression
```

## Comparing `heybooster-toolkit-0.0.37.tar` & `heybooster-toolkit-0.0.39.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 ilteriskeskin   (501) staff       (20)        0 2023-01-11 10:58:44.068441 heybooster-toolkit-0.0.37/
--rw-r--r--   0 ilteriskeskin   (501) staff       (20)     1067 2023-01-11 10:49:58.000000 heybooster-toolkit-0.0.37/LICENSE
--rw-r--r--   0 ilteriskeskin   (501) staff       (20)       83 2023-01-11 10:49:58.000000 heybooster-toolkit-0.0.37/MANIFEST.in
--rw-r--r--   0 ilteriskeskin   (501) staff       (20)     1482 2023-01-11 10:58:44.068305 heybooster-toolkit-0.0.37/PKG-INFO
--rw-r--r--   0 ilteriskeskin   (501) staff       (20)      964 2023-01-11 10:49:58.000000 heybooster-toolkit-0.0.37/README.md
-drwxr-xr-x   0 ilteriskeskin   (501) staff       (20)        0 2023-01-11 10:58:44.065718 heybooster-toolkit-0.0.37/heybooster/
--rw-r--r--   0 ilteriskeskin   (501) staff       (20)        0 2023-01-11 10:49:58.000000 heybooster-toolkit-0.0.37/heybooster/__init__.py
-drwxr-xr-x   0 ilteriskeskin   (501) staff       (20)        0 2023-01-11 10:58:44.065929 heybooster-toolkit-0.0.37/heybooster/exception/
--rw-r--r--   0 ilteriskeskin   (501) staff       (20)        0 2023-01-11 10:49:58.000000 heybooster-toolkit-0.0.37/heybooster/exception/__init__.py
--rw-r--r--   0 ilteriskeskin   (501) staff       (20)     2594 2023-01-11 10:49:58.000000 heybooster-toolkit-0.0.37/heybooster/exception/exception_catcher.py
-drwxr-xr-x   0 ilteriskeskin   (501) staff       (20)        0 2023-01-11 10:58:44.066100 heybooster-toolkit-0.0.37/heybooster/helpers/
--rw-r--r--   0 ilteriskeskin   (501) staff       (20)        0 2023-01-11 10:49:58.000000 heybooster-toolkit-0.0.37/heybooster/helpers/__init__.py
-drwxr-xr-x   0 ilteriskeskin   (501) staff       (20)        0 2023-01-11 10:58:44.066775 heybooster-toolkit-0.0.37/heybooster/helpers/database/
--rw-r--r--   0 ilteriskeskin   (501) staff       (20)        0 2023-01-11 10:49:58.000000 heybooster-toolkit-0.0.37/heybooster/helpers/database/__init__.py
--rw-r--r--   0 ilteriskeskin   (501) staff       (20)     5794 2023-01-11 10:49:58.000000 heybooster-toolkit-0.0.37/heybooster/helpers/database/mongodb.py
--rw-r--r--   0 ilteriskeskin   (501) staff       (20)     3317 2023-01-11 10:54:01.000000 heybooster-toolkit-0.0.37/heybooster/helpers/database/opensearch.py
--rw-r--r--   0 ilteriskeskin   (501) staff       (20)     3285 2023-01-11 10:49:58.000000 heybooster-toolkit-0.0.37/heybooster/helpers/database/postgre.py
-drwxr-xr-x   0 ilteriskeskin   (501) staff       (20)        0 2023-01-11 10:58:44.067024 heybooster-toolkit-0.0.37/heybooster/helpers/email/
--rw-r--r--   0 ilteriskeskin   (501) staff       (20)        0 2023-01-11 10:49:58.000000 heybooster-toolkit-0.0.37/heybooster/helpers/email/__init__.py
--rw-r--r--   0 ilteriskeskin   (501) staff       (20)     4835 2023-01-11 10:49:58.000000 heybooster-toolkit-0.0.37/heybooster/helpers/email/sendpulse.py
-drwxr-xr-x   0 ilteriskeskin   (501) staff       (20)        0 2023-01-11 10:58:44.067170 heybooster-toolkit-0.0.37/heybooster/helpers/email/statics/
--rw-r--r--   0 ilteriskeskin   (501) staff       (20)      109 2023-01-11 10:49:58.000000 heybooster-toolkit-0.0.37/heybooster/helpers/email/statics/__init__.py
-drwxr-xr-x   0 ilteriskeskin   (501) staff       (20)        0 2023-01-11 10:58:44.067307 heybooster-toolkit-0.0.37/heybooster/helpers/email/utils/
--rw-r--r--   0 ilteriskeskin   (501) staff       (20)      360 2023-01-11 10:49:58.000000 heybooster-toolkit-0.0.37/heybooster/helpers/email/utils/__init__.py
-drwxr-xr-x   0 ilteriskeskin   (501) staff       (20)        0 2023-01-11 10:58:44.067539 heybooster-toolkit-0.0.37/heybooster/helpers/hubspot/
--rw-r--r--   0 ilteriskeskin   (501) staff       (20)        0 2023-01-11 10:49:58.000000 heybooster-toolkit-0.0.37/heybooster/helpers/hubspot/__init__.py
--rw-r--r--   0 ilteriskeskin   (501) staff       (20)     4267 2023-01-11 10:49:58.000000 heybooster-toolkit-0.0.37/heybooster/helpers/hubspot/contacts.py
-drwxr-xr-x   0 ilteriskeskin   (501) staff       (20)        0 2023-01-11 10:58:44.068135 heybooster-toolkit-0.0.37/heybooster_toolkit.egg-info/
--rw-r--r--   0 ilteriskeskin   (501) staff       (20)     1482 2023-01-11 10:58:44.000000 heybooster-toolkit-0.0.37/heybooster_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 ilteriskeskin   (501) staff       (20)      822 2023-01-11 10:58:44.000000 heybooster-toolkit-0.0.37/heybooster_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 ilteriskeskin   (501) staff       (20)        1 2023-01-11 10:58:44.000000 heybooster-toolkit-0.0.37/heybooster_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 ilteriskeskin   (501) staff       (20)       39 2023-01-11 10:58:44.000000 heybooster-toolkit-0.0.37/heybooster_toolkit.egg-info/requires.txt
--rw-r--r--   0 ilteriskeskin   (501) staff       (20)       11 2023-01-11 10:58:44.000000 heybooster-toolkit-0.0.37/heybooster_toolkit.egg-info/top_level.txt
--rw-r--r--   0 ilteriskeskin   (501) staff       (20)      103 2023-01-11 10:49:58.000000 heybooster-toolkit-0.0.37/pyproject.toml
--rw-r--r--   0 ilteriskeskin   (501) staff       (20)       38 2023-01-11 10:58:44.068480 heybooster-toolkit-0.0.37/setup.cfg
--rw-r--r--   0 ilteriskeskin   (501) staff       (20)      960 2023-01-11 10:49:58.000000 heybooster-toolkit-0.0.37/setup.py
--rw-r--r--   0 ilteriskeskin   (501) staff       (20)        6 2023-01-11 10:58:36.000000 heybooster-toolkit-0.0.37/version.txt
--rw-r--r--   0 ilteriskeskin   (501) staff       (20)      341 2023-01-11 10:49:58.000000 heybooster-toolkit-0.0.37/version_update.py
+drwxr-xr-x   0 abdullahkulcu   (501) staff       (20)        0 2023-06-13 09:22:36.000000 heybooster-toolkit-0.0.39/
+-rw-r--r--   0 abdullahkulcu   (501) staff       (20)     1067 2023-06-13 09:16:14.000000 heybooster-toolkit-0.0.39/LICENSE
+-rw-r--r--   0 abdullahkulcu   (501) staff       (20)       83 2023-06-13 09:16:14.000000 heybooster-toolkit-0.0.39/MANIFEST.in
+-rw-r--r--   0 abdullahkulcu   (501) staff       (20)     1482 2023-06-13 09:22:36.000000 heybooster-toolkit-0.0.39/PKG-INFO
+-rw-r--r--   0 abdullahkulcu   (501) staff       (20)      964 2023-06-13 09:16:14.000000 heybooster-toolkit-0.0.39/README.md
+drwxr-xr-x   0 abdullahkulcu   (501) staff       (20)        0 2023-06-13 09:22:36.000000 heybooster-toolkit-0.0.39/heybooster/
+-rw-r--r--   0 abdullahkulcu   (501) staff       (20)        0 2023-06-13 09:16:14.000000 heybooster-toolkit-0.0.39/heybooster/__init__.py
+drwxr-xr-x   0 abdullahkulcu   (501) staff       (20)        0 2023-06-13 09:22:36.000000 heybooster-toolkit-0.0.39/heybooster/exception/
+-rw-r--r--   0 abdullahkulcu   (501) staff       (20)        0 2023-06-13 09:16:14.000000 heybooster-toolkit-0.0.39/heybooster/exception/__init__.py
+-rw-r--r--   0 abdullahkulcu   (501) staff       (20)     2594 2023-06-13 09:16:14.000000 heybooster-toolkit-0.0.39/heybooster/exception/exception_catcher.py
+drwxr-xr-x   0 abdullahkulcu   (501) staff       (20)        0 2023-06-13 09:22:36.000000 heybooster-toolkit-0.0.39/heybooster/helpers/
+-rw-r--r--   0 abdullahkulcu   (501) staff       (20)        0 2023-06-13 09:16:14.000000 heybooster-toolkit-0.0.39/heybooster/helpers/__init__.py
+drwxr-xr-x   0 abdullahkulcu   (501) staff       (20)        0 2023-06-13 09:22:36.000000 heybooster-toolkit-0.0.39/heybooster/helpers/database/
+-rw-r--r--   0 abdullahkulcu   (501) staff       (20)        0 2023-06-13 09:16:14.000000 heybooster-toolkit-0.0.39/heybooster/helpers/database/__init__.py
+-rw-r--r--   0 abdullahkulcu   (501) staff       (20)     5794 2023-06-13 09:16:14.000000 heybooster-toolkit-0.0.39/heybooster/helpers/database/mongodb.py
+-rw-r--r--   0 abdullahkulcu   (501) staff       (20)     3677 2023-06-13 09:19:04.000000 heybooster-toolkit-0.0.39/heybooster/helpers/database/opensearch.py
+-rw-r--r--   0 abdullahkulcu   (501) staff       (20)     3285 2023-06-13 09:16:14.000000 heybooster-toolkit-0.0.39/heybooster/helpers/database/postgre.py
+drwxr-xr-x   0 abdullahkulcu   (501) staff       (20)        0 2023-06-13 09:22:36.000000 heybooster-toolkit-0.0.39/heybooster/helpers/email/
+-rw-r--r--   0 abdullahkulcu   (501) staff       (20)        0 2023-06-13 09:16:14.000000 heybooster-toolkit-0.0.39/heybooster/helpers/email/__init__.py
+-rw-r--r--   0 abdullahkulcu   (501) staff       (20)     4835 2023-06-13 09:21:34.000000 heybooster-toolkit-0.0.39/heybooster/helpers/email/sendpulse.py
+drwxr-xr-x   0 abdullahkulcu   (501) staff       (20)        0 2023-06-13 09:22:36.000000 heybooster-toolkit-0.0.39/heybooster/helpers/email/statics/
+-rw-r--r--   0 abdullahkulcu   (501) staff       (20)      109 2023-06-13 09:16:14.000000 heybooster-toolkit-0.0.39/heybooster/helpers/email/statics/__init__.py
+drwxr-xr-x   0 abdullahkulcu   (501) staff       (20)        0 2023-06-13 09:22:36.000000 heybooster-toolkit-0.0.39/heybooster/helpers/email/utils/
+-rw-r--r--   0 abdullahkulcu   (501) staff       (20)      360 2023-06-13 09:16:14.000000 heybooster-toolkit-0.0.39/heybooster/helpers/email/utils/__init__.py
+drwxr-xr-x   0 abdullahkulcu   (501) staff       (20)        0 2023-06-13 09:22:36.000000 heybooster-toolkit-0.0.39/heybooster/helpers/hubspot/
+-rw-r--r--   0 abdullahkulcu   (501) staff       (20)        0 2023-06-13 09:16:14.000000 heybooster-toolkit-0.0.39/heybooster/helpers/hubspot/__init__.py
+-rw-r--r--   0 abdullahkulcu   (501) staff       (20)     4267 2023-06-13 09:16:14.000000 heybooster-toolkit-0.0.39/heybooster/helpers/hubspot/contacts.py
+drwxr-xr-x   0 abdullahkulcu   (501) staff       (20)        0 2023-06-13 09:22:36.000000 heybooster-toolkit-0.0.39/heybooster_toolkit.egg-info/
+-rw-r--r--   0 abdullahkulcu   (501) staff       (20)     1482 2023-06-13 09:22:36.000000 heybooster-toolkit-0.0.39/heybooster_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 abdullahkulcu   (501) staff       (20)      822 2023-06-13 09:22:36.000000 heybooster-toolkit-0.0.39/heybooster_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 abdullahkulcu   (501) staff       (20)        1 2023-06-13 09:22:36.000000 heybooster-toolkit-0.0.39/heybooster_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 abdullahkulcu   (501) staff       (20)       39 2023-06-13 09:22:36.000000 heybooster-toolkit-0.0.39/heybooster_toolkit.egg-info/requires.txt
+-rw-r--r--   0 abdullahkulcu   (501) staff       (20)       11 2023-06-13 09:22:36.000000 heybooster-toolkit-0.0.39/heybooster_toolkit.egg-info/top_level.txt
+-rw-r--r--   0 abdullahkulcu   (501) staff       (20)      103 2023-06-13 09:16:14.000000 heybooster-toolkit-0.0.39/pyproject.toml
+-rw-r--r--   0 abdullahkulcu   (501) staff       (20)       38 2023-06-13 09:22:36.000000 heybooster-toolkit-0.0.39/setup.cfg
+-rw-r--r--   0 abdullahkulcu   (501) staff       (20)      960 2023-06-13 09:16:14.000000 heybooster-toolkit-0.0.39/setup.py
+-rw-r--r--   0 abdullahkulcu   (501) staff       (20)        6 2023-06-13 09:22:27.000000 heybooster-toolkit-0.0.39/version.txt
+-rw-r--r--   0 abdullahkulcu   (501) staff       (20)      341 2023-06-13 09:16:14.000000 heybooster-toolkit-0.0.39/version_update.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `heybooster-toolkit-0.0.37/LICENSE` & `heybooster-toolkit-0.0.39/LICENSE`

 * *Files identical despite different names*

### Comparing `heybooster-toolkit-0.0.37/PKG-INFO` & `heybooster-toolkit-0.0.39/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heybooster-toolkit
-Version: 0.0.37
+Version: 0.0.39
 Summary: Heybooster Toolkit
 Home-page: https://github.com/hey-booster/heybooster-toolkit
 Author: Heybooster
 Author-email: hey@heybooster.ai
 Project-URL: Bug Tracker, https://github.com/hey-booster/heybooster-toolkit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `heybooster-toolkit-0.0.37/README.md` & `heybooster-toolkit-0.0.39/README.md`

 * *Files identical despite different names*

### Comparing `heybooster-toolkit-0.0.37/heybooster/exception/exception_catcher.py` & `heybooster-toolkit-0.0.39/heybooster/exception/exception_catcher.py`

 * *Files identical despite different names*

### Comparing `heybooster-toolkit-0.0.37/heybooster/helpers/database/mongodb.py` & `heybooster-toolkit-0.0.39/heybooster/helpers/database/mongodb.py`

 * *Files identical despite different names*

### Comparing `heybooster-toolkit-0.0.37/heybooster/helpers/database/opensearch.py` & `heybooster-toolkit-0.0.39/heybooster/helpers/database/opensearch.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,8 @@
-import json
-import logging
 import requests
-
 from requests.auth import HTTPBasicAuth
 
 
 class OpenSearchHelper:
     """ OpenSearch (ElasticSearch) Helper """
     GET = "get"
     PUT = "put"
@@ -34,15 +31,15 @@
         response = requests.request(
             method=method,
             url=url,
             auth=self.auth,
             headers={
                 "Content-Type": "application/json"
             },
-            data=json.dumps(payload)
+            json=payload
         )
 
         if response.status_code != expected_status:
             raise Exception(f"Reponse Status Code -> {response.status_code} \n Message -> {response.text}")
 
         return response.json()
 
@@ -82,21 +79,39 @@
             raise Exception(exception)
 
     def search(self, size: int = 10, sort: str = "_id:desc", **kwargs):
         """
         This function returns search response
         """
         try:
-            params = [f"{key}:{value}" for key, value in kwargs.items()]
-            path = f"_search?q={','.join(params)}&size={size}&sort={sort}"
+            path = f"_search"
             url = self.get_url(path=path)
+            sort_key = sort.split(":")[0]
+            sort_order = sort.split(":")[1]
+
+            payload = {
+                "sort": [
+                    {
+                        sort_key: {
+                            "order": sort_order
+                        }
+                    }
+                ],
+                "size": size,
+                "query": {
+                    "match": {
+                        **kwargs
+                    }
+                }
+            }
 
             response = self.__perform_request(
                 method=OpenSearchHelper.GET,
                 url=url,
+                payload=payload,
             )
 
             return response
         except Exception as exception:
             raise Exception(exception)
 
     def get(self, payload: dict = {}):
```

### Comparing `heybooster-toolkit-0.0.37/heybooster/helpers/database/postgre.py` & `heybooster-toolkit-0.0.39/heybooster/helpers/database/postgre.py`

 * *Files identical despite different names*

### Comparing `heybooster-toolkit-0.0.37/heybooster/helpers/email/sendpulse.py` & `heybooster-toolkit-0.0.39/heybooster/helpers/email/sendpulse.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,45 +1,43 @@
 import requests
 from .utils import HTTPMethods, AuthenticationError, SendProcessFailureError
 from .statics import BASE_URL, ACCESS_URL_PATH, SMTP_URL_PATH
 
+
 class SendPulse:
     """ SendPulse SMTP API """
 
     def __init__(self, client_id: str, client_secret: str):
         """
             :client_id:     string, SendPulse client id
             :client_secret: string, SendPulse client secret key
         """
         self._client_id = client_id
         self._client_secret = client_secret
         self._access_token = self.__get_access_token()
 
-
-    def get_url(self, path: str=''):
+    def get_url(self, path: str = ''):
         """
             Concanates path and url
 
             :path: string
 
             return concanated url
         """
         return BASE_URL + path
 
-
-    def __get_header(self, use_access_token: bool=True):
+    def __get_header(self, use_access_token: bool = True):
         """
             Returns needed header
 
             return dict
         """
         return {'Authorization': 'Bearer ' + self._access_token} if use_access_token else {}
 
-
-    def __perform_request(self, path: str, http_method: HTTPMethods, params: dict={}, body: dict={}, use_access_token: bool=True) -> dict:
+    def __perform_request(self, path: str, http_method: HTTPMethods, params: dict = {}, body: dict = {}, use_access_token: bool = True) -> dict:
         """
             Sends request and refreshes access_token if necessary 
 
             :path:             string, added to end of the base url
             :http_method:      int, enum from HTTPMethods
             :params:           dict, request parameters
             :json:             dict, request body
@@ -53,22 +51,20 @@
         return request(
             url=self.get_url(path),
             headers=self.__get_header(use_access_token=use_access_token),
             params=params,
             json=body
         )
 
-    
     def refresh_token(self):
         """
             Gets new access token
         """
         self._access_token = self.__get_access_token()
 
-
     def __get_access_token(self) -> str:
         """
             Gets access token
 
             :path: string, added to end of the base url
 
             return str, access token
@@ -80,15 +76,14 @@
         })
 
         if response.status_code == 200:
             return response.json()['access_token']
         else:
             raise AuthenticationError
 
-
     def send_email_with_template(self, subject: str, template_id: str, variables: dict, from_name: str, from_email: str, to_data: list):
         """
             Sends email by using templates on Sendpulse
 
             :subject:     string, email subject
             :template_id: string, template_id on SenpPulse
             :variables:   dict, {<variable_name>: <value>}
@@ -110,15 +105,14 @@
                     'email': from_email
                 },
                 'to': to_data
             }}).json()
         except:
             raise SendProcessFailureError
 
-
     def send_email(self, subject: str, html: str, text: str, from_name: str, from_email: str, to_data: list):
         """
             Sends email by using templates on Sendpulse
 
             :subject:     string, email subject
             :html:        string, html of email encoded in Base64
             :text:        string, text of email
```

### Comparing `heybooster-toolkit-0.0.37/heybooster/helpers/hubspot/contacts.py` & `heybooster-toolkit-0.0.39/heybooster/helpers/hubspot/contacts.py`

 * *Files identical despite different names*

### Comparing `heybooster-toolkit-0.0.37/heybooster_toolkit.egg-info/PKG-INFO` & `heybooster-toolkit-0.0.39/heybooster_toolkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heybooster-toolkit
-Version: 0.0.37
+Version: 0.0.39
 Summary: Heybooster Toolkit
 Home-page: https://github.com/hey-booster/heybooster-toolkit
 Author: Heybooster
 Author-email: hey@heybooster.ai
 Project-URL: Bug Tracker, https://github.com/hey-booster/heybooster-toolkit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `heybooster-toolkit-0.0.37/heybooster_toolkit.egg-info/SOURCES.txt` & `heybooster-toolkit-0.0.39/heybooster_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `heybooster-toolkit-0.0.37/setup.py` & `heybooster-toolkit-0.0.39/setup.py`

 * *Files identical despite different names*

