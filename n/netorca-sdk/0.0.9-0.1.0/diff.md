# Comparing `tmp/netorca_sdk-0.0.9.tar.gz` & `tmp/netorca_sdk-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netorca_sdk-0.0.9.tar", last modified: Fri Feb 17 16:35:21 2023, max compression
+gzip compressed data, was "netorca_sdk-0.1.0.tar", last modified: Tue Jun 13 11:06:17 2023, max compression
```

## Comparing `netorca_sdk-0.0.9.tar` & `netorca_sdk-0.1.0.tar`

### file list

```diff
@@ -1,19 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-17 16:35:21.404152 netorca_sdk-0.0.9/
--rw-rw-rw-   0 root         (0) root         (0)     1067 2023-02-17 16:34:53.000000 netorca_sdk-0.0.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)      657 2023-02-17 16:35:21.404152 netorca_sdk-0.0.9/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      290 2023-02-17 16:34:53.000000 netorca_sdk-0.0.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-17 16:35:21.404152 netorca_sdk-0.0.9/netorca_sdk/
--rw-rw-rw-   0 root         (0) root         (0)     5468 2023-02-17 16:34:53.000000 netorca_sdk-0.0.9/netorca_sdk/auth.py
--rw-rw-rw-   0 root         (0) root         (0)      471 2023-02-17 16:34:53.000000 netorca_sdk-0.0.9/netorca_sdk/config.py
--rw-rw-rw-   0 root         (0) root         (0)     8978 2023-02-17 16:34:53.000000 netorca_sdk-0.0.9/netorca_sdk/consumer.py
--rw-rw-rw-   0 root         (0) root         (0)       43 2023-02-17 16:34:53.000000 netorca_sdk-0.0.9/netorca_sdk/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     9332 2023-02-17 16:34:53.000000 netorca_sdk-0.0.9/netorca_sdk/serviceowner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-17 16:35:21.404152 netorca_sdk-0.0.9/netorca_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)      657 2023-02-17 16:35:21.000000 netorca_sdk-0.0.9/netorca_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      335 2023-02-17 16:35:21.000000 netorca_sdk-0.0.9/netorca_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-17 16:35:21.000000 netorca_sdk-0.0.9/netorca_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-02-17 16:35:21.000000 netorca_sdk-0.0.9/netorca_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-02-17 16:35:21.000000 netorca_sdk-0.0.9/netorca_sdk.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      143 2023-02-17 16:34:53.000000 netorca_sdk-0.0.9/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-17 16:35:21.405153 netorca_sdk-0.0.9/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      852 2023-02-17 16:34:53.000000 netorca_sdk-0.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 11:06:17.227438 netorca_sdk-0.1.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1068 2023-06-13 11:06:03.000000 netorca_sdk-0.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      657 2023-06-13 11:06:17.227438 netorca_sdk-0.1.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      290 2023-06-13 11:06:03.000000 netorca_sdk-0.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 11:06:17.226438 netorca_sdk-0.1.0/netorca_sdk/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-13 11:06:03.000000 netorca_sdk-0.1.0/netorca_sdk/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5492 2023-06-13 11:06:03.000000 netorca_sdk-0.1.0/netorca_sdk/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)     1345 2023-06-13 11:06:03.000000 netorca_sdk-0.1.0/netorca_sdk/config.py
+-rw-rw-rw-   0 root         (0) root         (0)    10705 2023-06-13 11:06:03.000000 netorca_sdk-0.1.0/netorca_sdk/consumer.py
+-rw-rw-rw-   0 root         (0) root         (0)       43 2023-06-13 11:06:03.000000 netorca_sdk-0.1.0/netorca_sdk/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     8375 2023-06-13 11:06:03.000000 netorca_sdk-0.1.0/netorca_sdk/netorca.py
+-rw-rw-rw-   0 root         (0) root         (0)    10442 2023-06-13 11:06:03.000000 netorca_sdk-0.1.0/netorca_sdk/serviceowner.py
+-rw-rw-rw-   0 root         (0) root         (0)      156 2023-06-13 11:06:03.000000 netorca_sdk-0.1.0/netorca_sdk/validations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 11:06:17.226438 netorca_sdk-0.1.0/netorca_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      657 2023-06-13 11:06:17.000000 netorca_sdk-0.1.0/netorca_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      500 2023-06-13 11:06:17.000000 netorca_sdk-0.1.0/netorca_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 11:06:17.000000 netorca_sdk-0.1.0/netorca_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-06-13 11:06:17.000000 netorca_sdk-0.1.0/netorca_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-06-13 11:06:17.000000 netorca_sdk-0.1.0/netorca_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      144 2023-06-13 11:06:03.000000 netorca_sdk-0.1.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-13 11:06:17.227438 netorca_sdk-0.1.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      852 2023-06-13 11:06:03.000000 netorca_sdk-0.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 11:06:17.226438 netorca_sdk-0.1.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     3858 2023-06-13 11:06:03.000000 netorca_sdk-0.1.0/tests/test_auth.py
+-rw-rw-rw-   0 root         (0) root         (0)    10410 2023-06-13 11:06:03.000000 netorca_sdk-0.1.0/tests/test_consumer.py
+-rw-rw-rw-   0 root         (0) root         (0)    11854 2023-06-13 11:06:03.000000 netorca_sdk-0.1.0/tests/test_netorca.py
+-rw-rw-rw-   0 root         (0) root         (0)     7998 2023-06-13 11:06:03.000000 netorca_sdk-0.1.0/tests/test_serviceowner.py
```

### Comparing `netorca_sdk-0.0.9/LICENSE` & `netorca_sdk-0.1.0/LICENSE`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `netorca_sdk-0.0.9/PKG-INFO` & `netorca_sdk-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netorca_sdk
-Version: 0.0.9
+Version: 0.1.0
 Summary: A package for interacting with the NetOrca API
 Home-page: https://gitlab.com/netorca_public/netorca_sdk/
 Author: Scott Rowlandson
 Author-email: scott@netautomate.org
 License: MIT
 Keywords: netorca,orchestration,netautomate
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `netorca_sdk-0.0.9/netorca_sdk/auth.py` & `netorca_sdk-0.1.0/netorca_sdk/auth.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from abc import abstractmethod, ABC
+from abc import ABC, abstractmethod
 from time import sleep
 
-import urllib3
 import requests
+import urllib3
 
-from netorca_sdk.config import RETRY_TIMES, AUTH_ENDPOINT, TEAM_ENDPOINT
+from netorca_sdk.config import AUTH_ENDPOINT, RETRY_TIMES, TEAM_ENDPOINT
 from netorca_sdk.exceptions import NetorcaException
 
 urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
 
 class AbstractNetorcaAuth(ABC):
     @abstractmethod
@@ -34,122 +34,122 @@
 
 class NetorcaAuth(AbstractNetorcaAuth):
     def __init__(self, fqdn, username=None, password=None, api_key=None):
         self.username = username
         self.password = password
         self.api_key = api_key
         self.fqdn = fqdn
-        self.headers = {
-            'content-type': 'application/json'
-        }
+        self.headers = {"content-type": "application/json"}
 
         if self.username and self.password:
             self.token = self.get_auth_token()
-            self.headers['Authorization'] = f'Token {self.token}'
+            self.headers["Authorization"] = f"Token {self.token}"
         elif self.api_key:
-            self.headers['Authorization'] = f'Api-Key {self.api_key}'
+            self.headers["Authorization"] = f"Api-Key {self.api_key}"
         else:
-            raise NetorcaException(
-                f"Failed to authenticate. You must provide either (username and password) or API KEY")
+            raise NetorcaException("Failed to authenticate. You must provide either (username and password) or API KEY")
 
     def get(self, *args, **kwargs):
         url = kwargs.get("url")
         filters = kwargs.get("filters")
+        if filters:
+            url = f"{url}?{'&'.join([f'{k}={v}' for k, v in filters.items()])}"
         authentication_required = kwargs.get("authentication_required", False)
 
         if not url:
-            raise NetorcaException(f"URL not provided!")
+            raise NetorcaException("URL not provided!")
 
         for retry in range(RETRY_TIMES):
             if authentication_required:
-                response = requests.get(url=url, headers=self.headers, verify=False, params=filters)
+                response = requests.get(url=url, headers=self.headers, verify=False)
             else:
-                response = requests.get(url=url, verify=False, params=filters)
+                response = requests.get(url=url, verify=False)
             if 200 <= response.status_code < 500:
                 return response
             sleep(retry)
         raise NetorcaException(
-            f"Failed to send GET request. GET details: {args, kwargs}. Response details: {response.json()}")
+            f"Failed to send GET request. GET details: {args, kwargs}. Response details: {response.json()}"
+        )
 
     def post(self, *args, **kwargs):
         url = kwargs.get("url")
         data = kwargs.get("data")
         authentication_required = kwargs.get("authentication_required", False)
 
         if not url or not data:
-            raise NetorcaException(f"URL or data not provided!")
+            raise NetorcaException("URL or data not provided!")
 
         if authentication_required:
             response = requests.post(url=url, data=data, headers=self.headers, verify=False)
         else:
             response = requests.post(url=url, data=data, verify=False)
 
         if 200 <= response.status_code < 500:
             return response
         raise NetorcaException(
-            f"Failed to send POST request. POST details: {args, kwargs}. Response details: {response.json()}")
+            f"Failed to send POST request. POST details: {args, kwargs}. Response details: {response.json()}"
+        )
 
     def put(self, *args, **kwargs):
         url = kwargs.get("url")
         data = kwargs.get("data")
         authentication_required = kwargs.get("authentication_required", False)
 
         if not url or not data:
-            raise NetorcaException(f"URL or data not provided!")
+            raise NetorcaException("URL or data not provided!")
 
         if authentication_required:
             response = requests.put(url=url, data=data, headers=self.headers, verify=False)
         else:
             response = requests.put(url=url, data=data, verify=False)
         if 200 <= response.status_code < 500:
             return response
         raise NetorcaException(
-            f"Failed to send PUT request. PUT details: {args, kwargs}. Response details: {response.json()}")
+            f"Failed to send PUT request. PUT details: {args, kwargs}. Response details: {response.json()}"
+        )
 
     def patch(self, *args, **kwargs):
         url = kwargs.get("url")
         data = kwargs.get("data")
         authentication_required = kwargs.get("authentication_required", False)
 
         if not url or not data:
-            raise NetorcaException(f"URL or data not provided!")
+            raise NetorcaException("URL or data not provided!")
 
         if authentication_required:
             response = requests.patch(url=url, data=data, headers=self.headers, verify=False)
         else:
             response = requests.patch(url=url, data=data, verify=False)
         if 200 <= response.status_code < 500:
             return response
         raise NetorcaException(
-            f"Failed to send PATCH request. PATCH details: {args, kwargs}. Response details: {response.json()}")
+            f"Failed to send PATCH request. PATCH details: {args, kwargs}. Response details: {response.json()}"
+        )
 
     def delete(self, *args, **kwargs):
         NetorcaException("Not implemented.")
 
     def get_auth_token(self) -> str:
         AUTH_URL = f"{self.fqdn}{AUTH_ENDPOINT}"
 
-        data = {
-            "username": self.username,
-            "password": self.password
-        }
+        data = {"username": self.username, "password": self.password}
         response = self.post(url=AUTH_URL, data=data, verify=False)
         if response.status_code == 200:
-            return response.json()['token']
+            return response.json()["token"]
         raise NetorcaException(f"Authentication failed due to: {response.json()}")
 
     def refresh_auth_token(self):
         return self.get_auth_token()
 
     def get_teams_info(self) -> list:
-        """ Get team info for given user"""
+        """Get team info for given user"""
         TEAM_URL = f"{self.fqdn}{TEAM_ENDPOINT}"
         response = self.get(url=TEAM_URL, authentication_required=True)
         if response.status_code == 200:
-            return response.json()['results']
-        raise NetorcaException(f"Error fetching team info.")
+            return response.json()["results"]
+        raise NetorcaException("Error fetching team info.")
 
     def __str__(self):
         return f"Username: {self.username}, netorca instance: {self.fqdn}."
 
     def __repr__(self):
         return f"Username: {self.username}, netorca instance: {self.fqdn}."
```

