# Comparing `tmp/ayon-python-api-0.2.0.tar.gz` & `tmp/ayon-python-api-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ayon-python-api-0.2.0.tar", last modified: Wed May 31 08:28:29 2023, max compression
+gzip compressed data, was "ayon-python-api-0.2.1.tar", last modified: Tue Jun 13 09:28:06 2023, max compression
```

## Comparing `ayon-python-api-0.2.0.tar` & `ayon-python-api-0.2.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:28:29.524663 ayon-python-api-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-31 08:28:24.000000 ayon-python-api-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-05-31 08:28:29.524663 ayon-python-api-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-05-31 08:28:24.000000 ayon-python-api-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:28:29.520663 ayon-python-api-0.2.0/ayon_api/
--rw-r--r--   0 runner    (1001) docker     (123)     6445 2023-05-31 08:28:24.000000 ayon-python-api-0.2.0/ayon_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27676 2023-05-31 08:28:24.000000 ayon-python-api-0.2.0/ayon_api/_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-05-31 08:28:24.000000 ayon-python-api-0.2.0/ayon_api/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    56730 2023-05-31 08:28:24.000000 ayon-python-api-0.2.0/ayon_api/entity_hub.py
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-05-31 08:28:24.000000 ayon-python-api-0.2.0/ayon_api/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-05-31 08:28:24.000000 ayon-python-api-0.2.0/ayon_api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    25639 2023-05-31 08:28:24.000000 ayon-python-api-0.2.0/ayon_api/graphql.py
--rw-r--r--   0 runner    (1001) docker     (123)    15583 2023-05-31 08:28:24.000000 ayon-python-api-0.2.0/ayon_api/graphql_queries.py
--rw-r--r--   0 runner    (1001) docker     (123)    19430 2023-05-31 08:28:24.000000 ayon-python-api-0.2.0/ayon_api/operations.py
--rw-r--r--   0 runner    (1001) docker     (123)   161889 2023-05-31 08:28:24.000000 ayon-python-api-0.2.0/ayon_api/server_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6856 2023-05-31 08:28:24.000000 ayon-python-api-0.2.0/ayon_api/thumbnails.py
--rw-r--r--   0 runner    (1001) docker     (123)    11714 2023-05-31 08:28:24.000000 ayon-python-api-0.2.0/ayon_api/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-31 08:28:24.000000 ayon-python-api-0.2.0/ayon_api/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:28:29.524663 ayon-python-api-0.2.0/ayon_python_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-05-31 08:28:29.000000 ayon-python-api-0.2.0/ayon_python_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-31 08:28:29.000000 ayon-python-api-0.2.0/ayon_python_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 08:28:29.000000 ayon-python-api-0.2.0/ayon_python_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-31 08:28:29.000000 ayon-python-api-0.2.0/ayon_python_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-31 08:28:29.000000 ayon-python-api-0.2.0/ayon_python_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-31 08:28:24.000000 ayon-python-api-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 08:28:29.524663 ayon-python-api-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-05-31 08:28:24.000000 ayon-python-api-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:28:06.866135 ayon-python-api-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-13 09:27:58.000000 ayon-python-api-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-06-13 09:28:06.866135 ayon-python-api-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-06-13 09:27:58.000000 ayon-python-api-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:28:06.862134 ayon-python-api-0.2.1/ayon_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     7301 2023-06-13 09:27:58.000000 ayon-python-api-0.2.1/ayon_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30053 2023-06-13 09:27:58.000000 ayon-python-api-0.2.1/ayon_api/_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-06-13 09:27:58.000000 ayon-python-api-0.2.1/ayon_api/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59757 2023-06-13 09:27:58.000000 ayon-python-api-0.2.1/ayon_api/entity_hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-06-13 09:27:58.000000 ayon-python-api-0.2.1/ayon_api/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-06-13 09:27:58.000000 ayon-python-api-0.2.1/ayon_api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25639 2023-06-13 09:27:58.000000 ayon-python-api-0.2.1/ayon_api/graphql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15583 2023-06-13 09:27:58.000000 ayon-python-api-0.2.1/ayon_api/graphql_queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19430 2023-06-13 09:27:58.000000 ayon-python-api-0.2.1/ayon_api/operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)   180006 2023-06-13 09:27:58.000000 ayon-python-api-0.2.1/ayon_api/server_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6856 2023-06-13 09:27:58.000000 ayon-python-api-0.2.1/ayon_api/thumbnails.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11714 2023-06-13 09:27:58.000000 ayon-python-api-0.2.1/ayon_api/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-13 09:27:58.000000 ayon-python-api-0.2.1/ayon_api/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:28:06.866135 ayon-python-api-0.2.1/ayon_python_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-06-13 09:28:06.000000 ayon-python-api-0.2.1/ayon_python_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-13 09:28:06.000000 ayon-python-api-0.2.1/ayon_python_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 09:28:06.000000 ayon-python-api-0.2.1/ayon_python_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-13 09:28:06.000000 ayon-python-api-0.2.1/ayon_python_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-13 09:28:06.000000 ayon-python-api-0.2.1/ayon_python_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-13 09:27:58.000000 ayon-python-api-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 09:28:06.866135 ayon-python-api-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-06-13 09:27:58.000000 ayon-python-api-0.2.1/setup.py
```

### Comparing `ayon-python-api-0.2.0/LICENSE` & `ayon-python-api-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.2.0/PKG-INFO` & `ayon-python-api-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ayon-python-api
-Version: 0.2.0
+Version: 0.2.1
 Summary: AYON Python API
 Home-page: https://github.com/ynput/ayon-python-api
 Author: ynput.io
 Author-email: info@ynput.io
 License: Apache License (2.0)
 Keywords: AYON,ynput,OpenPype,vfx
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ayon-python-api-0.2.0/README.md` & `ayon-python-api-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.2.0/ayon_api/__init__.py` & `ayon-python-api-0.2.1/ayon_api/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,21 +55,39 @@
 
     query_graphql,
 
     get_addons_info,
     get_addon_url,
     download_addon_private_file,
 
+    get_installers,
+    create_installer,
+    update_installer,
+    delete_installer,
+    download_installer,
+    upload_installer,
+
     get_dependencies_info,
     update_dependency_info,
