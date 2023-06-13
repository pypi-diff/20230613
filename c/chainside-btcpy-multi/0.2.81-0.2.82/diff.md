# Comparing `tmp/chainside-btcpy-multi-0.2.81.tar.gz` & `tmp/chainside-btcpy-multi-0.2.82.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chainside-btcpy-multi-0.2.81.tar", last modified: Tue Feb  1 09:39:21 2022, max compression
+gzip compressed data, was "chainside-btcpy-multi-0.2.82.tar", last modified: Tue Jun 13 09:35:45 2023, max compression
```

## Comparing `chainside-btcpy-multi-0.2.81.tar` & `chainside-btcpy-multi-0.2.82.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxrwxr-x   0 oskar     (1000) oskar     (1000)        0 2022-02-01 09:39:21.070762 chainside-btcpy-multi-0.2.81/
--rw-rw-r--   0 oskar     (1000) oskar     (1000)      517 2022-02-01 09:39:21.070762 chainside-btcpy-multi-0.2.81/PKG-INFO
--rw-rw-r--   0 oskar     (1000) oskar     (1000)    35627 2022-02-01 09:38:40.000000 chainside-btcpy-multi-0.2.81/README.md
-drwxrwxr-x   0 oskar     (1000) oskar     (1000)        0 2022-02-01 09:39:21.066764 chainside-btcpy-multi-0.2.81/btcpy/
--rw-rw-r--   0 oskar     (1000) oskar     (1000)      570 2022-02-01 09:38:40.000000 chainside-btcpy-multi-0.2.81/btcpy/__init__.py
--rw-rw-r--   0 oskar     (1000) oskar     (1000)     6863 2022-02-01 09:38:40.000000 chainside-btcpy-multi-0.2.81/btcpy/constants.py
-drwxrwxr-x   0 oskar     (1000) oskar     (1000)        0 2022-02-01 09:39:21.070762 chainside-btcpy-multi-0.2.81/btcpy/lib/
--rw-rw-r--   0 oskar     (1000) oskar     (1000)      362 2022-02-01 09:38:40.000000 chainside-btcpy-multi-0.2.81/btcpy/lib/__init__.py
--rw-rw-r--   0 oskar     (1000) oskar     (1000)     2206 2022-02-01 09:38:40.000000 chainside-btcpy-multi-0.2.81/btcpy/lib/base58.py
--rw-rw-r--   0 oskar     (1000) oskar     (1000)     4356 2022-02-01 09:38:40.000000 chainside-btcpy-multi-0.2.81/btcpy/lib/bech32.py
--rw-rw-r--   0 oskar     (1000) oskar     (1000)     3764 2022-02-01 09:38:40.000000 chainside-btcpy-multi-0.2.81/btcpy/lib/codecs.py
--rw-rw-r--   0 oskar     (1000) oskar     (1000)     5394 2022-02-01 09:38:40.000000 chainside-btcpy-multi-0.2.81/btcpy/lib/opcodes.py
--rw-rw-r--   0 oskar     (1000) oskar     (1000)    13763 2022-02-01 09:38:40.000000 chainside-btcpy-multi-0.2.81/btcpy/lib/parsing.py
--rw-rw-r--   0 oskar     (1000) oskar     (1000)     2149 2022-02-01 09:38:40.000000 chainside-btcpy-multi-0.2.81/btcpy/lib/types.py
--rw-rw-r--   0 oskar     (1000) oskar     (1000)     1106 2022-02-01 09:38:40.000000 chainside-btcpy-multi-0.2.81/btcpy/setup.py
-drwxrwxr-x   0 oskar     (1000) oskar     (1000)        0 2022-02-01 09:39:21.070762 chainside-btcpy-multi-0.2.81/btcpy/structs/
--rw-rw-r--   0 oskar     (1000) oskar     (1000)      362 2022-02-01 09:38:40.000000 chainside-btcpy-multi-0.2.81/btcpy/structs/__init__.py
--rw-rw-r--   0 oskar     (1000) oskar     (1000)     2593 2022-02-01 09:38:40.000000 chainside-btcpy-multi-0.2.81/btcpy/structs/address.py
--rw-rw-r--   0 oskar     (1000) oskar     (1000)     3854 2022-02-01 09:38:40.000000 chainside-btcpy-multi-0.2.81/btcpy/structs/block.py
--rw-rw-r--   0 oskar     (1000) oskar     (1000)     8031 2022-02-01 09:38:40.000000 chainside-btcpy-multi-0.2.81/btcpy/structs/crypto.py
--rw-rw-r--   0 oskar     (1000) oskar     (1000)    10574 2022-02-01 09:38:40.000000 chainside-btcpy-multi-0.2.81/btcpy/structs/hd.py
--rw-rw-r--   0 oskar     (1000) oskar     (1000)    38783 2022-02-01 09:38:40.000000 chainside-btcpy-multi-0.2.81/btcpy/structs/script.py
--rw-rw-r--   0 oskar     (1000) oskar     (1000)     7816 2022-02-01 09:38:40.000000 chainside-btcpy-multi-0.2.81/btcpy/structs/sig.py
--rw-rw-r--   0 oskar     (1000) oskar     (1000)    28632 2022-02-01 09:38:40.000000 chainside-btcpy-multi-0.2.81/btcpy/structs/transaction.py
-drwxrwxr-x   0 oskar     (1000) oskar     (1000)        0 2022-02-01 09:39:21.070762 chainside-btcpy-multi-0.2.81/chainside_btcpy_multi.egg-info/
--rw-rw-r--   0 oskar     (1000) oskar     (1000)      517 2022-02-01 09:39:20.000000 chainside-btcpy-multi-0.2.81/chainside_btcpy_multi.egg-info/PKG-INFO
--rw-rw-r--   0 oskar     (1000) oskar     (1000)      743 2022-02-01 09:39:20.000000 chainside-btcpy-multi-0.2.81/chainside_btcpy_multi.egg-info/SOURCES.txt
--rw-rw-r--   0 oskar     (1000) oskar     (1000)        1 2022-02-01 09:39:20.000000 chainside-btcpy-multi-0.2.81/chainside_btcpy_multi.egg-info/dependency_links.txt
--rw-rw-r--   0 oskar     (1000) oskar     (1000)        1 2022-02-01 09:39:20.000000 chainside-btcpy-multi-0.2.81/chainside_btcpy_multi.egg-info/not-zip-safe
--rw-rw-r--   0 oskar     (1000) oskar     (1000)       58 2022-02-01 09:39:20.000000 chainside-btcpy-multi-0.2.81/chainside_btcpy_multi.egg-info/requires.txt
--rw-rw-r--   0 oskar     (1000) oskar     (1000)       12 2022-02-01 09:39:20.000000 chainside-btcpy-multi-0.2.81/chainside_btcpy_multi.egg-info/top_level.txt
--rw-rw-r--   0 oskar     (1000) oskar     (1000)       38 2022-02-01 09:39:21.070762 chainside-btcpy-multi-0.2.81/setup.cfg
--rw-rw-r--   0 oskar     (1000) oskar     (1000)     1098 2022-02-01 09:39:13.000000 chainside-btcpy-multi-0.2.81/setup.py
-drwxrwxr-x   0 oskar     (1000) oskar     (1000)        0 2022-02-01 09:39:21.070762 chainside-btcpy-multi-0.2.81/tests/
--rw-rw-r--   0 oskar     (1000) oskar     (1000)        0 2022-02-01 09:38:40.000000 chainside-btcpy-multi-0.2.81/tests/__init__.py
--rw-rw-r--   0 oskar     (1000) oskar     (1000)    22998 2022-02-01 09:38:40.000000 chainside-btcpy-multi-0.2.81/tests/integration.py
--rwxrwxr-x   0 oskar     (1000) oskar     (1000)     5223 2022-02-01 09:38:40.000000 chainside-btcpy-multi-0.2.81/tests/regtest.py
--rw-rw-r--   0 oskar     (1000) oskar     (1000)    46097 2022-02-01 09:38:40.000000 chainside-btcpy-multi-0.2.81/tests/unit.py
+drwxrwxr-x   0 ilker     (1001) ilker     (1001)        0 2023-06-13 09:35:45.940247 chainside-btcpy-multi-0.2.82/
+-rw-rw-r--   0 ilker     (1001) ilker     (1001)     7651 2022-08-23 14:53:30.000000 chainside-btcpy-multi-0.2.82/LICENSE
+-rw-rw-r--   0 ilker     (1001) ilker     (1001)      531 2023-06-13 09:35:45.940247 chainside-btcpy-multi-0.2.82/PKG-INFO
+-rw-rw-r--   0 ilker     (1001) ilker     (1001)    35627 2022-08-23 14:53:30.000000 chainside-btcpy-multi-0.2.82/README.md
+drwxrwxr-x   0 ilker     (1001) ilker     (1001)        0 2023-06-13 09:35:45.936247 chainside-btcpy-multi-0.2.82/btcpy/
+-rw-rw-r--   0 ilker     (1001) ilker     (1001)      570 2022-08-23 14:53:30.000000 chainside-btcpy-multi-0.2.82/btcpy/__init__.py
+-rw-rw-r--   0 ilker     (1001) ilker     (1001)     6863 2022-08-23 14:53:30.000000 chainside-btcpy-multi-0.2.82/btcpy/constants.py
+drwxrwxr-x   0 ilker     (1001) ilker     (1001)        0 2023-06-13 09:35:45.940247 chainside-btcpy-multi-0.2.82/btcpy/lib/
+-rw-rw-r--   0 ilker     (1001) ilker     (1001)      362 2022-08-23 14:53:30.000000 chainside-btcpy-multi-0.2.82/btcpy/lib/__init__.py
+-rw-rw-r--   0 ilker     (1001) ilker     (1001)     2206 2022-08-23 14:53:30.000000 chainside-btcpy-multi-0.2.82/btcpy/lib/base58.py
+-rw-rw-r--   0 ilker     (1001) ilker     (1001)     4356 2022-08-23 14:53:30.000000 chainside-btcpy-multi-0.2.82/btcpy/lib/bech32.py
+-rw-rw-r--   0 ilker     (1001) ilker     (1001)     3764 2022-08-23 14:53:30.000000 chainside-btcpy-multi-0.2.82/btcpy/lib/codecs.py
+-rw-rw-r--   0 ilker     (1001) ilker     (1001)     5394 2022-08-23 14:53:30.000000 chainside-btcpy-multi-0.2.82/btcpy/lib/opcodes.py
+-rw-rw-r--   0 ilker     (1001) ilker     (1001)    13763 2022-08-23 14:53:30.000000 chainside-btcpy-multi-0.2.82/btcpy/lib/parsing.py
+-rw-rw-r--   0 ilker     (1001) ilker     (1001)     2149 2022-08-23 14:53:30.000000 chainside-btcpy-multi-0.2.82/btcpy/lib/types.py
+-rw-rw-r--   0 ilker     (1001) ilker     (1001)     1106 2022-08-23 14:53:30.000000 chainside-btcpy-multi-0.2.82/btcpy/setup.py
+drwxrwxr-x   0 ilker     (1001) ilker     (1001)        0 2023-06-13 09:35:45.940247 chainside-btcpy-multi-0.2.82/btcpy/structs/
+-rw-rw-r--   0 ilker     (1001) ilker     (1001)      362 2022-08-23 14:53:30.000000 chainside-btcpy-multi-0.2.82/btcpy/structs/__init__.py
+-rw-rw-r--   0 ilker     (1001) ilker     (1001)     2593 2022-08-23 14:53:30.000000 chainside-btcpy-multi-0.2.82/btcpy/structs/address.py
+-rw-rw-r--   0 ilker     (1001) ilker     (1001)     3854 2022-08-23 14:53:30.000000 chainside-btcpy-multi-0.2.82/btcpy/structs/block.py
+-rw-rw-r--   0 ilker     (1001) ilker     (1001)     8031 2022-08-23 14:53:30.000000 chainside-btcpy-multi-0.2.82/btcpy/structs/crypto.py
+-rw-rw-r--   0 ilker     (1001) ilker     (1001)    10579 2023-06-12 14:09:41.000000 chainside-btcpy-multi-0.2.82/btcpy/structs/hd.py
+-rw-rw-r--   0 ilker     (1001) ilker     (1001)    38783 2022-08-23 14:53:30.000000 chainside-btcpy-multi-0.2.82/btcpy/structs/script.py
+-rw-rw-r--   0 ilker     (1001) ilker     (1001)     7816 2022-08-23 14:53:30.000000 chainside-btcpy-multi-0.2.82/btcpy/structs/sig.py
+-rw-rw-r--   0 ilker     (1001) ilker     (1001)    28632 2022-08-23 14:53:30.000000 chainside-btcpy-multi-0.2.82/btcpy/structs/transaction.py
+drwxrwxr-x   0 ilker     (1001) ilker     (1001)        0 2023-06-13 09:35:45.940247 chainside-btcpy-multi-0.2.82/chainside_btcpy_multi.egg-info/
+-rw-rw-r--   0 ilker     (1001) ilker     (1001)      531 2023-06-13 09:35:45.000000 chainside-btcpy-multi-0.2.82/chainside_btcpy_multi.egg-info/PKG-INFO
+-rw-rw-r--   0 ilker     (1001) ilker     (1001)      751 2023-06-13 09:35:45.000000 chainside-btcpy-multi-0.2.82/chainside_btcpy_multi.egg-info/SOURCES.txt
+-rw-rw-r--   0 ilker     (1001) ilker     (1001)        1 2023-06-13 09:35:45.000000 chainside-btcpy-multi-0.2.82/chainside_btcpy_multi.egg-info/dependency_links.txt
+-rw-rw-r--   0 ilker     (1001) ilker     (1001)        1 2023-06-13 09:35:45.000000 chainside-btcpy-multi-0.2.82/chainside_btcpy_multi.egg-info/not-zip-safe
+-rw-rw-r--   0 ilker     (1001) ilker     (1001)       58 2023-06-13 09:35:45.000000 chainside-btcpy-multi-0.2.82/chainside_btcpy_multi.egg-info/requires.txt
+-rw-rw-r--   0 ilker     (1001) ilker     (1001)       12 2023-06-13 09:35:45.000000 chainside-btcpy-multi-0.2.82/chainside_btcpy_multi.egg-info/top_level.txt
+-rw-rw-r--   0 ilker     (1001) ilker     (1001)       38 2023-06-13 09:35:45.940247 chainside-btcpy-multi-0.2.82/setup.cfg
+-rw-rw-r--   0 ilker     (1001) ilker     (1001)     1101 2023-06-13 09:30:27.000000 chainside-btcpy-multi-0.2.82/setup.py
+drwxrwxr-x   0 ilker     (1001) ilker     (1001)        0 2023-06-13 09:35:45.940247 chainside-btcpy-multi-0.2.82/tests/
+-rw-rw-r--   0 ilker     (1001) ilker     (1001)        0 2022-08-23 14:53:30.000000 chainside-btcpy-multi-0.2.82/tests/__init__.py
+-rw-rw-r--   0 ilker     (1001) ilker     (1001)    22998 2022-08-23 14:53:30.000000 chainside-btcpy-multi-0.2.82/tests/integration.py
+-rwxrwxr-x   0 ilker     (1001) ilker     (1001)     5223 2023-06-12 12:56:18.000000 chainside-btcpy-multi-0.2.82/tests/regtest.py
+-rw-rw-r--   0 ilker     (1001) ilker     (1001)    46097 2022-08-23 14:53:30.000000 chainside-btcpy-multi-0.2.82/tests/unit.py
```

### Comparing `chainside-btcpy-multi-0.2.81/PKG-INFO` & `chainside-btcpy-multi-0.2.82/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 Metadata-Version: 2.1
 Name: chainside-btcpy-multi
