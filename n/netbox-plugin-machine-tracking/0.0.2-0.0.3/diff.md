# Comparing `tmp/netbox_plugin_machine_tracking-0.0.2.tar.gz` & `tmp/netbox_plugin_machine_tracking-0.0.3.tar.gz`

## Comparing `netbox_plugin_machine_tracking-0.0.2.tar` & `netbox_plugin_machine_tracking-0.0.3.tar`

### file list

```diff
@@ -1,26 +1,25 @@
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.2/MANIFEST.in
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.2/setup.py
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.2/machine_tracking/__init__.py
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.2/machine_tracking/filtersets.py
--rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.2/machine_tracking/forms.py
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.2/machine_tracking/models.py
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.2/machine_tracking/navigation.py
--rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.2/machine_tracking/tables.py
--rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.2/machine_tracking/template_content.py
--rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.2/machine_tracking/urls.py
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.2/machine_tracking/views.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.2/machine_tracking/api/__init__.py
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.2/machine_tracking/api/serializers.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.2/machine_tracking/api/urls.py
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.2/machine_tracking/api/views.py
--rw-r--r--   0        0        0     2640 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.2/machine_tracking/migrations/0001_initial.py
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.2/machine_tracking/migrations/0002_event_part_type.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.2/machine_tracking/migrations/0003_alter_replacement_part_type.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.2/machine_tracking/migrations/__init__.py
--rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.2/machine_tracking/templates/machine_tracking/device_panel.html
--rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.2/machine_tracking/templates/machine_tracking/event.html
--rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.2/machine_tracking/templates/machine_tracking/replacement.html
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.2/LICENCE
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.2/README.md
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.3/setup.py
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.3/machine_tracking/__init__.py
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.3/machine_tracking/filtersets.py
+-rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.3/machine_tracking/forms.py
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.3/machine_tracking/models.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.3/machine_tracking/navigation.py
+-rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.3/machine_tracking/tables.py
+-rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.3/machine_tracking/template_content.py
+-rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.3/machine_tracking/urls.py
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.3/machine_tracking/views.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.3/machine_tracking/api/__init__.py
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.3/machine_tracking/api/serializers.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.3/machine_tracking/api/urls.py
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.3/machine_tracking/api/views.py
+-rw-r--r--   0        0        0     2640 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.3/machine_tracking/migrations/0001_initial.py
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.3/machine_tracking/migrations/0002_event_part_type.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.3/machine_tracking/migrations/0003_alter_replacement_part_type.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.3/machine_tracking/migrations/__init__.py
+-rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.3/machine_tracking/templates/machine_tracking/device_panel.html
+-rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.3/machine_tracking/templates/machine_tracking/event.html
+-rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.3/machine_tracking/templates/machine_tracking/replacement.html
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.3/LICENCE
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.3/README.md
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.3/PKG-INFO
```

### Comparing `netbox_plugin_machine_tracking-0.0.2/machine_tracking/filtersets.py` & `netbox_plugin_machine_tracking-0.0.3/machine_tracking/filtersets.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_machine_tracking-0.0.2/machine_tracking/forms.py` & `netbox_plugin_machine_tracking-0.0.3/machine_tracking/forms.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_machine_tracking-0.0.2/machine_tracking/models.py` & `netbox_plugin_machine_tracking-0.0.3/machine_tracking/models.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_machine_tracking-0.0.2/machine_tracking/tables.py` & `netbox_plugin_machine_tracking-0.0.3/machine_tracking/tables.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_machine_tracking-0.0.2/machine_tracking/template_content.py` & `netbox_plugin_machine_tracking-0.0.3/machine_tracking/template_content.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_machine_tracking-0.0.2/machine_tracking/urls.py` & `netbox_plugin_machine_tracking-0.0.3/machine_tracking/urls.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_machine_tracking-0.0.2/machine_tracking/views.py` & `netbox_plugin_machine_tracking-0.0.3/machine_tracking/views.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_machine_tracking-0.0.2/machine_tracking/api/serializers.py` & `netbox_plugin_machine_tracking-0.0.3/machine_tracking/api/serializers.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_machine_tracking-0.0.2/machine_tracking/api/views.py` & `netbox_plugin_machine_tracking-0.0.3/machine_tracking/api/views.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_machine_tracking-0.0.2/machine_tracking/migrations/0001_initial.py` & `netbox_plugin_machine_tracking-0.0.3/machine_tracking/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_machine_tracking-0.0.2/machine_tracking/templates/machine_tracking/device_panel.html` & `netbox_plugin_machine_tracking-0.0.3/machine_tracking/templates/machine_tracking/device_panel.html`

 * *Files identical despite different names*

### Comparing `netbox_plugin_machine_tracking-0.0.2/machine_tracking/templates/machine_tracking/event.html` & `netbox_plugin_machine_tracking-0.0.3/machine_tracking/templates/machine_tracking/event.html`

 * *Files identical despite different names*

### Comparing `netbox_plugin_machine_tracking-0.0.2/machine_tracking/templates/machine_tracking/replacement.html` & `netbox_plugin_machine_tracking-0.0.3/machine_tracking/templates/machine_tracking/replacement.html`

 * *Files identical despite different names*

### Comparing `netbox_plugin_machine_tracking-0.0.2/LICENCE` & `netbox_plugin_machine_tracking-0.0.3/LICENCE`

 * *Files identical despite different names*

### Comparing `netbox_plugin_machine_tracking-0.0.2/README.md` & `netbox_plugin_machine_tracking-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `netbox_plugin_machine_tracking-0.0.2/PKG-INFO` & `netbox_plugin_machine_tracking-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-plugin-machine-tracking
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Netbox plugin tracking failures and other state changes in devices.
 Author-email: Lisa Guo <lisguo@cisco.com>
 License-File: LICENCE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