+    get_dependency_packages,
+    create_dependency_package,
+    update_dependency_package,
+    delete_dependency_package,
 
     download_dependency_package,
     upload_dependency_package,
-    delete_dependency_package,
 
+    get_bundles,
+    create_bundle,
+    update_bundle,
+    delete_bundle,
+
+    get_info,
+    get_server_version,
+    get_server_version_tuple,
     get_user,
     get_users,
 
     get_attributes_for_type,
     get_default_fields_for_type,
 
     get_project_anatomy_preset,
@@ -83,17 +101,19 @@
     get_addon_studio_settings,
     get_addon_project_settings,
     get_addon_settings,
     get_addons_studio_settings,
     get_addons_project_settings,
     get_addons_settings,
 
+    get_project_names,
     get_projects,
     get_project,
     create_project,
+    update_project,
     delete_project,
 
     get_folder_by_id,
     get_folder_by_name,
     get_folder_by_path,
     get_folders,
 
@@ -214,21 +234,39 @@
 
     "query_graphql",
 
     "get_addons_info",
     "get_addon_url",
     "download_addon_private_file",
 
+    "get_installers",
+    "create_installer",
+    "update_installer",
+    "delete_installer",
+    "download_installer",
+    "upload_installer",
+
     "get_dependencies_info",
     "update_dependency_info",
+    "get_dependency_packages",
+    "create_dependency_package",
+    "update_dependency_package",
+    "delete_dependency_package",
 
     "download_dependency_package",
     "upload_dependency_package",
-    "delete_dependency_package",
 
+    "get_bundles",
+    "create_bundle",
+    "update_bundle",
+    "delete_bundle",
+
+    "get_info",
+    "get_server_version",
+    "get_server_version_tuple",
     "get_user",
     "get_users",
 
     "get_attributes_for_type",
     "get_default_fields_for_type",
 
     "get_project_anatomy_preset",
@@ -241,17 +279,19 @@
     "get_addon_studio_settings",
     "get_addon_project_settings",
     "get_addon_settings",
     "get_addons_studio_settings",
     "get_addons_project_settings",
     "get_addons_settings",
 
+    "get_project_names",
     "get_projects",
     "get_project",
     "create_project",
+    "update_project",
     "delete_project",
 
     "get_folder_by_id",
     "get_folder_by_name",
     "get_folder_by_path",
     "get_folders",
```

### Comparing `ayon-python-api-0.2.0/ayon_api/_api.py` & `ayon-python-api-0.2.1/ayon_api/_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -527,14 +527,61 @@
 
 
 def download_addon_private_file(*args, **kwargs):
     con = get_server_api_connection()
     return con.download_addon_private_file(*args, **kwargs)
 
 
+def get_info(*args, **kwargs):
+    con = get_server_api_connection()
+    return con.get_info(*args, **kwargs)
+
+
+def get_server_version(*args, **kwargs):
+    con = get_server_api_connection()
+    return con.get_server_version(*args, **kwargs)
+
+
+def get_server_version_tuple(*args, **kwargs):
+    con = get_server_api_connection()
+    return con.get_server_version_tuple(*args, **kwargs)
+
+
+# Installers
+def get_installers(*args, **kwargs):
+    con = get_server_api_connection()
+    return con.get_installers(*args, **kwargs)
+
+
+def create_installer(*args, **kwargs):
+    con = get_server_api_connection()
+    return con.create_installer(*args, **kwargs)
+
+
+def update_installer(*args, **kwargs):
+    con = get_server_api_connection()
+    return con.update_installer(*args, **kwargs)
+
+
+def delete_installer(*args, **kwargs):
+    con = get_server_api_connection()
+    return con.delete_installer(*args, **kwargs)
+
+
+def download_installer(*args, **kwargs):
+    con = get_server_api_connection()
+    con.download_installer(*args, **kwargs)
+
+
+def upload_installer(*args, **kwargs):
+    con = get_server_api_connection()
+    con.upload_installer(*args, **kwargs)
+
+
+# Dependency packages
 def get_dependencies_info(*args, **kwargs):
     con = get_server_api_connection()
     return con.get_dependencies_info(*args, **kwargs)
 
 
 def update_dependency_info(*args, **kwargs):
     con = get_server_api_connection()
@@ -547,24 +594,59 @@
 
 
 def upload_dependency_package(*args, **kwargs):
     con = get_server_api_connection()
     return con.upload_dependency_package(*args, **kwargs)
 
 
+def get_dependency_packages(*args, **kwargs):
+    con = get_server_api_connection()
+    return con.get_dependency_packages(*args, **kwargs)
+
+
+def create_dependency_package(*args, **kwargs):
+    con = get_server_api_connection()
+    return con.create_dependency_package(*args, **kwargs)
+
+
+def update_dependency_package(*args, **kwargs):
+    con = get_server_api_connection()
+    return con.update_dependency_package(*args, **kwargs)
+
+
 def delete_dependency_package(*args, **kwargs):
     con = get_server_api_connection()
     return con.delete_dependency_package(*args, **kwargs)
 
 
 def get_project_anatomy_presets(*args, **kwargs):
     con = get_server_api_connection()
     return con.get_project_anatomy_presets(*args, **kwargs)
 
 
+def get_bundles(*args, **kwargs):
+    con = get_server_api_connection()
+    return con.get_bundles(*args, **kwargs)
+
+
+def create_bundle(*args, **kwargs):
+    con = get_server_api_connection()
+    return con.create_bundle(*args, **kwargs)
+
+
+def update_bundle(*args, **kwargs):
+    con = get_server_api_connection()
+    return con.update_bundle(*args, **kwargs)
+
+
+def delete_bundle(*args, **kwargs):
+    con = get_server_api_connection()
+    return con.delete_bundle(*args, **kwargs)
+
+
 def get_project_anatomy_preset(*args, **kwargs):
     con = get_server_api_connection()
     return con.get_project_anatomy_preset(*args, **kwargs)
 
 
 def get_project_roots_by_site(*args, **kwargs):
     con = get_server_api_connection()
