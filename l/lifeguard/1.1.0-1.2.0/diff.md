# Comparing `tmp/lifeguard-1.1.0.tar.gz` & `tmp/lifeguard-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lifeguard-1.1.0.tar", last modified: Fri May 26 13:55:35 2023, max compression
+gzip compressed data, was "lifeguard-1.2.0.tar", last modified: Tue Jun 13 13:06:43 2023, max compression
```

## Comparing `lifeguard-1.1.0.tar` & `lifeguard-1.2.0.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:55:35.184851 lifeguard-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-05-26 13:55:35.184851 lifeguard-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4520 2023-05-26 13:55:24.000000 lifeguard-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:55:35.180851 lifeguard-1.1.0/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2929 2023-05-26 13:55:24.000000 lifeguard-1.1.0/bin/lifeguard
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:55:35.184851 lifeguard-1.1.0/lifeguard/
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-26 13:55:24.000000 lifeguard-1.1.0/lifeguard/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:55:35.184851 lifeguard-1.1.0/lifeguard/actions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:55:24.000000 lifeguard-1.1.0/lifeguard/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-26 13:55:24.000000 lifeguard-1.1.0/lifeguard/actions/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-05-26 13:55:24.000000 lifeguard-1.1.0/lifeguard/actions/email.py
--rw-r--r--   0 runner    (1001) docker     (123)     6248 2023-05-26 13:55:24.000000 lifeguard-1.1.0/lifeguard/actions/notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-26 13:55:24.000000 lifeguard-1.1.0/lifeguard/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-26 13:55:24.000000 lifeguard-1.1.0/lifeguard/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-26 13:55:24.000000 lifeguard-1.1.0/lifeguard/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:55:35.184851 lifeguard-1.1.0/lifeguard/controllers/
--rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-05-26 13:55:24.000000 lifeguard-1.1.0/lifeguard/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-05-26 13:55:24.000000 lifeguard-1.1.0/lifeguard/controllers/assets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-26 13:55:24.000000 lifeguard-1.1.0/lifeguard/http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-05-26 13:55:24.000000 lifeguard-1.1.0/lifeguard/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-05-26 13:55:24.000000 lifeguard-1.1.0/lifeguard/notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-05-26 13:55:24.000000 lifeguard-1.1.0/lifeguard/repositories.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-05-26 13:55:24.000000 lifeguard-1.1.0/lifeguard/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-05-26 13:55:24.000000 lifeguard-1.1.0/lifeguard/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     6810 2023-05-26 13:55:24.000000 lifeguard-1.1.0/lifeguard/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-26 13:55:24.000000 lifeguard-1.1.0/lifeguard/statuses.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-26 13:55:24.000000 lifeguard-1.1.0/lifeguard/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6028 2023-05-26 13:55:24.000000 lifeguard-1.1.0/lifeguard/validations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:55:35.184851 lifeguard-1.1.0/lifeguard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-05-26 13:55:35.000000 lifeguard-1.1.0/lifeguard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-05-26 13:55:35.000000 lifeguard-1.1.0/lifeguard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 13:55:35.000000 lifeguard-1.1.0/lifeguard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-26 13:55:35.000000 lifeguard-1.1.0/lifeguard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-26 13:55:35.000000 lifeguard-1.1.0/lifeguard.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-26 13:55:35.184851 lifeguard-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-26 13:55:24.000000 lifeguard-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:55:35.184851 lifeguard-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:55:24.000000 lifeguard-1.1.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:55:35.184851 lifeguard-1.1.0/tests/actions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:55:24.000000 lifeguard-1.1.0/tests/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-26 13:55:24.000000 lifeguard-1.1.0/tests/actions/test_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     5295 2023-05-26 13:55:24.000000 lifeguard-1.1.0/tests/actions/test_email.py
--rw-r--r--   0 runner    (1001) docker     (123)    15144 2023-05-26 13:55:24.000000 lifeguard-1.1.0/tests/actions/test_notification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:55:35.184851 lifeguard-1.1.0/tests/controllers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:55:24.000000 lifeguard-1.1.0/tests/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-05-26 13:55:24.000000 lifeguard-1.1.0/tests/controllers/test_assets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:55:35.184851 lifeguard-1.1.0/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:55:24.000000 lifeguard-1.1.0/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-26 13:55:24.000000 lifeguard-1.1.0/tests/fixtures/fixtures_repositories.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-26 13:55:24.000000 lifeguard-1.1.0/tests/fixtures/mock_lifeguard_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-05-26 13:55:24.000000 lifeguard-1.1.0/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-26 13:55:24.000000 lifeguard-1.1.0/tests/test_bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)    11566 2023-05-26 13:55:24.000000 lifeguard-1.1.0/tests/test_controllers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-05-26 13:55:24.000000 lifeguard-1.1.0/tests/test_http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-05-26 13:55:24.000000 lifeguard-1.1.0/tests/test_lifeguard_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-26 13:55:24.000000 lifeguard-1.1.0/tests/test_notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-05-26 13:55:24.000000 lifeguard-1.1.0/tests/test_repositories.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-05-26 13:55:24.000000 lifeguard-1.1.0/tests/test_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-05-26 13:55:24.000000 lifeguard-1.1.0/tests/test_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     7064 2023-05-26 13:55:24.000000 lifeguard-1.1.0/tests/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     7160 2023-05-26 13:55:24.000000 lifeguard-1.1.0/tests/test_validations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:06:43.089350 lifeguard-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-06-13 13:06:43.089350 lifeguard-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-06-13 13:06:33.000000 lifeguard-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:06:43.085350 lifeguard-1.2.0/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2929 2023-06-13 13:06:33.000000 lifeguard-1.2.0/bin/lifeguard
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:06:43.085350 lifeguard-1.2.0/lifeguard/
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-06-13 13:06:33.000000 lifeguard-1.2.0/lifeguard/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:06:43.085350 lifeguard-1.2.0/lifeguard/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:06:33.000000 lifeguard-1.2.0/lifeguard/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-13 13:06:33.000000 lifeguard-1.2.0/lifeguard/actions/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-06-13 13:06:33.000000 lifeguard-1.2.0/lifeguard/actions/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6248 2023-06-13 13:06:33.000000 lifeguard-1.2.0/lifeguard/actions/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-06-13 13:06:33.000000 lifeguard-1.2.0/lifeguard/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-13 13:06:33.000000 lifeguard-1.2.0/lifeguard/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-06-13 13:06:33.000000 lifeguard-1.2.0/lifeguard/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:06:43.085350 lifeguard-1.2.0/lifeguard/controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-06-13 13:06:33.000000 lifeguard-1.2.0/lifeguard/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-06-13 13:06:33.000000 lifeguard-1.2.0/lifeguard/controllers/assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-13 13:06:33.000000 lifeguard-1.2.0/lifeguard/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-13 13:06:33.000000 lifeguard-1.2.0/lifeguard/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-06-13 13:06:33.000000 lifeguard-1.2.0/lifeguard/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-06-13 13:06:33.000000 lifeguard-1.2.0/lifeguard/repositories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-06-13 13:06:33.000000 lifeguard-1.2.0/lifeguard/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-06-13 13:06:33.000000 lifeguard-1.2.0/lifeguard/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6810 2023-06-13 13:06:33.000000 lifeguard-1.2.0/lifeguard/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-13 13:06:33.000000 lifeguard-1.2.0/lifeguard/statuses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-13 13:06:33.000000 lifeguard-1.2.0/lifeguard/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6028 2023-06-13 13:06:33.000000 lifeguard-1.2.0/lifeguard/validations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:06:43.085350 lifeguard-1.2.0/lifeguard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-06-13 13:06:43.000000 lifeguard-1.2.0/lifeguard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-13 13:06:43.000000 lifeguard-1.2.0/lifeguard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 13:06:43.000000 lifeguard-1.2.0/lifeguard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-13 13:06:43.000000 lifeguard-1.2.0/lifeguard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-13 13:06:43.000000 lifeguard-1.2.0/lifeguard.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-13 13:06:43.089350 lifeguard-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-13 13:06:33.000000 lifeguard-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:06:43.085350 lifeguard-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:06:33.000000 lifeguard-1.2.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:06:43.085350 lifeguard-1.2.0/tests/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:06:33.000000 lifeguard-1.2.0/tests/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-13 13:06:33.000000 lifeguard-1.2.0/tests/actions/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5295 2023-06-13 13:06:33.000000 lifeguard-1.2.0/tests/actions/test_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15144 2023-06-13 13:06:33.000000 lifeguard-1.2.0/tests/actions/test_notification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:06:43.085350 lifeguard-1.2.0/tests/controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:06:33.000000 lifeguard-1.2.0/tests/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-06-13 13:06:33.000000 lifeguard-1.2.0/tests/controllers/test_assets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:06:43.089350 lifeguard-1.2.0/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:06:33.000000 lifeguard-1.2.0/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-13 13:06:33.000000 lifeguard-1.2.0/tests/fixtures/fixtures_repositories.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-13 13:06:33.000000 lifeguard-1.2.0/tests/fixtures/mock_lifeguard_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-06-13 13:06:33.000000 lifeguard-1.2.0/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-13 13:06:33.000000 lifeguard-1.2.0/tests/test_bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11566 2023-06-13 13:06:33.000000 lifeguard-1.2.0/tests/test_controllers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-06-13 13:06:33.000000 lifeguard-1.2.0/tests/test_http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-13 13:06:33.000000 lifeguard-1.2.0/tests/test_lifeguard_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-06-13 13:06:33.000000 lifeguard-1.2.0/tests/test_notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-06-13 13:06:33.000000 lifeguard-1.2.0/tests/test_repositories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-06-13 13:06:33.000000 lifeguard-1.2.0/tests/test_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6307 2023-06-13 13:06:33.000000 lifeguard-1.2.0/tests/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7064 2023-06-13 13:06:33.000000 lifeguard-1.2.0/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7160 2023-06-13 13:06:33.000000 lifeguard-1.2.0/tests/test_validations.py
```

### Comparing `lifeguard-1.1.0/PKG-INFO` & `lifeguard-1.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lifeguard
-Version: 1.1.0
+Version: 1.2.0
 Summary: Application to monitor your systems and give you the security to sleep peacefully at night
 Home-page: https://github.com/LifeguardSystem/lifeguard
 Author: Diego Rubin
 Author-email: contact@diegorubin.dev
 License: GPL2
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -48,18 +48,18 @@
 
 ### Create a validation
 
 To create a validation you should create a file into `validations` directory. The file should ends with `_validation.py`.
 Example:
 
 ```python
-import requests
 from lifeguard import NORMAL, PROBLEM, change_status
 from lifeguard.actions.database import save_result_into_database
 from lifeguard.actions.notifications import notify_in_single_message
+from lifeguard.http_client import get
 from lifeguard.logger import lifeguard_logger as logger
 from lifeguard.validations import ValidationResponse, validation
 
 
 @validation(
     "check if pudim is alive",
     actions=[save_result_into_database, notify_in_single_message],
@@ -70,18 +70,16 @@
     result = requests.get("http://pudim.com.br")
     logger.info("pudim status code: %s", result.status_code)
 
     if result.status_code != 200:
         status = change_status(status, PROBLEM)
 
     return ValidationResponse(
-        "pudim_is_alive",
-        NORMAL,
+        status,
         {status: result.status_code},
-        {"notification": {"notify": True}},
     )
 ```
 
 ### Validation Actions
 
 Action is a simple python function with only 2 arguments: a validation response and a dict called settings. These settings are the parameter called settings in validation.