### Comparing `netorca_sdk-0.0.9/netorca_sdk/consumer.py` & `netorca_sdk-0.1.0/netorca_sdk/consumer.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,169 +2,204 @@
 import os
 from typing import Tuple
 
 import yaml
 from beautifultable import BeautifulTable
 
 from netorca_sdk.auth import AbstractNetorcaAuth, NetorcaAuth
-from netorca_sdk.config import VALIDATE_CONSUMER_REQUEST_ENDPOINT, SUBMIT_CONSUMER_REQUEST_ENDPOINT
+from netorca_sdk.config import SUBMIT_CONSUMER_SUBMISSION_ENDPOINT, VALIDATE_CONSUMER_SUBMISSION_ENDPOINT
 from netorca_sdk.exceptions import NetorcaException
 
 
-class ConsumerRequest:
+class ConsumerSubmission:
     def __init__(self, netorca_api_key: str):
         self.netorca_api_key = netorca_api_key
 
         self.config = None
-        self.consumer_request = None
+        self.consumer_submission = None
         self.auth = None
 
-    def load_from_repository(self, repository_path: str) -> None:
+    def load_from_repository(
+        self, repository_path: str, netorca_directory: str = ".netorca", repository_config: dict = None
+    ) -> None:
         """
-            Check if valid and load request and config from consumer's repository.
-            Repository must contain `.netorca` directory and `config.yaml` file.
-            Note: Only one allowed extensions in `.netorca` directory is `*.yaml`
+        Check if valid and load request and config from consumer's repository.
 
-            Args:
-                repository_path: str    path to consumer repository
+        Note: Only one allowed extensions in netorca_directory directory is `*.yaml/*.yml`
 
-            Returns: None
+        Args:
+            repository_path: str    path to consumer repository
+
+        Returns: None
+        :param repository_path:     path to consumer repository
+        :param netorca_directory:   netorca directory name, defaults to ".netorca"
+        :param repository_config:      optional: you can specify config from dictionary instead of config.y(a)ml
         """