-Version: 0.2.81
+Version: 0.2.82
 Summary: A Python3 SegWit-compliant library which provides tools to handle Bitcoin data structures in a simple fashion.
-Home-page: https://github.com/chainside/btcpy
+Home-page: https://github.com/oskyk/btcpy
 Author: chainside srl
 Author-email: simone.bronzini@chainside.net
 License: UNKNOWN
-Download-URL: https://github.com/chainside/btcpy/archive/0.2.7.tar.gz
-Description: UNKNOWN
+Download-URL: https://github.com/oskyk/btcpy/archive/refs/tags/0.2.82.tar.gz
 Keywords: bitcoin,blockchain,bitcoind,chainside
 Platform: UNKNOWN
 Requires-Python: >=3
 Provides-Extra: develop
+License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `chainside-btcpy-multi-0.2.81/README.md` & `chainside-btcpy-multi-0.2.82/README.md`

 * *Files identical despite different names*

### Comparing `chainside-btcpy-multi-0.2.81/btcpy/__init__.py` & `chainside-btcpy-multi-0.2.82/btcpy/__init__.py`

 * *Files identical despite different names*

### Comparing `chainside-btcpy-multi-0.2.81/btcpy/constants.py` & `chainside-btcpy-multi-0.2.82/btcpy/constants.py`

 * *Files identical despite different names*

