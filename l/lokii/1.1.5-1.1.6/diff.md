# Comparing `tmp/lokii-1.1.5.tar.gz` & `tmp/lokii-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lokii-1.1.5.tar", last modified: Mon Jun  5 15:37:12 2023, max compression
+gzip compressed data, was "lokii-1.1.6.tar", last modified: Tue Jun 13 06:28:19 2023, max compression
```

## Comparing `lokii-1.1.5.tar` & `lokii-1.1.6.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-05 15:37:12.910365 lokii-1.1.5/
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     1083 2023-05-26 20:12:04.000000 lokii-1.1.5/LICENSE
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     6557 2023-06-05 15:37:12.910365 lokii-1.1.5/PKG-INFO
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     5434 2023-06-02 08:01:36.000000 lokii-1.1.5/README.md
-drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-05 15:37:12.902366 lokii-1.1.5/lokii/
--rw-rw-r--   0 doruk     (1000) doruk     (1000)       77 2023-06-05 15:37:06.000000 lokii-1.1.5/lokii/__init__.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)       78 2023-05-26 20:12:04.000000 lokii-1.1.5/lokii/__main__.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     3176 2023-06-02 08:01:36.000000 lokii-1.1.5/lokii/cli.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     2142 2023-06-04 11:01:51.000000 lokii-1.1.5/lokii/config.py
-drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-05 15:37:12.902366 lokii-1.1.5/lokii/exec/
--rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.1.5/lokii/exec/__init__.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     2620 2023-05-31 14:39:03.000000 lokii-1.1.5/lokii/exec/node_executor.py
-drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-05 15:37:12.906365 lokii-1.1.5/lokii/logger/
--rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.1.5/lokii/logger/__init__.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     1268 2023-06-02 08:52:49.000000 lokii-1.1.5/lokii/logger/color.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     1756 2023-05-26 20:12:04.000000 lokii-1.1.5/lokii/logger/context.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)      877 2023-06-03 07:10:34.000000 lokii-1.1.5/lokii/logger/formatter.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)      639 2023-05-26 20:12:04.000000 lokii-1.1.5/lokii/logger/progress.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     7475 2023-06-04 18:47:42.000000 lokii-1.1.5/lokii/main.py
-drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-05 15:37:12.906365 lokii-1.1.5/lokii/model/
--rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.1.5/lokii/model/__init__.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)      943 2023-06-02 08:01:36.000000 lokii-1.1.5/lokii/model/group_module.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     1083 2023-05-31 14:39:03.000000 lokii-1.1.5/lokii/model/node_module.py
-drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-05 15:37:12.906365 lokii-1.1.5/lokii/parse/
--rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.1.5/lokii/parse/__init__.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)      709 2023-05-31 14:39:03.000000 lokii-1.1.5/lokii/parse/base_parser.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     3109 2023-06-03 07:18:23.000000 lokii-1.1.5/lokii/parse/group_parser.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     2928 2023-06-03 07:15:57.000000 lokii-1.1.5/lokii/parse/node_parser.py
-drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-05 15:37:12.906365 lokii-1.1.5/lokii/storage/
--rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.1.5/lokii/storage/__init__.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)      983 2023-06-02 08:01:36.000000 lokii-1.1.5/lokii/storage/batch_iterator.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     5065 2023-06-05 15:36:58.000000 lokii-1.1.5/lokii/storage/data_storage.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)      888 2023-06-05 15:28:47.000000 lokii-1.1.5/lokii/storage/temp_storage.py
-drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-05 15:37:12.906365 lokii-1.1.5/lokii/util/
--rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.1.5/lokii/util/__init__.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     2160 2023-05-31 14:39:03.000000 lokii-1.1.5/lokii/util/graph_analyzer.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     1464 2023-05-31 14:39:03.000000 lokii-1.1.5/lokii/util/module_file_loader.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)      610 2023-05-26 20:12:04.000000 lokii-1.1.5/lokii/util/perf_timer_context.py
-drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-05 15:37:12.902366 lokii-1.1.5/lokii.egg-info/
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     6557 2023-06-05 15:37:12.000000 lokii-1.1.5/lokii.egg-info/PKG-INFO
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     1341 2023-06-05 15:37:12.000000 lokii-1.1.5/lokii.egg-info/SOURCES.txt
--rw-rw-r--   0 doruk     (1000) doruk     (1000)        1 2023-06-05 15:37:12.000000 lokii-1.1.5/lokii.egg-info/dependency_links.txt
--rw-rw-r--   0 doruk     (1000) doruk     (1000)       45 2023-06-05 15:37:12.000000 lokii-1.1.5/lokii.egg-info/entry_points.txt
--rw-rw-r--   0 doruk     (1000) doruk     (1000)        1 2021-03-08 06:45:18.000000 lokii-1.1.5/lokii.egg-info/not-zip-safe
--rw-rw-r--   0 doruk     (1000) doruk     (1000)       71 2023-06-05 15:37:12.000000 lokii-1.1.5/lokii.egg-info/requires.txt
--rw-rw-r--   0 doruk     (1000) doruk     (1000)       12 2023-06-05 15:37:12.000000 lokii-1.1.5/lokii.egg-info/top_level.txt
--rw-rw-r--   0 doruk     (1000) doruk     (1000)       84 2023-06-05 15:37:12.910365 lokii-1.1.5/setup.cfg
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     1664 2023-06-04 11:07:21.000000 lokii-1.1.5/setup.py
-drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-05 15:37:12.910365 lokii-1.1.5/tests/
--rw-rw-r--   0 doruk     (1000) doruk     (1000)        1 2023-05-26 20:12:04.000000 lokii-1.1.5/tests/__init__.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     2501 2023-06-02 08:01:36.000000 lokii-1.1.5/tests/conftest.py
-drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-05 15:37:12.910365 lokii-1.1.5/tests/exec/
--rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.1.5/tests/exec/__init__.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     1098 2023-05-31 14:39:03.000000 lokii-1.1.5/tests/exec/test_node_executor.py
-drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-05 15:37:12.910365 lokii-1.1.5/tests/parse/
--rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.1.5/tests/parse/__init__.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     2230 2023-06-02 08:01:36.000000 lokii-1.1.5/tests/parse/test_group_parser.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     3165 2023-05-31 14:39:03.000000 lokii-1.1.5/tests/parse/test_node_parser.py
-drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-05 15:37:12.910365 lokii-1.1.5/tests/storage/
--rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.1.5/tests/storage/__init__.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     4195 2023-06-02 09:34:04.000000 lokii-1.1.5/tests/storage/test_data_storage.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)      369 2023-05-26 20:12:04.000000 lokii-1.1.5/tests/storage/test_temp_storage.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     3345 2023-06-03 05:56:09.000000 lokii-1.1.5/tests/test_cli.py
-drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-05 15:37:12.910365 lokii-1.1.5/tests/util/
--rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.1.5/tests/util/__init__.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)      953 2023-05-31 14:39:03.000000 lokii-1.1.5/tests/util/test_graph_analyzer.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     1007 2023-05-26 20:12:04.000000 lokii-1.1.5/tests/util/test_module_file_loader.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)      629 2023-05-26 20:12:04.000000 lokii-1.1.5/tests/util/test_perf_timer_context.py
+drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-13 06:28:19.573342 lokii-1.1.6/
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     1083 2023-05-26 20:12:04.000000 lokii-1.1.6/LICENSE
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     6557 2023-06-13 06:28:19.573342 lokii-1.1.6/PKG-INFO
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     5434 2023-06-02 08:01:36.000000 lokii-1.1.6/README.md
+drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-13 06:28:19.569342 lokii-1.1.6/lokii/
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)       77 2023-06-13 06:26:19.000000 lokii-1.1.6/lokii/__init__.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)       78 2023-05-26 20:12:04.000000 lokii-1.1.6/lokii/__main__.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     3176 2023-06-02 08:01:36.000000 lokii-1.1.6/lokii/cli.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     2706 2023-06-13 06:27:40.000000 lokii-1.1.6/lokii/config.py
+drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-13 06:28:19.569342 lokii-1.1.6/lokii/exec/
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.1.6/lokii/exec/__init__.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     2620 2023-05-31 14:39:03.000000 lokii-1.1.6/lokii/exec/node_executor.py
+drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-13 06:28:19.569342 lokii-1.1.6/lokii/logger/
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.1.6/lokii/logger/__init__.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     1268 2023-06-02 08:52:49.000000 lokii-1.1.6/lokii/logger/color.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     1756 2023-05-26 20:12:04.000000 lokii-1.1.6/lokii/logger/context.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)      877 2023-06-03 07:10:34.000000 lokii-1.1.6/lokii/logger/formatter.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)      639 2023-05-26 20:12:04.000000 lokii-1.1.6/lokii/logger/progress.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     7475 2023-06-04 18:47:42.000000 lokii-1.1.6/lokii/main.py
+drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-13 06:28:19.569342 lokii-1.1.6/lokii/model/
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.1.6/lokii/model/__init__.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)      943 2023-06-02 08:01:36.000000 lokii-1.1.6/lokii/model/group_module.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     1083 2023-05-31 14:39:03.000000 lokii-1.1.6/lokii/model/node_module.py
+drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-13 06:28:19.573342 lokii-1.1.6/lokii/parse/
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.1.6/lokii/parse/__init__.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)      709 2023-05-31 14:39:03.000000 lokii-1.1.6/lokii/parse/base_parser.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     3109 2023-06-03 07:18:23.000000 lokii-1.1.6/lokii/parse/group_parser.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     2928 2023-06-03 07:15:57.000000 lokii-1.1.6/lokii/parse/node_parser.py
+drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-13 06:28:19.573342 lokii-1.1.6/lokii/storage/
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.1.6/lokii/storage/__init__.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)      983 2023-06-02 08:01:36.000000 lokii-1.1.6/lokii/storage/batch_iterator.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     5249 2023-06-13 06:15:30.000000 lokii-1.1.6/lokii/storage/data_storage.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)      888 2023-06-05 15:28:47.000000 lokii-1.1.6/lokii/storage/temp_storage.py
+drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-13 06:28:19.573342 lokii-1.1.6/lokii/util/
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.1.6/lokii/util/__init__.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     2160 2023-05-31 14:39:03.000000 lokii-1.1.6/lokii/util/graph_analyzer.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     1464 2023-05-31 14:39:03.000000 lokii-1.1.6/lokii/util/module_file_loader.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)      610 2023-05-26 20:12:04.000000 lokii-1.1.6/lokii/util/perf_timer_context.py
+drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-13 06:28:19.569342 lokii-1.1.6/lokii.egg-info/
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     6557 2023-06-13 06:28:19.000000 lokii-1.1.6/lokii.egg-info/PKG-INFO
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     1341 2023-06-13 06:28:19.000000 lokii-1.1.6/lokii.egg-info/SOURCES.txt
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)        1 2023-06-13 06:28:19.000000 lokii-1.1.6/lokii.egg-info/dependency_links.txt
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)       45 2023-06-13 06:28:19.000000 lokii-1.1.6/lokii.egg-info/entry_points.txt
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)        1 2021-03-08 06:45:18.000000 lokii-1.1.6/lokii.egg-info/not-zip-safe
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)       71 2023-06-13 06:28:19.000000 lokii-1.1.6/lokii.egg-info/requires.txt
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)       12 2023-06-13 06:28:19.000000 lokii-1.1.6/lokii.egg-info/top_level.txt
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)       84 2023-06-13 06:28:19.577343 lokii-1.1.6/setup.cfg
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     1664 2023-06-04 11:07:21.000000 lokii-1.1.6/setup.py
+drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-13 06:28:19.573342 lokii-1.1.6/tests/
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)        1 2023-05-26 20:12:04.000000 lokii-1.1.6/tests/__init__.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     2501 2023-06-02 08:01:36.000000 lokii-1.1.6/tests/conftest.py
+drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-13 06:28:19.573342 lokii-1.1.6/tests/exec/
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.1.6/tests/exec/__init__.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     1098 2023-05-31 14:39:03.000000 lokii-1.1.6/tests/exec/test_node_executor.py
+drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-13 06:28:19.573342 lokii-1.1.6/tests/parse/
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.1.6/tests/parse/__init__.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     2230 2023-06-02 08:01:36.000000 lokii-1.1.6/tests/parse/test_group_parser.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     3165 2023-05-31 14:39:03.000000 lokii-1.1.6/tests/parse/test_node_parser.py
+drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-13 06:28:19.573342 lokii-1.1.6/tests/storage/
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.1.6/tests/storage/__init__.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     4195 2023-06-02 09:34:04.000000 lokii-1.1.6/tests/storage/test_data_storage.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)      369 2023-05-26 20:12:04.000000 lokii-1.1.6/tests/storage/test_temp_storage.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     3345 2023-06-12 16:16:23.000000 lokii-1.1.6/tests/test_cli.py
+drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-13 06:28:19.573342 lokii-1.1.6/tests/util/
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.1.6/tests/util/__init__.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)      953 2023-05-31 14:39:03.000000 lokii-1.1.6/tests/util/test_graph_analyzer.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     1007 2023-05-26 20:12:04.000000 lokii-1.1.6/tests/util/test_module_file_loader.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)      629 2023-05-26 20:12:04.000000 lokii-1.1.6/tests/util/test_perf_timer_context.py
```

### Comparing `lokii-1.1.5/LICENSE` & `lokii-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `lokii-1.1.5/PKG-INFO` & `lokii-1.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lokii
-Version: 1.1.5
+Version: 1.1.6
 Summary: Generate, Load, Develop and Test with consistent relational datasets!
 Home-page: https://github.com/dorukerenaktas/lokii
 Author: Doruk Eren Aktaş
 Author-email: dorukerenaktas@gmail.com
 License: MIT License
 Keywords: data generation,relational datasets,development environment,testing,database
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `lokii-1.1.5/README.md` & `lokii-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `lokii-1.1.5/lokii/cli.py` & `lokii-1.1.6/lokii/cli.py`

 * *Files identical despite different names*

