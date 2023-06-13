# Comparing `tmp/znetwork-0.1.1.tar.gz` & `tmp/znetwork-1.0.0.tar.gz`

## Comparing `znetwork-0.1.1.tar` & `znetwork-1.0.0.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 znetwork-0.1.1/src/znetwork/__init__.py
--rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 znetwork-0.1.1/src/znetwork/dom.py
--rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 znetwork-0.1.1/src/znetwork/mail.py
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 znetwork-0.1.1/tests/1.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 znetwork-0.1.1/LICENSE
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 znetwork-0.1.1/README.md
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 znetwork-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 znetwork-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 znetwork-1.0.0/src/znetwork/__init__.py
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 znetwork-1.0.0/src/znetwork/mail.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 znetwork-1.0.0/tests/1.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 znetwork-1.0.0/LICENSE
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 znetwork-1.0.0/README.md
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 znetwork-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 znetwork-1.0.0/PKG-INFO
```

### Comparing `znetwork-0.1.1/LICENSE` & `znetwork-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `znetwork-0.1.1/pyproject.toml` & `znetwork-1.0.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "znetwork"
-version = "0.1.1"
+version = "1.0.0"
 authors = [
   { name="inspirare6", email="inspirare6@163.com" },
 ]
 description = "zen network library"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.6"
 dependencies = [
   "requests",
-  "beautifulsoup4",
-  "lxml",
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `znetwork-0.1.1/PKG-INFO` & `znetwork-1.0.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: znetwork
-Version: 0.1.1
+Version: 1.0.0
 Summary: zen network library
 Project-URL: Homepage, https://github.com/inspirare6/znetwork
 Project-URL: Bug Tracker, https://github.com/inspirare6/znetwork/issues
 Author-email: inspirare6 <inspirare6@163.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Requires-Dist: beautifulsoup4
-Requires-Dist: lxml
+Requires-Python: >=3.6
 Requires-Dist: requests
 Description-Content-Type: text/markdown
 
 # znetwork
 
 Zen network library.
```

