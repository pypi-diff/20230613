# Comparing `tmp/resoto-plugin-digitalocean-3.5.1.tar.gz` & `tmp/resoto-plugin-digitalocean-3.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-digitalocean-3.5.1.tar", last modified: Fri Jun  2 14:55:23 2023, max compression
+gzip compressed data, was "resoto-plugin-digitalocean-3.5.2.tar", last modified: Tue Jun 13 13:11:38 2023, max compression
```

## Comparing `resoto-plugin-digitalocean-3.5.1.tar` & `resoto-plugin-digitalocean-3.5.2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:55:23.034830 resoto-plugin-digitalocean-3.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-02 14:49:58.000000 resoto-plugin-digitalocean-3.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-02 14:55:23.034830 resoto-plugin-digitalocean-3.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-02 14:49:58.000000 resoto-plugin-digitalocean-3.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-06-02 14:49:58.000000 resoto-plugin-digitalocean-3.5.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:55:23.026830 resoto-plugin-digitalocean-3.5.1/resoto_plugin_digitalocean/
--rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-06-02 14:49:58.000000 resoto-plugin-digitalocean-3.5.1/resoto_plugin_digitalocean/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15090 2023-06-02 14:49:58.000000 resoto-plugin-digitalocean-3.5.1/resoto_plugin_digitalocean/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    43638 2023-06-02 14:49:58.000000 resoto-plugin-digitalocean-3.5.1/resoto_plugin_digitalocean/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-02 14:49:58.000000 resoto-plugin-digitalocean-3.5.1/resoto_plugin_digitalocean/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    19972 2023-06-02 14:49:58.000000 resoto-plugin-digitalocean-3.5.1/resoto_plugin_digitalocean/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-06-02 14:49:58.000000 resoto-plugin-digitalocean-3.5.1/resoto_plugin_digitalocean/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:55:23.026830 resoto-plugin-digitalocean-3.5.1/resoto_plugin_digitalocean.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-02 14:55:23.000000 resoto-plugin-digitalocean-3.5.1/resoto_plugin_digitalocean.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-02 14:55:23.000000 resoto-plugin-digitalocean-3.5.1/resoto_plugin_digitalocean.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:55:23.000000 resoto-plugin-digitalocean-3.5.1/resoto_plugin_digitalocean.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-02 14:55:23.000000 resoto-plugin-digitalocean-3.5.1/resoto_plugin_digitalocean.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:51:36.000000 resoto-plugin-digitalocean-3.5.1/resoto_plugin_digitalocean.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-02 14:55:23.000000 resoto-plugin-digitalocean-3.5.1/resoto_plugin_digitalocean.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-02 14:55:23.000000 resoto-plugin-digitalocean-3.5.1/resoto_plugin_digitalocean.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-02 14:55:23.034830 resoto-plugin-digitalocean-3.5.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:55:23.030830 resoto-plugin-digitalocean-3.5.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 14:49:58.000000 resoto-plugin-digitalocean-3.5.1/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:55:23.034830 resoto-plugin-digitalocean-3.5.1/test/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-02 14:49:58.000000 resoto-plugin-digitalocean-3.5.1/test/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-02 14:49:58.000000 resoto-plugin-digitalocean-3.5.1/test/fixtures/alerts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-06-02 14:49:58.000000 resoto-plugin-digitalocean-3.5.1/test/fixtures/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-02 14:49:58.000000 resoto-plugin-digitalocean-3.5.1/test/fixtures/cdns.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-02 14:49:58.000000 resoto-plugin-digitalocean-3.5.1/test/fixtures/certificates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-06-02 14:49:58.000000 resoto-plugin-digitalocean-3.5.1/test/fixtures/databases.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-06-02 14:49:58.000000 resoto-plugin-digitalocean-3.5.1/test/fixtures/domain_records.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-02 14:49:58.000000 resoto-plugin-digitalocean-3.5.1/test/fixtures/domains.py
--rw-r--r--   0 runner    (1001) docker     (123)    10579 2023-06-02 14:49:58.000000 resoto-plugin-digitalocean-3.5.1/test/fixtures/droplets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-06-02 14:49:58.000000 resoto-plugin-digitalocean-3.5.1/test/fixtures/firewalls.py
--rw-r--r--   0 runner    (1001) docker     (123)     8942 2023-06-02 14:49:58.000000 resoto-plugin-digitalocean-3.5.1/test/fixtures/floatingip.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-06-02 14:49:58.000000 resoto-plugin-digitalocean-3.5.1/test/fixtures/k8s.py
--rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-06-02 14:49:58.000000 resoto-plugin-digitalocean-3.5.1/test/fixtures/loadbalancers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-06-02 14:49:58.000000 resoto-plugin-digitalocean-3.5.1/test/fixtures/projectresources.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-02 14:49:58.000000 resoto-plugin-digitalocean-3.5.1/test/fixtures/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-06-02 14:49:58.000000 resoto-plugin-digitalocean-3.5.1/test/fixtures/regions.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-02 14:49:58.000000 resoto-plugin-digitalocean-3.5.1/test/fixtures/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-06-02 14:49:58.000000 resoto-plugin-digitalocean-3.5.1/test/fixtures/registry_repositories.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-02 14:49:58.000000 resoto-plugin-digitalocean-3.5.1/test/fixtures/registry_repository_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-02 14:49:58.000000 resoto-plugin-digitalocean-3.5.1/test/fixtures/snapshots.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-02 14:49:58.000000 resoto-plugin-digitalocean-3.5.1/test/fixtures/spaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-02 14:49:58.000000 resoto-plugin-digitalocean-3.5.1/test/fixtures/ssh_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-06-02 14:49:58.000000 resoto-plugin-digitalocean-3.5.1/test/fixtures/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-06-02 14:49:58.000000 resoto-plugin-digitalocean-3.5.1/test/fixtures/volumes.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-02 14:49:58.000000 resoto-plugin-digitalocean-3.5.1/test/fixtures/vpcs.py
--rw-r--r--   0 runner    (1001) docker     (123)    25604 2023-06-02 14:49:58.000000 resoto-plugin-digitalocean-3.5.1/test/test_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-02 14:49:58.000000 resoto-plugin-digitalocean-3.5.1/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:11:38.992960 resoto-plugin-digitalocean-3.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-13 13:07:31.000000 resoto-plugin-digitalocean-3.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-13 13:11:38.992960 resoto-plugin-digitalocean-3.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-13 13:07:31.000000 resoto-plugin-digitalocean-3.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-06-13 13:07:31.000000 resoto-plugin-digitalocean-3.5.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:11:38.988960 resoto-plugin-digitalocean-3.5.2/resoto_plugin_digitalocean/
+-rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-06-13 13:07:31.000000 resoto-plugin-digitalocean-3.5.2/resoto_plugin_digitalocean/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15090 2023-06-13 13:07:31.000000 resoto-plugin-digitalocean-3.5.2/resoto_plugin_digitalocean/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43638 2023-06-13 13:07:31.000000 resoto-plugin-digitalocean-3.5.2/resoto_plugin_digitalocean/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-13 13:07:31.000000 resoto-plugin-digitalocean-3.5.2/resoto_plugin_digitalocean/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19972 2023-06-13 13:07:31.000000 resoto-plugin-digitalocean-3.5.2/resoto_plugin_digitalocean/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-06-13 13:07:31.000000 resoto-plugin-digitalocean-3.5.2/resoto_plugin_digitalocean/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:11:38.988960 resoto-plugin-digitalocean-3.5.2/resoto_plugin_digitalocean.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-13 13:11:38.000000 resoto-plugin-digitalocean-3.5.2/resoto_plugin_digitalocean.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-13 13:11:38.000000 resoto-plugin-digitalocean-3.5.2/resoto_plugin_digitalocean.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 13:11:38.000000 resoto-plugin-digitalocean-3.5.2/resoto_plugin_digitalocean.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-13 13:11:38.000000 resoto-plugin-digitalocean-3.5.2/resoto_plugin_digitalocean.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 13:08:56.000000 resoto-plugin-digitalocean-3.5.2/resoto_plugin_digitalocean.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-13 13:11:38.000000 resoto-plugin-digitalocean-3.5.2/resoto_plugin_digitalocean.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-13 13:11:38.000000 resoto-plugin-digitalocean-3.5.2/resoto_plugin_digitalocean.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-13 13:11:38.992960 resoto-plugin-digitalocean-3.5.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:11:38.992960 resoto-plugin-digitalocean-3.5.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:31.000000 resoto-plugin-digitalocean-3.5.2/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:11:38.992960 resoto-plugin-digitalocean-3.5.2/test/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-13 13:07:31.000000 resoto-plugin-digitalocean-3.5.2/test/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-13 13:07:31.000000 resoto-plugin-digitalocean-3.5.2/test/fixtures/alerts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-06-13 13:07:31.000000 resoto-plugin-digitalocean-3.5.2/test/fixtures/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-13 13:07:31.000000 resoto-plugin-digitalocean-3.5.2/test/fixtures/cdns.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-13 13:07:31.000000 resoto-plugin-digitalocean-3.5.2/test/fixtures/certificates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-06-13 13:07:31.000000 resoto-plugin-digitalocean-3.5.2/test/fixtures/databases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-06-13 13:07:31.000000 resoto-plugin-digitalocean-3.5.2/test/fixtures/domain_records.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-13 13:07:31.000000 resoto-plugin-digitalocean-3.5.2/test/fixtures/domains.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10579 2023-06-13 13:07:31.000000 resoto-plugin-digitalocean-3.5.2/test/fixtures/droplets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-06-13 13:07:31.000000 resoto-plugin-digitalocean-3.5.2/test/fixtures/firewalls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8942 2023-06-13 13:07:31.000000 resoto-plugin-digitalocean-3.5.2/test/fixtures/floatingip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-06-13 13:07:31.000000 resoto-plugin-digitalocean-3.5.2/test/fixtures/k8s.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-06-13 13:07:31.000000 resoto-plugin-digitalocean-3.5.2/test/fixtures/loadbalancers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-06-13 13:07:31.000000 resoto-plugin-digitalocean-3.5.2/test/fixtures/projectresources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-13 13:07:31.000000 resoto-plugin-digitalocean-3.5.2/test/fixtures/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-06-13 13:07:31.000000 resoto-plugin-digitalocean-3.5.2/test/fixtures/regions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-13 13:07:31.000000 resoto-plugin-digitalocean-3.5.2/test/fixtures/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-06-13 13:07:31.000000 resoto-plugin-digitalocean-3.5.2/test/fixtures/registry_repositories.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-13 13:07:31.000000 resoto-plugin-digitalocean-3.5.2/test/fixtures/registry_repository_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-13 13:07:31.000000 resoto-plugin-digitalocean-3.5.2/test/fixtures/snapshots.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-13 13:07:31.000000 resoto-plugin-digitalocean-3.5.2/test/fixtures/spaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-13 13:07:31.000000 resoto-plugin-digitalocean-3.5.2/test/fixtures/ssh_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-06-13 13:07:31.000000 resoto-plugin-digitalocean-3.5.2/test/fixtures/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-06-13 13:07:31.000000 resoto-plugin-digitalocean-3.5.2/test/fixtures/volumes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-13 13:07:31.000000 resoto-plugin-digitalocean-3.5.2/test/fixtures/vpcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25604 2023-06-13 13:07:31.000000 resoto-plugin-digitalocean-3.5.2/test/test_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-13 13:07:31.000000 resoto-plugin-digitalocean-3.5.2/test/test_config.py
```

### Comparing `resoto-plugin-digitalocean-3.5.1/PKG-INFO` & `resoto-plugin-digitalocean-3.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-digitalocean
-Version: 3.5.1
+Version: 3.5.2
 Summary: Resoto DigitalOcean Collector Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/digitalocean
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-digitalocean-3.5.1/pyproject.toml` & `resoto-plugin-digitalocean-3.5.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "resoto-plugin-digitalocean"
 description = "Resoto DigitalOcean Collector Plugin"
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
     "boto3",
     "requests",
     "botocore",
     "retrying"
 ]
 
 [project.optional-dependencies]
