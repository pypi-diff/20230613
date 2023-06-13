# Comparing `tmp/payable-subscriptions-1.0.7.zip` & `tmp/payable-subscriptions-1.0.8.zip`

## zipinfo {}

```diff
@@ -1,42 +1,42 @@
-Zip file size: 38463 bytes, number of entries: 40
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-26 15:51 payable-subscriptions-1.0.7/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-26 15:51 payable-subscriptions-1.0.7/payable_subscriptions.egg-info/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-26 15:51 payable-subscriptions-1.0.7/sandbox/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-26 15:51 payable-subscriptions-1.0.7/payablesubs/
--rw-r--r--  2.0 unx     3404 b- defN 23-May-26 15:51 payable-subscriptions-1.0.7/PKG-INFO
--rw-r--r--  2.0 unx    35149 b- defN 22-Dec-11 13:43 payable-subscriptions-1.0.7/LICENSE
--rw-r--r--  2.0 unx     2697 b- defN 23-Feb-10 16:56 payable-subscriptions-1.0.7/README.md
--rw-r--r--  2.0 unx     1371 b- defN 23-May-26 15:48 payable-subscriptions-1.0.7/setup.py
--rw-r--r--  2.0 unx       38 b- defN 23-May-26 15:51 payable-subscriptions-1.0.7/setup.cfg
--rw-r--r--  2.0 unx     3404 b- defN 23-May-26 15:51 payable-subscriptions-1.0.7/payable_subscriptions.egg-info/PKG-INFO
--rw-r--r--  2.0 unx      955 b- defN 23-May-26 15:51 payable-subscriptions-1.0.7/payable_subscriptions.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx      156 b- defN 23-May-26 15:51 payable-subscriptions-1.0.7/payable_subscriptions.egg-info/requires.txt
--rw-r--r--  2.0 unx       20 b- defN 23-May-26 15:51 payable-subscriptions-1.0.7/payable_subscriptions.egg-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-May-26 15:51 payable-subscriptions-1.0.7/payable_subscriptions.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx      383 b- defN 22-Dec-28 13:33 payable-subscriptions-1.0.7/sandbox/asgi.py
--rw-r--r--  2.0 unx        0 b- defN 22-Dec-28 13:33 payable-subscriptions-1.0.7/sandbox/__init__.py
--rw-r--r--  2.0 unx     4072 b- defN 23-Feb-28 15:35 payable-subscriptions-1.0.7/sandbox/settings.py
--rwxr-xr-x  2.0 unx      655 b- defN 22-Dec-28 13:33 payable-subscriptions-1.0.7/sandbox/manage.py
--rw-r--r--  2.0 unx      186 b- defN 22-Dec-28 21:40 payable-subscriptions-1.0.7/sandbox/urls.py
--rw-r--r--  2.0 unx      383 b- defN 22-Dec-28 13:33 payable-subscriptions-1.0.7/sandbox/wsgi.py
--rwxr-xr-x  2.0 unx     4421 b- defN 23-Jan-30 06:30 payable-subscriptions-1.0.7/sandbox/init_db.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-26 15:51 payable-subscriptions-1.0.7/payablesubs/clients/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-26 15:51 payable-subscriptions-1.0.7/payablesubs/migrations/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-26 15:51 payable-subscriptions-1.0.7/payablesubs/management/
--rw-r--r--  2.0 unx     2806 b- defN 23-Jan-06 15:56 payable-subscriptions-1.0.7/payablesubs/models.py
--rw-r--r--  2.0 unx        0 b- defN 22-Dec-23 11:11 payable-subscriptions-1.0.7/payablesubs/__init__.py
--rw-r--r--  2.0 unx      273 b- defN 23-Jan-02 15:41 payable-subscriptions-1.0.7/payablesubs/apps.py
--rw-r--r--  2.0 unx        0 b- defN 23-Feb-10 16:56 payable-subscriptions-1.0.7/payablesubs/clients/__init__.py
--rw-r--r--  2.0 unx     4681 b- defN 23-Feb-10 16:56 payable-subscriptions-1.0.7/payablesubs/clients/google.py
--rw-r--r--  2.0 unx      589 b- defN 23-Feb-10 16:56 payable-subscriptions-1.0.7/payablesubs/clients/venmo.py
--rw-r--r--  2.0 unx        0 b- defN 22-Dec-28 13:33 payable-subscriptions-1.0.7/payablesubs/migrations/__init__.py
--rw-r--r--  2.0 unx     2005 b- defN 23-Jan-06 15:56 payable-subscriptions-1.0.7/payablesubs/migrations/0003_payment_delete_venmotransaction.py
--rw-r--r--  2.0 unx     1156 b- defN 23-Jan-02 20:39 payable-subscriptions-1.0.7/payablesubs/migrations/0002_venmotransaction.py
--rw-r--r--  2.0 unx     3238 b- defN 23-Jan-02 20:39 payable-subscriptions-1.0.7/payablesubs/migrations/0001_initial.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-26 15:51 payable-subscriptions-1.0.7/payablesubs/management/commands/
--rw-r--r--  2.0 unx        0 b- defN 22-Dec-28 13:33 payable-subscriptions-1.0.7/payablesubs/management/__init__.py
--rw-r--r--  2.0 unx     3715 b- defN 23-Feb-10 16:56 payable-subscriptions-1.0.7/payablesubs/management/commands/add_subscription.py
--rw-r--r--  2.0 unx        0 b- defN 22-Dec-28 13:33 payable-subscriptions-1.0.7/payablesubs/management/commands/__init__.py
--rw-r--r--  2.0 unx     8887 b- defN 23-Mar-07 08:44 payable-subscriptions-1.0.7/payablesubs/management/commands/_payable_manager.py
--rw-r--r--  2.0 unx     1972 b- defN 23-May-26 15:22 payable-subscriptions-1.0.7/payablesubs/management/commands/print_subscriptions.py
-40 files, 86617 bytes uncompressed, 30977 bytes compressed:  64.2%
+Zip file size: 38812 bytes, number of entries: 40
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-13 14:35 payable-subscriptions-1.0.8/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-13 14:35 payable-subscriptions-1.0.8/payable_subscriptions.egg-info/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-13 14:35 payable-subscriptions-1.0.8/sandbox/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-13 14:35 payable-subscriptions-1.0.8/payablesubs/
+-rw-r--r--  2.0 unx     3404 b- defN 23-Jun-13 14:35 payable-subscriptions-1.0.8/PKG-INFO
+-rw-r--r--  2.0 unx    35149 b- defN 22-Dec-11 13:43 payable-subscriptions-1.0.8/LICENSE
+-rw-r--r--  2.0 unx     2697 b- defN 23-Feb-10 16:56 payable-subscriptions-1.0.8/README.md
+-rw-r--r--  2.0 unx     1371 b- defN 23-Jun-13 14:35 payable-subscriptions-1.0.8/setup.py
+-rw-r--r--  2.0 unx       38 b- defN 23-Jun-13 14:35 payable-subscriptions-1.0.8/setup.cfg
+-rw-r--r--  2.0 unx     3404 b- defN 23-Jun-13 14:35 payable-subscriptions-1.0.8/payable_subscriptions.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx      955 b- defN 23-Jun-13 14:35 payable-subscriptions-1.0.8/payable_subscriptions.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx      156 b- defN 23-Jun-13 14:35 payable-subscriptions-1.0.8/payable_subscriptions.egg-info/requires.txt
+-rw-r--r--  2.0 unx       20 b- defN 23-Jun-13 14:35 payable-subscriptions-1.0.8/payable_subscriptions.egg-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Jun-13 14:35 payable-subscriptions-1.0.8/payable_subscriptions.egg-info/dependency_links.txt
+-rw-r--r--  2.0 unx      383 b- defN 22-Dec-28 13:33 payable-subscriptions-1.0.8/sandbox/asgi.py
+-rw-r--r--  2.0 unx        0 b- defN 22-Dec-28 13:33 payable-subscriptions-1.0.8/sandbox/__init__.py
+-rw-r--r--  2.0 unx     4440 b- defN 23-Jun-13 14:34 payable-subscriptions-1.0.8/sandbox/settings.py
+-rwxr-xr-x  2.0 unx      655 b- defN 22-Dec-28 13:33 payable-subscriptions-1.0.8/sandbox/manage.py
+-rw-r--r--  2.0 unx      186 b- defN 22-Dec-28 21:40 payable-subscriptions-1.0.8/sandbox/urls.py
+-rw-r--r--  2.0 unx      383 b- defN 22-Dec-28 13:33 payable-subscriptions-1.0.8/sandbox/wsgi.py
+-rwxr-xr-x  2.0 unx     4421 b- defN 23-Jan-30 06:30 payable-subscriptions-1.0.8/sandbox/init_db.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-13 14:35 payable-subscriptions-1.0.8/payablesubs/clients/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-13 14:35 payable-subscriptions-1.0.8/payablesubs/migrations/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-13 14:35 payable-subscriptions-1.0.8/payablesubs/management/
+-rw-r--r--  2.0 unx     2806 b- defN 23-Jan-06 15:56 payable-subscriptions-1.0.8/payablesubs/models.py
+-rw-r--r--  2.0 unx        0 b- defN 22-Dec-23 11:11 payable-subscriptions-1.0.8/payablesubs/__init__.py
+-rw-r--r--  2.0 unx      273 b- defN 23-Jan-02 15:41 payable-subscriptions-1.0.8/payablesubs/apps.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Feb-10 16:56 payable-subscriptions-1.0.8/payablesubs/clients/__init__.py
+-rw-r--r--  2.0 unx     4681 b- defN 23-Feb-10 16:56 payable-subscriptions-1.0.8/payablesubs/clients/google.py
+-rw-r--r--  2.0 unx      589 b- defN 23-Feb-10 16:56 payable-subscriptions-1.0.8/payablesubs/clients/venmo.py
+-rw-r--r--  2.0 unx        0 b- defN 22-Dec-28 13:33 payable-subscriptions-1.0.8/payablesubs/migrations/__init__.py
+-rw-r--r--  2.0 unx     2005 b- defN 23-Jan-06 15:56 payable-subscriptions-1.0.8/payablesubs/migrations/0003_payment_delete_venmotransaction.py
+-rw-r--r--  2.0 unx     1156 b- defN 23-Jan-02 20:39 payable-subscriptions-1.0.8/payablesubs/migrations/0002_venmotransaction.py
+-rw-r--r--  2.0 unx     3238 b- defN 23-Jan-02 20:39 payable-subscriptions-1.0.8/payablesubs/migrations/0001_initial.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-13 14:35 payable-subscriptions-1.0.8/payablesubs/management/commands/
+-rw-r--r--  2.0 unx        0 b- defN 22-Dec-28 13:33 payable-subscriptions-1.0.8/payablesubs/management/__init__.py
+-rw-r--r--  2.0 unx     3715 b- defN 23-Feb-10 16:56 payable-subscriptions-1.0.8/payablesubs/management/commands/add_subscription.py
+-rw-r--r--  2.0 unx        0 b- defN 22-Dec-28 13:33 payable-subscriptions-1.0.8/payablesubs/management/commands/__init__.py
+-rw-r--r--  2.0 unx     8887 b- defN 23-Mar-07 08:44 payable-subscriptions-1.0.8/payablesubs/management/commands/_payable_manager.py
+-rw-r--r--  2.0 unx     2616 b- defN 23-Jun-13 14:34 payable-subscriptions-1.0.8/payablesubs/management/commands/print_subscriptions.py
+40 files, 87629 bytes uncompressed, 31326 bytes compressed:  64.3%
```