```

### Comparing `lifeguard-1.1.0/README.md` & `lifeguard-1.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -32,18 +32,18 @@
 
 ### Create a validation
 
 To create a validation you should create a file into `validations` directory. The file should ends with `_validation.py`.
 Example:
 
 ```python
-import requests
 from lifeguard import NORMAL, PROBLEM, change_status
 from lifeguard.actions.database import save_result_into_database
 from lifeguard.actions.notifications import notify_in_single_message
+from lifeguard.http_client import get
 from lifeguard.logger import lifeguard_logger as logger
 from lifeguard.validations import ValidationResponse, validation
 
 
 @validation(
     "check if pudim is alive",
     actions=[save_result_into_database, notify_in_single_message],
@@ -54,18 +54,16 @@
     result = requests.get("http://pudim.com.br")
     logger.info("pudim status code: %s", result.status_code)
 
     if result.status_code != 200:
         status = change_status(status, PROBLEM)
 
     return ValidationResponse(
-        "pudim_is_alive",
-        NORMAL,
+        status,
         {status: result.status_code},
-        {"notification": {"notify": True}},
     )
 ```
 
 ### Validation Actions
 
 Action is a simple python function with only 2 arguments: a validation response and a dict called settings. These settings are the parameter called settings in validation.
```

### Comparing `lifeguard-1.1.0/bin/lifeguard` & `lifeguard-1.2.0/bin/lifeguard`

 * *Files identical despite different names*

### Comparing `lifeguard-1.1.0/lifeguard/__init__.py` & `lifeguard-1.2.0/lifeguard/__init__.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.1.0/lifeguard/actions/email.py` & `lifeguard-1.2.0/lifeguard/actions/email.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.1.0/lifeguard/actions/notifications.py` & `lifeguard-1.2.0/lifeguard/actions/notifications.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.1.0/lifeguard/auth.py` & `lifeguard-1.2.0/lifeguard/auth.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.1.0/lifeguard/context.py` & `lifeguard-1.2.0/lifeguard/context.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.1.0/lifeguard/controllers/__init__.py` & `lifeguard-1.2.0/lifeguard/controllers/__init__.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.1.0/lifeguard/controllers/assets.py` & `lifeguard-1.2.0/lifeguard/controllers/assets.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.1.0/lifeguard/http_client.py` & `lifeguard-1.2.0/lifeguard/http_client.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.1.0/lifeguard/logger.py` & `lifeguard-1.2.0/lifeguard/logger.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.1.0/lifeguard/notifications.py` & `lifeguard-1.2.0/lifeguard/notifications.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.1.0/lifeguard/repositories.py` & `lifeguard-1.2.0/lifeguard/repositories.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,19 @@
 
     def fetch_last_validation_result(self, validation_name):
         return self.__implementation__.fetch_last_validation_result(validation_name)
 
     def fetch_all_validation_results(self):
         return self.__implementation__.fetch_all_validation_results()
 
