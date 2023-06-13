# Comparing `tmp/tabulario-0.3.0.tar.gz` & `tmp/tabulario-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tabulario-0.3.0.tar", max compression
+gzip compressed data, was "tabulario-0.3.1.tar", max compression
```

## Comparing `tabulario-0.3.0.tar` & `tabulario-0.3.1.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0    11358 2023-02-14 11:04:14.321381 tabulario-0.3.0/LICENSE
--rw-r--r--   0        0        0     6005 2023-02-14 11:04:14.321381 tabulario-0.3.0/README.md
--rw-r--r--   0        0        0     2487 2023-02-14 11:04:24.313656 tabulario-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      785 2023-02-14 11:04:14.325381 tabulario-0.3.0/tab/__init__.py
--rw-r--r--   0        0        0     3786 2023-02-14 11:04:14.325381 tabulario-0.3.0/tab/cli.py
--rw-r--r--   0        0        0      871 2023-02-14 11:04:14.325381 tabulario-0.3.0/tab/exceptions.py
--rw-r--r--   0        0        0     5185 2023-02-14 11:04:14.325381 tabulario-0.3.0/tab/oauth.py
--rw-r--r--   0        0        0     1004 2023-02-14 11:04:14.325381 tabulario-0.3.0/tab/util.py
--rw-r--r--   0        0        0        0 2023-02-14 11:04:14.325381 tabulario-0.3.0/tabular/__init__.py
--rw-r--r--   0        0        0     4955 2023-02-14 11:04:14.325381 tabulario-0.3.0/tabular/loader.py
--rw-r--r--   0        0        0     6892 1970-01-01 00:00:00.000000 tabulario-0.3.0/setup.py
--rw-r--r--   0        0        0     7018 1970-01-01 00:00:00.000000 tabulario-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-06-13 07:58:34.858905 tabulario-0.3.1/LICENSE
+-rw-r--r--   0        0        0     5831 2023-06-13 07:58:34.858905 tabulario-0.3.1/README.md
+-rw-r--r--   0        0        0     2487 2023-06-13 07:58:51.099009 tabulario-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      785 2023-06-13 07:58:34.858905 tabulario-0.3.1/tab/__init__.py
+-rw-r--r--   0        0        0     3716 2023-06-13 07:58:34.858905 tabulario-0.3.1/tab/cli.py
+-rw-r--r--   0        0        0      871 2023-06-13 07:58:34.858905 tabulario-0.3.1/tab/exceptions.py
+-rw-r--r--   0        0        0     5045 2023-06-13 07:58:34.858905 tabulario-0.3.1/tab/oauth.py
+-rw-r--r--   0        0        0     1004 2023-06-13 07:58:34.858905 tabulario-0.3.1/tab/util.py
+-rw-r--r--   0        0        0        0 2023-06-13 07:58:34.858905 tabulario-0.3.1/tabular/__init__.py
+-rw-r--r--   0        0        0     4955 2023-06-13 07:58:34.858905 tabulario-0.3.1/tabular/loader.py
+-rw-r--r--   0        0        0     6642 1970-01-01 00:00:00.000000 tabulario-0.3.1/PKG-INFO
```

### Comparing `tabulario-0.3.0/LICENSE` & `tabulario-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tabulario-0.3.0/README.md` & `tabulario-0.3.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -38,17 +38,15 @@
 ```bash
 ➜ tab request-token t-GdCZGj5OpoQ:jIcDDITVeIOnqxo7FxWbI21Y3kI | jq
 {
     "access_token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJSUzUxMiJ9.eyJjcmVkc0tleSI6InQtR2RDWkdqNU9wb1EiLCJzdWJJZCI6ImViMzc2NTQ4LTIwNmItNDBiYS1hN2E1LWVkYmUzZjg4YWVlZCIsInN1YiI6ImZva2tvQHRhYnVsYXIuaW8iLCJ3YXJlaG91c2VJZCI6IjhiY2IwODM4LTUwZmMtNDcyZC05ZGRiLThmZWI4OWVmNWYxZSIsImlzcyI6InRhYnVsYXIuaW8iLCJsb2NhdGlvbiI6InMzOi8vdGFidWxhci13aC11cy13ZXN0LTItZGV2LzhiY2IwODM4LTUwZmMtNDcyZC05ZGRiLThmZWI4OWVmNWYxZS8iLCJ0eXBlIjoiV0FSRUhPVVNFIiwicmVnaW9uIjoidXMtd2VzdC0yIiwiZXhwIjoxNjY1NzU1MzU2LCJpYXQiOjE2NjU2Njg5NTYsImp0aSI6IjRhZjcyMzk3LTVlOGQtNDc0OS1iZThmLWI4OTFmYTMwNjNhNiIsIm9yZ0lkIjoiMWM1MmU4MzItMjY2Yy00OTYxLTk3YWYtMTE1ZDFiNzJmY2UwIn0.sTu-j2lGG02Ui_Ts7_rMfkT-zha6ugMzz0JyiumHpTupqEXnDdNiaxyEJmJcu81IcjEaWwT32hxAlznLy6Qhr-yTeSoVY5pJnTiXMNxeAZwzDkGh87uLcp0PjgwRLc6DmD3ZAXC2WQEUf8PS_mcMXF_6HoegHv1GHGLk9aHhWLze6WI_SIKSLc0Gmw8ZjjZoUpL8SSwt-uinT8gY_D0TksHkeVzM5DFxhLvhXMjJ1VyRUbsrE_6An83-aG0NzsFFgK3IhCf-RsEsOXH1MKZpdLdIlelcz8Av1uFzgWA6kFAcy9dGVZu_Ycj19e58e17IKHgLbtk4cc4wJOAg6lCBsw",
     "issued_token_type": "urn:ietf:params:oauth:token-type:access_token",
     "token_type": "Bearer",
     "expires_in": 86400,
-    "scope": null,
-    "warehouse_id": "8bcb0838-50fc-472d-9ddb-8feb89ef5f1e",
-    "region": "us-west-2"
+    "scope": null
 }
 ```
 
 Also, stdin is supported:
 
 ```bash
 ➜ cat cred.json | jq
@@ -57,17 +55,15 @@
 }
 ➜ cat cred.json | tab request-token | jq
 {
     "access_token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJSUzUxMiJ9.eyJjcmVkc0tleSI6InQtR2RDWkdqNU9wb1EiLCJzdWJJZCI6ImViMzc2NTQ4LTIwNmItNDBiYS1hN2E1LWVkYmUzZjg4YWVlZCIsInN1YiI6ImZva2tvQHRhYnVsYXIuaW8iLCJ3YXJlaG91c2VJZCI6IjhiY2IwODM4LTUwZmMtNDcyZC05ZGRiLThmZWI4OWVmNWYxZSIsImlzcyI6InRhYnVsYXIuaW8iLCJsb2NhdGlvbiI6InMzOi8vdGFidWxhci13aC11cy13ZXN0LTItZGV2LzhiY2IwODM4LTUwZmMtNDcyZC05ZGRiLThmZWI4OWVmNWYxZS8iLCJ0eXBlIjoiV0FSRUhPVVNFIiwicmVnaW9uIjoidXMtd2VzdC0yIiwiZXhwIjoxNjY1NzU1Mjg2LCJpYXQiOjE2NjU2Njg4ODYsImp0aSI6IjZhNzljNzU1LTYzNGEtNDJlNC04YmVlLTEzZjgxOWFlYTYyNCIsIm9yZ0lkIjoiMWM1MmU4MzItMjY2Yy00OTYxLTk3YWYtMTE1ZDFiNzJmY2UwIn0.WZNP_e-cMKX9pj7ydPA_sm2Zyy54Iht1bOx7g3lr8p5NRh8jyyD2RHY1hAhvDgLASZr49vBcjAsbRdvmq3WEAO_LV3c_ts-5edDhLfetAfmcDjR5Xv70HDvpmofkEkZVK7HE8P_IPA6z2YX-CbnEcAHPzZ3hrjfR6nc2ouo0h8tlg6OqmT8w75aX5PA9inh6xquMhBLYSfeGlET5XF3fryQ6Kd2PfTTftMRqo-DbkdMHHF7t8E8wrbf-I7cE7--o_KfF2paaebyRAuS9n7RSdOw82FL2dBn9V3cMwyNeTPH05m6OKChnXenG9xorgKnRkEeB_P6UdwEPcPH8YeQJHA",
     "issued_token_type": "urn:ietf:params:oauth:token-type:access_token",
     "token_type": "Bearer",
     "expires_in": 86400,
-    "scope": null,
-    "warehouse_id": "8bcb0838-50fc-472d-9ddb-8feb89ef5f1e",
-    "region": "us-west-2"
+    "scope": null
 }
 ```
 
 ### Requesting a user access token
 
 ```bash
 tab request-user-token eyJ0e...eQJHA urn:ietf:params:oauth:token-type:id_token eyJ0e...eQJHA urn:ietf:params:oauth:token-type:access_token | jq
```

