# Comparing `tmp/peek-plugin-docdb-generic-menu-3.4.1.tar.gz` & `tmp/peek-plugin-docdb-generic-menu-3.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peek-plugin-docdb-generic-menu-3.4.1.tar", last modified: Wed May 17 03:32:47 2023, max compression
+gzip compressed data, was "peek-plugin-docdb-generic-menu-3.4.2.tar", last modified: Tue Jun 13 12:00:49 2023, max compression
```

## Comparing `peek-plugin-docdb-generic-menu-3.4.1.tar` & `peek-plugin-docdb-generic-menu-3.4.2.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:32:47.202469 peek-plugin-docdb-generic-menu-3.4.1/
--rw-r--r--   0 root         (0) root         (0)      420 2023-05-17 03:32:47.202469 peek-plugin-docdb-generic-menu-3.4.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      288 2023-05-17 03:29:57.000000 peek-plugin-docdb-generic-menu-3.4.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:32:47.198469 peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/
--rw-r--r--   0 root         (0) root         (0)      679 2023-05-17 03:32:47.000000 peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:32:47.199469 peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/_private/
--rw-r--r--   0 root         (0) root         (0)      344 2023-05-17 03:29:57.000000 peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/_private/PluginNames.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 03:29:57.000000 peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/_private/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:32:47.199469 peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/_private/admin-app/
--rw-r--r--   0 root         (0) root         (0)     1631 2023-05-17 03:29:57.000000 peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/_private/admin-app/docDbGenericMenu.component.html
--rw-r--r--   0 root         (0) root         (0)      239 2023-05-17 03:29:57.000000 peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/_private/admin-app/docDbGenericMenu.component.ts
--rw-r--r--   0 root         (0) root         (0)      950 2023-05-17 03:29:57.000000 peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/_private/admin-app/docDbGenericMenu.module.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:32:47.199469 peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/_private/admin-app/edit-docdb-generic-menu-table/
--rw-r--r--   0 root         (0) root         (0)     3608 2023-05-17 03:29:57.000000 peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/_private/admin-app/edit-docdb-generic-menu-table/edit.component.html
--rw-r--r--   0 root         (0) root         (0)     2894 2023-05-17 03:29:57.000000 peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/_private/admin-app/edit-docdb-generic-menu-table/edit.component.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:32:47.199469 peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/_private/admin-app/edit-setting-table/
--rw-r--r--   0 root         (0) root         (0)     2595 2023-05-17 03:29:57.000000 peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/_private/admin-app/edit-setting-table/edit.component.html
--rw-r--r--   0 root         (0) root         (0)     1508 2023-05-17 03:29:57.000000 peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/_private/admin-app/edit-setting-table/edit.component.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:32:47.199469 peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/_private/alembic/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 03:29:57.000000 peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/_private/alembic/__init__.py
--rw-r--r--   0 root         (0) root         (0)      356 2023-05-17 03:29:57.000000 peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/_private/alembic/env.py
--rw-r--r--   0 root         (0) root         (0)      543 2023-05-17 03:29:57.000000 peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/_private/alembic/script.py.mako
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:32:47.200469 peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/_private/alembic/versions/
--rw-r--r--   0 root         (0) root         (0)     1344 2023-05-17 03:29:57.000000 peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/_private/alembic/versions/1ac6c325c7e5_added_condition.py
--rw-r--r--   0 root         (0) root         (0)     2496 2023-05-17 03:29:57.000000 peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/_private/alembic/versions/1f288982a4e2_initial.py
--rw-r--r--   0 root         (0) root         (0)     1027 2023-05-17 03:29:57.000000 peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/_private/alembic/versions/9e52cf449784_rename_diagram_to_object.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 03:29:57.000000 peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/_private/alembic/versions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1061 2023-05-17 03:29:57.000000 peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/_private/alembic/versions/bac1e4f7a3d9_renamed_diagramgeneric_table.py
--rw-r--r--   0 root         (0) root         (0)       94 2023-05-17 03:29:57.000000 peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/_private/alembic.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:32:47.200469 peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/_private/client/
--rw-r--r--   0 root         (0) root         (0)     2156 2023-05-17 03:29:57.000000 peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/_private/client/ClientEntryHook.py
--rw-r--r--   0 root         (0) root         (0)      584 2023-05-17 03:29:57.000000 peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/_private/client/DeviceTupleDataObservableProxy.py
--rw-r--r--   0 root         (0) root         (0)      572 2023-05-17 03:29:57.000000 peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/_private/client/DeviceTupleProcessorActionProxy.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 03:29:57.000000 peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/_private/client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:32:47.200469 peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/_private/server/
--rw-r--r--   0 root         (0) root         (0)      925 2023-05-17 03:29:57.000000 peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/_private/server/DocDbGenericMenuApi.py
--rw-r--r--   0 root         (0) root         (0)     6331 2023-05-17 03:29:57.000000 peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/_private/server/LogicEntryHook.py
--rw-r--r--   0 root         (0) root         (0)      609 2023-05-17 03:29:57.000000 peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/_private/server/TupleActionProcessor.py
--rw-r--r--   0 root         (0) root         (0)     1204 2023-05-17 03:29:57.000000 peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/_private/server/TupleDataObservable.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 03:29:57.000000 peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/_private/server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:32:47.200469 peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/_private/server/admin_backend/
--rw-r--r--   0 root         (0) root         (0)     1849 2023-05-17 03:29:57.000000 peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/_private/server/admin_backend/DocDbGenericMenuTableHandler.py
--rw-r--r--   0 root         (0) root         (0)     1036 2023-05-17 03:29:57.000000 peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/_private/server/admin_backend/SettingPropertyHandler.py
--rw-r--r--   0 root         (0) root         (0)      463 2023-05-17 03:29:57.000000 peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/_private/server/admin_backend/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:32:47.201469 peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/_private/server/controller/
--rw-r--r--   0 root         (0) root         (0)      720 2023-05-17 03:29:57.000000 peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/_private/server/controller/MainController.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 03:29:57.000000 peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/_private/server/controller/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:32:47.201469 peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/_private/server/tuple_providers/
--rw-r--r--   0 root         (0) root         (0)     1048 2023-05-17 03:29:57.000000 peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/_private/server/tuple_providers/DocDbGenericMenuTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 03:29:57.000000 peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/_private/server/tuple_providers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:32:47.201469 peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/_private/storage/
--rw-r--r--   0 root         (0) root         (0)      648 2023-05-17 03:29:57.000000 peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/_private/storage/DeclarativeBase.py
--rw-r--r--   0 root         (0) root         (0)      792 2023-05-17 03:29:57.000000 peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/_private/storage/DocDbGenericMenuTuple.py
--rw-r--r--   0 root         (0) root         (0)     7750 2023-05-17 03:29:57.000000 peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/_private/storage/Setting.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 03:29:57.000000 peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/_private/storage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:32:47.201469 peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/_private/tuples/
--rw-r--r--   0 root         (0) root         (0)      197 2023-05-17 03:29:57.000000 peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/_private/tuples/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:32:47.201469 peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/admin-doc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:32:47.201469 peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/admin-doc/admin_tasks/
--rw-r--r--   0 root         (0) root         (0)      794 2023-05-17 03:29:57.000000 peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/admin-doc/admin_tasks/admin_tasks.rst
--rw-r--r--   0 root         (0) root         (0)      370 2023-05-17 03:29:57.000000 peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/admin-doc/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:32:47.201469 peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/admin-doc/menus/
--rw-r--r--   0 root         (0) root         (0)    55306 2023-05-17 03:29:57.000000 peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/admin-doc/menus/menus.png
--rw-r--r--   0 root         (0) root         (0)      709 2023-05-17 03:29:57.000000 peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/admin-doc/menus/menus.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:32:47.198469 peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/plugin-module/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:32:47.201469 peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/plugin-module/_private/
--rw-r--r--   0 root         (0) root         (0)      485 2023-05-17 03:29:57.000000 peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/plugin-module/_private/PluginNames.ts
--rw-r--r--   0 root         (0) root         (0)      173 2023-05-17 03:29:57.000000 peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/plugin-module/_private/index.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:32:47.201469 peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/plugin-module/_private/services/
--rw-r--r--   0 root         (0) root         (0)     5180 2023-05-17 03:29:57.000000 peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/plugin-module/_private/services/PrivateGenericMenuService.ts
--rw-r--r--   0 root         (0) root         (0)     2047 2023-05-17 03:29:57.000000 peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/plugin-module/_private/services/PrivateGenericTupleService.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:32:47.201469 peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/plugin-module/_private/tuples/
--rw-r--r--   0 root         (0) root         (0)      593 2023-05-17 03:29:57.000000 peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/plugin-module/_private/tuples/DocDbGenericMenuTuple.ts
--rw-r--r--   0 root         (0) root         (0)      597 2023-05-17 03:29:57.000000 peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/plugin-module/_private/tuples/SettingPropertyTuple.ts
--rw-r--r--   0 root         (0) root         (0)     1692 2023-05-17 03:32:47.000000 peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/plugin_package.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:32:47.202469 peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/server/
--rw-r--r--   0 root         (0) root         (0)      430 2023-05-17 03:29:57.000000 peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/server/DocDbGenericMenuApiABC.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 03:29:57.000000 peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:32:47.202469 peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/tuples/
--rw-r--r--   0 root         (0) root         (0)      194 2023-05-17 03:29:57.000000 peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/tuples/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:32:47.199469 peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu.egg-info/
--rw-r--r--   0 root         (0) root         (0)      420 2023-05-17 03:32:47.000000 peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4168 2023-05-17 03:32:47.000000 peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 03:32:47.000000 peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-05-17 03:32:47.000000 peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-05-17 03:32:47.000000 peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-17 03:32:47.202469 peek-plugin-docdb-generic-menu-3.4.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2494 2023-05-17 03:32:47.000000 peek-plugin-docdb-generic-menu-3.4.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 12:00:49.314171 peek-plugin-docdb-generic-menu-3.4.2/
+-rw-r--r--   0 root         (0) root         (0)      420 2023-06-13 12:00:49.314171 peek-plugin-docdb-generic-menu-3.4.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      288 2023-06-13 11:58:06.000000 peek-plugin-docdb-generic-menu-3.4.2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 12:00:49.310171 peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/
+-rw-r--r--   0 root         (0) root         (0)      679 2023-06-13 12:00:49.000000 peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 12:00:49.311172 peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/_private/
+-rw-r--r--   0 root         (0) root         (0)      344 2023-06-13 11:58:06.000000 peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/_private/PluginNames.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 11:58:06.000000 peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/_private/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 12:00:49.311172 peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/_private/admin-app/
+-rw-r--r--   0 root         (0) root         (0)     1631 2023-06-13 11:58:06.000000 peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/_private/admin-app/docDbGenericMenu.component.html
+-rw-r--r--   0 root         (0) root         (0)      239 2023-06-13 11:58:06.000000 peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/_private/admin-app/docDbGenericMenu.component.ts
+-rw-r--r--   0 root         (0) root         (0)      950 2023-06-13 11:58:06.000000 peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/_private/admin-app/docDbGenericMenu.module.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 12:00:49.311172 peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/_private/admin-app/edit-docdb-generic-menu-table/
+-rw-r--r--   0 root         (0) root         (0)     3608 2023-06-13 11:58:06.000000 peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/_private/admin-app/edit-docdb-generic-menu-table/edit.component.html
+-rw-r--r--   0 root         (0) root         (0)     2894 2023-06-13 11:58:06.000000 peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/_private/admin-app/edit-docdb-generic-menu-table/edit.component.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 12:00:49.311172 peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/_private/admin-app/edit-setting-table/
+-rw-r--r--   0 root         (0) root         (0)     2595 2023-06-13 11:58:06.000000 peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/_private/admin-app/edit-setting-table/edit.component.html
+-rw-r--r--   0 root         (0) root         (0)     1508 2023-06-13 11:58:06.000000 peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/_private/admin-app/edit-setting-table/edit.component.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 12:00:49.311172 peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/_private/alembic/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 11:58:06.000000 peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/_private/alembic/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      356 2023-06-13 11:58:06.000000 peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/_private/alembic/env.py
+-rw-r--r--   0 root         (0) root         (0)      543 2023-06-13 11:58:06.000000 peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/_private/alembic/script.py.mako
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 12:00:49.312172 peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/_private/alembic/versions/
+-rw-r--r--   0 root         (0) root         (0)     1344 2023-06-13 11:58:06.000000 peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/_private/alembic/versions/1ac6c325c7e5_added_condition.py
+-rw-r--r--   0 root         (0) root         (0)     2496 2023-06-13 11:58:06.000000 peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/_private/alembic/versions/1f288982a4e2_initial.py
+-rw-r--r--   0 root         (0) root         (0)     1027 2023-06-13 11:58:06.000000 peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/_private/alembic/versions/9e52cf449784_rename_diagram_to_object.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 11:58:06.000000 peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/_private/alembic/versions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1061 2023-06-13 11:58:06.000000 peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/_private/alembic/versions/bac1e4f7a3d9_renamed_diagramgeneric_table.py
+-rw-r--r--   0 root         (0) root         (0)       94 2023-06-13 11:58:06.000000 peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/_private/alembic.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 12:00:49.312172 peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/_private/client/
+-rw-r--r--   0 root         (0) root         (0)     2156 2023-06-13 11:58:06.000000 peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/_private/client/ClientEntryHook.py
+-rw-r--r--   0 root         (0) root         (0)      584 2023-06-13 11:58:06.000000 peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/_private/client/DeviceTupleDataObservableProxy.py
+-rw-r--r--   0 root         (0) root         (0)      572 2023-06-13 11:58:06.000000 peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/_private/client/DeviceTupleProcessorActionProxy.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 11:58:06.000000 peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/_private/client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 12:00:49.312172 peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/_private/server/
+-rw-r--r--   0 root         (0) root         (0)      925 2023-06-13 11:58:06.000000 peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/_private/server/DocDbGenericMenuApi.py
+-rw-r--r--   0 root         (0) root         (0)     6331 2023-06-13 11:58:06.000000 peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/_private/server/LogicEntryHook.py
+-rw-r--r--   0 root         (0) root         (0)      609 2023-06-13 11:58:06.000000 peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/_private/server/TupleActionProcessor.py
+-rw-r--r--   0 root         (0) root         (0)     1204 2023-06-13 11:58:06.000000 peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/_private/server/TupleDataObservable.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 11:58:06.000000 peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/_private/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 12:00:49.312172 peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/_private/server/admin_backend/
+-rw-r--r--   0 root         (0) root         (0)     1849 2023-06-13 11:58:06.000000 peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/_private/server/admin_backend/DocDbGenericMenuTableHandler.py
+-rw-r--r--   0 root         (0) root         (0)     1036 2023-06-13 11:58:06.000000 peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/_private/server/admin_backend/SettingPropertyHandler.py
+-rw-r--r--   0 root         (0) root         (0)      463 2023-06-13 11:58:06.000000 peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/_private/server/admin_backend/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 12:00:49.312172 peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/_private/server/controller/
+-rw-r--r--   0 root         (0) root         (0)      720 2023-06-13 11:58:06.000000 peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/_private/server/controller/MainController.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 11:58:06.000000 peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/_private/server/controller/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 12:00:49.312172 peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/_private/server/tuple_providers/
+-rw-r--r--   0 root         (0) root         (0)     1048 2023-06-13 11:58:06.000000 peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/_private/server/tuple_providers/DocDbGenericMenuTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 11:58:06.000000 peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/_private/server/tuple_providers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 12:00:49.313171 peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/_private/storage/
+-rw-r--r--   0 root         (0) root         (0)      648 2023-06-13 11:58:06.000000 peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/_private/storage/DeclarativeBase.py
+-rw-r--r--   0 root         (0) root         (0)      792 2023-06-13 11:58:06.000000 peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/_private/storage/DocDbGenericMenuTuple.py
+-rw-r--r--   0 root         (0) root         (0)     7750 2023-06-13 11:58:06.000000 peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/_private/storage/Setting.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 11:58:06.000000 peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/_private/storage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 12:00:49.313171 peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/_private/tuples/
+-rw-r--r--   0 root         (0) root         (0)      197 2023-06-13 11:58:06.000000 peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/_private/tuples/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 12:00:49.313171 peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/admin-doc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 12:00:49.313171 peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/admin-doc/admin_tasks/
+-rw-r--r--   0 root         (0) root         (0)      794 2023-06-13 11:58:06.000000 peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/admin-doc/admin_tasks/admin_tasks.rst
+-rw-r--r--   0 root         (0) root         (0)      370 2023-06-13 11:58:06.000000 peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/admin-doc/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 12:00:49.313171 peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/admin-doc/menus/
+-rw-r--r--   0 root         (0) root         (0)    55306 2023-06-13 11:58:06.000000 peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/admin-doc/menus/menus.png
+-rw-r--r--   0 root         (0) root         (0)      709 2023-06-13 11:58:06.000000 peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/admin-doc/menus/menus.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 12:00:49.310171 peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/plugin-module/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 12:00:49.313171 peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/plugin-module/_private/
+-rw-r--r--   0 root         (0) root         (0)      485 2023-06-13 11:58:06.000000 peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/plugin-module/_private/PluginNames.ts
+-rw-r--r--   0 root         (0) root         (0)      173 2023-06-13 11:58:06.000000 peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/plugin-module/_private/index.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 12:00:49.313171 peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/plugin-module/_private/services/
+-rw-r--r--   0 root         (0) root         (0)     5180 2023-06-13 11:58:06.000000 peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/plugin-module/_private/services/PrivateGenericMenuService.ts
+-rw-r--r--   0 root         (0) root         (0)     2047 2023-06-13 11:58:06.000000 peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/plugin-module/_private/services/PrivateGenericTupleService.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 12:00:49.313171 peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/plugin-module/_private/tuples/
+-rw-r--r--   0 root         (0) root         (0)      593 2023-06-13 11:58:06.000000 peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/plugin-module/_private/tuples/DocDbGenericMenuTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      597 2023-06-13 11:58:06.000000 peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/plugin-module/_private/tuples/SettingPropertyTuple.ts
+-rw-r--r--   0 root         (0) root         (0)     1692 2023-06-13 12:00:49.000000 peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/plugin_package.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 12:00:49.313171 peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/server/
+-rw-r--r--   0 root         (0) root         (0)      430 2023-06-13 11:58:06.000000 peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/server/DocDbGenericMenuApiABC.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 11:58:06.000000 peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 12:00:49.313171 peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/tuples/
+-rw-r--r--   0 root         (0) root         (0)      194 2023-06-13 11:58:06.000000 peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/tuples/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 12:00:49.311172 peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      420 2023-06-13 12:00:49.000000 peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4168 2023-06-13 12:00:49.000000 peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 12:00:49.000000 peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-06-13 12:00:49.000000 peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-06-13 12:00:49.000000 peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-13 12:00:49.314171 peek-plugin-docdb-generic-menu-3.4.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2494 2023-06-13 12:00:49.000000 peek-plugin-docdb-generic-menu-3.4.2/setup.py
```

### Comparing `peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/__init__.py` & `peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from peek_plugin_base.server.PluginLogicEntryHookABC import PluginLogicEntryHookABC
 from peek_plugin_base.client.PluginClientEntryHookABC import PluginClientEntryHookABC
 from typing import Type
 
