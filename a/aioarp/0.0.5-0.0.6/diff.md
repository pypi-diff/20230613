# Comparing `tmp/aioarp-0.0.5.tar.gz` & `tmp/aioarp-0.0.6.tar.gz`

## Comparing `aioarp-0.0.5.tar` & `aioarp-0.0.6.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 aioarp-0.0.5/CHANGELOG.md
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 aioarp-0.0.5/requirements.txt
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 aioarp-0.0.5/unasync.py
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 aioarp-0.0.5/.github/workflows/main.yml
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 aioarp-0.0.5/.github/workflows/publish.yml
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 aioarp-0.0.5/aioarp/__about__.py
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 aioarp-0.0.5/aioarp/__init__.py
--rw-r--r--   0        0        0     4739 2020-02-02 00:00:00.000000 aioarp-0.0.5/aioarp/_arp.py
--rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 aioarp-0.0.5/aioarp/_async.py
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 aioarp-0.0.5/aioarp/_cli.py
--rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 aioarp-0.0.5/aioarp/_client.py
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 aioarp-0.0.5/aioarp/_exceptions.py
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 aioarp-0.0.5/aioarp/_mock.py
--rw-r--r--   0        0        0     1986 2020-02-02 00:00:00.000000 aioarp-0.0.5/aioarp/_sync.py
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 aioarp-0.0.5/aioarp/_utils.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 aioarp-0.0.5/aioarp/defaults.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 aioarp-0.0.5/aioarp/_backends/__init__.py
--rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 aioarp-0.0.5/aioarp/_backends/_async.py
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 aioarp-0.0.5/aioarp/_backends/_base.py
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 aioarp-0.0.5/aioarp/_backends/_mock.py
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 aioarp-0.0.5/aioarp/_backends/_sync.py
--rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 aioarp-0.0.5/scripts/check
--rwxr-xr-x   0        0        0       30 2020-02-02 00:00:00.000000 aioarp-0.0.5/scripts/lint
--rwxr-xr-x   0        0        0       60 2020-02-02 00:00:00.000000 aioarp-0.0.5/scripts/publish
--rwxr-xr-x   0        0        0      132 2020-02-02 00:00:00.000000 aioarp-0.0.5/scripts/test
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 aioarp-0.0.5/tests/__init__.py
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 aioarp-0.0.5/tests/conftest.py
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 aioarp-0.0.5/tests/test_async.py
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 aioarp-0.0.5/tests/test_client.py
--rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 aioarp-0.0.5/tests/test_proto.py
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 aioarp-0.0.5/tests/test_sync.py
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 aioarp-0.0.5/tests/test_utils.py
--rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 aioarp-0.0.5/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 aioarp-0.0.5/LICENSE.txt
--rw-r--r--   0        0        0     4834 2020-02-02 00:00:00.000000 aioarp-0.0.5/README.md
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 aioarp-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     6024 2020-02-02 00:00:00.000000 aioarp-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 aioarp-0.0.6/CHANGELOG.md
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 aioarp-0.0.6/requirements.txt
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 aioarp-0.0.6/unasync.py
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 aioarp-0.0.6/.github/workflows/main.yml
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 aioarp-0.0.6/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 aioarp-0.0.6/aioarp/__about__.py
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 aioarp-0.0.6/aioarp/__init__.py
+-rw-r--r--   0        0        0     4739 2020-02-02 00:00:00.000000 aioarp-0.0.6/aioarp/_arp.py
+-rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 aioarp-0.0.6/aioarp/_async.py
+-rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 aioarp-0.0.6/aioarp/_cli.py
+-rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 aioarp-0.0.6/aioarp/_client.py
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 aioarp-0.0.6/aioarp/_exceptions.py
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 aioarp-0.0.6/aioarp/_mock.py
+-rw-r--r--   0        0        0     1986 2020-02-02 00:00:00.000000 aioarp-0.0.6/aioarp/_sync.py
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 aioarp-0.0.6/aioarp/_utils.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 aioarp-0.0.6/aioarp/defaults.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 aioarp-0.0.6/aioarp/_backends/__init__.py
+-rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 aioarp-0.0.6/aioarp/_backends/_async.py
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 aioarp-0.0.6/aioarp/_backends/_base.py
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 aioarp-0.0.6/aioarp/_backends/_mock.py
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 aioarp-0.0.6/aioarp/_backends/_sync.py
+-rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 aioarp-0.0.6/scripts/check
+-rwxr-xr-x   0        0        0       30 2020-02-02 00:00:00.000000 aioarp-0.0.6/scripts/lint
+-rwxr-xr-x   0        0        0       60 2020-02-02 00:00:00.000000 aioarp-0.0.6/scripts/publish
+-rwxr-xr-x   0        0        0      132 2020-02-02 00:00:00.000000 aioarp-0.0.6/scripts/test
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 aioarp-0.0.6/tests/__init__.py
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 aioarp-0.0.6/tests/conftest.py
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 aioarp-0.0.6/tests/test_async.py
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 aioarp-0.0.6/tests/test_client.py
+-rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 aioarp-0.0.6/tests/test_proto.py
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 aioarp-0.0.6/tests/test_sync.py
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 aioarp-0.0.6/tests/test_utils.py
+-rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 aioarp-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 aioarp-0.0.6/LICENSE.txt
+-rw-r--r--   0        0        0     4834 2020-02-02 00:00:00.000000 aioarp-0.0.6/README.md
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 aioarp-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     6024 2020-02-02 00:00:00.000000 aioarp-0.0.6/PKG-INFO
```

### Comparing `aioarp-0.0.5/unasync.py` & `aioarp-0.0.6/unasync.py`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.5/.github/workflows/main.yml` & `aioarp-0.0.6/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.5/.github/workflows/publish.yml` & `aioarp-0.0.6/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.5/aioarp/_arp.py` & `aioarp-0.0.6/aioarp/_arp.py`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.5/aioarp/_async.py` & `aioarp-0.0.6/aioarp/_async.py`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.5/aioarp/_cli.py` & `aioarp-0.0.6/aioarp/_cli.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,18 @@
+try:
+    import typer
+except ImportError as e:
+    text = ("You are attempting to use aioarp cli without "
+            "installing the necessary dependencies; install "
+            "aioarp with all required cli dependencies using "
+            "this command `pip install aioarp[cli]`")
+    raise ImportError(text) from e
+
 import typing
 
-import typer
 from typing_extensions import Annotated
 
 import aioarp
 
 app = typer.Typer()
 
 # TODO: add tests
```

