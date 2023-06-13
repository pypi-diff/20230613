# Comparing `tmp/geoinsight-0.4.7.tar.gz` & `tmp/geoinsight-0.5.1.tar.gz`

## Comparing `geoinsight-0.4.7.tar` & `geoinsight-0.5.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 geoinsight-0.4.7/geoinsight/src/__init__.py
--rw-r--r--   0        0        0    73943 2020-02-02 00:00:00.000000 geoinsight-0.4.7/geoinsight/src/api.py
--rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 geoinsight-0.4.7/geoinsight/src/geoinsight.py
--rw-r--r--   0        0        0     4999 2020-02-02 00:00:00.000000 geoinsight-0.4.7/geoinsight/src/util.py
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 geoinsight-0.4.7/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geoinsight-0.4.7/LICENSE
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 geoinsight-0.4.7/README.md
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 geoinsight-0.4.7/pyproject.toml
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 geoinsight-0.4.7/PKG-INFO
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 geoinsight-0.5.1/geoinsight/src/__init__.py
+-rw-r--r--   0        0        0    75247 2020-02-02 00:00:00.000000 geoinsight-0.5.1/geoinsight/src/api.py
+-rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 geoinsight-0.5.1/geoinsight/src/geoinsight.py
+-rw-r--r--   0        0        0     4999 2020-02-02 00:00:00.000000 geoinsight-0.5.1/geoinsight/src/util.py
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 geoinsight-0.5.1/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geoinsight-0.5.1/LICENSE
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 geoinsight-0.5.1/README.md
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 geoinsight-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 geoinsight-0.5.1/PKG-INFO
```

### Comparing `geoinsight-0.4.7/geoinsight/src/api.py` & `geoinsight-0.5.1/geoinsight/src/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,44 +1,62 @@
 import requests
 import logging
+from auth0.authentication.token_verifier import TokenVerifier, AsymmetricSignatureVerifier
 
+AUTH0_DOMAIN = 'dev-pcpa2zpghqzahboo.eu.auth0.com'
+AUTH0_CLIENT_ID = 'KiQTUkMsTKEyCZfie0EPvQSDh4YDMndJ'
 
 class api(object):
-    def __init__(self, url):
-        self.url = url
+    def __init__(self):
+        self.url = ""
         self.headers = requests.structures.CaseInsensitiveDict()
         self.headers["Accept"] = "application/json"
         self.headers["Content-Type"] = "application/json"
         self.headers["Accept-Encoding"] = "gzip, deflate, br"
         self.headers["Connection"] = "keep-alive"
         self.headers["Authorization"] = ""
 
-    def is_api_online(self):
-        return requests.get(self.url)
+    def is_online(self):
+        r = requests.get(self.url)
+        if 200 <= r.status_code <= 299:
+            return True
+        else:
+            return False
 
-    def login(self, _email, _pass):
-        endpoint = '/rpc/login'
-        body = {"_email": _email, "_pass": _pass}
-        r = requests.post(self.url + endpoint, json=body, headers=self.headers)
-        if r and r.json()['token'] is not None:
-            self.headers["Authorization"] = "Bearer " + '{token}'.format(token=r.json()['token'])
+    def set_access_token(self, _refresh_token, _client_secret, _apiurl="https://api.geoinsight.ai",):
+        body = {"grant_type": "refresh_token", "client_id": AUTH0_CLIENT_ID, "refresh_token": _refresh_token, "client_secret": _client_secret}
+        r = requests.post('https://{}/oauth/token'.format(AUTH0_DOMAIN), data=body)
+        self.url = _apiurl
+        if 200 <= r.status_code <= 299 and self.is_online():
+            jwks_url = 'https://{}/.well-known/jwks.json'.format(AUTH0_DOMAIN)
+            issuer = 'https://{}/'.format(AUTH0_DOMAIN)
+            sv = AsymmetricSignatureVerifier(jwks_url)
+            tv = TokenVerifier(signature_verifier=sv, issuer=issuer, audience=AUTH0_CLIENT_ID)
+            tv.verify(r.json()['id_token'])
+            self.headers["Authorization"] = "Bearer " + '{token}'.format(token=r.json()['access_token'])
+            logging.info('Access Token has been set')
         else:
