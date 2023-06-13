# Comparing `tmp/peek-abstract-chunked-data-loader-3.4.1.tar.gz` & `tmp/peek-abstract-chunked-data-loader-3.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peek-abstract-chunked-data-loader-3.4.1.tar", last modified: Wed May 17 03:30:22 2023, max compression
+gzip compressed data, was "peek-abstract-chunked-data-loader-3.4.2.tar", last modified: Tue Jun 13 11:58:31 2023, max compression
```

## Comparing `peek-abstract-chunked-data-loader-3.4.1.tar` & `peek-abstract-chunked-data-loader-3.4.2.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:30:22.864295 peek-abstract-chunked-data-loader-3.4.1/
--rw-r--r--   0 root         (0) root         (0)      453 2023-05-17 03:30:22.864295 peek-abstract-chunked-data-loader-3.4.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      301 2023-05-17 03:29:54.000000 peek-abstract-chunked-data-loader-3.4.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:30:22.861295 peek-abstract-chunked-data-loader-3.4.1/peek_abstract_chunked_data_loader/
--rw-r--r--   0 root         (0) root         (0)      460 2023-05-17 03:29:54.000000 peek-abstract-chunked-data-loader-3.4.1/peek_abstract_chunked_data_loader/PlatformDependencyTest.py
--rw-r--r--   0 root         (0) root         (0)      599 2023-05-17 03:30:22.000000 peek-abstract-chunked-data-loader-3.4.1/peek_abstract_chunked_data_loader/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:30:22.862295 peek-abstract-chunked-data-loader-3.4.1/peek_abstract_chunked_data_loader/private/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 03:29:54.000000 peek-abstract-chunked-data-loader-3.4.1/peek_abstract_chunked_data_loader/private/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:30:22.862295 peek-abstract-chunked-data-loader-3.4.1/peek_abstract_chunked_data_loader/private/admin-app.abctodo/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 03:29:54.000000 peek-abstract-chunked-data-loader-3.4.1/peek_abstract_chunked_data_loader/private/admin-app.abctodo/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2905 2023-05-17 03:29:54.000000 peek-abstract-chunked-data-loader-3.4.1/peek_abstract_chunked_data_loader/private/admin-app.abctodo/abstracDataLoader.component.html
--rw-r--r--   0 root         (0) root         (0)      243 2023-05-17 03:29:54.000000 peek-abstract-chunked-data-loader-3.4.1/peek_abstract_chunked_data_loader/private/admin-app.abctodo/abstracDataLoader.component.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:30:22.862295 peek-abstract-chunked-data-loader-3.4.1/peek_abstract_chunked_data_loader/private/admin-app.abctodo/edit-setting-table/
--rw-r--r--   0 root         (0) root         (0)     2977 2023-05-17 03:29:54.000000 peek-abstract-chunked-data-loader-3.4.1/peek_abstract_chunked_data_loader/private/admin-app.abctodo/edit-setting-table/edit.component.html
--rw-r--r--   0 root         (0) root         (0)     1520 2023-05-17 03:29:54.000000 peek-abstract-chunked-data-loader-3.4.1/peek_abstract_chunked_data_loader/private/admin-app.abctodo/edit-setting-table/edit.component.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:30:22.862295 peek-abstract-chunked-data-loader-3.4.1/peek_abstract_chunked_data_loader/private/admin-app.abctodo/edit-source-settings/
--rw-r--r--   0 root         (0) root         (0)     1890 2023-05-17 03:29:54.000000 peek-abstract-chunked-data-loader-3.4.1/peek_abstract_chunked_data_loader/private/admin-app.abctodo/edit-source-settings/edit.component.html
--rw-r--r--   0 root         (0) root         (0)     1788 2023-05-17 03:29:54.000000 peek-abstract-chunked-data-loader-3.4.1/peek_abstract_chunked_data_loader/private/admin-app.abctodo/edit-source-settings/edit.component.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:30:22.862295 peek-abstract-chunked-data-loader-3.4.1/peek_abstract_chunked_data_loader/private/admin-app.abctodo/status/
--rw-r--r--   0 root         (0) root         (0)      476 2023-05-17 03:29:54.000000 peek-abstract-chunked-data-loader-3.4.1/peek_abstract_chunked_data_loader/private/admin-app.abctodo/status/status.component.html
--rw-r--r--   0 root         (0) root         (0)      998 2023-05-17 03:29:54.000000 peek-abstract-chunked-data-loader-3.4.1/peek_abstract_chunked_data_loader/private/admin-app.abctodo/status/status.component.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:30:22.862295 peek-abstract-chunked-data-loader-3.4.1/peek_abstract_chunked_data_loader/private/admin-app.abctodo/tuples/
--rw-r--r--   0 root         (0) root         (0)      615 2023-05-17 03:29:54.000000 peek-abstract-chunked-data-loader-3.4.1/peek_abstract_chunked_data_loader/private/admin-app.abctodo/tuples/AppServerSettingsTuple.ts
--rw-r--r--   0 root         (0) root         (0)      436 2023-05-17 03:29:54.000000 peek-abstract-chunked-data-loader-3.4.1/peek_abstract_chunked_data_loader/private/admin-app.abctodo/tuples/LoaderStatusTuple.ts
--rw-r--r--   0 root         (0) root         (0)      624 2023-05-17 03:29:54.000000 peek-abstract-chunked-data-loader-3.4.1/peek_abstract_chunked_data_loader/private/admin-app.abctodo/tuples/SettingPropertyTuple.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:30:22.863295 peek-abstract-chunked-data-loader-3.4.1/peek_abstract_chunked_data_loader/private/agent/
--rw-r--r--   0 root         (0) root         (0)      883 2023-05-17 03:29:54.000000 peek-abstract-chunked-data-loader-3.4.1/peek_abstract_chunked_data_loader/private/agent/AgentController.py.abctodo
--rw-r--r--   0 root         (0) root         (0)     4611 2023-05-17 03:29:54.000000 peek-abstract-chunked-data-loader-3.4.1/peek_abstract_chunked_data_loader/private/agent/AgentEntryHook.py.abctodo
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 03:29:54.000000 peek-abstract-chunked-data-loader-3.4.1/peek_abstract_chunked_data_loader/private/agent/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:30:22.863295 peek-abstract-chunked-data-loader-3.4.1/peek_abstract_chunked_data_loader/private/agent/imp/
--rw-r--r--   0 root         (0) root         (0)     7067 2023-05-17 03:29:54.000000 peek-abstract-chunked-data-loader-3.4.1/peek_abstract_chunked_data_loader/private/agent/imp/DataImportChunk.py.abctodo
--rw-r--r--   0 root         (0) root         (0)    10593 2023-05-17 03:29:54.000000 peek-abstract-chunked-data-loader-3.4.1/peek_abstract_chunked_data_loader/private/agent/imp/DataImportChunks.py.abctodo
--rw-r--r--   0 root         (0) root         (0)       20 2023-05-17 03:29:54.000000 peek-abstract-chunked-data-loader-3.4.1/peek_abstract_chunked_data_loader/private/agent/imp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:30:22.863295 peek-abstract-chunked-data-loader-3.4.1/peek_abstract_chunked_data_loader/private/server/
--rw-r--r--   0 root         (0) root         (0)     4354 2023-05-17 03:29:54.000000 peek-abstract-chunked-data-loader-3.4.1/peek_abstract_chunked_data_loader/private/server/LogicEntryHook.py.abctodo
--rw-r--r--   0 root         (0) root         (0)      604 2023-05-17 03:29:54.000000 peek-abstract-chunked-data-loader-3.4.1/peek_abstract_chunked_data_loader/private/server/TupleActionProcessor.py.abctodo
--rw-r--r--   0 root         (0) root         (0)     1425 2023-05-17 03:29:54.000000 peek-abstract-chunked-data-loader-3.4.1/peek_abstract_chunked_data_loader/private/server/TupleDataObservable.py.abctodo
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 03:29:54.000000 peek-abstract-chunked-data-loader-3.4.1/peek_abstract_chunked_data_loader/private/server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:30:22.863295 peek-abstract-chunked-data-loader-3.4.1/peek_abstract_chunked_data_loader/private/server/admin_backend/
--rw-r--r--   0 root         (0) root         (0)     1292 2023-05-17 03:29:54.000000 peek-abstract-chunked-data-loader-3.4.1/peek_abstract_chunked_data_loader/private/server/admin_backend/AppSettingHandler.py.abctodo
--rw-r--r--   0 root         (0) root         (0)     1044 2023-05-17 03:29:54.000000 peek-abstract-chunked-data-loader-3.4.1/peek_abstract_chunked_data_loader/private/server/admin_backend/SettingPropertyHandler.py.abctodo
--rw-r--r--   0 root         (0) root         (0)      969 2023-05-17 03:29:54.000000 peek-abstract-chunked-data-loader-3.4.1/peek_abstract_chunked_data_loader/private/server/admin_backend/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:30:22.863295 peek-abstract-chunked-data-loader-3.4.1/peek_abstract_chunked_data_loader/private/server/agent_handlers/
--rw-r--r--   0 root         (0) root         (0)     2005 2023-05-17 03:29:54.000000 peek-abstract-chunked-data-loader-3.4.1/peek_abstract_chunked_data_loader/private/server/agent_handlers/ACDLRpcForAgentImportABC.py
--rw-r--r--   0 root         (0) root         (0)     3675 2023-05-17 03:29:54.000000 peek-abstract-chunked-data-loader-3.4.1/peek_abstract_chunked_data_loader/private/server/agent_handlers/ADLRpcForAgentABC.py.abctodo
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 03:29:54.000000 peek-abstract-chunked-data-loader-3.4.1/peek_abstract_chunked_data_loader/private/server/agent_handlers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:30:22.863295 peek-abstract-chunked-data-loader-3.4.1/peek_abstract_chunked_data_loader/private/server/controller/
--rw-r--r--   0 root         (0) root         (0)     1009 2023-05-17 03:29:54.000000 peek-abstract-chunked-data-loader-3.4.1/peek_abstract_chunked_data_loader/private/server/controller/MainController.py.abctodo
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 03:29:54.000000 peek-abstract-chunked-data-loader-3.4.1/peek_abstract_chunked_data_loader/private/server/controller/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:30:22.863295 peek-abstract-chunked-data-loader-3.4.1/peek_abstract_chunked_data_loader/private/server/tuple_providers/
--rw-r--r--   0 root         (0) root         (0)      928 2023-05-17 03:29:54.000000 peek-abstract-chunked-data-loader-3.4.1/peek_abstract_chunked_data_loader/private/server/tuple_providers/LoaderStatusTupleProvider.py.abctodo
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 03:29:54.000000 peek-abstract-chunked-data-loader-3.4.1/peek_abstract_chunked_data_loader/private/server/tuple_providers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:30:22.864295 peek-abstract-chunked-data-loader-3.4.1/peek_abstract_chunked_data_loader/private/tuples/
--rw-r--r--   0 root         (0) root         (0)     1357 2023-05-17 03:29:54.000000 peek-abstract-chunked-data-loader-3.4.1/peek_abstract_chunked_data_loader/private/tuples/ACDLChunkLoadStateTupleABC.py
--rw-r--r--   0 root         (0) root         (0)      779 2023-05-17 03:29:54.000000 peek-abstract-chunked-data-loader-3.4.1/peek_abstract_chunked_data_loader/private/tuples/AppServerSettingsTuple.py.abctodo
--rw-r--r--   0 root         (0) root         (0)      485 2023-05-17 03:29:54.000000 peek-abstract-chunked-data-loader-3.4.1/peek_abstract_chunked_data_loader/private/tuples/LoaderStatusTuple.py.abctodo
--rw-r--r--   0 root         (0) root         (0)      348 2023-05-17 03:29:54.000000 peek-abstract-chunked-data-loader-3.4.1/peek_abstract_chunked_data_loader/private/tuples/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:30:22.862295 peek-abstract-chunked-data-loader-3.4.1/peek_abstract_chunked_data_loader.egg-info/
--rw-r--r--   0 root         (0) root         (0)      453 2023-05-17 03:30:22.000000 peek-abstract-chunked-data-loader-3.4.1/peek_abstract_chunked_data_loader.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3455 2023-05-17 03:30:22.000000 peek-abstract-chunked-data-loader-3.4.1/peek_abstract_chunked_data_loader.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 03:30:22.000000 peek-abstract-chunked-data-loader-3.4.1/peek_abstract_chunked_data_loader.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-05-17 03:30:22.000000 peek-abstract-chunked-data-loader-3.4.1/peek_abstract_chunked_data_loader.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       34 2023-05-17 03:30:22.000000 peek-abstract-chunked-data-loader-3.4.1/peek_abstract_chunked_data_loader.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-17 03:30:22.864295 peek-abstract-chunked-data-loader-3.4.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2521 2023-05-17 03:30:22.000000 peek-abstract-chunked-data-loader-3.4.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 11:58:31.808889 peek-abstract-chunked-data-loader-3.4.2/
+-rw-r--r--   0 root         (0) root         (0)      453 2023-06-13 11:58:31.808889 peek-abstract-chunked-data-loader-3.4.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      301 2023-06-13 11:58:03.000000 peek-abstract-chunked-data-loader-3.4.2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 11:58:31.806889 peek-abstract-chunked-data-loader-3.4.2/peek_abstract_chunked_data_loader/
+-rw-r--r--   0 root         (0) root         (0)      460 2023-06-13 11:58:03.000000 peek-abstract-chunked-data-loader-3.4.2/peek_abstract_chunked_data_loader/PlatformDependencyTest.py
+-rw-r--r--   0 root         (0) root         (0)      599 2023-06-13 11:58:31.000000 peek-abstract-chunked-data-loader-3.4.2/peek_abstract_chunked_data_loader/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 11:58:31.806889 peek-abstract-chunked-data-loader-3.4.2/peek_abstract_chunked_data_loader/private/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 11:58:03.000000 peek-abstract-chunked-data-loader-3.4.2/peek_abstract_chunked_data_loader/private/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 11:58:31.806889 peek-abstract-chunked-data-loader-3.4.2/peek_abstract_chunked_data_loader/private/admin-app.abctodo/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 11:58:03.000000 peek-abstract-chunked-data-loader-3.4.2/peek_abstract_chunked_data_loader/private/admin-app.abctodo/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2905 2023-06-13 11:58:03.000000 peek-abstract-chunked-data-loader-3.4.2/peek_abstract_chunked_data_loader/private/admin-app.abctodo/abstracDataLoader.component.html
+-rw-r--r--   0 root         (0) root         (0)      243 2023-06-13 11:58:03.000000 peek-abstract-chunked-data-loader-3.4.2/peek_abstract_chunked_data_loader/private/admin-app.abctodo/abstracDataLoader.component.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 11:58:31.806889 peek-abstract-chunked-data-loader-3.4.2/peek_abstract_chunked_data_loader/private/admin-app.abctodo/edit-setting-table/
+-rw-r--r--   0 root         (0) root         (0)     2977 2023-06-13 11:58:03.000000 peek-abstract-chunked-data-loader-3.4.2/peek_abstract_chunked_data_loader/private/admin-app.abctodo/edit-setting-table/edit.component.html
+-rw-r--r--   0 root         (0) root         (0)     1520 2023-06-13 11:58:03.000000 peek-abstract-chunked-data-loader-3.4.2/peek_abstract_chunked_data_loader/private/admin-app.abctodo/edit-setting-table/edit.component.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 11:58:31.807890 peek-abstract-chunked-data-loader-3.4.2/peek_abstract_chunked_data_loader/private/admin-app.abctodo/edit-source-settings/
+-rw-r--r--   0 root         (0) root         (0)     1890 2023-06-13 11:58:03.000000 peek-abstract-chunked-data-loader-3.4.2/peek_abstract_chunked_data_loader/private/admin-app.abctodo/edit-source-settings/edit.component.html
+-rw-r--r--   0 root         (0) root         (0)     1788 2023-06-13 11:58:03.000000 peek-abstract-chunked-data-loader-3.4.2/peek_abstract_chunked_data_loader/private/admin-app.abctodo/edit-source-settings/edit.component.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 11:58:31.807890 peek-abstract-chunked-data-loader-3.4.2/peek_abstract_chunked_data_loader/private/admin-app.abctodo/status/
+-rw-r--r--   0 root         (0) root         (0)      476 2023-06-13 11:58:03.000000 peek-abstract-chunked-data-loader-3.4.2/peek_abstract_chunked_data_loader/private/admin-app.abctodo/status/status.component.html
+-rw-r--r--   0 root         (0) root         (0)      998 2023-06-13 11:58:03.000000 peek-abstract-chunked-data-loader-3.4.2/peek_abstract_chunked_data_loader/private/admin-app.abctodo/status/status.component.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 11:58:31.807890 peek-abstract-chunked-data-loader-3.4.2/peek_abstract_chunked_data_loader/private/admin-app.abctodo/tuples/
+-rw-r--r--   0 root         (0) root         (0)      615 2023-06-13 11:58:03.000000 peek-abstract-chunked-data-loader-3.4.2/peek_abstract_chunked_data_loader/private/admin-app.abctodo/tuples/AppServerSettingsTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      436 2023-06-13 11:58:03.000000 peek-abstract-chunked-data-loader-3.4.2/peek_abstract_chunked_data_loader/private/admin-app.abctodo/tuples/LoaderStatusTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      624 2023-06-13 11:58:03.000000 peek-abstract-chunked-data-loader-3.4.2/peek_abstract_chunked_data_loader/private/admin-app.abctodo/tuples/SettingPropertyTuple.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 11:58:31.807890 peek-abstract-chunked-data-loader-3.4.2/peek_abstract_chunked_data_loader/private/agent/
+-rw-r--r--   0 root         (0) root         (0)      883 2023-06-13 11:58:03.000000 peek-abstract-chunked-data-loader-3.4.2/peek_abstract_chunked_data_loader/private/agent/AgentController.py.abctodo
+-rw-r--r--   0 root         (0) root         (0)     4611 2023-06-13 11:58:03.000000 peek-abstract-chunked-data-loader-3.4.2/peek_abstract_chunked_data_loader/private/agent/AgentEntryHook.py.abctodo
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 11:58:03.000000 peek-abstract-chunked-data-loader-3.4.2/peek_abstract_chunked_data_loader/private/agent/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 11:58:31.807890 peek-abstract-chunked-data-loader-3.4.2/peek_abstract_chunked_data_loader/private/agent/imp/
+-rw-r--r--   0 root         (0) root         (0)     7067 2023-06-13 11:58:03.000000 peek-abstract-chunked-data-loader-3.4.2/peek_abstract_chunked_data_loader/private/agent/imp/DataImportChunk.py.abctodo
+-rw-r--r--   0 root         (0) root         (0)    10593 2023-06-13 11:58:03.000000 peek-abstract-chunked-data-loader-3.4.2/peek_abstract_chunked_data_loader/private/agent/imp/DataImportChunks.py.abctodo
+-rw-r--r--   0 root         (0) root         (0)       20 2023-06-13 11:58:03.000000 peek-abstract-chunked-data-loader-3.4.2/peek_abstract_chunked_data_loader/private/agent/imp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 11:58:31.807890 peek-abstract-chunked-data-loader-3.4.2/peek_abstract_chunked_data_loader/private/server/
+-rw-r--r--   0 root         (0) root         (0)     4354 2023-06-13 11:58:03.000000 peek-abstract-chunked-data-loader-3.4.2/peek_abstract_chunked_data_loader/private/server/LogicEntryHook.py.abctodo
+-rw-r--r--   0 root         (0) root         (0)      604 2023-06-13 11:58:03.000000 peek-abstract-chunked-data-loader-3.4.2/peek_abstract_chunked_data_loader/private/server/TupleActionProcessor.py.abctodo
+-rw-r--r--   0 root         (0) root         (0)     1425 2023-06-13 11:58:03.000000 peek-abstract-chunked-data-loader-3.4.2/peek_abstract_chunked_data_loader/private/server/TupleDataObservable.py.abctodo
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 11:58:03.000000 peek-abstract-chunked-data-loader-3.4.2/peek_abstract_chunked_data_loader/private/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 11:58:31.807890 peek-abstract-chunked-data-loader-3.4.2/peek_abstract_chunked_data_loader/private/server/admin_backend/
+-rw-r--r--   0 root         (0) root         (0)     1292 2023-06-13 11:58:03.000000 peek-abstract-chunked-data-loader-3.4.2/peek_abstract_chunked_data_loader/private/server/admin_backend/AppSettingHandler.py.abctodo
+-rw-r--r--   0 root         (0) root         (0)     1044 2023-06-13 11:58:03.000000 peek-abstract-chunked-data-loader-3.4.2/peek_abstract_chunked_data_loader/private/server/admin_backend/SettingPropertyHandler.py.abctodo
+-rw-r--r--   0 root         (0) root         (0)      969 2023-06-13 11:58:03.000000 peek-abstract-chunked-data-loader-3.4.2/peek_abstract_chunked_data_loader/private/server/admin_backend/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 11:58:31.808889 peek-abstract-chunked-data-loader-3.4.2/peek_abstract_chunked_data_loader/private/server/agent_handlers/
+-rw-r--r--   0 root         (0) root         (0)     2005 2023-06-13 11:58:03.000000 peek-abstract-chunked-data-loader-3.4.2/peek_abstract_chunked_data_loader/private/server/agent_handlers/ACDLRpcForAgentImportABC.py
+-rw-r--r--   0 root         (0) root         (0)     3675 2023-06-13 11:58:03.000000 peek-abstract-chunked-data-loader-3.4.2/peek_abstract_chunked_data_loader/private/server/agent_handlers/ADLRpcForAgentABC.py.abctodo
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 11:58:03.000000 peek-abstract-chunked-data-loader-3.4.2/peek_abstract_chunked_data_loader/private/server/agent_handlers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 11:58:31.808889 peek-abstract-chunked-data-loader-3.4.2/peek_abstract_chunked_data_loader/private/server/controller/
+-rw-r--r--   0 root         (0) root         (0)     1009 2023-06-13 11:58:03.000000 peek-abstract-chunked-data-loader-3.4.2/peek_abstract_chunked_data_loader/private/server/controller/MainController.py.abctodo
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 11:58:03.000000 peek-abstract-chunked-data-loader-3.4.2/peek_abstract_chunked_data_loader/private/server/controller/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 11:58:31.808889 peek-abstract-chunked-data-loader-3.4.2/peek_abstract_chunked_data_loader/private/server/tuple_providers/
+-rw-r--r--   0 root         (0) root         (0)      928 2023-06-13 11:58:03.000000 peek-abstract-chunked-data-loader-3.4.2/peek_abstract_chunked_data_loader/private/server/tuple_providers/LoaderStatusTupleProvider.py.abctodo
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 11:58:03.000000 peek-abstract-chunked-data-loader-3.4.2/peek_abstract_chunked_data_loader/private/server/tuple_providers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 11:58:31.808889 peek-abstract-chunked-data-loader-3.4.2/peek_abstract_chunked_data_loader/private/tuples/
+-rw-r--r--   0 root         (0) root         (0)     1357 2023-06-13 11:58:03.000000 peek-abstract-chunked-data-loader-3.4.2/peek_abstract_chunked_data_loader/private/tuples/ACDLChunkLoadStateTupleABC.py
+-rw-r--r--   0 root         (0) root         (0)      779 2023-06-13 11:58:03.000000 peek-abstract-chunked-data-loader-3.4.2/peek_abstract_chunked_data_loader/private/tuples/AppServerSettingsTuple.py.abctodo
+-rw-r--r--   0 root         (0) root         (0)      485 2023-06-13 11:58:03.000000 peek-abstract-chunked-data-loader-3.4.2/peek_abstract_chunked_data_loader/private/tuples/LoaderStatusTuple.py.abctodo
+-rw-r--r--   0 root         (0) root         (0)      348 2023-06-13 11:58:03.000000 peek-abstract-chunked-data-loader-3.4.2/peek_abstract_chunked_data_loader/private/tuples/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 11:58:31.806889 peek-abstract-chunked-data-loader-3.4.2/peek_abstract_chunked_data_loader.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      453 2023-06-13 11:58:31.000000 peek-abstract-chunked-data-loader-3.4.2/peek_abstract_chunked_data_loader.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3455 2023-06-13 11:58:31.000000 peek-abstract-chunked-data-loader-3.4.2/peek_abstract_chunked_data_loader.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 11:58:31.000000 peek-abstract-chunked-data-loader-3.4.2/peek_abstract_chunked_data_loader.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-06-13 11:58:31.000000 peek-abstract-chunked-data-loader-3.4.2/peek_abstract_chunked_data_loader.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       34 2023-06-13 11:58:31.000000 peek-abstract-chunked-data-loader-3.4.2/peek_abstract_chunked_data_loader.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-13 11:58:31.808889 peek-abstract-chunked-data-loader-3.4.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2521 2023-06-13 11:58:31.000000 peek-abstract-chunked-data-loader-3.4.2/setup.py
```

### Comparing `peek-abstract-chunked-data-loader-3.4.1/peek_abstract_chunked_data_loader/__init__.py` & `peek-abstract-chunked-data-loader-3.4.2/peek_abstract_chunked_data_loader/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from peek_plugin_base.server.PluginLogicEntryHookABC import PluginLogicEntryHookABC
 from peek_plugin_base.client.PluginClientEntryHookABC import PluginClientEntryHookABC
 from peek_plugin_base.agent.PluginAgentEntryHookABC import PluginAgentEntryHookABC
 from typing import Type
 