+
         repository_exists = os.path.isdir(repository_path)
         if not repository_exists:
-            raise NetorcaException(
-                f"`{repository_path}` directory does not exist.")
-        netorca_exists = os.path.isdir(f"{repository_path}/.netorca")
+            raise NetorcaException(f"`{repository_path}` directory does not exist.")
+
+        netorca_exists = os.path.isdir(f"{repository_path}/{netorca_directory}")
         if not netorca_exists:
-            raise NetorcaException("`.netorca` directory does not exist.")
+            raise NetorcaException(f"`{netorca_directory}` directory does not exist.")
 
-        dotnetorca_path = f"{repository_path}/.netorca"
+        dotnetorca_path = f"{repository_path}/{netorca_directory}"
+        if repository_config:
+            netorca_global = repository_config.get("netorca_global", {})
+            if not (netorca_global and netorca_global.get("base_url")):
+                raise NetorcaException("No `netorca_global.base_url` provided.")
+
+            # Check for empty base_url
+            base_url = netorca_global.get("base_url", "") or ""
+            base_url = base_url.strip()
+            if not base_url:
+                raise NetorcaException("`netorca_global.base_url` is empty.")
+
+            self.config = repository_config
+            self.auth = self.get_auth()
+        else:
+            # check and load config from file if it exists
+            config_path_yaml = f"{repository_path}/{netorca_directory}/config.yaml"
+            config_path_yml = f"{repository_path}/{netorca_directory}/config.yml"
+
+            if os.path.exists(config_path_yml):
+                config_path = config_path_yml
+            elif os.path.exists(config_path_yaml):
+                config_path = config_path_yaml
+            else:
+                raise NetorcaException("No config file in the repository.")
 
