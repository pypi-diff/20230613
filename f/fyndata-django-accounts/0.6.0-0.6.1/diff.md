# Comparing `tmp/fyndata-django-accounts-0.6.0.tar.gz` & `tmp/fyndata-django-accounts-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fyndata-django-accounts-0.6.0.tar", last modified: Tue Mar 14 21:10:59 2023, max compression
+gzip compressed data, was "fyndata-django-accounts-0.6.1.tar", last modified: Tue Jun 13 13:44:14 2023, max compression
```

## Comparing `fyndata-django-accounts-0.6.0.tar` & `fyndata-django-accounts-0.6.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 21:10:59.120942 fyndata-django-accounts-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-03-14 21:10:31.000000 fyndata-django-accounts-0.6.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-03-14 21:10:31.000000 fyndata-django-accounts-0.6.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5220 2023-03-14 21:10:31.000000 fyndata-django-accounts-0.6.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-03-14 21:10:31.000000 fyndata-django-accounts-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-03-14 21:10:31.000000 fyndata-django-accounts-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8972 2023-03-14 21:10:59.120942 fyndata-django-accounts-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-03-14 21:10:31.000000 fyndata-django-accounts-0.6.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 21:10:59.116942 fyndata-django-accounts-0.6.0/fd_dj_accounts/
--rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-03-14 21:10:31.000000 fyndata-django-accounts-0.6.0/fd_dj_accounts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-03-14 21:10:31.000000 fyndata-django-accounts-0.6.0/fd_dj_accounts/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-03-14 21:10:31.000000 fyndata-django-accounts-0.6.0/fd_dj_accounts/auth_backends.py
--rw-r--r--   0 runner    (1001) docker     (123)     7777 2023-03-14 21:10:31.000000 fyndata-django-accounts-0.6.0/fd_dj_accounts/base_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 21:10:59.116942 fyndata-django-accounts-0.6.0/fd_dj_accounts/management/
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-03-14 21:10:31.000000 fyndata-django-accounts-0.6.0/fd_dj_accounts/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 21:10:59.116942 fyndata-django-accounts-0.6.0/fd_dj_accounts/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 21:10:31.000000 fyndata-django-accounts-0.6.0/fd_dj_accounts/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7970 2023-03-14 21:10:31.000000 fyndata-django-accounts-0.6.0/fd_dj_accounts/management/commands/createsuperuser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 21:10:59.116942 fyndata-django-accounts-0.6.0/fd_dj_accounts/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-03-14 21:10:31.000000 fyndata-django-accounts-0.6.0/fd_dj_accounts/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 21:10:31.000000 fyndata-django-accounts-0.6.0/fd_dj_accounts/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-03-14 21:10:31.000000 fyndata-django-accounts-0.6.0/fd_dj_accounts/models.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 21:10:31.000000 fyndata-django-accounts-0.6.0/fd_dj_accounts/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-03-14 21:10:31.000000 fyndata-django-accounts-0.6.0/fd_dj_accounts/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-03-14 21:10:31.000000 fyndata-django-accounts-0.6.0/fd_dj_accounts/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 21:10:59.120942 fyndata-django-accounts-0.6.0/fyndata_django_accounts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8972 2023-03-14 21:10:59.000000 fyndata-django-accounts-0.6.0/fyndata_django_accounts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-03-14 21:10:59.000000 fyndata-django-accounts-0.6.0/fyndata_django_accounts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 21:10:59.000000 fyndata-django-accounts-0.6.0/fyndata_django_accounts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 21:10:58.000000 fyndata-django-accounts-0.6.0/fyndata_django_accounts.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-14 21:10:59.000000 fyndata-django-accounts-0.6.0/fyndata_django_accounts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-14 21:10:59.000000 fyndata-django-accounts-0.6.0/fyndata_django_accounts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-03-14 21:10:59.120942 fyndata-django-accounts-0.6.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3059 2023-03-14 21:10:31.000000 fyndata-django-accounts-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 21:10:59.120942 fyndata-django-accounts-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-03-14 21:10:31.000000 fyndata-django-accounts-0.6.0/tests/test_apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     7114 2023-03-14 21:10:31.000000 fyndata-django-accounts-0.6.0/tests/test_auth_backends.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-03-14 21:10:31.000000 fyndata-django-accounts-0.6.0/tests/test_factories.py
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-03-14 21:10:31.000000 fyndata-django-accounts-0.6.0/tests/test_management.py
--rw-r--r--   0 runner    (1001) docker     (123)     8502 2023-03-14 21:10:31.000000 fyndata-django-accounts-0.6.0/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-03-14 21:10:31.000000 fyndata-django-accounts-0.6.0/tests/test_signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:44:14.470327 fyndata-django-accounts-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-13 13:43:45.000000 fyndata-django-accounts-0.6.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-06-13 13:43:45.000000 fyndata-django-accounts-0.6.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-06-13 13:43:45.000000 fyndata-django-accounts-0.6.1/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-13 13:43:45.000000 fyndata-django-accounts-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-13 13:43:45.000000 fyndata-django-accounts-0.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9261 2023-06-13 13:44:14.470327 fyndata-django-accounts-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-06-13 13:43:45.000000 fyndata-django-accounts-0.6.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:44:14.466328 fyndata-django-accounts-0.6.1/fd_dj_accounts/
+-rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-06-13 13:43:45.000000 fyndata-django-accounts-0.6.1/fd_dj_accounts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-06-13 13:43:45.000000 fyndata-django-accounts-0.6.1/fd_dj_accounts/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-06-13 13:43:45.000000 fyndata-django-accounts-0.6.1/fd_dj_accounts/auth_backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7777 2023-06-13 13:43:45.000000 fyndata-django-accounts-0.6.1/fd_dj_accounts/base_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:44:14.466328 fyndata-django-accounts-0.6.1/fd_dj_accounts/management/
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-13 13:43:45.000000 fyndata-django-accounts-0.6.1/fd_dj_accounts/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:44:14.466328 fyndata-django-accounts-0.6.1/fd_dj_accounts/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:43:45.000000 fyndata-django-accounts-0.6.1/fd_dj_accounts/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7970 2023-06-13 13:43:45.000000 fyndata-django-accounts-0.6.1/fd_dj_accounts/management/commands/createsuperuser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:44:14.466328 fyndata-django-accounts-0.6.1/fd_dj_accounts/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-06-13 13:43:45.000000 fyndata-django-accounts-0.6.1/fd_dj_accounts/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:43:45.000000 fyndata-django-accounts-0.6.1/fd_dj_accounts/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-06-13 13:43:45.000000 fyndata-django-accounts-0.6.1/fd_dj_accounts/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:43:45.000000 fyndata-django-accounts-0.6.1/fd_dj_accounts/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-13 13:43:45.000000 fyndata-django-accounts-0.6.1/fd_dj_accounts/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-13 13:43:45.000000 fyndata-django-accounts-0.6.1/fd_dj_accounts/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:44:14.470327 fyndata-django-accounts-0.6.1/fyndata_django_accounts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9261 2023-06-13 13:44:14.000000 fyndata-django-accounts-0.6.1/fyndata_django_accounts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-13 13:44:14.000000 fyndata-django-accounts-0.6.1/fyndata_django_accounts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 13:44:14.000000 fyndata-django-accounts-0.6.1/fyndata_django_accounts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 13:44:13.000000 fyndata-django-accounts-0.6.1/fyndata_django_accounts.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-13 13:44:14.000000 fyndata-django-accounts-0.6.1/fyndata_django_accounts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-13 13:44:14.000000 fyndata-django-accounts-0.6.1/fyndata_django_accounts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-13 13:44:14.474328 fyndata-django-accounts-0.6.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3059 2023-06-13 13:43:45.000000 fyndata-django-accounts-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:44:14.470327 fyndata-django-accounts-0.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-13 13:43:45.000000 fyndata-django-accounts-0.6.1/tests/test_apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7114 2023-06-13 13:43:45.000000 fyndata-django-accounts-0.6.1/tests/test_auth_backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-06-13 13:43:45.000000 fyndata-django-accounts-0.6.1/tests/test_factories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-13 13:43:45.000000 fyndata-django-accounts-0.6.1/tests/test_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8502 2023-06-13 13:43:45.000000 fyndata-django-accounts-0.6.1/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-13 13:43:45.000000 fyndata-django-accounts-0.6.1/tests/test_signals.py
```

### Comparing `fyndata-django-accounts-0.6.0/CONTRIBUTING.rst` & `fyndata-django-accounts-0.6.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `fyndata-django-accounts-0.6.0/HISTORY.rst` & `fyndata-django-accounts-0.6.1/HISTORY.rst`

 * *Files 11% similar despite different names*

