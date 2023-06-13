# Comparing `tmp/phase_dev-1.0.0.tar.gz` & `tmp/phase_dev-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phase_dev-1.0.0.tar", last modified: Fri Jun  2 10:03:31 2023, max compression
+gzip compressed data, was "phase_dev-1.1.0.tar", last modified: Tue Jun 13 09:47:20 2023, max compression
```

## Comparing `phase_dev-1.0.0.tar` & `phase_dev-1.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 ascendance  (1000) ascendance  (1000)        0 2023-06-02 10:03:31.985133 phase_dev-1.0.0/
--rw-r--r--   0 ascendance  (1000) ascendance  (1000)     1062 2023-06-01 07:28:57.000000 phase_dev-1.0.0/LICENSE
--rw-r--r--   0 ascendance  (1000) ascendance  (1000)      913 2023-06-02 10:03:31.984133 phase_dev-1.0.0/PKG-INFO
--rw-r--r--   0 ascendance  (1000) ascendance  (1000)      447 2023-06-02 09:41:28.000000 phase_dev-1.0.0/README.md
--rw-r--r--   0 ascendance  (1000) ascendance  (1000)      659 2023-06-02 09:41:35.000000 phase_dev-1.0.0/pyproject.toml
--rw-r--r--   0 ascendance  (1000) ascendance  (1000)       38 2023-06-02 10:03:31.985133 phase_dev-1.0.0/setup.cfg
-drwxr-xr-x   0 ascendance  (1000) ascendance  (1000)        0 2023-06-02 10:03:31.981133 phase_dev-1.0.0/src/
-drwxr-xr-x   0 ascendance  (1000) ascendance  (1000)        0 2023-06-02 10:03:31.982133 phase_dev-1.0.0/src/phase/
--rw-r--r--   0 ascendance  (1000) ascendance  (1000)       46 2023-06-01 07:28:57.000000 phase_dev-1.0.0/src/phase/__init__.py
--rw-r--r--   0 ascendance  (1000) ascendance  (1000)     3510 2023-06-01 07:28:57.000000 phase_dev-1.0.0/src/phase/phase.py
-drwxr-xr-x   0 ascendance  (1000) ascendance  (1000)        0 2023-06-02 10:03:31.983133 phase_dev-1.0.0/src/phase/utils/
--rw-r--r--   0 ascendance  (1000) ascendance  (1000)        0 2023-06-01 07:28:57.000000 phase_dev-1.0.0/src/phase/utils/__init__.py
--rw-r--r--   0 ascendance  (1000) ascendance  (1000)     4728 2023-06-01 07:28:57.000000 phase_dev-1.0.0/src/phase/utils/crypto.py
--rw-r--r--   0 ascendance  (1000) ascendance  (1000)       44 2023-06-02 09:41:46.000000 phase_dev-1.0.0/src/phase/version.py
-drwxr-xr-x   0 ascendance  (1000) ascendance  (1000)        0 2023-06-02 10:03:31.983133 phase_dev-1.0.0/src/phase_dev.egg-info/
--rw-r--r--   0 ascendance  (1000) ascendance  (1000)      913 2023-06-02 10:03:31.000000 phase_dev-1.0.0/src/phase_dev.egg-info/PKG-INFO
--rw-r--r--   0 ascendance  (1000) ascendance  (1000)      395 2023-06-02 10:03:31.000000 phase_dev-1.0.0/src/phase_dev.egg-info/SOURCES.txt
--rw-r--r--   0 ascendance  (1000) ascendance  (1000)        1 2023-06-02 10:03:31.000000 phase_dev-1.0.0/src/phase_dev.egg-info/dependency_links.txt
--rw-r--r--   0 ascendance  (1000) ascendance  (1000)       55 2023-06-02 10:03:31.000000 phase_dev-1.0.0/src/phase_dev.egg-info/requires.txt
--rw-r--r--   0 ascendance  (1000) ascendance  (1000)        6 2023-06-02 10:03:31.000000 phase_dev-1.0.0/src/phase_dev.egg-info/top_level.txt
-drwxr-xr-x   0 ascendance  (1000) ascendance  (1000)        0 2023-06-02 10:03:31.984133 phase_dev-1.0.0/tests/
--rw-r--r--   0 ascendance  (1000) ascendance  (1000)     1504 2023-06-01 07:28:57.000000 phase_dev-1.0.0/tests/test_decrypt.py
--rw-r--r--   0 ascendance  (1000) ascendance  (1000)     1378 2023-05-28 08:54:34.000000 phase_dev-1.0.0/tests/test_encrypt.py
--rw-r--r--   0 ascendance  (1000) ascendance  (1000)     1103 2023-06-01 07:28:57.000000 phase_dev-1.0.0/tests/test_init.py
+drwxr-xr-x   0 ascendance  (1000) ascendance  (1000)        0 2023-06-13 09:47:20.203977 phase_dev-1.1.0/
+-rw-r--r--   0 ascendance  (1000) ascendance  (1000)     1062 2023-06-01 07:28:57.000000 phase_dev-1.1.0/LICENSE
+-rw-r--r--   0 ascendance  (1000) ascendance  (1000)      913 2023-06-13 09:47:20.203977 phase_dev-1.1.0/PKG-INFO
+-rw-r--r--   0 ascendance  (1000) ascendance  (1000)      447 2023-06-10 04:57:49.000000 phase_dev-1.1.0/README.md
+-rw-r--r--   0 ascendance  (1000) ascendance  (1000)      659 2023-06-13 09:46:45.000000 phase_dev-1.1.0/pyproject.toml
+-rw-r--r--   0 ascendance  (1000) ascendance  (1000)       38 2023-06-13 09:47:20.203977 phase_dev-1.1.0/setup.cfg
+drwxr-xr-x   0 ascendance  (1000) ascendance  (1000)        0 2023-06-13 09:47:20.199977 phase_dev-1.1.0/src/
+drwxr-xr-x   0 ascendance  (1000) ascendance  (1000)        0 2023-06-13 09:47:20.201977 phase_dev-1.1.0/src/phase/
+-rw-r--r--   0 ascendance  (1000) ascendance  (1000)       46 2023-06-01 07:28:57.000000 phase_dev-1.1.0/src/phase/__init__.py
+-rw-r--r--   0 ascendance  (1000) ascendance  (1000)     3702 2023-06-13 09:46:45.000000 phase_dev-1.1.0/src/phase/phase.py
+drwxr-xr-x   0 ascendance  (1000) ascendance  (1000)        0 2023-06-13 09:47:20.201977 phase_dev-1.1.0/src/phase/utils/
+-rw-r--r--   0 ascendance  (1000) ascendance  (1000)        0 2023-06-01 07:28:57.000000 phase_dev-1.1.0/src/phase/utils/__init__.py
+-rw-r--r--   0 ascendance  (1000) ascendance  (1000)     4683 2023-06-13 09:46:45.000000 phase_dev-1.1.0/src/phase/utils/crypto.py
+-rw-r--r--   0 ascendance  (1000) ascendance  (1000)       44 2023-06-13 09:46:45.000000 phase_dev-1.1.0/src/phase/version.py
+drwxr-xr-x   0 ascendance  (1000) ascendance  (1000)        0 2023-06-13 09:47:20.202977 phase_dev-1.1.0/src/phase_dev.egg-info/
+-rw-r--r--   0 ascendance  (1000) ascendance  (1000)      913 2023-06-13 09:47:20.000000 phase_dev-1.1.0/src/phase_dev.egg-info/PKG-INFO
+-rw-r--r--   0 ascendance  (1000) ascendance  (1000)      395 2023-06-13 09:47:20.000000 phase_dev-1.1.0/src/phase_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 ascendance  (1000) ascendance  (1000)        1 2023-06-13 09:47:20.000000 phase_dev-1.1.0/src/phase_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 ascendance  (1000) ascendance  (1000)       55 2023-06-13 09:47:20.000000 phase_dev-1.1.0/src/phase_dev.egg-info/requires.txt
+-rw-r--r--   0 ascendance  (1000) ascendance  (1000)        6 2023-06-13 09:47:20.000000 phase_dev-1.1.0/src/phase_dev.egg-info/top_level.txt
+drwxr-xr-x   0 ascendance  (1000) ascendance  (1000)        0 2023-06-13 09:47:20.203977 phase_dev-1.1.0/tests/
+-rw-r--r--   0 ascendance  (1000) ascendance  (1000)     1526 2023-06-13 09:46:45.000000 phase_dev-1.1.0/tests/test_decrypt.py
+-rw-r--r--   0 ascendance  (1000) ascendance  (1000)     1378 2023-05-28 08:54:34.000000 phase_dev-1.1.0/tests/test_encrypt.py
+-rw-r--r--   0 ascendance  (1000) ascendance  (1000)     1103 2023-06-01 07:28:57.000000 phase_dev-1.1.0/tests/test_init.py
```

### Comparing `phase_dev-1.0.0/LICENSE` & `phase_dev-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `phase_dev-1.0.0/PKG-INFO` & `phase_dev-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phase_dev
-Version: 1.0.0
+Version: 1.1.0
 Summary: Python SDK for Phase
 Author-email: Phase <rohan@phase.dev>
 Project-URL: Homepage, https://phase.dev
 Project-URL: Documentation, https://docs.phase.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `phase_dev-1.0.0/pyproject.toml` & `phase_dev-1.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "phase_dev"