+    def delete_validation_result(self, validation_name):
+        if hasattr(self.__implementation__, "delete_validation_result"):
+            return self.__implementation__.delete_validation_result(validation_name)
+        logger.warn("delete_validation_result not implemented")
+
 
 class NotificationRepository(BaseRepository):
     def __init__(self):
         BaseRepository.__init_repository__(self, "notification")
 
     def save_last_notification_for_a_validation(self, notification):
         self.__implementation__.save_last_notification_for_a_validation(notification)
```

### Comparing `lifeguard-1.1.0/lifeguard/scheduler.py` & `lifeguard-1.2.0/lifeguard/scheduler.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.1.0/lifeguard/server.py` & `lifeguard-1.2.0/lifeguard/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import traceback
 from datetime import datetime, timedelta
 
 from flask import Flask, make_response
 
 from lifeguard import NORMAL, change_status
-from lifeguard.controllers import custom_controllers, login_required
+from lifeguard.controllers import custom_controllers, login_required, request
 from lifeguard.logger import lifeguard_logger as logger
 from lifeguard.repositories import ValidationRepository
 from lifeguard.settings import LIFEGUARD_SECRET_KEY, PERMANENT_SESSION_LIFETIME
 from lifeguard.validations import VALIDATIONS, ValidationResponseEncoder
 
 APP = Flask(__name__)
 APP.secret_key = LIFEGUARD_SECRET_KEY
