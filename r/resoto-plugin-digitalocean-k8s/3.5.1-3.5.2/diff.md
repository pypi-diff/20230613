# Comparing `tmp/resoto-plugin-digitalocean-k8s-3.5.1.tar.gz` & `tmp/resoto-plugin-digitalocean-k8s-3.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-digitalocean-k8s-3.5.1.tar", last modified: Fri Jun  2 14:56:51 2023, max compression
+gzip compressed data, was "resoto-plugin-digitalocean-k8s-3.5.2.tar", last modified: Tue Jun 13 13:10:34 2023, max compression
```

## Comparing `resoto-plugin-digitalocean-k8s-3.5.1.tar` & `resoto-plugin-digitalocean-k8s-3.5.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:56:51.853901 resoto-plugin-digitalocean-k8s-3.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-02 14:53:11.000000 resoto-plugin-digitalocean-k8s-3.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-02 14:56:51.853901 resoto-plugin-digitalocean-k8s-3.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-02 14:53:11.000000 resoto-plugin-digitalocean-k8s-3.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-06-02 14:53:11.000000 resoto-plugin-digitalocean-k8s-3.5.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:56:51.853901 resoto-plugin-digitalocean-k8s-3.5.1/resoto_plugin_digitalocean_k8s/
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-06-02 14:53:11.000000 resoto-plugin-digitalocean-k8s-3.5.1/resoto_plugin_digitalocean_k8s/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:56:51.853901 resoto-plugin-digitalocean-k8s-3.5.1/resoto_plugin_digitalocean_k8s.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-02 14:56:51.000000 resoto-plugin-digitalocean-k8s-3.5.1/resoto_plugin_digitalocean_k8s.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-02 14:56:51.000000 resoto-plugin-digitalocean-k8s-3.5.1/resoto_plugin_digitalocean_k8s.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:56:51.000000 resoto-plugin-digitalocean-k8s-3.5.1/resoto_plugin_digitalocean_k8s.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-02 14:56:51.000000 resoto-plugin-digitalocean-k8s-3.5.1/resoto_plugin_digitalocean_k8s.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:54:21.000000 resoto-plugin-digitalocean-k8s-3.5.1/resoto_plugin_digitalocean_k8s.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-02 14:56:51.000000 resoto-plugin-digitalocean-k8s-3.5.1/resoto_plugin_digitalocean_k8s.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-02 14:56:51.000000 resoto-plugin-digitalocean-k8s-3.5.1/resoto_plugin_digitalocean_k8s.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-02 14:56:51.857901 resoto-plugin-digitalocean-k8s-3.5.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:56:51.853901 resoto-plugin-digitalocean-k8s-3.5.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 14:53:11.000000 resoto-plugin-digitalocean-k8s-3.5.1/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-06-02 14:53:11.000000 resoto-plugin-digitalocean-k8s-3.5.1/test/test_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:10:34.030323 resoto-plugin-digitalocean-k8s-3.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-13 13:06:59.000000 resoto-plugin-digitalocean-k8s-3.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-13 13:10:34.030323 resoto-plugin-digitalocean-k8s-3.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-13 13:06:59.000000 resoto-plugin-digitalocean-k8s-3.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-06-13 13:06:59.000000 resoto-plugin-digitalocean-k8s-3.5.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:10:34.026323 resoto-plugin-digitalocean-k8s-3.5.2/resoto_plugin_digitalocean_k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-06-13 13:06:59.000000 resoto-plugin-digitalocean-k8s-3.5.2/resoto_plugin_digitalocean_k8s/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:10:34.030323 resoto-plugin-digitalocean-k8s-3.5.2/resoto_plugin_digitalocean_k8s.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-13 13:10:34.000000 resoto-plugin-digitalocean-k8s-3.5.2/resoto_plugin_digitalocean_k8s.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-13 13:10:34.000000 resoto-plugin-digitalocean-k8s-3.5.2/resoto_plugin_digitalocean_k8s.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 13:10:34.000000 resoto-plugin-digitalocean-k8s-3.5.2/resoto_plugin_digitalocean_k8s.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-13 13:10:34.000000 resoto-plugin-digitalocean-k8s-3.5.2/resoto_plugin_digitalocean_k8s.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 13:08:06.000000 resoto-plugin-digitalocean-k8s-3.5.2/resoto_plugin_digitalocean_k8s.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-13 13:10:34.000000 resoto-plugin-digitalocean-k8s-3.5.2/resoto_plugin_digitalocean_k8s.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-13 13:10:34.000000 resoto-plugin-digitalocean-k8s-3.5.2/resoto_plugin_digitalocean_k8s.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-13 13:10:34.030323 resoto-plugin-digitalocean-k8s-3.5.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:10:34.030323 resoto-plugin-digitalocean-k8s-3.5.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:06:59.000000 resoto-plugin-digitalocean-k8s-3.5.2/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-06-13 13:06:59.000000 resoto-plugin-digitalocean-k8s-3.5.2/test/test_collector.py
```

### Comparing `resoto-plugin-digitalocean-k8s-3.5.1/PKG-INFO` & `resoto-plugin-digitalocean-k8s-3.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-digitalocean-k8s
-Version: 3.5.1
+Version: 3.5.2
 Summary: Resoto DigitalOcean-K8s Collector Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/digitalocean_k8s
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-digitalocean-k8s-3.5.1/pyproject.toml` & `resoto-plugin-digitalocean-k8s-3.5.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "resoto-plugin-digitalocean-k8s"
 description = "Resoto DigitalOcean-K8s Collector Plugin"
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
 
 [project.optional-dependencies]
 dev = [
     "mypy",
 ]
```

### Comparing `resoto-plugin-digitalocean-k8s-3.5.1/resoto_plugin_digitalocean_k8s/__init__.py` & `resoto-plugin-digitalocean-k8s-3.5.2/resoto_plugin_digitalocean_k8s/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-k8s-3.5.1/resoto_plugin_digitalocean_k8s.egg-info/PKG-INFO` & `resoto-plugin-digitalocean-k8s-3.5.2/resoto_plugin_digitalocean_k8s.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-digitalocean-k8s
-Version: 3.5.1
+Version: 3.5.2
 Summary: Resoto DigitalOcean-K8s Collector Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/digitalocean_k8s
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-digitalocean-k8s-3.5.1/test/test_collector.py` & `resoto-plugin-digitalocean-k8s-3.5.2/test/test_collector.py`

 * *Files identical despite different names*