-version = "1.0.0"
+version = "1.1.0"
 description = "Python SDK for Phase"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `phase_dev-1.0.0/src/phase/phase.py` & `phase_dev-1.1.0/src/phase/phase.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,44 +1,48 @@
 import re
 from nacl.bindings import crypto_kx_server_session_keys, crypto_kx_client_session_keys
 from dataclasses import dataclass
 from .utils.crypto import decrypt_b64, encrypt_b64, fetch_app_key, random_key_pair, reconstruct_secret
 from .version import __version__, __ph_version__
 
+DEFAULT_KMS_HOST = "https://kms.phase.dev"
+
 
 @dataclass
 class AppSecret:
     prefix: str
     pss_version: str
     app_token: str
     keyshare0: str
     keyshare1_unwrap_key: str
 
 
 class Phase:
     _app_id = ''
     _app_pub_key = ''
     _app_secret = None
+    _kms_host = ''
 
-    def __init__(self, app_id, app_secret):
+    def __init__(self, app_id, app_secret, custom_kms_host=None):
         app_id_pattern = re.compile(r"^phApp:v(\d+):([a-fA-F0-9]{64})$")
         app_secret_pattern = re.compile(
             r"^pss:v(\d+):([a-fA-F0-9]{64}):([a-fA-F0-9]{64,128}):([a-fA-F0-9]{64})$")
 
         if not app_id_pattern.match(app_id):
             raise ValueError("Invalid Phase APP_ID")
 
         if not app_secret_pattern.match(app_secret):
             raise ValueError("Invalid Phase APP_SECRET")
 
         self._app_id = app_id
         self._app_pub_key = app_id.split(':')[2]
-        app_secret_segments = app_secret.split(':')
 
+        app_secret_segments = app_secret.split(':')
         self._app_secret = AppSecret(*app_secret_segments)
+        self._kms_host = f"{custom_kms_host}/kms" if custom_kms_host else DEFAULT_KMS_HOST
 
     def encrypt(self, plaintext, tag="") -> str | None:
         """
         Encrypts a plaintext string.
 
         Args:
             plaintext (str): The plaintext to encrypt.
@@ -77,15 +81,15 @@
             [prefix, version, client_pub_key_hex, ct,
                 tag] = phase_ciphertext.split(':')
             if prefix != 'ph' or len(phase_ciphertext.split(':')) != 5:
                 raise ValueError('Ciphertext is invalid')
             client_pub_key = bytes.fromhex(client_pub_key_hex)
 
             keyshare1 = fetch_app_key(
-                self._app_secret.app_token, self._app_secret.keyshare1_unwrap_key, self._app_id, len(ct)/2)
+                self._app_secret.app_token, self._app_secret.keyshare1_unwrap_key, self._app_id, len(ct)/2, self._kms_host)
 
             app_priv_key = reconstruct_secret(
                 [self._app_secret.keyshare0, keyshare1])
 
             session_keys = crypto_kx_server_session_keys(bytes.fromhex(
                 self._app_pub_key), bytes.fromhex(app_priv_key), client_pub_key)
```

