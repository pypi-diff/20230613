# Comparing `tmp/vents-0.1.3.tar.gz` & `tmp/vents-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vents-0.1.3.tar", last modified: Thu Jun  8 10:21:35 2023, max compression
+gzip compressed data, was "vents-0.1.4.tar", last modified: Tue Jun 13 13:29:09 2023, max compression
```

## Comparing `vents-0.1.3.tar` & `vents-0.1.4.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-06-08 10:21:35.418310 vents-0.1.3/
--rw-r--r--   0 mourad     (501) staff       (20)      172 2023-06-08 10:20:54.000000 vents-0.1.3/MANIFEST.in
--rw-r--r--   0 mourad     (501) staff       (20)     1568 2023-06-08 10:21:35.418379 vents-0.1.3/PKG-INFO
--rw-r--r--   0 mourad     (501) staff       (20)     1031 2023-06-08 10:21:35.418774 vents-0.1.3/setup.cfg
--rw-r--r--   0 mourad     (501) staff       (20)     2695 2023-06-08 10:20:54.000000 vents-0.1.3/setup.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-06-08 10:21:35.413614 vents-0.1.3/vents/
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-06-08 10:20:54.000000 vents-0.1.3/vents/__init__.py
--rw-r--r--   0 mourad     (501) staff       (20)     4857 2023-06-08 10:20:54.000000 vents-0.1.3/vents/config.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-06-08 10:21:35.415112 vents-0.1.3/vents/connections/
--rw-r--r--   0 mourad     (501) staff       (20)      335 2023-06-08 10:20:54.000000 vents-0.1.3/vents/connections/__init__.py
--rw-r--r--   0 mourad     (501) staff       (20)     2485 2023-06-08 10:20:54.000000 vents-0.1.3/vents/connections/catalog.py
--rw-r--r--   0 mourad     (501) staff       (20)     3842 2023-06-08 10:20:54.000000 vents-0.1.3/vents/connections/connection.py
--rw-r--r--   0 mourad     (501) staff       (20)      513 2023-06-08 10:20:54.000000 vents-0.1.3/vents/connections/connection_resource.py
--rw-r--r--   0 mourad     (501) staff       (20)     3301 2023-06-08 10:20:54.000000 vents-0.1.3/vents/connections/connection_schema.py
--rw-r--r--   0 mourad     (501) staff       (20)       37 2023-06-08 10:20:54.000000 vents-0.1.3/vents/exceptions.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-06-08 10:21:35.416350 vents-0.1.3/vents/notifiers/
--rw-r--r--   0 mourad     (501) staff       (20)      866 2023-06-08 10:20:54.000000 vents-0.1.3/vents/notifiers/__init__.py
--rw-r--r--   0 mourad     (501) staff       (20)     4589 2023-06-08 10:20:54.000000 vents-0.1.3/vents/notifiers/base.py
--rw-r--r--   0 mourad     (501) staff       (20)     1303 2023-06-08 10:20:54.000000 vents-0.1.3/vents/notifiers/discord_webhook.py
--rw-r--r--   0 mourad     (501) staff       (20)     1277 2023-06-08 10:20:54.000000 vents-0.1.3/vents/notifiers/hipchat_webhook.py
--rw-r--r--   0 mourad     (501) staff       (20)     1764 2023-06-08 10:20:54.000000 vents-0.1.3/vents/notifiers/mattermost_webhook.py
--rw-r--r--   0 mourad     (501) staff       (20)     1723 2023-06-08 10:20:54.000000 vents-0.1.3/vents/notifiers/pagerduty_webhook.py
--rw-r--r--   0 mourad     (501) staff       (20)     2051 2023-06-08 10:20:54.000000 vents-0.1.3/vents/notifiers/slack_webhook.py
--rw-r--r--   0 mourad     (501) staff       (20)      372 2023-06-08 10:20:54.000000 vents-0.1.3/vents/notifiers/spec.py
--rw-r--r--   0 mourad     (501) staff       (20)     1847 2023-06-08 10:20:54.000000 vents-0.1.3/vents/notifiers/webhook.py
--rw-r--r--   0 mourad     (501) staff       (20)      233 2023-06-08 10:20:54.000000 vents-0.1.3/vents/pkg.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-06-08 10:21:35.416710 vents-0.1.3/vents/providers/
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-06-08 10:20:54.000000 vents-0.1.3/vents/providers/__init__.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-06-08 10:21:35.417217 vents-0.1.3/vents/providers/aws/
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-06-08 10:20:54.000000 vents-0.1.3/vents/providers/aws/__init__.py
--rw-r--r--   0 mourad     (501) staff       (20)     3724 2023-06-08 10:20:54.000000 vents-0.1.3/vents/providers/aws/base.py
--rw-r--r--   0 mourad     (501) staff       (20)     1656 2023-06-08 10:20:54.000000 vents-0.1.3/vents/providers/aws/s3.py
--rw-r--r--   0 mourad     (501) staff       (20)     3456 2023-06-08 10:20:54.000000 vents-0.1.3/vents/providers/aws/service.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-06-08 10:21:35.417708 vents-0.1.3/vents/providers/azure/
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-06-08 10:20:54.000000 vents-0.1.3/vents/providers/azure/__init__.py
--rw-r--r--   0 mourad     (501) staff       (20)     2609 2023-06-08 10:20:54.000000 vents-0.1.3/vents/providers/azure/base.py
--rw-r--r--   0 mourad     (501) staff       (20)     1831 2023-06-08 10:20:54.000000 vents-0.1.3/vents/providers/azure/blob_storage.py
--rw-r--r--   0 mourad     (501) staff       (20)     2251 2023-06-08 10:20:54.000000 vents-0.1.3/vents/providers/azure/service.py
--rw-r--r--   0 mourad     (501) staff       (20)     1620 2023-06-08 10:20:54.000000 vents-0.1.3/vents/providers/base.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-06-08 10:21:35.418192 vents-0.1.3/vents/providers/gcp/
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-06-08 10:20:54.000000 vents-0.1.3/vents/providers/gcp/__init__.py
--rw-r--r--   0 mourad     (501) staff       (20)     3750 2023-06-08 10:20:54.000000 vents-0.1.3/vents/providers/gcp/base.py
--rw-r--r--   0 mourad     (501) staff       (20)      995 2023-06-08 10:20:54.000000 vents-0.1.3/vents/providers/gcp/gcs.py
--rw-r--r--   0 mourad     (501) staff       (20)     2513 2023-06-08 10:20:54.000000 vents-0.1.3/vents/providers/gcp/service.py
--rw-r--r--   0 mourad     (501) staff       (20)     2337 2023-06-08 10:20:54.000000 vents-0.1.3/vents/providers/kinds.py
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-06-08 10:20:54.000000 vents-0.1.3/vents/py.typed
--rw-r--r--   0 mourad     (501) staff       (20)      256 2023-06-08 10:20:54.000000 vents-0.1.3/vents/settings.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-06-08 10:21:35.414279 vents-0.1.3/vents.egg-info/
--rw-r--r--   0 mourad     (501) staff       (20)     1568 2023-06-08 10:21:35.000000 vents-0.1.3/vents.egg-info/PKG-INFO
--rw-r--r--   0 mourad     (501) staff       (20)     1216 2023-06-08 10:21:35.000000 vents-0.1.3/vents.egg-info/SOURCES.txt
--rw-r--r--   0 mourad     (501) staff       (20)        1 2023-06-08 10:21:35.000000 vents-0.1.3/vents.egg-info/dependency_links.txt
--rw-r--r--   0 mourad     (501) staff       (20)       66 2023-06-08 10:21:35.000000 vents-0.1.3/vents.egg-info/requires.txt
--rw-r--r--   0 mourad     (501) staff       (20)        6 2023-06-08 10:21:35.000000 vents-0.1.3/vents.egg-info/top_level.txt
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-06-13 13:29:09.817380 vents-0.1.4/
+-rw-r--r--   0 mourad     (501) staff       (20)      172 2023-06-13 13:28:00.000000 vents-0.1.4/MANIFEST.in
+-rw-r--r--   0 mourad     (501) staff       (20)     1568 2023-06-13 13:29:09.817480 vents-0.1.4/PKG-INFO
+-rw-r--r--   0 mourad     (501) staff       (20)     1031 2023-06-13 13:29:09.817940 vents-0.1.4/setup.cfg
+-rw-r--r--   0 mourad     (501) staff       (20)     2695 2023-06-13 13:28:00.000000 vents-0.1.4/setup.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-06-13 13:29:09.811830 vents-0.1.4/vents/
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-06-13 13:28:00.000000 vents-0.1.4/vents/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)     5003 2023-06-13 13:28:00.000000 vents-0.1.4/vents/config.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-06-13 13:29:09.813426 vents-0.1.4/vents/connections/
+-rw-r--r--   0 mourad     (501) staff       (20)      335 2023-06-13 13:28:00.000000 vents-0.1.4/vents/connections/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2485 2023-06-13 13:28:00.000000 vents-0.1.4/vents/connections/catalog.py
+-rw-r--r--   0 mourad     (501) staff       (20)     3842 2023-06-13 13:28:00.000000 vents-0.1.4/vents/connections/connection.py
+-rw-r--r--   0 mourad     (501) staff       (20)      513 2023-06-13 13:28:00.000000 vents-0.1.4/vents/connections/connection_resource.py
+-rw-r--r--   0 mourad     (501) staff       (20)     3301 2023-06-13 13:28:00.000000 vents-0.1.4/vents/connections/connection_schema.py
+-rw-r--r--   0 mourad     (501) staff       (20)       37 2023-06-13 13:28:00.000000 vents-0.1.4/vents/exceptions.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-06-13 13:29:09.814746 vents-0.1.4/vents/notifiers/
+-rw-r--r--   0 mourad     (501) staff       (20)      866 2023-06-13 13:28:00.000000 vents-0.1.4/vents/notifiers/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)     4589 2023-06-13 13:28:00.000000 vents-0.1.4/vents/notifiers/base.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1303 2023-06-13 13:28:00.000000 vents-0.1.4/vents/notifiers/discord_webhook.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1277 2023-06-13 13:28:00.000000 vents-0.1.4/vents/notifiers/hipchat_webhook.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1764 2023-06-13 13:28:00.000000 vents-0.1.4/vents/notifiers/mattermost_webhook.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1723 2023-06-13 13:28:00.000000 vents-0.1.4/vents/notifiers/pagerduty_webhook.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2051 2023-06-13 13:28:00.000000 vents-0.1.4/vents/notifiers/slack_webhook.py
+-rw-r--r--   0 mourad     (501) staff       (20)      372 2023-06-13 13:28:00.000000 vents-0.1.4/vents/notifiers/spec.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1847 2023-06-13 13:28:00.000000 vents-0.1.4/vents/notifiers/webhook.py
+-rw-r--r--   0 mourad     (501) staff       (20)      233 2023-06-13 13:28:00.000000 vents-0.1.4/vents/pkg.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-06-13 13:29:09.815129 vents-0.1.4/vents/providers/
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-06-13 13:28:00.000000 vents-0.1.4/vents/providers/__init__.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-06-13 13:29:09.815684 vents-0.1.4/vents/providers/aws/
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-06-13 13:28:00.000000 vents-0.1.4/vents/providers/aws/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)     3724 2023-06-13 13:28:00.000000 vents-0.1.4/vents/providers/aws/base.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1656 2023-06-13 13:28:00.000000 vents-0.1.4/vents/providers/aws/s3.py
+-rw-r--r--   0 mourad     (501) staff       (20)     3456 2023-06-13 13:28:00.000000 vents-0.1.4/vents/providers/aws/service.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-06-13 13:29:09.816249 vents-0.1.4/vents/providers/azure/
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-06-13 13:28:00.000000 vents-0.1.4/vents/providers/azure/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2609 2023-06-13 13:28:00.000000 vents-0.1.4/vents/providers/azure/base.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1831 2023-06-13 13:28:00.000000 vents-0.1.4/vents/providers/azure/blob_storage.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2251 2023-06-13 13:28:00.000000 vents-0.1.4/vents/providers/azure/service.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1620 2023-06-13 13:28:00.000000 vents-0.1.4/vents/providers/base.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-06-13 13:29:09.817215 vents-0.1.4/vents/providers/gcp/
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-06-13 13:28:00.000000 vents-0.1.4/vents/providers/gcp/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)     3750 2023-06-13 13:28:00.000000 vents-0.1.4/vents/providers/gcp/base.py
+-rw-r--r--   0 mourad     (501) staff       (20)      995 2023-06-13 13:28:00.000000 vents-0.1.4/vents/providers/gcp/gcs.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2513 2023-06-13 13:28:00.000000 vents-0.1.4/vents/providers/gcp/service.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2337 2023-06-13 13:28:00.000000 vents-0.1.4/vents/providers/kinds.py
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-06-13 13:28:00.000000 vents-0.1.4/vents/py.typed
+-rw-r--r--   0 mourad     (501) staff       (20)      256 2023-06-13 13:28:00.000000 vents-0.1.4/vents/settings.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-06-13 13:29:09.812702 vents-0.1.4/vents.egg-info/
+-rw-r--r--   0 mourad     (501) staff       (20)     1568 2023-06-13 13:29:09.000000 vents-0.1.4/vents.egg-info/PKG-INFO
+-rw-r--r--   0 mourad     (501) staff       (20)     1216 2023-06-13 13:29:09.000000 vents-0.1.4/vents.egg-info/SOURCES.txt
+-rw-r--r--   0 mourad     (501) staff       (20)        1 2023-06-13 13:29:09.000000 vents-0.1.4/vents.egg-info/dependency_links.txt
+-rw-r--r--   0 mourad     (501) staff       (20)       66 2023-06-13 13:29:09.000000 vents-0.1.4/vents.egg-info/requires.txt
+-rw-r--r--   0 mourad     (501) staff       (20)        6 2023-06-13 13:29:09.000000 vents-0.1.4/vents.egg-info/top_level.txt
```

### Comparing `vents-0.1.3/PKG-INFO` & `vents-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vents
-Version: 0.1.3
+Version: 0.1.4
 Summary: Open source integrations, alerting, and notification library.
 Home-page: https://github.com/mmourafiq/vents
 Author: Mourad Mourafiq
 Author-email: mourad.mourafiq@gmail.com
 Maintainer: Mourad Mourafiq
 Maintainer-email: mourad.mourafiq@gmail.com
 License: Apache 2.0
