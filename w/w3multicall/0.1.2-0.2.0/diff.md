# Comparing `tmp/w3multicall-0.1.2.tar.gz` & `tmp/w3multicall-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "w3multicall-0.1.2.tar", last modified: Tue Jun 13 03:37:33 2023, max compression
+gzip compressed data, was "w3multicall-0.2.0.tar", last modified: Tue Jun 13 04:32:37 2023, max compression
```

## Comparing `w3multicall-0.1.2.tar` & `w3multicall-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,22 @@
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-06-13 03:37:33.033415 w3multicall-0.1.2/
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     1098 2022-07-17 06:13:39.000000 w3multicall-0.1.2/LICENSE
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     5253 2023-06-13 03:37:33.033415 w3multicall-0.1.2/PKG-INFO
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     3547 2023-06-12 23:24:10.000000 w3multicall-0.1.2/README.md
--rw-rw-r--   0 ortis     (1000) ortis     (1000)      599 2023-06-13 03:37:20.000000 w3multicall-0.1.2/pyproject.toml
--rw-rw-r--   0 ortis     (1000) ortis     (1000)      624 2023-06-13 03:37:33.033415 w3multicall-0.1.2/setup.cfg
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-06-13 03:37:33.033415 w3multicall-0.1.2/src/
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-06-13 03:37:33.033415 w3multicall-0.1.2/src/w3multicall/
--rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2023-06-11 13:17:07.000000 w3multicall-0.1.2/src/w3multicall/__init__.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     6256 2023-06-13 01:16:16.000000 w3multicall-0.1.2/src/w3multicall/multicall.py
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-06-13 03:37:33.033415 w3multicall-0.1.2/src/w3multicall/threading/
--rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2023-06-12 13:16:33.000000 w3multicall-0.1.2/src/w3multicall/threading/__init__.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     7357 2023-06-13 03:37:20.000000 w3multicall-0.1.2/src/w3multicall/threading/w3multicall_executor.py
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-06-13 03:37:33.033415 w3multicall-0.1.2/src/w3multicall.egg-info/
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     5253 2023-06-13 03:37:33.000000 w3multicall-0.1.2/src/w3multicall.egg-info/PKG-INFO
--rw-rw-r--   0 ortis     (1000) ortis     (1000)      381 2023-06-13 03:37:33.000000 w3multicall-0.1.2/src/w3multicall.egg-info/SOURCES.txt
--rw-rw-r--   0 ortis     (1000) ortis     (1000)        1 2023-06-13 03:37:33.000000 w3multicall-0.1.2/src/w3multicall.egg-info/dependency_links.txt
--rw-rw-r--   0 ortis     (1000) ortis     (1000)       60 2023-06-13 03:37:33.000000 w3multicall-0.1.2/src/w3multicall.egg-info/requires.txt
--rw-rw-r--   0 ortis     (1000) ortis     (1000)       12 2023-06-13 03:37:33.000000 w3multicall-0.1.2/src/w3multicall.egg-info/top_level.txt
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-06-13 04:32:37.209878 w3multicall-0.2.0/
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     1098 2022-07-17 06:13:39.000000 w3multicall-0.2.0/LICENSE
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     5407 2023-06-13 04:32:37.209878 w3multicall-0.2.0/PKG-INFO
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     3704 2023-06-13 04:30:27.000000 w3multicall-0.2.0/README.md
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)      599 2023-06-13 04:32:06.000000 w3multicall-0.2.0/pyproject.toml
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)      624 2023-06-13 04:32:37.209878 w3multicall-0.2.0/setup.cfg
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-06-13 04:32:37.205881 w3multicall-0.2.0/src/
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-06-13 04:32:37.209878 w3multicall-0.2.0/src/w3multicall/
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2023-06-11 13:17:07.000000 w3multicall-0.2.0/src/w3multicall/__init__.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     6256 2023-06-13 01:16:16.000000 w3multicall-0.2.0/src/w3multicall/multicall.py
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-06-13 04:32:37.209878 w3multicall-0.2.0/src/w3multicall/threading/
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2023-06-12 13:16:33.000000 w3multicall-0.2.0/src/w3multicall/threading/__init__.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     5034 2023-06-13 04:23:57.000000 w3multicall-0.2.0/src/w3multicall/threading/w3multicall_executor.py
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-06-13 04:32:37.209878 w3multicall-0.2.0/src/w3multicall/web3/
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2023-06-13 04:22:07.000000 w3multicall-0.2.0/src/w3multicall/web3/__init__.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     2442 2023-06-13 04:28:32.000000 w3multicall-0.2.0/src/w3multicall/web3/web3.py
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-06-13 04:32:37.209878 w3multicall-0.2.0/src/w3multicall.egg-info/
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     5407 2023-06-13 04:32:37.000000 w3multicall-0.2.0/src/w3multicall.egg-info/PKG-INFO
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)      443 2023-06-13 04:32:37.000000 w3multicall-0.2.0/src/w3multicall.egg-info/SOURCES.txt
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)        1 2023-06-13 04:32:37.000000 w3multicall-0.2.0/src/w3multicall.egg-info/dependency_links.txt
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)       60 2023-06-13 04:32:37.000000 w3multicall-0.2.0/src/w3multicall.egg-info/requires.txt
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)       12 2023-06-13 04:32:37.000000 w3multicall-0.2.0/src/w3multicall.egg-info/top_level.txt
```

### Comparing `w3multicall-0.1.2/LICENSE` & `w3multicall-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `w3multicall-0.1.2/PKG-INFO` & `w3multicall-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: w3multicall
-Version: 0.1.2
+Version: 0.2.0
 Summary: Python interface and utilities for Solidity multicall contract
 Home-page: https://github.com/0rtis/w3multicall
 Author: Ortis
 Author-email: Ortis <ortis@ortis.io>
 License: MIT License
         
         Copyright (c) 2022 Ortis (ortis@ortis.io)
@@ -56,14 +56,17 @@
 However, [multicall.py](https://github.com/banteg/multicall.py) is built on [asyncio](https://docs.python.org/3/library/asyncio.html) and
 [does not support multi-threading](https://github.com/banteg/multicall.py/issues/77)*
 
 This implementation fixes that.
 
 # W3Multicall
 
+## Build and install locally
+From the root folder `web3multicall` do `pip install .` to build and install the package in the current python environment 
+
 ## Multicall Smart Contract
 [Multicall](https://github.com/mds1/multicall) smart contract are deployed on numerous chains and can help reduce the strain
 put on RPC by order of magnitude by *batching* multiple requests into a single one.
 
 ## Simple Multicall
 
 ```