### Comparing `phase_dev-1.0.0/src/phase/utils/crypto.py` & `phase_dev-1.1.0/src/phase/utils/crypto.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,14 @@
 import functools
 import base64
 from typing import Tuple
 from nacl.bindings import crypto_kx_keypair, crypto_aead_xchacha20poly1305_ietf_encrypt, crypto_aead_xchacha20poly1305_ietf_decrypt, randombytes, crypto_secretbox_NONCEBYTES
 from ..version import __version__
 
 
-PHASE_KMS_URI = "https://kms.phase.dev/"
-
-
 def xor_bytes(a, b) -> bytes:
     """
     Computes the XOR of two byte arrays byte by byte.
 
     Args:
         a (bytes): The first byte array
         b (bytes): The second byte array.
@@ -125,15 +122,15 @@
     key_bytes = bytes.fromhex(key)
 
     plaintext_bytes = decrypt_raw(ct_bytes, key_bytes)
 
     return plaintext_bytes.decode('utf-8')
 
 
-def fetch_app_key(appToken, wrapKey, appId, dataSize) -> str:
+def fetch_app_key(appToken, wrapKey, appId, dataSize, host) -> str:
     """
     Fetches the application key share from Phase KMS.
 
     Args:
         appToken (str): The token for the application to retrieve the key for.
         wrapKey (str): The key used to encrypt the wrapped key share.
         appId (str): The identifier for the application to retrieve the key for.
