# Comparing `tmp/uid2_client-2.0.0.tar.gz` & `tmp/uid2_client-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uid2_client-2.0.0.tar", last modified: Tue Apr 18 15:18:52 2023, max compression
+gzip compressed data, was "uid2_client-2.0.2.tar", last modified: Tue Jun 13 03:30:31 2023, max compression
```

## Comparing `uid2_client-2.0.0.tar` & `uid2_client-2.0.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:18:52.002849 uid2_client-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-04-18 15:18:44.000000 uid2_client-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-04-18 15:18:52.002849 uid2_client-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-04-18 15:18:44.000000 uid2_client-2.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-18 15:18:44.000000 uid2_client-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-18 15:18:52.002849 uid2_client-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-18 15:18:44.000000 uid2_client-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:18:52.002849 uid2_client-2.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    27874 2023-04-18 15:18:44.000000 uid2_client-2.0.0/tests/test_encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-04-18 15:18:44.000000 uid2_client-2.0.0/tests/test_key_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-04-18 15:18:44.000000 uid2_client-2.0.0/tests/test_keys.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:18:52.002849 uid2_client-2.0.0/uid2_client/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-18 15:18:44.000000 uid2_client-2.0.0/uid2_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-18 15:18:44.000000 uid2_client-2.0.0/uid2_client/advertising_token_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-04-18 15:18:44.000000 uid2_client-2.0.0/uid2_client/auto_refresh.py
--rw-r--r--   0 runner    (1001) docker     (123)     4572 2023-04-18 15:18:44.000000 uid2_client-2.0.0/uid2_client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    17626 2023-04-18 15:18:44.000000 uid2_client-2.0.0/uid2_client/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-18 15:18:44.000000 uid2_client-2.0.0/uid2_client/identity_scope.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-18 15:18:44.000000 uid2_client-2.0.0/uid2_client/identity_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-04-18 15:18:44.000000 uid2_client-2.0.0/uid2_client/keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-04-18 15:18:44.000000 uid2_client-2.0.0/uid2_client/uid2_base64_url_coder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:18:52.002849 uid2_client-2.0.0/uid2_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-04-18 15:18:51.000000 uid2_client-2.0.0/uid2_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-18 15:18:51.000000 uid2_client-2.0.0/uid2_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 15:18:51.000000 uid2_client-2.0.0/uid2_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-18 15:18:51.000000 uid2_client-2.0.0/uid2_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-18 15:18:51.000000 uid2_client-2.0.0/uid2_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 15:18:51.000000 uid2_client-2.0.0/uid2_client.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:30:31.488512 uid2_client-2.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-06-13 03:30:22.000000 uid2_client-2.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-06-13 03:30:31.488512 uid2_client-2.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-06-13 03:30:22.000000 uid2_client-2.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-13 03:30:22.000000 uid2_client-2.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-13 03:30:31.492512 uid2_client-2.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-13 03:30:22.000000 uid2_client-2.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:30:31.488512 uid2_client-2.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    29028 2023-06-13 03:30:22.000000 uid2_client-2.0.2/tests/test_encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-06-13 03:30:22.000000 uid2_client-2.0.2/tests/test_key_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-06-13 03:30:22.000000 uid2_client-2.0.2/tests/test_keys.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:30:31.488512 uid2_client-2.0.2/uid2_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-13 03:30:22.000000 uid2_client-2.0.2/uid2_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-13 03:30:22.000000 uid2_client-2.0.2/uid2_client/advertising_token_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-06-13 03:30:22.000000 uid2_client-2.0.2/uid2_client/auto_refresh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4572 2023-06-13 03:30:22.000000 uid2_client-2.0.2/uid2_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17626 2023-06-13 03:30:22.000000 uid2_client-2.0.2/uid2_client/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-13 03:30:22.000000 uid2_client-2.0.2/uid2_client/identity_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-13 03:30:22.000000 uid2_client-2.0.2/uid2_client/identity_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-06-13 03:30:22.000000 uid2_client-2.0.2/uid2_client/keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-13 03:30:22.000000 uid2_client-2.0.2/uid2_client/uid2_base64_url_coder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:30:31.488512 uid2_client-2.0.2/uid2_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-06-13 03:30:31.000000 uid2_client-2.0.2/uid2_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-13 03:30:31.000000 uid2_client-2.0.2/uid2_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 03:30:31.000000 uid2_client-2.0.2/uid2_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-13 03:30:31.000000 uid2_client-2.0.2/uid2_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-13 03:30:31.000000 uid2_client-2.0.2/uid2_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 03:30:31.000000 uid2_client-2.0.2/uid2_client.egg-info/zip-safe
```

### Comparing `uid2_client-2.0.0/LICENSE` & `uid2_client-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `uid2_client-2.0.0/PKG-INFO` & `uid2_client-2.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,54 +1,58 @@
 Metadata-Version: 2.1
 Name: uid2_client
-Version: 2.0.0
-Summary: UID2 sdk for the UID2 and EUID apis
+Version: 2.0.2
+Summary: UID2 SDK for Python
 Home-page: https://iabtechlab.com
 Author: UID2 team
-Author-email: Cody Constine <cody.constine@thetradedesk.com>
+Author-email: UID2 team <unifiedid-admin@thetradedesk.com>
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/IABTechLab/uid2-client-python
 Project-URL: Bug Tracker, https://github.com/IABTechLab/uid2-client-python/issues
 Keywords: uid2
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Uid2 Client Python
+# UID2 SDK for Python
 
-The UID 2 Project is subject to Tech Lab IPR’s Policy and is managed by the IAB Tech Lab Addressability Working Group and Privacy & Rearc Commit Group. Please review the governance rules [here](https://github.com/IABTechLab/uid2-core/blob/master/Software%20Development%20and%20Release%20Procedures.md)
+The UID 2 Project is subject to Tech Lab IPR’s Policy and is managed by the IAB Tech Lab Addressability Working Group and Privacy & Rearc Commit Group. Please review [the governance rules](https://github.com/IABTechLab/uid2-core/blob/master/Software%20Development%20and%20Release%20Procedures.md).
 
-Client SDK for working with UID2 services.
+This SDK simplifies integration with UID2 for those using Python.
 
-SDK supports Python 3.6 and above.
+## Dependencies
+
+This SDK supports Python 3.6 and above.
 
 ## Quick Start
 
-Connect to the UID2 service, refresh encryption keys and use those to decrypt an advertising ID
-from an advertising token:
+Connect to the UID2 service, refresh the encryption keys, and then use the keys to decrypt an advertising token, to arrive at the corresponding advertising ID:
 
 ```
 from uid2_client import Uid2Client, decrypt_token
 
 client = Uid2Client('https://prod.uidapi.com', 'my-auth-token', 'my-secret-key')
 keys = client.refresh_keys()
 advertising_token = 'AgAAAANRdREk+IWqqnQkZ2rZdK0TgSUP/owLryysSkUGZJT+Gy551L1WJMAZA/G2B1UMDQ20WAqwwTu6o9TexWyux0lg0HHIbmJjN6IYwo+42KC8ugaR+PX0y18qQ+3yzkxmJ/ee//4IGu/1Yq4AmO4ArXN6CeszPTxByTkysVqyQVNY2A=='
 decrypted_token = decrypt_token(advertising_token, keys)
 print(decrypted_token.uid2)
 ```
 
-More examples can be found in the [examples] directory.
+Additional examples are in the [examples] directory:
+* [sample_auto_refresh.py](examples/sample_auto_refresh.py)
+* [sample_client.py](examples/sample_client.py)
+* [sample_encryption.py](examples/sample_encryption.py)
 
 ## Development
 
-Required for all subsequent commands, build docker image with Python 3.6 and all dev dependencies:
+First, build the Docker image with Python 3.6 and all dev dependencies. This is required for all subsequent commands. Run the following:
 
 ```
 make docker
 ```
 
 Run unit tests:
 
@@ -58,30 +62,30 @@
 
 Build a bdist wheel:
 
 ```
 make wheel
 ```
 
-Get access to interactive shell within the Python 3.6 docker image:
+Get access to an interactive shell within the Python 3.6 Docker image:
 
 ```
 make shell
 ```
 
-Run all the example applications:
+## Example Usage
+
+To run all the example applications:
 
 ```
 make examples BASE_URL=https://prod.uidapi.com AUTH_KEY=my-auth-key SECRET_KEY=my-secret-key \
 	AD_TOKEN=AgAAAANRdREk+IWqqnQkZ2rZdK0TgSUP/owLryysSkUGZJT+Gy551L1WJMAZA/G2B1UMDQ20WAqwwTu6o9TexWyux0lg0HHIbmJjN6IYwo+42KC8ugaR+PX0y18qQ+3yzkxmJ/ee//4IGu/1Yq4AmO4ArXN6CeszPTxByTkysVqyQVNY2A==
 ```
 
-Or specific examples:
+Alternatively, you can run specific examples:
 
 ```
 make example_client BASE_URL=https://prod.uidapi.com AUTH_KEY=my-auth-key SECRET_KEY=my-secret-key \
 	AD_TOKEN=AgAAAANRdREk+IWqqnQkZ2rZdK0TgSUP/owLryysSkUGZJT+Gy551L1WJMAZA/G2B1UMDQ20WAqwwTu6o9TexWyux0lg0HHIbmJjN6IYwo+42KC8ugaR+PX0y18qQ+3yzkxmJ/ee//4IGu/1Yq4AmO4ArXN6CeszPTxByTkysVqyQVNY2A==
 make example_auto_refresh BASE_URL=https://prod.uidapi.com AUTH_KEY=my-auth-key SECRET_KEY=my-secret-key \
 	AD_TOKEN=AgAAAANRdREk+IWqqnQkZ2rZdK0TgSUP/owLryysSkUGZJT+Gy551L1WJMAZA/G2B1UMDQ20WAqwwTu6o9TexWyux0lg0HHIbmJjN6IYwo+42KC8ugaR+PX0y18qQ+3yzkxmJ/ee//4IGu/1Yq4AmO4ArXN6CeszPTxByTkysVqyQVNY2A==
 ```
-
-
```