-__version__ = '3.4.1'
+__version__ = '3.4.2'
 
 
 def peekLogicEntryHook() -> Type[PluginLogicEntryHookABC]:
     from .private.server.LogicEntryHook import LogicEntryHook
 
     return LogicEntryHook
```

### Comparing `peek-abstract-chunked-data-loader-3.4.1/peek_abstract_chunked_data_loader/private/admin-app.abctodo/abstracDataLoader.component.html` & `peek-abstract-chunked-data-loader-3.4.2/peek_abstract_chunked_data_loader/private/admin-app.abctodo/abstracDataLoader.component.html`

 * *Files identical despite different names*

### Comparing `peek-abstract-chunked-data-loader-3.4.1/peek_abstract_chunked_data_loader/private/admin-app.abctodo/edit-setting-table/edit.component.html` & `peek-abstract-chunked-data-loader-3.4.2/peek_abstract_chunked_data_loader/private/admin-app.abctodo/edit-setting-table/edit.component.html`

 * *Files identical despite different names*

### Comparing `peek-abstract-chunked-data-loader-3.4.1/peek_abstract_chunked_data_loader/private/admin-app.abctodo/edit-setting-table/edit.component.ts` & `peek-abstract-chunked-data-loader-3.4.2/peek_abstract_chunked_data_loader/private/admin-app.abctodo/edit-setting-table/edit.component.ts`

 * *Files identical despite different names*

### Comparing `peek-abstract-chunked-data-loader-3.4.1/peek_abstract_chunked_data_loader/private/admin-app.abctodo/edit-source-settings/edit.component.html` & `peek-abstract-chunked-data-loader-3.4.2/peek_abstract_chunked_data_loader/private/admin-app.abctodo/edit-source-settings/edit.component.html`

 * *Files identical despite different names*

### Comparing `peek-abstract-chunked-data-loader-3.4.1/peek_abstract_chunked_data_loader/private/admin-app.abctodo/edit-source-settings/edit.component.ts` & `peek-abstract-chunked-data-loader-3.4.2/peek_abstract_chunked_data_loader/private/admin-app.abctodo/edit-source-settings/edit.component.ts`

 * *Files identical despite different names*

### Comparing `peek-abstract-chunked-data-loader-3.4.1/peek_abstract_chunked_data_loader/private/admin-app.abctodo/status/status.component.ts` & `peek-abstract-chunked-data-loader-3.4.2/peek_abstract_chunked_data_loader/private/admin-app.abctodo/status/status.component.ts`

 * *Files identical despite different names*

### Comparing `peek-abstract-chunked-data-loader-3.4.1/peek_abstract_chunked_data_loader/private/admin-app.abctodo/tuples/AppServerSettingsTuple.ts` & `peek-abstract-chunked-data-loader-3.4.2/peek_abstract_chunked_data_loader/private/admin-app.abctodo/tuples/AppServerSettingsTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-abstract-chunked-data-loader-3.4.1/peek_abstract_chunked_data_loader/private/admin-app.abctodo/tuples/SettingPropertyTuple.ts` & `peek-abstract-chunked-data-loader-3.4.2/peek_abstract_chunked_data_loader/private/admin-app.abctodo/tuples/SettingPropertyTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-abstract-chunked-data-loader-3.4.1/peek_abstract_chunked_data_loader/private/agent/AgentController.py.abctodo` & `peek-abstract-chunked-data-loader-3.4.2/peek_abstract_chunked_data_loader/private/agent/AgentController.py.abctodo`

 * *Files identical despite different names*

### Comparing `peek-abstract-chunked-data-loader-3.4.1/peek_abstract_chunked_data_loader/private/agent/AgentEntryHook.py.abctodo` & `peek-abstract-chunked-data-loader-3.4.2/peek_abstract_chunked_data_loader/private/agent/AgentEntryHook.py.abctodo`

 * *Files identical despite different names*

### Comparing `peek-abstract-chunked-data-loader-3.4.1/peek_abstract_chunked_data_loader/private/agent/imp/DataImportChunk.py.abctodo` & `peek-abstract-chunked-data-loader-3.4.2/peek_abstract_chunked_data_loader/private/agent/imp/DataImportChunk.py.abctodo`

 * *Files identical despite different names*

### Comparing `peek-abstract-chunked-data-loader-3.4.1/peek_abstract_chunked_data_loader/private/agent/imp/DataImportChunks.py.abctodo` & `peek-abstract-chunked-data-loader-3.4.2/peek_abstract_chunked_data_loader/private/agent/imp/DataImportChunks.py.abctodo`

 * *Files identical despite different names*

### Comparing `peek-abstract-chunked-data-loader-3.4.1/peek_abstract_chunked_data_loader/private/server/LogicEntryHook.py.abctodo` & `peek-abstract-chunked-data-loader-3.4.2/peek_abstract_chunked_data_loader/private/server/LogicEntryHook.py.abctodo`

 * *Files identical despite different names*

### Comparing `peek-abstract-chunked-data-loader-3.4.1/peek_abstract_chunked_data_loader/private/server/TupleActionProcessor.py.abctodo` & `peek-abstract-chunked-data-loader-3.4.2/peek_abstract_chunked_data_loader/private/server/TupleActionProcessor.py.abctodo`

 * *Files identical despite different names*

### Comparing `peek-abstract-chunked-data-loader-3.4.1/peek_abstract_chunked_data_loader/private/server/TupleDataObservable.py.abctodo` & `peek-abstract-chunked-data-loader-3.4.2/peek_abstract_chunked_data_loader/private/server/TupleDataObservable.py.abctodo`

 * *Files identical despite different names*

### Comparing `peek-abstract-chunked-data-loader-3.4.1/peek_abstract_chunked_data_loader/private/server/admin_backend/AppSettingHandler.py.abctodo` & `peek-abstract-chunked-data-loader-3.4.2/peek_abstract_chunked_data_loader/private/server/admin_backend/AppSettingHandler.py.abctodo`

 * *Files identical despite different names*

### Comparing `peek-abstract-chunked-data-loader-3.4.1/peek_abstract_chunked_data_loader/private/server/admin_backend/SettingPropertyHandler.py.abctodo` & `peek-abstract-chunked-data-loader-3.4.2/peek_abstract_chunked_data_loader/private/server/admin_backend/SettingPropertyHandler.py.abctodo`

 * *Files identical despite different names*

### Comparing `peek-abstract-chunked-data-loader-3.4.1/peek_abstract_chunked_data_loader/private/server/admin_backend/__init__.py` & `peek-abstract-chunked-data-loader-3.4.2/peek_abstract_chunked_data_loader/private/server/admin_backend/__init__.py`

 * *Files identical despite different names*

### Comparing `peek-abstract-chunked-data-loader-3.4.1/peek_abstract_chunked_data_loader/private/server/agent_handlers/ACDLRpcForAgentImportABC.py` & `peek-abstract-chunked-data-loader-3.4.2/peek_abstract_chunked_data_loader/private/server/agent_handlers/ACDLRpcForAgentImportABC.py`

 * *Files identical despite different names*

### Comparing `peek-abstract-chunked-data-loader-3.4.1/peek_abstract_chunked_data_loader/private/server/agent_handlers/ADLRpcForAgentABC.py.abctodo` & `peek-abstract-chunked-data-loader-3.4.2/peek_abstract_chunked_data_loader/private/server/agent_handlers/ADLRpcForAgentABC.py.abctodo`

 * *Files identical despite different names*

### Comparing `peek-abstract-chunked-data-loader-3.4.1/peek_abstract_chunked_data_loader/private/server/controller/MainController.py.abctodo` & `peek-abstract-chunked-data-loader-3.4.2/peek_abstract_chunked_data_loader/private/server/controller/MainController.py.abctodo`

 * *Files identical despite different names*

### Comparing `peek-abstract-chunked-data-loader-3.4.1/peek_abstract_chunked_data_loader/private/server/tuple_providers/LoaderStatusTupleProvider.py.abctodo` & `peek-abstract-chunked-data-loader-3.4.2/peek_abstract_chunked_data_loader/private/server/tuple_providers/LoaderStatusTupleProvider.py.abctodo`

 * *Files identical despite different names*

### Comparing `peek-abstract-chunked-data-loader-3.4.1/peek_abstract_chunked_data_loader/private/tuples/ACDLChunkLoadStateTupleABC.py` & `peek-abstract-chunked-data-loader-3.4.2/peek_abstract_chunked_data_loader/private/tuples/ACDLChunkLoadStateTupleABC.py`

 * *Files identical despite different names*

### Comparing `peek-abstract-chunked-data-loader-3.4.1/peek_abstract_chunked_data_loader/private/tuples/AppServerSettingsTuple.py.abctodo` & `peek-abstract-chunked-data-loader-3.4.2/peek_abstract_chunked_data_loader/private/tuples/AppServerSettingsTuple.py.abctodo`

 * *Files identical despite different names*

### Comparing `peek-abstract-chunked-data-loader-3.4.1/peek_abstract_chunked_data_loader.egg-info/SOURCES.txt` & `peek-abstract-chunked-data-loader-3.4.2/peek_abstract_chunked_data_loader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `peek-abstract-chunked-data-loader-3.4.1/setup.py` & `peek-abstract-chunked-data-loader-3.4.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #
 # Modify these values to fork a new plugin
 #
 author = "Synerty"
 author_email = "contact@synerty.com"
 py_package_name = "peek_abstract_chunked_data_loader"
 pip_package_name = py_package_name.replace("_", "-")
-package_version = "3.4.1"
+package_version = "3.4.2"
 description = "Peek Plugin AbstractDataLoader - My first enhancement."
 
 download_url = "https://bitbucket.org/synerty/%s/get/%s.zip"
 download_url %= pip_package_name, package_version
 url = "https://bitbucket.org/synerty/%s" % pip_package_name
 
 #
```