-            logging.info('An error has occurred. {e}'.format(e=r.json()))
-        return r
+            logging.error('An error occurred: {e}'.format(e=r.json()))
+        return
 
     def atlas_source(self):
         """API endpoint for atlas_source"""
         endpoint = '/atlas_source'
         return requests.get(self.url + endpoint, headers=self.headers)
 
     def atlas_source_overview(self):
         """API endpoint for atlas_source_overview"""
         endpoint = '/atlas_source_overview'
         return requests.get(self.url + endpoint, headers=self.headers)
 
+    def auth_get_rt(self):
+        """API endpoint for auth_get_rt"""
+        endpoint = '/auth_get_rt'
+        return requests.get(self.url + endpoint, headers=self.headers)
+
     def destination_source_overview(self):
         """API endpoint for destination_source_overview"""
         endpoint = '/destination_source_overview'
         return requests.get(self.url + endpoint, headers=self.headers)
 
     def isea3h_data_aoi(self):
         """API endpoint for isea3h_data_aoi"""
@@ -283,14 +301,34 @@
                  "_dct_references_s": _dct_references_s,
                  "_dct_identifier_sm": _dct_identifier_sm,
                  "_gbl_mdversion_s": _gbl_mdversion_s,
                  "_gi_destination": _gi_destination
                 }
         return requests.post(self.url + endpoint, json=body, headers=self.headers)
 
+    def auth_delete_rt(self, _auth0_refresh_token):
+        """API endpoint /rpc/auth_delete_rt"""
+        endpoint = '/rpc/auth_delete_rt'
+        if type(_auth0_refresh_token) != str and _auth0_refresh_token is not None:
+            logging.error('{}: {} is not {}'.format('_auth0_refresh_token', _auth0_refresh_token, 'text'))
+        body = {
+                 "_auth0_refresh_token": _auth0_refresh_token
+                }
+        return requests.post(self.url + endpoint, json=body, headers=self.headers)
+
+    def auth_insert_rt(self, _auth0_refresh_token):
+        """API endpoint /rpc/auth_insert_rt"""
+        endpoint = '/rpc/auth_insert_rt'
+        if type(_auth0_refresh_token) != str and _auth0_refresh_token is not None:
+            logging.error('{}: {} is not {}'.format('_auth0_refresh_token', _auth0_refresh_token, 'text'))
+        body = {
+                 "_auth0_refresh_token": _auth0_refresh_token
+                }
+        return requests.post(self.url + endpoint, json=body, headers=self.headers)
+
     def check_aoi_exists(self, _aoi):
         """API endpoint /rpc/check_aoi_exists"""
         endpoint = '/rpc/check_aoi_exists'
         if type(_aoi) != str and _aoi is not None:
             logging.error('{}: {} is not {}'.format('_aoi', _aoi, 'text'))
         body = {
                  "_aoi": _aoi
@@ -1001,30 +1039,14 @@
         if type(_hf) != list:
             logging.error('{}: {} is not {}'.format('_hf', _hf, 'ARRAY'))
         body = {
                  "_hf": _hf
                 }
         return requests.post(self.url + endpoint, json=body, headers=self.headers)
 
-    def register(self, _name, _email, _pass):
-        """API endpoint /rpc/register"""
-        endpoint = '/rpc/register'
-        if type(_name) != str and _name is not None:
-            logging.error('{}: {} is not {}'.format('_name', _name, 'text'))
-        if type(_email) != str and _email is not None:
-            logging.error('{}: {} is not {}'.format('_email', _email, 'text'))
-        if type(_pass) != str and _pass is not None:
-            logging.error('{}: {} is not {}'.format('_pass', _pass, 'text'))
-        body = {
-                 "_name": _name,
-                 "_email": _email,
-                 "_pass": _pass
-                }
-        return requests.post(self.url + endpoint, json=body, headers=self.headers)
-
     def task_gendggs_batch(self, _limit=1):
         """API endpoint /rpc/task_gendggs_batch"""
         endpoint = '/rpc/task_gendggs_batch'
         if type(_limit) != int and _limit is not None:
             logging.error('{}: {} is not {}'.format('_limit', _limit, 'integer'))
         body = {
                  "_limit": _limit
```

### Comparing `geoinsight-0.4.7/geoinsight/src/geoinsight.py` & `geoinsight-0.5.1/geoinsight/src/geoinsight.py`

 * *Files identical despite different names*

### Comparing `geoinsight-0.4.7/geoinsight/src/util.py` & `geoinsight-0.5.1/geoinsight/src/util.py`

 * *Files identical despite different names*

### Comparing `geoinsight-0.4.7/.gitignore` & `geoinsight-0.5.1/.gitignore`

 * *Files identical despite different names*

