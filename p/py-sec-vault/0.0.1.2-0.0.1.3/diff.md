# Comparing `tmp/py_sec_vault-0.0.1.2.tar.gz` & `tmp/py_sec_vault-0.0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_sec_vault-0.0.1.2.tar", max compression
+gzip compressed data, was "py_sec_vault-0.0.1.3.tar", max compression
```

## Comparing `py_sec_vault-0.0.1.2.tar` & `py_sec_vault-0.0.1.3.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     1096 2023-06-09 13:11:12.838127 py_sec_vault-0.0.1.2/LICENSE
--rw-r--r--   0        0        0       65 2023-06-09 13:10:13.618732 py_sec_vault-0.0.1.2/README.md
--rw-r--r--   0        0        0      900 2023-06-13 10:58:18.194103 py_sec_vault-0.0.1.2/pyproject.toml
--rw-r--r--   0        0        0       48 2023-06-12 20:29:45.699053 py_sec_vault-0.0.1.2/src/__init__.py
--rw-r--r--   0        0        0       62 2023-06-13 10:53:23.328606 py_sec_vault-0.0.1.2/src/vault/__init__.py
--rw-r--r--   0        0        0       39 2023-06-13 10:51:26.649903 py_sec_vault-0.0.1.2/src/vault/main.py
--rw-r--r--   0        0        0      940 1970-01-01 00:00:00.000000 py_sec_vault-0.0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1096 2023-06-09 13:11:12.838127 py_sec_vault-0.0.1.3/LICENSE
+-rw-r--r--   0        0        0       65 2023-06-09 13:10:13.618732 py_sec_vault-0.0.1.3/README.md
+-rw-r--r--   0        0        0      902 2023-06-13 11:02:11.938830 py_sec_vault-0.0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       56 2023-06-13 11:01:48.495001 py_sec_vault-0.0.1.3/vault/__init__.py
+-rw-r--r--   0        0        0       39 2023-06-13 10:51:26.649903 py_sec_vault-0.0.1.3/vault/main.py
+-rw-r--r--   0        0        0      940 1970-01-01 00:00:00.000000 py_sec_vault-0.0.1.3/PKG-INFO
```

### Comparing `py_sec_vault-0.0.1.2/LICENSE` & `py_sec_vault-0.0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `py_sec_vault-0.0.1.2/pyproject.toml` & `py_sec_vault-0.0.1.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 name = "py-sec-vault"
-version = "0.0.1.2"
+version = "0.0.1.3"
 description = "Hashicorp Vault implementation in python software"
 authors = ["CISolutions B.V. <info@cisolutions.nl>"]
 license = "MIT"
 readme = "README.md"
-packages = [{include = "src"}]
+packages = [{include = "vault"}]
 homepage = "https://github.com/zEktONO/py-sec-vault"
 repository = "https://github.com/zEktONO/py-sec-vault"
 keywords = ["vault", "hashicorp", "security"]
 classifiers = [
     "Environment :: Console",
     "Operating System :: OS Independent",
     "Topic :: Software Development :: Documentation",
```

### Comparing `py_sec_vault-0.0.1.2/PKG-INFO` & `py_sec_vault-0.0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-sec-vault
-Version: 0.0.1.2
+Version: 0.0.1.3
 Summary: Hashicorp Vault implementation in python software
 Home-page: https://github.com/zEktONO/py-sec-vault
 License: MIT
 Keywords: vault,hashicorp,security
 Author: CISolutions B.V.
 Author-email: info@cisolutions.nl
 Requires-Python: >=3.11,<4.0
```

