# Comparing `tmp/NovumApiClient-0.0.8.tar.gz` & `tmp/novumapiclient-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NovumApiClient-0.0.8.tar", last modified: Mon Feb 13 14:47:07 2023, max compression
+gzip compressed data, was "novumapiclient-0.0.9.tar", max compression
```

## Comparing `NovumApiClient-0.0.8.tar` & `novumapiclient-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,6 @@
-drwxrwxr-x   0 leonardo  (1001) leonardo  (1001)        0 2023-02-13 14:47:07.961683 NovumApiClient-0.0.8/
--rw-rw-r--   0 leonardo  (1001) leonardo  (1001)        0 2023-02-08 08:09:41.000000 NovumApiClient-0.0.8/LICENSE
--rw-rw-r--   0 leonardo  (1001) leonardo  (1001)      397 2023-02-13 14:47:07.961683 NovumApiClient-0.0.8/PKG-INFO
--rw-rw-r--   0 leonardo  (1001) leonardo  (1001)      375 2023-02-13 14:43:40.000000 NovumApiClient-0.0.8/README.md
--rw-rw-r--   0 leonardo  (1001) leonardo  (1001)      105 2023-02-08 08:58:46.000000 NovumApiClient-0.0.8/pyproject.toml
--rw-rw-r--   0 leonardo  (1001) leonardo  (1001)      489 2023-02-13 14:47:07.961683 NovumApiClient-0.0.8/setup.cfg
-drwxrwxr-x   0 leonardo  (1001) leonardo  (1001)        0 2023-02-13 14:47:07.957683 NovumApiClient-0.0.8/src/
-drwxrwxr-x   0 leonardo  (1001) leonardo  (1001)        0 2023-02-13 14:47:07.957683 NovumApiClient-0.0.8/src/NovumApiClient/
--rw-rw-r--   0 leonardo  (1001) leonardo  (1001)        0 2023-02-08 08:09:41.000000 NovumApiClient-0.0.8/src/NovumApiClient/__init__.py
--rw-rw-r--   0 leonardo  (1001) leonardo  (1001)    10264 2023-02-13 14:19:08.000000 NovumApiClient-0.0.8/src/NovumApiClient/apiClientBase.py
--rw-rw-r--   0 leonardo  (1001) leonardo  (1001)    12924 2023-02-13 14:34:31.000000 NovumApiClient-0.0.8/src/NovumApiClient/apiClientPublic.py
-drwxrwxr-x   0 leonardo  (1001) leonardo  (1001)        0 2023-02-13 14:47:07.961683 NovumApiClient-0.0.8/src/NovumApiClient.egg-info/
--rw-rw-r--   0 leonardo  (1001) leonardo  (1001)      397 2023-02-13 14:47:07.000000 NovumApiClient-0.0.8/src/NovumApiClient.egg-info/PKG-INFO
--rw-rw-r--   0 leonardo  (1001) leonardo  (1001)      315 2023-02-13 14:47:07.000000 NovumApiClient-0.0.8/src/NovumApiClient.egg-info/SOURCES.txt
--rw-rw-r--   0 leonardo  (1001) leonardo  (1001)        1 2023-02-13 14:47:07.000000 NovumApiClient-0.0.8/src/NovumApiClient.egg-info/dependency_links.txt
--rw-rw-r--   0 leonardo  (1001) leonardo  (1001)       15 2023-02-13 14:47:07.000000 NovumApiClient-0.0.8/src/NovumApiClient.egg-info/top_level.txt
+-rw-r--r--   0        0        0     1064 2023-06-12 12:38:04.666162 novumapiclient-0.0.9/LICENSE
+-rw-r--r--   0        0        0      371 2023-06-12 13:12:03.524610 novumapiclient-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-12 12:37:13.494428 novumapiclient-0.0.9/src/novumapiclient/__init__.py
+-rw-r--r--   0        0        0     9201 2023-06-12 12:37:13.494428 novumapiclient-0.0.9/src/novumapiclient/base.py
+-rw-r--r--   0        0        0    15320 2023-06-12 13:12:11.120497 novumapiclient-0.0.9/src/novumapiclient/public.py
+-rw-r--r--   0        0        0      569 1970-01-01 00:00:00.000000 novumapiclient-0.0.9/PKG-INFO
```

### Comparing `NovumApiClient-0.0.8/src/NovumApiClient/apiClientBase.py` & `novumapiclient-0.0.9/src/novumapiclient/base.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,284 +1,241 @@
+# pylint: disable=C0115
+# pylint: disable=C0116
+# pylint: disable=C0301
+# flake8: noqa
+
+import hashlib
 import json