-__version__ = '3.4.1'
+__version__ = '3.4.2'
 
 
 def peekLogicEntryHook() -> Type[PluginLogicEntryHookABC]:
     from ._private.server.LogicEntryHook import LogicEntryHook
 
     return LogicEntryHook
```

### Comparing `peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/_private/admin-app/docDbGenericMenu.component.html` & `peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/_private/admin-app/docDbGenericMenu.component.html`

 * *Files identical despite different names*

### Comparing `peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/_private/admin-app/docDbGenericMenu.module.ts` & `peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/_private/admin-app/docDbGenericMenu.module.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/_private/admin-app/edit-docdb-generic-menu-table/edit.component.html` & `peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/_private/admin-app/edit-docdb-generic-menu-table/edit.component.html`

 * *Files identical despite different names*

### Comparing `peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/_private/admin-app/edit-docdb-generic-menu-table/edit.component.ts` & `peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/_private/admin-app/edit-docdb-generic-menu-table/edit.component.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/_private/admin-app/edit-setting-table/edit.component.html` & `peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/_private/admin-app/edit-setting-table/edit.component.html`

 * *Files identical despite different names*

### Comparing `peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/_private/admin-app/edit-setting-table/edit.component.ts` & `peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/_private/admin-app/edit-setting-table/edit.component.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/_private/alembic/script.py.mako` & `peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/_private/alembic/script.py.mako`

 * *Files identical despite different names*

### Comparing `peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/_private/alembic/versions/1ac6c325c7e5_added_condition.py` & `peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/_private/alembic/versions/1ac6c325c7e5_added_condition.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/_private/alembic/versions/1f288982a4e2_initial.py` & `peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/_private/alembic/versions/1f288982a4e2_initial.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/_private/alembic/versions/9e52cf449784_rename_diagram_to_object.py` & `peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/_private/alembic/versions/9e52cf449784_rename_diagram_to_object.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/_private/alembic/versions/bac1e4f7a3d9_renamed_diagramgeneric_table.py` & `peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/_private/alembic/versions/bac1e4f7a3d9_renamed_diagramgeneric_table.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/_private/client/ClientEntryHook.py` & `peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/_private/client/ClientEntryHook.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/_private/client/DeviceTupleDataObservableProxy.py` & `peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/_private/client/DeviceTupleDataObservableProxy.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/_private/client/DeviceTupleProcessorActionProxy.py` & `peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/_private/client/DeviceTupleProcessorActionProxy.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/_private/server/DocDbGenericMenuApi.py` & `peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/_private/server/DocDbGenericMenuApi.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/_private/server/LogicEntryHook.py` & `peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/_private/server/LogicEntryHook.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/_private/server/TupleActionProcessor.py` & `peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/_private/server/TupleActionProcessor.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/_private/server/TupleDataObservable.py` & `peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/_private/server/TupleDataObservable.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/_private/server/admin_backend/DocDbGenericMenuTableHandler.py` & `peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/_private/server/admin_backend/DocDbGenericMenuTableHandler.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/_private/server/admin_backend/SettingPropertyHandler.py` & `peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/_private/server/admin_backend/SettingPropertyHandler.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/_private/server/controller/MainController.py` & `peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/_private/server/controller/MainController.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/_private/server/tuple_providers/DocDbGenericMenuTupleProvider.py` & `peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/_private/server/tuple_providers/DocDbGenericMenuTupleProvider.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/_private/storage/DeclarativeBase.py` & `peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/_private/storage/DeclarativeBase.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/_private/storage/DocDbGenericMenuTuple.py` & `peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/_private/storage/DocDbGenericMenuTuple.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/_private/storage/Setting.py` & `peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/_private/storage/Setting.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/admin-doc/admin_tasks/admin_tasks.rst` & `peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/admin-doc/admin_tasks/admin_tasks.rst`

 * *Files identical despite different names*

### Comparing `peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/admin-doc/menus/menus.png` & `peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/admin-doc/menus/menus.png`

 * *Files identical despite different names*

### Comparing `peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/admin-doc/menus/menus.rst` & `peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/admin-doc/menus/menus.rst`

 * *Files identical despite different names*

### Comparing `peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/plugin-module/_private/services/PrivateGenericMenuService.ts` & `peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/plugin-module/_private/services/PrivateGenericMenuService.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/plugin-module/_private/services/PrivateGenericTupleService.ts` & `peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/plugin-module/_private/services/PrivateGenericTupleService.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/plugin-module/_private/tuples/DocDbGenericMenuTuple.ts` & `peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/plugin-module/_private/tuples/DocDbGenericMenuTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/plugin-module/_private/tuples/SettingPropertyTuple.ts` & `peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/plugin-module/_private/tuples/SettingPropertyTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu/plugin_package.json` & `peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu/plugin_package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9955357142857143%*

 * *Differences: {"'plugin'": "{'version': '3.4.2'}"}*