-        # check and load config
-        with open(f"{repository_path}/.netorca/config.yaml", "r") as stream:
-            try:
-                config = yaml.safe_load(stream)
-                netorca_global = config.get("netorca_global", {})
-                if not (netorca_global or netorca_global.get("base_url")):
-                    raise NetorcaException(
-                        "No `netorca_global.base_url` provided.")
+            with open(config_path, "r") as stream:
+                try:
+                    config = yaml.safe_load(stream)
+                    netorca_global = config.get("netorca_global", {})
+                    if not (netorca_global and netorca_global.get("base_url")):
+                        raise NetorcaException("No `netorca_global.base_url` provided.")
+
+                    # Check for empty base_url
+                    base_url = netorca_global.get("base_url", "") or ""
+                    base_url = base_url.strip()
 
-                self.config = config
-                self.auth = self.get_auth()
-            except yaml.YAMLError as exc:
-                raise NetorcaException(
-                    f"Error while parsing file: `config.yml`. Exception: {exc.problem}")
+                    if not base_url:
+                        raise NetorcaException("`netorca_global.base_url` is empty.")
+
+                    self.config = config
+                    self.auth = self.get_auth()
+                except yaml.YAMLError as exc:
+                    raise NetorcaException(f"Error while parsing file: `config.yaml`. Exception: {exc.problem}")
 
-        _tmp_consumer_request = {}
+        _tmp_consumer_submission = {}
         # check and load consumer request
         for filename in os.listdir(dotnetorca_path):
-            if filename == "config.yaml":
+            if filename == "config.yaml" or filename == "config.yml":
                 continue
 
             f = os.path.join(dotnetorca_path, filename)
-            # checking if it is a file and is `*.yaml`
-            if not (os.path.isfile(f) and f.endswith('.yaml')):
-                raise NetorcaException(
-                    f"Consumer request files must have `.yaml` extension")
+            # checking if it is a file and is `*.yaml/*.yml`
+            if not (os.path.isfile(f) and (f.endswith(".yaml") or f.endswith(".yml"))):
+                continue
 
             with open(f, "r") as stream:
                 try:
                     app = yaml.safe_load(stream)
                 except yaml.YAMLError as exc:
-                    raise NetorcaException(
-                        f"Error while parsing file: `{filename}`. Exception: {exc.problem}")
+                    raise NetorcaException(f"Error while parsing file: `{filename}`. Exception: {exc.problem}")
+
+            if not isinstance(app, dict) or not app:
+                raise NetorcaException(
+                    f"Invalid format in file: `{filename}`. The file should contain a dictionary with at least one key-value pair."
+                )
 
-                for key in app.keys():
-                    if key in _tmp_consumer_request:
-                        raise NetorcaException(
-                            f"Application with name `{key}` already exists in different `.yaml` declaration.")
+            for key in app.keys():
+                if key in _tmp_consumer_submission:
+                    raise NetorcaException(
+                        f"Application with name `{key}` already exists in different yaml declaration."
+                    )
 
-                _tmp_consumer_request.update(app)
-        self.consumer_request = _tmp_consumer_request
+                _tmp_consumer_submission.update(app)
+        self.consumer_submission = _tmp_consumer_submission
 
     def get_auth(self) -> AbstractNetorcaAuth:
         if not self.config:
-            raise NetorcaException(f"Cannot authenticate before loading repository config.")
+            raise NetorcaException("Cannot authenticate before loading repository config.")
 
         netorca_fqdn = self.config.get("netorca_global", {}).get("base_url")
         self.auth = NetorcaAuth(fqdn=netorca_fqdn, api_key=self.netorca_api_key)
         return self.auth
 
     def get_team(self) -> dict:
         teams = self.auth.get_teams_info()
         if teams:
             return teams[0]
         return {}
 
     def prepare_request(self) -> dict:
         team = self.get_team()
         metadata = self.config.get("netorca_global", {}).get("metadata", {})
+        if not (team and self.config and self.consumer_submission and self.auth):
+            raise NetorcaException("Team, config and consumer request should be fetched at this stage.")
+
+        full_request = {team["name"]: self.consumer_submission}
+
+        if metadata is not None:
+            full_request[team["name"]]["metadata"] = metadata
 
