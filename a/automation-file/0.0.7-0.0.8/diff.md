# Comparing `tmp/automation_file-0.0.7.tar.gz` & `tmp/automation_file-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automation_file-0.0.7.tar", last modified: Mon Jun 12 07:34:56 2023, max compression
+gzip compressed data, was "automation_file-0.0.8.tar", last modified: Tue Jun 13 07:20:16 2023, max compression
```

## Comparing `automation_file-0.0.7.tar` & `automation_file-0.0.8.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 07:34:56.397887 automation_file-0.0.7/
--rw-rw-rw-   0        0        0     1085 2023-05-18 06:36:21.000000 automation_file-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     1302 2023-06-12 07:34:56.396880 automation_file-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      679 2023-05-30 06:22:36.000000 automation_file-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 07:34:56.289681 automation_file-0.0.7/automation_file.egg-info/
--rw-rw-rw-   0        0        0     1302 2023-06-12 07:34:56.000000 automation_file-0.0.7/automation_file.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1992 2023-06-12 07:34:56.000000 automation_file-0.0.7/automation_file.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 07:34:56.000000 automation_file-0.0.7/automation_file.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       79 2023-06-12 07:34:56.000000 automation_file-0.0.7/automation_file.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-12 07:34:56.000000 automation_file-0.0.7/automation_file.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-12 07:34:56.292659 automation_file-0.0.7/file_automation/
--rw-rw-rw-   0        0        0     1804 2023-06-08 09:31:05.000000 automation_file-0.0.7/file_automation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 07:34:56.296162 automation_file-0.0.7/file_automation/local/
--rw-rw-rw-   0        0        0        0 2023-05-29 02:05:02.000000 automation_file-0.0.7/file_automation/local/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 07:34:56.302143 automation_file-0.0.7/file_automation/local/dir/
--rw-rw-rw-   0        0        0        0 2023-05-18 06:38:51.000000 automation_file-0.0.7/file_automation/local/dir/__init__.py
--rw-rw-rw-   0        0        0     2135 2023-06-08 06:26:10.000000 automation_file-0.0.7/file_automation/local/dir/dir_process.py
-drwxrwxrwx   0        0        0        0 2023-06-12 07:34:56.307855 automation_file-0.0.7/file_automation/local/file/
--rw-rw-rw-   0        0        0        0 2023-05-18 06:38:46.000000 automation_file-0.0.7/file_automation/local/file/__init__.py
--rw-rw-rw-   0        0        0     3716 2023-06-08 06:40:19.000000 automation_file-0.0.7/file_automation/local/file/file_process.py
-drwxrwxrwx   0        0        0        0 2023-06-12 07:34:56.313016 automation_file-0.0.7/file_automation/local/zip/
--rw-rw-rw-   0        0        0        0 2023-05-19 07:24:05.000000 automation_file-0.0.7/file_automation/local/zip/__init__.py
--rw-rw-rw-   0        0        0     3626 2023-06-12 07:22:51.000000 automation_file-0.0.7/file_automation/local/zip/zip_process.py
-drwxrwxrwx   0        0        0        0 2023-06-12 07:34:56.316013 automation_file-0.0.7/file_automation/remote/
--rw-rw-rw-   0        0        0        0 2023-05-29 02:05:15.000000 automation_file-0.0.7/file_automation/remote/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 07:34:56.320049 automation_file-0.0.7/file_automation/remote/google_drive/
--rw-rw-rw-   0        0        0        0 2023-05-29 02:05:24.000000 automation_file-0.0.7/file_automation/remote/google_drive/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 07:34:56.326053 automation_file-0.0.7/file_automation/remote/google_drive/delete/
--rw-rw-rw-   0        0        0        0 2023-06-05 01:25:46.000000 automation_file-0.0.7/file_automation/remote/google_drive/delete/__init__.py
--rw-rw-rw-   0        0        0      648 2023-06-08 07:37:31.000000 automation_file-0.0.7/file_automation/remote/google_drive/delete/delete_manager.py
-drwxrwxrwx   0        0        0        0 2023-06-12 07:34:56.331210 automation_file-0.0.7/file_automation/remote/google_drive/dir/
--rw-rw-rw-   0        0        0        0 2023-06-05 01:25:46.000000 automation_file-0.0.7/file_automation/remote/google_drive/dir/__init__.py
--rw-rw-rw-   0        0        0      876 2023-06-08 07:41:43.000000 automation_file-0.0.7/file_automation/remote/google_drive/dir/folder_manager.py
-drwxrwxrwx   0        0        0        0 2023-06-12 07:34:56.336207 automation_file-0.0.7/file_automation/remote/google_drive/download/
--rw-rw-rw-   0        0        0        0 2023-06-05 01:25:46.000000 automation_file-0.0.7/file_automation/remote/google_drive/download/__init__.py
--rw-rw-rw-   0        0        0     2139 2023-06-08 07:46:57.000000 automation_file-0.0.7/file_automation/remote/google_drive/download/download_file.py
--rw-rw-rw-   0        0        0     2153 2023-06-08 08:45:58.000000 automation_file-0.0.7/file_automation/remote/google_drive/driver_instance.py
-drwxrwxrwx   0        0        0        0 2023-06-12 07:34:56.341596 automation_file-0.0.7/file_automation/remote/google_drive/search/
--rw-rw-rw-   0        0        0        0 2023-06-05 01:25:46.000000 automation_file-0.0.7/file_automation/remote/google_drive/search/__init__.py
--rw-rw-rw-   0        0        0     2308 2023-06-08 07:49:23.000000 automation_file-0.0.7/file_automation/remote/google_drive/search/search_drive.py
-drwxrwxrwx   0        0        0        0 2023-06-12 07:34:56.346825 automation_file-0.0.7/file_automation/remote/google_drive/share/
--rw-rw-rw-   0        0        0        0 2023-06-05 01:25:46.000000 automation_file-0.0.7/file_automation/remote/google_drive/share/__init__.py
--rw-rw-rw-   0        0        0     2524 2023-06-08 07:55:10.000000 automation_file-0.0.7/file_automation/remote/google_drive/share/share_file.py
-drwxrwxrwx   0        0        0        0 2023-06-12 07:34:56.351344 automation_file-0.0.7/file_automation/remote/google_drive/upload/
--rw-rw-rw-   0        0        0        0 2023-06-05 01:25:46.000000 automation_file-0.0.7/file_automation/remote/google_drive/upload/__init__.py
--rw-rw-rw-   0        0        0     3823 2023-06-08 08:10:58.000000 automation_file-0.0.7/file_automation/remote/google_drive/upload/upload_to_driver.py
-drwxrwxrwx   0        0        0        0 2023-06-12 07:34:56.353344 automation_file-0.0.7/file_automation/utils/
--rw-rw-rw-   0        0        0        0 2023-05-18 07:59:01.000000 automation_file-0.0.7/file_automation/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 07:34:56.357856 automation_file-0.0.7/file_automation/utils/callback/
--rw-rw-rw-   0        0        0        0 2023-03-31 01:55:17.000000 automation_file-0.0.7/file_automation/utils/callback/__init__.py
--rw-rw-rw-   0        0        0     5297 2023-06-12 07:00:20.000000 automation_file-0.0.7/file_automation/utils/callback/callback_function_executor.py
-drwxrwxrwx   0        0        0        0 2023-06-12 07:34:56.368888 automation_file-0.0.7/file_automation/utils/exception/
--rw-rw-rw-   0        0        0        0 2023-05-18 07:59:15.000000 automation_file-0.0.7/file_automation/utils/exception/__init__.py
--rw-rw-rw-   0        0        0      726 2023-06-08 09:16:50.000000 automation_file-0.0.7/file_automation/utils/exception/exception_tags.py
--rw-rw-rw-   0        0        0      541 2023-06-08 09:16:50.000000 automation_file-0.0.7/file_automation/utils/exception/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-06-12 07:34:56.373891 automation_file-0.0.7/file_automation/utils/executor/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 automation_file-0.0.7/file_automation/utils/executor/__init__.py
--rw-rw-rw-   0        0        0     6611 2023-06-12 07:17:42.000000 automation_file-0.0.7/file_automation/utils/executor/action_executor.py
-drwxrwxrwx   0        0        0        0 2023-06-12 07:34:56.380965 automation_file-0.0.7/file_automation/utils/json/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 automation_file-0.0.7/file_automation/utils/json/__init__.py
--rw-rw-rw-   0        0        0     1600 2023-06-12 07:17:42.000000 automation_file-0.0.7/file_automation/utils/json/json_file.py
-drwxrwxrwx   0        0        0        0 2023-06-12 07:34:56.387112 automation_file-0.0.7/file_automation/utils/logging/
--rw-rw-rw-   0        0        0        0 2023-06-08 03:44:59.000000 automation_file-0.0.7/file_automation/utils/logging/__init__.py
--rw-rw-rw-   0        0        0      620 2023-06-12 07:11:23.000000 automation_file-0.0.7/file_automation/utils/logging/loggin_instance.py
-drwxrwxrwx   0        0        0        0 2023-06-12 07:34:56.393200 automation_file-0.0.7/file_automation/utils/scheduler/
--rw-rw-rw-   0        0        0        0 2023-05-31 01:17:46.000000 automation_file-0.0.7/file_automation/utils/scheduler/__init__.py
--rw-rw-rw-   0        0        0     7002 2023-06-12 07:17:42.000000 automation_file-0.0.7/file_automation/utils/scheduler/extend_apscheduler.py
--rw-rw-rw-   0        0        0     1004 2023-06-12 07:34:34.000000 automation_file-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-12 07:34:56.398922 automation_file-0.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-13 07:20:16.851022 automation_file-0.0.8/
+-rw-rw-rw-   0        0        0     1085 2023-05-18 06:36:21.000000 automation_file-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     1302 2023-06-13 07:20:16.850022 automation_file-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      679 2023-05-30 06:22:36.000000 automation_file-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-06-13 07:20:16.723709 automation_file-0.0.8/automation_file.egg-info/
+-rw-rw-rw-   0        0        0     1302 2023-06-13 07:20:16.000000 automation_file-0.0.8/automation_file.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1992 2023-06-13 07:20:16.000000 automation_file-0.0.8/automation_file.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 07:20:16.000000 automation_file-0.0.8/automation_file.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       79 2023-06-13 07:20:16.000000 automation_file-0.0.8/automation_file.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-13 07:20:16.000000 automation_file-0.0.8/automation_file.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-13 07:20:16.727785 automation_file-0.0.8/file_automation/
+-rw-rw-rw-   0        0        0     1804 2023-06-08 09:31:05.000000 automation_file-0.0.8/file_automation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 07:20:16.730841 automation_file-0.0.8/file_automation/local/
+-rw-rw-rw-   0        0        0        0 2023-05-29 02:05:02.000000 automation_file-0.0.8/file_automation/local/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 07:20:16.738828 automation_file-0.0.8/file_automation/local/dir/
+-rw-rw-rw-   0        0        0        0 2023-05-18 06:38:51.000000 automation_file-0.0.8/file_automation/local/dir/__init__.py
+-rw-rw-rw-   0        0        0     2135 2023-06-08 06:26:10.000000 automation_file-0.0.8/file_automation/local/dir/dir_process.py
+drwxrwxrwx   0        0        0        0 2023-06-13 07:20:16.743836 automation_file-0.0.8/file_automation/local/file/
+-rw-rw-rw-   0        0        0        0 2023-05-18 06:38:46.000000 automation_file-0.0.8/file_automation/local/file/__init__.py
+-rw-rw-rw-   0        0        0     3716 2023-06-08 06:40:19.000000 automation_file-0.0.8/file_automation/local/file/file_process.py
+drwxrwxrwx   0        0        0        0 2023-06-13 07:20:16.750357 automation_file-0.0.8/file_automation/local/zip/
+-rw-rw-rw-   0        0        0        0 2023-05-19 07:24:05.000000 automation_file-0.0.8/file_automation/local/zip/__init__.py
+-rw-rw-rw-   0        0        0     3626 2023-06-12 07:22:51.000000 automation_file-0.0.8/file_automation/local/zip/zip_process.py
+drwxrwxrwx   0        0        0        0 2023-06-13 07:20:16.753422 automation_file-0.0.8/file_automation/remote/
+-rw-rw-rw-   0        0        0        0 2023-05-29 02:05:15.000000 automation_file-0.0.8/file_automation/remote/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 07:20:16.759485 automation_file-0.0.8/file_automation/remote/google_drive/
+-rw-rw-rw-   0        0        0        0 2023-05-29 02:05:24.000000 automation_file-0.0.8/file_automation/remote/google_drive/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 07:20:16.766907 automation_file-0.0.8/file_automation/remote/google_drive/delete/
+-rw-rw-rw-   0        0        0        0 2023-06-05 01:25:46.000000 automation_file-0.0.8/file_automation/remote/google_drive/delete/__init__.py
+-rw-rw-rw-   0        0        0      648 2023-06-08 07:37:31.000000 automation_file-0.0.8/file_automation/remote/google_drive/delete/delete_manager.py
+drwxrwxrwx   0        0        0        0 2023-06-13 07:20:16.774458 automation_file-0.0.8/file_automation/remote/google_drive/dir/
+-rw-rw-rw-   0        0        0        0 2023-06-05 01:25:46.000000 automation_file-0.0.8/file_automation/remote/google_drive/dir/__init__.py
+-rw-rw-rw-   0        0        0      876 2023-06-08 07:41:43.000000 automation_file-0.0.8/file_automation/remote/google_drive/dir/folder_manager.py
+drwxrwxrwx   0        0        0        0 2023-06-13 07:20:16.780546 automation_file-0.0.8/file_automation/remote/google_drive/download/
+-rw-rw-rw-   0        0        0        0 2023-06-05 01:25:46.000000 automation_file-0.0.8/file_automation/remote/google_drive/download/__init__.py
+-rw-rw-rw-   0        0        0     2139 2023-06-08 07:46:57.000000 automation_file-0.0.8/file_automation/remote/google_drive/download/download_file.py
+-rw-rw-rw-   0        0        0     2153 2023-06-08 08:45:58.000000 automation_file-0.0.8/file_automation/remote/google_drive/driver_instance.py
+drwxrwxrwx   0        0        0        0 2023-06-13 07:20:16.788669 automation_file-0.0.8/file_automation/remote/google_drive/search/
+-rw-rw-rw-   0        0        0        0 2023-06-05 01:25:46.000000 automation_file-0.0.8/file_automation/remote/google_drive/search/__init__.py
+-rw-rw-rw-   0        0        0     2308 2023-06-08 07:49:23.000000 automation_file-0.0.8/file_automation/remote/google_drive/search/search_drive.py
+drwxrwxrwx   0        0        0        0 2023-06-13 07:20:16.794773 automation_file-0.0.8/file_automation/remote/google_drive/share/
+-rw-rw-rw-   0        0        0        0 2023-06-05 01:25:46.000000 automation_file-0.0.8/file_automation/remote/google_drive/share/__init__.py
+-rw-rw-rw-   0        0        0     2524 2023-06-08 07:55:10.000000 automation_file-0.0.8/file_automation/remote/google_drive/share/share_file.py
+drwxrwxrwx   0        0        0        0 2023-06-13 07:20:16.801855 automation_file-0.0.8/file_automation/remote/google_drive/upload/
+-rw-rw-rw-   0        0        0        0 2023-06-05 01:25:46.000000 automation_file-0.0.8/file_automation/remote/google_drive/upload/__init__.py
+-rw-rw-rw-   0        0        0     3823 2023-06-08 08:10:58.000000 automation_file-0.0.8/file_automation/remote/google_drive/upload/upload_to_driver.py
+drwxrwxrwx   0        0        0        0 2023-06-13 07:20:16.806902 automation_file-0.0.8/file_automation/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-18 07:59:01.000000 automation_file-0.0.8/file_automation/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 07:20:16.813169 automation_file-0.0.8/file_automation/utils/callback/
+-rw-rw-rw-   0        0        0        0 2023-03-31 01:55:17.000000 automation_file-0.0.8/file_automation/utils/callback/__init__.py
+-rw-rw-rw-   0        0        0     5297 2023-06-12 07:00:20.000000 automation_file-0.0.8/file_automation/utils/callback/callback_function_executor.py
+drwxrwxrwx   0        0        0        0 2023-06-13 07:20:16.821801 automation_file-0.0.8/file_automation/utils/exception/
+-rw-rw-rw-   0        0        0        0 2023-05-18 07:59:15.000000 automation_file-0.0.8/file_automation/utils/exception/__init__.py
+-rw-rw-rw-   0        0        0      726 2023-06-08 09:16:50.000000 automation_file-0.0.8/file_automation/utils/exception/exception_tags.py
+-rw-rw-rw-   0        0        0      541 2023-06-08 09:16:50.000000 automation_file-0.0.8/file_automation/utils/exception/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-06-13 07:20:16.828717 automation_file-0.0.8/file_automation/utils/executor/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 automation_file-0.0.8/file_automation/utils/executor/__init__.py
+-rw-rw-rw-   0        0        0     6741 2023-06-13 06:29:23.000000 automation_file-0.0.8/file_automation/utils/executor/action_executor.py
+drwxrwxrwx   0        0        0        0 2023-06-13 07:20:16.834938 automation_file-0.0.8/file_automation/utils/json/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:05:06.000000 automation_file-0.0.8/file_automation/utils/json/__init__.py
+-rw-rw-rw-   0        0        0     1600 2023-06-12 07:17:42.000000 automation_file-0.0.8/file_automation/utils/json/json_file.py
+drwxrwxrwx   0        0        0        0 2023-06-13 07:20:16.841504 automation_file-0.0.8/file_automation/utils/logging/
+-rw-rw-rw-   0        0        0        0 2023-06-08 03:44:59.000000 automation_file-0.0.8/file_automation/utils/logging/__init__.py
+-rw-rw-rw-   0        0        0      620 2023-06-12 07:11:23.000000 automation_file-0.0.8/file_automation/utils/logging/loggin_instance.py
+drwxrwxrwx   0        0        0        0 2023-06-13 07:20:16.847472 automation_file-0.0.8/file_automation/utils/scheduler/
+-rw-rw-rw-   0        0        0        0 2023-05-31 01:17:46.000000 automation_file-0.0.8/file_automation/utils/scheduler/__init__.py
+-rw-rw-rw-   0        0        0     7002 2023-06-12 07:17:42.000000 automation_file-0.0.8/file_automation/utils/scheduler/extend_apscheduler.py
+-rw-rw-rw-   0        0        0     1004 2023-06-13 07:19:53.000000 automation_file-0.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-13 07:20:16.851022 automation_file-0.0.8/setup.cfg
```

### Comparing `automation_file-0.0.7/LICENSE` & `automation_file-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `automation_file-0.0.7/PKG-INFO` & `automation_file-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automation_file
-Version: 0.0.7
+Version: 0.0.8
 Author-email: JE-Chen <zenmailman@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/JE-Chen/Integration-testing-environment
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Environment :: MacOS X
```

