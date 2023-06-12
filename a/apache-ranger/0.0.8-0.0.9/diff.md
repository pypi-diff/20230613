# Comparing `tmp/apache-ranger-0.0.8.tar.gz` & `tmp/apache-ranger-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-ranger-0.0.8.tar", last modified: Thu Dec  1 18:34:22 2022, max compression
+gzip compressed data, was "apache-ranger-0.0.9.tar", last modified: Sat Feb 11 07:14:09 2023, max compression
```

## Comparing `apache-ranger-0.0.8.tar` & `apache-ranger-0.0.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 madhan    (1000) madhan    (1000)        0 2022-12-01 18:34:22.000000 apache-ranger-0.0.8/
-drwxrwxr-x   0 madhan    (1000) madhan    (1000)        0 2022-12-01 18:34:22.000000 apache-ranger-0.0.8/apache_ranger/
-drwxrwxr-x   0 madhan    (1000) madhan    (1000)        0 2022-12-01 18:34:22.000000 apache-ranger-0.0.8/apache_ranger/client/
--rw-rw-r--   0 madhan    (1000) madhan    (1000)      802 2022-03-30 16:20:04.000000 apache-ranger-0.0.8/apache_ranger/client/__init__.py
--rw-rw-r--   0 madhan    (1000) madhan    (1000)    22794 2022-12-01 18:30:44.000000 apache-ranger-0.0.8/apache_ranger/client/ranger_client.py
--rw-rw-r--   0 madhan    (1000) madhan    (1000)     7459 2022-12-01 18:30:44.000000 apache-ranger-0.0.8/apache_ranger/client/ranger_kms_client.py
-drwxrwxr-x   0 madhan    (1000) madhan    (1000)        0 2022-12-01 18:34:22.000000 apache-ranger-0.0.8/apache_ranger/model/
--rw-rw-r--   0 madhan    (1000) madhan    (1000)      802 2022-03-30 16:20:04.000000 apache-ranger-0.0.8/apache_ranger/model/__init__.py
--rw-rw-r--   0 madhan    (1000) madhan    (1000)     1739 2022-03-30 16:20:04.000000 apache-ranger-0.0.8/apache_ranger/model/grant_revoke_role_request.py
--rw-rw-r--   0 madhan    (1000) madhan    (1000)     2250 2022-12-01 18:30:44.000000 apache-ranger-0.0.8/apache_ranger/model/ranger_base.py
--rw-rw-r--   0 madhan    (1000) madhan    (1000)     2708 2022-12-01 18:30:44.000000 apache-ranger-0.0.8/apache_ranger/model/ranger_kms.py
--rw-rw-r--   0 madhan    (1000) madhan    (1000)     7496 2022-07-26 17:16:29.000000 apache-ranger-0.0.8/apache_ranger/model/ranger_policy.py
--rw-rw-r--   0 madhan    (1000) madhan    (1000)     1723 2022-03-30 16:20:04.000000 apache-ranger-0.0.8/apache_ranger/model/ranger_role.py
--rw-rw-r--   0 madhan    (1000) madhan    (1000)     1738 2022-03-30 16:20:04.000000 apache-ranger-0.0.8/apache_ranger/model/ranger_security_zone.py
--rw-rw-r--   0 madhan    (1000) madhan    (1000)     1613 2022-03-30 16:20:04.000000 apache-ranger-0.0.8/apache_ranger/model/ranger_service.py
--rw-rw-r--   0 madhan    (1000) madhan    (1000)     9766 2022-03-30 16:20:04.000000 apache-ranger-0.0.8/apache_ranger/model/ranger_service_def.py
--rw-rw-r--   0 madhan    (1000) madhan    (1000)     1833 2022-07-11 05:18:01.000000 apache-ranger-0.0.8/apache_ranger/model/ranger_service_resource.py
--rw-rw-r--   0 madhan    (1000) madhan    (1000)     2395 2022-07-11 05:18:01.000000 apache-ranger-0.0.8/apache_ranger/model/ranger_service_tags.py
--rw-rw-r--   0 madhan    (1000) madhan    (1000)     1548 2022-07-11 05:18:01.000000 apache-ranger-0.0.8/apache_ranger/model/ranger_tag.py
--rw-rw-r--   0 madhan    (1000) madhan    (1000)     1567 2022-07-11 05:18:01.000000 apache-ranger-0.0.8/apache_ranger/model/ranger_tagdef.py
--rw-rw-r--   0 madhan    (1000) madhan    (1000)      802 2022-03-30 16:20:04.000000 apache-ranger-0.0.8/apache_ranger/__init__.py
--rw-rw-r--   0 madhan    (1000) madhan    (1000)     2102 2022-12-01 18:30:44.000000 apache-ranger-0.0.8/apache_ranger/exceptions.py
--rw-rw-r--   0 madhan    (1000) madhan    (1000)     3023 2022-12-01 18:30:44.000000 apache-ranger-0.0.8/apache_ranger/utils.py
-drwxrwxr-x   0 madhan    (1000) madhan    (1000)        0 2022-12-01 18:34:22.000000 apache-ranger-0.0.8/apache_ranger.egg-info/
--rw-rw-r--   0 madhan    (1000) madhan    (1000)     9667 2022-12-01 18:34:22.000000 apache-ranger-0.0.8/apache_ranger.egg-info/PKG-INFO
--rw-rw-r--   0 madhan    (1000) madhan    (1000)      943 2022-12-01 18:34:22.000000 apache-ranger-0.0.8/apache_ranger.egg-info/SOURCES.txt
--rw-rw-r--   0 madhan    (1000) madhan    (1000)        1 2022-12-01 18:34:22.000000 apache-ranger-0.0.8/apache_ranger.egg-info/dependency_links.txt
--rw-rw-r--   0 madhan    (1000) madhan    (1000)        1 2022-12-01 18:34:22.000000 apache-ranger-0.0.8/apache_ranger.egg-info/not-zip-safe
--rw-rw-r--   0 madhan    (1000) madhan    (1000)       15 2022-12-01 18:34:22.000000 apache-ranger-0.0.8/apache_ranger.egg-info/requires.txt
--rw-rw-r--   0 madhan    (1000) madhan    (1000)       14 2022-12-01 18:34:22.000000 apache-ranger-0.0.8/apache_ranger.egg-info/top_level.txt
--rw-rw-r--   0 madhan    (1000) madhan    (1000)    11349 2022-03-30 16:20:04.000000 apache-ranger-0.0.8/LICENSE
--rw-rw-r--   0 madhan    (1000) madhan    (1000)     7269 2022-12-01 18:30:44.000000 apache-ranger-0.0.8/README.md
--rw-rw-r--   0 madhan    (1000) madhan    (1000)     1744 2022-12-01 18:30:44.000000 apache-ranger-0.0.8/setup.py
--rw-rw-r--   0 madhan    (1000) madhan    (1000)     9667 2022-12-01 18:34:22.000000 apache-ranger-0.0.8/PKG-INFO
--rw-rw-r--   0 madhan    (1000) madhan    (1000)       38 2022-12-01 18:34:22.000000 apache-ranger-0.0.8/setup.cfg
+drwxr-xr-x   0 madhan     (501) staff       (20)        0 2023-02-11 07:14:09.004345 apache-ranger-0.0.9/
+-rw-r--r--   0 madhan     (501) staff       (20)    11349 2023-02-10 19:25:46.000000 apache-ranger-0.0.9/LICENSE
+-rw-r--r--   0 madhan     (501) staff       (20)     7830 2023-02-11 07:14:09.003383 apache-ranger-0.0.9/PKG-INFO
+-rw-r--r--   0 madhan     (501) staff       (20)     7269 2023-02-11 07:08:53.000000 apache-ranger-0.0.9/README.md
+drwxr-xr-x   0 madhan     (501) staff       (20)        0 2023-02-11 07:14:08.968736 apache-ranger-0.0.9/apache_ranger/
+-rw-r--r--   0 madhan     (501) staff       (20)      802 2023-02-10 19:25:46.000000 apache-ranger-0.0.9/apache_ranger/__init__.py
+drwxr-xr-x   0 madhan     (501) staff       (20)        0 2023-02-11 07:14:08.987737 apache-ranger-0.0.9/apache_ranger/client/
+-rw-r--r--   0 madhan     (501) staff       (20)      802 2023-02-10 19:25:46.000000 apache-ranger-0.0.9/apache_ranger/client/__init__.py
+-rw-r--r--   0 madhan     (501) staff       (20)    24303 2023-02-11 06:54:45.000000 apache-ranger-0.0.9/apache_ranger/client/ranger_client.py
+-rw-r--r--   0 madhan     (501) staff       (20)     7459 2023-02-10 19:25:46.000000 apache-ranger-0.0.9/apache_ranger/client/ranger_kms_client.py
+-rw-r--r--   0 madhan     (501) staff       (20)     2102 2023-02-10 19:25:46.000000 apache-ranger-0.0.9/apache_ranger/exceptions.py
+drwxr-xr-x   0 madhan     (501) staff       (20)        0 2023-02-11 07:14:09.001802 apache-ranger-0.0.9/apache_ranger/model/
+-rw-r--r--   0 madhan     (501) staff       (20)      802 2023-02-10 19:25:46.000000 apache-ranger-0.0.9/apache_ranger/model/__init__.py
+-rw-r--r--   0 madhan     (501) staff       (20)     1739 2023-02-10 19:25:46.000000 apache-ranger-0.0.9/apache_ranger/model/grant_revoke_role_request.py
+-rw-r--r--   0 madhan     (501) staff       (20)     2250 2023-02-10 19:25:46.000000 apache-ranger-0.0.9/apache_ranger/model/ranger_base.py
+-rw-r--r--   0 madhan     (501) staff       (20)     2708 2023-02-10 19:25:46.000000 apache-ranger-0.0.9/apache_ranger/model/ranger_kms.py
+-rw-r--r--   0 madhan     (501) staff       (20)     7496 2023-02-10 19:25:46.000000 apache-ranger-0.0.9/apache_ranger/model/ranger_policy.py
+-rw-r--r--   0 madhan     (501) staff       (20)     1723 2023-02-10 19:25:46.000000 apache-ranger-0.0.9/apache_ranger/model/ranger_role.py
+-rw-r--r--   0 madhan     (501) staff       (20)     1738 2023-02-10 19:25:46.000000 apache-ranger-0.0.9/apache_ranger/model/ranger_security_zone.py
+-rw-r--r--   0 madhan     (501) staff       (20)     1613 2023-02-10 19:25:46.000000 apache-ranger-0.0.9/apache_ranger/model/ranger_service.py
+-rw-r--r--   0 madhan     (501) staff       (20)     9766 2023-02-10 19:25:46.000000 apache-ranger-0.0.9/apache_ranger/model/ranger_service_def.py
+-rw-r--r--   0 madhan     (501) staff       (20)     1833 2023-02-10 19:25:46.000000 apache-ranger-0.0.9/apache_ranger/model/ranger_service_resource.py
+-rw-r--r--   0 madhan     (501) staff       (20)     2395 2023-02-10 19:25:46.000000 apache-ranger-0.0.9/apache_ranger/model/ranger_service_tags.py
+-rw-r--r--   0 madhan     (501) staff       (20)     1548 2023-02-10 19:25:46.000000 apache-ranger-0.0.9/apache_ranger/model/ranger_tag.py
+-rw-r--r--   0 madhan     (501) staff       (20)     1567 2023-02-10 19:25:46.000000 apache-ranger-0.0.9/apache_ranger/model/ranger_tagdef.py
+-rw-r--r--   0 madhan     (501) staff       (20)     3023 2023-02-10 19:25:46.000000 apache-ranger-0.0.9/apache_ranger/utils.py
+drwxr-xr-x   0 madhan     (501) staff       (20)        0 2023-02-11 07:14:08.983786 apache-ranger-0.0.9/apache_ranger.egg-info/
+-rw-r--r--   0 madhan     (501) staff       (20)     7830 2023-02-11 07:14:08.000000 apache-ranger-0.0.9/apache_ranger.egg-info/PKG-INFO
+-rw-r--r--   0 madhan     (501) staff       (20)      943 2023-02-11 07:14:08.000000 apache-ranger-0.0.9/apache_ranger.egg-info/SOURCES.txt
+-rw-r--r--   0 madhan     (501) staff       (20)        1 2023-02-11 07:14:08.000000 apache-ranger-0.0.9/apache_ranger.egg-info/dependency_links.txt
+-rw-r--r--   0 madhan     (501) staff       (20)        1 2023-02-11 07:07:58.000000 apache-ranger-0.0.9/apache_ranger.egg-info/not-zip-safe
+-rw-r--r--   0 madhan     (501) staff       (20)       15 2023-02-11 07:14:08.000000 apache-ranger-0.0.9/apache_ranger.egg-info/requires.txt
+-rw-r--r--   0 madhan     (501) staff       (20)       14 2023-02-11 07:14:08.000000 apache-ranger-0.0.9/apache_ranger.egg-info/top_level.txt
+-rw-r--r--   0 madhan     (501) staff       (20)       38 2023-02-11 07:14:09.004563 apache-ranger-0.0.9/setup.cfg
+-rw-r--r--   0 madhan     (501) staff       (20)     1744 2023-02-11 07:10:09.000000 apache-ranger-0.0.9/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `apache-ranger-0.0.8/apache_ranger/client/__init__.py` & `apache-ranger-0.0.9/apache_ranger/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-ranger-0.0.8/apache_ranger/client/ranger_client.py` & `apache-ranger-0.0.9/apache_ranger/client/ranger_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,17 +36,17 @@
 
 LOG = logging.getLogger(__name__)
 
 QUERY_PARAM_USER_DOT_NAME = 'user.name'.encode("utf-8")
 
 
 class RangerClient:
-    def __init__(self, url, auth):
-        self.client_http = RangerClientHttp(url, auth)
-
+    def __init__(self, url, auth, query_params=None, headers=None):
+        self.client_http = RangerClientHttp(url, auth, query_params, headers)
+        self.session     = self.client_http.session
         logging.getLogger("requests").setLevel(logging.WARNING)
 
 
     # Service Definition APIs
     def create_service_def(self, serviceDef):
         resp = self.client_http.call_api(RangerClient.CREATE_SERVICEDEF, request_data=serviceDef)
 
@@ -134,14 +134,19 @@
         return type_coerce(resp, RangerPolicy)
 
     def get_policy(self, serviceName, policyName):
         resp = self.client_http.call_api(RangerClient.GET_POLICY_BY_NAME.format_path({ 'serviceName': serviceName, 'policyName': policyName}))
 
         return type_coerce(resp, RangerPolicy)
 
+    def get_policy_by_name_zone(self, serviceName, policyName, zoneName):
+        resp = self.client_http.call_api(RangerClient.GET_POLICY_BY_NAME.format_path({ 'serviceName': serviceName, 'policyName': policyName}), { 'zoneName': zoneName })
+
+        return type_coerce(resp, RangerPolicy)
+
     def get_policies_in_service(self, serviceName, params=None):
         resp = self.client_http.call_api(RangerClient.GET_POLICIES_IN_SERVICE.format_path({ 'serviceName': serviceName }), params)
 
         return type_coerce_list(resp, RangerPolicy)
 
     def update_policy_by_id(self, policyId, policy):
         resp = self.client_http.call_api(RangerClient.UPDATE_POLICY_BY_ID.format_path({ 'id': policyId }), request_data=policy)
@@ -149,25 +154,33 @@
         return type_coerce(resp, RangerPolicy)
 
     def update_policy(self, serviceName, policyName, policy):
         resp = self.client_http.call_api(RangerClient.UPDATE_POLICY_BY_NAME.format_path({ 'serviceName': serviceName, 'policyName': policyName}), request_data=policy)
 
         return type_coerce(resp, RangerPolicy)
 
+    def update_policy_by_name_zone(self, serviceName, policyName, zoneName, policy):
+        resp = self.client_http.call_api(RangerClient.UPDATE_POLICY_BY_NAME.format_path({ 'serviceName': serviceName, 'policyName': policyName}), { 'zoneName': zoneName },  request_data=policy)
+
+        return type_coerce(resp, RangerPolicy)
+
     def apply_policy(self, policy, params=None):
         resp = self.client_http.call_api(RangerClient.APPLY_POLICY, params, policy)
 
         return type_coerce(resp, RangerPolicy)
 
     def delete_policy_by_id(self, policyId):
         self.client_http.call_api(RangerClient.DELETE_POLICY_BY_ID.format_path({ 'id': policyId }))
 
     def delete_policy(self, serviceName, policyName):
         self.client_http.call_api(RangerClient.DELETE_POLICY_BY_NAME, { 'servicename': serviceName, 'policyname': policyName })
 
+    def delete_policy_by_name_zone(self, serviceName, policyName, zoneName):
+        self.client_http.call_api(RangerClient.DELETE_POLICY_BY_NAME, { 'servicename': serviceName, 'policyname': policyName, 'zoneName': zoneName })
+
     def find_policies(self, filter=None):
         resp = self.client_http.call_api(RangerClient.FIND_POLICIES, filter)
 
         return type_coerce_list(resp, RangerPolicy)
 
 
     # SecurityZone APIs
@@ -416,24 +429,40 @@
     def type_coerce_attrs(self):
         super(RangerPolicy, self).type_coerce_attrs()
 
         self.messageList = type_coerce_dict(self.messageList, Message)
 
 
 class RangerClientHttp:
-    def __init__(self, url, auth):
-        self.url          = url.rstrip('/')
+    def __init__(self, url, auth, query_params=None, headers=None):
+        self.url          = url.rstrip('/') + '/' # ensure that self.url ends with a /
+        self.query_params = query_params
+        self.headers      = headers
         self.session      = Session()
         self.session.auth = auth
 
 
     def call_api(self, api, query_params=None, request_data=None):
         ret    = None
         params = { 'headers': { 'Accept': api.consumes, 'Content-type': api.produces } }
 
+        if self.headers:
+          params['headers'].update(self.headers)
+
+        if self.query_params:
+          if query_params:
+              merged_query_params = {}
+
+              merged_query_params.update(self.query_params)
+              merged_query_params.update(query_params)
+
+              query_params = merged_query_params
+          else:
+              query_params = self.query_params
+
         if query_params:
             params['params'] = query_params
 
         if request_data:
             params['data'] = json.dumps(request_data)
 
         path = urljoin(self.url, api.path.lstrip('/'))
```