### Comparing `tabulario-0.3.0/pyproject.toml` & `tabulario-0.3.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 [tool.poetry]
 name = "tabulario"
-version = "0.3.0"
+version = "0.3.1"
 readme = "README.md"
 homepage = "https://tabular.io/"
 repository = "https://github.com/tabular-io/"
 description = "Utility library for Tabular.io"
 authors = ["Tabular Technologies, Inc. <fokko@tabular.io>"]
 license = "Apache License 2.0"
```

### Comparing `tabulario-0.3.0/tab/__init__.py` & `tabulario-0.3.1/tab/__init__.py`

 * *Files identical despite different names*

### Comparing `tabulario-0.3.0/tab/cli.py` & `tabulario-0.3.1/tab/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,22 +19,21 @@
 from dataclasses import dataclass
 from json import JSONDecodeError
 from typing import (
     Any,
     Dict,
     List,
     Optional,
-    Union,
 )
 
 import click
 from click import Context
 
 from tab.exceptions import InvalidInputError
-from tab.oauth import ClientOauthTokenResponse, OAuthTokenResponse, TabularOAuth
+from tab.oauth import OAuthTokenResponse, TabularOAuth
 from tab.util import EnhancedJSONEncoder
 
 
 @dataclass(frozen=True)
 class TabularContext:
     environment: str
 