@@ -148,15 +145,15 @@
     headers = {
         "Authorization": f"Bearer {appToken}",
         "EventType": "decrypt",
         "PhaseNode": f"python:{__version__}",
         "PhSize": f"{dataSize}"
     }
 
-    response = requests.get(f"{PHASE_KMS_URI}{appId}", headers=headers)
+    response = requests.get(f"{host}/{appId}", headers=headers)
 
     if response.status_code == 404:
         raise Exception("Invalid app token")
     else:
         json_data = response.json()
         wrapped_key_share = json_data["wrappedKeyShare"]
         unwrapped_key = decrypt_raw(bytes.fromhex(
```

### Comparing `phase_dev-1.0.0/src/phase_dev.egg-info/PKG-INFO` & `phase_dev-1.1.0/src/phase_dev.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phase-dev
-Version: 1.0.0
+Version: 1.1.0
 Summary: Python SDK for Phase
 Author-email: Phase <rohan@phase.dev>
 Project-URL: Homepage, https://phase.dev
 Project-URL: Documentation, https://docs.phase.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `phase_dev-1.0.0/tests/test_decrypt.py` & `phase_dev-1.1.0/tests/test_decrypt.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 @pytest.fixture(scope="module")
 def phase_instance():
     return Phase(APP_ID, APP_SECRET)
 
 
-def mock_fetch_app_key(appToken, wrapKey, appId, dataSize):
+def mock_fetch_app_key(appToken, wrapKey, appId, dataSize, custom_kms_host=None):
     return "e35ae9560207c90fa3dd68a8715e13a1ef988bffa284db73f04328df17f37cfe"
 
 
 def test_phase_decrypt_returns_correct_plaintext(phase_instance, monkeypatch):
     data = "Signal"
 
     monkeypatch.setattr("src.phase.phase.fetch_app_key", mock_fetch_app_key)
```

### Comparing `phase_dev-1.0.0/tests/test_encrypt.py` & `phase_dev-1.1.0/tests/test_encrypt.py`

 * *Files identical despite different names*

### Comparing `phase_dev-1.0.0/tests/test_init.py` & `phase_dev-1.1.0/tests/test_init.py`

 * *Files identical despite different names*