## zipnote {}

```diff
@@ -1,121 +1,121 @@
-Filename: payable-subscriptions-1.0.7/
+Filename: payable-subscriptions-1.0.8/
 Comment: 
 
-Filename: payable-subscriptions-1.0.7/payable_subscriptions.egg-info/
+Filename: payable-subscriptions-1.0.8/payable_subscriptions.egg-info/
 Comment: 
 
-Filename: payable-subscriptions-1.0.7/sandbox/
+Filename: payable-subscriptions-1.0.8/sandbox/
 Comment: 
 
-Filename: payable-subscriptions-1.0.7/payablesubs/
+Filename: payable-subscriptions-1.0.8/payablesubs/
 Comment: 
 
-Filename: payable-subscriptions-1.0.7/PKG-INFO
+Filename: payable-subscriptions-1.0.8/PKG-INFO
 Comment: 
 
-Filename: payable-subscriptions-1.0.7/LICENSE
+Filename: payable-subscriptions-1.0.8/LICENSE
 Comment: 
 
-Filename: payable-subscriptions-1.0.7/README.md
+Filename: payable-subscriptions-1.0.8/README.md
 Comment: 
 
-Filename: payable-subscriptions-1.0.7/setup.py
+Filename: payable-subscriptions-1.0.8/setup.py
 Comment: 
 
-Filename: payable-subscriptions-1.0.7/setup.cfg
+Filename: payable-subscriptions-1.0.8/setup.cfg
 Comment: 
 
-Filename: payable-subscriptions-1.0.7/payable_subscriptions.egg-info/PKG-INFO
+Filename: payable-subscriptions-1.0.8/payable_subscriptions.egg-info/PKG-INFO
 Comment: 
 
-Filename: payable-subscriptions-1.0.7/payable_subscriptions.egg-info/SOURCES.txt
+Filename: payable-subscriptions-1.0.8/payable_subscriptions.egg-info/SOURCES.txt
 Comment: 
 
-Filename: payable-subscriptions-1.0.7/payable_subscriptions.egg-info/requires.txt
+Filename: payable-subscriptions-1.0.8/payable_subscriptions.egg-info/requires.txt
 Comment: 
 
-Filename: payable-subscriptions-1.0.7/payable_subscriptions.egg-info/top_level.txt
+Filename: payable-subscriptions-1.0.8/payable_subscriptions.egg-info/top_level.txt
 Comment: 
 
-Filename: payable-subscriptions-1.0.7/payable_subscriptions.egg-info/dependency_links.txt
+Filename: payable-subscriptions-1.0.8/payable_subscriptions.egg-info/dependency_links.txt
 Comment: 
 
-Filename: payable-subscriptions-1.0.7/sandbox/asgi.py
+Filename: payable-subscriptions-1.0.8/sandbox/asgi.py
 Comment: 
 
-Filename: payable-subscriptions-1.0.7/sandbox/__init__.py
+Filename: payable-subscriptions-1.0.8/sandbox/__init__.py
 Comment: 
 
-Filename: payable-subscriptions-1.0.7/sandbox/settings.py
+Filename: payable-subscriptions-1.0.8/sandbox/settings.py
 Comment: 
 
-Filename: payable-subscriptions-1.0.7/sandbox/manage.py
+Filename: payable-subscriptions-1.0.8/sandbox/manage.py
 Comment: 
 
-Filename: payable-subscriptions-1.0.7/sandbox/urls.py
+Filename: payable-subscriptions-1.0.8/sandbox/urls.py
 Comment: 
 
-Filename: payable-subscriptions-1.0.7/sandbox/wsgi.py
+Filename: payable-subscriptions-1.0.8/sandbox/wsgi.py
 Comment: 
 
-Filename: payable-subscriptions-1.0.7/sandbox/init_db.py
+Filename: payable-subscriptions-1.0.8/sandbox/init_db.py
 Comment: 
 
-Filename: payable-subscriptions-1.0.7/payablesubs/clients/
+Filename: payable-subscriptions-1.0.8/payablesubs/clients/
 Comment: 
 
-Filename: payable-subscriptions-1.0.7/payablesubs/migrations/
+Filename: payable-subscriptions-1.0.8/payablesubs/migrations/
 Comment: 
 
-Filename: payable-subscriptions-1.0.7/payablesubs/management/
+Filename: payable-subscriptions-1.0.8/payablesubs/management/
 Comment: 
 
-Filename: payable-subscriptions-1.0.7/payablesubs/models.py
+Filename: payable-subscriptions-1.0.8/payablesubs/models.py
 Comment: 
 
-Filename: payable-subscriptions-1.0.7/payablesubs/__init__.py
+Filename: payable-subscriptions-1.0.8/payablesubs/__init__.py
 Comment: 
 
-Filename: payable-subscriptions-1.0.7/payablesubs/apps.py
+Filename: payable-subscriptions-1.0.8/payablesubs/apps.py
 Comment: 
 
-Filename: payable-subscriptions-1.0.7/payablesubs/clients/__init__.py
+Filename: payable-subscriptions-1.0.8/payablesubs/clients/__init__.py
 Comment: 
 
-Filename: payable-subscriptions-1.0.7/payablesubs/clients/google.py
+Filename: payable-subscriptions-1.0.8/payablesubs/clients/google.py
 Comment: 
 
-Filename: payable-subscriptions-1.0.7/payablesubs/clients/venmo.py
+Filename: payable-subscriptions-1.0.8/payablesubs/clients/venmo.py
 Comment: 
 
-Filename: payable-subscriptions-1.0.7/payablesubs/migrations/__init__.py
+Filename: payable-subscriptions-1.0.8/payablesubs/migrations/__init__.py
 Comment: 
 
-Filename: payable-subscriptions-1.0.7/payablesubs/migrations/0003_payment_delete_venmotransaction.py
+Filename: payable-subscriptions-1.0.8/payablesubs/migrations/0003_payment_delete_venmotransaction.py
 Comment: 
 
-Filename: payable-subscriptions-1.0.7/payablesubs/migrations/0002_venmotransaction.py
+Filename: payable-subscriptions-1.0.8/payablesubs/migrations/0002_venmotransaction.py
 Comment: 
 
-Filename: payable-subscriptions-1.0.7/payablesubs/migrations/0001_initial.py
+Filename: payable-subscriptions-1.0.8/payablesubs/migrations/0001_initial.py
 Comment: 
 
-Filename: payable-subscriptions-1.0.7/payablesubs/management/commands/
+Filename: payable-subscriptions-1.0.8/payablesubs/management/commands/
 Comment: 
 
-Filename: payable-subscriptions-1.0.7/payablesubs/management/__init__.py
+Filename: payable-subscriptions-1.0.8/payablesubs/management/__init__.py
 Comment: 
 
-Filename: payable-subscriptions-1.0.7/payablesubs/management/commands/add_subscription.py
+Filename: payable-subscriptions-1.0.8/payablesubs/management/commands/add_subscription.py
 Comment: 
 
-Filename: payable-subscriptions-1.0.7/payablesubs/management/commands/__init__.py
+Filename: payable-subscriptions-1.0.8/payablesubs/management/commands/__init__.py
 Comment: 
 
-Filename: payable-subscriptions-1.0.7/payablesubs/management/commands/_payable_manager.py
+Filename: payable-subscriptions-1.0.8/payablesubs/management/commands/_payable_manager.py
 Comment: 
 
-Filename: payable-subscriptions-1.0.7/payablesubs/management/commands/print_subscriptions.py
+Filename: payable-subscriptions-1.0.8/payablesubs/management/commands/print_subscriptions.py
 Comment: 
 
 Zip file comment:
```