@@ -54,15 +53,15 @@
                 return json.loads(raw_json)
         except JSONDecodeError as e:
             raise InvalidInputError("Invalid JSON") from e
 
     return None
 
 
-def _out(output: Union[OAuthTokenResponse, ClientOauthTokenResponse]):
+def _out(output: OAuthTokenResponse):
     click.echo(json.dumps(output, cls=EnhancedJSONEncoder))
 
 
 @run.command()
 @click.pass_obj
 @click.argument("credential", required=False)
 @click.argument("scopes", required=False, nargs=-1)
```

### Comparing `tabulario-0.3.0/tab/exceptions.py` & `tabulario-0.3.1/tab/exceptions.py`

 * *Files identical despite different names*

### Comparing `tabulario-0.3.0/tab/oauth.py` & `tabulario-0.3.1/tab/oauth.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,20 +61,14 @@
     access_token: str
     issued_token_type: str
     token_type: str
     expires_in: Optional[int]
     scope: Optional[str]
 
 
-@dataclass(frozen=True)
-class ClientOauthTokenResponse(OAuthTokenResponse):
-    warehouse_id: str
-    region: str
-
-
 def _parse_scopes(scopes: Any) -> Set[str]:
     if scopes:
         if isinstance(scopes, str):
             return {scopes}
         else:
             # Assume that it is some kind of iterable
             return set(scopes)
@@ -96,38 +90,38 @@
     except HTTPError as e:
         raise ValueError(f"Request failed {response.text}") from e
 
     return response_type(**{**{"scope": None, "expires_in": None}, **response.json()})
 
 
 ENVIRONMENT_URLS = {
-    "prod": "https://api.tabulardata.io/ws/v1/oauth/tokens",
-    "test": "https://api.test.tabulardata.io/ws/v1/oauth/tokens",
-    "dev": "https://api.dev.tabulardata.io/ws/v1/oauth/tokens",
+    "prod": "https://api.tabular.io/ws/v1/oauth/tokens",
+    "test": "https://api.test.tabular.io/ws/v1/oauth/tokens",
+    "dev": "https://api.dev.tabular.io/ws/v1/oauth/tokens",
 }
 
 
 class TabularOAuth:
     base_url: str
 
     def __init__(self, environment: str):
         self.base_url = ENVIRONMENT_URLS[environment]
 
-    def request_token(self, credential: str, scopes: Optional[Any] = None) -> ClientOauthTokenResponse:
+    def request_token(self, credential: str, scopes: Optional[Any] = None) -> OAuthTokenResponse:
         if SEMICOLON in credential:
             client_id, client_secret = credential.split(SEMICOLON)
         else:
             client_id, client_secret = None, credential
 
         payload = {GRANT_TYPE: CLIENT_CREDENTIALS, CLIENT_SECRET: client_secret, SCOPE: _join_scopes(_parse_scopes(scopes))}
 
         if client_id is not None:
             payload[CLIENT_ID] = client_id
 