@@ -617,14 +699,19 @@
 
 
 def get_addons_settings(*args, **kwargs):
     con = get_server_api_connection()
     return con.get_addons_settings(*args, **kwargs)
 
 
+def get_project_names(*args, **kwargs):
+    con = get_server_api_connection()
+    return con.get_project_names(*args, **kwargs)
+
+
 def get_project(*args, **kwargs):
     con = get_server_api_connection()
     return con.get_project(*args, **kwargs)
 
 
 def get_projects(*args, **kwargs):
     con = get_server_api_connection()
@@ -797,14 +884,19 @@
         project_name,
         project_code,
         library_project,
         preset_name
     )
 
 
+def update_project(project_name, *args, **kwargs):
+    con = get_server_api_connection()
+    return con.update_project(project_name, *args, **kwargs)
+
+
 def delete_project(project_name):
     con = get_server_api_connection()
     return con.delete_project(project_name)
 
 
 def get_thumbnail(project_name, entity_type, entity_id, thumbnail_id=None):
     con = get_server_api_connection()
```

### Comparing `ayon-python-api-0.2.0/ayon_api/constants.py` & `ayon-python-api-0.2.1/ayon_api/constants.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.2.0/ayon_api/entity_hub.py` & `ayon-python-api-0.2.1/ayon_api/entity_hub.py`

 * *Files 6% similar despite different names*

```diff
@@ -679,21 +679,100 @@
     def _get_delete_body(self, entity):
         return {
             "type": "delete",
             "entityType": entity.entity_type,
             "entityId": entity.id
         }
 
+    def _pre_commit_types_changes(
+        self, project_changes, orig_types, changes_key, post_changes
+    ):
+        """Compare changes of types on a project.
+
+        Compare old and new types. Change project changes content if some old
+        types were removed. In that case the  final change of types will
+        happen when all other entities have changed.
+
+        Args:
+            project_changes (dict[str, Any]): Project changes.
+            orig_types (list[dict[str, Any]]): Original types.
+            changes_key (Literal[folderTypes, taskTypes]): Key of type changes
+                in project changes.
+            post_changes (dict[str, Any]): An object where post changes will
+                be stored.
+        """
+
+        if changes_key not in project_changes:
+            return
+
+        new_types = project_changes[changes_key]
+
+        orig_types_by_name = {
+            type_info["name"]: type_info
+            for type_info in orig_types
+        }
+        new_names = {
+            type_info["name"]
+            for type_info in new_types
+        }
+        diff_names = set(orig_types_by_name) - new_names
+        if not diff_names:
+            return
+
+        # Create copy of folder type changes to post changes
+        #   - post changes will be commited at the end
+        post_changes[changes_key] = copy.deepcopy(new_types)
+
+        for type_name in diff_names:
+            new_types.append(orig_types_by_name[type_name])
+
+    def _pre_commit_project(self):
+        """Some project changes cannot be committed before hierarchy changes.
+
+        It is not possible to change folder types or task types if there are
+        existing hierarchy items using the removed types. For that purposes
+        is first committed union of all old and new types and post changes
+        are prepared when all existing entities are changed.
+
+        Returns:
+            dict[str, Any]: Changes that will be committed after hierarchy
+                changes.
+        """
+
+        project_changes = self.project_entity.changes
+
+        post_changes = {}
+        if not project_changes:
+            return post_changes
+
+        self._pre_commit_types_changes(
+            project_changes,
+            self.project_entity.get_orig_folder_types(),
+            "folderType",
+            post_changes
+        )
+        self._pre_commit_types_changes(
+            project_changes,
+            self.project_entity.get_orig_task_types(),
+            "taskType",
+            post_changes
+        )
+        self._connection.update_project(self.project_name, **project_changes)
+        return post_changes
+
     def commit_changes(self):
         """Commit any changes that happened on entities.
 
         Todos:
             Use Operations Session instead of known operations body.
         """
 
+        post_project_changes = self._pre_commit_project()
+        self.project_entity.lock()
+
         project_changes = self.project_entity.changes
         if project_changes:
             response = self._connection.patch(
                 "projects/{}".format(self.project_name),
                 **project_changes
             )
             if response.status_code != 204:
@@ -756,14 +835,17 @@
 
             if not entity.created:
                 operations_body.append(self._get_delete_body(entity))
 
         self._connection.send_batch_operations(
             self.project_name, operations_body
         )
+        if post_project_changes:
+            self._connection.update_project(
+                self.project_name, **post_project_changes)
 
         self.lock()
 
 
 class AttributeValue(object):
     def __init__(self, value):
         self._value = value
@@ -1459,25 +1541,31 @@
     def set_parent(self, parent):
         raise ValueError(
             "Parent of project cannot be set to {}".format(parent)
         )
 
     parent = property(get_parent, set_parent)
 
+    def get_orig_folder_types(self):
+        return copy.deepcopy(self._orig_folder_types)
+
     def get_folder_types(self):
         return copy.deepcopy(self._folder_types)
 
     def set_folder_types(self, folder_types):
         new_folder_types = []
         for folder_type in folder_types:
             if "icon" not in folder_type:
                 folder_type["icon"] = self.default_folder_type_icon
             new_folder_types.append(folder_type)
         self._folder_types = new_folder_types
 
+    def get_orig_task_types(self):
+        return copy.deepcopy(self._orig_task_types)
+
     def get_task_types(self):
         return copy.deepcopy(self._task_types)
 
     def set_task_types(self, task_types):
         new_task_types = []
         for task_type in task_types:
             if "icon" not in task_type:
```

### Comparing `ayon-python-api-0.2.0/ayon_api/events.py` & `ayon-python-api-0.2.1/ayon_api/events.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.2.0/ayon_api/exceptions.py` & `ayon-python-api-0.2.1/ayon_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.2.0/ayon_api/graphql.py` & `ayon-python-api-0.2.1/ayon_api/graphql.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.2.0/ayon_api/graphql_queries.py` & `ayon-python-api-0.2.1/ayon_api/graphql_queries.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.2.0/ayon_api/operations.py` & `ayon-python-api-0.2.1/ayon_api/operations.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.2.0/ayon_api/server_api.py` & `ayon-python-api-0.2.1/ayon_api/server_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 import re
 import io
 import json
 import logging
 import collections