### Comparing `automation_file-0.0.7/README.md` & `automation_file-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `automation_file-0.0.7/automation_file.egg-info/PKG-INFO` & `automation_file-0.0.8/automation_file.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automation-file
-Version: 0.0.7
+Version: 0.0.8
 Author-email: JE-Chen <zenmailman@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/JE-Chen/Integration-testing-environment
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Environment :: MacOS X
```

### Comparing `automation_file-0.0.7/automation_file.egg-info/SOURCES.txt` & `automation_file-0.0.8/automation_file.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `automation_file-0.0.7/file_automation/__init__.py` & `automation_file-0.0.8/file_automation/__init__.py`

 * *Files identical despite different names*

### Comparing `automation_file-0.0.7/file_automation/local/dir/dir_process.py` & `automation_file-0.0.8/file_automation/local/dir/dir_process.py`

 * *Files identical despite different names*

### Comparing `automation_file-0.0.7/file_automation/local/file/file_process.py` & `automation_file-0.0.8/file_automation/local/file/file_process.py`

 * *Files identical despite different names*

### Comparing `automation_file-0.0.7/file_automation/local/zip/zip_process.py` & `automation_file-0.0.8/file_automation/local/zip/zip_process.py`

 * *Files identical despite different names*

### Comparing `automation_file-0.0.7/file_automation/remote/google_drive/delete/delete_manager.py` & `automation_file-0.0.8/file_automation/remote/google_drive/delete/delete_manager.py`

 * *Files identical despite different names*

