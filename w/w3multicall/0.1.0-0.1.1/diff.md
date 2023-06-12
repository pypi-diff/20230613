# Comparing `tmp/w3multicall-0.1.0.tar.gz` & `tmp/w3multicall-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "w3multicall-0.1.0.tar", last modified: Mon Jun 12 15:11:45 2023, max compression
+gzip compressed data, was "w3multicall-0.1.1.tar", last modified: Mon Jun 12 23:15:09 2023, max compression
```

## Comparing `w3multicall-0.1.0.tar` & `w3multicall-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-06-12 15:11:45.979601 w3multicall-0.1.0/
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     1098 2022-07-17 06:13:39.000000 w3multicall-0.1.0/LICENSE
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     5221 2023-06-12 15:11:45.979601 w3multicall-0.1.0/PKG-INFO
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     3513 2023-06-12 15:08:40.000000 w3multicall-0.1.0/README.md
--rw-rw-r--   0 ortis     (1000) ortis     (1000)      599 2023-06-12 15:11:39.000000 w3multicall-0.1.0/pyproject.toml
--rw-rw-r--   0 ortis     (1000) ortis     (1000)      624 2023-06-12 15:11:45.979601 w3multicall-0.1.0/setup.cfg
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-06-12 15:11:45.979601 w3multicall-0.1.0/src/
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-06-12 15:11:45.979601 w3multicall-0.1.0/src/w3multicall/
--rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2023-06-11 13:17:07.000000 w3multicall-0.1.0/src/w3multicall/__init__.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     5624 2023-06-12 13:12:08.000000 w3multicall-0.1.0/src/w3multicall/multicall.py
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-06-12 15:11:45.979601 w3multicall-0.1.0/src/w3multicall/threading/
--rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2023-06-12 13:16:33.000000 w3multicall-0.1.0/src/w3multicall/threading/__init__.py
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     6207 2023-06-12 15:07:37.000000 w3multicall-0.1.0/src/w3multicall/threading/w3multicall_executor.py
-drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-06-12 15:11:45.979601 w3multicall-0.1.0/src/w3multicall.egg-info/
--rw-rw-r--   0 ortis     (1000) ortis     (1000)     5221 2023-06-12 15:11:45.000000 w3multicall-0.1.0/src/w3multicall.egg-info/PKG-INFO
--rw-rw-r--   0 ortis     (1000) ortis     (1000)      381 2023-06-12 15:11:45.000000 w3multicall-0.1.0/src/w3multicall.egg-info/SOURCES.txt
--rw-rw-r--   0 ortis     (1000) ortis     (1000)        1 2023-06-12 15:11:45.000000 w3multicall-0.1.0/src/w3multicall.egg-info/dependency_links.txt
--rw-rw-r--   0 ortis     (1000) ortis     (1000)       60 2023-06-12 15:11:45.000000 w3multicall-0.1.0/src/w3multicall.egg-info/requires.txt
--rw-rw-r--   0 ortis     (1000) ortis     (1000)       12 2023-06-12 15:11:45.000000 w3multicall-0.1.0/src/w3multicall.egg-info/top_level.txt
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-06-12 23:15:09.922179 w3multicall-0.1.1/
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     1098 2022-07-17 06:13:39.000000 w3multicall-0.1.1/LICENSE
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     5235 2023-06-12 23:15:09.922179 w3multicall-0.1.1/PKG-INFO
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     3527 2023-06-12 23:14:46.000000 w3multicall-0.1.1/README.md
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)      599 2023-06-12 23:15:03.000000 w3multicall-0.1.1/pyproject.toml
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)      624 2023-06-12 23:15:09.922179 w3multicall-0.1.1/setup.cfg
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-06-12 23:15:09.922179 w3multicall-0.1.1/src/
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-06-12 23:15:09.922179 w3multicall-0.1.1/src/w3multicall/
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2023-06-11 13:17:07.000000 w3multicall-0.1.1/src/w3multicall/__init__.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     5883 2023-06-12 23:12:31.000000 w3multicall-0.1.1/src/w3multicall/multicall.py
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-06-12 23:15:09.922179 w3multicall-0.1.1/src/w3multicall/threading/
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)        0 2023-06-12 13:16:33.000000 w3multicall-0.1.1/src/w3multicall/threading/__init__.py
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     7263 2023-06-12 23:12:31.000000 w3multicall-0.1.1/src/w3multicall/threading/w3multicall_executor.py
+drwxrwxr-x   0 ortis     (1000) ortis     (1000)        0 2023-06-12 23:15:09.922179 w3multicall-0.1.1/src/w3multicall.egg-info/
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)     5235 2023-06-12 23:15:09.000000 w3multicall-0.1.1/src/w3multicall.egg-info/PKG-INFO
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)      381 2023-06-12 23:15:09.000000 w3multicall-0.1.1/src/w3multicall.egg-info/SOURCES.txt
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)        1 2023-06-12 23:15:09.000000 w3multicall-0.1.1/src/w3multicall.egg-info/dependency_links.txt
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)       60 2023-06-12 23:15:09.000000 w3multicall-0.1.1/src/w3multicall.egg-info/requires.txt
+-rw-rw-r--   0 ortis     (1000) ortis     (1000)       12 2023-06-12 23:15:09.000000 w3multicall-0.1.1/src/w3multicall.egg-info/top_level.txt
```

### Comparing `w3multicall-0.1.0/LICENSE` & `w3multicall-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `w3multicall-0.1.0/PKG-INFO` & `w3multicall-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: w3multicall
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python interface and utilities for Solidity multicall contract
 Home-page: https://github.com/0rtis/w3multicall
 Author: Ortis
 Author-email: Ortis <ortis@ortis.io>
 License: MIT License
         
         Copyright (c) 2022 Ortis (ortis@ortis.io)
@@ -35,15 +35,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 [![Pypi_repo](https://img.shields.io/pypi/v/w3multicall?style=flat-square)](https://pypi.org/project/w3multicall/)
 [![GitHub license](https://img.shields.io/github/license/0rtis/w3multicall.svg?style=flat-square)](https://github.com/0rtis/w3multicall/blob/master/LICENSE)
 [![GitHub stars](https://img.shields.io/github/stars/0rtis?style=flat-square)](https://github.com/0rtis)
-[![Follow @twitter handle](https://img.shields.io/twitter/follow/Knockturn_io.svg?style=flat-square)](https://twitter.com/intent/follow?screen_name=ortis95)
+[![Follow @twitter handle](https://img.shields.io/twitter/follow/Knockturn_io.svg?style=flat-square)](https://twitter.com/intent/follow?screen_name=Knockturn_io)
 
 
 Install with `pip install w3multicall`
 
 https://pypi.org/project/w3multicall/
 
 
@@ -56,15 +56,15 @@
 However, [multicall.py](https://github.com/banteg/multicall.py) is built on [asyncio](https://docs.python.org/3/library/asyncio.html) and
 [does not support multi-threading](https://github.com/banteg/multicall.py/issues/77)*
 
 This implementation fixes that.
 
 # Multicall Smart Contract
 [Multicall](https://github.com/mds1/multicall) smart contract are deployed on numerous chains and can help reduce the strain
-put on RPC by order of magnitude by *batching* multiple requests into one.
+put on RPC by order of magnitude by *batching* multiple requests into a single one.
 
 # Simple Multicall
 
 ```
 from web3 import Web3
 from w3multicall.multicall import W3Multicall
