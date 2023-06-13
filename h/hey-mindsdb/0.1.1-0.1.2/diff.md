# Comparing `tmp/hey_mindsdb-0.1.1.tar.gz` & `tmp/hey_mindsdb-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hey_mindsdb-0.1.1.tar", last modified: Mon May 29 09:54:44 2023, max compression
+gzip compressed data, was "hey_mindsdb-0.1.2.tar", last modified: Tue Jun 13 11:53:27 2023, max compression
```

## Comparing `hey_mindsdb-0.1.1.tar` & `hey_mindsdb-0.1.2.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 sadra      (501) staff       (20)        0 2023-05-29 09:54:44.635686 hey_mindsdb-0.1.1/
--rw-r--r--   0 sadra      (501) staff       (20)     1074 2023-04-18 07:11:57.000000 hey_mindsdb-0.1.1/LICENSE
--rw-r--r--   0 sadra      (501) staff       (20)      196 2023-04-22 18:25:34.000000 hey_mindsdb-0.1.1/MANIFEST.in
--rw-r--r--   0 sadra      (501) staff       (20)     4858 2023-05-29 09:54:44.635776 hey_mindsdb-0.1.1/PKG-INFO
--rw-r--r--   0 sadra      (501) staff       (20)     3969 2023-05-29 09:48:55.000000 hey_mindsdb-0.1.1/README.md
-drwxr-xr-x   0 sadra      (501) staff       (20)        0 2023-05-29 09:54:44.631824 hey_mindsdb-0.1.1/hey/
--rw-r--r--   0 sadra      (501) staff       (20)      126 2023-05-29 09:48:55.000000 hey_mindsdb-0.1.1/hey/__init__.py
--rw-r--r--   0 sadra      (501) staff       (20)     2841 2023-05-29 09:48:55.000000 hey_mindsdb-0.1.1/hey/cli.py
-drwxr-xr-x   0 sadra      (501) staff       (20)        0 2023-05-29 09:54:44.632269 hey_mindsdb-0.1.1/hey/constants/
--rw-r--r--   0 sadra      (501) staff       (20)        0 2023-04-18 09:52:09.000000 hey_mindsdb-0.1.1/hey/constants/__init__.py
--rw-r--r--   0 sadra      (501) staff       (20)      550 2023-04-23 16:07:39.000000 hey_mindsdb-0.1.1/hey/constants/informations.py
--rw-r--r--   0 sadra      (501) staff       (20)      130 2023-05-07 16:48:50.000000 hey_mindsdb-0.1.1/hey/constants/service.py
--rw-r--r--   0 sadra      (501) staff       (20)      110 2023-04-22 12:11:15.000000 hey_mindsdb-0.1.1/hey/constants/system.py
-drwxr-xr-x   0 sadra      (501) staff       (20)        0 2023-05-29 09:54:44.632703 hey_mindsdb-0.1.1/hey/exceptions/
--rw-r--r--   0 sadra      (501) staff       (20)        0 2023-04-18 14:10:13.000000 hey_mindsdb-0.1.1/hey/exceptions/__init__.py
--rw-r--r--   0 sadra      (501) staff       (20)      105 2023-04-22 08:03:57.000000 hey_mindsdb-0.1.1/hey/exceptions/auth.py
--rw-r--r--   0 sadra      (501) staff       (20)       83 2023-04-22 08:04:02.000000 hey_mindsdb-0.1.1/hey/exceptions/connection.py
--rw-r--r--   0 sadra      (501) staff       (20)      221 2023-04-22 12:18:05.000000 hey_mindsdb-0.1.1/hey/exceptions/system.py
-drwxr-xr-x   0 sadra      (501) staff       (20)        0 2023-05-29 09:54:44.632919 hey_mindsdb-0.1.1/hey/middlewares/
--rw-r--r--   0 sadra      (501) staff       (20)        0 2023-04-18 13:04:22.000000 hey_mindsdb-0.1.1/hey/middlewares/__init__.py
--rw-r--r--   0 sadra      (501) staff       (20)     2564 2023-05-22 09:08:57.000000 hey_mindsdb-0.1.1/hey/middlewares/mindsdb.py
-drwxr-xr-x   0 sadra      (501) staff       (20)        0 2023-05-29 09:54:44.633172 hey_mindsdb-0.1.1/hey/templates/
--rw-r--r--   0 sadra      (501) staff       (20)        0 2023-04-24 06:30:05.000000 hey_mindsdb-0.1.1/hey/templates/__init__.py
--rw-r--r--   0 sadra      (501) staff       (20)      153 2023-04-24 07:25:14.000000 hey_mindsdb-0.1.1/hey/templates/mindsdb_queries.py
-drwxr-xr-x   0 sadra      (501) staff       (20)        0 2023-05-29 09:54:44.634213 hey_mindsdb-0.1.1/hey_mindsdb.egg-info/
--rw-r--r--   0 sadra      (501) staff       (20)     4858 2023-05-29 09:54:44.000000 hey_mindsdb-0.1.1/hey_mindsdb.egg-info/PKG-INFO
--rw-r--r--   0 sadra      (501) staff       (20)      962 2023-05-29 09:54:44.000000 hey_mindsdb-0.1.1/hey_mindsdb.egg-info/SOURCES.txt
--rw-r--r--   0 sadra      (501) staff       (20)        1 2023-05-29 09:54:44.000000 hey_mindsdb-0.1.1/hey_mindsdb.egg-info/dependency_links.txt
--rw-r--r--   0 sadra      (501) staff       (20)       37 2023-05-29 09:54:44.000000 hey_mindsdb-0.1.1/hey_mindsdb.egg-info/entry_points.txt
--rw-r--r--   0 sadra      (501) staff       (20)        1 2023-04-22 16:08:14.000000 hey_mindsdb-0.1.1/hey_mindsdb.egg-info/not-zip-safe
--rw-r--r--   0 sadra      (501) staff       (20)       49 2023-05-29 09:54:44.000000 hey_mindsdb-0.1.1/hey_mindsdb.egg-info/requires.txt
--rw-r--r--   0 sadra      (501) staff       (20)        4 2023-05-29 09:54:44.000000 hey_mindsdb-0.1.1/hey_mindsdb.egg-info/top_level.txt
--rw-r--r--   0 sadra      (501) staff       (20)     1440 2023-05-29 09:54:44.636203 hey_mindsdb-0.1.1/setup.cfg
--rw-r--r--   0 sadra      (501) staff       (20)       37 2023-04-21 19:28:33.000000 hey_mindsdb-0.1.1/setup.py
-drwxr-xr-x   0 sadra      (501) staff       (20)        0 2023-05-29 09:54:44.634555 hey_mindsdb-0.1.1/tests/
--rw-r--r--   0 sadra      (501) staff       (20)       33 2023-04-18 07:11:58.000000 hey_mindsdb-0.1.1/tests/__init__.py
-drwxr-xr-x   0 sadra      (501) staff       (20)        0 2023-05-29 09:54:44.634958 hey_mindsdb-0.1.1/tests/exceptions/
--rw-r--r--   0 sadra      (501) staff       (20)        0 2023-05-07 10:56:13.000000 hey_mindsdb-0.1.1/tests/exceptions/__init__.py
--rw-r--r--   0 sadra      (501) staff       (20)      194 2023-05-07 10:56:13.000000 hey_mindsdb-0.1.1/tests/exceptions/test_auth.py
--rw-r--r--   0 sadra      (501) staff       (20)      178 2023-05-07 10:56:13.000000 hey_mindsdb-0.1.1/tests/exceptions/test_connection.py
--rw-r--r--   0 sadra      (501) staff       (20)      589 2023-05-07 10:56:13.000000 hey_mindsdb-0.1.1/tests/exceptions/test_system.py
-drwxr-xr-x   0 sadra      (501) staff       (20)        0 2023-05-29 09:54:44.635214 hey_mindsdb-0.1.1/tests/middlewares/
--rw-r--r--   0 sadra      (501) staff       (20)        0 2023-05-07 10:56:13.000000 hey_mindsdb-0.1.1/tests/middlewares/__init__.py
--rw-r--r--   0 sadra      (501) staff       (20)     1700 2023-05-07 10:56:13.000000 hey_mindsdb-0.1.1/tests/middlewares/test_mindsdb.py
-drwxr-xr-x   0 sadra      (501) staff       (20)        0 2023-05-29 09:54:44.635575 hey_mindsdb-0.1.1/tests/templates/
--rw-r--r--   0 sadra      (501) staff       (20)        0 2023-05-07 10:56:13.000000 hey_mindsdb-0.1.1/tests/templates/__init__.py
--rw-r--r--   0 sadra      (501) staff       (20)      542 2023-05-07 10:56:13.000000 hey_mindsdb-0.1.1/tests/templates/test_mindsdb_queries.py
--rw-r--r--   0 sadra      (501) staff       (20)      166 2023-04-22 15:27:42.000000 hey_mindsdb-0.1.1/tests/test_accounts.py
--rw-r--r--   0 sadra      (501) staff       (20)      249 2023-05-29 09:48:55.000000 hey_mindsdb-0.1.1/tests/test_cli.py
+drwxr-xr-x   0 sadra      (501) staff       (20)        0 2023-06-13 11:53:27.612456 hey_mindsdb-0.1.2/
+-rw-r--r--   0 sadra      (501) staff       (20)     1074 2023-04-18 07:11:57.000000 hey_mindsdb-0.1.2/LICENSE
+-rw-r--r--   0 sadra      (501) staff       (20)      196 2023-04-22 18:25:34.000000 hey_mindsdb-0.1.2/MANIFEST.in
+-rw-r--r--   0 sadra      (501) staff       (20)     4858 2023-06-13 11:53:27.612515 hey_mindsdb-0.1.2/PKG-INFO
+-rw-r--r--   0 sadra      (501) staff       (20)     3969 2023-05-29 09:48:55.000000 hey_mindsdb-0.1.2/README.md
+drwxr-xr-x   0 sadra      (501) staff       (20)        0 2023-06-13 11:53:27.607407 hey_mindsdb-0.1.2/hey/
+-rw-r--r--   0 sadra      (501) staff       (20)      126 2023-06-13 11:52:48.000000 hey_mindsdb-0.1.2/hey/__init__.py
+-rw-r--r--   0 sadra      (501) staff       (20)     3013 2023-05-31 10:45:47.000000 hey_mindsdb-0.1.2/hey/cli.py
+drwxr-xr-x   0 sadra      (501) staff       (20)        0 2023-06-13 11:53:27.608214 hey_mindsdb-0.1.2/hey/constants/
+-rw-r--r--   0 sadra      (501) staff       (20)        0 2023-04-18 09:52:09.000000 hey_mindsdb-0.1.2/hey/constants/__init__.py
+-rw-r--r--   0 sadra      (501) staff       (20)      550 2023-04-23 16:07:39.000000 hey_mindsdb-0.1.2/hey/constants/informations.py
+-rw-r--r--   0 sadra      (501) staff       (20)      130 2023-05-07 16:48:50.000000 hey_mindsdb-0.1.2/hey/constants/service.py
+-rw-r--r--   0 sadra      (501) staff       (20)      110 2023-04-22 12:11:15.000000 hey_mindsdb-0.1.2/hey/constants/system.py
+drwxr-xr-x   0 sadra      (501) staff       (20)        0 2023-06-13 11:53:27.608967 hey_mindsdb-0.1.2/hey/exceptions/
+-rw-r--r--   0 sadra      (501) staff       (20)        0 2023-04-18 14:10:13.000000 hey_mindsdb-0.1.2/hey/exceptions/__init__.py
+-rw-r--r--   0 sadra      (501) staff       (20)      105 2023-04-22 08:03:57.000000 hey_mindsdb-0.1.2/hey/exceptions/auth.py
+-rw-r--r--   0 sadra      (501) staff       (20)       83 2023-04-22 08:04:02.000000 hey_mindsdb-0.1.2/hey/exceptions/connection.py
+-rw-r--r--   0 sadra      (501) staff       (20)      221 2023-04-22 12:18:05.000000 hey_mindsdb-0.1.2/hey/exceptions/system.py
+drwxr-xr-x   0 sadra      (501) staff       (20)        0 2023-06-13 11:53:27.609297 hey_mindsdb-0.1.2/hey/middlewares/
+-rw-r--r--   0 sadra      (501) staff       (20)        0 2023-04-18 13:04:22.000000 hey_mindsdb-0.1.2/hey/middlewares/__init__.py
+-rw-r--r--   0 sadra      (501) staff       (20)     2564 2023-05-22 09:08:57.000000 hey_mindsdb-0.1.2/hey/middlewares/mindsdb.py
+drwxr-xr-x   0 sadra      (501) staff       (20)        0 2023-06-13 11:53:27.609610 hey_mindsdb-0.1.2/hey/templates/
+-rw-r--r--   0 sadra      (501) staff       (20)        0 2023-04-24 06:30:05.000000 hey_mindsdb-0.1.2/hey/templates/__init__.py
+-rw-r--r--   0 sadra      (501) staff       (20)      153 2023-04-24 07:25:14.000000 hey_mindsdb-0.1.2/hey/templates/mindsdb_queries.py
+drwxr-xr-x   0 sadra      (501) staff       (20)        0 2023-06-13 11:53:27.610557 hey_mindsdb-0.1.2/hey_mindsdb.egg-info/
+-rw-r--r--   0 sadra      (501) staff       (20)     4858 2023-06-13 11:53:27.000000 hey_mindsdb-0.1.2/hey_mindsdb.egg-info/PKG-INFO
+-rw-r--r--   0 sadra      (501) staff       (20)      962 2023-06-13 11:53:27.000000 hey_mindsdb-0.1.2/hey_mindsdb.egg-info/SOURCES.txt
+-rw-r--r--   0 sadra      (501) staff       (20)        1 2023-06-13 11:53:27.000000 hey_mindsdb-0.1.2/hey_mindsdb.egg-info/dependency_links.txt
+-rw-r--r--   0 sadra      (501) staff       (20)       37 2023-06-13 11:53:27.000000 hey_mindsdb-0.1.2/hey_mindsdb.egg-info/entry_points.txt
+-rw-r--r--   0 sadra      (501) staff       (20)        1 2023-04-22 16:08:14.000000 hey_mindsdb-0.1.2/hey_mindsdb.egg-info/not-zip-safe
+-rw-r--r--   0 sadra      (501) staff       (20)       49 2023-06-13 11:53:27.000000 hey_mindsdb-0.1.2/hey_mindsdb.egg-info/requires.txt
+-rw-r--r--   0 sadra      (501) staff       (20)        4 2023-06-13 11:53:27.000000 hey_mindsdb-0.1.2/hey_mindsdb.egg-info/top_level.txt
+-rw-r--r--   0 sadra      (501) staff       (20)     1440 2023-06-13 11:53:27.612792 hey_mindsdb-0.1.2/setup.cfg
+-rw-r--r--   0 sadra      (501) staff       (20)       37 2023-04-21 19:28:33.000000 hey_mindsdb-0.1.2/setup.py
+drwxr-xr-x   0 sadra      (501) staff       (20)        0 2023-06-13 11:53:27.611106 hey_mindsdb-0.1.2/tests/
+-rw-r--r--   0 sadra      (501) staff       (20)       33 2023-04-18 07:11:58.000000 hey_mindsdb-0.1.2/tests/__init__.py
+drwxr-xr-x   0 sadra      (501) staff       (20)        0 2023-06-13 11:53:27.611862 hey_mindsdb-0.1.2/tests/exceptions/
+-rw-r--r--   0 sadra      (501) staff       (20)        0 2023-05-07 10:56:13.000000 hey_mindsdb-0.1.2/tests/exceptions/__init__.py
+-rw-r--r--   0 sadra      (501) staff       (20)      194 2023-05-07 10:56:13.000000 hey_mindsdb-0.1.2/tests/exceptions/test_auth.py
+-rw-r--r--   0 sadra      (501) staff       (20)      178 2023-05-07 10:56:13.000000 hey_mindsdb-0.1.2/tests/exceptions/test_connection.py
+-rw-r--r--   0 sadra      (501) staff       (20)      589 2023-05-07 10:56:13.000000 hey_mindsdb-0.1.2/tests/exceptions/test_system.py
+drwxr-xr-x   0 sadra      (501) staff       (20)        0 2023-06-13 11:53:27.612103 hey_mindsdb-0.1.2/tests/middlewares/
+-rw-r--r--   0 sadra      (501) staff       (20)        0 2023-05-07 10:56:13.000000 hey_mindsdb-0.1.2/tests/middlewares/__init__.py
+-rw-r--r--   0 sadra      (501) staff       (20)     1700 2023-05-07 10:56:13.000000 hey_mindsdb-0.1.2/tests/middlewares/test_mindsdb.py
+drwxr-xr-x   0 sadra      (501) staff       (20)        0 2023-06-13 11:53:27.612333 hey_mindsdb-0.1.2/tests/templates/
+-rw-r--r--   0 sadra      (501) staff       (20)        0 2023-05-07 10:56:13.000000 hey_mindsdb-0.1.2/tests/templates/__init__.py
+-rw-r--r--   0 sadra      (501) staff       (20)      542 2023-05-07 10:56:13.000000 hey_mindsdb-0.1.2/tests/templates/test_mindsdb_queries.py
+-rw-r--r--   0 sadra      (501) staff       (20)      166 2023-04-22 15:27:42.000000 hey_mindsdb-0.1.2/tests/test_accounts.py
+-rw-r--r--   0 sadra      (501) staff       (20)      249 2023-05-29 09:48:55.000000 hey_mindsdb-0.1.2/tests/test_cli.py
```

### Comparing `hey_mindsdb-0.1.1/LICENSE` & `hey_mindsdb-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hey_mindsdb-0.1.1/PKG-INFO` & `hey_mindsdb-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hey_mindsdb
-Version: 0.1.1
+Version: 0.1.2
 Summary: Your AI-powered pair programming friend.
 Home-page: https://github.com/lnxpy/hey
 Author: Sadra Yahyapour
 Author-email: lnxpylnxpy@gmail.com
 License: MIT
 Keywords: hey
 Classifier: Development Status :: 4 - Beta
