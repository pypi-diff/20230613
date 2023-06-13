# Comparing `tmp/w3multicall-0.1.1.tar.gz` & `tmp/w3multicall-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "w3multicall-0.1.1.tar", last modified: Mon Jun 12 23:15:09 2023, max compression
+gzip compressed data, was "w3multicall-0.1.2.tar", last modified: Tue Jun 13 03:37:33 2023, max compression
```

## Comparing `w3multicall-0.1.1.tar` & `w3multicall-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-06-12 23:15:09.922179 w3multicall-0.1.1/
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     1098 2022-07-17 06:13:39.000000 w3multicall-0.1.1/LICENSE
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     5235 2023-06-12 23:15:09.922179 w3multicall-0.1.1/PKG-INFO
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     3527 2023-06-12 23:14:46.000000 w3multicall-0.1.1/README.md
--rw-rw-r--   0 ortis     (1000) ortis     (1000)      599 2023-06-12 23:15:03.000000 w3multicall-0.1.1/pyproject.toml
--rw-rw-r--   0 ortis     (1000) ortis     (1000)      624 2023-06-12 23:15:09.922179 w3multicall-0.1.1/setup.cfg
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-06-12 23:15:09.922179 w3multicall-0.1.1/src/
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-06-12 23:15:09.922179 w3multicall-0.1.1/src/w3multicall/
--rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2023-06-11 13:17:07.000000 w3multicall-0.1.1/src/w3multicall/__init__.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     5883 2023-06-12 23:12:31.000000 w3multicall-0.1.1/src/w3multicall/multicall.py
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-06-12 23:15:09.922179 w3multicall-0.1.1/src/w3multicall/threading/
--rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2023-06-12 13:16:33.000000 w3multicall-0.1.1/src/w3multicall/threading/__init__.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     7263 2023-06-12 23:12:31.000000 w3multicall-0.1.1/src/w3multicall/threading/w3multicall_executor.py
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-06-12 23:15:09.922179 w3multicall-0.1.1/src/w3multicall.egg-info/
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     5235 2023-06-12 23:15:09.000000 w3multicall-0.1.1/src/w3multicall.egg-info/PKG-INFO
--rw-rw-r--   0 ortis     (1000) ortis     (1000)      381 2023-06-12 23:15:09.000000 w3multicall-0.1.1/src/w3multicall.egg-info/SOURCES.txt
--rw-rw-r--   0 ortis     (1000) ortis     (1000)        1 2023-06-12 23:15:09.000000 w3multicall-0.1.1/src/w3multicall.egg-info/dependency_links.txt
--rw-rw-r--   0 ortis     (1000) ortis     (1000)       60 2023-06-12 23:15:09.000000 w3multicall-0.1.1/src/w3multicall.egg-info/requires.txt
--rw-rw-r--   0 ortis     (1000) ortis     (1000)       12 2023-06-12 23:15:09.000000 w3multicall-0.1.1/src/w3multicall.egg-info/top_level.txt
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-06-13 03:37:33.033415 w3multicall-0.1.2/
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     1098 2022-07-17 06:13:39.000000 w3multicall-0.1.2/LICENSE
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     5253 2023-06-13 03:37:33.033415 w3multicall-0.1.2/PKG-INFO
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     3547 2023-06-12 23:24:10.000000 w3multicall-0.1.2/README.md
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)      599 2023-06-13 03:37:20.000000 w3multicall-0.1.2/pyproject.toml
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)      624 2023-06-13 03:37:33.033415 w3multicall-0.1.2/setup.cfg
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-06-13 03:37:33.033415 w3multicall-0.1.2/src/
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-06-13 03:37:33.033415 w3multicall-0.1.2/src/w3multicall/
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2023-06-11 13:17:07.000000 w3multicall-0.1.2/src/w3multicall/__init__.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     6256 2023-06-13 01:16:16.000000 w3multicall-0.1.2/src/w3multicall/multicall.py
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-06-13 03:37:33.033415 w3multicall-0.1.2/src/w3multicall/threading/
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2023-06-12 13:16:33.000000 w3multicall-0.1.2/src/w3multicall/threading/__init__.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     7357 2023-06-13 03:37:20.000000 w3multicall-0.1.2/src/w3multicall/threading/w3multicall_executor.py
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-06-13 03:37:33.033415 w3multicall-0.1.2/src/w3multicall.egg-info/
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     5253 2023-06-13 03:37:33.000000 w3multicall-0.1.2/src/w3multicall.egg-info/PKG-INFO
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)      381 2023-06-13 03:37:33.000000 w3multicall-0.1.2/src/w3multicall.egg-info/SOURCES.txt
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)        1 2023-06-13 03:37:33.000000 w3multicall-0.1.2/src/w3multicall.egg-info/dependency_links.txt
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)       60 2023-06-13 03:37:33.000000 w3multicall-0.1.2/src/w3multicall.egg-info/requires.txt
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)       12 2023-06-13 03:37:33.000000 w3multicall-0.1.2/src/w3multicall.egg-info/top_level.txt
```

### Comparing `w3multicall-0.1.1/LICENSE` & `w3multicall-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `w3multicall-0.1.1/PKG-INFO` & `w3multicall-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: w3multicall
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python interface and utilities for Solidity multicall contract
 Home-page: https://github.com/0rtis/w3multicall
 Author: Ortis
 Author-email: Ortis <ortis@ortis.io>
 License: MIT License
         
         Copyright (c) 2022 Ortis (ortis@ortis.io)
@@ -54,19 +54,21 @@
 
 *This software is derived from [multicall.py](https://github.com/banteg/multicall.py).
 However, [multicall.py](https://github.com/banteg/multicall.py) is built on [asyncio](https://docs.python.org/3/library/asyncio.html) and
 [does not support multi-threading](https://github.com/banteg/multicall.py/issues/77)*
 
 This implementation fixes that.
 
-# Multicall Smart Contract
+# W3Multicall
+
+## Multicall Smart Contract
 [Multicall](https://github.com/mds1/multicall) smart contract are deployed on numerous chains and can help reduce the strain
 put on RPC by order of magnitude by *batching* multiple requests into a single one.
 
-# Simple Multicall
+## Simple Multicall
 
 ```
 from web3 import Web3
 from w3multicall.multicall import W3Multicall
 
 w3 = Web3(Web3.HTTPProvider(rpc))
 