```diff
@@ -40,15 +40,15 @@
     },
     "plugin": {
         "buildDate": "#BUILD_DATE#",
         "buildNumber": "#PLUGIN_BUILD#",
         "creator": "Synerty Pty Ltd",
         "packageName": "peek_plugin_docdb_generic_menu",
         "title": "DocDB Generic Menu",
-        "version": "3.4.1",
+        "version": "3.4.2",
         "website": "www.synerty.com"
     },
     "requiresServices": [
         "logic",
         "storage",
         "admin",
         "field",
```

### Comparing `peek-plugin-docdb-generic-menu-3.4.1/peek_plugin_docdb_generic_menu.egg-info/SOURCES.txt` & `peek-plugin-docdb-generic-menu-3.4.2/peek_plugin_docdb_generic_menu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `peek-plugin-docdb-generic-menu-3.4.1/setup.py` & `peek-plugin-docdb-generic-menu-3.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #
 # Modify these values to fork a new plugin
 #
 author = "Synerty"
 author_email = "contact@synerty.com"
 py_package_name = "peek_plugin_docdb_generic_menu"
 pip_package_name = py_package_name.replace("_", "-")
-package_version = "3.4.1"
+package_version = "3.4.2"
 description = "Peek Plugin DocDB Generic Menu"
 
 download_url = "https://bitbucket.org/synerty/%s/get/%s.zip"
 download_url %= pip_package_name, package_version
 url = "https://bitbucket.org/synerty/%s" % pip_package_name
 
 #
```

