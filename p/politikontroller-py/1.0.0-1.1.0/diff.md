# Comparing `tmp/politikontroller_py-1.0.0.tar.gz` & `tmp/politikontroller_py-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "politikontroller_py-1.0.0.tar", max compression
+gzip compressed data, was "politikontroller_py-1.1.0.tar", max compression
```

## Comparing `politikontroller_py-1.0.0.tar` & `politikontroller_py-1.1.0.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     1054 2023-06-11 22:31:59.445967 politikontroller_py-1.0.0/README.md
--rw-r--r--   0        0        0       78 2023-06-11 20:02:32.626027 politikontroller_py-1.0.0/politikontroller_py/__init__.py
--rw-r--r--   0        0        0     2382 2023-06-11 19:34:18.379760 politikontroller_py-1.0.0/politikontroller_py/cli.py
--rw-r--r--   0        0        0     5555 2023-06-11 22:32:54.334188 politikontroller_py-1.0.0/politikontroller_py/client.py
--rw-r--r--   0        0        0      354 2023-06-03 19:58:09.156460 politikontroller_py-1.0.0/politikontroller_py/constants.py
--rw-r--r--   0        0        0       96 2023-06-03 20:20:51.468283 politikontroller_py-1.0.0/politikontroller_py/exceptions.py
--rw-r--r--   0        0        0     3636 2023-06-11 22:40:49.348081 politikontroller_py-1.0.0/politikontroller_py/models.py
--rw-r--r--   0        0        0     4097 2023-06-11 22:33:50.490414 politikontroller_py-1.0.0/politikontroller_py/utils.py
--rw-r--r--   0        0        0      679 2023-06-11 21:44:58.442420 politikontroller_py-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1801 1970-01-01 00:00:00.000000 politikontroller_py-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-11 23:05:05.810836 politikontroller_py-1.1.0/LICENSE
+-rw-r--r--   0        0        0     1018 2023-06-13 00:09:17.352013 politikontroller_py-1.1.0/README.md
+-rw-r--r--   0        0        0       78 2023-06-11 23:05:05.814836 politikontroller_py-1.1.0/politikontroller_py/__init__.py
+-rw-r--r--   0        0        0     2382 2023-06-11 23:05:05.814836 politikontroller_py-1.1.0/politikontroller_py/cli.py
+-rw-r--r--   0        0        0     5265 2023-06-13 00:04:29.550179 politikontroller_py-1.1.0/politikontroller_py/client.py
+-rw-r--r--   0        0        0      441 2023-06-12 23:56:29.371118 politikontroller_py-1.1.0/politikontroller_py/constants.py
+-rw-r--r--   0        0        0       96 2023-06-11 23:05:05.810836 politikontroller_py-1.1.0/politikontroller_py/exceptions.py
+-rw-r--r--   0        0        0     3390 2023-06-13 00:07:44.003418 politikontroller_py-1.1.0/politikontroller_py/models.py
+-rw-r--r--   0        0        0     4097 2023-06-11 23:05:05.814836 politikontroller_py-1.1.0/politikontroller_py/utils.py
+-rw-r--r--   0        0        0      679 2023-06-13 00:11:32.376874 politikontroller_py-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1765 1970-01-01 00:00:00.000000 politikontroller_py-1.1.0/PKG-INFO
```

### Comparing `politikontroller_py-1.0.0/README.md` & `politikontroller_py-1.1.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -10,20 +10,17 @@
 
 ```python
 from politikontroller_py import Client
 from politikontroller_py.models import Account
 
 # A valid registered user @ politikontroller.no
 user = Account(
-    phone_number=90112233,
-    phone_prefix=47,
+    username="4790112233",  # Include 2 digit prefix - or else DEFAULT_COUNTRY is assumed
     password="super-secret",
 )
-# Alternative;
-user = Account(username="4790112233", password="super-secret")
 
 client = Client(user)
 
 police_controls = client.get_controls(63, 11)
 
 ```
```

### Comparing `politikontroller_py-1.0.0/politikontroller_py/cli.py` & `politikontroller_py-1.1.0/politikontroller_py/cli.py`

 * *Files identical despite different names*

### Comparing `politikontroller_py-1.0.0/politikontroller_py/client.py` & `politikontroller_py-1.1.0/politikontroller_py/client.py`

 * *Files 18% similar despite different names*

```diff
@@ -34,45 +34,37 @@
             raise NoAccessException()
         _LOGGER.debug("Got response: %s", data)
         return data
 
     def set_user(self, user: Account):
         self.user = user
 