### Comparing `apache-ranger-0.0.8/apache_ranger/client/ranger_kms_client.py` & `apache-ranger-0.0.9/apache_ranger/client/ranger_kms_client.py`

 * *Files identical despite different names*

### Comparing `apache-ranger-0.0.8/apache_ranger/model/__init__.py` & `apache-ranger-0.0.9/apache_ranger/client/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-ranger-0.0.8/apache_ranger/model/grant_revoke_role_request.py` & `apache-ranger-0.0.9/apache_ranger/model/grant_revoke_role_request.py`

 * *Files identical despite different names*

### Comparing `apache-ranger-0.0.8/apache_ranger/model/ranger_base.py` & `apache-ranger-0.0.9/apache_ranger/model/ranger_base.py`

 * *Files identical despite different names*

### Comparing `apache-ranger-0.0.8/apache_ranger/model/ranger_kms.py` & `apache-ranger-0.0.9/apache_ranger/model/ranger_kms.py`

 * *Files identical despite different names*

### Comparing `apache-ranger-0.0.8/apache_ranger/model/ranger_policy.py` & `apache-ranger-0.0.9/apache_ranger/model/ranger_policy.py`

 * *Files identical despite different names*

### Comparing `apache-ranger-0.0.8/apache_ranger/model/ranger_role.py` & `apache-ranger-0.0.9/apache_ranger/model/ranger_role.py`

 * *Files identical despite different names*

