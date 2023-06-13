# Comparing `tmp/devcycle-python-server-sdk-1.2.2.tar.gz` & `tmp/devcycle-python-server-sdk-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devcycle-python-server-sdk-1.2.2.tar", last modified: Tue May 16 18:58:26 2023, max compression
+gzip compressed data, was "devcycle-python-server-sdk-2.0.0.tar", last modified: Tue Jun 13 17:45:43 2023, max compression
```

## Comparing `devcycle-python-server-sdk-1.2.2.tar` & `devcycle-python-server-sdk-2.0.0.tar`

### file list

```diff
@@ -1,43 +1,39 @@
-drwxr-xr-x   0 jonathannorris   (501) staff       (20)        0 2023-05-16 18:58:26.084557 devcycle-python-server-sdk-1.2.2/
--rw-r--r--   0 jonathannorris   (501) staff       (20)     1071 2021-12-17 15:42:42.000000 devcycle-python-server-sdk-1.2.2/LICENSE
--rw-r--r--   0 jonathannorris   (501) staff       (20)      455 2023-05-16 18:58:26.084633 devcycle-python-server-sdk-1.2.2/PKG-INFO
--rw-r--r--   0 jonathannorris   (501) staff       (20)     1482 2023-05-16 18:57:48.000000 devcycle-python-server-sdk-1.2.2/README.md
-drwxr-xr-x   0 jonathannorris   (501) staff       (20)        0 2023-05-16 18:58:26.080422 devcycle-python-server-sdk-1.2.2/devcycle_python_sdk/
--rw-r--r--   0 jonathannorris   (501) staff       (20)        5 2023-05-16 18:58:00.000000 devcycle-python-server-sdk-1.2.2/devcycle_python_sdk/VERSION.txt
--rw-r--r--   0 jonathannorris   (501) staff       (20)     1103 2023-05-09 21:26:17.000000 devcycle-python-server-sdk-1.2.2/devcycle_python_sdk/__init__.py
-drwxr-xr-x   0 jonathannorris   (501) staff       (20)        0 2023-05-16 18:58:26.080876 devcycle-python-server-sdk-1.2.2/devcycle_python_sdk/api/
--rw-r--r--   0 jonathannorris   (501) staff       (20)      144 2021-12-17 15:42:42.000000 devcycle-python-server-sdk-1.2.2/devcycle_python_sdk/api/__init__.py
--rw-r--r--   0 jonathannorris   (501) staff       (20)    18491 2023-05-16 18:57:48.000000 devcycle-python-server-sdk-1.2.2/devcycle_python_sdk/api/dvc_client.py
--rw-r--r--   0 jonathannorris   (501) staff       (20)    24815 2021-12-17 15:42:42.000000 devcycle-python-server-sdk-1.2.2/devcycle_python_sdk/api_client.py
--rw-r--r--   0 jonathannorris   (501) staff       (20)     8288 2023-05-09 21:26:17.000000 devcycle-python-server-sdk-1.2.2/devcycle_python_sdk/configuration.py
--rw-r--r--   0 jonathannorris   (501) staff       (20)       97 2023-05-09 21:26:17.000000 devcycle-python-server-sdk-1.2.2/devcycle_python_sdk/dvc_options.py
-drwxr-xr-x   0 jonathannorris   (501) staff       (20)        0 2023-05-16 18:58:26.082282 devcycle-python-server-sdk-1.2.2/devcycle_python_sdk/models/
--rw-r--r--   0 jonathannorris   (501) staff       (20)      833 2021-12-17 15:42:42.000000 devcycle-python-server-sdk-1.2.2/devcycle_python_sdk/models/__init__.py
--rw-r--r--   0 jonathannorris   (501) staff       (20)     4015 2021-12-17 15:42:42.000000 devcycle-python-server-sdk-1.2.2/devcycle_python_sdk/models/error_response.py
--rw-r--r--   0 jonathannorris   (501) staff       (20)     6173 2021-12-17 15:42:42.000000 devcycle-python-server-sdk-1.2.2/devcycle_python_sdk/models/event.py
--rw-r--r--   0 jonathannorris   (501) staff       (20)     8501 2023-05-09 21:26:17.000000 devcycle-python-server-sdk-1.2.2/devcycle_python_sdk/models/feature.py
--rw-r--r--   0 jonathannorris   (501) staff       (20)     3137 2021-12-17 15:42:42.000000 devcycle-python-server-sdk-1.2.2/devcycle_python_sdk/models/inline_response201.py
--rw-r--r--   0 jonathannorris   (501) staff       (20)    15928 2021-12-17 15:42:42.000000 devcycle-python-server-sdk-1.2.2/devcycle_python_sdk/models/user_data.py
--rw-r--r--   0 jonathannorris   (501) staff       (20)     3801 2021-12-17 15:42:42.000000 devcycle-python-server-sdk-1.2.2/devcycle_python_sdk/models/user_data_and_events_body.py
--rw-r--r--   0 jonathannorris   (501) staff       (20)     6525 2021-12-17 15:42:42.000000 devcycle-python-server-sdk-1.2.2/devcycle_python_sdk/models/variable.py
--rw-r--r--   0 jonathannorris   (501) staff       (20)    13219 2021-12-17 15:42:42.000000 devcycle-python-server-sdk-1.2.2/devcycle_python_sdk/rest.py
-drwxr-xr-x   0 jonathannorris   (501) staff       (20)        0 2023-05-16 18:58:26.082967 devcycle-python-server-sdk-1.2.2/devcycle_python_server_sdk.egg-info/
--rw-r--r--   0 jonathannorris   (501) staff       (20)      455 2023-05-16 18:58:26.000000 devcycle-python-server-sdk-1.2.2/devcycle_python_server_sdk.egg-info/PKG-INFO
--rw-r--r--   0 jonathannorris   (501) staff       (20)     1145 2023-05-16 18:58:26.000000 devcycle-python-server-sdk-1.2.2/devcycle_python_server_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 jonathannorris   (501) staff       (20)        1 2023-05-16 18:58:26.000000 devcycle-python-server-sdk-1.2.2/devcycle_python_server_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 jonathannorris   (501) staff       (20)       48 2023-05-16 18:58:26.000000 devcycle-python-server-sdk-1.2.2/devcycle_python_server_sdk.egg-info/requires.txt
--rw-r--r--   0 jonathannorris   (501) staff       (20)       33 2023-05-16 18:58:26.000000 devcycle-python-server-sdk-1.2.2/devcycle_python_server_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 jonathannorris   (501) staff       (20)        0 2023-05-16 18:58:26.083169 devcycle-python-server-sdk-1.2.2/example/
--rw-r--r--   0 jonathannorris   (501) staff       (20)        0 2021-12-17 15:42:42.000000 devcycle-python-server-sdk-1.2.2/example/__init__.py
--rw-r--r--   0 jonathannorris   (501) staff       (20)     2506 2023-05-16 18:57:48.000000 devcycle-python-server-sdk-1.2.2/example/example.py
--rw-r--r--   0 jonathannorris   (501) staff       (20)       79 2023-05-16 18:58:26.084876 devcycle-python-server-sdk-1.2.2/setup.cfg
--rw-r--r--   0 jonathannorris   (501) staff       (20)     1320 2023-05-09 21:26:17.000000 devcycle-python-server-sdk-1.2.2/setup.py
-drwxr-xr-x   0 jonathannorris   (501) staff       (20)        0 2023-05-16 18:58:26.084416 devcycle-python-server-sdk-1.2.2/test/
--rw-r--r--   0 jonathannorris   (501) staff       (20)        0 2021-12-17 15:42:42.000000 devcycle-python-server-sdk-1.2.2/test/__init__.py
--rw-r--r--   0 jonathannorris   (501) staff       (20)     1376 2021-12-17 15:42:42.000000 devcycle-python-server-sdk-1.2.2/test/test_devcycle_api.py
--rw-r--r--   0 jonathannorris   (501) staff       (20)      965 2021-12-17 15:42:42.000000 devcycle-python-server-sdk-1.2.2/test/test_error_response.py
--rw-r--r--   0 jonathannorris   (501) staff       (20)      915 2021-12-17 15:42:42.000000 devcycle-python-server-sdk-1.2.2/test/test_feature.py
--rw-r--r--   0 jonathannorris   (501) staff       (20)      997 2021-12-17 15:42:42.000000 devcycle-python-server-sdk-1.2.2/test/test_inline_response200.py
--rw-r--r--   0 jonathannorris   (501) staff       (20)      925 2021-12-17 15:42:42.000000 devcycle-python-server-sdk-1.2.2/test/test_user_data.py
--rw-r--r--   0 jonathannorris   (501) staff       (20)     1027 2021-12-17 15:42:42.000000 devcycle-python-server-sdk-1.2.2/test/test_user_data_and_event_body.py
--rw-r--r--   0 jonathannorris   (501) staff       (20)      923 2021-12-17 15:42:42.000000 devcycle-python-server-sdk-1.2.2/test/test_variable.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-06-13 17:45:43.851686 devcycle-python-server-sdk-2.0.0/
+-rw-r--r--   0 chris      (501) staff       (20)     1071 2023-06-01 17:48:25.000000 devcycle-python-server-sdk-2.0.0/LICENSE
+-rw-r--r--   0 chris      (501) staff       (20)      277 2023-06-13 17:45:43.851748 devcycle-python-server-sdk-2.0.0/PKG-INFO
+-rw-r--r--   0 chris      (501) staff       (20)     2013 2023-06-13 17:41:34.000000 devcycle-python-server-sdk-2.0.0/README.md
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-06-13 17:45:43.848900 devcycle-python-server-sdk-2.0.0/devcycle_python_sdk/
+-rw-r--r--   0 chris      (501) staff       (20)        5 2023-06-13 17:44:48.000000 devcycle-python-server-sdk-2.0.0/devcycle_python_sdk/VERSION.txt
+-rw-r--r--   0 chris      (501) staff       (20)      186 2023-06-13 17:41:34.000000 devcycle-python-server-sdk-2.0.0/devcycle_python_sdk/__init__.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-06-13 17:45:43.849181 devcycle-python-server-sdk-2.0.0/devcycle_python_sdk/api/
+-rw-r--r--   0 chris      (501) staff       (20)        1 2023-06-13 17:41:34.000000 devcycle-python-server-sdk-2.0.0/devcycle_python_sdk/api/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)     5186 2023-06-13 17:41:34.000000 devcycle-python-server-sdk-2.0.0/devcycle_python_sdk/api/bucketing_client.py
+-rw-r--r--   0 chris      (501) staff       (20)     5637 2023-06-13 17:41:34.000000 devcycle-python-server-sdk-2.0.0/devcycle_python_sdk/dvc_cloud_client.py
+-rw-r--r--   0 chris      (501) staff       (20)      783 2023-06-13 17:41:34.000000 devcycle-python-server-sdk-2.0.0/devcycle_python_sdk/dvc_options.py
+-rw-r--r--   0 chris      (501) staff       (20)      522 2023-06-13 17:41:34.000000 devcycle-python-server-sdk-2.0.0/devcycle_python_sdk/exceptions.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-06-13 17:45:43.849898 devcycle-python-server-sdk-2.0.0/devcycle_python_sdk/models/
+-rw-r--r--   0 chris      (501) staff       (20)        0 2023-06-13 17:41:34.000000 devcycle-python-server-sdk-2.0.0/devcycle_python_sdk/models/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)      442 2023-06-13 17:41:34.000000 devcycle-python-server-sdk-2.0.0/devcycle_python_sdk/models/error_response.py
+-rw-r--r--   0 chris      (501) staff       (20)      551 2023-06-13 17:41:34.000000 devcycle-python-server-sdk-2.0.0/devcycle_python_sdk/models/event.py
+-rw-r--r--   0 chris      (501) staff       (20)      480 2023-06-13 17:41:34.000000 devcycle-python-server-sdk-2.0.0/devcycle_python_sdk/models/feature.py
+-rw-r--r--   0 chris      (501) staff       (20)     1002 2023-06-13 17:41:34.000000 devcycle-python-server-sdk-2.0.0/devcycle_python_sdk/models/user.py
+-rw-r--r--   0 chris      (501) staff       (20)     1380 2023-06-13 17:41:34.000000 devcycle-python-server-sdk-2.0.0/devcycle_python_sdk/models/variable.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-06-13 17:45:43.850155 devcycle-python-server-sdk-2.0.0/devcycle_python_sdk/util/
+-rw-r--r--   0 chris      (501) staff       (20)        1 2023-06-13 17:41:34.000000 devcycle-python-server-sdk-2.0.0/devcycle_python_sdk/util/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)      253 2023-06-13 17:41:34.000000 devcycle-python-server-sdk-2.0.0/devcycle_python_sdk/util/version.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-06-13 17:45:43.850713 devcycle-python-server-sdk-2.0.0/devcycle_python_server_sdk.egg-info/
+-rw-r--r--   0 chris      (501) staff       (20)      277 2023-06-13 17:45:43.000000 devcycle-python-server-sdk-2.0.0/devcycle_python_server_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 chris      (501) staff       (20)      980 2023-06-13 17:45:43.000000 devcycle-python-server-sdk-2.0.0/devcycle_python_server_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 chris      (501) staff       (20)        1 2023-06-13 17:45:43.000000 devcycle-python-server-sdk-2.0.0/devcycle_python_server_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 chris      (501) staff       (20)       75 2023-06-13 17:45:43.000000 devcycle-python-server-sdk-2.0.0/devcycle_python_server_sdk.egg-info/requires.txt
+-rw-r--r--   0 chris      (501) staff       (20)       33 2023-06-13 17:45:43.000000 devcycle-python-server-sdk-2.0.0/devcycle_python_server_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-06-13 17:45:43.850899 devcycle-python-server-sdk-2.0.0/example/
+-rw-r--r--   0 chris      (501) staff       (20)        0 2023-06-01 17:48:25.000000 devcycle-python-server-sdk-2.0.0/example/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)     2289 2023-06-13 17:41:34.000000 devcycle-python-server-sdk-2.0.0/example/example.py
+-rw-r--r--   0 chris      (501) staff       (20)       79 2023-06-13 17:45:43.851930 devcycle-python-server-sdk-2.0.0/setup.cfg
+-rw-r--r--   0 chris      (501) staff       (20)      853 2023-06-13 17:41:34.000000 devcycle-python-server-sdk-2.0.0/setup.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-06-13 17:45:43.851442 devcycle-python-server-sdk-2.0.0/test/
+-rw-r--r--   0 chris      (501) staff       (20)        0 2023-06-01 17:48:25.000000 devcycle-python-server-sdk-2.0.0/test/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)     7285 2023-06-13 17:41:34.000000 devcycle-python-server-sdk-2.0.0/test/test_bucketing_client.py
+-rw-r--r--   0 chris      (501) staff       (20)    11559 2023-06-13 17:41:34.000000 devcycle-python-server-sdk-2.0.0/test/test_dvc_cloud_client.py
+-rw-r--r--   0 chris      (501) staff       (20)      368 2023-06-13 17:42:32.000000 devcycle-python-server-sdk-2.0.0/test/test_version.py
```

### Comparing `devcycle-python-server-sdk-1.2.2/LICENSE` & `devcycle-python-server-sdk-2.0.0/LICENSE`

 * *Files identical despite different names*