```diff
@@ -2,14 +2,22 @@
 
 History
 -------
 
 unreleased (YYYY-MM-DD)
 +++++++++++++++++++++++
 
+0.6.1 (2023-06-09)
+++++++++++++++++++
+
+- (PR #228, 2023-04-04) Add Git commit linter
+- (PR #225, 2023-04-05) Bump wheel from 0.38.4 to 0.40.0
+- (PR #227, 2023-05-23) chore(deps): Bump actions/dependency-review-action from 3.0.3 to 3.0.4
+- (PR #234, 2023-06-05) Add Codecov to CI workflow
+
 0.6.0 (2023-03-14)
 ++++++++++++++++++
 
 - (PR #218, 2023-03-08) Drop support for Python 3.7
 - (PR #209, 2023-03-14) chore(deps): bump coverage from 7.1.0 to 7.2.1
 - (PR #219, 2023-03-14) chore(deps): bump setuptools from 67.1.0 to 67.6.0
 - (PR #220, 2023-03-14) chore: bump actions/cache from 3.2.5 to 3.3.1
```

### Comparing `fyndata-django-accounts-0.6.0/LICENSE` & `fyndata-django-accounts-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fyndata-django-accounts-0.6.0/PKG-INFO` & `fyndata-django-accounts-0.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fyndata-django-accounts
-Version: 0.6.0
+Version: 0.6.1
 Summary: Reusable Django app to replace the default Django user (account) model.
 Home-page: https://github.com/fyndata/fyndata-django-accounts
 Author: Fyndata (Fynpal SpA)
 Author-email: no-reply@fyndata.com
 License: MIT
 Keywords: fyndata-django-accounts
 Classifier: Development Status :: 3 - Alpha