### Comparing `automation_file-0.0.7/file_automation/remote/google_drive/dir/folder_manager.py` & `automation_file-0.0.8/file_automation/remote/google_drive/dir/folder_manager.py`

 * *Files identical despite different names*

### Comparing `automation_file-0.0.7/file_automation/remote/google_drive/download/download_file.py` & `automation_file-0.0.8/file_automation/remote/google_drive/download/download_file.py`

 * *Files identical despite different names*

### Comparing `automation_file-0.0.7/file_automation/remote/google_drive/driver_instance.py` & `automation_file-0.0.8/file_automation/remote/google_drive/driver_instance.py`

 * *Files identical despite different names*

### Comparing `automation_file-0.0.7/file_automation/remote/google_drive/search/search_drive.py` & `automation_file-0.0.8/file_automation/remote/google_drive/search/search_drive.py`

 * *Files identical despite different names*

### Comparing `automation_file-0.0.7/file_automation/remote/google_drive/share/share_file.py` & `automation_file-0.0.8/file_automation/remote/google_drive/share/share_file.py`

 * *Files identical despite different names*

### Comparing `automation_file-0.0.7/file_automation/remote/google_drive/upload/upload_to_driver.py` & `automation_file-0.0.8/file_automation/remote/google_drive/upload/upload_to_driver.py`

 * *Files identical despite different names*

