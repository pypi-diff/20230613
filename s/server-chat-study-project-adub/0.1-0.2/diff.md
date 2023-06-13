# Comparing `tmp/server_chat_study_project_adub-0.1.tar.gz` & `tmp/server_chat_study_project_adub-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "server_chat_study_project_adub-0.1.tar", last modified: Tue Jun 13 09:13:24 2023, max compression
+gzip compressed data, was "server_chat_study_project_adub-0.2.tar", last modified: Tue Jun 13 09:34:30 2023, max compression
```

## Comparing `server_chat_study_project_adub-0.1.tar` & `server_chat_study_project_adub-0.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 09:13:24.947084 server_chat_study_project_adub-0.1/
--rw-rw-rw-   0        0        0      157 2023-06-13 09:13:24.947084 server_chat_study_project_adub-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-13 09:13:24.904084 server_chat_study_project_adub-0.1/server_chat_study_project_adub.egg-info/
--rw-rw-rw-   0        0        0      157 2023-06-13 09:13:24.000000 server_chat_study_project_adub-0.1/server_chat_study_project_adub.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      739 2023-06-13 09:13:24.000000 server_chat_study_project_adub-0.1/server_chat_study_project_adub.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 09:13:24.000000 server_chat_study_project_adub-0.1/server_chat_study_project_adub.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-06-13 09:13:24.000000 server_chat_study_project_adub-0.1/server_chat_study_project_adub.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-06-13 09:13:24.000000 server_chat_study_project_adub-0.1/server_chat_study_project_adub.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-13 09:13:24.947084 server_chat_study_project_adub-0.1/setup.cfg
--rw-rw-rw-   0        0        0      356 2023-06-13 09:13:10.000000 server_chat_study_project_adub-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-13 09:13:24.909084 server_chat_study_project_adub-0.1/src/
--rw-rw-rw-   0        0        0        0 2023-06-12 20:38:33.000000 server_chat_study_project_adub-0.1/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 09:13:24.914084 server_chat_study_project_adub-0.1/src/common/
--rw-rw-rw-   0        0        0        0 2023-06-12 17:37:33.000000 server_chat_study_project_adub-0.1/src/common/__init__.py
--rw-rw-rw-   0        0        0     1182 2023-06-12 17:37:33.000000 server_chat_study_project_adub-0.1/src/common/data_transfer.py
--rw-rw-rw-   0        0        0     2998 2023-06-12 17:37:33.000000 server_chat_study_project_adub-0.1/src/common/decorators.py
--rw-rw-rw-   0        0        0     1123 2023-06-12 19:56:09.000000 server_chat_study_project_adub-0.1/src/common/descriptors.py
--rw-rw-rw-   0        0        0      393 2023-06-12 17:37:33.000000 server_chat_study_project_adub-0.1/src/common/errors.py
--rw-rw-rw-   0        0        0     3603 2023-06-12 17:37:33.000000 server_chat_study_project_adub-0.1/src/common/metaclasses.py
-drwxrwxrwx   0        0        0        0 2023-06-13 09:13:24.917084 server_chat_study_project_adub-0.1/src/logs/
--rw-rw-rw-   0        0        0        0 2023-06-12 17:37:33.000000 server_chat_study_project_adub-0.1/src/logs/__init__.py
--rw-rw-rw-   0        0        0      656 2023-06-12 19:29:57.000000 server_chat_study_project_adub-0.1/src/logs/client_log_config.py
--rw-rw-rw-   0        0        0      924 2023-06-12 19:21:27.000000 server_chat_study_project_adub-0.1/src/logs/server_log_config.py
-drwxrwxrwx   0        0        0        0 2023-06-13 09:13:24.946084 server_chat_study_project_adub-0.1/src/server/
--rw-rw-rw-   0        0        0        0 2023-06-12 17:37:33.000000 server_chat_study_project_adub-0.1/src/server/__init__.py
--rw-rw-rw-   0        0        0     3773 2023-06-12 17:37:33.000000 server_chat_study_project_adub-0.1/src/server/add_user.py
--rw-rw-rw-   0        0        0     4748 2023-06-12 19:36:15.000000 server_chat_study_project_adub-0.1/src/server/config_window.py
--rw-rw-rw-   0        0        0     4602 2023-06-12 17:37:33.000000 server_chat_study_project_adub-0.1/src/server/main_window.py
--rw-rw-rw-   0        0        0     2094 2023-06-12 17:37:33.000000 server_chat_study_project_adub-0.1/src/server/remove_user.py
--rw-rw-rw-   0        0        0    18324 2023-06-12 20:00:21.000000 server_chat_study_project_adub-0.1/src/server/server_core.py
--rw-rw-rw-   0        0        0    14941 2023-06-12 19:41:31.000000 server_chat_study_project_adub-0.1/src/server/server_db.py
--rw-rw-rw-   0        0        0     2033 2023-06-12 17:37:33.000000 server_chat_study_project_adub-0.1/src/server/stat_window.py
--rw-rw-rw-   0        0        0     2861 2023-06-12 19:32:56.000000 server_chat_study_project_adub-0.1/src/server.py
+drwxrwxrwx   0        0        0        0 2023-06-13 09:34:30.776930 server_chat_study_project_adub-0.2/
+-rw-rw-rw-   0        0        0      157 2023-06-13 09:34:30.775929 server_chat_study_project_adub-0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-13 09:34:30.750383 server_chat_study_project_adub-0.2/server_chat_adub/
+-rw-rw-rw-   0        0        0        0 2023-06-12 20:38:33.000000 server_chat_study_project_adub-0.2/server_chat_adub/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 09:34:30.753759 server_chat_study_project_adub-0.2/server_chat_adub/common/
+-rw-rw-rw-   0        0        0        0 2023-06-12 17:37:33.000000 server_chat_study_project_adub-0.2/server_chat_adub/common/__init__.py
+-rw-rw-rw-   0        0        0     1182 2023-06-12 17:37:33.000000 server_chat_study_project_adub-0.2/server_chat_adub/common/data_transfer.py
+-rw-rw-rw-   0        0        0     2998 2023-06-12 17:37:33.000000 server_chat_study_project_adub-0.2/server_chat_adub/common/decorators.py
+-rw-rw-rw-   0        0        0     1123 2023-06-12 19:56:09.000000 server_chat_study_project_adub-0.2/server_chat_adub/common/descriptors.py
+-rw-rw-rw-   0        0        0      393 2023-06-12 17:37:33.000000 server_chat_study_project_adub-0.2/server_chat_adub/common/errors.py
+-rw-rw-rw-   0        0        0     3603 2023-06-12 17:37:33.000000 server_chat_study_project_adub-0.2/server_chat_adub/common/metaclasses.py
+drwxrwxrwx   0        0        0        0 2023-06-13 09:34:30.755766 server_chat_study_project_adub-0.2/server_chat_adub/logs/
+-rw-rw-rw-   0        0        0        0 2023-06-12 17:37:33.000000 server_chat_study_project_adub-0.2/server_chat_adub/logs/__init__.py
+-rw-rw-rw-   0        0        0      656 2023-06-12 19:29:57.000000 server_chat_study_project_adub-0.2/server_chat_adub/logs/client_log_config.py
+-rw-rw-rw-   0        0        0      924 2023-06-12 19:21:27.000000 server_chat_study_project_adub-0.2/server_chat_adub/logs/server_log_config.py
+drwxrwxrwx   0        0        0        0 2023-06-13 09:34:30.759766 server_chat_study_project_adub-0.2/server_chat_adub/server/
+-rw-rw-rw-   0        0        0        0 2023-06-12 17:37:33.000000 server_chat_study_project_adub-0.2/server_chat_adub/server/__init__.py
+-rw-rw-rw-   0        0        0     3773 2023-06-12 17:37:33.000000 server_chat_study_project_adub-0.2/server_chat_adub/server/add_user.py
+-rw-rw-rw-   0        0        0     4748 2023-06-12 19:36:15.000000 server_chat_study_project_adub-0.2/server_chat_adub/server/config_window.py
+-rw-rw-rw-   0        0        0     4602 2023-06-12 17:37:33.000000 server_chat_study_project_adub-0.2/server_chat_adub/server/main_window.py
+-rw-rw-rw-   0        0        0     2094 2023-06-12 17:37:33.000000 server_chat_study_project_adub-0.2/server_chat_adub/server/remove_user.py
+-rw-rw-rw-   0        0        0    18324 2023-06-12 20:00:21.000000 server_chat_study_project_adub-0.2/server_chat_adub/server/server_core.py
+-rw-rw-rw-   0        0        0    14941 2023-06-12 19:41:31.000000 server_chat_study_project_adub-0.2/server_chat_adub/server/server_db.py
+-rw-rw-rw-   0        0        0     2033 2023-06-12 17:37:33.000000 server_chat_study_project_adub-0.2/server_chat_adub/server/stat_window.py
+-rw-rw-rw-   0        0        0     2861 2023-06-12 19:32:56.000000 server_chat_study_project_adub-0.2/server_chat_adub/server.py
+drwxrwxrwx   0        0        0        0 2023-06-13 09:34:30.775929 server_chat_study_project_adub-0.2/server_chat_study_project_adub.egg-info/
+-rw-rw-rw-   0        0        0      157 2023-06-13 09:34:30.000000 server_chat_study_project_adub-0.2/server_chat_study_project_adub.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      986 2023-06-13 09:34:30.000000 server_chat_study_project_adub-0.2/server_chat_study_project_adub.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 09:34:30.000000 server_chat_study_project_adub-0.2/server_chat_study_project_adub.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2023-06-13 09:34:30.000000 server_chat_study_project_adub-0.2/server_chat_study_project_adub.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-06-13 09:34:30.000000 server_chat_study_project_adub-0.2/server_chat_study_project_adub.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-13 09:34:30.776930 server_chat_study_project_adub-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      356 2023-06-13 09:34:18.000000 server_chat_study_project_adub-0.2/setup.py
```

### Comparing `server_chat_study_project_adub-0.1/server_chat_study_project_adub.egg-info/SOURCES.txt` & `server_chat_study_project_adub-0.2/server_chat_study_project_adub.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 setup.py
+server_chat_adub/__init__.py
+server_chat_adub/server.py
+server_chat_adub/common/__init__.py
+server_chat_adub/common/data_transfer.py
+server_chat_adub/common/decorators.py
+server_chat_adub/common/descriptors.py
+server_chat_adub/common/errors.py
+server_chat_adub/common/metaclasses.py
+server_chat_adub/logs/__init__.py
+server_chat_adub/logs/client_log_config.py
+server_chat_adub/logs/server_log_config.py
+server_chat_adub/server/__init__.py
+server_chat_adub/server/add_user.py
+server_chat_adub/server/config_window.py
+server_chat_adub/server/main_window.py
+server_chat_adub/server/remove_user.py
+server_chat_adub/server/server_core.py
+server_chat_adub/server/server_db.py
+server_chat_adub/server/stat_window.py
 server_chat_study_project_adub.egg-info/PKG-INFO
 server_chat_study_project_adub.egg-info/SOURCES.txt
 server_chat_study_project_adub.egg-info/dependency_links.txt
 server_chat_study_project_adub.egg-info/requires.txt