@@ -143,14 +143,22 @@
 
 History
 -------
 
 unreleased (YYYY-MM-DD)
 +++++++++++++++++++++++
 
+0.6.1 (2023-06-09)
+++++++++++++++++++
+
+- (PR #228, 2023-04-04) Add Git commit linter
+- (PR #225, 2023-04-05) Bump wheel from 0.38.4 to 0.40.0
+- (PR #227, 2023-05-23) chore(deps): Bump actions/dependency-review-action from 3.0.3 to 3.0.4
+- (PR #234, 2023-06-05) Add Codecov to CI workflow
+
 0.6.0 (2023-03-14)
 ++++++++++++++++++
 
 - (PR #218, 2023-03-08) Drop support for Python 3.7
 - (PR #209, 2023-03-14) chore(deps): bump coverage from 7.1.0 to 7.2.1
 - (PR #219, 2023-03-14) chore(deps): bump setuptools from 67.1.0 to 67.6.0
 - (PR #220, 2023-03-14) chore: bump actions/cache from 3.2.5 to 3.3.1
```

### Comparing `fyndata-django-accounts-0.6.0/README.rst` & `fyndata-django-accounts-0.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `fyndata-django-accounts-0.6.0/fd_dj_accounts/__init__.py` & `fyndata-django-accounts-0.6.1/fd_dj_accounts/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,11 +94,11 @@
     https://docs.djangoproject.com/en/2.1/topics/auth/customizing/#specifying-a-custom-user-model
     https://docs.djangoproject.com/en/2.1/ref/contrib/auth/#django.contrib.auth.models.User
 
 
 """
 
 
-__version__ = '0.6.0'
+__version__ = '0.6.1'
 
 
 default_app_config = 'fd_dj_accounts.apps.AccountsAppConfig'
```

### Comparing `fyndata-django-accounts-0.6.0/fd_dj_accounts/apps.py` & `fyndata-django-accounts-0.6.1/fd_dj_accounts/apps.py`

 * *Files identical despite different names*

### Comparing `fyndata-django-accounts-0.6.0/fd_dj_accounts/auth_backends.py` & `fyndata-django-accounts-0.6.1/fd_dj_accounts/auth_backends.py`

 * *Files identical despite different names*

### Comparing `fyndata-django-accounts-0.6.0/fd_dj_accounts/base_models.py` & `fyndata-django-accounts-0.6.1/fd_dj_accounts/base_models.py`

 * *Files identical despite different names*

### Comparing `fyndata-django-accounts-0.6.0/fd_dj_accounts/management/__init__.py` & `fyndata-django-accounts-0.6.1/fd_dj_accounts/management/__init__.py`

 * *Files identical despite different names*

### Comparing `fyndata-django-accounts-0.6.0/fd_dj_accounts/management/commands/createsuperuser.py` & `fyndata-django-accounts-0.6.1/fd_dj_accounts/management/commands/createsuperuser.py`

 * *Files identical despite different names*

### Comparing `fyndata-django-accounts-0.6.0/fd_dj_accounts/migrations/0001_initial.py` & `fyndata-django-accounts-0.6.1/fd_dj_accounts/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `fyndata-django-accounts-0.6.0/fd_dj_accounts/models.py` & `fyndata-django-accounts-0.6.1/fd_dj_accounts/models.py`

 * *Files identical despite different names*

### Comparing `fyndata-django-accounts-0.6.0/fd_dj_accounts/urls.py` & `fyndata-django-accounts-0.6.1/fd_dj_accounts/urls.py`

 * *Files identical despite different names*

### Comparing `fyndata-django-accounts-0.6.0/fyndata_django_accounts.egg-info/PKG-INFO` & `fyndata-django-accounts-0.6.1/fyndata_django_accounts.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fyndata-django-accounts
-Version: 0.6.0
+Version: 0.6.1
 Summary: Reusable Django app to replace the default Django user (account) model.
 Home-page: https://github.com/fyndata/fyndata-django-accounts
 Author: Fyndata (Fynpal SpA)
 Author-email: no-reply@fyndata.com
 License: MIT
 Keywords: fyndata-django-accounts
 Classifier: Development Status :: 3 - Alpha
@@ -143,14 +143,22 @@
 
 History
 -------
 
 unreleased (YYYY-MM-DD)
 +++++++++++++++++++++++
 
+0.6.1 (2023-06-09)
+++++++++++++++++++
+
+- (PR #228, 2023-04-04) Add Git commit linter
+- (PR #225, 2023-04-05) Bump wheel from 0.38.4 to 0.40.0
+- (PR #227, 2023-05-23) chore(deps): Bump actions/dependency-review-action from 3.0.3 to 3.0.4
+- (PR #234, 2023-06-05) Add Codecov to CI workflow
+
 0.6.0 (2023-03-14)
 ++++++++++++++++++
 
 - (PR #218, 2023-03-08) Drop support for Python 3.7
 - (PR #209, 2023-03-14) chore(deps): bump coverage from 7.1.0 to 7.2.1
 - (PR #219, 2023-03-14) chore(deps): bump setuptools from 67.1.0 to 67.6.0
 - (PR #220, 2023-03-14) chore: bump actions/cache from 3.2.5 to 3.3.1
```

### Comparing `fyndata-django-accounts-0.6.0/fyndata_django_accounts.egg-info/SOURCES.txt` & `fyndata-django-accounts-0.6.1/fyndata_django_accounts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fyndata-django-accounts-0.6.0/setup.cfg` & `fyndata-django-accounts-0.6.1/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -9,14 +9,17 @@
 
 [coverage:report]
 exclude_lines = 
 	pragma: no cover
 	if __name__ == .__main__.
 show_missing = True
 
+[coverage:xml]
+output = test-reports/coverage/xml/coverage.xml
+
 [coverage:html]
 directory = test-reports/coverage/html
 
 [flake8]
 ignore = 
 	W503
 exclude =
```

### Comparing `fyndata-django-accounts-0.6.0/setup.py` & `fyndata-django-accounts-0.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `fyndata-django-accounts-0.6.0/tests/test_apps.py` & `fyndata-django-accounts-0.6.1/tests/test_apps.py`

 * *Files identical despite different names*

### Comparing `fyndata-django-accounts-0.6.0/tests/test_auth_backends.py` & `fyndata-django-accounts-0.6.1/tests/test_auth_backends.py`

 * *Files identical despite different names*

### Comparing `fyndata-django-accounts-0.6.0/tests/test_factories.py` & `fyndata-django-accounts-0.6.1/tests/test_factories.py`

 * *Files identical despite different names*

### Comparing `fyndata-django-accounts-0.6.0/tests/test_management.py` & `fyndata-django-accounts-0.6.1/tests/test_management.py`

 * *Files identical despite different names*

### Comparing `fyndata-django-accounts-0.6.0/tests/test_models.py` & `fyndata-django-accounts-0.6.1/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `fyndata-django-accounts-0.6.0/tests/test_signals.py` & `fyndata-django-accounts-0.6.1/tests/test_signals.py`

 * *Files identical despite different names*