### Comparing `lokii-1.1.5/lokii/config.py` & `lokii-1.1.6/lokii/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,14 +15,17 @@
 # -
 GEN_CONCURRENCY = environ.get("LOKII__GEN_CONCURRENCY", cpu_count())
 # -
 GEN_BATCH_SIZE = environ.get("LOKII__GEN_BATCH_SIZE", 100000)
 # -
 GEN_CHUNK_SIZE = environ.get("LOKII__GEN_CHUNK_SIZE", 200)
 
+# -
+DATA_DISABLE_OPTIMIZERS = environ.get("LOKII__DATA_DISABLE_OPTIMIZERS", "true")
+
 
 class __Config:
     class __TempConfig:
         """
         Global configuration for storing temp file paths.
         """
 
@@ -59,21 +62,36 @@
         def batch_size(self) -> int:
             return int(GEN_BATCH_SIZE)
 
         @property
         def chunk_size(self) -> int:
             return int(GEN_CHUNK_SIZE)
 
+    class __DataConfig:
+        """
+        Global configuration for storing data query information.
+        """
+
+        @property
+        def disable_optimizers(self) -> bool:
+            # prevents duckdb issue that causes error when optimizing multiple joins in query
+            # https://github.com/duckdb/duckdb/issues/5880#issuecomment-1523613623
+            return DATA_DISABLE_OPTIMIZERS == "true"
+
     @property
     def version(self):
         return lokii.__version__
 
     @property
     def temp(self):
         return self.__TempConfig()
 
     @property
     def gen(self):
         return self.__GenConfig()
 