-server_chat_study_project_adub.egg-info/top_level.txt
-src/__init__.py
-src/server.py
-src/common/__init__.py
-src/common/data_transfer.py
-src/common/decorators.py
-src/common/descriptors.py
-src/common/errors.py
-src/common/metaclasses.py
-src/logs/__init__.py
-src/logs/client_log_config.py
-src/logs/server_log_config.py
-src/server/__init__.py
-src/server/add_user.py
-src/server/config_window.py
-src/server/main_window.py
-src/server/remove_user.py
-src/server/server_core.py
-src/server/server_db.py
-src/server/stat_window.py
+server_chat_study_project_adub.egg-info/top_level.txt
```

### Comparing `server_chat_study_project_adub-0.1/src/common/data_transfer.py` & `server_chat_study_project_adub-0.2/server_chat_adub/common/data_transfer.py`

 * *Files identical despite different names*

### Comparing `server_chat_study_project_adub-0.1/src/common/decorators.py` & `server_chat_study_project_adub-0.2/server_chat_adub/common/decorators.py`

 * *Files identical despite different names*

### Comparing `server_chat_study_project_adub-0.1/src/common/descriptors.py` & `server_chat_study_project_adub-0.2/server_chat_adub/common/descriptors.py`

 * *Files identical despite different names*

### Comparing `server_chat_study_project_adub-0.1/src/common/metaclasses.py` & `server_chat_study_project_adub-0.2/server_chat_adub/common/metaclasses.py`

 * *Files identical despite different names*

### Comparing `server_chat_study_project_adub-0.1/src/logs/client_log_config.py` & `server_chat_study_project_adub-0.2/server_chat_adub/logs/client_log_config.py`

 * *Files identical despite different names*

### Comparing `server_chat_study_project_adub-0.1/src/logs/server_log_config.py` & `server_chat_study_project_adub-0.2/server_chat_adub/logs/server_log_config.py`

 * *Files identical despite different names*

### Comparing `server_chat_study_project_adub-0.1/src/server/add_user.py` & `server_chat_study_project_adub-0.2/server_chat_adub/server/add_user.py`

 * *Files identical despite different names*

### Comparing `server_chat_study_project_adub-0.1/src/server/config_window.py` & `server_chat_study_project_adub-0.2/server_chat_adub/server/config_window.py`

 * *Files identical despite different names*

### Comparing `server_chat_study_project_adub-0.1/src/server/main_window.py` & `server_chat_study_project_adub-0.2/server_chat_adub/server/main_window.py`

 * *Files identical despite different names*

### Comparing `server_chat_study_project_adub-0.1/src/server/remove_user.py` & `server_chat_study_project_adub-0.2/server_chat_adub/server/remove_user.py`

 * *Files identical despite different names*

### Comparing `server_chat_study_project_adub-0.1/src/server/server_core.py` & `server_chat_study_project_adub-0.2/server_chat_adub/server/server_core.py`

 * *Files identical despite different names*

### Comparing `server_chat_study_project_adub-0.1/src/server/server_db.py` & `server_chat_study_project_adub-0.2/server_chat_adub/server/server_db.py`

 * *Files identical despite different names*

### Comparing `server_chat_study_project_adub-0.1/src/server/stat_window.py` & `server_chat_study_project_adub-0.2/server_chat_adub/server/stat_window.py`

 * *Files identical despite different names*

### Comparing `server_chat_study_project_adub-0.1/src/server.py` & `server_chat_study_project_adub-0.2/server_chat_adub/server.py`

 * *Files identical despite different names*

