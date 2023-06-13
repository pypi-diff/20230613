# Comparing `tmp/zemail-1.0.0.tar.gz` & `tmp/zemail-1.0.1.tar.gz`

## Comparing `zemail-1.0.0.tar` & `zemail-1.0.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 zemail-1.0.0/src/zemail/__init__.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 zemail-1.0.0/LICENSE
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 zemail-1.0.0/README.md
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 zemail-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 zemail-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 zemail-1.0.1/src/zemail/__init__.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 zemail-1.0.1/LICENSE
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 zemail-1.0.1/README.md
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 zemail-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 zemail-1.0.1/PKG-INFO
```

### Comparing `zemail-1.0.0/src/zemail/__init__.py` & `zemail-1.0.1/src/zemail/__init__.py`

 * *Files identical despite different names*

### Comparing `zemail-1.0.0/LICENSE` & `zemail-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zemail-1.0.0/pyproject.toml` & `zemail-1.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "zemail"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="inspirare6", email="inspirare6@163.com" },
 ]
 description = "zen email library"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.6"
 dependencies = []
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `zemail-1.0.0/PKG-INFO` & `zemail-1.0.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: zemail
-Version: 1.0.0
+Version: 1.0.1
 Summary: zen email library
 Project-URL: Homepage, https://github.com/inspirare6/zemail
 Project-URL: Bug Tracker, https://github.com/inspirare6/zemail/issues
 Author-email: inspirare6 <inspirare6@163.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # zemail
 
 Zen email library.
```