+    @property
+    def data(self):
+        return self.__DataConfig()
+
 
 CONFIG = __Config()
```

### Comparing `lokii-1.1.5/lokii/exec/node_executor.py` & `lokii-1.1.6/lokii/exec/node_executor.py`

 * *Files identical despite different names*

### Comparing `lokii-1.1.5/lokii/logger/color.py` & `lokii-1.1.6/lokii/logger/color.py`

 * *Files identical despite different names*

### Comparing `lokii-1.1.5/lokii/logger/context.py` & `lokii-1.1.6/lokii/logger/context.py`

 * *Files identical despite different names*

### Comparing `lokii-1.1.5/lokii/logger/formatter.py` & `lokii-1.1.6/lokii/logger/formatter.py`

 * *Files identical despite different names*

### Comparing `lokii-1.1.5/lokii/logger/progress.py` & `lokii-1.1.6/lokii/logger/progress.py`

 * *Files identical despite different names*

### Comparing `lokii-1.1.5/lokii/main.py` & `lokii-1.1.6/lokii/main.py`

 * *Files identical despite different names*

### Comparing `lokii-1.1.5/lokii/model/group_module.py` & `lokii-1.1.6/lokii/model/group_module.py`

 * *Files identical despite different names*

### Comparing `lokii-1.1.5/lokii/model/node_module.py` & `lokii-1.1.6/lokii/model/node_module.py`

 * *Files identical despite different names*

### Comparing `lokii-1.1.5/lokii/parse/base_parser.py` & `lokii-1.1.6/lokii/parse/base_parser.py`

 * *Files identical despite different names*

### Comparing `lokii-1.1.5/lokii/parse/group_parser.py` & `lokii-1.1.6/lokii/parse/group_parser.py`

 * *Files identical despite different names*

### Comparing `lokii-1.1.5/lokii/parse/node_parser.py` & `lokii-1.1.6/lokii/parse/node_parser.py`

 * *Files identical despite different names*

### Comparing `lokii-1.1.5/lokii/storage/batch_iterator.py` & `lokii-1.1.6/lokii/storage/batch_iterator.py`

 * *Files identical despite different names*

### Comparing `lokii-1.1.5/lokii/storage/data_storage.py` & `lokii-1.1.6/lokii/storage/data_storage.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,25 +27,29 @@
 
     def deps(self, query: str) -> list:
         names = duckdb.get_table_names(query)
         return list(names)
 
     def count(self, query: str) -> int:
         q = "WITH _t AS (%s) SELECT COUNT() FROM _t;" % query