## Comparing `payable-subscriptions-1.0.7/PKG-INFO` & `payable-subscriptions-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: payable-subscriptions
-Version: 1.0.7
+Version: 1.0.8
 Summary: Integrates out-of-the-box payment processing for django-flexible-subscriptions
 Home-page: https://github.com/curtis628/payable-subscriptions
 Author: Tyler Curtis
 Author-email: tjcurt@gmail.com
 Project-URL: Source code, https://github.com/curtis628/payable-subscriptions
 Project-URL: Issues, https://github.com/curtis628/payable-subscriptions/issues
 Classifier: Framework :: Django :: 4.1
```

## Comparing `payable-subscriptions-1.0.7/LICENSE` & `payable-subscriptions-1.0.8/LICENSE`

 * *Files identical despite different names*

## Comparing `payable-subscriptions-1.0.7/README.md` & `payable-subscriptions-1.0.8/README.md`

 * *Files identical despite different names*

## Comparing `payable-subscriptions-1.0.7/setup.py` & `payable-subscriptions-1.0.8/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="payable-subscriptions",
-    version="1.0.7",
+    version="1.0.8",
     url='https://github.com/curtis628/payable-subscriptions',
     author='Tyler Curtis',
     author_email="tjcurt@gmail.com",
     description="Integrates out-of-the-box payment processing for django-flexible-subscriptions",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(exclude=['tests*']),