-        if not (team and self.config and self.consumer_request and self.auth):
-            raise NetorcaException(
-                "Team, config and consumer request should be fetched at this stage.")
-
-        full_request = {
-            team['name']: {
-                "metadata": metadata,
-                **self.consumer_request
-            }
-        }
         return full_request
 
     def validate(self, pretty_print=False) -> Tuple[bool, dict]:
         """
-            Validate consume request.
-            NOTE: Data must be first imported with `load_from_repository` method
+        Validate consume request.
+        NOTE: Data must be first imported with `load_from_repository` method
 
-            Returns:
-                Tuple[bool, str]    ->  is_valid, validation_errors
+        Returns:
+            Tuple[bool, str]    ->  is_valid, validation_errors
         """
-        if not (self.config and self.consumer_request and self.auth):
-            raise NetorcaException(f"Use `load_from_repository(repository_path)` method to load configuration.")
-        VALIDATE_REQUEST_PATH = f"{self.auth.fqdn}{VALIDATE_CONSUMER_REQUEST_ENDPOINT}"
+        if not (self.config and self.auth):
+            raise NetorcaException("Use `load_from_repository(repository_path)` method to load configuration.")
+        VALIDATE_REQUEST_PATH = f"{self.auth.fqdn}{VALIDATE_CONSUMER_SUBMISSION_ENDPOINT}"
         full_request = self.prepare_request()
 
-        response = self.auth.post(url=VALIDATE_REQUEST_PATH, data=json.dumps(full_request),
-                                  authentication_required=True)
+        response = self.auth.post(
+            url=VALIDATE_REQUEST_PATH, data=json.dumps(full_request), authentication_required=True
+        )
 
         response = response.json()
         if response.get("is_valid"):
             return True, {}
         errors = response.get("errors")
 
         if pretty_print:
-            ConsumerRequest.pretty_print_errors(errors)
+            ConsumerSubmission.pretty_print_errors(errors)
         return False, errors
 
     def submit(self) -> Tuple[bool, str]:
         """
-            Validate and submit consumer request.
-            NOTE: Data must be first imported with `load_from_repository` method
+        Validate and submit consumer request.
+        NOTE: Data must be first imported with `load_from_repository` method
 
-            Returns:
-                bool, str    ->  submission successful, submission messages
+        Returns:
+            bool, str    ->  submission successful, submission messages
         """
         is_valid = self.validate(pretty_print=True)
         if not is_valid[0]:
             return False, "Consumer request is invalid and cannot be submitted."
 
-        SUBMIT_REQUEST_PATH = f"{self.auth.fqdn}{SUBMIT_CONSUMER_REQUEST_ENDPOINT}"
+        SUBMIT_REQUEST_PATH = f"{self.auth.fqdn}{SUBMIT_CONSUMER_SUBMISSION_ENDPOINT}"
         full_request = self.prepare_request()
-        response = self.auth.post(url=SUBMIT_REQUEST_PATH, data=json.dumps(full_request),
-                                  authentication_required=True)
+        response = self.auth.post(url=SUBMIT_REQUEST_PATH, data=json.dumps(full_request), authentication_required=True)
         if response.status_code == 201:
             return True, "Submitted successfuly."
         return False, response.text
 
     @staticmethod
     def pretty_print_errors(errors: dict) -> None:
         """
-            Pretty print errors
-            #TODO: this should be refactored to cleaner code (probably recursive)
+        Pretty print errors
+        #TODO: this should be refactored to cleaner code (probably recursive)
         """
 
         table = BeautifulTable(maxwidth=100)
         table.set_style(BeautifulTable.STYLE_SEPARATED)
         table.columns.header = ["Team", "Field", "Reason"]
         for item1, value1 in errors.items():
             if isinstance(value1, str) or isinstance(value1, list):
@@ -195,19 +230,19 @@
                                 table.rows.append([item2, "", "", item3, value3])
                             elif isinstance(value3, list):
                                 for err in value3:
                                     table.rows.append([item2, "", "", item3, err])
                             elif isinstance(value3, dict):
                                 for item4, value4 in value3.items():
                                     if isinstance(value4, str) or isinstance(value4, list):
-                                        table.rows.append(["", item3, "", item4, value4])
+                                        table.rows.append([item2, item3, "", item4, value4])
                                     elif isinstance(value4, dict):
                                         for item5, value5 in value4.items():
                                             if isinstance(value5, str) or isinstance(value5, list):
-                                                table.rows.append(["", item3, item4, item5, value5])
+                                                table.rows.append([item2, item3, item4, item5, value5])
 
                         if table.rows:
                             print("-" * 100)
                             print(f"Application: `{item2}` validation errors")
                             print("-" * 100)
                             print(table)
                             print()
```

### Comparing `netorca_sdk-0.0.9/netorca_sdk/serviceowner.py` & `netorca_sdk-0.1.0/netorca_sdk/serviceowner.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,203 +4,230 @@
 from string import Template
 from typing import Tuple
 
 import requests
 from beautifultable import BeautifulTable
 
 from netorca_sdk.auth import AbstractNetorcaAuth, NetorcaAuth