-        return _do_request(self.base_url, payload, ClientOauthTokenResponse)
+        return _do_request(self.base_url, payload, OAuthTokenResponse)
 
     def request_user_token(
         self,
         service_token: str,
         id_token: str,
         service_token_type: str = TOKEN_ACCESS_TYPE,
         id_token_type: str = TOKEN_JWT_TYPE,
```

### Comparing `tabulario-0.3.0/tab/util.py` & `tabulario-0.3.1/tab/util.py`

 * *Files identical despite different names*

### Comparing `tabulario-0.3.0/tabular/loader.py` & `tabulario-0.3.1/tabular/loader.py`

 * *Files identical despite different names*

### Comparing `tabulario-0.3.0/setup.py` & `tabulario-0.3.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,113 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: tabulario
+Version: 0.3.1
+Summary: Utility library for Tabular.io
+Home-page: https://tabular.io/
+License: Apache-2.0
+Author: Tabular Technologies, Inc.
+Author-email: fokko@tabular.io
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: pyiceberg (==0.3.0)
+Requires-Dist: requests (>=2.28.1,<3.0.0)
+Project-URL: Repository, https://github.com/tabular-io/
+Description-Content-Type: text/markdown
+
+# Tab
+
+This is a helper library to easily fetch and refresh access token from Tabular.
+
+## Usage
+
+Every command has `--help` available:
+
+```bash
+➜ tab --help
+Usage: tab [OPTIONS] COMMAND [ARGS]...
+
+Options:
+--environment TEXT
+--help              Show this message and exit.
+
+Commands:
+refresh-token       Retrieves a fresh token based on an existing token
+request-token       Retrieves an access token based on credentials
+request-user-token  Retrieves a user token based on credentials
+```
+
+And the specific commands:
+
+```bash
+➜ tab request-user-token --help
+Usage: tab request-user-token [OPTIONS] [SERVICE_TOKEN] [SERVICE_TOKEN_TYPE]
+[ID_TOKEN] [ID_TOKEN_TYPE] [SCOPES]...
+
+Retrieves a user token based on credentials
+
+Options:
+--help  Show this message and exit.
+```
+
+### Requesting access token
+
+```bash
+➜ tab request-token t-GdCZGj5OpoQ:jIcDDITVeIOnqxo7FxWbI21Y3kI | jq
+{
+    "access_token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJSUzUxMiJ9.eyJjcmVkc0tleSI6InQtR2RDWkdqNU9wb1EiLCJzdWJJZCI6ImViMzc2NTQ4LTIwNmItNDBiYS1hN2E1LWVkYmUzZjg4YWVlZCIsInN1YiI6ImZva2tvQHRhYnVsYXIuaW8iLCJ3YXJlaG91c2VJZCI6IjhiY2IwODM4LTUwZmMtNDcyZC05ZGRiLThmZWI4OWVmNWYxZSIsImlzcyI6InRhYnVsYXIuaW8iLCJsb2NhdGlvbiI6InMzOi8vdGFidWxhci13aC11cy13ZXN0LTItZGV2LzhiY2IwODM4LTUwZmMtNDcyZC05ZGRiLThmZWI4OWVmNWYxZS8iLCJ0eXBlIjoiV0FSRUhPVVNFIiwicmVnaW9uIjoidXMtd2VzdC0yIiwiZXhwIjoxNjY1NzU1MzU2LCJpYXQiOjE2NjU2Njg5NTYsImp0aSI6IjRhZjcyMzk3LTVlOGQtNDc0OS1iZThmLWI4OTFmYTMwNjNhNiIsIm9yZ0lkIjoiMWM1MmU4MzItMjY2Yy00OTYxLTk3YWYtMTE1ZDFiNzJmY2UwIn0.sTu-j2lGG02Ui_Ts7_rMfkT-zha6ugMzz0JyiumHpTupqEXnDdNiaxyEJmJcu81IcjEaWwT32hxAlznLy6Qhr-yTeSoVY5pJnTiXMNxeAZwzDkGh87uLcp0PjgwRLc6DmD3ZAXC2WQEUf8PS_mcMXF_6HoegHv1GHGLk9aHhWLze6WI_SIKSLc0Gmw8ZjjZoUpL8SSwt-uinT8gY_D0TksHkeVzM5DFxhLvhXMjJ1VyRUbsrE_6An83-aG0NzsFFgK3IhCf-RsEsOXH1MKZpdLdIlelcz8Av1uFzgWA6kFAcy9dGVZu_Ycj19e58e17IKHgLbtk4cc4wJOAg6lCBsw",
+    "issued_token_type": "urn:ietf:params:oauth:token-type:access_token",
+    "token_type": "Bearer",
+    "expires_in": 86400,
+    "scope": null
+}
+```
+
+Also, stdin is supported:
 
-packages = \
-['tab', 'tabular']
+```bash
+➜ cat cred.json | jq
+{
+    "credential": "t-GdCZGj5OpoQ:jIcDDITVeIOnqxo7FxWbI21Y3kI"
+}
+➜ cat cred.json | tab request-token | jq
+{
+    "access_token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJSUzUxMiJ9.eyJjcmVkc0tleSI6InQtR2RDWkdqNU9wb1EiLCJzdWJJZCI6ImViMzc2NTQ4LTIwNmItNDBiYS1hN2E1LWVkYmUzZjg4YWVlZCIsInN1YiI6ImZva2tvQHRhYnVsYXIuaW8iLCJ3YXJlaG91c2VJZCI6IjhiY2IwODM4LTUwZmMtNDcyZC05ZGRiLThmZWI4OWVmNWYxZSIsImlzcyI6InRhYnVsYXIuaW8iLCJsb2NhdGlvbiI6InMzOi8vdGFidWxhci13aC11cy13ZXN0LTItZGV2LzhiY2IwODM4LTUwZmMtNDcyZC05ZGRiLThmZWI4OWVmNWYxZS8iLCJ0eXBlIjoiV0FSRUhPVVNFIiwicmVnaW9uIjoidXMtd2VzdC0yIiwiZXhwIjoxNjY1NzU1Mjg2LCJpYXQiOjE2NjU2Njg4ODYsImp0aSI6IjZhNzljNzU1LTYzNGEtNDJlNC04YmVlLTEzZjgxOWFlYTYyNCIsIm9yZ0lkIjoiMWM1MmU4MzItMjY2Yy00OTYxLTk3YWYtMTE1ZDFiNzJmY2UwIn0.WZNP_e-cMKX9pj7ydPA_sm2Zyy54Iht1bOx7g3lr8p5NRh8jyyD2RHY1hAhvDgLASZr49vBcjAsbRdvmq3WEAO_LV3c_ts-5edDhLfetAfmcDjR5Xv70HDvpmofkEkZVK7HE8P_IPA6z2YX-CbnEcAHPzZ3hrjfR6nc2ouo0h8tlg6OqmT8w75aX5PA9inh6xquMhBLYSfeGlET5XF3fryQ6Kd2PfTTftMRqo-DbkdMHHF7t8E8wrbf-I7cE7--o_KfF2paaebyRAuS9n7RSdOw82FL2dBn9V3cMwyNeTPH05m6OKChnXenG9xorgKnRkEeB_P6UdwEPcPH8YeQJHA",
+    "issued_token_type": "urn:ietf:params:oauth:token-type:access_token",
+    "token_type": "Bearer",
+    "expires_in": 86400,
+    "scope": null
+}
+```
 
-package_data = \
-{'': ['*']}
+### Requesting a user access token
 
-install_requires = \
-['click>=8.1.3,<9.0.0', 'pyiceberg==0.3.0', 'requests>=2.28.1,<3.0.0']
-
-entry_points = \
-{'console_scripts': ['tab = tab.cli:run']}
-
-setup_kwargs = {
-    'name': 'tabulario',
-    'version': '0.3.0',
-    'description': 'Utility library for Tabular.io',
-    'long_description': '# Tab\n\nThis is a helper library to easily fetch and refresh access token from Tabular.\n\n## Usage\n\nEvery command has `--help` available:\n\n```bash\n➜ tab --help\nUsage: tab [OPTIONS] COMMAND [ARGS]...\n\nOptions:\n--environment TEXT\n--help              Show this message and exit.\n\nCommands:\nrefresh-token       Retrieves a fresh token based on an existing token\nrequest-token       Retrieves an access token based on credentials\nrequest-user-token  Retrieves a user token based on credentials\n```\n\nAnd the specific commands:\n\n```bash\n➜ tab request-user-token --help\nUsage: tab request-user-token [OPTIONS] [SERVICE_TOKEN] [SERVICE_TOKEN_TYPE]\n[ID_TOKEN] [ID_TOKEN_TYPE] [SCOPES]...\n\nRetrieves a user token based on credentials\n\nOptions:\n--help  Show this message and exit.\n```\n\n### Requesting access token\n\n```bash\n➜ tab request-token t-GdCZGj5OpoQ:jIcDDITVeIOnqxo7FxWbI21Y3kI | jq\n{\n    "access_token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJSUzUxMiJ9.eyJjcmVkc0tleSI6InQtR2RDWkdqNU9wb1EiLCJzdWJJZCI6ImViMzc2NTQ4LTIwNmItNDBiYS1hN2E1LWVkYmUzZjg4YWVlZCIsInN1YiI6ImZva2tvQHRhYnVsYXIuaW8iLCJ3YXJlaG91c2VJZCI6IjhiY2IwODM4LTUwZmMtNDcyZC05ZGRiLThmZWI4OWVmNWYxZSIsImlzcyI6InRhYnVsYXIuaW8iLCJsb2NhdGlvbiI6InMzOi8vdGFidWxhci13aC11cy13ZXN0LTItZGV2LzhiY2IwODM4LTUwZmMtNDcyZC05ZGRiLThmZWI4OWVmNWYxZS8iLCJ0eXBlIjoiV0FSRUhPVVNFIiwicmVnaW9uIjoidXMtd2VzdC0yIiwiZXhwIjoxNjY1NzU1MzU2LCJpYXQiOjE2NjU2Njg5NTYsImp0aSI6IjRhZjcyMzk3LTVlOGQtNDc0OS1iZThmLWI4OTFmYTMwNjNhNiIsIm9yZ0lkIjoiMWM1MmU4MzItMjY2Yy00OTYxLTk3YWYtMTE1ZDFiNzJmY2UwIn0.sTu-j2lGG02Ui_Ts7_rMfkT-zha6ugMzz0JyiumHpTupqEXnDdNiaxyEJmJcu81IcjEaWwT32hxAlznLy6Qhr-yTeSoVY5pJnTiXMNxeAZwzDkGh87uLcp0PjgwRLc6DmD3ZAXC2WQEUf8PS_mcMXF_6HoegHv1GHGLk9aHhWLze6WI_SIKSLc0Gmw8ZjjZoUpL8SSwt-uinT8gY_D0TksHkeVzM5DFxhLvhXMjJ1VyRUbsrE_6An83-aG0NzsFFgK3IhCf-RsEsOXH1MKZpdLdIlelcz8Av1uFzgWA6kFAcy9dGVZu_Ycj19e58e17IKHgLbtk4cc4wJOAg6lCBsw",\n    "issued_token_type": "urn:ietf:params:oauth:token-type:access_token",\n    "token_type": "Bearer",\n    "expires_in": 86400,\n    "scope": null,\n    "warehouse_id": "8bcb0838-50fc-472d-9ddb-8feb89ef5f1e",\n    "region": "us-west-2"\n}\n```\n\nAlso, stdin is supported:\n\n```bash\n➜ cat cred.json | jq\n{\n    "credential": "t-GdCZGj5OpoQ:jIcDDITVeIOnqxo7FxWbI21Y3kI"\n}\n➜ cat cred.json | tab request-token | jq\n{\n    "access_token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJSUzUxMiJ9.eyJjcmVkc0tleSI6InQtR2RDWkdqNU9wb1EiLCJzdWJJZCI6ImViMzc2NTQ4LTIwNmItNDBiYS1hN2E1LWVkYmUzZjg4YWVlZCIsInN1YiI6ImZva2tvQHRhYnVsYXIuaW8iLCJ3YXJlaG91c2VJZCI6IjhiY2IwODM4LTUwZmMtNDcyZC05ZGRiLThmZWI4OWVmNWYxZSIsImlzcyI6InRhYnVsYXIuaW8iLCJsb2NhdGlvbiI6InMzOi8vdGFidWxhci13aC11cy13ZXN0LTItZGV2LzhiY2IwODM4LTUwZmMtNDcyZC05ZGRiLThmZWI4OWVmNWYxZS8iLCJ0eXBlIjoiV0FSRUhPVVNFIiwicmVnaW9uIjoidXMtd2VzdC0yIiwiZXhwIjoxNjY1NzU1Mjg2LCJpYXQiOjE2NjU2Njg4ODYsImp0aSI6IjZhNzljNzU1LTYzNGEtNDJlNC04YmVlLTEzZjgxOWFlYTYyNCIsIm9yZ0lkIjoiMWM1MmU4MzItMjY2Yy00OTYxLTk3YWYtMTE1ZDFiNzJmY2UwIn0.WZNP_e-cMKX9pj7ydPA_sm2Zyy54Iht1bOx7g3lr8p5NRh8jyyD2RHY1hAhvDgLASZr49vBcjAsbRdvmq3WEAO_LV3c_ts-5edDhLfetAfmcDjR5Xv70HDvpmofkEkZVK7HE8P_IPA6z2YX-CbnEcAHPzZ3hrjfR6nc2ouo0h8tlg6OqmT8w75aX5PA9inh6xquMhBLYSfeGlET5XF3fryQ6Kd2PfTTftMRqo-DbkdMHHF7t8E8wrbf-I7cE7--o_KfF2paaebyRAuS9n7RSdOw82FL2dBn9V3cMwyNeTPH05m6OKChnXenG9xorgKnRkEeB_P6UdwEPcPH8YeQJHA",\n    "issued_token_type": "urn:ietf:params:oauth:token-type:access_token",\n    "token_type": "Bearer",\n    "expires_in": 86400,\n    "scope": null,\n    "warehouse_id": "8bcb0838-50fc-472d-9ddb-8feb89ef5f1e",\n    "region": "us-west-2"\n}\n```\n\n### Requesting a user access token\n\n```bash\ntab request-user-token eyJ0e...eQJHA urn:ietf:params:oauth:token-type:id_token eyJ0e...eQJHA urn:ietf:params:oauth:token-type:access_token | jq\n{\n    "access_token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJSUzUxMiJ9.eyJjcmVkc0tleSI6InQtR2RDWkdqNU9wb1EiLCJzdWJJZCI6ImViMzc2NTQ4LTIwNmItNDBiYS1hN2E1LWVkYmUzZjg4YWVlZCIsInN1YiI6ImZva2tvQHRhYnVsYXIuaW8iLCJ3YXJlaG91c2VJZCI6IjhiY2IwODM4LTUwZmMtNDcyZC05ZGRiLThmZWI4OWVmNWYxZSIsImlzcyI6InRhYnVsYXIuaW8iLCJsb2NhdGlvbiI6InMzOi8vdGFidWxhci13aC11cy13ZXN0LTItZGV2LzhiY2IwODM4LTUwZmMtNDcyZC05ZGRiLThmZWI4OWVmNWYxZS8iLCJ0eXBlIjoiV0FSRUhPVVNFIiwicmVnaW9uIjoidXMtd2VzdC0yIiwiZXhwIjoxNjY1NzU1Mjg2LCJpYXQiOjE2NjU2Njg4ODYsImp0aSI6IjZhNzljNzU1LTYzNGEtNDJlNC04YmVlLTEzZjgxOWFlYTYyNCIsIm9yZ0lkIjoiMWM1MmU4MzItMjY2Yy00OTYxLTk3YWYtMTE1ZDFiNzJmY2UwIn0.WZNP_e-cMKX9pj7ydPA_sm2Zyy54Iht1bOx7g3lr8p5NRh8jyyD2RHY1hAhvDgLASZr49vBcjAsbRdvmq3WEAO_LV3c_ts-5edDhLfetAfmcDjR5Xv70HDvpmofkEkZVK7HE8P_IPA6z2YX-CbnEcAHPzZ3hrjfR6nc2ouo0h8tlg6OqmT8w75aX5PA9inh6xquMhBLYSfeGlET5XF3fryQ6Kd2PfTTftMRqo-DbkdMHHF7t8E8wrbf-I7cE7--o_KfF2paaebyRAuS9n7RSdOw82FL2dBn9V3cMwyNeTPH05m6OKChnXenG9xorgKnRkEeB_P6UdwEPcPH8YeQJHA",\n    "issued_token_type": "urn:ietf:params:oauth:token-type:access_token",\n    "token_type": "Bearer",\n    "expires_in": 64982,\n    "scope": null\n}\n```\n\n### Refreshing an access token\n\n```bash\n➜ tab refresh-token eyJ0e...eQJHA urn:ietf:params:oauth:token-type:access_token | jq\n{\n    "access_token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJSUzUxMiJ9.eyJjcmVkc0tleSI6InQtR2RDWkdqNU9wb1EiLCJzdWJJZCI6ImViMzc2NTQ4LTIwNmItNDBiYS1hN2E1LWVkYmUzZjg4YWVlZCIsInN1YiI6ImZva2tvQHRhYnVsYXIuaW8iLCJ3YXJlaG91c2VJZCI6IjhiY2IwODM4LTUwZmMtNDcyZC05ZGRiLThmZWI4OWVmNWYxZSIsImlzcyI6InRhYnVsYXIuaW8iLCJsb2NhdGlvbiI6InMzOi8vdGFidWxhci13aC11cy13ZXN0LTItZGV2LzhiY2IwODM4LTUwZmMtNDcyZC05ZGRiLThmZWI4OWVmNWYxZS8iLCJ0eXBlIjoiV0FSRUhPVVNFIiwicmVnaW9uIjoidXMtd2VzdC0yIiwiZXhwIjoxNjY1NzU1NDM5LCJpYXQiOjE2NjU2NjkwMzksImp0aSI6IjZhNzljNzU1LTYzNGEtNDJlNC04YmVlLTEzZjgxOWFlYTYyNCIsIm9yZ0lkIjoiMWM1MmU4MzItMjY2Yy00OTYxLTk3YWYtMTE1ZDFiNzJmY2UwIn0.DBmmCfyj4hNaP0eVwzyv6R5aoSLrwWwHbHKePs2lEphA8zzilVreN1BPligIjezLPsn57S8FiOHqsCAwkeNWPthxxCI_gBkeZuCDhqbP90GsIuKwsFIaECZjn2_sO7UAhT3oSLgSeSB289QsQck6qIPPLLXM95jKrfzClKIF3Me4lKPmsRdLNRwCEDAOIgiR9sjBEUbSxgSkRvwxPQNDu75T25pn8O18EMlhmOUROSYva8VPRCc9PIFJL0PfcD_D7wlKZfiug8v58-q-1RAfB57IF0p-o9G_5RNeDrbEDA35OM8jTZEFDpL8Q-WlzT_6EZTvsIx_b7HxNW6kxf6WsQ",\n    "issued_token_type": "urn:ietf:params:oauth:token-type:access_token",\n    "token_type": "Bearer",\n    "expires_in": 86400,\n    "scope": null\n}\n```\n',
-    'author': 'Tabular Technologies, Inc.',
-    'author_email': 'fokko@tabular.io',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://tabular.io/',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<4.0',
+```bash
+tab request-user-token eyJ0e...eQJHA urn:ietf:params:oauth:token-type:id_token eyJ0e...eQJHA urn:ietf:params:oauth:token-type:access_token | jq
+{
+    "access_token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJSUzUxMiJ9.eyJjcmVkc0tleSI6InQtR2RDWkdqNU9wb1EiLCJzdWJJZCI6ImViMzc2NTQ4LTIwNmItNDBiYS1hN2E1LWVkYmUzZjg4YWVlZCIsInN1YiI6ImZva2tvQHRhYnVsYXIuaW8iLCJ3YXJlaG91c2VJZCI6IjhiY2IwODM4LTUwZmMtNDcyZC05ZGRiLThmZWI4OWVmNWYxZSIsImlzcyI6InRhYnVsYXIuaW8iLCJsb2NhdGlvbiI6InMzOi8vdGFidWxhci13aC11cy13ZXN0LTItZGV2LzhiY2IwODM4LTUwZmMtNDcyZC05ZGRiLThmZWI4OWVmNWYxZS8iLCJ0eXBlIjoiV0FSRUhPVVNFIiwicmVnaW9uIjoidXMtd2VzdC0yIiwiZXhwIjoxNjY1NzU1Mjg2LCJpYXQiOjE2NjU2Njg4ODYsImp0aSI6IjZhNzljNzU1LTYzNGEtNDJlNC04YmVlLTEzZjgxOWFlYTYyNCIsIm9yZ0lkIjoiMWM1MmU4MzItMjY2Yy00OTYxLTk3YWYtMTE1ZDFiNzJmY2UwIn0.WZNP_e-cMKX9pj7ydPA_sm2Zyy54Iht1bOx7g3lr8p5NRh8jyyD2RHY1hAhvDgLASZr49vBcjAsbRdvmq3WEAO_LV3c_ts-5edDhLfetAfmcDjR5Xv70HDvpmofkEkZVK7HE8P_IPA6z2YX-CbnEcAHPzZ3hrjfR6nc2ouo0h8tlg6OqmT8w75aX5PA9inh6xquMhBLYSfeGlET5XF3fryQ6Kd2PfTTftMRqo-DbkdMHHF7t8E8wrbf-I7cE7--o_KfF2paaebyRAuS9n7RSdOw82FL2dBn9V3cMwyNeTPH05m6OKChnXenG9xorgKnRkEeB_P6UdwEPcPH8YeQJHA",
+    "issued_token_type": "urn:ietf:params:oauth:token-type:access_token",
+    "token_type": "Bearer",
+    "expires_in": 64982,
+    "scope": null
 }
+```
+
+### Refreshing an access token
 
+```bash
+➜ tab refresh-token eyJ0e...eQJHA urn:ietf:params:oauth:token-type:access_token | jq
+{
+    "access_token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJSUzUxMiJ9.eyJjcmVkc0tleSI6InQtR2RDWkdqNU9wb1EiLCJzdWJJZCI6ImViMzc2NTQ4LTIwNmItNDBiYS1hN2E1LWVkYmUzZjg4YWVlZCIsInN1YiI6ImZva2tvQHRhYnVsYXIuaW8iLCJ3YXJlaG91c2VJZCI6IjhiY2IwODM4LTUwZmMtNDcyZC05ZGRiLThmZWI4OWVmNWYxZSIsImlzcyI6InRhYnVsYXIuaW8iLCJsb2NhdGlvbiI6InMzOi8vdGFidWxhci13aC11cy13ZXN0LTItZGV2LzhiY2IwODM4LTUwZmMtNDcyZC05ZGRiLThmZWI4OWVmNWYxZS8iLCJ0eXBlIjoiV0FSRUhPVVNFIiwicmVnaW9uIjoidXMtd2VzdC0yIiwiZXhwIjoxNjY1NzU1NDM5LCJpYXQiOjE2NjU2NjkwMzksImp0aSI6IjZhNzljNzU1LTYzNGEtNDJlNC04YmVlLTEzZjgxOWFlYTYyNCIsIm9yZ0lkIjoiMWM1MmU4MzItMjY2Yy00OTYxLTk3YWYtMTE1ZDFiNzJmY2UwIn0.DBmmCfyj4hNaP0eVwzyv6R5aoSLrwWwHbHKePs2lEphA8zzilVreN1BPligIjezLPsn57S8FiOHqsCAwkeNWPthxxCI_gBkeZuCDhqbP90GsIuKwsFIaECZjn2_sO7UAhT3oSLgSeSB289QsQck6qIPPLLXM95jKrfzClKIF3Me4lKPmsRdLNRwCEDAOIgiR9sjBEUbSxgSkRvwxPQNDu75T25pn8O18EMlhmOUROSYva8VPRCc9PIFJL0PfcD_D7wlKZfiug8v58-q-1RAfB57IF0p-o9G_5RNeDrbEDA35OM8jTZEFDpL8Q-WlzT_6EZTvsIx_b7HxNW6kxf6WsQ",
+    "issued_token_type": "urn:ietf:params:oauth:token-type:access_token",
+    "token_type": "Bearer",
+    "expires_in": 86400,
+    "scope": null
+}
+```
 
-setup(**setup_kwargs)
```

