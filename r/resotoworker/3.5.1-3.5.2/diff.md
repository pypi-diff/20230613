# Comparing `tmp/resotoworker-3.5.1.tar.gz` & `tmp/resotoworker-3.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resotoworker-3.5.1.tar", last modified: Fri Jun  2 14:49:51 2023, max compression
+gzip compressed data, was "resotoworker-3.5.2.tar", last modified: Tue Jun 13 13:06:57 2023, max compression
```

## Comparing `resotoworker-3.5.1.tar` & `resotoworker-3.5.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:49:51.866352 resotoworker-3.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-02 14:46:08.000000 resotoworker-3.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-06-02 14:49:51.866352 resotoworker-3.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4965 2023-06-02 14:46:08.000000 resotoworker-3.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-02 14:46:08.000000 resotoworker-3.5.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:49:51.866352 resotoworker-3.5.1/resotoworker/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-02 14:46:08.000000 resotoworker-3.5.1/resotoworker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11784 2023-06-02 14:46:08.000000 resotoworker-3.5.1/resotoworker/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5518 2023-06-02 14:46:08.000000 resotoworker-3.5.1/resotoworker/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-06-02 14:46:08.000000 resotoworker-3.5.1/resotoworker/collect.py
--rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-06-02 14:46:08.000000 resotoworker-3.5.1/resotoworker/config.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-02 14:46:08.000000 resotoworker-3.5.1/resotoworker/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-06-02 14:46:08.000000 resotoworker-3.5.1/resotoworker/pluginloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-06-02 14:46:08.000000 resotoworker-3.5.1/resotoworker/resotocore.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-06-02 14:46:08.000000 resotoworker-3.5.1/resotoworker/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-06-02 14:46:08.000000 resotoworker-3.5.1/resotoworker/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:49:51.866352 resotoworker-3.5.1/resotoworker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-06-02 14:49:51.000000 resotoworker-3.5.1/resotoworker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-02 14:49:51.000000 resotoworker-3.5.1/resotoworker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:49:51.000000 resotoworker-3.5.1/resotoworker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-02 14:49:51.000000 resotoworker-3.5.1/resotoworker.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:47:17.000000 resotoworker-3.5.1/resotoworker.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-02 14:49:51.000000 resotoworker-3.5.1/resotoworker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-02 14:49:51.000000 resotoworker-3.5.1/resotoworker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-02 14:49:51.866352 resotoworker-3.5.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:49:51.866352 resotoworker-3.5.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 14:46:08.000000 resotoworker-3.5.1/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-02 14:46:08.000000 resotoworker-3.5.1/test/fakeconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-02 14:46:08.000000 resotoworker-3.5.1/test/test_args.py
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-06-02 14:46:08.000000 resotoworker-3.5.1/test/test_collect.py
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-06-02 14:46:08.000000 resotoworker-3.5.1/test/test_resotocore.py
--rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-06-02 14:46:08.000000 resotoworker-3.5.1/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:06:57.587864 resotoworker-3.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-13 13:03:07.000000 resotoworker-3.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-06-13 13:06:57.587864 resotoworker-3.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4965 2023-06-13 13:03:07.000000 resotoworker-3.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-13 13:03:07.000000 resotoworker-3.5.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:06:57.583864 resotoworker-3.5.2/resotoworker/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-13 13:03:07.000000 resotoworker-3.5.2/resotoworker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11784 2023-06-13 13:03:07.000000 resotoworker-3.5.2/resotoworker/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5518 2023-06-13 13:03:07.000000 resotoworker-3.5.2/resotoworker/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-06-13 13:03:07.000000 resotoworker-3.5.2/resotoworker/collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-06-13 13:03:07.000000 resotoworker-3.5.2/resotoworker/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-13 13:03:07.000000 resotoworker-3.5.2/resotoworker/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-06-13 13:03:07.000000 resotoworker-3.5.2/resotoworker/pluginloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-06-13 13:03:07.000000 resotoworker-3.5.2/resotoworker/resotocore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-06-13 13:03:07.000000 resotoworker-3.5.2/resotoworker/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-06-13 13:03:07.000000 resotoworker-3.5.2/resotoworker/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:06:57.583864 resotoworker-3.5.2/resotoworker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-06-13 13:06:57.000000 resotoworker-3.5.2/resotoworker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-13 13:06:57.000000 resotoworker-3.5.2/resotoworker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 13:06:57.000000 resotoworker-3.5.2/resotoworker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-13 13:06:57.000000 resotoworker-3.5.2/resotoworker.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 13:04:20.000000 resotoworker-3.5.2/resotoworker.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-13 13:06:57.000000 resotoworker-3.5.2/resotoworker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-13 13:06:57.000000 resotoworker-3.5.2/resotoworker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-13 13:06:57.587864 resotoworker-3.5.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:06:57.583864 resotoworker-3.5.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:03:07.000000 resotoworker-3.5.2/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-13 13:03:07.000000 resotoworker-3.5.2/test/fakeconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-13 13:03:07.000000 resotoworker-3.5.2/test/test_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-06-13 13:03:07.000000 resotoworker-3.5.2/test/test_collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-06-13 13:03:07.000000 resotoworker-3.5.2/test/test_resotocore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-06-13 13:03:07.000000 resotoworker-3.5.2/test/test_utils.py
```

### Comparing `resotoworker-3.5.1/PKG-INFO` & `resotoworker-3.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotoworker
-Version: 3.5.1
+Version: 3.5.2
 Summary: Runs collector plugins and sends the result to resotocore.
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/resotoworker
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `resotoworker-3.5.1/README.md` & `resotoworker-3.5.2/README.md`

 * *Files identical despite different names*