-import requests
-import urllib
-import math
-from hashlib import md5
-import jwt
 import time
 import base64
+import urllib
+import requests
 from threading import Timer
 
 TOKEN_REFRESH_INTERVAL_SCALE = 0.9
 UNMISTAKABLE_CHARS = "23456789ABCDEFGHJKLMNPQRSTWXYZabcdefghijkmnopqrstuvwxyz"
 PRODUCTION_API_HOST = "https://novum-batteries.com"
 
 
-def with_filter_or_option(
-    url: str,
-    filter: dict,
-    option: dict,
-    fields: dict,
-):
-    query = {}
-    if len(filter) != 0:
-        query["filter"] = json.dumps(filter)
-    if len(option) != 0:
-        query["option"] = json.dumps(option)
-    if len(fields) != 0:
-        query["fields"] = json.dumps(fields)
-    return url, query.json()  # withQuery
-
-
-def getSHA256(toHash: str) -> str:
-    return md5("sha256").update(toHash).hexdigest("hex")
-
-
-def gen_mongo_id(charsCount=17) -> str:
-    def choice(arrayOrString: str):
-        index = math.floor(math.random() * len(arrayOrString))
-        if type(arrayOrString) == "string":
-            return arrayOrString.substr(index, 1)
-        return arrayOrString[index]
-
-    result = 0
-    for i in range(0, charsCount):
-        result += choice(UNMISTAKABLE_CHARS)
-    return result
+class novum_api_error(Exception):
+    def __init__(self, message: str, status_code: int):
+        self.message = message
+        self.status_code = status_code
+        super().__init__(f"novum_api_error: {message} (status: {status_code})")
+
+
+def getSHA256(to_hash: str) -> str:
+    return hashlib.sha256(to_hash).hexdigest()
 
 
 def user_name(user: dict) -> str:
     return user["profile"]["name"]
 
 
 def full_name(user: dict) -> str:
-    if len(user != None):
+    if len(user.keys()) > 0:
         return str(user["profile"]["first_name"]) + str(user["profile"]["family_name"])
     else:
-        return "User not found!"
+        raise novum_api_error("User not found!", 400)
 
 
-def parse_jwt(token: str) -> any:
-    base64Input = token.split(".")[1]
-    base64 = base64Input.replace("/-/g", "+").replace("/_/g", "/")
-    return jwt.decode(base64, verify=False)
-
-
-class APIError:
-    def __init__(self, res: any):
-        self._text = ""
-        self._json = None
-        self._res = res
-        self._code = res.status
-        self.details = None
-
-    def resolve(self) -> str:
-        try:
-            response = str(self._res)
-            self._text = response
-            try:
-                self._json = json.loads(self._text)
-            except:
-                self._json = {"body": self._text}
-                self.details = {"json": self._json, "code": self._code, "headers": self._res.headers}
-                return self._json["error"]
-        except:
-            return "Unknown API Error"
+def parse_jwt(token: str) -> dict:
+    base64_input = token.split(".")[1]
+    base64_bytes = base64_input.encode("utf-8")
+    # replace '-' with '+' and '_' with '/' as base64url is different than base64
+    base64_bytes += b"=" * (4 - len(base64_bytes) % 4)
+    base64_string = base64_bytes.decode("utf-8").replace("-", "+").replace("_", "/")
+    if "window" in base64_string:
+        json_payload = urllib.parse.unquote(base64.b64decode(base64_string).decode("utf-8"))
+    else:
+        json_payload = urllib.parse.unquote(base64.b64decode(base64_string.encode("utf-8")).decode("utf-8"))
+    return json.loads(json_payload)
 
 
-class BaseAPIClient:
+class base_api_client:
     def __init__(
         self,
-        user="",
-        _host=PRODUCTION_API_HOST,
-        _refreshTokenWarning=True,
-        _refreshIntervalScale=TOKEN_REFRESH_INTERVAL_SCALE,
-        props=None,
+        user=None,
+        host=PRODUCTION_API_HOST,
+        refresh_token_warning=True,
+        refresh_interval_scale=TOKEN_REFRESH_INTERVAL_SCALE,
+        _relogin_timer_handle=None,
+        _authenticated=False,
     ):
         self.user = user