```

## Comparing `payable-subscriptions-1.0.7/payable_subscriptions.egg-info/PKG-INFO` & `payable-subscriptions-1.0.8/payable_subscriptions.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: payable-subscriptions
-Version: 1.0.7
+Version: 1.0.8
 Summary: Integrates out-of-the-box payment processing for django-flexible-subscriptions
 Home-page: https://github.com/curtis628/payable-subscriptions
 Author: Tyler Curtis
 Author-email: tjcurt@gmail.com
 Project-URL: Source code, https://github.com/curtis628/payable-subscriptions
 Project-URL: Issues, https://github.com/curtis628/payable-subscriptions/issues
 Classifier: Framework :: Django :: 4.1
```

## Comparing `payable-subscriptions-1.0.7/payable_subscriptions.egg-info/SOURCES.txt` & `payable-subscriptions-1.0.8/payable_subscriptions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

## Comparing `payable-subscriptions-1.0.7/sandbox/settings.py` & `payable-subscriptions-1.0.8/sandbox/settings.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import os
 import sys
 
 # Build paths inside the project like this: BASE_DIR / 'subdir'.
 BASE_DIR = Path(__file__).resolve().parent
 
 DFS_MANAGER_CLASS = 'payablesubs.management.commands._payable_manager.PayableManager'