@@ -59,18 +59,22 @@
 def get_status_complete():
     """
     Return global status with details
     """
     return build_global_status(True)
 
 
-@APP.route("/lifeguard/validations/<validation>", methods=["GET"])
+@APP.route("/lifeguard/validations/<validation>", methods=["GET", "DELETE"])
 @login_required
-def get_validation(validation):
+def validation_endpoint(validation):
     repository = ValidationRepository()
+    if request.method == "DELETE":
+        repository.delete_validation_result(validation)
+        return make_json_response(json.dumps({"status": "ok"}))
+
     result = repository.fetch_last_validation_result(validation)
     return make_json_response(ValidationResponseEncoder().encode(result))
 
 
 @APP.route("/lifeguard/validations/<validation>/execute", methods=["POST"])
 @login_required
 def execute_validation(validation):
```

### Comparing `lifeguard-1.1.0/lifeguard/settings.py` & `lifeguard-1.2.0/lifeguard/settings.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.1.0/lifeguard/validations.py` & `lifeguard-1.2.0/lifeguard/validations.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.1.0/lifeguard.egg-info/PKG-INFO` & `lifeguard-1.2.0/lifeguard.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lifeguard
-Version: 1.1.0
+Version: 1.2.0
 Summary: Application to monitor your systems and give you the security to sleep peacefully at night
 Home-page: https://github.com/LifeguardSystem/lifeguard
 Author: Diego Rubin
 Author-email: contact@diegorubin.dev
 License: GPL2
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -48,18 +48,18 @@
 
 ### Create a validation
 
 To create a validation you should create a file into `validations` directory. The file should ends with `_validation.py`.
 Example:
 
 ```python
-import requests
 from lifeguard import NORMAL, PROBLEM, change_status
 from lifeguard.actions.database import save_result_into_database
 from lifeguard.actions.notifications import notify_in_single_message
+from lifeguard.http_client import get
 from lifeguard.logger import lifeguard_logger as logger
 from lifeguard.validations import ValidationResponse, validation
 
 
 @validation(
     "check if pudim is alive",
     actions=[save_result_into_database, notify_in_single_message],
@@ -70,18 +70,16 @@
     result = requests.get("http://pudim.com.br")
     logger.info("pudim status code: %s", result.status_code)
 
     if result.status_code != 200:
         status = change_status(status, PROBLEM)
 
     return ValidationResponse(
-        "pudim_is_alive",
-        NORMAL,
+        status,
         {status: result.status_code},
-        {"notification": {"notify": True}},
     )
 ```
 
 ### Validation Actions
 
 Action is a simple python function with only 2 arguments: a validation response and a dict called settings. These settings are the parameter called settings in validation.