+import datetime
 import platform
 import copy
 import uuid
 from contextlib import contextmanager
 try:
     from http import HTTPStatus
 except ImportError:
@@ -66,14 +67,22 @@
 JSONDecodeError = getattr(json, "JSONDecodeError", ValueError)
 # This should be collected from server schema
 PROJECT_NAME_ALLOWED_SYMBOLS = "a-zA-Z0-9_"
 PROJECT_NAME_REGEX = re.compile(
     "^[{}]+$".format(PROJECT_NAME_ALLOWED_SYMBOLS)
 )
 
+VERSION_REGEX = re.compile(
+    r"(?P<major>0|[1-9]\d*)"
+    r"\.(?P<minor>0|[1-9]\d*)"
+    r"\.(?P<patch>0|[1-9]\d*)"
+    r"(?:-(?P<prerelease>[a-zA-Z\d\-.]*))?"
+    r"(?:\+(?P<buildmetadata>[a-zA-Z\d\-.]*))?"
+)
+
 
 def _get_description(response):
     if HTTPStatus is None:
         return str(response.orig_response)
     return HTTPStatus(response.status).description
 
 
@@ -325,14 +334,16 @@
         self._access_token = token
         self._site_id = site_id
         self._client_version = client_version
         self._default_settings_variant = default_settings_variant
         self._access_token_is_service = None
         self._token_is_valid = None
         self._server_available = None