```

### Comparing `vents-0.1.3/setup.cfg` & `vents-0.1.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `vents-0.1.3/setup.py` & `vents-0.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.3/vents/config.py` & `vents-0.1.4/vents/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -107,14 +107,17 @@
     def get_connections_catalog(
         connections: Optional[List[Connection]],
     ) -> Optional[ConnectionCatalog]:
         if not connections:
             return None
         return ConnectionCatalog(connections=connections)
 
+    def set_connections_catalog(self, connections: Optional[List[Connection]]):
+        self.catalog = self.get_connections_catalog(connections)
+
     def load_connections_catalog(self) -> Optional[ConnectionCatalog]:
         catalog_env_name = self.get_connections_catalog_env_name()
         connections_catalog = os.environ.get(catalog_env_name)
         if not connections_catalog:
             return None
         return ConnectionCatalog.read(connections_catalog, config_type=".json")
```

### Comparing `vents-0.1.3/vents/connections/catalog.py` & `vents-0.1.4/vents/connections/catalog.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.3/vents/connections/connection.py` & `vents-0.1.4/vents/connections/connection.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.3/vents/connections/connection_resource.py` & `vents-0.1.4/vents/connections/connection_resource.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.3/vents/connections/connection_schema.py` & `vents-0.1.4/vents/connections/connection_schema.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.3/vents/notifiers/__init__.py` & `vents-0.1.4/vents/notifiers/__init__.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.3/vents/notifiers/base.py` & `vents-0.1.4/vents/notifiers/base.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.3/vents/notifiers/discord_webhook.py` & `vents-0.1.4/vents/notifiers/discord_webhook.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.3/vents/notifiers/hipchat_webhook.py` & `vents-0.1.4/vents/notifiers/hipchat_webhook.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.3/vents/notifiers/mattermost_webhook.py` & `vents-0.1.4/vents/notifiers/mattermost_webhook.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.3/vents/notifiers/pagerduty_webhook.py` & `vents-0.1.4/vents/notifiers/pagerduty_webhook.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.3/vents/notifiers/slack_webhook.py` & `vents-0.1.4/vents/notifiers/slack_webhook.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.3/vents/notifiers/webhook.py` & `vents-0.1.4/vents/notifiers/webhook.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.3/vents/providers/aws/base.py` & `vents-0.1.4/vents/providers/aws/base.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.3/vents/providers/aws/s3.py` & `vents-0.1.4/vents/providers/aws/s3.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.3/vents/providers/aws/service.py` & `vents-0.1.4/vents/providers/aws/service.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.3/vents/providers/azure/base.py` & `vents-0.1.4/vents/providers/azure/base.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.3/vents/providers/azure/blob_storage.py` & `vents-0.1.4/vents/providers/azure/blob_storage.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.3/vents/providers/azure/service.py` & `vents-0.1.4/vents/providers/azure/service.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.3/vents/providers/base.py` & `vents-0.1.4/vents/providers/base.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.3/vents/providers/gcp/base.py` & `vents-0.1.4/vents/providers/gcp/base.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.3/vents/providers/gcp/gcs.py` & `vents-0.1.4/vents/providers/gcp/gcs.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.3/vents/providers/gcp/service.py` & `vents-0.1.4/vents/providers/gcp/service.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.3/vents/providers/kinds.py` & `vents-0.1.4/vents/providers/kinds.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.3/vents.egg-info/PKG-INFO` & `vents-0.1.4/vents.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vents
-Version: 0.1.3
+Version: 0.1.4
 Summary: Open source integrations, alerting, and notification library.
 Home-page: https://github.com/mmourafiq/vents
 Author: Mourad Mourafiq
 Author-email: mourad.mourafiq@gmail.com
 Maintainer: Mourad Mourafiq
 Maintainer-email: mourad.mourafiq@gmail.com
 License: Apache 2.0
```

### Comparing `vents-0.1.3/vents.egg-info/SOURCES.txt` & `vents-0.1.4/vents.egg-info/SOURCES.txt`

 * *Files identical despite different names*

