# Comparing `tmp/resoto-plugin-aws-k8s-3.5.1.tar.gz` & `tmp/resoto-plugin-aws-k8s-3.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-aws-k8s-3.5.1.tar", last modified: Fri Jun  2 14:57:25 2023, max compression
+gzip compressed data, was "resoto-plugin-aws-k8s-3.5.2.tar", last modified: Tue Jun 13 13:06:39 2023, max compression
```

## Comparing `resoto-plugin-aws-k8s-3.5.1.tar` & `resoto-plugin-aws-k8s-3.5.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:57:25.795444 resoto-plugin-aws-k8s-3.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-02 14:53:44.000000 resoto-plugin-aws-k8s-3.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-02 14:57:25.795444 resoto-plugin-aws-k8s-3.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-02 14:53:44.000000 resoto-plugin-aws-k8s-3.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-06-02 14:53:44.000000 resoto-plugin-aws-k8s-3.5.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:57:25.795444 resoto-plugin-aws-k8s-3.5.1/resoto_plugin_aws_k8s/
--rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-06-02 14:53:44.000000 resoto-plugin-aws-k8s-3.5.1/resoto_plugin_aws_k8s/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:57:25.795444 resoto-plugin-aws-k8s-3.5.1/resoto_plugin_aws_k8s.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-02 14:57:25.000000 resoto-plugin-aws-k8s-3.5.1/resoto_plugin_aws_k8s.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-02 14:57:25.000000 resoto-plugin-aws-k8s-3.5.1/resoto_plugin_aws_k8s.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:57:25.000000 resoto-plugin-aws-k8s-3.5.1/resoto_plugin_aws_k8s.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-02 14:57:25.000000 resoto-plugin-aws-k8s-3.5.1/resoto_plugin_aws_k8s.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:54:57.000000 resoto-plugin-aws-k8s-3.5.1/resoto_plugin_aws_k8s.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-02 14:57:25.000000 resoto-plugin-aws-k8s-3.5.1/resoto_plugin_aws_k8s.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-02 14:57:25.000000 resoto-plugin-aws-k8s-3.5.1/resoto_plugin_aws_k8s.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-02 14:57:25.795444 resoto-plugin-aws-k8s-3.5.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:57:25.795444 resoto-plugin-aws-k8s-3.5.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 14:53:44.000000 resoto-plugin-aws-k8s-3.5.1/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-02 14:53:44.000000 resoto-plugin-aws-k8s-3.5.1/test/test_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:06:39.348255 resoto-plugin-aws-k8s-3.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-13 13:03:04.000000 resoto-plugin-aws-k8s-3.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-13 13:06:39.348255 resoto-plugin-aws-k8s-3.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-13 13:03:04.000000 resoto-plugin-aws-k8s-3.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-06-13 13:03:04.000000 resoto-plugin-aws-k8s-3.5.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:06:39.348255 resoto-plugin-aws-k8s-3.5.2/resoto_plugin_aws_k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-06-13 13:03:04.000000 resoto-plugin-aws-k8s-3.5.2/resoto_plugin_aws_k8s/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:06:39.348255 resoto-plugin-aws-k8s-3.5.2/resoto_plugin_aws_k8s.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-13 13:06:39.000000 resoto-plugin-aws-k8s-3.5.2/resoto_plugin_aws_k8s.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-13 13:06:39.000000 resoto-plugin-aws-k8s-3.5.2/resoto_plugin_aws_k8s.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 13:06:39.000000 resoto-plugin-aws-k8s-3.5.2/resoto_plugin_aws_k8s.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-13 13:06:39.000000 resoto-plugin-aws-k8s-3.5.2/resoto_plugin_aws_k8s.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 13:04:11.000000 resoto-plugin-aws-k8s-3.5.2/resoto_plugin_aws_k8s.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-13 13:06:39.000000 resoto-plugin-aws-k8s-3.5.2/resoto_plugin_aws_k8s.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-13 13:06:39.000000 resoto-plugin-aws-k8s-3.5.2/resoto_plugin_aws_k8s.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-13 13:06:39.348255 resoto-plugin-aws-k8s-3.5.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:06:39.348255 resoto-plugin-aws-k8s-3.5.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:03:04.000000 resoto-plugin-aws-k8s-3.5.2/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-13 13:03:04.000000 resoto-plugin-aws-k8s-3.5.2/test/test_collector.py
```

### Comparing `resoto-plugin-aws-k8s-3.5.1/PKG-INFO` & `resoto-plugin-aws-k8s-3.5.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-aws-k8s
-Version: 3.5.1
+Version: 3.5.2
 Summary: Resoto AWS-K8s Collector Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/aws_k8s
 Keywords: aws,k8s
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
```

### Comparing `resoto-plugin-aws-k8s-3.5.1/pyproject.toml` & `resoto-plugin-aws-k8s-3.5.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "resoto-plugin-aws-k8s"
-version = "3.5.1"
+version = "3.5.2"
 authors = [{name="Some Engineering Inc."}]
 description = "Resoto AWS-K8s Collector Plugin"
 license = {file="LICENSE"}
 requires-python = ">=3.9"
 classifiers = [
     # Current project status
     "Development Status :: 4 - Beta",
@@ -23,15 +23,15 @@
     "Natural Language :: English",
     "Topic :: Security",
     "Topic :: Utilities",
 ]
 readme = {file="README.md", content-type="text/markdown"}
 keywords = ["aws", "k8s"]
 
-dependencies = [ "resotolib==3.5.1" ]
+dependencies = [ "resotolib==3.5.2" ]
 
 [project.optional-dependencies]
 dev = [ "mypy" ]
 
 [project.entry-points."resoto.plugins"]
 aws_k8s_collector = "resoto_plugin_aws_k8s:AWSK8sCollectorPlugin"
```

### Comparing `resoto-plugin-aws-k8s-3.5.1/resoto_plugin_aws_k8s/__init__.py` & `resoto-plugin-aws-k8s-3.5.2/resoto_plugin_aws_k8s/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-k8s-3.5.1/resoto_plugin_aws_k8s.egg-info/PKG-INFO` & `resoto-plugin-aws-k8s-3.5.2/resoto_plugin_aws_k8s.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-aws-k8s
-Version: 3.5.1
+Version: 3.5.2
 Summary: Resoto AWS-K8s Collector Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/aws_k8s
 Keywords: aws,k8s
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
```

### Comparing `resoto-plugin-aws-k8s-3.5.1/test/test_collector.py` & `resoto-plugin-aws-k8s-3.5.2/test/test_collector.py`

 * *Files identical despite different names*