### Comparing `apache-ranger-0.0.8/apache_ranger/model/ranger_security_zone.py` & `apache-ranger-0.0.9/apache_ranger/model/ranger_security_zone.py`

 * *Files identical despite different names*

### Comparing `apache-ranger-0.0.8/apache_ranger/model/ranger_service.py` & `apache-ranger-0.0.9/apache_ranger/model/ranger_service.py`

 * *Files identical despite different names*

### Comparing `apache-ranger-0.0.8/apache_ranger/model/ranger_service_def.py` & `apache-ranger-0.0.9/apache_ranger/model/ranger_service_def.py`

 * *Files identical despite different names*

### Comparing `apache-ranger-0.0.8/apache_ranger/model/ranger_service_resource.py` & `apache-ranger-0.0.9/apache_ranger/model/ranger_service_resource.py`

 * *Files identical despite different names*

### Comparing `apache-ranger-0.0.8/apache_ranger/model/ranger_service_tags.py` & `apache-ranger-0.0.9/apache_ranger/model/ranger_service_tags.py`

 * *Files identical despite different names*

### Comparing `apache-ranger-0.0.8/apache_ranger/model/ranger_tag.py` & `apache-ranger-0.0.9/apache_ranger/model/ranger_tag.py`

 * *Files identical despite different names*

