# Comparing `tmp/py_sec_vault-0.0.1.3.tar.gz` & `tmp/py_sec_vault-0.0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_sec_vault-0.0.1.3.tar", max compression
+gzip compressed data, was "py_sec_vault-0.0.1.4.tar", max compression
```

## Comparing `py_sec_vault-0.0.1.3.tar` & `py_sec_vault-0.0.1.4.tar`

### file list

```diff
@@ -1,6 +1,8 @@
--rw-r--r--   0        0        0     1096 2023-06-09 13:11:12.838127 py_sec_vault-0.0.1.3/LICENSE
--rw-r--r--   0        0        0       65 2023-06-09 13:10:13.618732 py_sec_vault-0.0.1.3/README.md
--rw-r--r--   0        0        0      902 2023-06-13 11:02:11.938830 py_sec_vault-0.0.1.3/pyproject.toml
--rw-r--r--   0        0        0       56 2023-06-13 11:01:48.495001 py_sec_vault-0.0.1.3/vault/__init__.py
--rw-r--r--   0        0        0       39 2023-06-13 10:51:26.649903 py_sec_vault-0.0.1.3/vault/main.py
--rw-r--r--   0        0        0      940 1970-01-01 00:00:00.000000 py_sec_vault-0.0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1096 2023-06-09 13:11:12.838127 py_sec_vault-0.0.1.4/LICENSE
+-rw-r--r--   0        0        0       65 2023-06-09 13:10:13.618732 py_sec_vault-0.0.1.4/README.md
+-rw-r--r--   0        0        0      902 2023-06-13 20:33:37.348083 py_sec_vault-0.0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      262 2023-06-13 19:45:09.845294 py_sec_vault-0.0.1.4/vault/__init__.py
+-rw-r--r--   0        0        0      472 2023-06-13 19:47:07.525818 py_sec_vault-0.0.1.4/vault/config.py
+-rw-r--r--   0        0        0      199 2023-06-13 19:39:16.178247 py_sec_vault-0.0.1.4/vault/exceptions.py
+-rw-r--r--   0        0        0     3389 2023-06-13 19:50:10.481908 py_sec_vault-0.0.1.4/vault/main.py
+-rw-r--r--   0        0        0      940 1970-01-01 00:00:00.000000 py_sec_vault-0.0.1.4/PKG-INFO
```

### Comparing `py_sec_vault-0.0.1.3/LICENSE` & `py_sec_vault-0.0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `py_sec_vault-0.0.1.3/pyproject.toml` & `py_sec_vault-0.0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-sec-vault"
-version = "0.0.1.3"
+version = "0.0.1.4"
 description = "Hashicorp Vault implementation in python software"
 authors = ["CISolutions B.V. <info@cisolutions.nl>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "vault"}]
 homepage = "https://github.com/zEktONO/py-sec-vault"
 repository = "https://github.com/zEktONO/py-sec-vault"
```

### Comparing `py_sec_vault-0.0.1.3/PKG-INFO` & `py_sec_vault-0.0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-sec-vault
-Version: 0.0.1.3
+Version: 0.0.1.4
 Summary: Hashicorp Vault implementation in python software
 Home-page: https://github.com/zEktONO/py-sec-vault
 License: MIT
 Keywords: vault,hashicorp,security
 Author: CISolutions B.V.
 Author-email: info@cisolutions.nl
 Requires-Python: >=3.11,<4.0
```