```

### Comparing `hey_mindsdb-0.1.1/README.md` & `hey_mindsdb-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `hey_mindsdb-0.1.1/hey/cli.py` & `hey_mindsdb-0.1.2/hey/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,18 +3,23 @@
 import sys
 from getpass import getpass
 
 import keyring
 from rich.console import Console
 
 from hey import __version__
-from hey.constants.informations import APPLICATION_DESCRIPTION, EPILOG_DESCRIPTION, INSTALLATION_GUIDE, VERSION_INFO
+from hey.constants.informations import APPLICATION_DESCRIPTION
+from hey.constants.informations import EPILOG_DESCRIPTION
+from hey.constants.informations import INSTALLATION_GUIDE
+from hey.constants.informations import VERSION_INFO
 from hey.constants.service import SERVICE_NAME
 from hey.constants.system import LOCAL_EMAIL_ADDRESS_VARIABLE_NAME
-from hey.exceptions.system import BrokenCredentials, EmailEnvVarNotExists, KeyringIssue
+from hey.exceptions.system import BrokenCredentials
+from hey.exceptions.system import EmailEnvVarNotExists
+from hey.exceptions.system import KeyringIssue
 from hey.middlewares.mindsdb import MindsDB
 
 parser = argparse.ArgumentParser(
     description=APPLICATION_DESCRIPTION + '\n\r\n\r' + INSTALLATION_GUIDE,
     epilog=EPILOG_DESCRIPTION,
     formatter_class=argparse.RawDescriptionHelpFormatter,
 )
@@ -65,15 +70,15 @@
     credentials = keyring.get_credential(
         service_name=SERVICE_NAME.lower(),
         username=os.environ.get(LOCAL_EMAIL_ADDRESS_VARIABLE_NAME),
     )
 
     if not credentials:
         raise BrokenCredentials(
-            f'Make sure you have set your {LOCAL_EMAIL_ADDRESS_VARIABLE_NAME} and password via --set-password.'
+            f'Make sure you have set your {LOCAL_EMAIL_ADDRESS_VARIABLE_NAME} and password via --auth.'
         )
 
     if args.ask:
         with console.status('Creating instance..'):
             instance = MindsDB(
                 email=credentials.username,
                 password=credentials.password
```