### Comparing `uid2_client-2.0.0/README.md` & `uid2_client-2.0.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,39 @@
-# Uid2 Client Python
+# UID2 SDK for Python
 
-The UID 2 Project is subject to Tech Lab IPR’s Policy and is managed by the IAB Tech Lab Addressability Working Group and Privacy & Rearc Commit Group. Please review the governance rules [here](https://github.com/IABTechLab/uid2-core/blob/master/Software%20Development%20and%20Release%20Procedures.md)
+The UID 2 Project is subject to Tech Lab IPR’s Policy and is managed by the IAB Tech Lab Addressability Working Group and Privacy & Rearc Commit Group. Please review [the governance rules](https://github.com/IABTechLab/uid2-core/blob/master/Software%20Development%20and%20Release%20Procedures.md).
 
-Client SDK for working with UID2 services.
+This SDK simplifies integration with UID2 for those using Python.
 
-SDK supports Python 3.6 and above.
+## Dependencies
+
+This SDK supports Python 3.6 and above.
 
 ## Quick Start
 
-Connect to the UID2 service, refresh encryption keys and use those to decrypt an advertising ID
-from an advertising token:
+Connect to the UID2 service, refresh the encryption keys, and then use the keys to decrypt an advertising token, to arrive at the corresponding advertising ID:
 
 ```
 from uid2_client import Uid2Client, decrypt_token
 
 client = Uid2Client('https://prod.uidapi.com', 'my-auth-token', 'my-secret-key')
 keys = client.refresh_keys()
 advertising_token = 'AgAAAANRdREk+IWqqnQkZ2rZdK0TgSUP/owLryysSkUGZJT+Gy551L1WJMAZA/G2B1UMDQ20WAqwwTu6o9TexWyux0lg0HHIbmJjN6IYwo+42KC8ugaR+PX0y18qQ+3yzkxmJ/ee//4IGu/1Yq4AmO4ArXN6CeszPTxByTkysVqyQVNY2A=='
 decrypted_token = decrypt_token(advertising_token, keys)
 print(decrypted_token.uid2)
 ```
 
-More examples can be found in the [examples] directory.
+Additional examples are in the [examples] directory:
+* [sample_auto_refresh.py](examples/sample_auto_refresh.py)
+* [sample_client.py](examples/sample_client.py)
+* [sample_encryption.py](examples/sample_encryption.py)
 
 ## Development
 
-Required for all subsequent commands, build docker image with Python 3.6 and all dev dependencies:
+First, build the Docker image with Python 3.6 and all dev dependencies. This is required for all subsequent commands. Run the following:
 
 ```
 make docker
 ```
 
 Run unit tests:
 
@@ -39,30 +43,30 @@
 
 Build a bdist wheel:
 
 ```
 make wheel
 ```
 
-Get access to interactive shell within the Python 3.6 docker image:
+Get access to an interactive shell within the Python 3.6 Docker image:
 
 ```
 make shell
 ```
 
-Run all the example applications:
+## Example Usage
+
+To run all the example applications:
 
 ```
 make examples BASE_URL=https://prod.uidapi.com AUTH_KEY=my-auth-key SECRET_KEY=my-secret-key \
 	AD_TOKEN=AgAAAANRdREk+IWqqnQkZ2rZdK0TgSUP/owLryysSkUGZJT+Gy551L1WJMAZA/G2B1UMDQ20WAqwwTu6o9TexWyux0lg0HHIbmJjN6IYwo+42KC8ugaR+PX0y18qQ+3yzkxmJ/ee//4IGu/1Yq4AmO4ArXN6CeszPTxByTkysVqyQVNY2A==
 ```
 
-Or specific examples:
+Alternatively, you can run specific examples:
 
 ```
 make example_client BASE_URL=https://prod.uidapi.com AUTH_KEY=my-auth-key SECRET_KEY=my-secret-key \
 	AD_TOKEN=AgAAAANRdREk+IWqqnQkZ2rZdK0TgSUP/owLryysSkUGZJT+Gy551L1WJMAZA/G2B1UMDQ20WAqwwTu6o9TexWyux0lg0HHIbmJjN6IYwo+42KC8ugaR+PX0y18qQ+3yzkxmJ/ee//4IGu/1Yq4AmO4ArXN6CeszPTxByTkysVqyQVNY2A==
 make example_auto_refresh BASE_URL=https://prod.uidapi.com AUTH_KEY=my-auth-key SECRET_KEY=my-secret-key \
 	AD_TOKEN=AgAAAANRdREk+IWqqnQkZ2rZdK0TgSUP/owLryysSkUGZJT+Gy551L1WJMAZA/G2B1UMDQ20WAqwwTu6o9TexWyux0lg0HHIbmJjN6IYwo+42KC8ugaR+PX0y18qQ+3yzkxmJ/ee//4IGu/1Yq4AmO4ArXN6CeszPTxByTkysVqyQVNY2A==
 ```
-
-
```

### Comparing `uid2_client-2.0.0/pyproject.toml` & `uid2_client-2.0.2/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -3,19 +3,19 @@
     "setuptools >= 40.9.0",
     "wheel",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "uid2_client"
-version = "2.0.0"
+version = "2.0.2"
 authors = [
-    { name = "Cody Constine", email = "cody.constine@thetradedesk.com" }
+    { name = "UID2 team", email = "unifiedid-admin@thetradedesk.com" }
 ]
-description = "UID2 sdk for the UID2 and EUID apis"
+description = "UID2 SDK for Python"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
```

### Comparing `uid2_client-2.0.0/setup.cfg` & `uid2_client-2.0.2/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 [metadata]
 name = uid2-client
-version = 2.0.1
 author = UID2 team
 author_email = unifiedid-admin@thetradedesk.com
 home_page = https://iabtechlab.com
 description = Client for working with advertising UID2 services
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = Apache 2.0
```

### Comparing `uid2_client-2.0.0/tests/test_encryption.py` & `uid2_client-2.0.2/tests/test_encryption.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,14 +44,36 @@
     def cross_platform_consistency_check_base64_url_test(self, raw_input, expected_base64_url_str):
         base64_url_encoded_str = Uid2Base64UrlCoder.encode(raw_input)
         self.assertEqual(expected_base64_url_str, base64_url_encoded_str)
 
         decoded = Uid2Base64UrlCoder.decode(base64_url_encoded_str)
         self.assertEqual(decoded, raw_input)
 
+    def validate_advertising_token(self, advertising_token_string, identity_scope, identity_type):
+        first_char = advertising_token_string[0]
+        if identity_scope == IdentityScope.UID2:
+            self.assertEqual("A" if identity_type == IdentityType.Email.value else "B", first_char)
+        else:
+            self.assertEqual("E" if identity_type == IdentityType.Email.value else "F", first_char)
+
+        second_char = advertising_token_string[1]
+        self.assertEqual("4", second_char)
+
+        # No URL-unfriendly characters allowed
+        self.assertEqual(-1, advertising_token_string.find("="))
+        self.assertEqual(-1, advertising_token_string.find("+"))
+        self.assertEqual(-1, advertising_token_string.find("/"))
+
+
+    def generate_uid2_token_v4(self, uid, master_key, site_id, site_key, params = Params(), identity_type = IdentityType.Email, identity_scope = IdentityScope.UID2):
+        advertising_token = UID2TokenGenerator.generate_uid2_token_v4(uid, master_key, site_id, site_key, params)
+        self.validate_advertising_token(advertising_token, identity_scope, identity_type)
+        return advertising_token
+
+
     def test_cross_platform_consistency_decrypt(self):
         crossPlatformAdvertisingToken = "AIAAAACkOqJj9VoxXJNnuX3v-ymceRf8_Av0vA5asOj9YBZJc1kV1vHdmb0AIjlzWnFF-gxIlgXqhRFhPo3iXpugPBl3gv4GKnGkw-Zgm2QqMsDPPLpMCYiWrIUqHPm8hQiq9PuTU-Ba9xecRsSIAN0WCwKLwA_EDVdzmnLJu64dQoeYmuu3u1G2EuTkuMrevmP98tJqSUePKwnfK73-0Zdshw";
         # Sunday, 1 January 2023 1:01:01 AM UTC
         referenceTimestampMs = 1672534861000
         # 1 hour before ref timestamp
         established_ms = referenceTimestampMs - (3600 * 1000);
         last_refreshed_ms = referenceTimestampMs;
@@ -74,56 +96,57 @@
                                    _master_secret)
         site_key = EncryptionKey(_site_key_id, -1, site_key_created, site_key_activates, site_key_expires,
                                  _site_secret)
 
         params = Params(dt.timedelta(days=1 * 365 * 20))
 
         # verify that the dynamically created ad token can be decrypted
-        runtime_advertising_token = UID2TokenGenerator.generate_uid2_token_v4(_example_id, master_key, _site_id, site_key, params)
+        runtime_advertising_token = self.generate_uid2_token_v4(_example_id, master_key, _site_id, site_key, params)
         # best effort check as the token might simply just not require padding
         self.assertEqual(-1, runtime_advertising_token.find('='))
         self.assertEqual(-1, runtime_advertising_token.find('+'))
         self.assertEqual(-1, runtime_advertising_token.find('/'))
 
         result = decrypt(runtime_advertising_token, EncryptionKeysCollection([_master_key, _site_key]))
         self.assertEqual(_example_id, result.uid2)
 
         # can also decrypt a known token generated from other SDK
         result = decrypt(crossPlatformAdvertisingToken, EncryptionKeysCollection([_master_key, _site_key]))
         self.assertEqual(_example_id, result.uid2)
 
+
     def test_decrypt_token_v4(self):
-        token = UID2TokenGenerator.generate_uid2_token_v4(_example_id, _master_key, _site_id, _site_key)
+        token = self.generate_uid2_token_v4(_example_id, _master_key, _site_id, _site_key)
 
         keys = EncryptionKeysCollection([_master_key, _site_key])
         result = decrypt(token, keys)
 
         self.assertEqual(_example_id, result.uid2)
 
 
     def test_decrypt_token_v4_empty_keys(self):
-        token = UID2TokenGenerator.generate_uid2_token_v4(_example_id, _master_key, _site_id, _site_key)
+        token = self.generate_uid2_token_v4(_example_id, _master_key, _site_id, _site_key)
 
         keys = EncryptionKeysCollection([])
 
         with self.assertRaises(EncryptionError):
             result = decrypt(token, keys)
 
 
     def test_decrypt_token_v4_no_master_key(self):
-        token = UID2TokenGenerator.generate_uid2_token_v4(_example_id, _master_key, _site_id, _site_key)
+        token = self.generate_uid2_token_v4(_example_id, _master_key, _site_id, _site_key)
 
         keys = EncryptionKeysCollection([_site_key])
 
         with self.assertRaises(EncryptionError):
             result = decrypt(token, keys)
 
 
     def test_decrypt_token_v4_no_site_key(self):
-        token = UID2TokenGenerator.generate_uid2_token_v4(_example_id, _master_key, _site_id, _site_key)
+        token = self.generate_uid2_token_v4(_example_id, _master_key, _site_id, _site_key)
 
         keys = EncryptionKeysCollection([_master_key])
 
         with self.assertRaises(EncryptionError):
             result = decrypt(token, keys)
 
     def test_decrypt_token_v4_invalid_version(self):
@@ -134,39 +157,39 @@
 
         with self.assertRaises(EncryptionError):
             result = decrypt(token, keys)
 
 
     def test_decrypt_token_v4_expired(self):
         params = Params(dt.timedelta(seconds=-1))
-        token = UID2TokenGenerator.generate_uid2_token_v4(_example_id, _master_key, _site_id, _site_key, params)
+        token = self.generate_uid2_token_v4(_example_id, _master_key, _site_id, _site_key, params)
 
         keys = EncryptionKeysCollection([_master_key, _site_key])
 
         with self.assertRaises(EncryptionError):
             result = decrypt(token, keys)
 
 
     def test_decrypt_token_v4_custom_now(self):
         expiry = dt.datetime(2021, 3, 22, 9, 1, 2, tzinfo=timezone.utc)
         params = Params(expiry)
-        token = UID2TokenGenerator.generate_uid2_token_v4(_example_id, _master_key, _site_id, _site_key, params)
+        token = self.generate_uid2_token_v4(_example_id, _master_key, _site_id, _site_key, params)
 
         keys = EncryptionKeysCollection([_master_key, _site_key])
 
         with self.assertRaises(EncryptionError):
             result = decrypt(token, keys, now=expiry + dt.timedelta(seconds=1))
 
         result = decrypt(token, keys, now=expiry - dt.timedelta(seconds=1))
         self.assertEqual(_example_id, result.uid2)
 
 
     def test_decrypt_token_v4_invalid_payload(self):
         params = Params(dt.timedelta(seconds=-1))
-        token = UID2TokenGenerator.generate_uid2_token_v4(_example_id, _master_key, _site_id, _site_key, params)
+        token = self.generate_uid2_token_v4(_example_id, _master_key, _site_id, _site_key, params)
 
         keys = EncryptionKeysCollection([_master_key, _site_key])
 
         with self.assertRaises(EncryptionError):
             result = decrypt(token[:-3], keys)
 
 
@@ -592,14 +615,15 @@
         keys = EncryptionKeysCollection([key])
         encrypted = UID2TokenGenerator.encrypt_data_v2(data, key=key, site_id=12345, now=now)
         decrypted = decrypt_data(encrypted, keys)
         self.assertEqual(data, decrypted.data)
         self.assertEqual(format_time(now), format_time(decrypted.encrypted_at))
 
 
+    # TODO - deduplicate the logic in sharing_test.py that has been copied from this file
     def test_raw_uid_produces_correct_identity_type_in_token(self):
         #v2 +12345678901. Although this was generated from a phone number, it's a v2 raw UID which doesn't encode this
         # information, so token assumes email by default.
         self.verify_identity_type("Q4bGug8t1xjsutKLCNjnb5fTlXSvIQukmahYDJeLBtk=",
                                                       IdentityType.Email.value)
         self.verify_identity_type("BEOGxroPLdcY7LrSiwjY52+X05V0ryELpJmoWAyXiwbZ",
                                                       IdentityType.Phone.value) #v3 +12345678901
@@ -607,15 +631,15 @@
                                                       IdentityType.Email.value) #v2 test@example.com
         self.verify_identity_type("AKCoNGWPYng/whjBIwANJHKvvGlGyzARtDIAk95FlJyb",
                                                       IdentityType.Email.value) #v3 test@example.com
         self.verify_identity_type("EKCoNGWPYng/whjBIwANJHKvvGlGyzARtDIAk95FlJyb",
                                                       IdentityType.Email.value) #v3 EUID test@example.com
 
     def verify_identity_type(self, raw_uid, expected_identity_type):
