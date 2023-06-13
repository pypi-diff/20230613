# Comparing `tmp/django-empty-users-app-1.0.0.tar.gz` & `tmp/django-empty-users-app-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-empty-users-app-1.0.0.tar", last modified: Tue Jun 13 11:08:14 2023, max compression
+gzip compressed data, was "django-empty-users-app-1.0.1.tar", last modified: Tue Jun 13 13:18:32 2023, max compression
```

## Comparing `django-empty-users-app-1.0.0.tar` & `django-empty-users-app-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-06-13 11:08:14.343815 django-empty-users-app-1.0.0/
--rw-r--r--   0 rustam     (501) staff       (20)     1063 2023-06-13 10:57:48.000000 django-empty-users-app-1.0.0/LICENSE
--rw-r--r--   0 rustam     (501) staff       (20)       58 2022-11-29 11:14:37.000000 django-empty-users-app-1.0.0/MANIFEST.in
--rw-r--r--   0 rustam     (501) staff       (20)     2217 2023-06-13 11:08:14.343938 django-empty-users-app-1.0.0/PKG-INFO
--rw-r--r--   0 rustam     (501) staff       (20)      791 2023-06-13 11:07:35.000000 django-empty-users-app-1.0.0/README.md
-drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-06-13 11:08:14.341246 django-empty-users-app-1.0.0/django_empty_users_app.egg-info/
--rw-r--r--   0 rustam     (501) staff       (20)     2217 2023-06-13 11:08:14.000000 django-empty-users-app-1.0.0/django_empty_users_app.egg-info/PKG-INFO
--rw-r--r--   0 rustam     (501) staff       (20)      371 2023-06-13 11:08:14.000000 django-empty-users-app-1.0.0/django_empty_users_app.egg-info/SOURCES.txt
--rw-r--r--   0 rustam     (501) staff       (20)        1 2023-06-13 11:08:14.000000 django-empty-users-app-1.0.0/django_empty_users_app.egg-info/dependency_links.txt
--rw-r--r--   0 rustam     (501) staff       (20)       12 2023-06-13 11:08:14.000000 django-empty-users-app-1.0.0/django_empty_users_app.egg-info/requires.txt
--rw-r--r--   0 rustam     (501) staff       (20)        6 2023-06-13 11:08:14.000000 django-empty-users-app-1.0.0/django_empty_users_app.egg-info/top_level.txt
--rw-r--r--   0 rustam     (501) staff       (20)     1240 2023-06-13 11:08:14.344503 django-empty-users-app-1.0.0/setup.cfg
--rw-r--r--   0 rustam     (501) staff       (20)      195 2022-11-29 11:14:37.000000 django-empty-users-app-1.0.0/setup.py
-drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-06-13 11:08:14.341736 django-empty-users-app-1.0.0/users/
--rw-r--r--   0 rustam     (501) staff       (20)        0 2023-06-13 09:04:08.000000 django-empty-users-app-1.0.0/users/__init__.py
--rw-r--r--   0 rustam     (501) staff       (20)      142 2023-06-13 09:04:08.000000 django-empty-users-app-1.0.0/users/apps.py
-drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-06-13 11:08:14.343506 django-empty-users-app-1.0.0/users/migrations/
--rw-r--r--   0 rustam     (501) staff       (20)      177 2023-06-13 09:06:04.000000 django-empty-users-app-1.0.0/users/migrations/0001_initial.py
--rw-r--r--   0 rustam     (501) staff       (20)        0 2023-06-13 09:04:08.000000 django-empty-users-app-1.0.0/users/migrations/__init__.py
+drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-06-13 13:18:32.534813 django-empty-users-app-1.0.1/
+-rw-r--r--   0 rustam     (501) staff       (20)     1063 2023-06-13 10:57:48.000000 django-empty-users-app-1.0.1/LICENSE
+-rw-r--r--   0 rustam     (501) staff       (20)       33 2023-06-13 11:17:35.000000 django-empty-users-app-1.0.1/MANIFEST.in
+-rw-r--r--   0 rustam     (501) staff       (20)     2221 2023-06-13 13:18:32.534961 django-empty-users-app-1.0.1/PKG-INFO
+-rw-r--r--   0 rustam     (501) staff       (20)      791 2023-06-13 11:07:35.000000 django-empty-users-app-1.0.1/README.md
+drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-06-13 13:18:32.518065 django-empty-users-app-1.0.1/django_empty_users_app.egg-info/
+-rw-r--r--   0 rustam     (501) staff       (20)     2221 2023-06-13 13:18:32.000000 django-empty-users-app-1.0.1/django_empty_users_app.egg-info/PKG-INFO
+-rw-r--r--   0 rustam     (501) staff       (20)      371 2023-06-13 13:18:32.000000 django-empty-users-app-1.0.1/django_empty_users_app.egg-info/SOURCES.txt
+-rw-r--r--   0 rustam     (501) staff       (20)        1 2023-06-13 13:18:32.000000 django-empty-users-app-1.0.1/django_empty_users_app.egg-info/dependency_links.txt
+-rw-r--r--   0 rustam     (501) staff       (20)       12 2023-06-13 13:18:32.000000 django-empty-users-app-1.0.1/django_empty_users_app.egg-info/requires.txt
+-rw-r--r--   0 rustam     (501) staff       (20)        6 2023-06-13 13:18:32.000000 django-empty-users-app-1.0.1/django_empty_users_app.egg-info/top_level.txt
+-rw-r--r--   0 rustam     (501) staff       (20)     1244 2023-06-13 13:18:32.535582 django-empty-users-app-1.0.1/setup.cfg
+-rw-r--r--   0 rustam     (501) staff       (20)      195 2022-11-29 11:14:37.000000 django-empty-users-app-1.0.1/setup.py
+drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-06-13 13:18:32.518554 django-empty-users-app-1.0.1/users/
+-rw-r--r--   0 rustam     (501) staff       (20)        0 2023-06-13 09:04:08.000000 django-empty-users-app-1.0.1/users/__init__.py
+-rw-r--r--   0 rustam     (501) staff       (20)      142 2023-06-13 09:04:08.000000 django-empty-users-app-1.0.1/users/apps.py
+drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-06-13 13:18:32.534510 django-empty-users-app-1.0.1/users/migrations/
+-rw-r--r--   0 rustam     (501) staff       (20)      177 2023-06-13 09:06:04.000000 django-empty-users-app-1.0.1/users/migrations/0001_initial.py
+-rw-r--r--   0 rustam     (501) staff       (20)        0 2023-06-13 09:04:08.000000 django-empty-users-app-1.0.1/users/migrations/__init__.py
```

### Comparing `django-empty-users-app-1.0.0/LICENSE` & `django-empty-users-app-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-empty-users-app-1.0.0/PKG-INFO` & `django-empty-users-app-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: django-empty-users-app
-Version: 1.0.0
+Version: 1.0.1
 Summary: Just an app with empty migration file inside.
