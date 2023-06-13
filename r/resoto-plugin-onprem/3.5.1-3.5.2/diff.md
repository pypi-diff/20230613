# Comparing `tmp/resoto-plugin-onprem-3.5.1.tar.gz` & `tmp/resoto-plugin-onprem-3.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-onprem-3.5.1.tar", last modified: Fri Jun  2 14:48:44 2023, max compression
+gzip compressed data, was "resoto-plugin-onprem-3.5.2.tar", last modified: Tue Jun 13 13:05:46 2023, max compression
```

## Comparing `resoto-plugin-onprem-3.5.1.tar` & `resoto-plugin-onprem-3.5.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:48:44.068211 resoto-plugin-onprem-3.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-02 14:46:01.000000 resoto-plugin-onprem-3.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-06-02 14:48:44.068211 resoto-plugin-onprem-3.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-02 14:46:01.000000 resoto-plugin-onprem-3.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-06-02 14:46:01.000000 resoto-plugin-onprem-3.5.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:48:44.068211 resoto-plugin-onprem-3.5.1/resoto_plugin_onprem/
--rw-r--r--   0 runner    (1001) docker     (123)     5398 2023-06-02 14:46:01.000000 resoto-plugin-onprem-3.5.1/resoto_plugin_onprem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-02 14:46:01.000000 resoto-plugin-onprem-3.5.1/resoto_plugin_onprem/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-06-02 14:46:01.000000 resoto-plugin-onprem-3.5.1/resoto_plugin_onprem/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-06-02 14:46:01.000000 resoto-plugin-onprem-3.5.1/resoto_plugin_onprem/ssh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:48:44.068211 resoto-plugin-onprem-3.5.1/resoto_plugin_onprem.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-06-02 14:48:44.000000 resoto-plugin-onprem-3.5.1/resoto_plugin_onprem.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-02 14:48:44.000000 resoto-plugin-onprem-3.5.1/resoto_plugin_onprem.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:48:44.000000 resoto-plugin-onprem-3.5.1/resoto_plugin_onprem.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-02 14:48:44.000000 resoto-plugin-onprem-3.5.1/resoto_plugin_onprem.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:47:08.000000 resoto-plugin-onprem-3.5.1/resoto_plugin_onprem.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-02 14:48:44.000000 resoto-plugin-onprem-3.5.1/resoto_plugin_onprem.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-02 14:48:44.000000 resoto-plugin-onprem-3.5.1/resoto_plugin_onprem.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-02 14:48:44.068211 resoto-plugin-onprem-3.5.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:48:44.068211 resoto-plugin-onprem-3.5.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-02 14:46:01.000000 resoto-plugin-onprem-3.5.1/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:05:46.710459 resoto-plugin-onprem-3.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-13 13:03:04.000000 resoto-plugin-onprem-3.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-06-13 13:05:46.710459 resoto-plugin-onprem-3.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-13 13:03:04.000000 resoto-plugin-onprem-3.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-06-13 13:03:04.000000 resoto-plugin-onprem-3.5.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:05:46.710459 resoto-plugin-onprem-3.5.2/resoto_plugin_onprem/
+-rw-r--r--   0 runner    (1001) docker     (123)     5398 2023-06-13 13:03:04.000000 resoto-plugin-onprem-3.5.2/resoto_plugin_onprem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-13 13:03:04.000000 resoto-plugin-onprem-3.5.2/resoto_plugin_onprem/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-06-13 13:03:04.000000 resoto-plugin-onprem-3.5.2/resoto_plugin_onprem/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-06-13 13:03:04.000000 resoto-plugin-onprem-3.5.2/resoto_plugin_onprem/ssh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:05:46.710459 resoto-plugin-onprem-3.5.2/resoto_plugin_onprem.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-06-13 13:05:46.000000 resoto-plugin-onprem-3.5.2/resoto_plugin_onprem.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-13 13:05:46.000000 resoto-plugin-onprem-3.5.2/resoto_plugin_onprem.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 13:05:46.000000 resoto-plugin-onprem-3.5.2/resoto_plugin_onprem.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-13 13:05:46.000000 resoto-plugin-onprem-3.5.2/resoto_plugin_onprem.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 13:04:11.000000 resoto-plugin-onprem-3.5.2/resoto_plugin_onprem.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-13 13:05:46.000000 resoto-plugin-onprem-3.5.2/resoto_plugin_onprem.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-13 13:05:46.000000 resoto-plugin-onprem-3.5.2/resoto_plugin_onprem.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-13 13:05:46.714459 resoto-plugin-onprem-3.5.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:05:46.710459 resoto-plugin-onprem-3.5.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-13 13:03:04.000000 resoto-plugin-onprem-3.5.2/test/test_config.py
```

### Comparing `resoto-plugin-onprem-3.5.1/PKG-INFO` & `resoto-plugin-onprem-3.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-onprem
-Version: 3.5.1
+Version: 3.5.2
 Summary: Resoto On-Premises Collector Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/onelogin
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-onprem-3.5.1/pyproject.toml` & `resoto-plugin-onprem-3.5.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "resoto-plugin-onprem"
 description = "Resoto On-Premises Collector Plugin"
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
     "paramiko",
 ]
 
 [project.entry-points."resoto.plugins"]
 onprem = "resoto_plugin_onprem:OnpremCollectorPlugin"
 
 [project.urls]
```

### Comparing `resoto-plugin-onprem-3.5.1/resoto_plugin_onprem/__init__.py` & `resoto-plugin-onprem-3.5.2/resoto_plugin_onprem/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-onprem-3.5.1/resoto_plugin_onprem/config.py` & `resoto-plugin-onprem-3.5.2/resoto_plugin_onprem/config.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-onprem-3.5.1/resoto_plugin_onprem/resources.py` & `resoto-plugin-onprem-3.5.2/resoto_plugin_onprem/resources.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-onprem-3.5.1/resoto_plugin_onprem/ssh.py` & `resoto-plugin-onprem-3.5.2/resoto_plugin_onprem/ssh.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-onprem-3.5.1/resoto_plugin_onprem.egg-info/PKG-INFO` & `resoto-plugin-onprem-3.5.2/resoto_plugin_onprem.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-onprem
-Version: 3.5.1
+Version: 3.5.2
 Summary: Resoto On-Premises Collector Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/onelogin
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-onprem-3.5.1/test/test_config.py` & `resoto-plugin-onprem-3.5.2/test/test_config.py`

 * *Files identical despite different names*