+        if CONFIG.data.disable_optimizers:
+            q = "pragma disable_optimizer; " + q
         try:
             with self.connect() as conn:
                 (count,) = conn.execute(q).fetchone()
                 return count
         except duckdb.Error as err:
             logging.error("Error occurred while executing count query:\n\n%s\n" % q)
             raise err
 
     def exec(self, query: str, index: int, size: int) -> list[dict]:
         args = (query, size, index * size)
         q = "WITH _t AS (%s) SELECT * FROM _t LIMIT %d OFFSET %d;" % args
+        if CONFIG.data.disable_optimizers:
+            q = "pragma disable_optimizer; " + q
         try:
             with self.connect() as conn:
                 data = conn.execute(q).fetch_df()
                 return data.to_dict("records")
         except duckdb.Error as err:
             logging.error("Error occurred while executing source query:\n\n%s\n" % q)
             raise err
```

### Comparing `lokii-1.1.5/lokii/storage/temp_storage.py` & `lokii-1.1.6/lokii/storage/temp_storage.py`

 * *Files identical despite different names*

### Comparing `lokii-1.1.5/lokii/util/graph_analyzer.py` & `lokii-1.1.6/lokii/util/graph_analyzer.py`

 * *Files identical despite different names*

### Comparing `lokii-1.1.5/lokii/util/module_file_loader.py` & `lokii-1.1.6/lokii/util/module_file_loader.py`

 * *Files identical despite different names*

### Comparing `lokii-1.1.5/lokii/util/perf_timer_context.py` & `lokii-1.1.6/lokii/util/perf_timer_context.py`

 * *Files identical despite different names*

### Comparing `lokii-1.1.5/lokii.egg-info/PKG-INFO` & `lokii-1.1.6/lokii.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lokii
-Version: 1.1.5
+Version: 1.1.6
 Summary: Generate, Load, Develop and Test with consistent relational datasets!
 Home-page: https://github.com/dorukerenaktas/lokii
 Author: Doruk Eren Aktaş
 Author-email: dorukerenaktas@gmail.com
 License: MIT License
 Keywords: data generation,relational datasets,development environment,testing,database
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `lokii-1.1.5/lokii.egg-info/SOURCES.txt` & `lokii-1.1.6/lokii.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lokii-1.1.5/setup.py` & `lokii-1.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `lokii-1.1.5/tests/conftest.py` & `lokii-1.1.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `lokii-1.1.5/tests/exec/test_node_executor.py` & `lokii-1.1.6/tests/exec/test_node_executor.py`

 * *Files identical despite different names*

### Comparing `lokii-1.1.5/tests/parse/test_group_parser.py` & `lokii-1.1.6/tests/parse/test_group_parser.py`

 * *Files identical despite different names*

### Comparing `lokii-1.1.5/tests/parse/test_node_parser.py` & `lokii-1.1.6/tests/parse/test_node_parser.py`

 * *Files identical despite different names*

### Comparing `lokii-1.1.5/tests/storage/test_data_storage.py` & `lokii-1.1.6/tests/storage/test_data_storage.py`

 * *Files identical despite different names*

### Comparing `lokii-1.1.5/tests/test_cli.py` & `lokii-1.1.6/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `lokii-1.1.5/tests/util/test_graph_analyzer.py` & `lokii-1.1.6/tests/util/test_graph_analyzer.py`

 * *Files identical despite different names*

### Comparing `lokii-1.1.5/tests/util/test_module_file_loader.py` & `lokii-1.1.6/tests/util/test_module_file_loader.py`

 * *Files identical despite different names*

### Comparing `lokii-1.1.5/tests/util/test_perf_timer_context.py` & `lokii-1.1.6/tests/util/test_perf_timer_context.py`

 * *Files identical despite different names*