```

### Comparing `resoto-plugin-digitalocean-3.5.1/resoto_plugin_digitalocean/__init__.py` & `resoto-plugin-digitalocean-3.5.2/resoto_plugin_digitalocean/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.5.1/resoto_plugin_digitalocean/client.py` & `resoto-plugin-digitalocean-3.5.2/resoto_plugin_digitalocean/client.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.5.1/resoto_plugin_digitalocean/collector.py` & `resoto-plugin-digitalocean-3.5.2/resoto_plugin_digitalocean/collector.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.5.1/resoto_plugin_digitalocean/resources.py` & `resoto-plugin-digitalocean-3.5.2/resoto_plugin_digitalocean/resources.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.5.1/resoto_plugin_digitalocean/utils.py` & `resoto-plugin-digitalocean-3.5.2/resoto_plugin_digitalocean/utils.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.5.1/resoto_plugin_digitalocean.egg-info/PKG-INFO` & `resoto-plugin-digitalocean-3.5.2/resoto_plugin_digitalocean.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-digitalocean
-Version: 3.5.1
+Version: 3.5.2
 Summary: Resoto DigitalOcean Collector Plugin
 Author: Some Engineering Inc.
 Project-URL: Documentation, https://resoto.com
 Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/digitalocean
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-digitalocean-3.5.1/resoto_plugin_digitalocean.egg-info/SOURCES.txt` & `resoto-plugin-digitalocean-3.5.2/resoto_plugin_digitalocean.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.5.1/test/fixtures/__init__.py` & `resoto-plugin-digitalocean-3.5.2/test/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.5.1/test/fixtures/apps.py` & `resoto-plugin-digitalocean-3.5.2/test/fixtures/apps.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.5.1/test/fixtures/databases.py` & `resoto-plugin-digitalocean-3.5.2/test/fixtures/databases.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.5.1/test/fixtures/domain_records.py` & `resoto-plugin-digitalocean-3.5.2/test/fixtures/domain_records.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.5.1/test/fixtures/droplets.py` & `resoto-plugin-digitalocean-3.5.2/test/fixtures/droplets.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.5.1/test/fixtures/firewalls.py` & `resoto-plugin-digitalocean-3.5.2/test/fixtures/firewalls.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.5.1/test/fixtures/floatingip.py` & `resoto-plugin-digitalocean-3.5.2/test/fixtures/floatingip.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.5.1/test/fixtures/k8s.py` & `resoto-plugin-digitalocean-3.5.2/test/fixtures/k8s.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.5.1/test/fixtures/loadbalancers.py` & `resoto-plugin-digitalocean-3.5.2/test/fixtures/loadbalancers.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.5.1/test/fixtures/projectresources.py` & `resoto-plugin-digitalocean-3.5.2/test/fixtures/projectresources.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.5.1/test/fixtures/projects.py` & `resoto-plugin-digitalocean-3.5.2/test/fixtures/projects.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.5.1/test/fixtures/regions.py` & `resoto-plugin-digitalocean-3.5.2/test/fixtures/regions.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.5.1/test/fixtures/registry_repositories.py` & `resoto-plugin-digitalocean-3.5.2/test/fixtures/registry_repositories.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.5.1/test/fixtures/tags.py` & `resoto-plugin-digitalocean-3.5.2/test/fixtures/tags.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.5.1/test/fixtures/volumes.py` & `resoto-plugin-digitalocean-3.5.2/test/fixtures/volumes.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.5.1/test/test_collector.py` & `resoto-plugin-digitalocean-3.5.2/test/test_collector.py`

 * *Files identical despite different names*

