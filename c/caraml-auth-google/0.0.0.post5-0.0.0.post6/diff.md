# Comparing `tmp/caraml-auth-google-0.0.0.post5.tar.gz` & `tmp/caraml-auth-google-0.0.0.post6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/caraml-auth-google-0.0.0.post5.tar", last modified: Tue Jun  6 07:02:37 2023, max compression
+gzip compressed data, was "dist/caraml-auth-google-0.0.0.post6.tar", last modified: Tue Jun 13 07:52:25 2023, max compression
```

## Comparing `caraml-auth-google-0.0.0.post5.tar` & `caraml-auth-google-0.0.0.post6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:02:37.000000 caraml-auth-google-0.0.0.post5/
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-06 07:02:37.000000 caraml-auth-google-0.0.0.post5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-06 07:02:21.000000 caraml-auth-google-0.0.0.post5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:02:37.000000 caraml-auth-google-0.0.0.post5/caraml_auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 07:02:21.000000 caraml-auth-google-0.0.0.post5/caraml_auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8610 2023-06-06 07:02:21.000000 caraml-auth-google-0.0.0.post5/caraml_auth/id_token_credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:02:37.000000 caraml-auth-google-0.0.0.post5/caraml_auth_google.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-06 07:02:37.000000 caraml-auth-google-0.0.0.post5/caraml_auth_google.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-06 07:02:37.000000 caraml-auth-google-0.0.0.post5/caraml_auth_google.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 07:02:37.000000 caraml-auth-google-0.0.0.post5/caraml_auth_google.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-06 07:02:37.000000 caraml-auth-google-0.0.0.post5/caraml_auth_google.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-06 07:02:37.000000 caraml-auth-google-0.0.0.post5/caraml_auth_google.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 07:02:37.000000 caraml-auth-google-0.0.0.post5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-06 07:02:21.000000 caraml-auth-google-0.0.0.post5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:02:37.000000 caraml-auth-google-0.0.0.post5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 07:02:21.000000 caraml-auth-google-0.0.0.post5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6967 2023-06-06 07:02:21.000000 caraml-auth-google-0.0.0.post5/tests/test_id_token_credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:52:25.000000 caraml-auth-google-0.0.0.post6/
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-13 07:52:25.000000 caraml-auth-google-0.0.0.post6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-13 07:52:09.000000 caraml-auth-google-0.0.0.post6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:52:25.000000 caraml-auth-google-0.0.0.post6/caraml_auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 07:52:09.000000 caraml-auth-google-0.0.0.post6/caraml_auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8610 2023-06-13 07:52:09.000000 caraml-auth-google-0.0.0.post6/caraml_auth/id_token_credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:52:25.000000 caraml-auth-google-0.0.0.post6/caraml_auth_google.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-13 07:52:24.000000 caraml-auth-google-0.0.0.post6/caraml_auth_google.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-13 07:52:24.000000 caraml-auth-google-0.0.0.post6/caraml_auth_google.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 07:52:24.000000 caraml-auth-google-0.0.0.post6/caraml_auth_google.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-13 07:52:24.000000 caraml-auth-google-0.0.0.post6/caraml_auth_google.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-13 07:52:24.000000 caraml-auth-google-0.0.0.post6/caraml_auth_google.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 07:52:25.000000 caraml-auth-google-0.0.0.post6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-13 07:52:09.000000 caraml-auth-google-0.0.0.post6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:52:25.000000 caraml-auth-google-0.0.0.post6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 07:52:09.000000 caraml-auth-google-0.0.0.post6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6967 2023-06-13 07:52:09.000000 caraml-auth-google-0.0.0.post6/tests/test_id_token_credentials.py
```

### Comparing `caraml-auth-google-0.0.0.post5/PKG-INFO` & `caraml-auth-google-0.0.0.post6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caraml-auth-google
-Version: 0.0.0.post5
+Version: 0.0.0.post6
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: # CaraML Google Authentication
         
         Utility package containing functions to authenticate users of the Python SDKs of CaraML.
```

### Comparing `caraml-auth-google-0.0.0.post5/caraml_auth/id_token_credentials.py` & `caraml-auth-google-0.0.0.post6/caraml_auth/id_token_credentials.py`

 * *Files identical despite different names*

### Comparing `caraml-auth-google-0.0.0.post5/caraml_auth_google.egg-info/PKG-INFO` & `caraml-auth-google-0.0.0.post6/caraml_auth_google.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caraml-auth-google
-Version: 0.0.0.post5
+Version: 0.0.0.post6
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: # CaraML Google Authentication
         
         Utility package containing functions to authenticate users of the Python SDKs of CaraML.
```

### Comparing `caraml-auth-google-0.0.0.post5/setup.py` & `caraml-auth-google-0.0.0.post6/setup.py`

 * *Files identical despite different names*

### Comparing `caraml-auth-google-0.0.0.post5/tests/test_id_token_credentials.py` & `caraml-auth-google-0.0.0.post6/tests/test_id_token_credentials.py`

 * *Files identical despite different names*