### Comparing `chainside-btcpy-multi-0.2.81/btcpy/lib/base58.py` & `chainside-btcpy-multi-0.2.82/btcpy/lib/base58.py`

 * *Files identical despite different names*

### Comparing `chainside-btcpy-multi-0.2.81/btcpy/lib/bech32.py` & `chainside-btcpy-multi-0.2.82/btcpy/lib/bech32.py`

 * *Files identical despite different names*

### Comparing `chainside-btcpy-multi-0.2.81/btcpy/lib/codecs.py` & `chainside-btcpy-multi-0.2.82/btcpy/lib/codecs.py`

 * *Files identical despite different names*

### Comparing `chainside-btcpy-multi-0.2.81/btcpy/lib/opcodes.py` & `chainside-btcpy-multi-0.2.82/btcpy/lib/opcodes.py`

 * *Files identical despite different names*

### Comparing `chainside-btcpy-multi-0.2.81/btcpy/lib/parsing.py` & `chainside-btcpy-multi-0.2.82/btcpy/lib/parsing.py`

 * *Files identical despite different names*

### Comparing `chainside-btcpy-multi-0.2.81/btcpy/lib/types.py` & `chainside-btcpy-multi-0.2.82/btcpy/lib/types.py`

 * *Files identical despite different names*