-from netorca_sdk.config import VALIDATE_SERVICEOWNER_REQUEST_ENDPOINT, SUBMIT_SERVICEOWNER_REQUEST_ENDPOINT, \
-    SUBMIT_SERVICEOWNER_REQUEST_DOCS_ENDPOINT
+from netorca_sdk.config import (
+    SUBMIT_SERVICEOWNER_SUBMISSION_DOCS_ENDPOINT,
+    SUBMIT_SERVICEOWNER_SUBMISSION_ENDPOINT,
+    VALIDATE_SERVICEOWNER_SUBMISSION_ENDPOINT,
+)
 from netorca_sdk.exceptions import NetorcaException
 
 
-class ServiceOwnerRequest:
+class ServiceOwnerSubmission:
     def __init__(self, netorca_api_key: str):
         self.netorca_api_key = netorca_api_key
 
         self.config = None
-        self.serviceowner_request = None
+        self.serviceowner_submission = None
         self.auth = None
 
-    def load_from_repository(self, repository_path: str) -> None:
+    def load_from_repository(
+        self, repository_path: str, netorca_directory: str = ".netorca", repository_config: dict = None
+    ) -> None:
+        """
+        Check if valid and load submission and config from service owner's repository.
+        Repository must contain `.netorca` directory and `config.json` file.
+        Note: Two allowed extensions in `.netorca` directory are: `*.yaml` and `*.md`.
+
+        Args:
+            repository_path: str    path to service owner repository
+
+        Returns: None
+        :param repository_path:     path to service owner repository
+        :param netorca_directory:   netorca directory name, defaults to ".netorca"
+        :param repository_config:      optional: you can specify config from dictionary instead of config.json
         """
-            Check if valid and load request and config from service owner's repository.
-            Repository must contain `.netorca` directory and `config.json` file.
-            Note: Two allowed extensions in `.netorca` directory are: `*.yaml` and `*.md`.
 
-            Args:
-                repository_path: str    path to service owner repository
-
-            Returns: None
-        """
         repository_exists = os.path.isdir(repository_path)
         if not repository_exists:
-            raise NetorcaException(
-                f"`{repository_path}` directory does not exist.")
-        netorca_exists = os.path.isdir(f"{repository_path}/.netorca")
-        if not netorca_exists:
-            raise NetorcaException("`.netorca` directory does not exist.")
+            raise NetorcaException(f"`{repository_path}` directory does not exist.")
 
-        dotnetorca_path = f"{repository_path}/.netorca"
+        netorca_path = os.path.join(repository_path, netorca_directory)
+        netorca_exists = os.path.isdir(netorca_path)
+        if not netorca_exists:
+            raise NetorcaException(f"`{netorca_directory}` directory does not exist.")
 
-        # check and load config
-        with open(f"{repository_path}/.netorca/config.json", "r") as stream:
-            try:
-                config = json.load(stream)
-                netorca_global = config.get("netorca_global", {})
-                if not (netorca_global or netorca_global.get("base_url")):
-                    raise NetorcaException(
-                        "No `netorca_global.base_url` provided.")
-
-                self.config = config
-                self.auth = self.get_auth()
-            except json.JSONDecodeError as exc:
-                raise NetorcaException(
-                    f"Error while parsing file: `config.json`. Exception: {exc.msg}")
+        if repository_config:
+            netorca_global = repository_config.get("netorca_global", {})
+            if not (netorca_global and netorca_global.get("base_url")):
+                raise NetorcaException("No `netorca_global.base_url` provided.")
+            self.config = repository_config
+            self.auth = self.get_auth()
+        else:
+            config_path = os.path.join(netorca_path, "config.json")
+            self.config = self.read_json_file(config_path)
+            netorca_global = self.config.get("netorca_global", {})
+            if not (netorca_global and netorca_global.get("base_url")):
+                raise NetorcaException("No `netorca_global.base_url` provided.")
+            self.auth = self.get_auth()
 
-        _tmp_serviceowner_request = defaultdict()
-        # check and load service owner request
-        for filename in os.listdir(dotnetorca_path):
+        _tmp_serviceowner_submission = defaultdict()
+        for filename in os.listdir(netorca_path):
             if filename == "config.json":
                 continue
 
-            f = os.path.join(dotnetorca_path, filename)
-            # checking if it is a file and is `*.json` or `*.md` file
-            if not os.path.isfile(f) and not (f.endswith('.json') or f.endswith('.md')):
+            file_path = os.path.join(netorca_path, filename)
+            if not os.path.isfile(file_path) and not (file_path.endswith(".json") or file_path.endswith(".md")):
                 raise NetorcaException(
-                    f"Consumer request file: `{f}` does not exist or must be `.json` or `.md` extension")
+                    f"ServiceOwner submission file: `{file_path}` does not exist or must be `.json` or `.md` extension"
+                )
 
-            with open(f, "r") as stream:
-                try:
-                    filename_without_ext = os.path.splitext(filename)[0]
-
-                    if filename.endswith('.json'):
-                        json_file = json.load(stream)
-                        _tmp_serviceowner_request.setdefault(filename_without_ext, {})
-                        _tmp_serviceowner_request[filename_without_ext]["service"] = json_file
-
-                    elif filename.endswith('.md'):
-                        _tmp_serviceowner_request.setdefault(filename_without_ext, {})
-                        _tmp_serviceowner_request[filename_without_ext]["readme"] = f
-                    else:
-                        raise ValueError(f"Error parsing file: {filename}.")
-                except json.JSONDecodeError as exc:
-                    raise NetorcaException(
-                        f"Error while parsing file: `{filename}`. Exception: {exc}")
+            if filename.endswith(".json"):
+                json_file = self.read_json_file(file_path)
+                filename_without_ext = os.path.splitext(filename)[0]
+                _tmp_serviceowner_submission.setdefault(filename_without_ext, {})
+                _tmp_serviceowner_submission[filename_without_ext]["service"] = json_file
+
+        for filename in os.listdir(netorca_path):
+            if filename == "config.json" or not filename.endswith(".md"):
+                continue
 
-        self.serviceowner_request = _tmp_serviceowner_request
+            file_path = os.path.join(netorca_path, filename)
+            filename_without_ext = os.path.splitext(filename)[0]
+
+            if not _tmp_serviceowner_submission.get(filename_without_ext):
+                raise NetorcaException(
+                    f"'\nYou are trying to add README file: `{filename}` for non existing service.\n"
+                    f"Readme file (.md) must have the same name as service definition file (.json)."
+                )
+
+            _tmp_serviceowner_submission[filename_without_ext]["readme"] = file_path
+
+        self.serviceowner_submission = _tmp_serviceowner_submission
+
+    def read_json_file(self, file_path: str):
+        try:
+            with open(file_path, "r") as stream:
+                return json.load(stream)
+        except FileNotFoundError as exc:
+            raise NetorcaException(f"File not found: `{file_path}`. Exception: {exc}")
+        except PermissionError as exc:
+            raise NetorcaException(f"Permission error while reading file: `{file_path}`. Exception: {exc}")
+        except json.JSONDecodeError as exc:
+            raise NetorcaException(f"Error while parsing file: `{file_path}`. Exception: {exc.msg}")
 
     def get_auth(self) -> AbstractNetorcaAuth:
         if not self.config:
-            raise NetorcaException(f"Cannot authenticate before loading repository config.")
+            raise NetorcaException("Cannot authenticate before loading repository config.")
 
         netorca_fqdn = self.config.get("netorca_global", {}).get("base_url")
         self.auth = NetorcaAuth(fqdn=netorca_fqdn, api_key=self.netorca_api_key)
         return self.auth
 
     def get_team(self) -> dict:
         teams = self.auth.get_teams_info()
         if teams:
             return teams[0]
         return {}
 
     def validate(self, pretty_print=False) -> Tuple[bool, str]:
         """
