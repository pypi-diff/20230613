# Comparing `tmp/pulumi_rke-3.3.0a1686291919.tar.gz` & `tmp/pulumi_rke-3.3.0a1686638253.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_rke-3.3.0a1686291919.tar", last modified: Fri Jun  9 06:37:54 2023, max compression
+gzip compressed data, was "pulumi_rke-3.3.0a1686638253.tar", last modified: Tue Jun 13 06:47:37 2023, max compression
```

## Comparing `pulumi_rke-3.3.0a1686291919.tar` & `pulumi_rke-3.3.0a1686638253.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:37:54.559623 pulumi_rke-3.3.0a1686291919/
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-06-09 06:37:54.559623 pulumi_rke-3.3.0a1686291919/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-06-09 06:37:54.000000 pulumi_rke-3.3.0a1686291919/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:37:54.555623 pulumi_rke-3.3.0a1686291919/pulumi_rke/
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-09 06:37:54.000000 pulumi_rke-3.3.0a1686291919/pulumi_rke/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   393841 2023-06-09 06:37:54.000000 pulumi_rke-3.3.0a1686291919/pulumi_rke/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7667 2023-06-09 06:37:54.000000 pulumi_rke-3.3.0a1686291919/pulumi_rke/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)   132925 2023-06-09 06:37:54.000000 pulumi_rke-3.3.0a1686291919/pulumi_rke/cluster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:37:54.559623 pulumi_rke-3.3.0a1686291919/pulumi_rke/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-09 06:37:54.000000 pulumi_rke-3.3.0a1686291919/pulumi_rke/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-09 06:37:54.000000 pulumi_rke-3.3.0a1686291919/pulumi_rke/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)   355040 2023-06-09 06:37:54.000000 pulumi_rke-3.3.0a1686291919/pulumi_rke/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-06-09 06:37:54.000000 pulumi_rke-3.3.0a1686291919/pulumi_rke/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-09 06:37:54.000000 pulumi_rke-3.3.0a1686291919/pulumi_rke/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 06:37:54.000000 pulumi_rke-3.3.0a1686291919/pulumi_rke/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:37:54.559623 pulumi_rke-3.3.0a1686291919/pulumi_rke.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-06-09 06:37:54.000000 pulumi_rke-3.3.0a1686291919/pulumi_rke.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-09 06:37:54.000000 pulumi_rke-3.3.0a1686291919/pulumi_rke.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 06:37:54.000000 pulumi_rke-3.3.0a1686291919/pulumi_rke.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 06:37:54.000000 pulumi_rke-3.3.0a1686291919/pulumi_rke.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-09 06:37:54.000000 pulumi_rke-3.3.0a1686291919/pulumi_rke.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-09 06:37:54.000000 pulumi_rke-3.3.0a1686291919/pulumi_rke.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 06:37:54.559623 pulumi_rke-3.3.0a1686291919/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-06-09 06:37:54.000000 pulumi_rke-3.3.0a1686291919/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:47:37.743987 pulumi_rke-3.3.0a1686638253/
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-06-13 06:47:37.743987 pulumi_rke-3.3.0a1686638253/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-06-13 06:47:37.000000 pulumi_rke-3.3.0a1686638253/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:47:37.735987 pulumi_rke-3.3.0a1686638253/pulumi_rke/
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-13 06:47:37.000000 pulumi_rke-3.3.0a1686638253/pulumi_rke/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   393841 2023-06-13 06:47:37.000000 pulumi_rke-3.3.0a1686638253/pulumi_rke/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7667 2023-06-13 06:47:37.000000 pulumi_rke-3.3.0a1686638253/pulumi_rke/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)   132925 2023-06-13 06:47:37.000000 pulumi_rke-3.3.0a1686638253/pulumi_rke/cluster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:47:37.739987 pulumi_rke-3.3.0a1686638253/pulumi_rke/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-13 06:47:37.000000 pulumi_rke-3.3.0a1686638253/pulumi_rke/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-13 06:47:37.000000 pulumi_rke-3.3.0a1686638253/pulumi_rke/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)   355040 2023-06-13 06:47:37.000000 pulumi_rke-3.3.0a1686638253/pulumi_rke/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-06-13 06:47:37.000000 pulumi_rke-3.3.0a1686638253/pulumi_rke/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-13 06:47:37.000000 pulumi_rke-3.3.0a1686638253/pulumi_rke/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 06:47:37.000000 pulumi_rke-3.3.0a1686638253/pulumi_rke/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:47:37.739987 pulumi_rke-3.3.0a1686638253/pulumi_rke.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-06-13 06:47:37.000000 pulumi_rke-3.3.0a1686638253/pulumi_rke.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-13 06:47:37.000000 pulumi_rke-3.3.0a1686638253/pulumi_rke.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 06:47:37.000000 pulumi_rke-3.3.0a1686638253/pulumi_rke.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 06:47:37.000000 pulumi_rke-3.3.0a1686638253/pulumi_rke.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-13 06:47:37.000000 pulumi_rke-3.3.0a1686638253/pulumi_rke.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-13 06:47:37.000000 pulumi_rke-3.3.0a1686638253/pulumi_rke.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 06:47:37.743987 pulumi_rke-3.3.0a1686638253/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-06-13 06:47:37.000000 pulumi_rke-3.3.0a1686638253/setup.py
```

### Comparing `pulumi_rke-3.3.0a1686291919/PKG-INFO` & `pulumi_rke-3.3.0a1686638253/pulumi_rke.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pulumi_rke
-Version: 3.3.0a1686291919
+Name: pulumi-rke
+Version: 3.3.0a1686638253
 Summary: A Pulumi package for creating and managing rke cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-rke
 Keywords: pulumi rke
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_rke-3.3.0a1686291919/README.md` & `pulumi_rke-3.3.0a1686638253/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_rke-3.3.0a1686291919/pulumi_rke/__init__.py` & `pulumi_rke-3.3.0a1686638253/pulumi_rke/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_rke-3.3.0a1686291919/pulumi_rke/_inputs.py` & `pulumi_rke-3.3.0a1686638253/pulumi_rke/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_rke-3.3.0a1686291919/pulumi_rke/_utilities.py` & `pulumi_rke-3.3.0a1686638253/pulumi_rke/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_rke-3.3.0a1686291919/pulumi_rke/cluster.py` & `pulumi_rke-3.3.0a1686638253/pulumi_rke/cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_rke-3.3.0a1686291919/pulumi_rke/config/vars.py` & `pulumi_rke-3.3.0a1686638253/pulumi_rke/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_rke-3.3.0a1686291919/pulumi_rke/outputs.py` & `pulumi_rke-3.3.0a1686638253/pulumi_rke/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_rke-3.3.0a1686291919/pulumi_rke/provider.py` & `pulumi_rke-3.3.0a1686638253/pulumi_rke/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_rke-3.3.0a1686291919/pulumi_rke.egg-info/PKG-INFO` & `pulumi_rke-3.3.0a1686638253/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pulumi-rke
-Version: 3.3.0a1686291919
+Name: pulumi_rke
+Version: 3.3.0a1686638253
 Summary: A Pulumi package for creating and managing rke cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-rke
 Keywords: pulumi rke
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_rke-3.3.0a1686291919/setup.py` & `pulumi_rke-3.3.0a1686638253/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "3.3.0a1686291919"
-PLUGIN_VERSION = "3.3.0-alpha.1686291919+8f220d71"
+VERSION = "3.3.0a1686638253"
+PLUGIN_VERSION = "3.3.0-alpha.1686638253+e0d150d0"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'rke', PLUGIN_VERSION])
         except OSError as error:
```