-    def authenticate_user(self, phone_prefix: int, phone_number: int, password: str):
+    def authenticate_user(self, username: str, password: str):
+        auth_user = Account(**{"username": username, "password": password})
         params = {
             'p': 'l',
-            'telefon': phone_number,
-            'retning': phone_prefix,
-            'passord': password,
-            # 'token': generate_device_id(),
             'lang': 'no',
-        }
-        # 'LOGIN_OK|NO|0|47|SKIP_AUTHENTICATION|308452|0||NO_SAPHE|NO_REGNR|29|NO|NO|+47400008'
+        } | auth_user.get_query_params()
+
         result = self._api_request(params)
         _LOGGER.debug("Got result: %s", result)
         user_dict = map_response_data(result, [
             'status',
             'country',
             None,
             'phone_prefix',
             'state',
             'uid',
         ])
         if user_dict.get('status') == AuthStatus.LOGIN_ERROR:
             raise AuthenticationError
 
         account_dict = {
-            **user_dict,
-            **{
-                "username": phone_number,
-                "phone_number": phone_number,
-                "password": password,
-            },
-        }
+            **user_dict
+        } | auth_user.get_query_params()
         account = Account(**{str(k): str(v) for k, v in account_dict.items()})
         self.set_user(account)
         return account
 
     def get_settings(self):
         params = {
             'p': 'instillinger',
```

### Comparing `politikontroller_py-1.0.0/politikontroller_py/models.py` & `politikontroller_py-1.1.0/politikontroller_py/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import re
 from datetime import datetime
 from enum import Enum
 from pydantic import BaseModel, validator
 
 from .utils import parse_time_format
+from .constants import DEFAULT_COUNTRY, PHONE_PREFIXES
 
 
 class AuthStatus(str, Enum):
     LOGIN_OK = 'LOGIN_OK'
     LOGIN_ERROR = 'LOGIN_ERROR'
 
 
@@ -30,50 +31,40 @@
     MC_CONTROL = "Mopedkontroll"
     BOAT_PATROL = "Politibåten"
 
 
 class Account(BaseModel):
     uid: int | None
     status: AuthStatus | None
-    country: str = "no"
-    phone_prefix: int = 47
-    phone_number: int
+    country: str = DEFAULT_COUNTRY
+    username: str
     password: str | None
     state: str | None
 
     @property
-    def username(self):
-        return f"{self.phone_prefix}{self.phone_number}"
+    def phone_number(self):
+        return int(self.username[2:]) if len(self.username) > 8 else int(self.username)
 
-    def set_username(self, value):
-        clean_value = re.sub('\D', '', str(value))
-        if len(clean_value) < 8:
-            self.phone_number = int(clean_value)
-        else:
-            self.phone_prefix = int(clean_value[:2])
-            self.phone_number = int(clean_value[2:])
-
-    def __setattr__(self, key, val):
-        method = self.__config__.property_set_methods.get(key)
-        if method is None:
-            super().__setattr__(key, val)
-        else:
-            getattr(self, method)(val)
+    @property
+    def phone_prefix(self):
+        return int(self.username[:2]) if len(self.username) > 8 else PHONE_PREFIXES.get(self.country)
+
+    @validator('username', pre=True)
+    def validate_username(cls, v):
+        v = re.sub('\D', '', str(v))
+        return v
 
     def get_query_params(self):
         """ Get query params. """
         return {
             'retning': self.phone_prefix,
             'telefon': self.phone_number,
             'passord': self.password,
         }
 
-    class Config:
-        property_set_methods = {"username": "set_username"}
-
 
 class PoliceControlType(BaseModel):
     id: int
     name: PoliceControlTypeEnum
     slug: str
 
 
@@ -117,15 +108,15 @@
         if len(v) == 0 or (v.isnumeric() and int(v) == 0):
             return None
         return parse_time_format(v)
 
     @property
     def description_truncated(self):
         return (
-            self.description[:25] + '..'
+                self.description[:25] + '..'
         ) if len(self.description) > 27 else self.description
 
     @property
     def title(self):
         return f"{self.type.value}: {self.description_truncated}"
 
     @property
@@ -144,8 +135,7 @@
             },
         }
 
 
 class ExchangePointsResponse(BaseModel):
     status: ExchangeStatus
     message: str
-
```

### Comparing `politikontroller_py-1.0.0/politikontroller_py/utils.py` & `politikontroller_py-1.1.0/politikontroller_py/utils.py`

 * *Files identical despite different names*

### Comparing `politikontroller_py-1.0.0/pyproject.toml` & `politikontroller_py-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "politikontroller-py"
-version = "1.0.0"
+version = "1.1.0"
 description = "Unofficial client for politikontroller.no"
 authors = ["Bendik R. Brenne <bendik@konstant.no>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "politikontroller_py" },
 ]
```

### Comparing `politikontroller_py-1.0.0/PKG-INFO` & `politikontroller_py-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: politikontroller-py
-Version: 1.0.0
+Version: 1.1.0
 Summary: Unofficial client for politikontroller.no
 License: MIT
 Author: Bendik R. Brenne
 Author-email: bendik@konstant.no
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -31,20 +31,17 @@
 
 ```python
 from politikontroller_py import Client
 from politikontroller_py.models import Account
 
 # A valid registered user @ politikontroller.no
 user = Account(
-    phone_number=90112233,
-    phone_prefix=47,
+    username="4790112233",  # Include 2 digit prefix - or else DEFAULT_COUNTRY is assumed
     password="super-secret",
 )
-# Alternative;
-user = Account(username="4790112233", password="super-secret")
 
 client = Client(user)
 
 police_controls = client.get_controls(63, 11)
 
 ```
```