@@ -82,15 +84,15 @@
 
 print("Vitalik holds {:.2f} USDC".format(results[0]/10**6))
 
 ```
 
 [See full example](/examples/simple_multicall.py)
 
-# Multithread Multicall
+## Multithread Multicall
 
 ```
 w3_pool = W3Pool([
         W3(Web3(Web3.HTTPProvider('https://eth-rpc.gateway.pokt.network')), 5),
         W3(Web3(Web3.HTTPProvider('https://ethereum.publicnode.com')), 5),
         W3(Web3(Web3.HTTPProvider('https://rpc.flashbots.net/')), 5)
     ], logger)
```

### Comparing `w3multicall-0.1.1/README.md` & `w3multicall-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -17,19 +17,21 @@
 
 *This software is derived from [multicall.py](https://github.com/banteg/multicall.py).
 However, [multicall.py](https://github.com/banteg/multicall.py) is built on [asyncio](https://docs.python.org/3/library/asyncio.html) and
 [does not support multi-threading](https://github.com/banteg/multicall.py/issues/77)*
 
 This implementation fixes that.
 
-# Multicall Smart Contract
+# W3Multicall
+
+## Multicall Smart Contract
 [Multicall](https://github.com/mds1/multicall) smart contract are deployed on numerous chains and can help reduce the strain
 put on RPC by order of magnitude by *batching* multiple requests into a single one.
 
-# Simple Multicall
+## Simple Multicall
 
 ```
 from web3 import Web3
 from w3multicall.multicall import W3Multicall
 
 w3 = Web3(Web3.HTTPProvider(rpc))
 
@@ -45,15 +47,15 @@
 
 print("Vitalik holds {:.2f} USDC".format(results[0]/10**6))
 
 ```
 
 [See full example](/examples/simple_multicall.py)
 
-# Multithread Multicall
+## Multithread Multicall
 
 ```
 w3_pool = W3Pool([
         W3(Web3(Web3.HTTPProvider('https://eth-rpc.gateway.pokt.network')), 5),
         W3(Web3(Web3.HTTPProvider('https://ethereum.publicnode.com')), 5),
         W3(Web3(Web3.HTTPProvider('https://rpc.flashbots.net/')), 5)
     ], logger)
```

### Comparing `w3multicall-0.1.1/pyproject.toml` & `w3multicall-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["setuptools>=57"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "w3multicall"
 description = "Python interface and utilities for Solidity multicall contract"
 authors = [{name = "Ortis", email = "ortis@ortis.io"}]
-version = "0.1.1"
+version = "0.1.2"
 readme = "README.md"
 keywords = ["blockchain", "web3", "etherum", "solidity"]
 license = {file = "LICENSE"}
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
     "Programming Language :: Python :: 3",
```

### Comparing `w3multicall-0.1.1/setup.cfg` & `w3multicall-0.1.2/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = w3multicall
-version = 0.1.1
+version = 0.1.2
 author = Ortis
 author_email = ortis@ortis.io
 description = Python interface and utilities for Solidity multicall contract
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/0rtis/w3multicall
 project_urls =
```

### Comparing `w3multicall-0.1.1/src/w3multicall/multicall.py` & `w3multicall-0.1.2/src/w3multicall/multicall.py`

 * *Files 8% similar despite different names*

```diff
@@ -108,14 +108,19 @@
     """
 
     MULTICALL_METHOD_NAME, MULTICALL_INPUT_TYPES, MULTICALL_OUTPUT_TYPES = _parse_signature("aggregate((address,bytes)[])(uint256,bytes[])")
     MULTICALL_SELECTOR = eth_utils.function_signature_to_4byte_selector(MULTICALL_METHOD_NAME)
 
     class Call:
         def __init__(self, address: str, signature: str, args=None):
+            """
+            :param address: address of the contract to call
+            :param signature: method signature to call (no space. Example: 'balanceOf(address)(uint256)')
+            :param args: arguments of the contract method to call (use python tuple for solidity struct, python list for solidity arrays and python int for solidity uint/int)
+            """
             self.address = address
             self.signature = signature.replace(" ", "")
 
             if args is not None and not isinstance(args, list) and not isinstance(args, tuple):
                 self.args = (args,)
             else:
                 self.args = args
```

### Comparing `w3multicall-0.1.1/src/w3multicall/threading/w3multicall_executor.py` & `w3multicall-0.1.2/src/w3multicall/threading/w3multicall_executor.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,22 +8,23 @@
 from web3 import Web3
 
 from ..multicall import W3Multicall
 
 
 class W3:
 
-    def __init__(self, w3: Web3, delay_between_call: float):
+    def __init__(self, w3: Web3, delay_between_call: float, label: Union[str, None] = None):
         self.w3 = w3
         self.delay_between_call = delay_between_call
         self.limit_rate_per_seconds = 1 / self.delay_between_call
         self.last_call_at = 0
+        self.label = str(self) if label is None else label
 
     def __repr__(self):
-        return '{} {:.2f}/s'.format(self.w3, self.limit_rate_per_seconds)
+        return '{} {:.2f}/s'.format(self.label, self.limit_rate_per_seconds)
 
     def use(self) -> Web3:
         self.last_call_at = time.time()
         return self.w3
 
     def usable_at(self):
         return self.last_call_at + self.delay_between_call
```

### Comparing `w3multicall-0.1.1/src/w3multicall.egg-info/PKG-INFO` & `w3multicall-0.1.2/src/w3multicall.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: w3multicall
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python interface and utilities for Solidity multicall contract
 Home-page: https://github.com/0rtis/w3multicall
 Author: Ortis
 Author-email: Ortis <ortis@ortis.io>
 License: MIT License
         
         Copyright (c) 2022 Ortis (ortis@ortis.io)
@@ -54,19 +54,21 @@
 
 *This software is derived from [multicall.py](https://github.com/banteg/multicall.py).
 However, [multicall.py](https://github.com/banteg/multicall.py) is built on [asyncio](https://docs.python.org/3/library/asyncio.html) and
 [does not support multi-threading](https://github.com/banteg/multicall.py/issues/77)*
 
 This implementation fixes that.
 
-# Multicall Smart Contract
+# W3Multicall
+
+## Multicall Smart Contract
 [Multicall](https://github.com/mds1/multicall) smart contract are deployed on numerous chains and can help reduce the strain
 put on RPC by order of magnitude by *batching* multiple requests into a single one.
 
-# Simple Multicall
+## Simple Multicall
 
 ```
 from web3 import Web3
 from w3multicall.multicall import W3Multicall
 
 w3 = Web3(Web3.HTTPProvider(rpc))
 
@@ -82,15 +84,15 @@
 
 print("Vitalik holds {:.2f} USDC".format(results[0]/10**6))
 
 ```
 
 [See full example](/examples/simple_multicall.py)
 
-# Multithread Multicall
+## Multithread Multicall
 
 ```
 w3_pool = W3Pool([
         W3(Web3(Web3.HTTPProvider('https://eth-rpc.gateway.pokt.network')), 5),
         W3(Web3(Web3.HTTPProvider('https://ethereum.publicnode.com')), 5),
         W3(Web3(Web3.HTTPProvider('https://rpc.flashbots.net/')), 5)
     ], logger)
```

