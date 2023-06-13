# Comparing `tmp/netbox_plugin_machine_tracking-0.0.3.tar.gz` & `tmp/netbox_plugin_machine_tracking-0.0.4.tar.gz`

## Comparing `netbox_plugin_machine_tracking-0.0.3.tar` & `netbox_plugin_machine_tracking-0.0.4.tar`

### file list

```diff
@@ -1,25 +1,24 @@
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.3/setup.py
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.3/machine_tracking/__init__.py
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.3/machine_tracking/filtersets.py
--rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.3/machine_tracking/forms.py
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.3/machine_tracking/models.py
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.3/machine_tracking/navigation.py
--rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.3/machine_tracking/tables.py
--rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.3/machine_tracking/template_content.py
--rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.3/machine_tracking/urls.py
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.3/machine_tracking/views.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.3/machine_tracking/api/__init__.py
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.3/machine_tracking/api/serializers.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.3/machine_tracking/api/urls.py
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.3/machine_tracking/api/views.py
--rw-r--r--   0        0        0     2640 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.3/machine_tracking/migrations/0001_initial.py
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.3/machine_tracking/migrations/0002_event_part_type.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.3/machine_tracking/migrations/0003_alter_replacement_part_type.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.3/machine_tracking/migrations/__init__.py
--rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.3/machine_tracking/templates/machine_tracking/device_panel.html
--rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.3/machine_tracking/templates/machine_tracking/event.html
--rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.3/machine_tracking/templates/machine_tracking/replacement.html
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.3/LICENCE
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.3/README.md
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.4/machine_tracking/__init__.py
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.4/machine_tracking/filtersets.py
+-rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.4/machine_tracking/forms.py
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.4/machine_tracking/models.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.4/machine_tracking/navigation.py
+-rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.4/machine_tracking/tables.py
+-rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.4/machine_tracking/template_content.py
+-rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.4/machine_tracking/urls.py
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.4/machine_tracking/views.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.4/machine_tracking/api/__init__.py
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.4/machine_tracking/api/serializers.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.4/machine_tracking/api/urls.py
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.4/machine_tracking/api/views.py
+-rw-r--r--   0        0        0     2640 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.4/machine_tracking/migrations/0001_initial.py
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.4/machine_tracking/migrations/0002_event_part_type.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.4/machine_tracking/migrations/0003_alter_replacement_part_type.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.4/machine_tracking/migrations/__init__.py
+-rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.4/machine_tracking/templates/machine_tracking/device_panel.html
+-rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.4/machine_tracking/templates/machine_tracking/event.html
+-rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.4/machine_tracking/templates/machine_tracking/replacement.html
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.4/LICENCE
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.4/README.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.4/PKG-INFO
```

### Comparing `netbox_plugin_machine_tracking-0.0.3/machine_tracking/filtersets.py` & `netbox_plugin_machine_tracking-0.0.4/machine_tracking/filtersets.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_machine_tracking-0.0.3/machine_tracking/forms.py` & `netbox_plugin_machine_tracking-0.0.4/machine_tracking/forms.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_machine_tracking-0.0.3/machine_tracking/models.py` & `netbox_plugin_machine_tracking-0.0.4/machine_tracking/models.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_machine_tracking-0.0.3/machine_tracking/tables.py` & `netbox_plugin_machine_tracking-0.0.4/machine_tracking/tables.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_machine_tracking-0.0.3/machine_tracking/template_content.py` & `netbox_plugin_machine_tracking-0.0.4/machine_tracking/template_content.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_machine_tracking-0.0.3/machine_tracking/urls.py` & `netbox_plugin_machine_tracking-0.0.4/machine_tracking/urls.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_machine_tracking-0.0.3/machine_tracking/views.py` & `netbox_plugin_machine_tracking-0.0.4/machine_tracking/views.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_machine_tracking-0.0.3/machine_tracking/api/serializers.py` & `netbox_plugin_machine_tracking-0.0.4/machine_tracking/api/serializers.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_machine_tracking-0.0.3/machine_tracking/api/views.py` & `netbox_plugin_machine_tracking-0.0.4/machine_tracking/api/views.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_machine_tracking-0.0.3/machine_tracking/migrations/0001_initial.py` & `netbox_plugin_machine_tracking-0.0.4/machine_tracking/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_machine_tracking-0.0.3/machine_tracking/templates/machine_tracking/device_panel.html` & `netbox_plugin_machine_tracking-0.0.4/machine_tracking/templates/machine_tracking/device_panel.html`

 * *Files identical despite different names*

### Comparing `netbox_plugin_machine_tracking-0.0.3/machine_tracking/templates/machine_tracking/event.html` & `netbox_plugin_machine_tracking-0.0.4/machine_tracking/templates/machine_tracking/event.html`

 * *Files identical despite different names*

### Comparing `netbox_plugin_machine_tracking-0.0.3/machine_tracking/templates/machine_tracking/replacement.html` & `netbox_plugin_machine_tracking-0.0.4/machine_tracking/templates/machine_tracking/replacement.html`

 * *Files identical despite different names*

### Comparing `netbox_plugin_machine_tracking-0.0.3/LICENCE` & `netbox_plugin_machine_tracking-0.0.4/LICENCE`

 * *Files identical despite different names*

### Comparing `netbox_plugin_machine_tracking-0.0.3/README.md` & `netbox_plugin_machine_tracking-0.0.4/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 # Machine failures tracking system
 
 A Netbox plugin for keeping track of failures and other state changes for individual devices.
 
 
 ## Installation
-Installation package to come.
+The plugin is available as a Python package in pypi and can be installed with pip
+
+```
+pip install netbox-plugin-machine-tracking
+```
 
 Once installed, the plugin needs to be added to the configuration.py file.
 
 ```python
 PLUGINS = ['machine_tracking']
 
 ```
```

### Comparing `netbox_plugin_machine_tracking-0.0.3/PKG-INFO` & `netbox_plugin_machine_tracking-0.0.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-plugin-machine-tracking
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Netbox plugin tracking failures and other state changes in devices.
 Author-email: Lisa Guo <lisguo@cisco.com>
 License-File: LICENCE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
@@ -12,15 +12,19 @@
 
 # Machine failures tracking system
 
 A Netbox plugin for keeping track of failures and other state changes for individual devices.
 
 
 ## Installation
-Installation package to come.
+The plugin is available as a Python package in pypi and can be installed with pip
+
+```
+pip install netbox-plugin-machine-tracking
+```
 
 Once installed, the plugin needs to be added to the configuration.py file.
 
 ```python
 PLUGINS = ['machine_tracking']
 
 ```
```