-        token = UID2TokenGenerator.generate_uid2_token_v4(raw_uid, _master_key, _site_id, _site_key)
+        token = self.generate_uid2_token_v4(raw_uid, _master_key, _site_id, _site_key, Params(), expected_identity_type)
         keys = EncryptionKeysCollection([_master_key, _site_key])
         result = decrypt(token, keys)
         self.assertEqual(raw_uid, result.uid2)
         self.assertEqual(expected_identity_type, get_token_identity_type(token))
 
 
 def get_token_identity_type(id):
```

### Comparing `uid2_client-2.0.0/tests/test_key_parse.py` & `uid2_client-2.0.2/tests/test_key_parse.py`

 * *Files identical despite different names*

### Comparing `uid2_client-2.0.0/tests/test_keys.py` & `uid2_client-2.0.2/tests/test_keys.py`

 * *Files identical despite different names*

### Comparing `uid2_client-2.0.0/uid2_client/auto_refresh.py` & `uid2_client-2.0.2/uid2_client/auto_refresh.py`

 * *Files identical despite different names*

### Comparing `uid2_client-2.0.0/uid2_client/client.py` & `uid2_client-2.0.2/uid2_client/client.py`

 * *Files identical despite different names*

### Comparing `uid2_client-2.0.0/uid2_client/encryption.py` & `uid2_client-2.0.2/uid2_client/encryption.py`

 * *Files identical despite different names*

### Comparing `uid2_client-2.0.0/uid2_client/keys.py` & `uid2_client-2.0.2/uid2_client/keys.py`

 * *Files identical despite different names*

### Comparing `uid2_client-2.0.0/uid2_client/uid2_base64_url_coder.py` & `uid2_client-2.0.2/uid2_client/uid2_base64_url_coder.py`

 * *Files identical despite different names*

### Comparing `uid2_client-2.0.0/uid2_client.egg-info/PKG-INFO` & `uid2_client-2.0.2/uid2_client.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,54 +1,58 @@
 Metadata-Version: 2.1
 Name: uid2-client