### Comparing `aioarp-0.0.5/aioarp/_client.py` & `aioarp-0.0.6/aioarp/_client.py`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.5/aioarp/_sync.py` & `aioarp-0.0.6/aioarp/_sync.py`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.5/aioarp/_utils.py` & `aioarp-0.0.6/aioarp/_utils.py`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.5/aioarp/_backends/_async.py` & `aioarp-0.0.6/aioarp/_backends/_async.py`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.5/aioarp/_backends/_mock.py` & `aioarp-0.0.6/aioarp/_backends/_mock.py`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.5/aioarp/_backends/_sync.py` & `aioarp-0.0.6/aioarp/_backends/_sync.py`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.5/tests/test_async.py` & `aioarp-0.0.6/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.5/tests/test_client.py` & `aioarp-0.0.6/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.5/tests/test_proto.py` & `aioarp-0.0.6/tests/test_proto.py`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.5/tests/test_sync.py` & `aioarp-0.0.6/tests/test_sync.py`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.5/.gitignore` & `aioarp-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.5/LICENSE.txt` & `aioarp-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.5/README.md` & `aioarp-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.5/pyproject.toml` & `aioarp-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aioarp-0.0.5/PKG-INFO` & `aioarp-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioarp
-Version: 0.0.5
+Version: 0.0.6
 Summary: Aioarp is a ARP protocol implementation that provides synchronous and asynchronous interfaces and gives you complete control over how ARP packets are sent.
 Project-URL: Documentation, https://github.com/karosis88/aioarp#readme
 Project-URL: Issues, https://github.com/karosis88/aioarp/issues
 Project-URL: Source, https://github.com/karosis88/aioarp
 Author-email: Karen Petrosyan <kar.petrosyanpy@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
```