-        self._host = _host
-        self._props = props
-        self._refreshTokenWarning = _refreshTokenWarning
-        self._refreshIntervalScale = _refreshIntervalScale
-
-    @staticmethod
-    def fromWindowLocation(window):
-        return BaseAPIClient(window.location.origin)
+        self.headers = (
+            None
+            if user is None
+            else dict({"Content-Type": "application/json", "Authorization": "Bearer " + str(self.user.get("jwt"))})
+        )
+        self.host = host
+        self._refresh_token_warning = refresh_token_warning
+        self._refresh_interval_scale = refresh_interval_scale
+        self._relogin_timer_handle = _relogin_timer_handle
+        self._authenticated = _authenticated
 
     def _set_user(self, user):
-        if user != "" and user["jwt"] != None:
+        if len(user.keys()) > 0 and user.get("jwt") is not None:
             user["expires_at"] = self._get_expire_time_from_token_in_unix_time_millis(user["jwt"]).isoformat()
             self.user = user
             self._install_token_refresh_procedure(user)
 
     def _clear_user(self):
         self.user = None
         self._remove_relogin_timer_handle()
 
     def _remove_relogin_timer_handle(self):
-        if self._reLoginTimerHandle != None:
-            # clearTimeout(self._reLoginTimerHandle)
-            self._reLoginTimerHandle = None
+        if self._relogin_timer_handle is not None:
+            # clearTimeout(self._reloginTimerHandle)
+            self._relogin_timer_handle = None
 
     def _get_expire_time_from_token_in_unix_time_millis(self, token: str) -> float:
-        if token != None:
-            innerToken = json.load(token)
-            if innerToken != None and innerToken["exp"] != None and type(innerToken["exp"]) == str:
-                return 1000 * innerToken["exp"]
+        if token is not None:
+            inner_token = parse_jwt(token)
+            if inner_token is not None:
+                return 1000 * inner_token["exp"]
         return 3600 * 1000
 
     def _install_token_refresh_procedure(self, user):
         self._remove_relogin_timer_handle()
-        expire_time_In_millis = self._get_expire_time_from_token_in_unix_time_millis(self.user["jwt"])
-        now = time.time()
+        expire_time_in_millis = self._get_expire_time_from_token_in_unix_time_millis(self.user["jwt"])
+        now = time.time() * 1000
 
-        if expire_time_In_millis != None and expire_time_In_millis > 1000 + now:
-            if user["refresh_token"] != None:
-                refreshIntervalInMillis = math.round(self._refreshIntervalScale * (expire_time_In_millis - now))
-                self._reLoginTimerHandle = Timer(self._refreshAccessToken, refreshIntervalInMillis)
+        if expire_time_in_millis is not None and expire_time_in_millis > 1000 + now:
+            if user.get("refresh_token") is not None:
+                refresh_interval_in_millis = round(self._refresh_interval_scale * (expire_time_in_millis - now), 10)
+                self._relogin_timer_handle = Timer(self._refresh_access_token, refresh_interval_in_millis)
             else:
-                if self._refreshTokenWarning:
-                    print("APIClient: There is no refreshToken! Autorefresh of access tokens is not possible.")
+                if self._refresh_token_warning:
+                    raise ValueError(
+                        "APIClient: There is no refreshToken! Autorefresh of access tokens is not possible."
+                    )
                 else:
-                    print("APIClient: Could not get expire_time_In_millis or token has already expired.")
+                    raise ValueError("APIClient: Could not get expire_time_In_millis or token has already expired.")
 
     def _refresh_access_token(self):