```

### Comparing `w3multicall-0.1.0/README.md` & `w3multicall-0.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 [![Pypi_repo](https://img.shields.io/pypi/v/w3multicall?style=flat-square)](https://pypi.org/project/w3multicall/)
 [![GitHub license](https://img.shields.io/github/license/0rtis/w3multicall.svg?style=flat-square)](https://github.com/0rtis/w3multicall/blob/master/LICENSE)
 [![GitHub stars](https://img.shields.io/github/stars/0rtis?style=flat-square)](https://github.com/0rtis)
-[![Follow @twitter handle](https://img.shields.io/twitter/follow/Knockturn_io.svg?style=flat-square)](https://twitter.com/intent/follow?screen_name=ortis95)
+[![Follow @twitter handle](https://img.shields.io/twitter/follow/Knockturn_io.svg?style=flat-square)](https://twitter.com/intent/follow?screen_name=Knockturn_io)
 
 
 Install with `pip install w3multicall`
 
 https://pypi.org/project/w3multicall/
 
 
@@ -19,15 +19,15 @@
 However, [multicall.py](https://github.com/banteg/multicall.py) is built on [asyncio](https://docs.python.org/3/library/asyncio.html) and
 [does not support multi-threading](https://github.com/banteg/multicall.py/issues/77)*
 
 This implementation fixes that.
 
 # Multicall Smart Contract
 [Multicall](https://github.com/mds1/multicall) smart contract are deployed on numerous chains and can help reduce the strain
-put on RPC by order of magnitude by *batching* multiple requests into one.
+put on RPC by order of magnitude by *batching* multiple requests into a single one.
 
 # Simple Multicall
 
 ```
 from web3 import Web3
 from w3multicall.multicall import W3Multicall
```

### Comparing `w3multicall-0.1.0/pyproject.toml` & `w3multicall-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["setuptools>=57"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "w3multicall"
 description = "Python interface and utilities for Solidity multicall contract"
 authors = [{name = "Ortis", email = "ortis@ortis.io"}]
-version = "0.1.0"
+version = "0.1.1"
 readme = "README.md"
 keywords = ["blockchain", "web3", "etherum", "solidity"]
 license = {file = "LICENSE"}
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
     "Programming Language :: Python :: 3",
```

### Comparing `w3multicall-0.1.0/setup.cfg` & `w3multicall-0.1.1/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = w3multicall
-version = 0.1.0
+version = 0.1.1
 author = Ortis
 author_email = ortis@ortis.io
 description = Python interface and utilities for Solidity multicall contract
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/0rtis/w3multicall
 project_urls =
```

### Comparing `w3multicall-0.1.0/src/w3multicall/multicall.py` & `w3multicall-0.1.1/src/w3multicall/multicall.py`

 * *Files 4% similar despite different names*

```diff
@@ -99,14 +99,18 @@
 
 
 def _unpack_aggregate_outputs(outputs: Any) -> Tuple[Tuple[Union[None, bool], bytes], ...]:
     return tuple((None, output) for output in outputs)
 
 
 class W3Multicall:
+    """
+    Interface for multicall3.sol contract
+    """
+
     MULTICALL_METHOD_NAME, MULTICALL_INPUT_TYPES, MULTICALL_OUTPUT_TYPES = _parse_signature("aggregate((address,bytes)[])(uint256,bytes[])")
     MULTICALL_SELECTOR = eth_utils.function_signature_to_4byte_selector(MULTICALL_METHOD_NAME)
 
     class Call:
         def __init__(self, address: str, signature: str, args=None):
             self.address = address
             self.signature = signature.replace(" ", "")
@@ -116,14 +120,19 @@
             else:
                 self.args = args
             self.name, self.input_types, self.output_types = _parse_signature(signature)
             self.selector = eth_utils.function_signature_to_4byte_selector(self.name)
             self.data = _encode_data(self.selector, self.input_types, self.args)
 
     def __init__(self, w3, address='0xcA11bde05977b3631167028862bE2a173976CA11', calls: List['W3Multicall.Call'] = None):
+        """
+        :param w3: Web3 instance
+        :param address: (optional) address of the multicall3.sol contract
+        :param calls: (optional) list of W3Multicall.Call to perform
+        """
         self.w3 = w3
         self.address = address
         self.calls: List['W3Multicall.Call'] = [] if calls is None else calls.copy()
         self.require_success = True
 
     def add(self, call: 'W3Multicall.Call'):
         self.calls.append(call)
```

### Comparing `w3multicall-0.1.0/src/w3multicall/threading/w3multicall_executor.py` & `w3multicall-0.1.1/src/w3multicall/threading/w3multicall_executor.py`

 * *Files 13% similar despite different names*

```diff
@@ -29,24 +29,36 @@
         return self.last_call_at + self.delay_between_call
 
     def usable_in(self):
         return self.usable_at() - time.time()
 
 
 class W3Pool:
+    """
+    Pool of W3 instances
+    """
 
     def __init__(self, w3s: List[W3], logger: Union[logging.Logger, None] = None):
+        """
+        :param w3s: list of W3 instances
+        :param logger: (optional) logging.Logger
+        """
         self.w3s = w3s
         self.logger = logger
 
     def add_w3(self, w3: W3) -> 'W3Pool':
         self.w3s.append(w3)
         return self
 
     def use(self, block: bool = True) -> Union[Web3, None]:
+        """
+        Return a Web3 instance that will not hit the rate limit upon calling (may block until the rate limit windows has passed)
+        :param block: (default: true) block until a Web3 instance is available
+        :return: Web3 instance
+        """
         next_available: Union[W3, None] = None
 
         for i in range(len(self.w3s)):
             tau = self.w3s[i].usable_in()
             if tau <= 0:
                 if self.logger is not None:
                     self.logger.debug("Using {}".format(self.w3s[i]))
@@ -66,14 +78,17 @@
             self.logger.debug("Using {}".format(next_available))
             return next_available.use()
         else:
             return None
 
 
 class W3MulticallExecutor:
+    """
+    Multi thread W3Multicall processor
+    """
 
     class Task:
         def __init__(self):
             self.sync = threading.Condition()
             self.creation_time = time.time()
             self.w3_calls: Dict[int, W3Multicall.Call] = {}
             self.w3_results = None
@@ -96,15 +111,24 @@
         def __init__(self, task: 'W3MulticallExecutor.Task', call_key: int):
             self.task = task
             self.call_key = call_key
 
         def get(self):
             return self.task.get(self.call_key)
 
-    def __init__(self, w3_pool: W3Pool, processes: int, multicall_contract_address = '0xcA11bde05977b3631167028862bE2a173976CA11', batch_max_size: int = 20, tick_duration: float = 0.05, logger: Union[logging.Logger, None] = None):
+    def __init__(self, w3_pool: W3Pool, processes: int, multicall_contract_address='0xcA11bde05977b3631167028862bE2a173976CA11', batch_max_size: int = 20, tick_duration: float = 0.05, logger: Union[logging.Logger, None] = None):
+        """
+        :param w3_pool: W3Pool
+        :param processes: number of thread to process W3Multicall
+        :param multicall_contract_address: (optional) address of the multicall3.sol contract
+        :param batch_max_size: (default 20) max call per W3Multicall
+        :param tick_duration: (default 0.05) update delay
+        :param logger: (optional) logging.Logger
+        """
+
         self.w3_pool = w3_pool
         self.processes = processes
         self.multicall_contract_address = multicall_contract_address
         self.batch_max_size = batch_max_size
         self.tick_duration = tick_duration
         self.logger = logger
         self.pending_task: Union[W3MulticallExecutor.Task, None] = None
@@ -125,15 +149,15 @@
     def __check_pending_task(self):
         with self.lock:
             if self.pending_task is not None and (time.time() >= self.pending_task.creation_time + self.tick_duration or len(self.pending_task.w3_calls) >= self.batch_max_size):
                 if self.logger is not None:
                     self.logger.debug("Triggering task {}".format(self.pending_task))
                 task = self.pending_task
                 self.pending_task = None
-                self.thread_pool.apply_async(func=self.__execute, args=(task, ))
+                self.thread_pool.apply_async(func=self.__execute, args=(task,))
 
     def __execute(self, task: 'W3MulticallExecutor.Task'):
         if self.logger is not None:
             self.logger.debug("Executing task {}".format(task))
         w3m = W3Multicall(self.w3_pool.use(), self.multicall_contract_address)
         for k in task.w3_calls:
             w3m.add(task.w3_calls[k])
@@ -151,14 +175,19 @@
                 task.exception = e
             finally:
                 task.sync.notify_all()
         if self.logger is not None:
             self.logger.debug("Task {} completed".format(task))
 
     def submit(self, call: W3Multicall.Call) -> Future:
+        """
+        Submit a W3Multicall.Call for execution
+        :param call: call to execute
+        :return: Future instance. Use Future.get() to wait until the call is executed
+        """
         with self.lock:
             if self.pending_task is None:
                 self.pending_task = W3MulticallExecutor.Task()
             call_key = len(self.pending_task.w3_calls)
             self.pending_task.w3_calls[call_key] = call
             task = self.pending_task
             self.__check_pending_task()
```

### Comparing `w3multicall-0.1.0/src/w3multicall.egg-info/PKG-INFO` & `w3multicall-0.1.1/src/w3multicall.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: w3multicall
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python interface and utilities for Solidity multicall contract
 Home-page: https://github.com/0rtis/w3multicall
 Author: Ortis
 Author-email: Ortis <ortis@ortis.io>
 License: MIT License
         
         Copyright (c) 2022 Ortis (ortis@ortis.io)
@@ -35,15 +35,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 [![Pypi_repo](https://img.shields.io/pypi/v/w3multicall?style=flat-square)](https://pypi.org/project/w3multicall/)
 [![GitHub license](https://img.shields.io/github/license/0rtis/w3multicall.svg?style=flat-square)](https://github.com/0rtis/w3multicall/blob/master/LICENSE)
 [![GitHub stars](https://img.shields.io/github/stars/0rtis?style=flat-square)](https://github.com/0rtis)
-[![Follow @twitter handle](https://img.shields.io/twitter/follow/Knockturn_io.svg?style=flat-square)](https://twitter.com/intent/follow?screen_name=ortis95)
+[![Follow @twitter handle](https://img.shields.io/twitter/follow/Knockturn_io.svg?style=flat-square)](https://twitter.com/intent/follow?screen_name=Knockturn_io)
 
 
 Install with `pip install w3multicall`
 
 https://pypi.org/project/w3multicall/
 
 
@@ -56,15 +56,15 @@
 However, [multicall.py](https://github.com/banteg/multicall.py) is built on [asyncio](https://docs.python.org/3/library/asyncio.html) and
 [does not support multi-threading](https://github.com/banteg/multicall.py/issues/77)*
 
 This implementation fixes that.
 
 # Multicall Smart Contract
 [Multicall](https://github.com/mds1/multicall) smart contract are deployed on numerous chains and can help reduce the strain
-put on RPC by order of magnitude by *batching* multiple requests into one.
+put on RPC by order of magnitude by *batching* multiple requests into a single one.
 
 # Simple Multicall
 
 ```
 from web3 import Web3
 from w3multicall.multicall import W3Multicall
```