```

### Comparing `w3multicall-0.1.2/README.md` & `w3multicall-0.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,17 @@
 However, [multicall.py](https://github.com/banteg/multicall.py) is built on [asyncio](https://docs.python.org/3/library/asyncio.html) and
 [does not support multi-threading](https://github.com/banteg/multicall.py/issues/77)*
 
 This implementation fixes that.
 
 # W3Multicall
 
+## Build and install locally
+From the root folder `web3multicall` do `pip install .` to build and install the package in the current python environment 
+
 ## Multicall Smart Contract
 [Multicall](https://github.com/mds1/multicall) smart contract are deployed on numerous chains and can help reduce the strain
 put on RPC by order of magnitude by *batching* multiple requests into a single one.
 
 ## Simple Multicall
 
 ```
```

### Comparing `w3multicall-0.1.2/pyproject.toml` & `w3multicall-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["setuptools>=57"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "w3multicall"
 description = "Python interface and utilities for Solidity multicall contract"
 authors = [{name = "Ortis", email = "ortis@ortis.io"}]
-version = "0.1.2"
+version = "0.2.0"
 readme = "README.md"
 keywords = ["blockchain", "web3", "etherum", "solidity"]
 license = {file = "LICENSE"}
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
     "Programming Language :: Python :: 3",
```

### Comparing `w3multicall-0.1.2/setup.cfg` & `w3multicall-0.2.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = w3multicall
-version = 0.1.2
+version = 0.2.0
 author = Ortis
 author_email = ortis@ortis.io
 description = Python interface and utilities for Solidity multicall contract
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/0rtis/w3multicall
 project_urls =
```

### Comparing `w3multicall-0.1.2/src/w3multicall/multicall.py` & `w3multicall-0.2.0/src/w3multicall/multicall.py`

 * *Files identical despite different names*

### Comparing `w3multicall-0.1.2/src/w3multicall/threading/w3multicall_executor.py` & `w3multicall-0.2.0/src/w3multicall/threading/w3multicall_executor.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,89 +1,16 @@
 from typing import List, Dict, Union, Callable
 import logging
 import threading
 from multiprocessing.pool import ThreadPool
 import time
 import datetime
 
-from web3 import Web3
-
 from ..multicall import W3Multicall
-
-
-class W3:
-
-    def __init__(self, w3: Web3, delay_between_call: float, label: Union[str, None] = None):
-        self.w3 = w3
-        self.delay_between_call = delay_between_call
-        self.limit_rate_per_seconds = 1 / self.delay_between_call
-        self.last_call_at = 0
-        self.label = str(self) if label is None else label
-
-    def __repr__(self):
-        return '{} {:.2f}/s'.format(self.label, self.limit_rate_per_seconds)
-
-    def use(self) -> Web3:
-        self.last_call_at = time.time()
-        return self.w3
-
-    def usable_at(self):
-        return self.last_call_at + self.delay_between_call
-
-    def usable_in(self):
-        return self.usable_at() - time.time()
-
-
-class W3Pool:
-    """
-    Pool of W3 instances
-    """
-
-    def __init__(self, w3s: List[W3], logger: Union[logging.Logger, None] = None):
-        """
-        :param w3s: list of W3 instances
-        :param logger: (optional) logging.Logger
-        """
-        self.w3s = w3s
-        self.logger = logger
-
-    def add_w3(self, w3: W3) -> 'W3Pool':
-        self.w3s.append(w3)
-        return self
-
-    def use(self, block: bool = True) -> Union[Web3, None]:
-        """
-        Return a Web3 instance that will not hit the rate limit upon calling (may block until the rate limit windows has passed)
-        :param block: (default: true) block until a Web3 instance is available
-        :return: Web3 instance
-        """
-        next_available: Union[W3, None] = None
-
-        for i in range(len(self.w3s)):
-            tau = self.w3s[i].usable_in()
-            if tau <= 0:
-                if self.logger is not None:
-                    self.logger.debug("Using {}".format(self.w3s[i]))
-                return self.w3s[i].use()
-            if next_available is None or tau < next_available.usable_in():
-                next_available = self.w3s[i]
-
-        if next_available is None:
-            raise Exception("No Web3 instance found")
-
-        if block:
-            sleep = next_available.usable_in()
-            if sleep > 0:
-                if self.logger is not None:
-                    self.logger.warning("Waiting {}s for {}".format(sleep, next_available))
-                time.sleep(sleep)
-            self.logger.debug("Using {}".format(next_available))
-            return next_available.use()
-        else:
-            return None
+from ..web3.web3 import W3Pool
 
 
 class W3MulticallExecutor:
     """
     Multi thread W3Multicall processor
     """
```

### Comparing `w3multicall-0.1.2/src/w3multicall.egg-info/PKG-INFO` & `w3multicall-0.2.0/src/w3multicall.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: w3multicall
-Version: 0.1.2
+Version: 0.2.0
 Summary: Python interface and utilities for Solidity multicall contract
 Home-page: https://github.com/0rtis/w3multicall
 Author: Ortis
 Author-email: Ortis <ortis@ortis.io>
 License: MIT License
         
         Copyright (c) 2022 Ortis (ortis@ortis.io)
@@ -56,14 +56,17 @@
 However, [multicall.py](https://github.com/banteg/multicall.py) is built on [asyncio](https://docs.python.org/3/library/asyncio.html) and
 [does not support multi-threading](https://github.com/banteg/multicall.py/issues/77)*
 
 This implementation fixes that.
 
 # W3Multicall
 
+## Build and install locally
+From the root folder `web3multicall` do `pip install .` to build and install the package in the current python environment 
+
 ## Multicall Smart Contract
 [Multicall](https://github.com/mds1/multicall) smart contract are deployed on numerous chains and can help reduce the strain
 put on RPC by order of magnitude by *batching* multiple requests into a single one.
 
 ## Simple Multicall
 
 ```
```