```

### Comparing `lifeguard-1.1.0/lifeguard.egg-info/SOURCES.txt` & `lifeguard-1.2.0/lifeguard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lifeguard-1.1.0/setup.py` & `lifeguard-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="lifeguard",
-    version="1.1.0",
+    version="1.2.0",
     url="https://github.com/LifeguardSystem/lifeguard",
     author="Diego Rubin",
     author_email="contact@diegorubin.dev",
     license="GPL2",
     scripts=["bin/lifeguard"],
     include_package_data=True,
     description="Application to monitor your systems and give you the security to sleep peacefully at night",
```

### Comparing `lifeguard-1.1.0/tests/actions/test_database.py` & `lifeguard-1.2.0/tests/actions/test_database.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.1.0/tests/actions/test_email.py` & `lifeguard-1.2.0/tests/actions/test_email.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.1.0/tests/actions/test_notification.py` & `lifeguard-1.2.0/tests/actions/test_notification.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.1.0/tests/controllers/test_assets.py` & `lifeguard-1.2.0/tests/controllers/test_assets.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.1.0/tests/test_auth.py` & `lifeguard-1.2.0/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.1.0/tests/test_bootstrap.py` & `lifeguard-1.2.0/tests/test_bootstrap.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.1.0/tests/test_controllers.py` & `lifeguard-1.2.0/tests/test_controllers.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.1.0/tests/test_http_client.py` & `lifeguard-1.2.0/tests/test_http_client.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.1.0/tests/test_lifeguard_core.py` & `lifeguard-1.2.0/tests/test_lifeguard_core.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.1.0/tests/test_notifications.py` & `lifeguard-1.2.0/tests/test_notifications.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.1.0/tests/test_repositories.py` & `lifeguard-1.2.0/tests/test_repositories.py`

 * *Files 5% similar despite different names*

```diff
@@ -124,14 +124,19 @@
             validation_name
         )
 
     def test_validation_repository_fetch_all_validation_results(self):
         self.validation_repository.fetch_all_validation_results()
         self.implementation.fetch_all_validation_results.assert_called()
 
