# Comparing `tmp/crunch_statuspageio-0.6.tar.gz` & `tmp/crunch_statuspageio-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crunch_statuspageio-0.6.tar", max compression
+gzip compressed data, was "crunch_statuspageio-0.7.tar", max compression
```

## Comparing `crunch_statuspageio-0.6.tar` & `crunch_statuspageio-0.7.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1137 2023-02-16 17:19:01.804276 crunch_statuspageio-0.6/pyproject.toml
--rw-r--r--   0        0        0     1145 2022-09-13 22:43:55.199395 crunch_statuspageio-0.6/statuspageio/__init__.py
--rw-r--r--   0        0        0     3154 2022-09-13 22:43:55.191869 crunch_statuspageio-0.6/statuspageio/client.py
--rw-r--r--   0        0        0      703 2021-09-09 19:28:55.000000 crunch_statuspageio-0.6/statuspageio/configuration.py
--rw-r--r--   0        0        0     2023 2022-12-06 16:20:15.539070 crunch_statuspageio-0.6/statuspageio/errors.py
--rw-r--r--   0        0        0     8120 2022-12-06 16:21:54.701295 crunch_statuspageio-0.6/statuspageio/http_client.py
--rw-r--r--   0        0        0    25334 2023-02-16 17:16:43.483269 crunch_statuspageio-0.6/statuspageio/services.py
--rw-r--r--   0        0        0      681 1970-01-01 00:00:00.000000 crunch_statuspageio-0.6/setup.py
--rw-r--r--   0        0        0      597 1970-01-01 00:00:00.000000 crunch_statuspageio-0.6/PKG-INFO
+-rw-r--r--   0        0        0     1137 2023-06-13 17:11:35.283853 crunch_statuspageio-0.7/pyproject.toml
+-rw-r--r--   0        0        0     1145 2022-09-13 22:43:55.199395 crunch_statuspageio-0.7/statuspageio/__init__.py
+-rw-r--r--   0        0        0     3154 2022-09-13 22:43:55.191869 crunch_statuspageio-0.7/statuspageio/client.py
+-rw-r--r--   0        0        0      703 2021-09-09 19:28:55.000000 crunch_statuspageio-0.7/statuspageio/configuration.py
+-rw-r--r--   0        0        0     2023 2022-12-06 16:20:15.539070 crunch_statuspageio-0.7/statuspageio/errors.py
+-rw-r--r--   0        0        0     8120 2022-12-06 16:21:54.701295 crunch_statuspageio-0.7/statuspageio/http_client.py
+-rw-r--r--   0        0        0    26827 2023-06-13 17:08:01.462712 crunch_statuspageio-0.7/statuspageio/services.py
+-rw-r--r--   0        0        0      597 1970-01-01 00:00:00.000000 crunch_statuspageio-0.7/PKG-INFO
```

### Comparing `crunch_statuspageio-0.6/pyproject.toml` & `crunch_statuspageio-0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "crunch-statuspageio"
-version = "0.6"
+version = "0.7"
 description = "Python client library for statuspage.io"
 authors = ["Adrien Pensart <adrien.pensart@corp.ovh.com>"]
 license = "MIT"
 packages = [
     { include = "statuspageio" },
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 requests = "^2.28.0"
-munch = "^2.5.0"
+munch = "^3.0.0"
 
 [tool.poetry.dev-dependencies]
 pylint = "^2.15.2"
 
 [tool.poetry.group.dev.dependencies]
 isort = "^5.10.1"
```

### Comparing `crunch_statuspageio-0.6/statuspageio/__init__.py` & `crunch_statuspageio-0.7/statuspageio/__init__.py`

 * *Files identical despite different names*

### Comparing `crunch_statuspageio-0.6/statuspageio/client.py` & `crunch_statuspageio-0.7/statuspageio/client.py`

 * *Files identical despite different names*

### Comparing `crunch_statuspageio-0.6/statuspageio/configuration.py` & `crunch_statuspageio-0.7/statuspageio/configuration.py`

 * *Files identical despite different names*

### Comparing `crunch_statuspageio-0.6/statuspageio/errors.py` & `crunch_statuspageio-0.7/statuspageio/errors.py`

 * *Files identical despite different names*

### Comparing `crunch_statuspageio-0.6/statuspageio/http_client.py` & `crunch_statuspageio-0.7/statuspageio/http_client.py`

 * *Files identical despite different names*

### Comparing `crunch_statuspageio-0.6/statuspageio/services.py` & `crunch_statuspageio-0.7/statuspageio/services.py`

 * *Files 12% similar despite different names*

```diff
@@ -76,15 +76,15 @@
             'css_light_font_color',
             'css_greens',
             'css_oranges',
             'css_reds',
             'css_yellows']
 
         if not kwargs:
-            raise Exception('attributes are missing')
+            raise ValueError('attributes are missing')
 
         attributes = dict((k, v) for k, v in kwargs.items()
                           if k in OPTS_KEYS_TO_PERSIST)
 
         page = self.http_client.patch(
             f'/pages/{self.page_id}.json',
             container=self.container,
@@ -159,15 +159,15 @@
         :calls: ``post pages/{page_id}/components.json``
         :param dict **kwargs:  component attributes to update.
         :return: Dictionary that support attribute-style access and represents updated Component resource.
         :rtype: dict
         """
 
         if not kwargs:
-            raise Exception('attributes are missing')
+            raise ValueError('attributes are missing')
 
         attributes = dict((k, v) for k, v in kwargs.items()
                           if k in self.OPTS_KEYS_TO_PERSIST)
 
         _, _, component = self.http_client.post(
             f'/pages/{self.page_id}/components.json',
             container=self.container,
@@ -208,15 +208,15 @@
         :param int component_id: Unique identifier of a component.
         :param dict **kwargs:  component attributes to update.
         :return: Dictionary that support attribute-style access and represents updated Component resource.
         :rtype: dict
         """
 
         if not kwargs:
-            raise Exception('attributes for Contact are missing')
+            raise ValueError('attributes for Contact are missing')
 
         attributes = dict((k, v) for k, v in kwargs.items()
                           if k in self.OPTS_KEYS_TO_PERSIST)
 
         _, _, component = self.http_client.patch(
             f"/pages/{self.page_id}/components/{component_id}.json",
             container=self.container,
@@ -315,47 +315,90 @@
         self.page_id = page_id
         self.container = 'incident'
 
     @property
     def http_client(self):
         return self.__http_client
 
-    def list(self):
+    def list(self, q=None, limit=100, page=1):
         """
         List all incidents
 
         :calls: ``get pages/{page_id}/incidents.json``
         :return: Dictionary that support attribute-style access and represents updated Component resource.
         :rtype: dict
         """
 
-        _, _, incidents = self.http_client.get(f'/pages/{self.page_id}/incidents.json')
+        params = {
+            "limit": limit,
+            "q": q,
+            "page": page,
+        }
+        _, _, incidents = self.http_client.get(f'/pages/{self.page_id}/incidents.json', params=params)
         return incidents
 
-    def list_unresolved(self):
+    def list_unresolved(self, page=1, per_page=100):
         """
         List unresolved incidents
 
         :calls: ``get pages/{page_id}/incidents/unresolved.json``
         :return: Dictionary that support attribute-style access and represents updated Component resource.
         :rtype: dict
         """
 
-        _, _, incidents = self.http_client.get(f'/pages/{self.page_id}/incidents/unresolved.json')
+        params = {
+            "page": page,
+            "per_page": per_page,
+        }
+        _, _, incidents = self.http_client.get(f'/pages/{self.page_id}/incidents/unresolved.json', params=params)
         return incidents
 
-    def list_scheduled(self):
+    def list_scheduled(self, page=1, per_page=100):
         """
         List scheduled incidents
 
         :calls: ``get pages/{page_id}/incidents/scheduled.json``
         :return: Dictionary that support attribute-style access and represents updated Component resource.
         :rtype: dict
         """
-        _, _, incidents = self.http_client.get(f'/pages/{self.page_id}/incidents/scheduled.json')
+        params = {
+            "page": page,
+            "per_page": per_page,
+        }
+        _, _, incidents = self.http_client.get(f'/pages/{self.page_id}/incidents/scheduled.json', params=params)
+        return incidents
+
+    def list_upcoming(self, page=1, per_page=100):
+        """
+        List upcoming incidents
+
+        :calls: ``get pages/{page_id}/incidents/upcoming.json``
+        :return: Dictionary that support attribute-style access and represents updated Component resource.
+        :rtype: dict
+        """
+        params = {
+            "page": page,
+            "per_page": per_page,
+        }
+        _, _, incidents = self.http_client.get(f'/pages/{self.page_id}/incidents/upcoming.json', params=params)
+        return incidents
+
+    def list_active_maintenance(self, page=1, per_page=100):
+        """
+        List active maintenances
+
+        :calls: ``get pages/{page_id}/incidents/active_maintenance.json``
+        :return: Dictionary that support attribute-style access and represents updated Component resource.
+        :rtype: dict
+        """
+        params = {
+            "page": page,
+            "per_page": per_page,
+        }
+        _, _, incidents = self.http_client.get(f'/pages/{self.page_id}/incidents/active_maintenance.json', params=params)
         return incidents
 
     def create(self, **kwargs):
         """
         Create a incident
 
         :calls: ``post pages/{page_id}/incidents.json``
@@ -371,15 +414,15 @@
             'wants_twitter_update',
             'impact_override',
             'component_ids',
             'metadata',
         ]
 
         if not kwargs:
-            raise Exception('attributes are missing')
+            raise ValueError('attributes are missing')
 
         attributes = dict((k, v) for k, v in kwargs.items()
                           if k in OPTS_KEYS_TO_PERSIST)
 
         _, _, incident = self.http_client.post(
             f'/pages/{self.page_id}/incidents.json',
             container=self.container,
@@ -409,15 +452,15 @@
             'scheduled_auto_in_progress',
             'scheduled_auto_completed',
             'impact_override',
             'component_ids',
             'metadata',
         ]
         if not kwargs:
-            raise Exception('attributes are missing')
+            raise ValueError('attributes are missing')
 
         attributes = dict((k, v) for k, v in kwargs.items()
                           if k in OPTS_KEYS_TO_PERSIST)
 
         _, _, incident = self.http_client.post(
             f'/pages/{self.page_id}/incidents.json',
             container=self.container,
@@ -459,15 +502,15 @@
             'wants_twitter_update',
             'impact_override',
             'component_ids',
             'metadata',
         ]
 
         if not kwargs:
-            raise Exception('attributes for Incident are missing')
+            raise ValueError('attributes for Incident are missing')
 
         attributes = dict((k, v) for k, v in kwargs.items()
                           if k in OPTS_KEYS_TO_PERSIST)
 
         _, _, component = self.http_client.patch(
             f"/pages/{self.page_id}/incidents/{incident_id}.json",
             container=self.container,
@@ -488,15 +531,15 @@
         OPTS_KEYS_TO_PERSIST = [
             'body',
             'wants_twitter_update',
             'deliver_notifications',
         ]
 
         if not kwargs:
-            raise Exception('attributes for Incident Update are missing')
+            raise ValueError('attributes for Incident Update are missing')
 
         attributes = dict((k, v) for k, v in kwargs.items()
                           if k in OPTS_KEYS_TO_PERSIST)
 
         _, _, component = self.http_client.patch(
             f"/pages/{self.page_id}/incidents/{incident_id}/incident_updates/{incident_update_id}",
             container='incident_update',
@@ -556,15 +599,15 @@
             'phone_number',
             'phone_country',
             'endpoint',
             'skip_confirmation_notification',
             'page_access_user']
 
         if not kwargs:
-            raise Exception('attributes are missing')
+            raise ValueError('attributes are missing')
 
         attributes = dict((k, v) for k, v in kwargs.items()
                           if k in OPTS_KEYS_TO_PERSIST)
 
         _, _, subscriber = self.http_client.post(
             f'/pages/{self.page_id}/subscribers.json',
             container=self.container,
@@ -658,15 +701,15 @@
             'display',
             'tooltip_description',
             'y_axis_min',
             'y_axis_max',
             'decimal_places']
 
         if not kwargs:
-            raise Exception('attributes are missing')
+            raise ValueError('attributes are missing')
 
         attributes = dict((k, v) for k, v in kwargs.items()
                           if k in OPTS_KEYS_TO_PERSIST)
 
         _, _, metric = self.http_client.post(
             f'/pages/{self.page_id}/metrics_providers/{provider_id}/metrics.json',
             container=self.container,
@@ -685,15 +728,15 @@
         :return: Dictionary that support attribute-style access and represents updated Component resource.
         :rtype: dict
         """
 
         OPTS_KEYS_TO_PERSIST = ['timestamp', 'value']
 
         if not kwargs:
-            raise Exception('attributes are missing')
+            raise ValueError('attributes are missing')
 
         attributes = dict((k, v) for k, v in kwargs.items()
                           if k in OPTS_KEYS_TO_PERSIST)
 
         _, _, metric = self.http_client.post(
             f'/pages/{self.page_id}/metrics/{metric_id}/data.json',
             container='data',
@@ -776,15 +819,15 @@
         :param dict **kwargs:  Users attributes to create.
         :return: Dictionary that support attribute-style access and represents updated User resource.
         :rtype: dict
         """
         OPTS_KEYS_TO_PERSIST = ['email', 'password', 'first_name', 'last_name']
 
         if not kwargs:
-            raise Exception('attributes are missing')
+            raise ValueError('attributes are missing')
 
         attributes = dict((k, v) for k, v in kwargs.items()
                           if k in OPTS_KEYS_TO_PERSIST)
 
         _, _, user = self.http_client.post(
             f'/organizations/{self.organization_id}/users.json',
             container=self.container,
```

### Comparing `crunch_statuspageio-0.6/PKG-INFO` & `crunch_statuspageio-0.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: crunch-statuspageio
-Version: 0.6
+Version: 0.7
 Summary: Python client library for statuspage.io
 License: MIT
 Author: Adrien Pensart
 Author-email: adrien.pensart@corp.ovh.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: munch (>=2.5.0,<3.0.0)
+Requires-Dist: munch (>=3.0.0,<4.0.0)
 Requires-Dist: requests (>=2.28.0,<3.0.0)
```

