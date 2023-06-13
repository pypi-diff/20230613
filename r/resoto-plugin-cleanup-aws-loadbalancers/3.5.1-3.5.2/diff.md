# Comparing `tmp/resoto-plugin-cleanup-aws-loadbalancers-3.5.1.tar.gz` & `tmp/resoto-plugin-cleanup-aws-loadbalancers-3.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-cleanup-aws-loadbalancers-3.5.1.tar", last modified: Fri Jun  2 14:51:16 2023, max compression
+gzip compressed data, was "resoto-plugin-cleanup-aws-loadbalancers-3.5.2.tar", last modified: Tue Jun 13 13:07:14 2023, max compression
```

## Comparing `resoto-plugin-cleanup-aws-loadbalancers-3.5.1.tar` & `resoto-plugin-cleanup-aws-loadbalancers-3.5.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:16.081314 resoto-plugin-cleanup-aws-loadbalancers-3.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-02 14:48:21.000000 resoto-plugin-cleanup-aws-loadbalancers-3.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-06-02 14:51:16.081314 resoto-plugin-cleanup-aws-loadbalancers-3.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-02 14:48:21.000000 resoto-plugin-cleanup-aws-loadbalancers-3.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-02 14:48:21.000000 resoto-plugin-cleanup-aws-loadbalancers-3.5.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:16.081314 resoto-plugin-cleanup-aws-loadbalancers-3.5.1/resoto_plugin_cleanup_aws_loadbalancers/
--rw-r--r--   0 runner    (1001) docker     (123)     5797 2023-06-02 14:48:21.000000 resoto-plugin-cleanup-aws-loadbalancers-3.5.1/resoto_plugin_cleanup_aws_loadbalancers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-02 14:48:21.000000 resoto-plugin-cleanup-aws-loadbalancers-3.5.1/resoto_plugin_cleanup_aws_loadbalancers/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:16.081314 resoto-plugin-cleanup-aws-loadbalancers-3.5.1/resoto_plugin_cleanup_aws_loadbalancers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-06-02 14:51:16.000000 resoto-plugin-cleanup-aws-loadbalancers-3.5.1/resoto_plugin_cleanup_aws_loadbalancers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-02 14:51:16.000000 resoto-plugin-cleanup-aws-loadbalancers-3.5.1/resoto_plugin_cleanup_aws_loadbalancers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:51:16.000000 resoto-plugin-cleanup-aws-loadbalancers-3.5.1/resoto_plugin_cleanup_aws_loadbalancers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-02 14:51:16.000000 resoto-plugin-cleanup-aws-loadbalancers-3.5.1/resoto_plugin_cleanup_aws_loadbalancers.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:49:34.000000 resoto-plugin-cleanup-aws-loadbalancers-3.5.1/resoto_plugin_cleanup_aws_loadbalancers.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-02 14:51:16.000000 resoto-plugin-cleanup-aws-loadbalancers-3.5.1/resoto_plugin_cleanup_aws_loadbalancers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-02 14:51:16.000000 resoto-plugin-cleanup-aws-loadbalancers-3.5.1/resoto_plugin_cleanup_aws_loadbalancers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-02 14:51:16.081314 resoto-plugin-cleanup-aws-loadbalancers-3.5.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:16.081314 resoto-plugin-cleanup-aws-loadbalancers-3.5.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-02 14:48:21.000000 resoto-plugin-cleanup-aws-loadbalancers-3.5.1/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:14.378982 resoto-plugin-cleanup-aws-loadbalancers-3.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-13 13:03:12.000000 resoto-plugin-cleanup-aws-loadbalancers-3.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-06-13 13:07:14.378982 resoto-plugin-cleanup-aws-loadbalancers-3.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-13 13:03:12.000000 resoto-plugin-cleanup-aws-loadbalancers-3.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-13 13:03:12.000000 resoto-plugin-cleanup-aws-loadbalancers-3.5.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:14.374982 resoto-plugin-cleanup-aws-loadbalancers-3.5.2/resoto_plugin_cleanup_aws_loadbalancers/
+-rw-r--r--   0 runner    (1001) docker     (123)     5797 2023-06-13 13:03:12.000000 resoto-plugin-cleanup-aws-loadbalancers-3.5.2/resoto_plugin_cleanup_aws_loadbalancers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-13 13:03:12.000000 resoto-plugin-cleanup-aws-loadbalancers-3.5.2/resoto_plugin_cleanup_aws_loadbalancers/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:14.374982 resoto-plugin-cleanup-aws-loadbalancers-3.5.2/resoto_plugin_cleanup_aws_loadbalancers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-06-13 13:07:14.000000 resoto-plugin-cleanup-aws-loadbalancers-3.5.2/resoto_plugin_cleanup_aws_loadbalancers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-13 13:07:14.000000 resoto-plugin-cleanup-aws-loadbalancers-3.5.2/resoto_plugin_cleanup_aws_loadbalancers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 13:07:14.000000 resoto-plugin-cleanup-aws-loadbalancers-3.5.2/resoto_plugin_cleanup_aws_loadbalancers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-13 13:07:14.000000 resoto-plugin-cleanup-aws-loadbalancers-3.5.2/resoto_plugin_cleanup_aws_loadbalancers.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 13:04:53.000000 resoto-plugin-cleanup-aws-loadbalancers-3.5.2/resoto_plugin_cleanup_aws_loadbalancers.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-13 13:07:14.000000 resoto-plugin-cleanup-aws-loadbalancers-3.5.2/resoto_plugin_cleanup_aws_loadbalancers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-13 13:07:14.000000 resoto-plugin-cleanup-aws-loadbalancers-3.5.2/resoto_plugin_cleanup_aws_loadbalancers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-13 13:07:14.378982 resoto-plugin-cleanup-aws-loadbalancers-3.5.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:14.374982 resoto-plugin-cleanup-aws-loadbalancers-3.5.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-13 13:03:12.000000 resoto-plugin-cleanup-aws-loadbalancers-3.5.2/test/test_config.py
```

### Comparing `resoto-plugin-cleanup-aws-loadbalancers-3.5.1/PKG-INFO` & `resoto-plugin-cleanup-aws-loadbalancers-3.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-cleanup-aws-loadbalancers
-Version: 3.5.1
+Version: 3.5.2
 Summary: AWS Loadbalancers Cleaner Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/cleanup_aws_loadbalancers
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-cleanup-aws-loadbalancers-3.5.1/README.md` & `resoto-plugin-cleanup-aws-loadbalancers-3.5.2/README.md`

 * *Files identical despite different names*

### Comparing `resoto-plugin-cleanup-aws-loadbalancers-3.5.1/pyproject.toml` & `resoto-plugin-cleanup-aws-loadbalancers-3.5.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "resoto-plugin-cleanup-aws-loadbalancers"
-version = "3.5.1"
+version = "3.5.2"
 authors = [{name="Some Engineering Inc."}]
 description = "AWS Loadbalancers Cleaner Plugin"
 license = {file="LICENSE"}
 requires-python = ">=3.9"
 classifiers = [
     # Current project status
     "Development Status :: 4 - Beta",
@@ -23,16 +23,16 @@
     "Natural Language :: English",
     "Topic :: Security",
     "Topic :: Utilities",
 ]
 readme = {file="README.md", content-type="text/markdown"}
 
 dependencies = [
-    "resotolib==3.5.1",
-    "resoto-plugin-aws==3.5.1"
+    "resotolib==3.5.2",
+    "resoto-plugin-aws==3.5.2"
 ]
 
 [project.entry-points."resoto.plugins"]
 cleanup_aws_loadbalancers = "resoto_plugin_cleanup_aws_loadbalancers:CleanupAWSLoadbalancersPlugin"
 
 [project.urls]
 Documentation = "https://resoto.com"