### Comparing `chainside-btcpy-multi-0.2.81/btcpy/setup.py` & `chainside-btcpy-multi-0.2.82/btcpy/setup.py`

 * *Files identical despite different names*

### Comparing `chainside-btcpy-multi-0.2.81/btcpy/structs/address.py` & `chainside-btcpy-multi-0.2.82/btcpy/structs/address.py`

 * *Files identical despite different names*

### Comparing `chainside-btcpy-multi-0.2.81/btcpy/structs/block.py` & `chainside-btcpy-multi-0.2.82/btcpy/structs/block.py`

 * *Files identical despite different names*

### Comparing `chainside-btcpy-multi-0.2.81/btcpy/structs/crypto.py` & `chainside-btcpy-multi-0.2.82/btcpy/structs/crypto.py`

 * *Files identical despite different names*

### Comparing `chainside-btcpy-multi-0.2.81/btcpy/structs/hd.py` & `chainside-btcpy-multi-0.2.82/btcpy/structs/hd.py`

 * *Files 0% similar despite different names*

```diff
@@ -207,15 +207,15 @@
         super().__init__(key, chaincode, depth, pfing, index, hardened)
 
     def __int__(self):
         return int.from_bytes(self.key.key, 'big')
     
     def get_child(self, index, hardened=False):
         left, right = self.get_hash(index, hardened)
-        k = (int(self) + left) % self.__class__.curve_order
+        k = int((int(self) + left) % self.__class__.curve_order)
         if k == 0:
             raise ValueError('Got 0 as k')
         return ExtendedPrivateKey(PrivateKey(k.to_bytes(32, 'big')),
                                   right,
                                   self.depth + 1,
                                   self.get_fingerprint(),
                                   index,
```