-        if self.user != None and self.user.refresh_token != None:
-            print("APIClient._refreshAccessToken - Refreshing the accesToken for userId" + self.user["id"])
-            refresh_token = self.user
-            new_access_object = self._post("/api/batman/v1/refresh", {refresh_token})
-            if new_access_object["jwt"] != None:
-                self._set_user(self.user, new_access_object)
+        if self.user is not None and self.user.get("refresh_token") is not None:
+            print("APIClient._refreshAccessToken - Refreshing the accessToken for userId" + self.user.get("id"))
+            new_access_object = self._post_json("/api/batman/v1/refresh", self.user)
+            if new_access_object.get("jwt") is not None:
+                self._set_user(self.user)
             else:
                 print("APIClient._refreshAccessToken - Error no user or refesh token found!")
 
-    def _fetch_by_URL(self, url: str, options: any):
+    def _fetch_by_URL(self, url: str, options: dict):
         response = self._get_json(url, option=options)
-        if response["ok"] == False:
-            error = APIError(f"Failed to load resource {url} -> Status:" + response["status"], response)
-            error.resolve()
-            return error
+        if response.get("ok") is False:
+            raise ValueError(f"Failed to load resource {url} -> Status:" + response.get("status"))
         return response
 
-    def _post_by_URL(self, url: str, options: any):
+    def _post_by_URL(self, url: str, options: dict):
         response = self._post_json(url, option=options)
-        if response["ok"] == False:
-            error = APIError(f"Failed to load resource {url} -> Status:" + response["status"], response)
-            error.resolve()
-            return error
+        if response.get("ok") is False:
+            raise ValueError(f"Failed to load resource {url} -> Status:" + response.get("status"), response)
         return response
 
-    def _fetch_by_path(self, path: str, options: any):
-        return self._fetch_by_URL(self._host + path, options)
+    def _fetch_by_path(self, path: str, options: dict):
+        return self._fetch_by_URL(self.host + path, options)
 
-    def _post_by_path(self, path: str, options: any):
-        return self._post_by_URL(self._host + path, options)
+    def _post_by_path(self, path: str, options: dict) -> dict:
+        return self._post_by_URL(self.host + path, options)
 
     def _encode_auth_header(self, username: str, password: str):
         return {"Authorization": "Basic " + str(base64.b64encode(username, password).decode("utf-8"))}
 
     def _headers(self, headers):
-        if self.user != None and self.user["jwt"] != None:
-            headers["Authorization"] = "Bearer " + str(self.user["jwt"])
+        if self.user is not None and self.user.get("jwt") is not None:
+            headers["Authorization"] = f"Bearer {self.user['jwt']}"
         return headers
 
-    def _get_json(self, url: str, filter=None, option=None, timeout: float = 4.0):
-        full_url = str(self._host) + url
-        headers = dict({"Content-Type": "application/json", "Authorization": "Bearer " + self.user["jwt"]})
-        param = {"filter": json.dumps(filter), "option": json.dumps(option)}
-        params = urllib.parse.urlencode(param)
-
+    def _get_json(self, url: str, filter_json=None, option=None, timeout: float = 4.0):
+        full_url = str(self.host) + url
+        headers = self.headers
+        params_json = {"filter": json.dumps(filter_json), "option": json.dumps(option)}
         response = requests.get(
             url=full_url,
             headers=headers,
-            params=params,
+            params=params_json,
             timeout=timeout,
         )
-
-        if response.status_code == requests.codes.ok:
+        if response.status_code == requests.codes.get("ok"):
             return response.json()
         else:
-            print("Error: Unable to get the data.", response.status_code)
+            raise novum_api_error("Unable to get data.", response.status_code)
 
-    def _post_file(self, path: str, file, headers):
-        files = {"upload_file": open(file)}
-        response = self._post_by_path(path, headers=headers, files=files)
-        return response.json()
-
-    def _post_json(self, url: str, data=None, filter=None, option=None, timeout: float = 4.0):
-        full_url = self._host + url
-        headers = dict({"Content-Type": "application/json", "Authorization": "Bearer " + self.user["jwt"]})
-        param = {"filter": json.dumps(filter), "option": json.dumps(option)}
-        params = urllib.parse.urlencode(param)
+    def _post_file(self, path: str, file):
+        options = {"upload_file": open(file)}
+        return self._post_by_path(path, options=options)
+
+    def _post_json(self, url: str, data=None, filter_json=None, option=None, timeout: float = 4):
+        full_url = self.host + url
+        headers = self.headers
+        params_json = {"filter": json.dumps(filter_json), "option": json.dumps(option)}
         data = json.dumps(data)
 
         response = requests.post(
             url=full_url,
             headers=headers,
-            params=params,
+            params=params_json,
             data=data,
             timeout=timeout,
         )
 
