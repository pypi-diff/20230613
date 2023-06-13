# Comparing `tmp/resoto-plugin-example-collector-3.5.0.tar.gz` & `tmp/resoto-plugin-example-collector-3.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-example-collector-3.5.0.tar", last modified: Fri May 26 18:27:01 2023, max compression
+gzip compressed data, was "resoto-plugin-example-collector-3.5.1.tar", last modified: Fri Jun  2 14:52:53 2023, max compression
```

## Comparing `resoto-plugin-example-collector-3.5.0.tar` & `resoto-plugin-example-collector-3.5.1.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:27:01.867364 resoto-plugin-example-collector-3.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-26 18:24:53.000000 resoto-plugin-example-collector-3.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-26 18:27:01.867364 resoto-plugin-example-collector-3.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-26 18:24:53.000000 resoto-plugin-example-collector-3.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-26 18:24:53.000000 resoto-plugin-example-collector-3.5.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:27:01.867364 resoto-plugin-example-collector-3.5.0/resoto_plugin_example_collector/
--rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-05-26 18:24:53.000000 resoto-plugin-example-collector-3.5.0/resoto_plugin_example_collector/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:27:01.867364 resoto-plugin-example-collector-3.5.0/resoto_plugin_example_collector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-26 18:27:01.000000 resoto-plugin-example-collector-3.5.0/resoto_plugin_example_collector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-26 18:27:01.000000 resoto-plugin-example-collector-3.5.0/resoto_plugin_example_collector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:27:01.000000 resoto-plugin-example-collector-3.5.0/resoto_plugin_example_collector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-26 18:27:01.000000 resoto-plugin-example-collector-3.5.0/resoto_plugin_example_collector.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:27:01.000000 resoto-plugin-example-collector-3.5.0/resoto_plugin_example_collector.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-26 18:27:01.000000 resoto-plugin-example-collector-3.5.0/resoto_plugin_example_collector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-26 18:27:01.000000 resoto-plugin-example-collector-3.5.0/resoto_plugin_example_collector.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-26 18:27:01.867364 resoto-plugin-example-collector-3.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-26 18:24:53.000000 resoto-plugin-example-collector-3.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:27:01.867364 resoto-plugin-example-collector-3.5.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-26 18:24:53.000000 resoto-plugin-example-collector-3.5.0/test/test_args.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-26 18:24:53.000000 resoto-plugin-example-collector-3.5.0/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:52:53.880910 resoto-plugin-example-collector-3.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-02 14:49:28.000000 resoto-plugin-example-collector-3.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-06-02 14:52:53.880910 resoto-plugin-example-collector-3.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-02 14:49:28.000000 resoto-plugin-example-collector-3.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-06-02 14:49:28.000000 resoto-plugin-example-collector-3.5.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:52:53.880910 resoto-plugin-example-collector-3.5.1/resoto_plugin_example_collector/
+-rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-06-02 14:49:28.000000 resoto-plugin-example-collector-3.5.1/resoto_plugin_example_collector/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:52:53.880910 resoto-plugin-example-collector-3.5.1/resoto_plugin_example_collector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-06-02 14:52:53.000000 resoto-plugin-example-collector-3.5.1/resoto_plugin_example_collector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-02 14:52:53.000000 resoto-plugin-example-collector-3.5.1/resoto_plugin_example_collector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:52:53.000000 resoto-plugin-example-collector-3.5.1/resoto_plugin_example_collector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-02 14:52:53.000000 resoto-plugin-example-collector-3.5.1/resoto_plugin_example_collector.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:50:54.000000 resoto-plugin-example-collector-3.5.1/resoto_plugin_example_collector.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-02 14:52:53.000000 resoto-plugin-example-collector-3.5.1/resoto_plugin_example_collector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-02 14:52:53.000000 resoto-plugin-example-collector-3.5.1/resoto_plugin_example_collector.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-02 14:52:53.880910 resoto-plugin-example-collector-3.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:52:53.880910 resoto-plugin-example-collector-3.5.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-02 14:49:28.000000 resoto-plugin-example-collector-3.5.1/test/test_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-02 14:49:28.000000 resoto-plugin-example-collector-3.5.1/test/test_config.py
```

### Comparing `resoto-plugin-example-collector-3.5.0/PKG-INFO` & `resoto-plugin-example-collector-3.5.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-example-collector
-Version: 3.5.0
+Version: 3.5.1
 Summary: Resoto Example Collector Plugin
-Home-page: https://github.com/someengineering/resoto/tree/main/plugins/example_collector
-License: Apache 2.0
-Keywords: cloud security
+Author: Some Engineering Inc.
+Project-URL: Documentation, https://resoto.com
+Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/example_collector
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # resoto-plugin-example-collector
 Example Collector Plugin for Resoto
```

### Comparing `resoto-plugin-example-collector-3.5.0/resoto_plugin_example_collector/__init__.py` & `resoto-plugin-example-collector-3.5.1/resoto_plugin_example_collector/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-example-collector-3.5.0/resoto_plugin_example_collector.egg-info/PKG-INFO` & `resoto-plugin-example-collector-3.5.1/resoto_plugin_example_collector.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-example-collector
-Version: 3.5.0
+Version: 3.5.1
 Summary: Resoto Example Collector Plugin
-Home-page: https://github.com/someengineering/resoto/tree/main/plugins/example_collector
-License: Apache 2.0
-Keywords: cloud security
+Author: Some Engineering Inc.
+Project-URL: Documentation, https://resoto.com
+Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/example_collector
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # resoto-plugin-example-collector
 Example Collector Plugin for Resoto
```

### Comparing `resoto-plugin-example-collector-3.5.0/resoto_plugin_example_collector.egg-info/SOURCES.txt` & `resoto-plugin-example-collector-3.5.1/resoto_plugin_example_collector.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 MANIFEST.in
 README.md
-requirements.txt
+pyproject.toml
 setup.cfg
-setup.py
 resoto_plugin_example_collector/__init__.py
 resoto_plugin_example_collector.egg-info/PKG-INFO
 resoto_plugin_example_collector.egg-info/SOURCES.txt
 resoto_plugin_example_collector.egg-info/dependency_links.txt
 resoto_plugin_example_collector.egg-info/entry_points.txt
 resoto_plugin_example_collector.egg-info/not-zip-safe
 resoto_plugin_example_collector.egg-info/requires.txt
```