### Comparing `chainside-btcpy-multi-0.2.81/btcpy/structs/script.py` & `chainside-btcpy-multi-0.2.82/btcpy/structs/script.py`

 * *Files identical despite different names*

### Comparing `chainside-btcpy-multi-0.2.81/btcpy/structs/sig.py` & `chainside-btcpy-multi-0.2.82/btcpy/structs/sig.py`

 * *Files identical despite different names*

### Comparing `chainside-btcpy-multi-0.2.81/btcpy/structs/transaction.py` & `chainside-btcpy-multi-0.2.82/btcpy/structs/transaction.py`

 * *Files identical despite different names*

### Comparing `chainside-btcpy-multi-0.2.81/chainside_btcpy_multi.egg-info/PKG-INFO` & `chainside-btcpy-multi-0.2.82/chainside_btcpy_multi.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 Metadata-Version: 2.1
 Name: chainside-btcpy-multi
-Version: 0.2.81
+Version: 0.2.82
 Summary: A Python3 SegWit-compliant library which provides tools to handle Bitcoin data structures in a simple fashion.
-Home-page: https://github.com/chainside/btcpy
+Home-page: https://github.com/oskyk/btcpy
 Author: chainside srl
 Author-email: simone.bronzini@chainside.net
 License: UNKNOWN