### Comparing `resotoworker-3.5.1/pyproject.toml` & `resotoworker-3.5.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [project]
 name = "resotoworker"
-version = "3.5.1"
+version = "3.5.2"
 authors = [{name="Some Engineering Inc."}]
 description = "Runs collector plugins and sends the result to resotocore."
 license = {file="LICENSE"}
 requires-python = ">=3.9"
 classifiers = [ "Programming Language :: Python :: 3" ]
 readme = {file="README.md", content-type="text/markdown"}
 
 dependencies = [
-    "resotolib==3.5.1",
+    "resotolib==3.5.2",
     "tenacity",
     "CherryPy",
 ]
 
 [project.scripts]
 resotoworker = "resotoworker.__main__:main"
```

### Comparing `resotoworker-3.5.1/resotoworker/__main__.py` & `resotoworker-3.5.2/resotoworker/__main__.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.5.1/resotoworker/cleanup.py` & `resotoworker-3.5.2/resotoworker/cleanup.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.5.1/resotoworker/collect.py` & `resotoworker-3.5.2/resotoworker/collect.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.5.1/resotoworker/config.py` & `resotoworker-3.5.2/resotoworker/config.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.5.1/resotoworker/pluginloader.py` & `resotoworker-3.5.2/resotoworker/pluginloader.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.5.1/resotoworker/resotocore.py` & `resotoworker-3.5.2/resotoworker/resotocore.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.5.1/resotoworker/tag.py` & `resotoworker-3.5.2/resotoworker/tag.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.5.1/resotoworker/utils.py` & `resotoworker-3.5.2/resotoworker/utils.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.5.1/resotoworker.egg-info/PKG-INFO` & `resotoworker-3.5.2/resotoworker.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotoworker
-Version: 3.5.1
+Version: 3.5.2
 Summary: Runs collector plugins and sends the result to resotocore.
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/resotoworker
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `resotoworker-3.5.1/resotoworker.egg-info/SOURCES.txt` & `resotoworker-3.5.2/resotoworker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resotoworker-3.5.1/test/test_args.py` & `resotoworker-3.5.2/test/test_args.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.5.1/test/test_collect.py` & `resotoworker-3.5.2/test/test_collect.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.5.1/test/test_resotocore.py` & `resotoworker-3.5.2/test/test_resotocore.py`

 * *Files identical despite different names*

### Comparing `resotoworker-3.5.1/test/test_utils.py` & `resotoworker-3.5.2/test/test_utils.py`

 * *Files identical despite different names*