-            Validate service owner request.
-            NOTE: Data must be first imported with `load_from_repository` method
+        Validate service owner submission.
+        NOTE: Data must be first imported with `load_from_repository` method
 
-            Returns:
-                bool    ->  validation successful
+        Returns:
+            bool    ->  validation successful
         """
-        VALIDATE_SERVICEOWNER_PATH = f"{self.auth.fqdn}{VALIDATE_SERVICEOWNER_REQUEST_ENDPOINT}"
+        if self.auth is None:
+            raise NetorcaException("Use `load_from_repository(repository_path)` method to load configuration.")
+        VALIDATE_SERVICEOWNER_PATH = f"{self.auth.fqdn}{VALIDATE_SERVICEOWNER_SUBMISSION_ENDPOINT}"
         invalid_services = []
 
-        if not (self.config and self.serviceowner_request and self.auth):
-            raise NetorcaException(f"Use `load_from_repository(repository_path)` method to load configuration.")
+        if not (self.config and self.serviceowner_submission and self.auth):
+            raise NetorcaException("Use `load_from_repository(repository_path)` method to load configuration.")
 
-        for service, service_request in self.serviceowner_request.items():
-            response = self.auth.post(url=VALIDATE_SERVICEOWNER_PATH,
-                                      data=json.dumps(service_request['service']),
-                                      authentication_required=True)
+        for service, service_submission in self.serviceowner_submission.items():
+            response = self.auth.post(
+                url=VALIDATE_SERVICEOWNER_PATH,
+                data=json.dumps(service_submission["service"]),
+                authentication_required=True,
+            )
             response = response.json()
             if response.get("is_valid"):
                 print(f"VALIDATION SUCCESSFUL for service: `{service}`.")
             else:
                 invalid_services.append(service)
                 errors = response.get("errors")
                 if pretty_print and errors:
-                    ServiceOwnerRequest.pretty_print_errors(service, errors)
+                    ServiceOwnerSubmission.pretty_print_errors(service, errors)
 
         if invalid_services:
             print("INVALID SERVICES: " + ", ".join(invalid_services))
             return False, "Invalid services: " + ", ".join(invalid_services)
         return True, "Services validated successfully."
 
     def submit(self) -> Tuple[bool, str]:
         """
-            Validate and submit consumer request.
-            NOTE: Data must be first imported with `load_from_repository` method
+        Validate and submit consumer submission.
+        NOTE: Data must be first imported with `load_from_repository` method
 