+DFS_ENABLE_ADMIN = True
 
 # Quick-start development settings - unsuitable for production
 # See https://docs.djangoproject.com/en/4.1/howto/deployment/checklist/
 
 # SECURITY WARNING: keep the secret key used in production secret!
 SECRET_KEY = 'django-insecure-*!5vx+@1a%35cad9vzv9w5@1g$_i(8nd_97(^&%hr=h@&-()b+'
 
@@ -104,20 +105,29 @@
 
 
 # Internationalization
 # https://docs.djangoproject.com/en/4.1/topics/i18n/
 
 LANGUAGE_CODE = 'en-us'
 
-TIME_ZONE = 'UTC'
+TIME_ZONE = 'America/Los_Angeles'
 
 USE_I18N = True
 
 USE_TZ = True
 
+# Email
+# https://docs.djangoproject.com/en/4.2/topics/email/
+# https://docs.djangoproject.com/en/4.2/ref/settings/#email-host
+EMAIL_HOST = 'smtp.gmail.com'
+EMAIL_HOST_USER = os.getenv("EMAIL_HOST_USER")
+EMAIL_HOST_PASSWORD = os.getenv("EMAIL_HOST_PASSWORD") #the key or app password here
+EMAIL_PORT = 587
+EMAIL_USE_TLS = True
+
 
 # Static files (CSS, JavaScript, Images)
 # https://docs.djangoproject.com/en/4.1/howto/static-files/
 
 STATIC_URL = 'static/'
 
 # Default primary key field type
