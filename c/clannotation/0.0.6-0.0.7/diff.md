# Comparing `tmp/clannotation-0.0.6.tar.gz` & `tmp/clannotation-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clannotation-0.0.6.tar", last modified: Wed May 10 11:30:20 2023, max compression
+gzip compressed data, was "clannotation-0.0.7.tar", last modified: Tue Jun 13 14:43:16 2023, max compression
```

## Comparing `clannotation-0.0.6.tar` & `clannotation-0.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-05-10 11:30:19.996841 clannotation-0.0.6/
--rw-rw-r--   0 martin    (1000) martin    (1000)     1054 2023-01-26 10:26:21.000000 clannotation-0.0.6/LICENSE.md
--rw-rw-r--   0 martin    (1000) martin    (1000)     2846 2023-05-10 11:30:19.996841 clannotation-0.0.6/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)      986 2023-04-20 09:30:48.000000 clannotation-0.0.6/README.md
--rw-rw-r--   0 martin    (1000) martin    (1000)      958 2023-05-10 11:29:05.000000 clannotation-0.0.6/pyproject.toml
--rw-rw-r--   0 martin    (1000) martin    (1000)      926 2023-05-10 11:30:19.996841 clannotation-0.0.6/setup.cfg
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-05-10 11:30:19.992841 clannotation-0.0.6/src/
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-05-10 11:30:19.992841 clannotation-0.0.6/src/clannotation/
--rw-rw-r--   0 martin    (1000) martin    (1000)        0 2023-04-20 07:44:29.000000 clannotation-0.0.6/src/clannotation/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    10784 2023-04-20 11:37:28.000000 clannotation-0.0.6/src/clannotation/annotator.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-05-10 11:30:19.996841 clannotation-0.0.6/src/clannotation.egg-info/
--rw-rw-r--   0 martin    (1000) martin    (1000)     2846 2023-05-10 11:30:19.000000 clannotation-0.0.6/src/clannotation.egg-info/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)      334 2023-05-10 11:30:19.000000 clannotation-0.0.6/src/clannotation.egg-info/SOURCES.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-05-10 11:30:19.000000 clannotation-0.0.6/src/clannotation.egg-info/dependency_links.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       72 2023-05-10 11:30:19.000000 clannotation-0.0.6/src/clannotation.egg-info/requires.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       13 2023-05-10 11:30:19.000000 clannotation-0.0.6/src/clannotation.egg-info/top_level.txt
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-05-10 11:30:19.996841 clannotation-0.0.6/tests/
--rw-rw-r--   0 martin    (1000) martin    (1000)    18311 2023-04-20 08:47:46.000000 clannotation-0.0.6/tests/test_annotator_plugin.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-13 14:43:16.872540 clannotation-0.0.7/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1054 2023-01-26 10:26:21.000000 clannotation-0.0.7/LICENSE.md
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2846 2023-06-13 14:43:16.872540 clannotation-0.0.7/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)      986 2023-04-20 09:30:48.000000 clannotation-0.0.7/README.md
+-rw-rw-r--   0 martin    (1000) martin    (1000)      958 2023-06-13 14:42:26.000000 clannotation-0.0.7/pyproject.toml
+-rw-rw-r--   0 martin    (1000) martin    (1000)      926 2023-06-13 14:43:16.872540 clannotation-0.0.7/setup.cfg
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-13 14:43:16.872540 clannotation-0.0.7/src/
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-13 14:43:16.872540 clannotation-0.0.7/src/clannotation/
+-rw-rw-r--   0 martin    (1000) martin    (1000)        0 2023-04-20 07:44:29.000000 clannotation-0.0.7/src/clannotation/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    10784 2023-04-20 11:37:28.000000 clannotation-0.0.7/src/clannotation/annotator.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-13 14:43:16.872540 clannotation-0.0.7/src/clannotation.egg-info/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2846 2023-06-13 14:43:16.000000 clannotation-0.0.7/src/clannotation.egg-info/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)      334 2023-06-13 14:43:16.000000 clannotation-0.0.7/src/clannotation.egg-info/SOURCES.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-06-13 14:43:16.000000 clannotation-0.0.7/src/clannotation.egg-info/dependency_links.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       72 2023-06-13 14:43:16.000000 clannotation-0.0.7/src/clannotation.egg-info/requires.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       13 2023-06-13 14:43:16.000000 clannotation-0.0.7/src/clannotation.egg-info/top_level.txt
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-13 14:43:16.872540 clannotation-0.0.7/tests/
+-rw-rw-r--   0 martin    (1000) martin    (1000)    18311 2023-04-20 08:47:46.000000 clannotation-0.0.7/tests/test_annotator_plugin.py
```

### Comparing `clannotation-0.0.6/LICENSE.md` & `clannotation-0.0.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `clannotation-0.0.6/PKG-INFO` & `clannotation-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clannotation
-Version: 0.0.6
+Version: 0.0.7
 Summary: The Crossref Labs annotation tool.
 Home-page: https://gitlab.com/crossref/labs/annotator
 Author: Martin Paul Eve
 Author-email: meve@crossref.org
 Maintainer-email: Martin Paul Eve <meve@crossref.org>
 License: Copyright &copy; 2023 Crossref
```

### Comparing `clannotation-0.0.6/README.md` & `clannotation-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `clannotation-0.0.6/pyproject.toml` & `clannotation-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "clannotation"
-version = "0.0.6"
+version = "0.0.7"
 description = "The Crossref Labs annotation tool."
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE.md"}
 keywords = ["API", "Crossref", "annotation", "AWS", "Lambda"]
 authors = [
   {email = "meve@crossref.org"},
```

### Comparing `clannotation-0.0.6/setup.cfg` & `clannotation-0.0.7/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = clannotation
-version = 0.0.6
+version = 0.0.7
 description = The Crossref Labs annotation tool.
 url = https://gitlab.com/crossref/labs/annotator
 author = Martin Paul Eve
 author_email = meve@crossref.org
 license = MIT
 classifiers = 
 	Intended Audience :: Developers
@@ -21,15 +21,15 @@
 
 [options]
 include_package_data = true
 package_dir = =src
 packages = find:
 python_requires = >=3.8
 install_requires = 
-	claws>=0.0.12
+	claws>=0.0.20
 	aws-lambda-powertools[all]
 	longsight>=1.0.5
 	moto
 	botocore
 
 [options.packages.find]
 where = src
```

### Comparing `clannotation-0.0.6/src/clannotation/annotator.py` & `clannotation-0.0.7/src/clannotation/annotator.py`

 * *Files identical despite different names*

### Comparing `clannotation-0.0.6/src/clannotation.egg-info/PKG-INFO` & `clannotation-0.0.7/src/clannotation.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clannotation
-Version: 0.0.6
+Version: 0.0.7
 Summary: The Crossref Labs annotation tool.
 Home-page: https://gitlab.com/crossref/labs/annotator
 Author: Martin Paul Eve
 Author-email: meve@crossref.org
 Maintainer-email: Martin Paul Eve <meve@crossref.org>
 License: Copyright &copy; 2023 Crossref
```

### Comparing `clannotation-0.0.6/tests/test_annotator_plugin.py` & `clannotation-0.0.7/tests/test_annotator_plugin.py`

 * *Files identical despite different names*

