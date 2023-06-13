# Comparing `tmp/planetmint_cryptoconditions-1.2.1.tar.gz` & `tmp/planetmint_cryptoconditions-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "planetmint_cryptoconditions-1.2.1.tar", max compression
+gzip compressed data, was "planetmint_cryptoconditions-1.2.2.tar", max compression
```

## Comparing `planetmint_cryptoconditions-1.2.1.tar` & `planetmint_cryptoconditions-1.2.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0    34523 2023-04-06 09:51:24.506960 planetmint_cryptoconditions-1.2.1/LICENSE
--rw-r--r--   0        0        0      277 2023-04-06 09:51:24.506960 planetmint_cryptoconditions-1.2.1/LICENSE-docs
--rw-r--r--   0        0        0     1686 2023-04-06 09:51:24.506960 planetmint_cryptoconditions-1.2.1/README.rst
--rw-r--r--   0        0        0     1798 2023-04-06 09:51:24.510960 planetmint_cryptoconditions-1.2.1/planetmint_cryptoconditions/__init__.py
--rw-r--r--   0        0        0    13917 2023-04-06 09:51:24.510960 planetmint_cryptoconditions-1.2.1/planetmint_cryptoconditions/condition.py
--rw-r--r--   0        0        0     6057 2023-04-06 09:51:24.510960 planetmint_cryptoconditions-1.2.1/planetmint_cryptoconditions/crypto.py
--rw-r--r--   0        0        0      764 2023-04-06 09:51:24.510960 planetmint_cryptoconditions-1.2.1/planetmint_cryptoconditions/exceptions.py
--rw-r--r--   0        0        0     7321 2023-04-06 09:51:24.510960 planetmint_cryptoconditions-1.2.1/planetmint_cryptoconditions/fulfillment.py
--rw-r--r--   0        0        0        0 2023-04-06 09:51:24.510960 planetmint_cryptoconditions-1.2.1/planetmint_cryptoconditions/schemas/__init__.py
--rw-r--r--   0        0        0     3641 2023-04-06 09:51:24.510960 planetmint_cryptoconditions-1.2.1/planetmint_cryptoconditions/schemas/condition.py
--rw-r--r--   0        0        0     2751 2023-04-06 09:51:24.510960 planetmint_cryptoconditions-1.2.1/planetmint_cryptoconditions/schemas/fingerprint.py
--rw-r--r--   0        0        0     4595 2023-04-06 09:51:24.510960 planetmint_cryptoconditions-1.2.1/planetmint_cryptoconditions/schemas/fulfillment.py
--rw-r--r--   0        0        0     3376 2023-04-06 09:51:24.510960 planetmint_cryptoconditions-1.2.1/planetmint_cryptoconditions/type_registry.py
--rw-r--r--   0        0        0        8 2023-04-06 09:51:24.510960 planetmint_cryptoconditions-1.2.1/planetmint_cryptoconditions/types/__init__.py
--rw-r--r--   0        0        0      499 2023-04-06 09:51:24.510960 planetmint_cryptoconditions-1.2.1/planetmint_cryptoconditions/types/base_sha256.py
--rw-r--r--   0        0        0     6780 2023-04-06 09:51:24.510960 planetmint_cryptoconditions-1.2.1/planetmint_cryptoconditions/types/ed25519.py
--rw-r--r--   0        0        0     9256 2023-04-06 09:51:24.510960 planetmint_cryptoconditions-1.2.1/planetmint_cryptoconditions/types/prefix.py
--rw-r--r--   0        0        0     3691 2023-04-06 09:51:24.510960 planetmint_cryptoconditions-1.2.1/planetmint_cryptoconditions/types/preimage.py
--rw-r--r--   0        0        0     6963 2023-04-06 09:51:24.510960 planetmint_cryptoconditions-1.2.1/planetmint_cryptoconditions/types/rsa.py
--rw-r--r--   0        0        0    14814 2023-04-06 09:51:24.510960 planetmint_cryptoconditions-1.2.1/planetmint_cryptoconditions/types/threshold.py
--rw-r--r--   0        0        0       48 2023-04-06 09:51:24.510960 planetmint_cryptoconditions-1.2.1/planetmint_cryptoconditions/version.py
--rw-r--r--   0        0        0     1547 2023-04-06 09:51:24.514960 planetmint_cryptoconditions-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     3115 1970-01-01 00:00:00.000000 planetmint_cryptoconditions-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-06-13 13:14:59.069047 planetmint_cryptoconditions-1.2.2/LICENSE
+-rw-r--r--   0        0        0      277 2023-06-13 13:14:59.069047 planetmint_cryptoconditions-1.2.2/LICENSE-docs
+-rw-r--r--   0        0        0     1686 2023-06-13 13:14:59.069047 planetmint_cryptoconditions-1.2.2/README.rst
+-rw-r--r--   0        0        0     1798 2023-06-13 13:14:59.073047 planetmint_cryptoconditions-1.2.2/planetmint_cryptoconditions/__init__.py
+-rw-r--r--   0        0        0    13917 2023-06-13 13:14:59.073047 planetmint_cryptoconditions-1.2.2/planetmint_cryptoconditions/condition.py
+-rw-r--r--   0        0        0     6057 2023-06-13 13:14:59.073047 planetmint_cryptoconditions-1.2.2/planetmint_cryptoconditions/crypto.py
+-rw-r--r--   0        0        0      764 2023-06-13 13:14:59.073047 planetmint_cryptoconditions-1.2.2/planetmint_cryptoconditions/exceptions.py
+-rw-r--r--   0        0        0     7321 2023-06-13 13:14:59.073047 planetmint_cryptoconditions-1.2.2/planetmint_cryptoconditions/fulfillment.py
+-rw-r--r--   0        0        0        0 2023-06-13 13:14:59.073047 planetmint_cryptoconditions-1.2.2/planetmint_cryptoconditions/schemas/__init__.py
+-rw-r--r--   0        0        0     3641 2023-06-13 13:14:59.073047 planetmint_cryptoconditions-1.2.2/planetmint_cryptoconditions/schemas/condition.py
+-rw-r--r--   0        0        0     2751 2023-06-13 13:14:59.073047 planetmint_cryptoconditions-1.2.2/planetmint_cryptoconditions/schemas/fingerprint.py
+-rw-r--r--   0        0        0     4595 2023-06-13 13:14:59.073047 planetmint_cryptoconditions-1.2.2/planetmint_cryptoconditions/schemas/fulfillment.py
+-rw-r--r--   0        0        0     3376 2023-06-13 13:14:59.073047 planetmint_cryptoconditions-1.2.2/planetmint_cryptoconditions/type_registry.py
+-rw-r--r--   0        0        0        8 2023-06-13 13:14:59.073047 planetmint_cryptoconditions-1.2.2/planetmint_cryptoconditions/types/__init__.py
+-rw-r--r--   0        0        0      499 2023-06-13 13:14:59.073047 planetmint_cryptoconditions-1.2.2/planetmint_cryptoconditions/types/base_sha256.py
+-rw-r--r--   0        0        0     6780 2023-06-13 13:14:59.073047 planetmint_cryptoconditions-1.2.2/planetmint_cryptoconditions/types/ed25519.py
+-rw-r--r--   0        0        0     9256 2023-06-13 13:14:59.073047 planetmint_cryptoconditions-1.2.2/planetmint_cryptoconditions/types/prefix.py
+-rw-r--r--   0        0        0     3691 2023-06-13 13:14:59.073047 planetmint_cryptoconditions-1.2.2/planetmint_cryptoconditions/types/preimage.py
+-rw-r--r--   0        0        0     6963 2023-06-13 13:14:59.073047 planetmint_cryptoconditions-1.2.2/planetmint_cryptoconditions/types/rsa.py
+-rw-r--r--   0        0        0    14814 2023-06-13 13:14:59.073047 planetmint_cryptoconditions-1.2.2/planetmint_cryptoconditions/types/threshold.py
+-rw-r--r--   0        0        0       48 2023-06-13 13:14:59.073047 planetmint_cryptoconditions-1.2.2/planetmint_cryptoconditions/version.py
+-rw-r--r--   0        0        0     1548 2023-06-13 13:14:59.073047 planetmint_cryptoconditions-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0     3073 1970-01-01 00:00:00.000000 planetmint_cryptoconditions-1.2.2/PKG-INFO
```

### Comparing `planetmint_cryptoconditions-1.2.1/LICENSE` & `planetmint_cryptoconditions-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `planetmint_cryptoconditions-1.2.1/README.rst` & `planetmint_cryptoconditions-1.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `planetmint_cryptoconditions-1.2.1/planetmint_cryptoconditions/__init__.py` & `planetmint_cryptoconditions-1.2.2/planetmint_cryptoconditions/__init__.py`

 * *Files identical despite different names*

### Comparing `planetmint_cryptoconditions-1.2.1/planetmint_cryptoconditions/condition.py` & `planetmint_cryptoconditions-1.2.2/planetmint_cryptoconditions/condition.py`

 * *Files identical despite different names*

### Comparing `planetmint_cryptoconditions-1.2.1/planetmint_cryptoconditions/crypto.py` & `planetmint_cryptoconditions-1.2.2/planetmint_cryptoconditions/crypto.py`

 * *Files identical despite different names*

### Comparing `planetmint_cryptoconditions-1.2.1/planetmint_cryptoconditions/exceptions.py` & `planetmint_cryptoconditions-1.2.2/planetmint_cryptoconditions/exceptions.py`

 * *Files identical despite different names*

### Comparing `planetmint_cryptoconditions-1.2.1/planetmint_cryptoconditions/fulfillment.py` & `planetmint_cryptoconditions-1.2.2/planetmint_cryptoconditions/fulfillment.py`

 * *Files identical despite different names*

### Comparing `planetmint_cryptoconditions-1.2.1/planetmint_cryptoconditions/schemas/condition.py` & `planetmint_cryptoconditions-1.2.2/planetmint_cryptoconditions/schemas/condition.py`

 * *Files identical despite different names*

### Comparing `planetmint_cryptoconditions-1.2.1/planetmint_cryptoconditions/schemas/fingerprint.py` & `planetmint_cryptoconditions-1.2.2/planetmint_cryptoconditions/schemas/fingerprint.py`

 * *Files identical despite different names*

### Comparing `planetmint_cryptoconditions-1.2.1/planetmint_cryptoconditions/schemas/fulfillment.py` & `planetmint_cryptoconditions-1.2.2/planetmint_cryptoconditions/schemas/fulfillment.py`

 * *Files identical despite different names*

### Comparing `planetmint_cryptoconditions-1.2.1/planetmint_cryptoconditions/type_registry.py` & `planetmint_cryptoconditions-1.2.2/planetmint_cryptoconditions/type_registry.py`

 * *Files identical despite different names*

### Comparing `planetmint_cryptoconditions-1.2.1/planetmint_cryptoconditions/types/ed25519.py` & `planetmint_cryptoconditions-1.2.2/planetmint_cryptoconditions/types/ed25519.py`

 * *Files identical despite different names*

### Comparing `planetmint_cryptoconditions-1.2.1/planetmint_cryptoconditions/types/prefix.py` & `planetmint_cryptoconditions-1.2.2/planetmint_cryptoconditions/types/prefix.py`

 * *Files identical despite different names*

### Comparing `planetmint_cryptoconditions-1.2.1/planetmint_cryptoconditions/types/preimage.py` & `planetmint_cryptoconditions-1.2.2/planetmint_cryptoconditions/types/preimage.py`

 * *Files identical despite different names*

### Comparing `planetmint_cryptoconditions-1.2.1/planetmint_cryptoconditions/types/rsa.py` & `planetmint_cryptoconditions-1.2.2/planetmint_cryptoconditions/types/rsa.py`

 * *Files identical despite different names*

### Comparing `planetmint_cryptoconditions-1.2.1/planetmint_cryptoconditions/types/threshold.py` & `planetmint_cryptoconditions-1.2.2/planetmint_cryptoconditions/types/threshold.py`

 * *Files identical despite different names*

### Comparing `planetmint_cryptoconditions-1.2.1/pyproject.toml` & `planetmint_cryptoconditions-1.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "planetmint-cryptoconditions"
-version = "1.2.1"
+version = "1.2.2"
 description = "Multi-algorithm, multi-level, multi-signature format for expressing conditions and fulfillments according to the Interledger Protocol (ILP)."
 authors = ["Cryptoconditions contributors <contact@ipdb.global>"]
 readme = "README.rst"
 keywords = ["cryptoconditions", "interledger", "merkle tree", "ed25519", "threshold signatures", "hash lock"]
 repository = "https://github.com/planetmint/cryptoconditions/"
 license = "MIT"
 classifiers=[
@@ -22,30 +22,30 @@
 exclude = ["tests*", "examples"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 base58 = "2.1.1"
 PyNaCl = "1.4.0"
 pyasn1 = "0.4.8"
-cryptography = "39.0.1"
+cryptography = "^41.0.1"
 setuptools = "^67.2.0"
 
 
 
 [tool.poetry.group.dev.dependencies]
 ipdb = "^0.13.9"
 ipython = "^8.5.0"
 coverage = "^6.4.4"
 hypothesis = "^6.54.5"
 pep8 = "^1.7.1"
 pyflakes = "^2.5.0"
 pylint = "^2.15.2"
 pytest = "^7.2.0"
 pytest-cov = "^3.0.0"
-pytest-xdist = "^2.5.0"
+pytest-xdist = "^3.3.1"
 recommonmark = ">=0.4.0"
 Sphinx = ">=1.3.5"
 sphinxcontrib-napoleon = ">=0.4.4"
 sphinx-press-theme = "0.8.0"
 black = "23.1.0"
```

### Comparing `planetmint_cryptoconditions-1.2.1/PKG-INFO` & `planetmint_cryptoconditions-1.2.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: planetmint-cryptoconditions
-Version: 1.2.1
+Version: 1.2.2
 Summary: Multi-algorithm, multi-level, multi-signature format for expressing conditions and fulfillments according to the Interledger Protocol (ILP).
 Home-page: https://github.com/planetmint/cryptoconditions/
 License: MIT
 Keywords: cryptoconditions,interledger,merkle tree,ed25519,threshold signatures,hash lock
 Author: Cryptoconditions contributors
 Author-email: contact@ipdb.global
 Requires-Python: >=3.9,<4.0
@@ -14,21 +14,20 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Database
 Classifier: Topic :: Database :: Database Engines/Servers
 Classifier: Topic :: Software Development
 Requires-Dist: PyNaCl (==1.4.0)
 Requires-Dist: base58 (==2.1.1)
-Requires-Dist: cryptography (==39.0.1)
+Requires-Dist: cryptography (>=41.0.1,<42.0.0)
 Requires-Dist: pyasn1 (==0.4.8)
 Requires-Dist: setuptools (>=67.2.0,<68.0.0)
 Project-URL: Repository, https://github.com/planetmint/cryptoconditions/
 Description-Content-Type: text/x-rst
 
 .. image:: https://badge.fury.io/py/planetmint-cryptoconditions.svg
         :target: https://badge.fury.io/py/planetmint-cryptoconditions
```