-        if response.status_code == requests.codes.ok:
+        if response.status_code == requests.codes.get("ok"):
             return response.json()
+
         else:
-            print("Error: The data could not be posted.", response.status_code)
+            raise novum_api_error("The data could not be posted", response.status_code)
 
-    def _put_json(self, url: str, data=None, filter=None, option=None, timeout: float = 4.0):
-        full_url = self._host + url
-        headers = dict({"Content-Type": "application/json", "Authorization": "Bearer " + self.user["jwt"]})
-        param = {"filter": json.dumps(filter), "option": json.dumps(option)}
-        params = urllib.parse.urlencode(param)
-        data = json.dumps(data)
+    def _put_json(self, url: str, data=None, filter_json=None, option=None, timeout: float = 4):
+        full_url = self.host + url
+        headers = self.headers
+        params_json = {"filter": json.dumps(filter_json), "option": json.dumps(option)}
+        data_json = json.dumps(data)
 
         response = requests.put(
             url=full_url,
             headers=headers,
-            params=params,
-            data=data,
+            params=params_json,
+            data=data_json,
             timeout=timeout,
         )
 
-        if response.status_code == requests.codes.ok:
+        if response.status_code == requests.codes.get("ok"):
             return response.json()
         else:
-            print("Error: The data was nou updated.", response.status_code)
+            raise novum_api_error("The data was not updated", response.status_code)
 
-    def _delete_json(self, url: str, filter=None, option=None, timeout: float = 4.0):
-        full_url = self._host + url
-        headers = dict({"Content-Type": "application/json", "Authorization": "Bearer " + self.user["jwt"]})
-        param = {"filter": json.dumps(filter), "option": json.dumps(option)}
-        params = urllib.parse.urlencode(param)
+    def _delete_json(self, url: str, filter_json=None, option=None, timeout: float = 4.0):
+        full_url = self.host + url
+        headers = self.headers
+        params_json = {"filter": json.dumps(filter_json), "option": json.dumps(option)}
 
         response = requests.delete(
             url=full_url,
             headers=headers,
-            params=params,
+            params=params_json,
             timeout=timeout,
         )
-        if response.status_code == requests.codes.ok:
-            return response.json()
+        if response.status_code <= 204:
+            return response
         else:
-            print("Error: The data was not removed.", response.status_code)
+            raise novum_api_error("The data was not removed", response.status_code)
 
     def _get_text(self, path: str, headers=None):
-        headers = headers.update({"Content-Type": "application/text"})
-        response = self._fetch_by_path(path, headers=headers)
+        headers.update({"Content-Type": "application/text"})
+        response = self._fetch_by_path(path, options=headers)
         return response.text()
 
-    def _get_array_buffer(self, path: str, headers):
-        headers = headers.update({"Content-Type": "application/text"})
-        response = self._fetch_by_path(path, headers=headers)
-        return [int(i) for i in response.content]
+    def _get_array_buffer(self, path: str, headers=None):
+        headers.update({"Content-Type": "application/text"})
+        response = self._fetch_by_path(path, options=headers)
+        return [int(i) for i in response.get("content")]
 
-    def host(self) -> str:
-        return self._host
+    def _host(self) -> str:
+        return self.host
 
     def authenticated(self) -> bool:
         return self._authenticated
 
-    def set_new_endpoint(self, newEndPoint: str):
-        self._host = newEndPoint
-
-    def _is_APIError(self, objectOrError) -> bool:
-        return objectOrError != None and objectOrError.details != None and objectOrError.details.code != None
+    def set_new_endpoint(self, new_end_point: str):
+        self.host = new_end_point
```

