# Comparing `tmp/resoto-plugin-onelogin-3.5.1.tar.gz` & `tmp/resoto-plugin-onelogin-3.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-onelogin-3.5.1.tar", last modified: Fri Jun  2 14:54:23 2023, max compression
+gzip compressed data, was "resoto-plugin-onelogin-3.5.2.tar", last modified: Tue Jun 13 13:05:44 2023, max compression
```

## Comparing `resoto-plugin-onelogin-3.5.1.tar` & `resoto-plugin-onelogin-3.5.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:54:23.494231 resoto-plugin-onelogin-3.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-02 14:50:52.000000 resoto-plugin-onelogin-3.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-06-02 14:54:23.494231 resoto-plugin-onelogin-3.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-02 14:50:52.000000 resoto-plugin-onelogin-3.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-06-02 14:50:52.000000 resoto-plugin-onelogin-3.5.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:54:23.494231 resoto-plugin-onelogin-3.5.1/resoto_plugin_onelogin/
--rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-06-02 14:50:52.000000 resoto-plugin-onelogin-3.5.1/resoto_plugin_onelogin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-02 14:50:52.000000 resoto-plugin-onelogin-3.5.1/resoto_plugin_onelogin/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:54:23.494231 resoto-plugin-onelogin-3.5.1/resoto_plugin_onelogin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-06-02 14:54:23.000000 resoto-plugin-onelogin-3.5.1/resoto_plugin_onelogin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-02 14:54:23.000000 resoto-plugin-onelogin-3.5.1/resoto_plugin_onelogin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:54:23.000000 resoto-plugin-onelogin-3.5.1/resoto_plugin_onelogin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-02 14:54:23.000000 resoto-plugin-onelogin-3.5.1/resoto_plugin_onelogin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:52:19.000000 resoto-plugin-onelogin-3.5.1/resoto_plugin_onelogin.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-02 14:54:23.000000 resoto-plugin-onelogin-3.5.1/resoto_plugin_onelogin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-02 14:54:23.000000 resoto-plugin-onelogin-3.5.1/resoto_plugin_onelogin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-02 14:54:23.494231 resoto-plugin-onelogin-3.5.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:54:23.494231 resoto-plugin-onelogin-3.5.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-02 14:50:52.000000 resoto-plugin-onelogin-3.5.1/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:05:44.079094 resoto-plugin-onelogin-3.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-13 13:03:04.000000 resoto-plugin-onelogin-3.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-06-13 13:05:44.079094 resoto-plugin-onelogin-3.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-13 13:03:04.000000 resoto-plugin-onelogin-3.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-06-13 13:03:04.000000 resoto-plugin-onelogin-3.5.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:05:44.079094 resoto-plugin-onelogin-3.5.2/resoto_plugin_onelogin/
+-rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-06-13 13:03:04.000000 resoto-plugin-onelogin-3.5.2/resoto_plugin_onelogin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-13 13:03:04.000000 resoto-plugin-onelogin-3.5.2/resoto_plugin_onelogin/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:05:44.079094 resoto-plugin-onelogin-3.5.2/resoto_plugin_onelogin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-06-13 13:05:44.000000 resoto-plugin-onelogin-3.5.2/resoto_plugin_onelogin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-13 13:05:44.000000 resoto-plugin-onelogin-3.5.2/resoto_plugin_onelogin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 13:05:44.000000 resoto-plugin-onelogin-3.5.2/resoto_plugin_onelogin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-13 13:05:44.000000 resoto-plugin-onelogin-3.5.2/resoto_plugin_onelogin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 13:04:08.000000 resoto-plugin-onelogin-3.5.2/resoto_plugin_onelogin.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-13 13:05:44.000000 resoto-plugin-onelogin-3.5.2/resoto_plugin_onelogin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-13 13:05:44.000000 resoto-plugin-onelogin-3.5.2/resoto_plugin_onelogin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-13 13:05:44.079094 resoto-plugin-onelogin-3.5.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:05:44.079094 resoto-plugin-onelogin-3.5.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-13 13:03:04.000000 resoto-plugin-onelogin-3.5.2/test/test_config.py
```

### Comparing `resoto-plugin-onelogin-3.5.1/PKG-INFO` & `resoto-plugin-onelogin-3.5.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-onelogin
-Version: 3.5.1
+Version: 3.5.2
 Summary: Resoto OneLogin Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/onelogin
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-onelogin-3.5.1/pyproject.toml` & `resoto-plugin-onelogin-3.5.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "resoto-plugin-onelogin"
 description = "Resoto OneLogin Plugin"
-version = "3.5.1"
+version = "3.5.2"
 authors = [{name="Some Engineering Inc."}]
 license = {file="LICENSE"}
 requires-python = ">=3.9"
 classifiers = [
     # Current project status
     "Development Status :: 4 - Beta",
     # Audience
@@ -23,15 +23,15 @@
     "Natural Language :: English",
     "Topic :: Security",
     "Topic :: Utilities",
 ]
 readme = {file="README.md", content-type="text/markdown"}
 
 dependencies = [
-    "resotolib==3.5.1",
+    "resotolib==3.5.2",
     "onelogin==2.0.4",
 ]
 
 [project.entry-points."resoto.plugins"]
 onelogin = "resoto_plugin_onelogin:OneLoginPlugin"
 
 [project.urls]
```

### Comparing `resoto-plugin-onelogin-3.5.1/resoto_plugin_onelogin/__init__.py` & `resoto-plugin-onelogin-3.5.2/resoto_plugin_onelogin/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-onelogin-3.5.1/resoto_plugin_onelogin.egg-info/PKG-INFO` & `resoto-plugin-onelogin-3.5.2/resoto_plugin_onelogin.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-onelogin
-Version: 3.5.1
+Version: 3.5.2
 Summary: Resoto OneLogin Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/onelogin
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