```

## Comparing `payable-subscriptions-1.0.7/sandbox/manage.py` & `payable-subscriptions-1.0.8/sandbox/manage.py`

 * *Files identical despite different names*

## Comparing `payable-subscriptions-1.0.7/sandbox/init_db.py` & `payable-subscriptions-1.0.8/sandbox/init_db.py`

 * *Files identical despite different names*

## Comparing `payable-subscriptions-1.0.7/payablesubs/models.py` & `payable-subscriptions-1.0.8/payablesubs/models.py`

 * *Files identical despite different names*

## Comparing `payable-subscriptions-1.0.7/payablesubs/clients/google.py` & `payable-subscriptions-1.0.8/payablesubs/clients/google.py`

 * *Files identical despite different names*

## Comparing `payable-subscriptions-1.0.7/payablesubs/clients/venmo.py` & `payable-subscriptions-1.0.8/payablesubs/clients/venmo.py`

 * *Files identical despite different names*

## Comparing `payable-subscriptions-1.0.7/payablesubs/migrations/0003_payment_delete_venmotransaction.py` & `payable-subscriptions-1.0.8/payablesubs/migrations/0003_payment_delete_venmotransaction.py`

 * *Files identical despite different names*

## Comparing `payable-subscriptions-1.0.7/payablesubs/migrations/0002_venmotransaction.py` & `payable-subscriptions-1.0.8/payablesubs/migrations/0002_venmotransaction.py`

 * *Files identical despite different names*

## Comparing `payable-subscriptions-1.0.7/payablesubs/migrations/0001_initial.py` & `payable-subscriptions-1.0.8/payablesubs/migrations/0001_initial.py`

 * *Files identical despite different names*

## Comparing `payable-subscriptions-1.0.7/payablesubs/management/commands/add_subscription.py` & `payable-subscriptions-1.0.8/payablesubs/management/commands/add_subscription.py`

 * *Files identical despite different names*

## Comparing `payable-subscriptions-1.0.7/payablesubs/management/commands/_payable_manager.py` & `payable-subscriptions-1.0.8/payablesubs/management/commands/_payable_manager.py`

 * *Files identical despite different names*