+    def test_validation_repository_delete_validation_result(self):
+        validation_name = MagicMock(name="validation_name")
+        self.validation_repository.delete_validation_result(validation_name)
+        self.implementation.delete_validation_result(validation_name)
+
 
 class TestRepositoriesFunctions(unittest.TestCase):
     def setUp(self):
         if "test" in IMPLEMENTATIONS:
             IMPLEMENTATIONS.pop("test")
         self.implementation = MagicMock(name="implementation")
         self.implementation.__name__ = "test"
```

### Comparing `lifeguard-1.1.0/tests/test_scheduler.py` & `lifeguard-1.2.0/tests/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.1.0/tests/test_server.py` & `lifeguard-1.2.0/tests/test_server.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import unittest
 from unittest.mock import MagicMock, patch
 
 from lifeguard import NORMAL, PROBLEM
 from lifeguard.server import (
     execute_validation,
-    get_validation,
+    validation_endpoint,
     get_status,
     get_status_complete,
 )
 from lifeguard.validations import ValidationResponse
 
 test_validation = MagicMock(name="test_validation")
 test_validation.return_value = ValidationResponse(NORMAL, {})
@@ -43,31 +43,50 @@
             "error on execute validation %s",
             "test_validation",
             extra={"traceback": "traceback"},
         )
 
     @patch("lifeguard.server.make_response")
     @patch("lifeguard.server.ValidationRepository")
-    def test_get_validation_result(
-        self, mock_validation_repository, mock_make_response
+    @patch("lifeguard.server.request")
+    def test_validation_endpoint_get_result(
+        self, mock_request, mock_validation_repository, mock_make_response
     ):
+        mock_request.method = "GET"
         mock_response = MagicMock(name="mock_response")
         mock_make_response.return_value = mock_response
 
         mock_repository_instance = MagicMock(name="mock_repository_instance")
         mock_validation_repository.return_value = mock_repository_instance
         mock_repository_instance.fetch_last_validation_result.return_value = (
             ValidationResponse(NORMAL, {})
         )
 
-        response = get_validation("test_validation")
+        response = validation_endpoint("test_validation")
         self.assertEqual(response, mock_response)
 
     @patch("lifeguard.server.make_response")
     @patch("lifeguard.server.ValidationRepository")
+    @patch("lifeguard.server.request")
+    def test_validation_endpoint_delete_result(
+        self, mock_request, mock_validation_repository, mock_make_response
+    ):
+        mock_request.method = "DELETE"
+
+        mock_repository_instance = MagicMock(name="mock_repository_instance")
+        mock_validation_repository.return_value = mock_repository_instance
+
+        validation_endpoint("test_validation")
+        mock_make_response.assert_called_with('{"status": "ok"}')
+        mock_repository_instance.delete_validation_result.assert_called_with(
+            "test_validation"
+        )
+
+    @patch("lifeguard.server.make_response")
+    @patch("lifeguard.server.ValidationRepository")
     def test_get_status(self, mock_validation_repository, mock_make_response):
         mock_response = MagicMock(name="mock_response")
         mock_make_response.return_value = mock_response
 
         mock_repository_instance = MagicMock(name="mock_repository_instance")
         mock_validation_repository.return_value = mock_repository_instance
         mock_repository_instance.fetch_all_validation_results.return_value = [
```

### Comparing `lifeguard-1.1.0/tests/test_settings.py` & `lifeguard-1.2.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `lifeguard-1.1.0/tests/test_validations.py` & `lifeguard-1.2.0/tests/test_validations.py`

 * *Files identical despite different names*