### Comparing `hey_mindsdb-0.1.1/hey/constants/informations.py` & `hey_mindsdb-0.1.2/hey/constants/informations.py`

 * *Files identical despite different names*

### Comparing `hey_mindsdb-0.1.1/hey/middlewares/mindsdb.py` & `hey_mindsdb-0.1.2/hey/middlewares/mindsdb.py`

 * *Files identical despite different names*

### Comparing `hey_mindsdb-0.1.1/hey_mindsdb.egg-info/PKG-INFO` & `hey_mindsdb-0.1.2/hey_mindsdb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hey-mindsdb
-Version: 0.1.1
+Version: 0.1.2
 Summary: Your AI-powered pair programming friend.
 Home-page: https://github.com/lnxpy/hey
 Author: Sadra Yahyapour
 Author-email: lnxpylnxpy@gmail.com
 License: MIT
 Keywords: hey
 Classifier: Development Status :: 4 - Beta
```

### Comparing `hey_mindsdb-0.1.1/hey_mindsdb.egg-info/SOURCES.txt` & `hey_mindsdb-0.1.2/hey_mindsdb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hey_mindsdb-0.1.1/setup.cfg` & `hey_mindsdb-0.1.2/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = hey_mindsdb
-version = 0.1.1
+version = 0.1.2
 description = Your AI-powered pair programming friend.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/lnxpy/hey
 author = Sadra Yahyapour
 author_email = lnxpylnxpy@gmail.com
 license = MIT
@@ -40,15 +40,15 @@
 	hey.*
 
 [options.entry_points]
 console_scripts = 
 	hey=hey.cli:main
 
 [bumpversion]
-current_version = 0.1.1
+current_version = 0.1.2
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = version='{current_version}'
 replace = version='{new_version}'
```

### Comparing `hey_mindsdb-0.1.1/tests/exceptions/test_system.py` & `hey_mindsdb-0.1.2/tests/exceptions/test_system.py`

 * *Files identical despite different names*

### Comparing `hey_mindsdb-0.1.1/tests/middlewares/test_mindsdb.py` & `hey_mindsdb-0.1.2/tests/middlewares/test_mindsdb.py`

 * *Files identical despite different names*

### Comparing `hey_mindsdb-0.1.1/tests/templates/test_mindsdb_queries.py` & `hey_mindsdb-0.1.2/tests/templates/test_mindsdb_queries.py`

 * *Files identical despite different names*