```

### Comparing `resoto-plugin-cleanup-aws-loadbalancers-3.5.1/resoto_plugin_cleanup_aws_loadbalancers/__init__.py` & `resoto-plugin-cleanup-aws-loadbalancers-3.5.2/resoto_plugin_cleanup_aws_loadbalancers/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-cleanup-aws-loadbalancers-3.5.1/resoto_plugin_cleanup_aws_loadbalancers/config.py` & `resoto-plugin-cleanup-aws-loadbalancers-3.5.2/resoto_plugin_cleanup_aws_loadbalancers/config.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-cleanup-aws-loadbalancers-3.5.1/resoto_plugin_cleanup_aws_loadbalancers.egg-info/PKG-INFO` & `resoto-plugin-cleanup-aws-loadbalancers-3.5.2/resoto_plugin_cleanup_aws_loadbalancers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-cleanup-aws-loadbalancers
-Version: 3.5.1
+Version: 3.5.2
 Summary: AWS Loadbalancers Cleaner Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/cleanup_aws_loadbalancers
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-cleanup-aws-loadbalancers-3.5.1/resoto_plugin_cleanup_aws_loadbalancers.egg-info/SOURCES.txt` & `resoto-plugin-cleanup-aws-loadbalancers-3.5.2/resoto_plugin_cleanup_aws_loadbalancers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