### Comparing `automation_file-0.0.7/file_automation/utils/callback/callback_function_executor.py` & `automation_file-0.0.8/file_automation/utils/callback/callback_function_executor.py`

 * *Files identical despite different names*

### Comparing `automation_file-0.0.7/file_automation/utils/exception/exception_tags.py` & `automation_file-0.0.8/file_automation/utils/exception/exception_tags.py`

 * *Files identical despite different names*

### Comparing `automation_file-0.0.7/file_automation/utils/exception/exceptions.py` & `automation_file-0.0.8/file_automation/utils/exception/exceptions.py`

 * *Files identical despite different names*

### Comparing `automation_file-0.0.7/file_automation/utils/executor/action_executor.py` & `automation_file-0.0.8/file_automation/utils/executor/action_executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,14 +107,17 @@
                 execute_record_dict.update({execute_record: event_response})
             except Exception as error:
                 file_automation_logger.error(
                     f"Execute {action} failed. {repr(error)}"
                 )
                 execute_record = "execute: " + str(action)
                 execute_record_dict.update({execute_record: repr(error)})
+        for key, value in execute_record_dict.items():
+            print(key, flush=True)
+            print(value, flush=True)
         return execute_record_dict
 
     def execute_files(self, execute_files_list: list) -> list:
         """
         :param execute_files_list: list include execute files path
         :return: every execute detail as list
         """
```

### Comparing `automation_file-0.0.7/file_automation/utils/json/json_file.py` & `automation_file-0.0.8/file_automation/utils/json/json_file.py`

 * *Files identical despite different names*

### Comparing `automation_file-0.0.7/file_automation/utils/logging/loggin_instance.py` & `automation_file-0.0.8/file_automation/utils/logging/loggin_instance.py`

 * *Files identical despite different names*

### Comparing `automation_file-0.0.7/file_automation/utils/scheduler/extend_apscheduler.py` & `automation_file-0.0.8/file_automation/utils/scheduler/extend_apscheduler.py`

 * *Files identical despite different names*

### Comparing `automation_file-0.0.7/pyproject.toml` & `automation_file-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # This is dev version
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "automation_file"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
     { name = "JE-Chen", email = "zenmailman@gmail.com" },
 ]
 description = ""
 readme = { file = "README.md", content-type = "text/markdown" }
 requires-python = ">=3.8"
 license = { text = "MIT" }
```

