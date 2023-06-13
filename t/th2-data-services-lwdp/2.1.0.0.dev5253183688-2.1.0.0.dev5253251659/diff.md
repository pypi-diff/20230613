# Comparing `tmp/th2_data_services_lwdp-2.1.0.0.dev5253183688.tar.gz` & `tmp/th2_data_services_lwdp-2.1.0.0.dev5253251659.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/th2_data_services_lwdp-2.1.0.0.dev5253183688.tar", last modified: Tue Jun 13 08:40:18 2023, max compression
+gzip compressed data, was "dist/th2_data_services_lwdp-2.1.0.0.dev5253251659.tar", last modified: Tue Jun 13 08:45:45 2023, max compression
```

## Comparing `th2_data_services_lwdp-2.1.0.0.dev5253183688.tar` & `th2_data_services_lwdp-2.1.0.0.dev5253251659.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:40:18.000000 th2_data_services_lwdp-2.1.0.0.dev5253183688/
--rw-r--r--   0 runner    (1001) docker     (122)       68 2023-06-13 08:37:39.000000 th2_data_services_lwdp-2.1.0.0.dev5253183688/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     9677 2023-06-13 08:40:18.000000 th2_data_services_lwdp-2.1.0.0.dev5253183688/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     7699 2023-06-13 08:37:39.000000 th2_data_services_lwdp-2.1.0.0.dev5253183688/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       92 2023-06-13 08:40:03.000000 th2_data_services_lwdp-2.1.0.0.dev5253183688/package_info.json
--rw-r--r--   0 runner    (1001) docker     (122)      236 2023-06-13 08:37:39.000000 th2_data_services_lwdp-2.1.0.0.dev5253183688/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-13 08:40:18.000000 th2_data_services_lwdp-2.1.0.0.dev5253183688/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1658 2023-06-13 08:37:39.000000 th2_data_services_lwdp-2.1.0.0.dev5253183688/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:40:18.000000 th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:40:18.000000 th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services/data_source/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:40:18.000000 th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services/data_source/lwdp/
--rw-r--r--   0 runner    (1001) docker     (122)     1059 2023-06-13 08:37:39.000000 th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services/data_source/lwdp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:40:18.000000 th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services/data_source/lwdp/adapters/
--rw-r--r--   0 runner    (1001) docker     (122)      819 2023-06-13 08:37:39.000000 th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services/data_source/lwdp/adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2000 2023-06-13 08:37:39.000000 th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services/data_source/lwdp/adapters/adapter_sse.py
--rw-r--r--   0 runner    (1001) docker     (122)     2442 2023-06-13 08:37:39.000000 th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services/data_source/lwdp/adapters/basic_adapters.py
--rw-r--r--   0 runner    (1001) docker     (122)     2980 2023-06-13 08:37:39.000000 th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services/data_source/lwdp/adapters/event_adapters.py
--rw-r--r--   0 runner    (1001) docker     (122)     1906 2023-06-13 08:37:39.000000 th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services/data_source/lwdp/adapters/message_adapters.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:40:18.000000 th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services/data_source/lwdp/commands/
--rw-r--r--   0 runner    (1001) docker     (122)      614 2023-06-13 08:37:39.000000 th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services/data_source/lwdp/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    17907 2023-06-13 08:37:39.000000 th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services/data_source/lwdp/commands/grpc.py
--rw-r--r--   0 runner    (1001) docker     (122)    51203 2023-06-13 08:37:39.000000 th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services/data_source/lwdp/commands/http.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:40:18.000000 th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services/data_source/lwdp/data_source/
--rw-r--r--   0 runner    (1001) docker     (122)      682 2023-06-13 08:37:39.000000 th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services/data_source/lwdp/data_source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3327 2023-06-13 08:37:39.000000 th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services/data_source/lwdp/data_source/grpc.py
--rw-r--r--   0 runner    (1001) docker     (122)     3586 2023-06-13 08:37:39.000000 th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services/data_source/lwdp/data_source/http.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:40:18.000000 th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services/data_source/lwdp/event_tree/
--rw-r--r--   0 runner    (1001) docker     (122)      658 2023-06-13 08:37:39.000000 th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services/data_source/lwdp/event_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3421 2023-06-13 08:37:39.000000 th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services/data_source/lwdp/event_tree/http_etc_driver.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:40:18.000000 th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services/data_source/lwdp/filters/
--rw-r--r--   0 runner    (1001) docker     (122)      665 2023-06-13 08:37:39.000000 th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services/data_source/lwdp/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      981 2023-06-13 08:37:39.000000 th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services/data_source/lwdp/filters/event_filters.py
--rw-r--r--   0 runner    (1001) docker     (122)     3527 2023-06-13 08:37:39.000000 th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services/data_source/lwdp/filters/filter.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:40:18.000000 th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services/data_source/lwdp/interfaces/
--rw-r--r--   0 runner    (1001) docker     (122)      614 2023-06-13 08:37:39.000000 th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services/data_source/lwdp/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1443 2023-06-13 08:37:39.000000 th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services/data_source/lwdp/interfaces/command.py
--rw-r--r--   0 runner    (1001) docker     (122)     5056 2023-06-13 08:37:39.000000 th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services/data_source/lwdp/interfaces/data_source.py
--rw-r--r--   0 runner    (1001) docker     (122)      670 2023-06-13 08:37:39.000000 th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services/data_source/lwdp/interfaces/filter.py
--rw-r--r--   0 runner    (1001) docker     (122)     1000 2023-06-13 08:37:39.000000 th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services/data_source/lwdp/interfaces/source_api.py
--rw-r--r--   0 runner    (1001) docker     (122)      722 2023-06-13 08:37:39.000000 th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services/data_source/lwdp/message_response_format.py
--rw-r--r--   0 runner    (1001) docker     (122)     1733 2023-06-13 08:37:39.000000 th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services/data_source/lwdp/page.py
--rw-r--r--   0 runner    (1001) docker     (122)     3593 2023-06-13 08:37:39.000000 th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services/data_source/lwdp/resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:40:18.000000 th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services/data_source/lwdp/source_api/
--rw-r--r--   0 runner    (1001) docker     (122)      669 2023-06-13 08:37:39.000000 th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services/data_source/lwdp/source_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    16862 2023-06-13 08:37:39.000000 th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services/data_source/lwdp/source_api/grpc.py
--rw-r--r--   0 runner    (1001) docker     (122)    14333 2023-06-13 08:37:39.000000 th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services/data_source/lwdp/source_api/http.py
--rw-r--r--   0 runner    (1001) docker     (122)     4687 2023-06-13 08:37:39.000000 th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services/data_source/lwdp/streams.py
--rw-r--r--   0 runner    (1001) docker     (122)     2995 2023-06-13 08:37:39.000000 th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services/data_source/lwdp/struct.py
--rw-r--r--   0 runner    (1001) docker     (122)     4571 2023-06-13 08:37:39.000000 th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services/data_source/lwdp/stub_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:40:18.000000 th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services/data_source/lwdp/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      697 2023-06-13 08:37:39.000000 th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services/data_source/lwdp/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1438 2023-06-13 08:37:39.000000 th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services/data_source/lwdp/utils/_misc.py
--rw-r--r--   0 runner    (1001) docker     (122)     1504 2023-06-13 08:37:39.000000 th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services/data_source/lwdp/utils/_response_formats.py
--rw-r--r--   0 runner    (1001) docker     (122)     2441 2023-06-13 08:37:39.000000 th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services/data_source/lwdp/utils/json.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:40:18.000000 th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services_lwdp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     9677 2023-06-13 08:40:17.000000 th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services_lwdp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2230 2023-06-13 08:40:18.000000 th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services_lwdp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-13 08:40:17.000000 th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services_lwdp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       42 2023-06-13 08:40:17.000000 th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services_lwdp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-13 08:40:17.000000 th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services_lwdp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:45:45.000000 th2_data_services_lwdp-2.1.0.0.dev5253251659/
+-rw-r--r--   0 runner    (1001) docker     (122)       68 2023-06-13 08:43:55.000000 th2_data_services_lwdp-2.1.0.0.dev5253251659/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     9677 2023-06-13 08:45:45.000000 th2_data_services_lwdp-2.1.0.0.dev5253251659/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     7699 2023-06-13 08:43:55.000000 th2_data_services_lwdp-2.1.0.0.dev5253251659/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       92 2023-06-13 08:45:31.000000 th2_data_services_lwdp-2.1.0.0.dev5253251659/package_info.json
+-rw-r--r--   0 runner    (1001) docker     (122)      236 2023-06-13 08:43:55.000000 th2_data_services_lwdp-2.1.0.0.dev5253251659/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-13 08:45:45.000000 th2_data_services_lwdp-2.1.0.0.dev5253251659/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1658 2023-06-13 08:43:55.000000 th2_data_services_lwdp-2.1.0.0.dev5253251659/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:45:45.000000 th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:45:45.000000 th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services/data_source/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:45:45.000000 th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services/data_source/lwdp/
+-rw-r--r--   0 runner    (1001) docker     (122)     1059 2023-06-13 08:43:55.000000 th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services/data_source/lwdp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:45:45.000000 th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services/data_source/lwdp/adapters/
+-rw-r--r--   0 runner    (1001) docker     (122)      819 2023-06-13 08:43:55.000000 th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services/data_source/lwdp/adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2000 2023-06-13 08:43:55.000000 th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services/data_source/lwdp/adapters/adapter_sse.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2442 2023-06-13 08:43:55.000000 th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services/data_source/lwdp/adapters/basic_adapters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2980 2023-06-13 08:43:55.000000 th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services/data_source/lwdp/adapters/event_adapters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1906 2023-06-13 08:43:55.000000 th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services/data_source/lwdp/adapters/message_adapters.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:45:45.000000 th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services/data_source/lwdp/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)      614 2023-06-13 08:43:55.000000 th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services/data_source/lwdp/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17907 2023-06-13 08:43:55.000000 th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services/data_source/lwdp/commands/grpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)    51359 2023-06-13 08:43:55.000000 th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services/data_source/lwdp/commands/http.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:45:45.000000 th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services/data_source/lwdp/data_source/
+-rw-r--r--   0 runner    (1001) docker     (122)      682 2023-06-13 08:43:55.000000 th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services/data_source/lwdp/data_source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3327 2023-06-13 08:43:55.000000 th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services/data_source/lwdp/data_source/grpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3586 2023-06-13 08:43:55.000000 th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services/data_source/lwdp/data_source/http.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:45:45.000000 th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services/data_source/lwdp/event_tree/
+-rw-r--r--   0 runner    (1001) docker     (122)      658 2023-06-13 08:43:55.000000 th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services/data_source/lwdp/event_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3421 2023-06-13 08:43:55.000000 th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services/data_source/lwdp/event_tree/http_etc_driver.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:45:45.000000 th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services/data_source/lwdp/filters/
+-rw-r--r--   0 runner    (1001) docker     (122)      665 2023-06-13 08:43:55.000000 th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services/data_source/lwdp/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      981 2023-06-13 08:43:55.000000 th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services/data_source/lwdp/filters/event_filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3527 2023-06-13 08:43:55.000000 th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services/data_source/lwdp/filters/filter.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:45:45.000000 th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services/data_source/lwdp/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (122)      614 2023-06-13 08:43:55.000000 th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services/data_source/lwdp/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1443 2023-06-13 08:43:55.000000 th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services/data_source/lwdp/interfaces/command.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5056 2023-06-13 08:43:55.000000 th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services/data_source/lwdp/interfaces/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (122)      670 2023-06-13 08:43:55.000000 th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services/data_source/lwdp/interfaces/filter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1000 2023-06-13 08:43:55.000000 th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services/data_source/lwdp/interfaces/source_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      722 2023-06-13 08:43:55.000000 th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services/data_source/lwdp/message_response_format.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1733 2023-06-13 08:43:55.000000 th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services/data_source/lwdp/page.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3593 2023-06-13 08:43:55.000000 th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services/data_source/lwdp/resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:45:45.000000 th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services/data_source/lwdp/source_api/
+-rw-r--r--   0 runner    (1001) docker     (122)      669 2023-06-13 08:43:55.000000 th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services/data_source/lwdp/source_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16862 2023-06-13 08:43:55.000000 th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services/data_source/lwdp/source_api/grpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14333 2023-06-13 08:43:55.000000 th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services/data_source/lwdp/source_api/http.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4687 2023-06-13 08:43:55.000000 th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services/data_source/lwdp/streams.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2995 2023-06-13 08:43:55.000000 th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services/data_source/lwdp/struct.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4571 2023-06-13 08:43:55.000000 th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services/data_source/lwdp/stub_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:45:45.000000 th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services/data_source/lwdp/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      697 2023-06-13 08:43:55.000000 th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services/data_source/lwdp/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1438 2023-06-13 08:43:55.000000 th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services/data_source/lwdp/utils/_misc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1504 2023-06-13 08:43:55.000000 th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services/data_source/lwdp/utils/_response_formats.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2441 2023-06-13 08:43:55.000000 th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services/data_source/lwdp/utils/json.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:45:45.000000 th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services_lwdp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     9677 2023-06-13 08:45:45.000000 th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services_lwdp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2230 2023-06-13 08:45:45.000000 th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services_lwdp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-13 08:45:45.000000 th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services_lwdp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       42 2023-06-13 08:45:45.000000 th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services_lwdp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-13 08:45:45.000000 th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services_lwdp.egg-info/top_level.txt
```

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5253183688/PKG-INFO` & `th2_data_services_lwdp-2.1.0.0.dev5253251659/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: th2_data_services_lwdp
-Version: 2.1.0.0.dev5253183688
+Version: 2.1.0.0.dev5253251659
 Summary: th2_data_services_lwdp
 Home-page: https://github.com/th2-net/th2-ds-source-lwdp
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
 Description: # Lightweight Data Provider Data Source (major version 2).
         # Introduction
```

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5253183688/README.md` & `th2_data_services_lwdp-2.1.0.0.dev5253251659/README.md`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5253183688/setup.py` & `th2_data_services_lwdp-2.1.0.0.dev5253251659/setup.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services/data_source/lwdp/__init__.py` & `th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services/data_source/lwdp/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services/data_source/lwdp/adapters/__init__.py` & `th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services/data_source/lwdp/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services/data_source/lwdp/adapters/adapter_sse.py` & `th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services/data_source/lwdp/adapters/adapter_sse.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services/data_source/lwdp/adapters/basic_adapters.py` & `th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services/data_source/lwdp/adapters/basic_adapters.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services/data_source/lwdp/adapters/event_adapters.py` & `th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services/data_source/lwdp/adapters/event_adapters.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services/data_source/lwdp/adapters/message_adapters.py` & `th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services/data_source/lwdp/adapters/message_adapters.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services/data_source/lwdp/commands/__init__.py` & `th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services/data_source/lwdp/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services/data_source/lwdp/commands/grpc.py` & `th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services/data_source/lwdp/commands/grpc.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services/data_source/lwdp/commands/http.py` & `th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services/data_source/lwdp/commands/http.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,29 +168,31 @@
     """
 
     def __init__(
         self,
         book_id: str,
         start_timestamp: datetime = None,
         end_timestamp: datetime = None,
-        buffer_limit: int = DEFAULT_BUFFER_LIMIT,
         cache: bool = False,
+        char_enc: str = "utf-8",
+        decode_error_handler: str = UNICODE_REPLACE_HANDLER,
+        buffer_limit: int = DEFAULT_BUFFER_LIMIT,
     ) -> None:
         """GetEventScopes Constructor.
 
         If start_timestamp and end_timestamp are not provided, it returns all aliases.
 
         Args:
             book_id (str): Book ID.
             start_timestamp (datetime): Start Timestamp.
             end_timestamp (datetime): End Timestamp.
             cache (Optional, bool): Cache Status. Defaults To `False`.
             buffer_limit: SSEAdapter BufferedJSONProcessor buffer limit.
         """
-        super().__init__(cache, buffer_limit=buffer_limit)
+        super().__init__(cache, buffer_limit=buffer_limit, char_enc=char_enc, decode_error_handler=decode_error_handler)
         if all(timestamp is None for timestamp in (start_timestamp, end_timestamp)):
             self._all_results = True
         else:
             _check_datetime(start_timestamp)
             _check_datetime(end_timestamp)
             self._start_timestamp = DatetimeConverter.to_nanoseconds(start_timestamp)
             self._end_timestamp = DatetimeConverter.to_nanoseconds(end_timestamp)
```

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services/data_source/lwdp/data_source/__init__.py` & `th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services/data_source/lwdp/data_source/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services/data_source/lwdp/data_source/grpc.py` & `th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services/data_source/lwdp/data_source/grpc.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services/data_source/lwdp/data_source/http.py` & `th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services/data_source/lwdp/data_source/http.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services/data_source/lwdp/event_tree/__init__.py` & `th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services/data_source/lwdp/event_tree/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services/data_source/lwdp/event_tree/http_etc_driver.py` & `th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services/data_source/lwdp/event_tree/http_etc_driver.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services/data_source/lwdp/filters/__init__.py` & `th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services/data_source/lwdp/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services/data_source/lwdp/filters/event_filters.py` & `th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services/data_source/lwdp/filters/event_filters.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services/data_source/lwdp/filters/filter.py` & `th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services/data_source/lwdp/filters/filter.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services/data_source/lwdp/interfaces/__init__.py` & `th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services/data_source/lwdp/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services/data_source/lwdp/interfaces/command.py` & `th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services/data_source/lwdp/interfaces/command.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services/data_source/lwdp/interfaces/data_source.py` & `th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services/data_source/lwdp/interfaces/data_source.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services/data_source/lwdp/interfaces/filter.py` & `th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services/data_source/lwdp/interfaces/filter.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services/data_source/lwdp/interfaces/source_api.py` & `th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services/data_source/lwdp/interfaces/source_api.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services/data_source/lwdp/message_response_format.py` & `th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services/data_source/lwdp/message_response_format.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services/data_source/lwdp/page.py` & `th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services/data_source/lwdp/page.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services/data_source/lwdp/resolver.py` & `th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services/data_source/lwdp/resolver.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services/data_source/lwdp/source_api/__init__.py` & `th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services/data_source/lwdp/source_api/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services/data_source/lwdp/source_api/grpc.py` & `th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services/data_source/lwdp/source_api/grpc.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services/data_source/lwdp/source_api/http.py` & `th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services/data_source/lwdp/source_api/http.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services/data_source/lwdp/streams.py` & `th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services/data_source/lwdp/streams.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services/data_source/lwdp/struct.py` & `th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services/data_source/lwdp/struct.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services/data_source/lwdp/stub_builder.py` & `th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services/data_source/lwdp/stub_builder.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services/data_source/lwdp/utils/__init__.py` & `th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services/data_source/lwdp/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services/data_source/lwdp/utils/_misc.py` & `th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services/data_source/lwdp/utils/_misc.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services/data_source/lwdp/utils/_response_formats.py` & `th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services/data_source/lwdp/utils/_response_formats.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services/data_source/lwdp/utils/json.py` & `th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services/data_source/lwdp/utils/json.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services_lwdp.egg-info/PKG-INFO` & `th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services_lwdp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: th2-data-services-lwdp
-Version: 2.1.0.0.dev5253183688
+Version: 2.1.0.0.dev5253251659
 Summary: th2_data_services_lwdp
 Home-page: https://github.com/th2-net/th2-ds-source-lwdp
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
 Description: # Lightweight Data Provider Data Source (major version 2).
         # Introduction
```

### Comparing `th2_data_services_lwdp-2.1.0.0.dev5253183688/th2_data_services_lwdp.egg-info/SOURCES.txt` & `th2_data_services_lwdp-2.1.0.0.dev5253251659/th2_data_services_lwdp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