+        self._server_version = None
+        self._server_version_tuple = None
 
         self._session = None
 
         self._base_functions_mapping = {
             RequestTypes.get: requests.get,
             RequestTypes.post: requests.post,
             RequestTypes.put: requests.put,
@@ -627,20 +638,60 @@
         logged user info also contains information about user and machines on
         which was logged in.
 
         Todos:
             Use this method for validation of token instead of 'get_user'.
 
         Returns:
-            Dict[str, Any]: Information from server.
+            dict[str, Any]: Information from server.
         """
 
         response = self.get("info")
         return response.data
 
+    def get_server_version(self):
+        """Get server version.
+
+        Version should match semantic version (https://semver.org/).
+
+        Returns:
+            str: Server version.
+        """
+
+        if self._server_version is None:
+            self._server_version = self.get_info()["version"]
+        return self._server_version
+
+    def get_server_version_tuple(self):
+        """Get server version as tuple.
+
+        Version should match semantic version (https://semver.org/).
+
+        This function only returns first three numbers of version.
+
+        Returns:
+            Tuple[int, int, int, Union[str, None], Union[str, None]]: Server
+                version.
+        """
+
+        if self._server_version_tuple is None:
+            re_match = VERSION_REGEX.fullmatch(
+                self.get_server_version())
+            self._server_version_tuple = (
+                int(re_match.group("major")),
+                int(re_match.group("minor")),
+                int(re_match.group("patch")),
+                re_match.group("prerelease"),
+                re_match.group("buildmetadata")
+            )
+        return self._server_version_tuple
+
+    server_version = property(get_server_version)
+    server_version_tuple = property(get_server_version_tuple)
+
     def _get_user_info(self):
         if self._access_token is None:
             return None
 
         if self._access_token_is_service is not None:
             response = self.get("users/me")
             return response.data
@@ -865,15 +916,15 @@
         Events received using event server do not contain full information. To
         get the full event information is required to receive it explicitly.
 
         Args:
             event_id (str): Id of event.
 
         Returns:
-            Dict[str, Any]: Full event data.
+            dict[str, Any]: Full event data.
         """
 
         response = self.get("events/{}".format(event_id))
         response.raise_for_status()
         return response.data
 
     def get_events(
@@ -898,15 +949,15 @@
             users (Optional[Iterable[str]]): Filtering by users
                 who created/triggered an event.
             include_logs (Optional[bool]): Query also log events.
             fields (Optional[Iterable[str]]): Fields that should be received
                 for each event.
 
         Returns:
-            Generator[Dict[str, Any]]: Available events matching filters.
+            Generator[dict[str, Any]]: Available events matching filters.
         """
 
         filters = {}
         if topics is not None:
             topics = set(topics)
             if not topics:
                 return
@@ -1265,15 +1316,15 @@
     def get_server_schema(self):
         """Get server schema with info, url paths, components etc.
 
         Todos:
             Cache schema - How to find out it is outdated?
 
         Returns:
-            Dict[str, Any]: Full server schema.
+            dict[str, Any]: Full server schema.
         """
 
         url = "{}/openapi.json".format(self._base_url)
         response = self._do_rest_request(RequestTypes.get, url)
         if response:
             return response.data
         return None
@@ -1283,15 +1334,15 @@
 
         Name of components does not match entity type names e.g. 'project' is
         under 'ProjectModel'. We should find out some mapping. Also, there
         are properties which don't have information about reference to object
         e.g. 'config' has just object definition without reference schema.
 
         Returns:
-            Dict[str, Any]: Component schemas.
+            dict[str, Any]: Component schemas.
         """
 
         server_schema = self.get_server_schema()
         return server_schema["components"]["schemas"]
 
     def get_attributes_schema(self, use_cache=True):
         if not use_cache:
@@ -1391,15 +1442,15 @@
         ```
 
         Args:
             entity_type (str): Entity type for which should be attributes
                 received.
 
         Returns:
-            Dict[str, Dict[str, Any]]: Attribute schemas that are available
+            dict[str, dict[str, Any]]: Attribute schemas that are available
                 for entered entity type.
         """
         attributes = self._entity_type_attributes_cache.get(entity_type)
         if attributes is None:
             attributes_schema = self.get_attributes_schema()
             attributes = {}
             for attr in attributes_schema["attributes"]:
@@ -1559,14 +1610,156 @@
             filename
         )
         self.download_file(
             url, dst_filepath, chunk_size=chunk_size, progress=progress
         )
         return dst_filepath
 
+    def get_installers(self, version=None, platform_name=None):
+        """Information about desktop application installers on server.
+
+        Desktop application installers are helpers to download/update AYON
+        desktop application for artists.
+
+        Args:
+            version (Optional[str]): Filter installers by version.
+            platform_name (Optional[str]): Filter installers by platform name.
+
+        Returns:
+            list[dict[str, Any]]:
+        """
+
+        query_fields = [
+            "{}={}".format(key, value)
+            for key, value in (
+                ("version", version),
+                ("platform", platform_name),
+            )
+            if value
+        ]
+        query = ""
+        if query_fields:
+            query = "?{}".format(",".join(query_fields))
+
+        response = self.get("desktop/installers{}".format(query))
+        response.raise_for_status()
+        return response.data
+
+    def create_installer(
+        self,
+        filename,
+        version,
+        python_version,
+        platform_name,
+        python_modules,
+        checksum,
+        checksum_type,
+        file_size,
+        sources=None,
+    ):
+        """Create new installer information on server.
+
+        This step will create only metadata. Make sure to upload installer
+            to the server using 'upload_installer' method.
+
+        Args:
+            filename (str): Installer filename.
+            version (str): Version of installer.
+            python_version (str): Version of Python.
+            platform_name (str): Name of platform.
+            python_modules (dict[str, str]): Python modules that are available
+                in installer.
+            checksum (str): Installer file checksum.
+            checksum_type (str): Type of checksum used to create checksum.
+            file_size (int): File size.
+            sources (Optional[list[dict[str, Any]]]): List of sources that
+                can be used to download file.
+        """
+
+        body = {
+            "filename": filename,
+            "version": version,
+            "pythonVersion": python_version,
+            "platform": platform_name,
+            "pythonModules": python_modules,
+            "checksum": checksum,
+            "checksumType": checksum_type,
+            "size": file_size,
+        }
+        if sources:
+            body["sources"] = sources
+
+        response = self.post("desktop/installers", **body)
+        response.raise_for_status()
+
+    def update_installer(self, filename, sources):
+        """Update installer information on server.
+
+        Args:
+            filename (str): Installer filename.
+            sources (list[dict[str, Any]]): List of sources that
+                can be used to download file. Fully replaces existing sources.
+        """
+
+        response = self.post(
+            "desktop/installers/{}".format(filename),
+            sources=sources
+        )
+        response.raise_for_status()
+
+    def delete_installer(self, filename):
+        """Delete installer from server.
+
+        Args:
+            filename (str): Installer filename.
+        """
+
+        response = self.delete("dekstop/installers/{}".format(filename))
+        response.raise_for_status()
+
+    def download_installer(
+        self,
+        filename,
+        dst_filepath,
+        chunk_size=None,
+        progress=None
+    ):
+        """Download installer file from server.
+
+        Args:
+            filename (str): Installer filename.
+            dst_filepath (str): Destination filepath.
+            chunk_size (Optional[int]): Download chunk size.
+            progress (Optional[TransferProgress]): Object that gives ability
+                to track download progress.
+        """
+
+        self.download_file(
+            "desktop/installers/{}".format(filename),
+            dst_filepath,
+            chunk_size=chunk_size,
+            progress=progress
+        )
+
+    def upload_installer(self, src_filepath, dst_filename, progress=None):
+        """Upload installer file to server.
+
+        Args:
+            src_filepath (str): Source filepath.
+            dst_filename (str): Destination filename.
+            progress (Optional[TransferProgress]): Object that gives ability
+                to track download progress.
+        """
+
+        self.upload_file(
+            "desktop/installers/{}".format(dst_filename),
+            src_filepath,
+            progress=progress
+        )
+
     def get_dependencies_info(self):
         """Information about dependency packages on server.
 
         Example data structure:
             {
                 "packages": [
                     {
@@ -1577,21 +1770,30 @@
                         "supportedAddons": dict[str, str],
                         "pythonModules": dict[str, str]
                     }
                 ],
                 "productionPackage": str
             }
 
+        Deprecated:
+            Deprecated since server version 0.2.1. Use
+                'get_dependency_packages' instead.
+
         Returns:
             dict[str, Any]: Information about dependency packages known for
                 server.
         """
 
-        result = self.get("dependencies")
-        return result.data
+        major, minor, patch, _, _ = self.server_version_tuple
+        if major == 0 and (minor < 2 or (minor == 2 and patch < 1)):
+            result = self.get("dependencies")
+            return result.data
+        packages = self.get_dependency_packages()
+        packages["productionPackage"] = None
+        return packages
 
     def update_dependency_info(
         self,
         name,
         platform_name,
         size,
         checksum,
@@ -1600,29 +1802,34 @@
         python_modules=None,
         sources=None
     ):
         """Update or create dependency package for identifiers.
 
         The endpoint can be used to create or update dependency package.
 
+
+        Deprecated:
+            Deprecated for server version 0.2.1. Use
+                'create_dependency_pacakge' instead.
+
         Args:
             name (str): Name of dependency package.
-            platform_name (Literal["windows", "linux", "darwin"]): Platform for
-                which is dependency package targeted.
+            platform_name (Literal["windows", "linux", "darwin"]): Platform
+                for which is dependency package targeted.
             size (int): Size of dependency package in bytes.
             checksum (str): Checksum of archive file where dependencies are.
             checksum_algorithm (Optional[str]): Algorithm used to calculate
                 checksum. By default, is used 'md5' (defined by server).
-            supported_addons (Optional[Dict[str, str]]): Name of addons for
+            supported_addons (Optional[dict[str, str]]): Name of addons for
                 which was the package created.
                 '{"<addon name>": "<addon version>", ...}'
-            python_modules (Optional[Dict[str, str]]): Python modules in
+            python_modules (Optional[dict[str, str]]): Python modules in
                 dependencies package.
                 '{"<module name>": "<module version>", ...}'
-            sources (Optional[List[Dict[str, Any]]]): Information about
+            sources (Optional[list[dict[str, Any]]]): Information about
                 sources where dependency package is available.
         """
 
         kwargs = {
             key: value
             for key, value in (
                 ("checksumAlgorithm", checksum_algorithm),
@@ -1641,96 +1848,351 @@
             checksum=checksum,
             **kwargs
         )
         if response.status not in (200, 201, 204):
             raise ServerError("Failed to create/update dependency")
         return response.data
 
+    def get_dependency_packages(self):
+        """Information about dependency packages on server.
+
+        To download dependency package, use 'download_dependency_package'
+        method and pass in 'filename'.
+
+        Example data structure:
+            {
+                "packages": [
+                    {
+                        "filename": str,
+                        "platform": str,
+                        "checksum": str,
+                        "checksumAlgorithm": str,
+                        "size": int,
+                        "sources": list[dict[str, Any]],
+                        "supportedAddons": dict[str, str],
+                        "pythonModules": dict[str, str]
+                    }
+                ]
+            }
+
+        Returns:
+            dict[str, Any]: Information about dependency packages known for
+                server.
+        """
+
+        result = self.get("desktop/dependency_packages")
+        result.raise_for_status()
+        return result.data
+
+    def create_dependency_package(
+        self,
+        filename,
+        python_modules,
+        source_addons,
+        installer_version,
+        checksum,
+        checksum_algorithm,
+        file_size,
+        sources=None,
+        platform_name=None,
+    ):
+        """Create dependency package on server.
+
+        The package will be created on a server, it is also required to upload
+        the package archive file (using 'upload_dependency_package').
+
+        Args:
+            filename (str): Filename of dependency package.
+            python_modules (dict[str, str]): Python modules in dependency
+                package.
+                '{"<module name>": "<module version>", ...}'
+            source_addons (dict[str, str]): Name of addons for which is
+                dependency package created.
+                '{"<addon name>": "<addon version>", ...}'
+            installer_version (str): Version of installer for which was
+                package created.
+            checksum (str): Checksum of archive file where dependencies are.
+            checksum_algorithm (str): Algorithm used to calculate checksum.
+            file_size (Optional[int]): Size of file.
+            sources (Optional[list[dict[str, Any]]]): Information about
+                sources from where it is possible to get file.
+            platform_name (Optional[str]): Name of platform for which is
+                dependency package targeted. Default value is
+                current platform.
+        """
+
+        post_body = {
+            "filename": filename,
+            "pythonModules": python_modules,
+            "sourceAddons": source_addons,
+            "installerVersion": installer_version,
+            "checksum": checksum,
+            "checksumAlgorithm": checksum_algorithm,
+            "size": file_size,
+            "platform": platform_name or platform.system().lower(),
+        }
+        if sources:
+            post_body["sources"] = sources
+
+        response = self.post("desktop/dependency_packages", **post_body)
+        response.raise_for_status()
+
+    def update_dependency_package(self, filename, sources):
+        """Update dependency package metadata on server.
+
+        Args:
+            filename (str): Filename of dependency package.
+            sources (list[dict[str, Any]]): Information about
+                sources from where it is possible to get file. Fully replaces
+                existing sources.
+        """
+
+        response = self.patch(
+            "desktop/dependency_packages/{}".format(filename),
+            sources=sources
+        )
+        response.raise_for_status()
+
+    def delete_dependency_package(self, filename, platform_name=None):
+        """Remove dependency package for specific platform.
+
+        Args:
+            filename (str): Filename of dependency package. Or name of package
+                for server version 0.2.0 or lower.
+            platform_name (Optional[str]): Which platform of the package
+                should be removed. Current platform is used if not passed.
+                Deprecated since version 0.2.1
+        """
+
+        major, minor, patch, _, _ = self.server_version_tuple
+        if major == 0 and (minor < 2 or (minor == 2 and patch < 1)):
+            if platform_name is None:
+                platform_name = platform.system().lower()
+            url = "dependencies/{}/{}".format(filename, platform_name)
+        else:
+            url = "desktop/dependency_packages/{}".format(filename)
+
+        response = self.delete(url)
+        if response.status != 200:
+            raise ServerError("Failed to delete dependency file")
+        return response.data
+
     def download_dependency_package(
         self,
-        package_name,
+        src_filename,
         dst_directory,
-        filename,
+        dst_filename,
         platform_name=None,
         chunk_size=None,
         progress=None,
     ):
         """Download dependency package from server.
 
-        This method requires to have authorized token available. The package is
-        only downloaded.
+        This method requires to have authorized token available. The package
+        is only downloaded.
 
         Args:
-            package_name (str): Name of package to download.
+            src_filename (str): Filename of dependency pacakge.
+                For server version 0.2.0 and lower it is name of package
+                to download.
             dst_directory (str): Where the file should be downloaded.
-            filename (str): Name of destination filename.
+            dst_filename (str): Name of destination filename.
             platform_name (Optional[str]): Name of platform for which the
                 dependency package is targeted. Default value is
-                current platform.
+                current platform. Deprecated since server version 0.2.1.
             chunk_size (Optional[int]): Download chunk size.
             progress (Optional[TransferProgress]): Object that gives ability
                 to track download progress.
 
         Returns:
             str: Filepath to downloaded file.
        """
-        if platform_name is None:
-            platform_name = platform.system().lower()
 
-        package_filepath = os.path.join(dst_directory, filename)
+        major, minor, patch, _, _ = self.server_version_tuple
+        if major == 0 and (minor < 2 or (minor == 2 and patch < 1)):
+            if platform_name is None:
+                platform_name = platform.system().lower()
+            url = "dependencies/{}/{}".format(src_filename, platform_name)
+        else:
+            url = "desktop/dependency_packages/{}".format(src_filename)
+
+        package_filepath = os.path.join(dst_directory, dst_filename)
         self.download_file(
-            "dependencies/{}/{}".format(package_name, platform_name),
+            url,
             package_filepath,
             chunk_size=chunk_size,
             progress=progress
         )
         return package_filepath
 
     def upload_dependency_package(
-        self, filepath, package_name, platform_name=None, progress=None
+        self, src_filepath, dst_filename, platform_name=None, progress=None
     ):
         """Upload dependency package to server.
 
         Args:
-            filepath (str): Path to a package file.
-            package_name (str): Name of package. Must be unique.
+            src_filepath (str): Path to a package file.
+            dst_filename (str): Dependency package filename or name of package
+                for server version 0.2.0 or lower. Must be unique.
             platform_name (Optional[str]): For which platform is the
-                package targeted.
+                package targeted. Deprecated since server version 0.2.1.
             progress (Optional[TransferProgress]): Object to keep track about
                 upload state.
         """
 
-        if platform_name is None:
-            platform_name = platform.system().lower()
+        major, minor, patch, _, _ = self.server_version_tuple
+        if major == 0 and (minor < 2 or (minor == 2 and patch < 1)):
+            if platform_name is None:
+                platform_name = platform.system().lower()
+            url = "dependencies/{}/{}".format(dst_filename, platform_name)
+        else:
+            url = "desktop/dependency_packages/{}".format(dst_filename)
 
-        self.upload_file(
-            "dependencies/{}/{}".format(package_name, platform_name),
-            filepath,
-            progress=progress
-        )
+        self.upload_file(url, src_filepath, progress=progress)
 
-    def delete_dependency_package(self, package_name, platform_name=None):
-        """Remove dependency package for specific platform.
+    def create_dependency_package_basename(self, platform_name=None):
+        """Create basename for dependency package file.
 
         Args:
-            package_name (str): Name of package to remove.
-            platform_name (Optional[str]): Which platform of the package
-                should be removed. Current platform is used if not passed.
+            platform_name (Optional[str]): Name of platform for which the
+                bundle is targeted. Default value is current platform.
+
+        Returns:
+            str: Dependency package name with timestamp and platform.
         """
 
         if platform_name is None:
             platform_name = platform.system().lower()
 
-        response = self.delete(
-            "dependencies/{}/{}".format(package_name, platform_name),
-        )
-        if response.status != 200:
-            raise ServerError("Failed to delete dependency file")
+        now_date = datetime.datetime.now()
+        time_stamp = now_date.strftime("%y%m%d%H%M")
+        return "ayon_{}_{}".format(time_stamp, platform_name)
+
+    def get_bundles(self):
+        """Server bundles with basic information.
+
+        Example output:
+            {
+                "bundles": [
+                    {
+                        "name": "my_bundle",
+                        "createdAt": "2023-06-12T15:37:02.420260",
+                        "installerVersion": "1.0.0",
+                        "addons": {
+                            "core": "1.2.3"
+                        },
+                        "dependencyPackages": {
+                            "windows": "a_windows_package123.zip",
+                            "linux": "a_linux_package123.zip",
+                            "darwin": "a_mac_package123.zip"
+                        },
+                        "isProduction": False,
+                        "isStaging": False
+                    }
+                ],
+                "productionBundle": "my_bundle",
+                "stagingBundle": "test_bundle"
+            }
+
+        Returns:
+            dict[str, Any]: Server bundles with basic information.
+        """
+
+        response = self.get("desktop/bundles")
+        response.raise_for_status()
         return response.data
 
+    def create_bundle(
+        self,
+        name,
+        addon_versions,
+        installer_version,
+        dependency_packages=None,
+        is_production=None,
+        is_staging=None
+    ):
+        """Create bundle on server.
+
+        Bundle cannot be changed once is created. Only isProduction, isStaging
+        and dependency packages can change after creation.
+
+        Args:
+            name (str): Name of bundle.
+            addon_versions (dict[str, str]): Addon versions.
+            installer_version (Union[str, None]): Installer version.
+            dependency_packages (Optional[dict[str, str]]): Dependency
+                package names. Keys are platform names and values are name of
+                packages.
+            is_production (Optional[bool]): Bundle will be marked as
+                production.
+            is_staging (Optional[bool]): Bundle will be marked as staging.
+        """
+
+        body = {
+            "name": name,
+            "installerVersion": installer_version,
+            "addons": addon_versions,
+        }
+        for key, value in (
+            ("dependencyPackages", dependency_packages),
+            ("isProduction", is_production),
+            ("isStaging", is_staging),
+        ):
+            if value is not None:
+                body[key] = value
+
+        response = self.post("desktop/bundles", **body)
+        response.raise_for_status()
+
+    def update_bundle(
+        self,
+        bundle_name,
+        dependency_packages=None,
+        is_production=None,
+        is_staging=None
+    ):
+        """Update bundle on server.
+
+        Dependency packages can be update only for single platform. Others
+        will be left untouched. Use 'None' value to unset dependency package
+        from bundle.
+
+        Args:
+            bundle_name (str): Name of bundle.
+            dependency_packages (Optional[dict[str, str]]): Dependency pacakge
+                names that should be used with the bundle.
+            is_production (Optional[bool]): Bundle will be marked as
+                production.
+            is_staging (Optional[bool]): Bundle will be marked as staging.
+        """
+
+        body = {
+            key: value
+            for key, value in (
+                ("dependencyPackages", dependency_packages),
+                ("isProduction", is_production),
+                ("isStaging", is_staging),
+            )
+            if value is not None
+        }
+        response = self.patch(
+            "desktop/bundles/{}".format(bundle_name), **body
+        )
+        response.raise_for_status()
+
+    def delete_bundle(self, bundle_name):
+        """Delete bundle from server.
+
+        Args:
+            bundle_name (str): Name of bundle to delete.
+        """
+
+        response = self.delete("desktop/bundles/{}".format(bundle_name))
+        response.raise_for_status()
+
     # Anatomy presets
     def get_project_anatomy_presets(self):
         """Anatomy presets available on server.
 
         Content has basic information about presets. Example output:
             [
                 {
@@ -2146,15 +2608,15 @@
 
         This call returns project with anatomy data.
 
         Args:
             project_name (str): Name of project.
 
         Returns:
-            Union[Dict[str, Any], None]: Project entity data or 'None' if
+            Union[dict[str, Any], None]: Project entity data or 'None' if
                 project was not found.
         """
 
         if not project_name:
             return None
 
         response = self.get("projects/{}".format(project_name))
@@ -2170,15 +2632,15 @@
         Args:
             active (Optional[bool]): Filter active/inactive projects. Both
                 are returned if 'None' is passed.
             library (Optional[bool]): Filter standard/library projects. Both
                 are returned if 'None' is passed.
 
         Returns:
-            Generator[Dict[str, Any]]: Available projects.
+            Generator[dict[str, Any]]: Available projects.
         """
 
         for project_name in self.get_project_names(active, library):
             project = self.get_rest_project(project_name)
             if project:
                 yield project
 
@@ -2231,15 +2693,15 @@
         Args:
             active (Optional[bool]): Filter active/inactive projects. Both
                 are returned if 'None' is passed.
             library (Optional[bool]): Filter standard/library projects. Both
                 are returned if 'None' is passed.
 
         Returns:
-            List[str]: List of available project names.
+            list[str]: List of available project names.
         """
 
         query_keys = {}
         if active is not None:
             query_keys["active"] = "true" if active else "false"
 
         if library is not None:
@@ -2272,15 +2734,15 @@
                 disabled when 'None' is passed.
             fields (Optional[Iterable[str]]): fields to be queried
                 for project.
             own_attributes (Optional[bool]): Attribute values that are
                 not explicitly set on entity will have 'None' value.
 
         Returns:
-            Generator[Dict[str, Any]]: Queried projects.
+            Generator[dict[str, Any]]: Queried projects.
         """
 
         if fields is None:
             use_rest = True
         else:
             use_rest = False
             fields = set(fields)
@@ -2312,15 +2774,15 @@
             project_name (str): Name of project.
             fields (Optional[Iterable[str]]): fields to be queried
                 for project.
             own_attributes (Optional[bool]): Attribute values that are
                 not explicitly set on entity will have 'None' value.
 
         Returns:
-            Union[Dict[str, Any], None]: Project entity data or None
+            Union[dict[str, Any], None]: Project entity data or None
                 if project was not found.
         """
 
         use_rest = True
         if fields is not None:
             use_rest = False
             _fields = set()
@@ -3108,15 +3570,15 @@
             fields (Optional[Iterable[str]]): Fields to be queried
                 for version. All possible folder fields are returned
                 if 'None' is passed.
             own_attributes (Optional[bool]): Attribute values that are
                 not explicitly set on entity will have 'None' value.
 
         Returns:
-            Generator[Dict[str, Any]]: Queried version entities.
+            Generator[dict[str, Any]]: Queried version entities.
         """
 
         if not fields:
             fields = self.get_default_fields_for_type("version")
         fields = set(fields)
 
         if active is not None:
@@ -3566,15 +4028,15 @@
             fields (Optional[Iterable[str]]): Fields to be queried for
                 representation. All possible fields are returned if 'None' is
                 passed.
             own_attributes (Optional[bool]): Attribute values that are
                 not explicitly set on entity will have 'None' value.
 
         Returns:
-            Generator[Dict[str, Any]]: Queried representation entities.
+            Generator[dict[str, Any]]: Queried representation entities.
         """
 
         if not fields:
             fields = self.get_default_fields_for_type("representation")
         fields = set(fields)
 
         use_rest = False
@@ -4249,15 +4711,15 @@
             preset_name (Optional[str]): Name of anatomy preset. Default is
                 used if not passed.
 
         Raises:
             ValueError: When project name already exists.
 
         Returns:
-            Dict[str, Any]: Created project entity.
+            dict[str, Any]: Created project entity.
         """
 
         if self.get_project(project_name):
             raise ValueError("Project with name \"{}\" already exists".format(
                 project_name
             ))
 
@@ -4282,14 +4744,78 @@
                 details = result.data.get("detail") or details
             raise ValueError("Failed to create project \"{}\": {}".format(
                 project_name, details
             ))
 
         return self.get_project(project_name)
 
+    def update_project(
+        self,
+        project_name,
+        library=None,
+        folder_types=None,
+        task_types=None,
+        link_types=None,
+        statuses=None,
+        tags=None,
+        config=None,
+        attrib=None,
+        data=None,
+        active=None,
+        project_code=None,
+        **changes
+    ):
+        """Update project entity on server.
+
+        Args:
+            project_name (str): Name of project.
+            library (Optional[bool]): Change library state.
+            folder_types (Optional[list[dict[str, Any]]]): Folder type
+                definitions.
+            task_types (Optional[list[dict[str, Any]]]): Task type
+                definitions.
+            link_types (Optional[list[dict[str, Any]]]): Link type
+                definitions.
+            statuses (Optional[list[dict[str, Any]]]): Status definitions.
+            tags (Optional[list[dict[str, Any]]]): List of tags available to
+                set on entities.
+            config (Optional[dict[dict[str, Any]]]): Project anatomy config
+                with templates and roots.
+            attrib (Optional[dict[str, Any]]): Project attributes to change.
+            data (Optional[dict[str, Any]]): Custom data of a project. This
+                value will 100% override project data.
+            active (Optional[bool]): Change active state of a project.
+            project_code (Optional[str]): Change project code. Not recommended
+                during production.
+            **changes: Other changed keys based on Rest API documentation.
+        """
+
+        changes.update({
+            key: value
+            for key, value in (
+                ("library", library),
+                ("folderTypes", folder_types),
+                ("taskTypes", task_types),
+                ("linkTypes", link_types),
+                ("statuses", statuses),
+                ("tags", tags),
+                ("config", config),
+                ("attrib", attrib),
+                ("data", data),
+                ("active", active),
+                ("code", project_code),
+            )
+            if value is not None
+        })
+        response = self.patch(
+            "projects/{}".format(project_name),
+            **changes
+        )
+        response.raise_for_status()
+
     def delete_project(self, project_name):
         """Delete project from server.
 
         This will completely remove project from server without any step back.
 
         Args:
             project_name (str): Project name that will be removed.
```

### Comparing `ayon-python-api-0.2.0/ayon_api/thumbnails.py` & `ayon-python-api-0.2.1/ayon_api/thumbnails.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.2.0/ayon_api/utils.py` & `ayon-python-api-0.2.1/ayon_api/utils.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.2.0/ayon_python_api.egg-info/PKG-INFO` & `ayon-python-api-0.2.1/ayon_python_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ayon-python-api
-Version: 0.2.0
+Version: 0.2.1
 Summary: AYON Python API
 Home-page: https://github.com/ynput/ayon-python-api
 Author: ynput.io
 Author-email: info@ynput.io
 License: Apache License (2.0)
 Keywords: AYON,ynput,OpenPype,vfx
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ayon-python-api-0.2.0/ayon_python_api.egg-info/SOURCES.txt` & `ayon-python-api-0.2.1/ayon_python_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.2.0/setup.py` & `ayon-python-api-0.2.1/setup.py`

 * *Files identical despite different names*