-            Returns:
-                bool, str    ->  is submission successful, submission messages
+        Returns:
+            bool, str    ->  is submission successful, submission messages
         """
-        SUBMIT_SERVICEOWNER_REQUEST_PATH = f"{self.auth.fqdn}{SUBMIT_SERVICEOWNER_REQUEST_ENDPOINT}"
+        SUBMIT_SERVICEOWNER_REQUEST_PATH = f"{self.auth.fqdn}{SUBMIT_SERVICEOWNER_SUBMISSION_ENDPOINT}"
         submitted_services = []
         is_valid = self.validate(pretty_print=True)
 
         if not is_valid[0]:
-            return False, "Some of your requests are invalid and were not submitted."
+            return False, "Some of your submissions are invalid and were not submitted."
 
         print()
-        for service, service_request in self.serviceowner_request.items():
-            response = self.auth.post(url=SUBMIT_SERVICEOWNER_REQUEST_PATH,
-                                      data=json.dumps(service_request['service']),
-                                      authentication_required=True)
+        for service, service_submission in self.serviceowner_submission.items():
+            response = self.auth.post(
+                url=SUBMIT_SERVICEOWNER_REQUEST_PATH,
+                data=json.dumps(service_submission["service"]),
+                authentication_required=True,
+            )
 
             if response.status_code == 201:
                 print(f"SUBMITTED service to NetOrca. Service: `{service}` is now available for consumers.")
-                if service_request.get("readme"):
-                    service_uuid = response.json()['uuid']
-                    docs_path = Template(SUBMIT_SERVICEOWNER_REQUEST_DOCS_ENDPOINT).substitute(uuid=service_uuid)
+                submitted_services.append(service)
+                if service_submission.get("readme"):
+                    service_uuid = response.json()["uuid"]
+                    docs_path = Template(SUBMIT_SERVICEOWNER_SUBMISSION_DOCS_ENDPOINT).substitute(uuid=service_uuid)
                     SUBMIT_SERVICEOWNER_DOCS_PATH = f"{self.auth.fqdn}{docs_path}"
-                    files = {'md_file': ('VM.md', open(service_request.get("readme"), 'rb'))}
-                    auth = self.auth.headers['Authorization']
-                    response = requests.post(SUBMIT_SERVICEOWNER_DOCS_PATH,
-                                             files=files,
-                                             headers={'Authorization': auth})
+                    files = {"md_file": ("VM.md", open(service_submission.get("readme"), "rb"))}
+                    auth = self.auth.headers["Authorization"]
+                    response = requests.post(
+                        SUBMIT_SERVICEOWNER_DOCS_PATH, files=files, headers={"Authorization": auth}, verify=False
+                    )
                     if response.status_code == 200:
                         print(f"SUBMITTED README file for service: `{service}`.")
                     else:
                         print(f"FAILED to submit README file for service: `{service}`. Reason: `{response.json()}.`")
                 else:
-                    print(f"NOTE. Service `{service}` does not have README file.")
+                    print(f"NOTE: Service `{service}` does not have a README file. Skipped.")
             else:
                 print(f"FAILED to submit service: `{service}`. Reason: {response.json()}")
                 print("\nMoving to next service...")
             print()
 
         if submitted_services:
             return True, "Submitted services: " + ", ".join(submitted_services)
         return False, "No services were submitted."
 
     @staticmethod
     def pretty_print_errors(service_name: str, errors: dict) -> None:
-        """
-            Pretty print errors
-            #TODO: this should be refactored to cleaner code (probably recursive)
-        """
+        def append_to_table(service_name: str, item: str, value: str, table: BeautifulTable) -> None:
+            if isinstance(value, str) or isinstance(value, list):
+                table.rows.append([service_name, item, value])
+            elif isinstance(value, dict):
+                for key, val in value.items():
+                    append_to_table(service_name, key, val, table)
+
         table = BeautifulTable(maxwidth=100)
         table.set_style(BeautifulTable.STYLE_SEPARATED)
         table.columns.header = ["Schema", "Property", "Reason"]
-        for item1, value1 in errors.items():
-            if isinstance(value1, str) or isinstance(value1, list):
-                table.rows.append([service_name, "general", value1])
-            elif isinstance(value1, dict):
-                for item2, value2 in value1.items():
-                    if isinstance(value2, str) or isinstance(value2, list):
-                        table.rows.append([service_name, item2, value2])
-            if table.rows:
-                print("-" * 100)
-                print(f"Schema: `{service_name}` validation errors")
-                print("-" * 100)
-                print(table)
-                print()
+
+        for item, value in errors.items():
+            append_to_table(service_name, item, value, table)
+
+        if table.rows:
+            print("-" * 100)
+            print(f"Schema: `{service_name}` validation errors")
+            print("-" * 100)
+            print(table)
+            print()
```

### Comparing `netorca_sdk-0.0.9/netorca_sdk.egg-info/PKG-INFO` & `netorca_sdk-0.1.0/netorca_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netorca-sdk
-Version: 0.0.9
+Version: 0.1.0
 Summary: A package for interacting with the NetOrca API
 Home-page: https://gitlab.com/netorca_public/netorca_sdk/
 Author: Scott Rowlandson
 Author-email: scott@netautomate.org
 License: MIT
 Keywords: netorca,orchestration,netautomate
 Classifier: Development Status :: 3 - Alpha
```