-Home-page: https://github.com/HarleyK1ng/django_empty_users
+Home-page: https://github.com/AllYouZombies/django-empty-users-app
 Author: Astafeev Rustam
-Author-email: astafeev0308@gmail.com
+Author-email: rustam@astafeev.dev
 License: MIT License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
```

### Comparing `django-empty-users-app-1.0.0/README.md` & `django-empty-users-app-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `django-empty-users-app-1.0.0/django_empty_users_app.egg-info/PKG-INFO` & `django-empty-users-app-1.0.1/django_empty_users_app.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: django-empty-users-app
-Version: 1.0.0
+Version: 1.0.1
 Summary: Just an app with empty migration file inside.
-Home-page: https://github.com/HarleyK1ng/django_empty_users
+Home-page: https://github.com/AllYouZombies/django-empty-users-app
 Author: Astafeev Rustam
-Author-email: astafeev0308@gmail.com
+Author-email: rustam@astafeev.dev
 License: MIT License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
```

### Comparing `django-empty-users-app-1.0.0/setup.cfg` & `django-empty-users-app-1.0.1/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [metadata]
 name = django-empty-users-app
-version = 1.0.0
+version = 1.0.1
 description = Just an app with empty migration file inside.
-url = https://github.com/HarleyK1ng/django_empty_users
+url = https://github.com/AllYouZombies/django-empty-users-app
 author = Astafeev Rustam
-author_email = astafeev0308@gmail.com
+author_email = rustam@astafeev.dev
 license = MIT License
 classifiers = 
 	Environment :: Web Environment
 	Framework :: Django
 	Framework :: Django :: 3
 	Framework :: Django :: 3.0
 	Framework :: Django :: 3.1
```

