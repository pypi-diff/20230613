# Comparing `tmp/resoto-plugin-random-3.5.1.tar.gz` & `tmp/resoto-plugin-random-3.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-random-3.5.1.tar", last modified: Fri Jun  2 14:52:52 2023, max compression
+gzip compressed data, was "resoto-plugin-random-3.5.2.tar", last modified: Tue Jun 13 13:09:50 2023, max compression
```

## Comparing `resoto-plugin-random-3.5.1.tar` & `resoto-plugin-random-3.5.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:52:52.476053 resoto-plugin-random-3.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-02 14:49:39.000000 resoto-plugin-random-3.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-06-02 14:52:52.476053 resoto-plugin-random-3.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-02 14:49:39.000000 resoto-plugin-random-3.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-06-02 14:49:39.000000 resoto-plugin-random-3.5.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:52:52.476053 resoto-plugin-random-3.5.1/resoto_plugin_random/
--rw-r--r--   0 runner    (1001) docker     (123)    11022 2023-06-02 14:49:39.000000 resoto-plugin-random-3.5.1/resoto_plugin_random/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-02 14:49:39.000000 resoto-plugin-random-3.5.1/resoto_plugin_random/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6272 2023-06-02 14:49:39.000000 resoto-plugin-random-3.5.1/resoto_plugin_random/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:52:52.476053 resoto-plugin-random-3.5.1/resoto_plugin_random.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-06-02 14:52:52.000000 resoto-plugin-random-3.5.1/resoto_plugin_random.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-02 14:52:52.000000 resoto-plugin-random-3.5.1/resoto_plugin_random.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:52:52.000000 resoto-plugin-random-3.5.1/resoto_plugin_random.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-02 14:52:52.000000 resoto-plugin-random-3.5.1/resoto_plugin_random.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:50:58.000000 resoto-plugin-random-3.5.1/resoto_plugin_random.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-02 14:52:52.000000 resoto-plugin-random-3.5.1/resoto_plugin_random.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-02 14:52:52.000000 resoto-plugin-random-3.5.1/resoto_plugin_random.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-02 14:52:52.480053 resoto-plugin-random-3.5.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:52:52.476053 resoto-plugin-random-3.5.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-02 14:49:39.000000 resoto-plugin-random-3.5.1/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:09:50.518200 resoto-plugin-random-3.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-13 13:06:44.000000 resoto-plugin-random-3.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-06-13 13:09:50.518200 resoto-plugin-random-3.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-13 13:06:44.000000 resoto-plugin-random-3.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-06-13 13:06:44.000000 resoto-plugin-random-3.5.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:09:50.518200 resoto-plugin-random-3.5.2/resoto_plugin_random/
+-rw-r--r--   0 runner    (1001) docker     (123)    11022 2023-06-13 13:06:44.000000 resoto-plugin-random-3.5.2/resoto_plugin_random/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-13 13:06:44.000000 resoto-plugin-random-3.5.2/resoto_plugin_random/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6272 2023-06-13 13:06:44.000000 resoto-plugin-random-3.5.2/resoto_plugin_random/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:09:50.518200 resoto-plugin-random-3.5.2/resoto_plugin_random.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-06-13 13:09:50.000000 resoto-plugin-random-3.5.2/resoto_plugin_random.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-13 13:09:50.000000 resoto-plugin-random-3.5.2/resoto_plugin_random.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 13:09:50.000000 resoto-plugin-random-3.5.2/resoto_plugin_random.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-13 13:09:50.000000 resoto-plugin-random-3.5.2/resoto_plugin_random.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 13:08:01.000000 resoto-plugin-random-3.5.2/resoto_plugin_random.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-13 13:09:50.000000 resoto-plugin-random-3.5.2/resoto_plugin_random.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-13 13:09:50.000000 resoto-plugin-random-3.5.2/resoto_plugin_random.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-13 13:09:50.518200 resoto-plugin-random-3.5.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:09:50.518200 resoto-plugin-random-3.5.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-13 13:06:44.000000 resoto-plugin-random-3.5.2/test/test_config.py
```

### Comparing `resoto-plugin-random-3.5.1/PKG-INFO` & `resoto-plugin-random-3.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-random
-Version: 3.5.1
+Version: 3.5.2
 Summary: Resoto Random Collector Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/random
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-random-3.5.1/README.md` & `resoto-plugin-random-3.5.2/README.md`

 * *Files identical despite different names*

### Comparing `resoto-plugin-random-3.5.1/pyproject.toml` & `resoto-plugin-random-3.5.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "resoto-plugin-random"
 description = "Resoto Random Collector Plugin"
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
 ]
 
 [project.entry-points."resoto.plugins"]
 random = "resoto_plugin_random:RandomCollectorPlugin"
 
 [project.urls]
 Documentation = "https://resoto.com"
```

### Comparing `resoto-plugin-random-3.5.1/resoto_plugin_random/__init__.py` & `resoto-plugin-random-3.5.2/resoto_plugin_random/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-random-3.5.1/resoto_plugin_random/resources.py` & `resoto-plugin-random-3.5.2/resoto_plugin_random/resources.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-random-3.5.1/resoto_plugin_random.egg-info/PKG-INFO` & `resoto-plugin-random-3.5.2/resoto_plugin_random.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-random
-Version: 3.5.1
+Version: 3.5.2
 Summary: Resoto Random Collector Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/random
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