-Download-URL: https://github.com/chainside/btcpy/archive/0.2.7.tar.gz
-Description: UNKNOWN
+Download-URL: https://github.com/oskyk/btcpy/archive/refs/tags/0.2.82.tar.gz
 Keywords: bitcoin,blockchain,bitcoind,chainside
 Platform: UNKNOWN
 Requires-Python: >=3
 Provides-Extra: develop
+License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `chainside-btcpy-multi-0.2.81/chainside_btcpy_multi.egg-info/SOURCES.txt` & `chainside-btcpy-multi-0.2.82/chainside_btcpy_multi.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 btcpy/__init__.py
 btcpy/constants.py
 btcpy/setup.py
 btcpy/lib/__init__.py
 btcpy/lib/base58.py
```

### Comparing `chainside-btcpy-multi-0.2.81/setup.py` & `chainside-btcpy-multi-0.2.82/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,19 +10,19 @@
 # LICENSE.md file.
 
 
 from distutils.core import setup
 from setuptools import find_packages
 
 setup(name='chainside-btcpy-multi',
-      version='0.2.81',
+      version='0.2.82',
       packages=find_packages(),
       install_requires=['ecdsa>=0.15.0,<0.16.0'],
       extras_require={'develop': ['python-bitcoinlib==0.7.0']},
       description='A Python3 SegWit-compliant library which provides tools to handle Bitcoin data structures in a simple fashion.',
       author='chainside srl',
       author_email='simone.bronzini@chainside.net',
-      url='https://github.com/chainside/btcpy',
-      download_url='https://github.com/chainside/btcpy/archive/0.2.7.tar.gz',
+      url='https://github.com/oskyk/btcpy',
+      download_url='https://github.com/oskyk/btcpy/archive/refs/tags/0.2.82.tar.gz',
       python_requires='>=3',
       keywords=['bitcoin', 'blockchain', 'bitcoind', 'chainside'],
       zip_safe=False)
```

### Comparing `chainside-btcpy-multi-0.2.81/tests/integration.py` & `chainside-btcpy-multi-0.2.82/tests/integration.py`

 * *Files identical despite different names*

### Comparing `chainside-btcpy-multi-0.2.81/tests/regtest.py` & `chainside-btcpy-multi-0.2.82/tests/regtest.py`

 * *Files identical despite different names*

### Comparing `chainside-btcpy-multi-0.2.81/tests/unit.py` & `chainside-btcpy-multi-0.2.82/tests/unit.py`

 * *Files identical despite different names*