-Version: 2.0.0
-Summary: UID2 sdk for the UID2 and EUID apis
+Version: 2.0.2
+Summary: UID2 SDK for Python
 Home-page: https://iabtechlab.com
 Author: UID2 team
-Author-email: Cody Constine <cody.constine@thetradedesk.com>
+Author-email: UID2 team <unifiedid-admin@thetradedesk.com>
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/IABTechLab/uid2-client-python
 Project-URL: Bug Tracker, https://github.com/IABTechLab/uid2-client-python/issues
 Keywords: uid2
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Uid2 Client Python
+# UID2 SDK for Python
 
-The UID 2 Project is subject to Tech Lab IPR’s Policy and is managed by the IAB Tech Lab Addressability Working Group and Privacy & Rearc Commit Group. Please review the governance rules [here](https://github.com/IABTechLab/uid2-core/blob/master/Software%20Development%20and%20Release%20Procedures.md)
+The UID 2 Project is subject to Tech Lab IPR’s Policy and is managed by the IAB Tech Lab Addressability Working Group and Privacy & Rearc Commit Group. Please review [the governance rules](https://github.com/IABTechLab/uid2-core/blob/master/Software%20Development%20and%20Release%20Procedures.md).
 
-Client SDK for working with UID2 services.
+This SDK simplifies integration with UID2 for those using Python.
 
-SDK supports Python 3.6 and above.
+## Dependencies
+
+This SDK supports Python 3.6 and above.
 
 ## Quick Start
 
-Connect to the UID2 service, refresh encryption keys and use those to decrypt an advertising ID
-from an advertising token:
+Connect to the UID2 service, refresh the encryption keys, and then use the keys to decrypt an advertising token, to arrive at the corresponding advertising ID:
 
 ```
 from uid2_client import Uid2Client, decrypt_token
 
 client = Uid2Client('https://prod.uidapi.com', 'my-auth-token', 'my-secret-key')
 keys = client.refresh_keys()
 advertising_token = 'AgAAAANRdREk+IWqqnQkZ2rZdK0TgSUP/owLryysSkUGZJT+Gy551L1WJMAZA/G2B1UMDQ20WAqwwTu6o9TexWyux0lg0HHIbmJjN6IYwo+42KC8ugaR+PX0y18qQ+3yzkxmJ/ee//4IGu/1Yq4AmO4ArXN6CeszPTxByTkysVqyQVNY2A=='
 decrypted_token = decrypt_token(advertising_token, keys)
 print(decrypted_token.uid2)
 ```
 
-More examples can be found in the [examples] directory.
+Additional examples are in the [examples] directory:
+* [sample_auto_refresh.py](examples/sample_auto_refresh.py)
+* [sample_client.py](examples/sample_client.py)
+* [sample_encryption.py](examples/sample_encryption.py)
 
 ## Development
 
-Required for all subsequent commands, build docker image with Python 3.6 and all dev dependencies:
+First, build the Docker image with Python 3.6 and all dev dependencies. This is required for all subsequent commands. Run the following:
 
 ```
 make docker
 ```
 
 Run unit tests:
 
@@ -58,30 +62,30 @@
 
 Build a bdist wheel:
 
 ```
 make wheel
 ```
 
-Get access to interactive shell within the Python 3.6 docker image:
+Get access to an interactive shell within the Python 3.6 Docker image:
 
 ```
 make shell
 ```
 
-Run all the example applications:
+## Example Usage
+
+To run all the example applications:
 
 ```
 make examples BASE_URL=https://prod.uidapi.com AUTH_KEY=my-auth-key SECRET_KEY=my-secret-key \
 	AD_TOKEN=AgAAAANRdREk+IWqqnQkZ2rZdK0TgSUP/owLryysSkUGZJT+Gy551L1WJMAZA/G2B1UMDQ20WAqwwTu6o9TexWyux0lg0HHIbmJjN6IYwo+42KC8ugaR+PX0y18qQ+3yzkxmJ/ee//4IGu/1Yq4AmO4ArXN6CeszPTxByTkysVqyQVNY2A==
 ```
 
-Or specific examples:
+Alternatively, you can run specific examples:
 
 ```
 make example_client BASE_URL=https://prod.uidapi.com AUTH_KEY=my-auth-key SECRET_KEY=my-secret-key \
 	AD_TOKEN=AgAAAANRdREk+IWqqnQkZ2rZdK0TgSUP/owLryysSkUGZJT+Gy551L1WJMAZA/G2B1UMDQ20WAqwwTu6o9TexWyux0lg0HHIbmJjN6IYwo+42KC8ugaR+PX0y18qQ+3yzkxmJ/ee//4IGu/1Yq4AmO4ArXN6CeszPTxByTkysVqyQVNY2A==
 make example_auto_refresh BASE_URL=https://prod.uidapi.com AUTH_KEY=my-auth-key SECRET_KEY=my-secret-key \
 	AD_TOKEN=AgAAAANRdREk+IWqqnQkZ2rZdK0TgSUP/owLryysSkUGZJT+Gy551L1WJMAZA/G2B1UMDQ20WAqwwTu6o9TexWyux0lg0HHIbmJjN6IYwo+42KC8ugaR+PX0y18qQ+3yzkxmJ/ee//4IGu/1Yq4AmO4ArXN6CeszPTxByTkysVqyQVNY2A==
 ```
-
-
```

### Comparing `uid2_client-2.0.0/uid2_client.egg-info/SOURCES.txt` & `uid2_client-2.0.2/uid2_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