### Comparing `apache-ranger-0.0.8/apache_ranger/model/ranger_tagdef.py` & `apache-ranger-0.0.9/apache_ranger/model/ranger_tagdef.py`

 * *Files identical despite different names*

### Comparing `apache-ranger-0.0.8/apache_ranger/__init__.py` & `apache-ranger-0.0.9/apache_ranger/model/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-ranger-0.0.8/apache_ranger/exceptions.py` & `apache-ranger-0.0.9/apache_ranger/exceptions.py`

 * *Files identical despite different names*

### Comparing `apache-ranger-0.0.8/apache_ranger/utils.py` & `apache-ranger-0.0.9/apache_ranger/utils.py`

 * *Files identical despite different names*

### Comparing `apache-ranger-0.0.8/apache_ranger.egg-info/PKG-INFO` & `apache-ranger-0.0.9/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,247 +1,231 @@
-Metadata-Version: 2.1
-Name: apache-ranger
-Version: 0.0.8
-Summary: Apache Ranger Python client
-Home-page: https://github.com/apache/ranger/tree/master/intg/src/main/python
-Author: Apache Ranger
-Author-email: dev@ranger.apache.org
-License: Apache LICENSE 2.0
-Description: <!---
-        Licensed to the Apache Software Foundation (ASF) under one
-        or more contributor license agreements.  See the NOTICE file
-        distributed with this work for additional information
-        regarding copyright ownership.  The ASF licenses this file
-        to you under the Apache License, Version 2.0 (the
-        "License"); you may not use this file except in compliance
-        with the License.  You may obtain a copy of the License at
-        
-          http://www.apache.org/licenses/LICENSE-2.0
-        
-        Unless required by applicable law or agreed to in writing,
-        software distributed under the License is distributed on an
-        "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
-        KIND, either express or implied.  See the License for the
-        specific language governing permissions and limitations
-        under the License.
-        -->
-        
-        # Apache Ranger - Python client
-        
-        Python library for Apache Ranger.
-        
-        ## Installation
-        
-        Use the package manager [pip](https://pip.pypa.io/en/stable/) to install python client for Apache Ranger.
-        
-        ```bash
-        > pip install apache-ranger
-        ```
-        
-        Verify if apache-ranger client is installed:
-        ```bash
-        > pip list
-        
-        Package      Version
-        ------------ ---------
-        apache-ranger 0.0.8
-        ```
-        
-        ## Usage
-        
-        ```python test_ranger.py```
-        ```python
-        # test_ranger.py
-        
-        from apache_ranger.model.ranger_service import *
-        from apache_ranger.client.ranger_client import *
-        from apache_ranger.model.ranger_policy  import *
-        
-        
-        ## Step 1: create a client to connect to Apache Ranger admin
-        ranger_url  = 'http://localhost:6080'
-        ranger_auth = ('admin', 'rangerR0cks!')
-        
-        # For Kerberos authentication
-        #
-        # from requests_kerberos import HTTPKerberosAuth
-        #
-        # ranger_auth = HTTPKerberosAuth()
-        
-        ranger = RangerClient(ranger_url, ranger_auth)
-        
-        # to disable SSL certificate validation (not recommended for production use!)
-        #
-        # ranger.session.verify = False
-        
-        
-        ## Step 2: Let's create a service
-        service         = RangerService()
-        service.name    = 'test_hive'
-        service.type    = 'hive'
-        service.configs = {'username':'hive', 'password':'hive', 'jdbc.driverClassName': 'org.apache.hive.jdbc.HiveDriver', 'jdbc.url': 'jdbc:hive2://ranger-hadoop:10000', 'hadoop.security.authorization': 'true'}
-        
-        print('Creating service: name=' + service.name)
-        
-        created_service = ranger.create_service(service)
-        
-        print('    created service: name=' + created_service.name + ', id=' + str(created_service.id))
-        
-        
-        ## Step 3: Let's create a policy
-        policy           = RangerPolicy()
-        policy.service   = service.name
-        policy.name      = 'test policy'
-        policy.resources = { 'database': RangerPolicyResource({ 'values': ['test_db'] }),
-                             'table':    RangerPolicyResource({ 'values': ['test_tbl'] }),
-                             'column':   RangerPolicyResource({ 'values': ['*'] }) }
-        
-        allowItem1          = RangerPolicyItem()
-        allowItem1.users    = [ 'admin' ]
-        allowItem1.accesses = [ RangerPolicyItemAccess({ 'type': 'create' }),
-                                RangerPolicyItemAccess({ 'type': 'alter' }) ]
-        
-        denyItem1          = RangerPolicyItem()
-        denyItem1.users    = [ 'admin' ]
-        denyItem1.accesses = [ RangerPolicyItemAccess({ 'type': 'drop' }) ]
-        
-        policy.policyItems     = [ allowItem1 ]
-        policy.denyPolicyItems = [ denyItem1 ]
-        
-        print('Creating policy: name=' + policy.name)
-        
-        created_policy = ranger.create_policy(policy)
-        
-        print('    created policy: name=' + created_policy.name + ', id=' + str(created_policy.id))
-        
-        
-        ## Step 4: Delete policy and service created above
-        print('Deleting policy: id=' + str(created_policy.id))
-        
-        ranger.delete_policy_by_id(created_policy.id)
-        
-        print('    deleted policy: id=' + str(created_policy.id))
-        
-        print('Deleting service: id=' + str(created_service.id))
-        
-        ranger.delete_service_by_id(created_service.id)
-        
-        print('    deleted service: id=' + str(created_service.id))
-        
-        ```
-        
-        ```python test_ranger_kms.py```
-        ```python
-        # test_ranger_kms.py
-        from apache_ranger.client.ranger_kms_client import RangerKMSClient
-        from apache_ranger.client.ranger_client     import HadoopSimpleAuth
-        from apache_ranger.model.ranger_kms         import RangerKey
-        import time
-        
-        
-        ##
-        ## Step 1: create a client to connect to Apache Ranger KMS
-        ##
-        kms_url  = 'http://localhost:9292'
-        kms_auth = HadoopSimpleAuth('keyadmin')
-        
-        # For Kerberos authentication
-        #
-        # from requests_kerberos import HTTPKerberosAuth
-        #
-        # kms_auth = HTTPKerberosAuth()
-        #
-        # For HTTP Basic authentication
-        #
-        # kms_auth = ('keyadmin', 'rangerR0cks!')
-        
-        kms_client = RangerKMSClient(kms_url, kms_auth)
-        
-        
-        
-        ##
-        ## Step 2: Let's call KMS APIs
-        ##
-        
-        kms_status = kms_client.kms_status()
-        print('kms_status():', kms_status)
-        print()
-        
-        key_name = 'test_' + str(int(time.time() * 1000))
-        
-        key = kms_client.create_key(RangerKey({'name':key_name}))
-        print('create_key(' + key_name + '):', key)
-        print()
-        
-        rollover_key = kms_client.rollover_key(key_name, key.material)
-        print('rollover_key(' + key_name + '):', rollover_key)
-        print()
-        
-        kms_client.invalidate_cache_for_key(key_name)
-        print('invalidate_cache_for_key(' + key_name + ')')
-        print()
-        
-        key_metadata = kms_client.get_key_metadata(key_name)
-        print('get_key_metadata(' + key_name + '):', key_metadata)
-        print()
-        
-        current_key = kms_client.get_current_key(key_name)
-        print('get_current_key(' + key_name + '):', current_key)
-        print()
-        
-        encrypted_keys = kms_client.generate_encrypted_key(key_name, 6)
-        print('generate_encrypted_key(' + key_name + ', ' + str(6) + '):')
-        for i in range(len(encrypted_keys)):
-          encrypted_key   = encrypted_keys[i]
-          decrypted_key   = kms_client.decrypt_encrypted_key(key_name, encrypted_key.versionName, encrypted_key.iv, encrypted_key.encryptedKeyVersion.material)
-          reencrypted_key = kms_client.reencrypt_encrypted_key(key_name, encrypted_key.versionName, encrypted_key.iv, encrypted_key.encryptedKeyVersion.material)
-          print('  encrypted_keys[' + str(i) + ']: ', encrypted_key)
-          print('  decrypted_key[' + str(i) + ']:  ', decrypted_key)
-          print('  reencrypted_key[' + str(i) + ']:', reencrypted_key)
-        print()
-        
-        reencrypted_keys = kms_client.batch_reencrypt_encrypted_keys(key_name, encrypted_keys)
-        print('batch_reencrypt_encrypted_keys(' + key_name + ', ' + str(len(encrypted_keys)) + '):')
-        for i in range(len(reencrypted_keys)):
-          print('  batch_reencrypt_encrypted_key[' + str(i) + ']:', reencrypted_keys[i])
-        print()
-        
-        key_versions = kms_client.get_key_versions(key_name)
-        print('get_key_versions(' + key_name + '):', len(key_versions))
-        for i in range(len(key_versions)):
-          print('  key_versions[' + str(i) + ']:', key_versions[i])
-        print()
-        
-        for i in range(len(key_versions)):
-          key_version = kms_client.get_key_version(key_versions[i].versionName)
-          print('get_key_version(' + str(i) + '):', key_version)
-        print()
-        
-        key_names = kms_client.get_key_names()
-        print('get_key_names():', len(key_names))
-        for i in range(len(key_names)):
-          print('  key_name[' + str(i) + ']:', key_names[i])
-        print()
-        
-        keys_metadata = kms_client.get_keys_metadata(key_names)
-        print('get_keys_metadata(' + str(key_names) + '):', len(keys_metadata))
-        for i in range(len(keys_metadata)):
-          print('  key_metadata[' + str(i) + ']:', keys_metadata[i])
-        print()
-        
-        key = kms_client.get_key(key_name)
-        print('get_key(' + key_name + '):', key)
-        print()
-        
-        kms_client.delete_key(key_name)
-        print('delete_key(' + key_name + ')')
-        ```
-        
-        For more examples, checkout `sample-client` python  project in [ranger-examples](https://github.com/apache/ranger/blob/master/ranger-examples/sample-client/src/main/python/sample_client.py) module.
-        
-Keywords: ranger client,apache ranger
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 2.7
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=2.7
-Description-Content-Type: text/markdown
+<!---
+Licensed to the Apache Software Foundation (ASF) under one
+or more contributor license agreements.  See the NOTICE file
+distributed with this work for additional information
+regarding copyright ownership.  The ASF licenses this file
+to you under the Apache License, Version 2.0 (the
+"License"); you may not use this file except in compliance
+with the License.  You may obtain a copy of the License at
+
+  http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing,
+software distributed under the License is distributed on an
+"AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
+KIND, either express or implied.  See the License for the
+specific language governing permissions and limitations
+under the License.
+-->
+
+# Apache Ranger - Python client
+
+Python library for Apache Ranger.
+
+## Installation
+
+Use the package manager [pip](https://pip.pypa.io/en/stable/) to install python client for Apache Ranger.
+
+```bash
+> pip install apache-ranger
+```
+
+Verify if apache-ranger client is installed:
+```bash
+> pip list
+
+Package      Version
+------------ ---------
+apache-ranger 0.0.9
+```
+
+## Usage
+
+```python test_ranger.py```
+```python
+# test_ranger.py
+
+from apache_ranger.model.ranger_service import *
+from apache_ranger.client.ranger_client import *
+from apache_ranger.model.ranger_policy  import *
+
+
+## Step 1: create a client to connect to Apache Ranger admin
+ranger_url  = 'http://localhost:6080'
+ranger_auth = ('admin', 'rangerR0cks!')
+
+# For Kerberos authentication
+#
+# from requests_kerberos import HTTPKerberosAuth
+#
+# ranger_auth = HTTPKerberosAuth()
+
+ranger = RangerClient(ranger_url, ranger_auth)
+
+# to disable SSL certificate validation (not recommended for production use!)
+#
+# ranger.session.verify = False
+
+
+## Step 2: Let's create a service
+service         = RangerService()
+service.name    = 'test_hive'
+service.type    = 'hive'
+service.configs = {'username':'hive', 'password':'hive', 'jdbc.driverClassName': 'org.apache.hive.jdbc.HiveDriver', 'jdbc.url': 'jdbc:hive2://ranger-hadoop:10000', 'hadoop.security.authorization': 'true'}
+
+print('Creating service: name=' + service.name)
+
+created_service = ranger.create_service(service)
+
+print('    created service: name=' + created_service.name + ', id=' + str(created_service.id))
+
+
+## Step 3: Let's create a policy
+policy           = RangerPolicy()
+policy.service   = service.name
+policy.name      = 'test policy'
+policy.resources = { 'database': RangerPolicyResource({ 'values': ['test_db'] }),
+                     'table':    RangerPolicyResource({ 'values': ['test_tbl'] }),
+                     'column':   RangerPolicyResource({ 'values': ['*'] }) }
+
+allowItem1          = RangerPolicyItem()
+allowItem1.users    = [ 'admin' ]
+allowItem1.accesses = [ RangerPolicyItemAccess({ 'type': 'create' }),
+                        RangerPolicyItemAccess({ 'type': 'alter' }) ]
+
+denyItem1          = RangerPolicyItem()
+denyItem1.users    = [ 'admin' ]
+denyItem1.accesses = [ RangerPolicyItemAccess({ 'type': 'drop' }) ]
+
+policy.policyItems     = [ allowItem1 ]
+policy.denyPolicyItems = [ denyItem1 ]
+
+print('Creating policy: name=' + policy.name)
+
+created_policy = ranger.create_policy(policy)
+
+print('    created policy: name=' + created_policy.name + ', id=' + str(created_policy.id))
+
+
+## Step 4: Delete policy and service created above
+print('Deleting policy: id=' + str(created_policy.id))
+
+ranger.delete_policy_by_id(created_policy.id)
+
+print('    deleted policy: id=' + str(created_policy.id))
+
+print('Deleting service: id=' + str(created_service.id))
+
+ranger.delete_service_by_id(created_service.id)
+
+print('    deleted service: id=' + str(created_service.id))
+
+```
+
+```python test_ranger_kms.py```
+```python
+# test_ranger_kms.py
+from apache_ranger.client.ranger_kms_client import RangerKMSClient
+from apache_ranger.client.ranger_client     import HadoopSimpleAuth
+from apache_ranger.model.ranger_kms         import RangerKey
+import time
+
+
+##
+## Step 1: create a client to connect to Apache Ranger KMS
+##
+kms_url  = 'http://localhost:9292'
+kms_auth = HadoopSimpleAuth('keyadmin')
+
+# For Kerberos authentication
+#
+# from requests_kerberos import HTTPKerberosAuth
+#
+# kms_auth = HTTPKerberosAuth()
+#
+# For HTTP Basic authentication
+#
+# kms_auth = ('keyadmin', 'rangerR0cks!')
+
+kms_client = RangerKMSClient(kms_url, kms_auth)
+
+
+
+##
+## Step 2: Let's call KMS APIs
+##
+
+kms_status = kms_client.kms_status()
+print('kms_status():', kms_status)
+print()
+
+key_name = 'test_' + str(int(time.time() * 1000))
+
+key = kms_client.create_key(RangerKey({'name':key_name}))
+print('create_key(' + key_name + '):', key)
+print()
+
+rollover_key = kms_client.rollover_key(key_name, key.material)
+print('rollover_key(' + key_name + '):', rollover_key)
+print()
+
+kms_client.invalidate_cache_for_key(key_name)
+print('invalidate_cache_for_key(' + key_name + ')')
+print()
+
+key_metadata = kms_client.get_key_metadata(key_name)
+print('get_key_metadata(' + key_name + '):', key_metadata)
+print()
+
+current_key = kms_client.get_current_key(key_name)
+print('get_current_key(' + key_name + '):', current_key)
+print()
+
+encrypted_keys = kms_client.generate_encrypted_key(key_name, 6)
+print('generate_encrypted_key(' + key_name + ', ' + str(6) + '):')
+for i in range(len(encrypted_keys)):
+  encrypted_key   = encrypted_keys[i]
+  decrypted_key   = kms_client.decrypt_encrypted_key(key_name, encrypted_key.versionName, encrypted_key.iv, encrypted_key.encryptedKeyVersion.material)
+  reencrypted_key = kms_client.reencrypt_encrypted_key(key_name, encrypted_key.versionName, encrypted_key.iv, encrypted_key.encryptedKeyVersion.material)
+  print('  encrypted_keys[' + str(i) + ']: ', encrypted_key)
+  print('  decrypted_key[' + str(i) + ']:  ', decrypted_key)
+  print('  reencrypted_key[' + str(i) + ']:', reencrypted_key)
+print()
+
+reencrypted_keys = kms_client.batch_reencrypt_encrypted_keys(key_name, encrypted_keys)
+print('batch_reencrypt_encrypted_keys(' + key_name + ', ' + str(len(encrypted_keys)) + '):')
+for i in range(len(reencrypted_keys)):
+  print('  batch_reencrypt_encrypted_key[' + str(i) + ']:', reencrypted_keys[i])
+print()
+
+key_versions = kms_client.get_key_versions(key_name)
+print('get_key_versions(' + key_name + '):', len(key_versions))
+for i in range(len(key_versions)):
+  print('  key_versions[' + str(i) + ']:', key_versions[i])
+print()
+
+for i in range(len(key_versions)):
+  key_version = kms_client.get_key_version(key_versions[i].versionName)
+  print('get_key_version(' + str(i) + '):', key_version)
+print()
+
+key_names = kms_client.get_key_names()
+print('get_key_names():', len(key_names))
+for i in range(len(key_names)):
+  print('  key_name[' + str(i) + ']:', key_names[i])
+print()
+
+keys_metadata = kms_client.get_keys_metadata(key_names)
+print('get_keys_metadata(' + str(key_names) + '):', len(keys_metadata))
+for i in range(len(keys_metadata)):
+  print('  key_metadata[' + str(i) + ']:', keys_metadata[i])
+print()
+
+key = kms_client.get_key(key_name)
+print('get_key(' + key_name + '):', key)
+print()
+
+kms_client.delete_key(key_name)
+print('delete_key(' + key_name + ')')
+```
+
+For more examples, checkout `sample-client` python  project in [ranger-examples](https://github.com/apache/ranger/blob/master/ranger-examples/sample-client/src/main/python/sample_client.py) module.
```

### Comparing `apache-ranger-0.0.8/apache_ranger.egg-info/SOURCES.txt` & `apache-ranger-0.0.9/apache_ranger.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-ranger-0.0.8/LICENSE` & `apache-ranger-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-ranger-0.0.8/README.md` & `apache-ranger-0.0.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: apache-ranger
+Version: 0.0.9
+Summary: Apache Ranger Python client
+Home-page: https://github.com/apache/ranger/tree/master/intg/src/main/python
+Author: Apache Ranger
+Author-email: dev@ranger.apache.org
+License: Apache LICENSE 2.0
+Keywords: ranger client,apache ranger
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 2.7
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=2.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <!---
 Licensed to the Apache Software Foundation (ASF) under one
 or more contributor license agreements.  See the NOTICE file
 distributed with this work for additional information
 regarding copyright ownership.  The ASF licenses this file
 to you under the Apache License, Version 2.0 (the
 "License"); you may not use this file except in compliance
@@ -31,15 +48,15 @@
 
 Verify if apache-ranger client is installed:
 ```bash
 > pip list
 
 Package      Version
 ------------ ---------
-apache-ranger 0.0.8
+apache-ranger 0.0.9
 ```
 
 ## Usage
 
 ```python test_ranger.py```
 ```python
 # test_ranger.py
@@ -225,7 +242,9 @@
 print()
 
 kms_client.delete_key(key_name)
 print('delete_key(' + key_name + ')')
 ```
 
 For more examples, checkout `sample-client` python  project in [ranger-examples](https://github.com/apache/ranger/blob/master/ranger-examples/sample-client/src/main/python/sample_client.py) module.
+
+
```

### Comparing `apache-ranger-0.0.8/setup.py` & `apache-ranger-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 long_description = ''
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="apache-ranger",
-    version="0.0.8",
+    version="0.0.9",
     author="Apache Ranger",
     author_email="dev@ranger.apache.org",
     description="Apache Ranger Python client",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/apache/ranger/tree/master/intg/src/main/python",
     license='Apache LICENSE 2.0',
```

