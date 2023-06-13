# Comparing `tmp/client_chat_study_project_adub-0.2.tar.gz` & `tmp/client_chat_study_project_adub-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "client_chat_study_project_adub-0.2.tar", last modified: Tue Jun 13 09:41:37 2023, max compression
+gzip compressed data, was "client_chat_study_project_adub-0.3.tar", last modified: Tue Jun 13 09:47:03 2023, max compression
```

## Comparing `client_chat_study_project_adub-0.2.tar` & `client_chat_study_project_adub-0.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 09:41:37.385693 client_chat_study_project_adub-0.2/
--rw-rw-rw-   0        0        0      157 2023-06-13 09:41:37.384393 client_chat_study_project_adub-0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-13 09:41:37.362301 client_chat_study_project_adub-0.2/client_chat_adub/
--rw-rw-rw-   0        0        0        0 2023-06-12 20:44:14.000000 client_chat_study_project_adub-0.2/client_chat_adub/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 09:41:37.366301 client_chat_study_project_adub-0.2/client_chat_adub/client/
--rw-rw-rw-   0        0        0        0 2023-06-12 17:37:33.000000 client_chat_study_project_adub-0.2/client_chat_adub/client/__init__.py
--rw-rw-rw-   0        0        0     3222 2023-06-12 17:37:33.000000 client_chat_study_project_adub-0.2/client_chat_adub/client/add_contact.py
--rw-rw-rw-   0        0        0     8228 2023-06-12 19:41:31.000000 client_chat_study_project_adub-0.2/client_chat_adub/client/client_db.py
--rw-rw-rw-   0        0        0     1590 2023-06-12 17:37:33.000000 client_chat_study_project_adub-0.2/client_chat_adub/client/del_contact.py
--rw-rw-rw-   0        0        0    15395 2023-06-12 17:37:33.000000 client_chat_study_project_adub-0.2/client_chat_adub/client/main_window.py
--rw-rw-rw-   0        0        0     5577 2023-06-12 17:37:33.000000 client_chat_study_project_adub-0.2/client_chat_adub/client/main_window_conv.py
--rw-rw-rw-   0        0        0     1760 2023-06-12 17:37:33.000000 client_chat_study_project_adub-0.2/client_chat_adub/client/start_dialog.py
--rw-rw-rw-   0        0        0    12954 2023-06-12 17:37:33.000000 client_chat_study_project_adub-0.2/client_chat_adub/client/transport.py
--rw-rw-rw-   0        0        0     3141 2023-06-12 19:32:56.000000 client_chat_study_project_adub-0.2/client_chat_adub/client.py
-drwxrwxrwx   0        0        0        0 2023-06-13 09:41:37.369300 client_chat_study_project_adub-0.2/client_chat_adub/common/
--rw-rw-rw-   0        0        0        0 2023-06-12 17:37:33.000000 client_chat_study_project_adub-0.2/client_chat_adub/common/__init__.py
--rw-rw-rw-   0        0        0     1182 2023-06-12 17:37:33.000000 client_chat_study_project_adub-0.2/client_chat_adub/common/data_transfer.py
--rw-rw-rw-   0        0        0     2998 2023-06-12 17:37:33.000000 client_chat_study_project_adub-0.2/client_chat_adub/common/decorators.py
--rw-rw-rw-   0        0        0     1123 2023-06-12 19:56:09.000000 client_chat_study_project_adub-0.2/client_chat_adub/common/descriptors.py
--rw-rw-rw-   0        0        0      393 2023-06-12 17:37:33.000000 client_chat_study_project_adub-0.2/client_chat_adub/common/errors.py
--rw-rw-rw-   0        0        0     3603 2023-06-12 17:37:33.000000 client_chat_study_project_adub-0.2/client_chat_adub/common/metaclasses.py
-drwxrwxrwx   0        0        0        0 2023-06-13 09:41:37.371301 client_chat_study_project_adub-0.2/client_chat_adub/logs/
--rw-rw-rw-   0        0        0        0 2023-06-12 17:37:33.000000 client_chat_study_project_adub-0.2/client_chat_adub/logs/__init__.py
--rw-rw-rw-   0        0        0      656 2023-06-12 19:29:57.000000 client_chat_study_project_adub-0.2/client_chat_adub/logs/client_log_config.py
--rw-rw-rw-   0        0        0      924 2023-06-12 19:21:27.000000 client_chat_study_project_adub-0.2/client_chat_adub/logs/server_log_config.py
-drwxrwxrwx   0        0        0        0 2023-06-13 09:41:37.384393 client_chat_study_project_adub-0.2/client_chat_study_project_adub.egg-info/
--rw-rw-rw-   0        0        0      157 2023-06-13 09:41:37.000000 client_chat_study_project_adub-0.2/client_chat_study_project_adub.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      991 2023-06-13 09:41:37.000000 client_chat_study_project_adub-0.2/client_chat_study_project_adub.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 09:41:37.000000 client_chat_study_project_adub-0.2/client_chat_study_project_adub.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-06-13 09:41:37.000000 client_chat_study_project_adub-0.2/client_chat_study_project_adub.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-06-13 09:41:37.000000 client_chat_study_project_adub-0.2/client_chat_study_project_adub.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-13 09:41:37.385693 client_chat_study_project_adub-0.2/setup.cfg
--rw-rw-rw-   0        0        0      356 2023-06-13 09:41:14.000000 client_chat_study_project_adub-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 09:47:03.114836 client_chat_study_project_adub-0.3/
+-rw-rw-rw-   0        0        0      157 2023-06-13 09:47:03.114836 client_chat_study_project_adub-0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-13 09:47:03.097851 client_chat_study_project_adub-0.3/client_chat_adub/
+-rw-rw-rw-   0        0        0        0 2023-06-12 20:44:14.000000 client_chat_study_project_adub-0.3/client_chat_adub/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 09:47:03.102167 client_chat_study_project_adub-0.3/client_chat_adub/client/
+-rw-rw-rw-   0        0        0        0 2023-06-12 17:37:33.000000 client_chat_study_project_adub-0.3/client_chat_adub/client/__init__.py
+-rw-rw-rw-   0        0        0     3222 2023-06-12 17:37:33.000000 client_chat_study_project_adub-0.3/client_chat_adub/client/add_contact.py
+-rw-rw-rw-   0        0        0     8228 2023-06-12 19:41:31.000000 client_chat_study_project_adub-0.3/client_chat_adub/client/client_db.py
+-rw-rw-rw-   0        0        0     1590 2023-06-12 17:37:33.000000 client_chat_study_project_adub-0.3/client_chat_adub/client/del_contact.py
+-rw-rw-rw-   0        0        0    15395 2023-06-12 17:37:33.000000 client_chat_study_project_adub-0.3/client_chat_adub/client/main_window.py
+-rw-rw-rw-   0        0        0     5577 2023-06-12 17:37:33.000000 client_chat_study_project_adub-0.3/client_chat_adub/client/main_window_conv.py
+-rw-rw-rw-   0        0        0     1760 2023-06-12 17:37:33.000000 client_chat_study_project_adub-0.3/client_chat_adub/client/start_dialog.py
+-rw-rw-rw-   0        0        0    12954 2023-06-12 17:37:33.000000 client_chat_study_project_adub-0.3/client_chat_adub/client/transport.py
+-rw-rw-rw-   0        0        0     3141 2023-06-12 19:32:56.000000 client_chat_study_project_adub-0.3/client_chat_adub/client.py
+drwxrwxrwx   0        0        0        0 2023-06-13 09:47:03.105165 client_chat_study_project_adub-0.3/client_chat_adub/common/
+-rw-rw-rw-   0        0        0        0 2023-06-12 17:37:33.000000 client_chat_study_project_adub-0.3/client_chat_adub/common/__init__.py
+-rw-rw-rw-   0        0        0     1182 2023-06-12 17:37:33.000000 client_chat_study_project_adub-0.3/client_chat_adub/common/data_transfer.py
+-rw-rw-rw-   0        0        0     2998 2023-06-12 17:37:33.000000 client_chat_study_project_adub-0.3/client_chat_adub/common/decorators.py
+-rw-rw-rw-   0        0        0     1123 2023-06-12 19:56:09.000000 client_chat_study_project_adub-0.3/client_chat_adub/common/descriptors.py
+-rw-rw-rw-   0        0        0      393 2023-06-12 17:37:33.000000 client_chat_study_project_adub-0.3/client_chat_adub/common/errors.py
+-rw-rw-rw-   0        0        0     3603 2023-06-12 17:37:33.000000 client_chat_study_project_adub-0.3/client_chat_adub/common/metaclasses.py
+drwxrwxrwx   0        0        0        0 2023-06-13 09:47:03.107578 client_chat_study_project_adub-0.3/client_chat_adub/logs/
+-rw-rw-rw-   0        0        0        0 2023-06-12 17:37:33.000000 client_chat_study_project_adub-0.3/client_chat_adub/logs/__init__.py
+-rw-rw-rw-   0        0        0      656 2023-06-12 19:29:57.000000 client_chat_study_project_adub-0.3/client_chat_adub/logs/client_log_config.py
+-rw-rw-rw-   0        0        0      924 2023-06-12 19:21:27.000000 client_chat_study_project_adub-0.3/client_chat_adub/logs/server_log_config.py
+drwxrwxrwx   0        0        0        0 2023-06-13 09:47:03.113835 client_chat_study_project_adub-0.3/client_chat_study_project_adub.egg-info/
+-rw-rw-rw-   0        0        0      157 2023-06-13 09:47:03.000000 client_chat_study_project_adub-0.3/client_chat_study_project_adub.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      991 2023-06-13 09:47:03.000000 client_chat_study_project_adub-0.3/client_chat_study_project_adub.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 09:47:03.000000 client_chat_study_project_adub-0.3/client_chat_study_project_adub.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2023-06-13 09:47:03.000000 client_chat_study_project_adub-0.3/client_chat_study_project_adub.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-06-13 09:47:03.000000 client_chat_study_project_adub-0.3/client_chat_study_project_adub.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-13 09:47:03.115836 client_chat_study_project_adub-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      356 2023-06-13 09:46:59.000000 client_chat_study_project_adub-0.3/setup.py
```

### Comparing `client_chat_study_project_adub-0.2/client_chat_adub/client/add_contact.py` & `client_chat_study_project_adub-0.3/client_chat_adub/client/add_contact.py`

 * *Files identical despite different names*

### Comparing `client_chat_study_project_adub-0.2/client_chat_adub/client/client_db.py` & `client_chat_study_project_adub-0.3/client_chat_adub/client/client_db.py`

 * *Files identical despite different names*

### Comparing `client_chat_study_project_adub-0.2/client_chat_adub/client/del_contact.py` & `client_chat_study_project_adub-0.3/client_chat_adub/client/del_contact.py`

 * *Files identical despite different names*

### Comparing `client_chat_study_project_adub-0.2/client_chat_adub/client/main_window.py` & `client_chat_study_project_adub-0.3/client_chat_adub/client/main_window.py`

 * *Files identical despite different names*

### Comparing `client_chat_study_project_adub-0.2/client_chat_adub/client/main_window_conv.py` & `client_chat_study_project_adub-0.3/client_chat_adub/client/main_window_conv.py`

 * *Files identical despite different names*

### Comparing `client_chat_study_project_adub-0.2/client_chat_adub/client/start_dialog.py` & `client_chat_study_project_adub-0.3/client_chat_adub/client/start_dialog.py`

 * *Files identical despite different names*

### Comparing `client_chat_study_project_adub-0.2/client_chat_adub/client/transport.py` & `client_chat_study_project_adub-0.3/client_chat_adub/client/transport.py`

 * *Files identical despite different names*

### Comparing `client_chat_study_project_adub-0.2/client_chat_adub/client.py` & `client_chat_study_project_adub-0.3/client_chat_adub/client.py`

 * *Files identical despite different names*

### Comparing `client_chat_study_project_adub-0.2/client_chat_adub/common/data_transfer.py` & `client_chat_study_project_adub-0.3/client_chat_adub/common/data_transfer.py`

 * *Files identical despite different names*

### Comparing `client_chat_study_project_adub-0.2/client_chat_adub/common/decorators.py` & `client_chat_study_project_adub-0.3/client_chat_adub/common/decorators.py`

 * *Files identical despite different names*

### Comparing `client_chat_study_project_adub-0.2/client_chat_adub/common/descriptors.py` & `client_chat_study_project_adub-0.3/client_chat_adub/common/descriptors.py`

 * *Files identical despite different names*

### Comparing `client_chat_study_project_adub-0.2/client_chat_adub/common/metaclasses.py` & `client_chat_study_project_adub-0.3/client_chat_adub/common/metaclasses.py`

 * *Files identical despite different names*

### Comparing `client_chat_study_project_adub-0.2/client_chat_adub/logs/client_log_config.py` & `client_chat_study_project_adub-0.3/client_chat_adub/logs/client_log_config.py`

 * *Files identical despite different names*

### Comparing `client_chat_study_project_adub-0.2/client_chat_adub/logs/server_log_config.py` & `client_chat_study_project_adub-0.3/client_chat_adub/logs/server_log_config.py`

 * *Files identical despite different names*

### Comparing `client_chat_study_project_adub-0.2/client_chat_study_project_adub.egg-info/SOURCES.txt` & `client_chat_study_project_adub-0.3/client_chat_study_project_adub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

