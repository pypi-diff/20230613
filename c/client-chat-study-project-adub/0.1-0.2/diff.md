# Comparing `tmp/client_chat_study_project_adub-0.1.tar.gz` & `tmp/client_chat_study_project_adub-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "client_chat_study_project_adub-0.1.tar", last modified: Tue Jun 13 09:11:50 2023, max compression
+gzip compressed data, was "client_chat_study_project_adub-0.2.tar", last modified: Tue Jun 13 09:41:37 2023, max compression
```

## Comparing `client_chat_study_project_adub-0.1.tar` & `client_chat_study_project_adub-0.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 09:11:50.479341 client_chat_study_project_adub-0.1/
--rw-rw-rw-   0        0        0      157 2023-06-13 09:11:50.479341 client_chat_study_project_adub-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-13 09:11:50.468342 client_chat_study_project_adub-0.1/client_chat_study_project_adub.egg-info/
--rw-rw-rw-   0        0        0      157 2023-06-13 09:11:50.000000 client_chat_study_project_adub-0.1/client_chat_study_project_adub.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      744 2023-06-13 09:11:50.000000 client_chat_study_project_adub-0.1/client_chat_study_project_adub.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 09:11:50.000000 client_chat_study_project_adub-0.1/client_chat_study_project_adub.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-06-13 09:11:50.000000 client_chat_study_project_adub-0.1/client_chat_study_project_adub.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-06-13 09:11:50.000000 client_chat_study_project_adub-0.1/client_chat_study_project_adub.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-13 09:11:50.479341 client_chat_study_project_adub-0.1/setup.cfg
--rw-rw-rw-   0        0        0      356 2023-06-13 09:11:44.000000 client_chat_study_project_adub-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-13 09:11:50.469342 client_chat_study_project_adub-0.1/src/
--rw-rw-rw-   0        0        0        0 2023-06-12 20:44:14.000000 client_chat_study_project_adub-0.1/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 09:11:50.473342 client_chat_study_project_adub-0.1/src/client/
--rw-rw-rw-   0        0        0        0 2023-06-12 17:37:33.000000 client_chat_study_project_adub-0.1/src/client/__init__.py
--rw-rw-rw-   0        0        0     3222 2023-06-12 17:37:33.000000 client_chat_study_project_adub-0.1/src/client/add_contact.py
--rw-rw-rw-   0        0        0     8228 2023-06-12 19:41:31.000000 client_chat_study_project_adub-0.1/src/client/client_db.py
--rw-rw-rw-   0        0        0     1590 2023-06-12 17:37:33.000000 client_chat_study_project_adub-0.1/src/client/del_contact.py
--rw-rw-rw-   0        0        0    15395 2023-06-12 17:37:33.000000 client_chat_study_project_adub-0.1/src/client/main_window.py
--rw-rw-rw-   0        0        0     5577 2023-06-12 17:37:33.000000 client_chat_study_project_adub-0.1/src/client/main_window_conv.py
--rw-rw-rw-   0        0        0     1760 2023-06-12 17:37:33.000000 client_chat_study_project_adub-0.1/src/client/start_dialog.py
--rw-rw-rw-   0        0        0    12954 2023-06-12 17:37:33.000000 client_chat_study_project_adub-0.1/src/client/transport.py
--rw-rw-rw-   0        0        0     3141 2023-06-12 19:32:56.000000 client_chat_study_project_adub-0.1/src/client.py
-drwxrwxrwx   0        0        0        0 2023-06-13 09:11:50.476342 client_chat_study_project_adub-0.1/src/common/
--rw-rw-rw-   0        0        0        0 2023-06-12 17:37:33.000000 client_chat_study_project_adub-0.1/src/common/__init__.py
--rw-rw-rw-   0        0        0     1182 2023-06-12 17:37:33.000000 client_chat_study_project_adub-0.1/src/common/data_transfer.py
--rw-rw-rw-   0        0        0     2998 2023-06-12 17:37:33.000000 client_chat_study_project_adub-0.1/src/common/decorators.py
--rw-rw-rw-   0        0        0     1123 2023-06-12 19:56:09.000000 client_chat_study_project_adub-0.1/src/common/descriptors.py
--rw-rw-rw-   0        0        0      393 2023-06-12 17:37:33.000000 client_chat_study_project_adub-0.1/src/common/errors.py
--rw-rw-rw-   0        0        0     3603 2023-06-12 17:37:33.000000 client_chat_study_project_adub-0.1/src/common/metaclasses.py
-drwxrwxrwx   0        0        0        0 2023-06-13 09:11:50.478341 client_chat_study_project_adub-0.1/src/logs/
--rw-rw-rw-   0        0        0        0 2023-06-12 17:37:33.000000 client_chat_study_project_adub-0.1/src/logs/__init__.py
--rw-rw-rw-   0        0        0      656 2023-06-12 19:29:57.000000 client_chat_study_project_adub-0.1/src/logs/client_log_config.py
--rw-rw-rw-   0        0        0      924 2023-06-12 19:21:27.000000 client_chat_study_project_adub-0.1/src/logs/server_log_config.py
+drwxrwxrwx   0        0        0        0 2023-06-13 09:41:37.385693 client_chat_study_project_adub-0.2/
+-rw-rw-rw-   0        0        0      157 2023-06-13 09:41:37.384393 client_chat_study_project_adub-0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-13 09:41:37.362301 client_chat_study_project_adub-0.2/client_chat_adub/
+-rw-rw-rw-   0        0        0        0 2023-06-12 20:44:14.000000 client_chat_study_project_adub-0.2/client_chat_adub/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 09:41:37.366301 client_chat_study_project_adub-0.2/client_chat_adub/client/
+-rw-rw-rw-   0        0        0        0 2023-06-12 17:37:33.000000 client_chat_study_project_adub-0.2/client_chat_adub/client/__init__.py
+-rw-rw-rw-   0        0        0     3222 2023-06-12 17:37:33.000000 client_chat_study_project_adub-0.2/client_chat_adub/client/add_contact.py
+-rw-rw-rw-   0        0        0     8228 2023-06-12 19:41:31.000000 client_chat_study_project_adub-0.2/client_chat_adub/client/client_db.py
+-rw-rw-rw-   0        0        0     1590 2023-06-12 17:37:33.000000 client_chat_study_project_adub-0.2/client_chat_adub/client/del_contact.py
+-rw-rw-rw-   0        0        0    15395 2023-06-12 17:37:33.000000 client_chat_study_project_adub-0.2/client_chat_adub/client/main_window.py
+-rw-rw-rw-   0        0        0     5577 2023-06-12 17:37:33.000000 client_chat_study_project_adub-0.2/client_chat_adub/client/main_window_conv.py
+-rw-rw-rw-   0        0        0     1760 2023-06-12 17:37:33.000000 client_chat_study_project_adub-0.2/client_chat_adub/client/start_dialog.py
+-rw-rw-rw-   0        0        0    12954 2023-06-12 17:37:33.000000 client_chat_study_project_adub-0.2/client_chat_adub/client/transport.py
+-rw-rw-rw-   0        0        0     3141 2023-06-12 19:32:56.000000 client_chat_study_project_adub-0.2/client_chat_adub/client.py
+drwxrwxrwx   0        0        0        0 2023-06-13 09:41:37.369300 client_chat_study_project_adub-0.2/client_chat_adub/common/
+-rw-rw-rw-   0        0        0        0 2023-06-12 17:37:33.000000 client_chat_study_project_adub-0.2/client_chat_adub/common/__init__.py
+-rw-rw-rw-   0        0        0     1182 2023-06-12 17:37:33.000000 client_chat_study_project_adub-0.2/client_chat_adub/common/data_transfer.py
+-rw-rw-rw-   0        0        0     2998 2023-06-12 17:37:33.000000 client_chat_study_project_adub-0.2/client_chat_adub/common/decorators.py
+-rw-rw-rw-   0        0        0     1123 2023-06-12 19:56:09.000000 client_chat_study_project_adub-0.2/client_chat_adub/common/descriptors.py
+-rw-rw-rw-   0        0        0      393 2023-06-12 17:37:33.000000 client_chat_study_project_adub-0.2/client_chat_adub/common/errors.py
+-rw-rw-rw-   0        0        0     3603 2023-06-12 17:37:33.000000 client_chat_study_project_adub-0.2/client_chat_adub/common/metaclasses.py
+drwxrwxrwx   0        0        0        0 2023-06-13 09:41:37.371301 client_chat_study_project_adub-0.2/client_chat_adub/logs/
+-rw-rw-rw-   0        0        0        0 2023-06-12 17:37:33.000000 client_chat_study_project_adub-0.2/client_chat_adub/logs/__init__.py
+-rw-rw-rw-   0        0        0      656 2023-06-12 19:29:57.000000 client_chat_study_project_adub-0.2/client_chat_adub/logs/client_log_config.py
+-rw-rw-rw-   0        0        0      924 2023-06-12 19:21:27.000000 client_chat_study_project_adub-0.2/client_chat_adub/logs/server_log_config.py
+drwxrwxrwx   0        0        0        0 2023-06-13 09:41:37.384393 client_chat_study_project_adub-0.2/client_chat_study_project_adub.egg-info/
+-rw-rw-rw-   0        0        0      157 2023-06-13 09:41:37.000000 client_chat_study_project_adub-0.2/client_chat_study_project_adub.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      991 2023-06-13 09:41:37.000000 client_chat_study_project_adub-0.2/client_chat_study_project_adub.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 09:41:37.000000 client_chat_study_project_adub-0.2/client_chat_study_project_adub.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2023-06-13 09:41:37.000000 client_chat_study_project_adub-0.2/client_chat_study_project_adub.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-06-13 09:41:37.000000 client_chat_study_project_adub-0.2/client_chat_study_project_adub.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-13 09:41:37.385693 client_chat_study_project_adub-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      356 2023-06-13 09:41:14.000000 client_chat_study_project_adub-0.2/setup.py
```

### Comparing `client_chat_study_project_adub-0.1/src/client/add_contact.py` & `client_chat_study_project_adub-0.2/client_chat_adub/client/add_contact.py`

 * *Files identical despite different names*

### Comparing `client_chat_study_project_adub-0.1/src/client/client_db.py` & `client_chat_study_project_adub-0.2/client_chat_adub/client/client_db.py`

 * *Files identical despite different names*

### Comparing `client_chat_study_project_adub-0.1/src/client/del_contact.py` & `client_chat_study_project_adub-0.2/client_chat_adub/client/del_contact.py`

 * *Files identical despite different names*

### Comparing `client_chat_study_project_adub-0.1/src/client/main_window.py` & `client_chat_study_project_adub-0.2/client_chat_adub/client/main_window.py`

 * *Files identical despite different names*

### Comparing `client_chat_study_project_adub-0.1/src/client/main_window_conv.py` & `client_chat_study_project_adub-0.2/client_chat_adub/client/main_window_conv.py`

 * *Files identical despite different names*

### Comparing `client_chat_study_project_adub-0.1/src/client/start_dialog.py` & `client_chat_study_project_adub-0.2/client_chat_adub/client/start_dialog.py`

 * *Files identical despite different names*

### Comparing `client_chat_study_project_adub-0.1/src/client/transport.py` & `client_chat_study_project_adub-0.2/client_chat_adub/client/transport.py`

 * *Files identical despite different names*

### Comparing `client_chat_study_project_adub-0.1/src/client.py` & `client_chat_study_project_adub-0.2/client_chat_adub/client.py`

 * *Files identical despite different names*

### Comparing `client_chat_study_project_adub-0.1/src/common/data_transfer.py` & `client_chat_study_project_adub-0.2/client_chat_adub/common/data_transfer.py`

 * *Files identical despite different names*

### Comparing `client_chat_study_project_adub-0.1/src/common/decorators.py` & `client_chat_study_project_adub-0.2/client_chat_adub/common/decorators.py`

 * *Files identical despite different names*

### Comparing `client_chat_study_project_adub-0.1/src/common/descriptors.py` & `client_chat_study_project_adub-0.2/client_chat_adub/common/descriptors.py`

 * *Files identical despite different names*

### Comparing `client_chat_study_project_adub-0.1/src/common/metaclasses.py` & `client_chat_study_project_adub-0.2/client_chat_adub/common/metaclasses.py`

 * *Files identical despite different names*

### Comparing `client_chat_study_project_adub-0.1/src/logs/client_log_config.py` & `client_chat_study_project_adub-0.2/client_chat_adub/logs/client_log_config.py`

 * *Files identical despite different names*

### Comparing `client_chat_study_project_adub-0.1/src/logs/server_log_config.py` & `client_chat_study_project_adub-0.2/client_chat_adub/logs/server_log_config.py`

 * *Files identical despite different names*

