# Comparing `tmp/django-twilio-0.9.2.tar.gz` & `tmp/django-twilio-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-twilio-0.9.2.tar", last modified: Thu Aug  9 01:37:45 2018, max compression
+gzip compressed data, was "dist/django-twilio-0.9.3.tar", last modified: Thu Aug 16 00:52:36 2018, max compression
```

## Comparing `django-twilio-0.9.2.tar` & `django-twilio-0.9.3.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2018-08-09 01:37:45.000000 django-twilio-0.9.2/
--rw-rw-r--   0 jason     (1000) jason     (1000)      117 2018-02-04 17:04:56.000000 django-twilio-0.9.2/requirements.txt
--rw-rw-r--   0 jason     (1000) jason     (1000)     1211 2017-12-29 01:02:24.000000 django-twilio-0.9.2/UNLICENSE
-drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2018-08-09 01:37:45.000000 django-twilio-0.9.2/test_project/
-drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2018-08-09 01:37:45.000000 django-twilio-0.9.2/test_project/test_app/
--rw-rw-r--   0 jason     (1000) jason     (1000)    16101 2018-08-04 17:08:39.000000 django-twilio-0.9.2/test_project/test_app/decorators.py
--rw-rw-r--   0 jason     (1000) jason     (1000)     1925 2018-02-04 17:04:56.000000 django-twilio-0.9.2/test_project/test_app/models.py
--rw-rw-r--   0 jason     (1000) jason     (1000)      718 2018-04-22 16:43:27.000000 django-twilio-0.9.2/test_project/test_app/urls.py
--rw-rw-r--   0 jason     (1000) jason     (1000)     6997 2018-02-04 17:04:56.000000 django-twilio-0.9.2/test_project/test_app/views.py
--rw-rw-r--   0 jason     (1000) jason     (1000)     1359 2018-02-06 01:43:33.000000 django-twilio-0.9.2/test_project/test_app/utils.py
--rw-rw-r--   0 jason     (1000) jason     (1000)     1257 2018-02-04 17:04:56.000000 django-twilio-0.9.2/test_project/test_app/client.py
--rw-rw-r--   0 jason     (1000) jason     (1000)      196 2018-02-04 17:04:56.000000 django-twilio-0.9.2/test_project/test_app/__init__.py
--rw-rw-r--   0 jason     (1000) jason     (1000)     2319 2018-02-04 17:04:56.000000 django-twilio-0.9.2/test_project/test_app/request.py
--rw-rw-r--   0 jason     (1000) jason     (1000)      352 2018-04-22 16:43:27.000000 django-twilio-0.9.2/test_project/urls.py
--rw-rw-r--   0 jason     (1000) jason     (1000)     6806 2018-04-29 02:34:05.000000 django-twilio-0.9.2/test_project/settings.py
--rw-rw-r--   0 jason     (1000) jason     (1000)        0 2017-12-29 01:02:24.000000 django-twilio-0.9.2/test_project/__init__.py
-drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2018-08-09 01:37:45.000000 django-twilio-0.9.2/django_twilio.egg-info/
--rw-rw-r--   0 jason     (1000) jason     (1000)        1 2018-08-09 01:37:45.000000 django-twilio-0.9.2/django_twilio.egg-info/dependency_links.txt
--rw-rw-r--   0 jason     (1000) jason     (1000)     1371 2018-08-09 01:37:45.000000 django-twilio-0.9.2/django_twilio.egg-info/SOURCES.txt
--rw-rw-r--   0 jason     (1000) jason     (1000)      247 2018-08-09 01:37:45.000000 django-twilio-0.9.2/django_twilio.egg-info/requires.txt
--rw-rw-r--   0 jason     (1000) jason     (1000)        1 2018-08-04 17:42:40.000000 django-twilio-0.9.2/django_twilio.egg-info/not-zip-safe
--rw-rw-r--   0 jason     (1000) jason     (1000)       27 2018-08-09 01:37:45.000000 django-twilio-0.9.2/django_twilio.egg-info/top_level.txt
--rw-rw-r--   0 jason     (1000) jason     (1000)     3095 2018-08-09 01:37:45.000000 django-twilio-0.9.2/django_twilio.egg-info/PKG-INFO
--rw-rw-r--   0 jason     (1000) jason     (1000)     2130 2018-08-09 01:35:58.000000 django-twilio-0.9.2/setup.py
-drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2018-08-09 01:37:45.000000 django-twilio-0.9.2/docs/
-drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2018-08-09 01:37:45.000000 django-twilio-0.9.2/docs/source/
--rw-r--r--   0 jason     (1000) jason     (1000)    16365 2018-03-02 02:51:00.000000 django-twilio-0.9.2/docs/source/views.rst
--rw-rw-r--   0 jason     (1000) jason     (1000)     1892 2018-02-04 17:04:56.000000 django-twilio-0.9.2/docs/source/gotchas.rst
--rw-rw-r--   0 jason     (1000) jason     (1000)     8991 2018-02-04 17:04:56.000000 django-twilio-0.9.2/docs/source/conf.py
--rw-r--r--   0 jason     (1000) jason     (1000)     3722 2018-03-02 02:51:00.000000 django-twilio-0.9.2/docs/source/decorators.rst
--rw-rw-r--   0 jason     (1000) jason     (1000)     5226 2018-02-04 17:04:56.000000 django-twilio-0.9.2/docs/source/install.rst
--rw-r--r--   0 jason     (1000) jason     (1000)     1825 2018-03-02 02:51:00.000000 django-twilio-0.9.2/docs/source/requests.rst
--rw-rw-r--   0 jason     (1000) jason     (1000)     3243 2018-02-04 17:04:56.000000 django-twilio-0.9.2/docs/source/rest.rst
--rw-rw-r--   0 jason     (1000) jason     (1000)     1295 2018-02-04 17:04:56.000000 django-twilio-0.9.2/docs/source/contributors.rst
--rw-rw-r--   0 jason     (1000) jason     (1000)     2096 2018-02-04 17:04:56.000000 django-twilio-0.9.2/docs/source/howto.rst
--rw-rw-r--   0 jason     (1000) jason     (1000)     2498 2018-02-04 17:04:56.000000 django-twilio-0.9.2/docs/source/foreword.rst
--rw-rw-r--   0 jason     (1000) jason     (1000)     2853 2018-02-04 17:04:56.000000 django-twilio-0.9.2/docs/source/settings.rst
--rw-rw-r--   0 jason     (1000) jason     (1000)     4752 2018-02-04 17:04:56.000000 django-twilio-0.9.2/docs/source/contribute.rst
--rw-rw-r--   0 jason     (1000) jason     (1000)     1957 2018-08-09 01:35:58.000000 django-twilio-0.9.2/docs/source/index.rst
--rw-rw-r--   0 jason     (1000) jason     (1000)     4622 2017-12-29 01:02:24.000000 django-twilio-0.9.2/docs/Makefile
--rw-rw-r--   0 jason     (1000) jason     (1000)      240 2018-02-04 17:04:56.000000 django-twilio-0.9.2/MANIFEST.in
--rw-rw-r--   0 jason     (1000) jason     (1000)       61 2018-08-09 01:37:45.000000 django-twilio-0.9.2/setup.cfg
--rw-rw-r--   0 jason     (1000) jason     (1000)     1381 2018-08-09 01:35:58.000000 django-twilio-0.9.2/README.rst
-drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2018-08-09 01:37:45.000000 django-twilio-0.9.2/django_twilio/
--rw-rw-r--   0 jason     (1000) jason     (1000)     4173 2018-02-06 01:43:33.000000 django-twilio-0.9.2/django_twilio/decorators.py
--rw-rw-r--   0 jason     (1000) jason     (1000)     2004 2018-02-04 17:04:56.000000 django-twilio-0.9.2/django_twilio/models.py
-drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2018-08-09 01:37:45.000000 django-twilio-0.9.2/django_twilio/south_migrations/
--rw-rw-r--   0 jason     (1000) jason     (1000)        1 2018-02-04 17:04:56.000000 django-twilio-0.9.2/django_twilio/south_migrations/__init__.py
--rw-rw-r--   0 jason     (1000) jason     (1000)     5693 2018-02-04 17:04:56.000000 django-twilio-0.9.2/django_twilio/south_migrations/0001_initial.py
--rw-rw-r--   0 jason     (1000) jason     (1000)     5088 2018-04-18 22:36:25.000000 django-twilio-0.9.2/django_twilio/views.py
--rw-rw-r--   0 jason     (1000) jason     (1000)      575 2018-02-04 17:04:56.000000 django-twilio-0.9.2/django_twilio/admin.py
--rw-rw-r--   0 jason     (1000) jason     (1000)      242 2018-02-04 17:04:56.000000 django-twilio-0.9.2/django_twilio/settings.py
--rw-rw-r--   0 jason     (1000) jason     (1000)     3005 2018-08-04 17:08:39.000000 django-twilio-0.9.2/django_twilio/utils.py
-drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2018-08-09 01:37:45.000000 django-twilio-0.9.2/django_twilio/migrations/
--rw-rw-r--   0 jason     (1000) jason     (1000)        0 2017-12-29 01:02:24.000000 django-twilio-0.9.2/django_twilio/migrations/__init__.py
--rw-rw-r--   0 jason     (1000) jason     (1000)     1401 2018-02-04 17:04:56.000000 django-twilio-0.9.2/django_twilio/migrations/0001_initial.py
--rw-rw-r--   0 jason     (1000) jason     (1000)      286 2018-02-04 17:04:56.000000 django-twilio-0.9.2/django_twilio/client.py
--rw-rw-r--   0 jason     (1000) jason     (1000)       79 2018-02-04 17:04:56.000000 django-twilio-0.9.2/django_twilio/exceptions.py
--rw-rw-r--   0 jason     (1000) jason     (1000)      174 2018-02-06 03:36:19.000000 django-twilio-0.9.2/django_twilio/__init__.py
--rw-rw-r--   0 jason     (1000) jason     (1000)     1548 2018-02-04 17:04:56.000000 django-twilio-0.9.2/django_twilio/request.py
--rw-rw-r--   0 jason     (1000) jason     (1000)     3095 2018-08-09 01:37:45.000000 django-twilio-0.9.2/PKG-INFO
--rw-rw-r--   0 jason     (1000) jason     (1000)      474 2018-02-04 17:04:56.000000 django-twilio-0.9.2/AUTHORS
+drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2018-08-16 00:52:36.000000 django-twilio-0.9.3/
+-rw-rw-r--   0 jason     (1000) jason     (1000)      117 2018-08-16 00:51:40.000000 django-twilio-0.9.3/requirements.txt
+-rw-rw-r--   0 jason     (1000) jason     (1000)     1211 2017-12-29 01:02:24.000000 django-twilio-0.9.3/UNLICENSE
+drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2018-08-16 00:52:36.000000 django-twilio-0.9.3/test_project/
+drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2018-08-16 00:52:36.000000 django-twilio-0.9.3/test_project/test_app/
+-rw-rw-r--   0 jason     (1000) jason     (1000)    16101 2018-08-04 17:08:39.000000 django-twilio-0.9.3/test_project/test_app/decorators.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)     1925 2018-02-04 17:04:56.000000 django-twilio-0.9.3/test_project/test_app/models.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)      718 2018-04-22 16:43:27.000000 django-twilio-0.9.3/test_project/test_app/urls.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)     6997 2018-02-04 17:04:56.000000 django-twilio-0.9.3/test_project/test_app/views.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)     1359 2018-02-06 01:43:33.000000 django-twilio-0.9.3/test_project/test_app/utils.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)     1257 2018-02-04 17:04:56.000000 django-twilio-0.9.3/test_project/test_app/client.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)      196 2018-02-04 17:04:56.000000 django-twilio-0.9.3/test_project/test_app/__init__.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)     2319 2018-02-04 17:04:56.000000 django-twilio-0.9.3/test_project/test_app/request.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)      352 2018-04-22 16:43:27.000000 django-twilio-0.9.3/test_project/urls.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)     6806 2018-04-29 02:34:05.000000 django-twilio-0.9.3/test_project/settings.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)        0 2017-12-29 01:02:24.000000 django-twilio-0.9.3/test_project/__init__.py
+drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2018-08-16 00:52:36.000000 django-twilio-0.9.3/django_twilio.egg-info/
+-rw-rw-r--   0 jason     (1000) jason     (1000)        1 2018-08-16 00:52:35.000000 django-twilio-0.9.3/django_twilio.egg-info/dependency_links.txt
+-rw-rw-r--   0 jason     (1000) jason     (1000)     1371 2018-08-16 00:52:35.000000 django-twilio-0.9.3/django_twilio.egg-info/SOURCES.txt
+-rw-rw-r--   0 jason     (1000) jason     (1000)      247 2018-08-16 00:52:35.000000 django-twilio-0.9.3/django_twilio.egg-info/requires.txt
+-rw-rw-r--   0 jason     (1000) jason     (1000)        1 2018-08-04 17:42:40.000000 django-twilio-0.9.3/django_twilio.egg-info/not-zip-safe
+-rw-rw-r--   0 jason     (1000) jason     (1000)       27 2018-08-16 00:52:35.000000 django-twilio-0.9.3/django_twilio.egg-info/top_level.txt
+-rw-rw-r--   0 jason     (1000) jason     (1000)     3117 2018-08-16 00:52:35.000000 django-twilio-0.9.3/django_twilio.egg-info/PKG-INFO
+-rw-rw-r--   0 jason     (1000) jason     (1000)     2130 2018-08-16 00:49:08.000000 django-twilio-0.9.3/setup.py
+drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2018-08-16 00:52:36.000000 django-twilio-0.9.3/docs/
+drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2018-08-16 00:52:36.000000 django-twilio-0.9.3/docs/source/
+-rw-r--r--   0 jason     (1000) jason     (1000)    16365 2018-03-02 02:51:00.000000 django-twilio-0.9.3/docs/source/views.rst
+-rw-rw-r--   0 jason     (1000) jason     (1000)     1892 2018-02-04 17:04:56.000000 django-twilio-0.9.3/docs/source/gotchas.rst
+-rw-rw-r--   0 jason     (1000) jason     (1000)     8991 2018-02-04 17:04:56.000000 django-twilio-0.9.3/docs/source/conf.py
+-rw-r--r--   0 jason     (1000) jason     (1000)     3722 2018-03-02 02:51:00.000000 django-twilio-0.9.3/docs/source/decorators.rst
+-rw-rw-r--   0 jason     (1000) jason     (1000)     5226 2018-02-04 17:04:56.000000 django-twilio-0.9.3/docs/source/install.rst
+-rw-r--r--   0 jason     (1000) jason     (1000)     1825 2018-03-02 02:51:00.000000 django-twilio-0.9.3/docs/source/requests.rst
+-rw-rw-r--   0 jason     (1000) jason     (1000)     3243 2018-02-04 17:04:56.000000 django-twilio-0.9.3/docs/source/rest.rst
+-rw-rw-r--   0 jason     (1000) jason     (1000)     1295 2018-02-04 17:04:56.000000 django-twilio-0.9.3/docs/source/contributors.rst
+-rw-rw-r--   0 jason     (1000) jason     (1000)     2096 2018-02-04 17:04:56.000000 django-twilio-0.9.3/docs/source/howto.rst
+-rw-rw-r--   0 jason     (1000) jason     (1000)     2498 2018-02-04 17:04:56.000000 django-twilio-0.9.3/docs/source/foreword.rst
+-rw-rw-r--   0 jason     (1000) jason     (1000)     2853 2018-02-04 17:04:56.000000 django-twilio-0.9.3/docs/source/settings.rst
+-rw-rw-r--   0 jason     (1000) jason     (1000)     4752 2018-02-04 17:04:56.000000 django-twilio-0.9.3/docs/source/contribute.rst
+-rw-rw-r--   0 jason     (1000) jason     (1000)     1979 2018-08-16 00:52:12.000000 django-twilio-0.9.3/docs/source/index.rst
+-rw-rw-r--   0 jason     (1000) jason     (1000)     4622 2017-12-29 01:02:24.000000 django-twilio-0.9.3/docs/Makefile
+-rw-rw-r--   0 jason     (1000) jason     (1000)      240 2018-02-04 17:04:56.000000 django-twilio-0.9.3/MANIFEST.in
+-rw-rw-r--   0 jason     (1000) jason     (1000)       61 2018-08-16 00:52:36.000000 django-twilio-0.9.3/setup.cfg
+-rw-rw-r--   0 jason     (1000) jason     (1000)     1403 2018-08-16 00:52:12.000000 django-twilio-0.9.3/README.rst
+drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2018-08-16 00:52:36.000000 django-twilio-0.9.3/django_twilio/
+-rw-rw-r--   0 jason     (1000) jason     (1000)     4173 2018-02-06 01:43:33.000000 django-twilio-0.9.3/django_twilio/decorators.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)     2004 2018-02-04 17:04:56.000000 django-twilio-0.9.3/django_twilio/models.py
+drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2018-08-16 00:52:36.000000 django-twilio-0.9.3/django_twilio/south_migrations/
+-rw-rw-r--   0 jason     (1000) jason     (1000)        1 2018-02-04 17:04:56.000000 django-twilio-0.9.3/django_twilio/south_migrations/__init__.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)     5693 2018-02-04 17:04:56.000000 django-twilio-0.9.3/django_twilio/south_migrations/0001_initial.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)     5088 2018-04-18 22:36:25.000000 django-twilio-0.9.3/django_twilio/views.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)      575 2018-02-04 17:04:56.000000 django-twilio-0.9.3/django_twilio/admin.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)      242 2018-02-04 17:04:56.000000 django-twilio-0.9.3/django_twilio/settings.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)     3005 2018-08-04 17:08:39.000000 django-twilio-0.9.3/django_twilio/utils.py
+drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2018-08-16 00:52:36.000000 django-twilio-0.9.3/django_twilio/migrations/
+-rw-rw-r--   0 jason     (1000) jason     (1000)        0 2017-12-29 01:02:24.000000 django-twilio-0.9.3/django_twilio/migrations/__init__.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)     1401 2018-02-04 17:04:56.000000 django-twilio-0.9.3/django_twilio/migrations/0001_initial.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)      286 2018-02-04 17:04:56.000000 django-twilio-0.9.3/django_twilio/client.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)       79 2018-02-04 17:04:56.000000 django-twilio-0.9.3/django_twilio/exceptions.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)      174 2018-02-06 03:36:19.000000 django-twilio-0.9.3/django_twilio/__init__.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)     1548 2018-02-04 17:04:56.000000 django-twilio-0.9.3/django_twilio/request.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)     3117 2018-08-16 00:52:36.000000 django-twilio-0.9.3/PKG-INFO
+-rw-rw-r--   0 jason     (1000) jason     (1000)      474 2018-02-04 17:04:56.000000 django-twilio-0.9.3/AUTHORS
```

### Comparing `django-twilio-0.9.2/UNLICENSE` & `django-twilio-0.9.3/UNLICENSE`

 * *Files identical despite different names*

### Comparing `django-twilio-0.9.2/test_project/test_app/decorators.py` & `django-twilio-0.9.3/test_project/test_app/decorators.py`

 * *Files identical despite different names*

### Comparing `django-twilio-0.9.2/test_project/test_app/models.py` & `django-twilio-0.9.3/test_project/test_app/models.py`

 * *Files identical despite different names*

### Comparing `django-twilio-0.9.2/test_project/test_app/urls.py` & `django-twilio-0.9.3/test_project/test_app/urls.py`

 * *Files identical despite different names*

### Comparing `django-twilio-0.9.2/test_project/test_app/views.py` & `django-twilio-0.9.3/test_project/test_app/views.py`

 * *Files identical despite different names*

### Comparing `django-twilio-0.9.2/test_project/test_app/utils.py` & `django-twilio-0.9.3/test_project/test_app/utils.py`

 * *Files identical despite different names*

### Comparing `django-twilio-0.9.2/test_project/test_app/client.py` & `django-twilio-0.9.3/test_project/test_app/client.py`

 * *Files identical despite different names*

### Comparing `django-twilio-0.9.2/test_project/test_app/request.py` & `django-twilio-0.9.3/test_project/test_app/request.py`

 * *Files identical despite different names*

### Comparing `django-twilio-0.9.2/test_project/settings.py` & `django-twilio-0.9.3/test_project/settings.py`

 * *Files identical despite different names*

### Comparing `django-twilio-0.9.2/django_twilio.egg-info/SOURCES.txt` & `django-twilio-0.9.3/django_twilio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-twilio-0.9.2/django_twilio.egg-info/PKG-INFO` & `django-twilio-0.9.3/django_twilio.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: django-twilio
-Version: 0.9.2
+Version: 0.9.3
 Summary: Build Twilio functionality into your Django apps.
 Home-page: https://github.com/rdegges/django-twilio
 Author: Randall Degges
 Author-email: rdegges@gmail.com
 License: UNLICENSE
 Description-Content-Type: UNKNOWN
 Description: =============
@@ -40,15 +40,15 @@
         
         Twilio makes it easy to send & receive SMS messages, and create & manage voice calls through software.
         
         Django-twilio makes it easy to use Twilio in your Django projects.
         
         Version 0.9.0 supports twilio 6.x and django 1.8-2.0.
         
-        Version 0.9.2 has minimal py3.7 and also allows django 2.1
+        Version 0.9.2 has minimal py3.7 support and 0.9.2 & 0.9.3 also allows django 2.1
         
         For legacy twilio (5.x SDK), please see the 0.8 version.
         
         Documentation
         -------------
         
         The documentation is hosted at ReadTheDocs. You can check out the docs
```

### Comparing `django-twilio-0.9.2/setup.py` & `django-twilio-0.9.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from setuptools import find_packages, setup
 
 
 setup(
 
     # Basic package information:
     name='django-twilio',
-    version='0.9.2',
+    version='0.9.3',
     packages=find_packages(),
 
     # Packaging options:
     zip_safe=False,
     include_package_data=True,
 
     # Package dependencies:
```

### Comparing `django-twilio-0.9.2/docs/source/views.rst` & `django-twilio-0.9.3/docs/source/views.rst`

 * *Files identical despite different names*

### Comparing `django-twilio-0.9.2/docs/source/gotchas.rst` & `django-twilio-0.9.3/docs/source/gotchas.rst`

 * *Files identical despite different names*

### Comparing `django-twilio-0.9.2/docs/source/conf.py` & `django-twilio-0.9.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `django-twilio-0.9.2/docs/source/decorators.rst` & `django-twilio-0.9.3/docs/source/decorators.rst`

 * *Files identical despite different names*

### Comparing `django-twilio-0.9.2/docs/source/install.rst` & `django-twilio-0.9.3/docs/source/install.rst`

 * *Files identical despite different names*

### Comparing `django-twilio-0.9.2/docs/source/requests.rst` & `django-twilio-0.9.3/docs/source/requests.rst`

 * *Files identical despite different names*

### Comparing `django-twilio-0.9.2/docs/source/rest.rst` & `django-twilio-0.9.3/docs/source/rest.rst`

 * *Files identical despite different names*

### Comparing `django-twilio-0.9.2/docs/source/contributors.rst` & `django-twilio-0.9.3/docs/source/contributors.rst`

 * *Files identical despite different names*

### Comparing `django-twilio-0.9.2/docs/source/howto.rst` & `django-twilio-0.9.3/docs/source/howto.rst`

 * *Files identical despite different names*

### Comparing `django-twilio-0.9.2/docs/source/foreword.rst` & `django-twilio-0.9.3/docs/source/foreword.rst`

 * *Files identical despite different names*

### Comparing `django-twilio-0.9.2/docs/source/settings.rst` & `django-twilio-0.9.3/docs/source/settings.rst`

 * *Files identical despite different names*

### Comparing `django-twilio-0.9.2/docs/source/contribute.rst` & `django-twilio-0.9.3/docs/source/contribute.rst`

 * *Files identical despite different names*

### Comparing `django-twilio-0.9.2/docs/source/index.rst` & `django-twilio-0.9.3/docs/source/index.rst`

 * *Files 9% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
 User's Guide
 ------------
 
 
 Version 0.9.0 supports twilio 6.x and django 1.8-2.0.
 
-Version 0.9.2 has minimal py3.7 and also allows django 2.1
+Version 0.9.2 has minimal py3.7 support and 0.9.2 & 0.9.3 also allows django 2.1
 
 For legacy twilio (5.x SDK), please see the 0.8 version.
 
 
 This part of the documentation contains an extensive walk through of
 django-twilio. It begins with some background information about django-twilio,
 then focuses on step-by-step integration of django-twilio into your existing
```

### Comparing `django-twilio-0.9.2/docs/Makefile` & `django-twilio-0.9.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-twilio-0.9.2/README.rst` & `django-twilio-0.9.3/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 Twilio makes it easy to send & receive SMS messages, and create & manage voice calls through software.
 
 Django-twilio makes it easy to use Twilio in your Django projects.
 
 Version 0.9.0 supports twilio 6.x and django 1.8-2.0.
 
-Version 0.9.2 has minimal py3.7 and also allows django 2.1
+Version 0.9.2 has minimal py3.7 support and 0.9.2 & 0.9.3 also allows django 2.1
 
 For legacy twilio (5.x SDK), please see the 0.8 version.
 
 Documentation
 -------------
 
 The documentation is hosted at ReadTheDocs. You can check out the docs
```

### Comparing `django-twilio-0.9.2/django_twilio/decorators.py` & `django-twilio-0.9.3/django_twilio/decorators.py`

 * *Files identical despite different names*

### Comparing `django-twilio-0.9.2/django_twilio/models.py` & `django-twilio-0.9.3/django_twilio/models.py`

 * *Files identical despite different names*

### Comparing `django-twilio-0.9.2/django_twilio/south_migrations/0001_initial.py` & `django-twilio-0.9.3/django_twilio/south_migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-twilio-0.9.2/django_twilio/views.py` & `django-twilio-0.9.3/django_twilio/views.py`

 * *Files identical despite different names*

### Comparing `django-twilio-0.9.2/django_twilio/admin.py` & `django-twilio-0.9.3/django_twilio/admin.py`

 * *Files identical despite different names*

### Comparing `django-twilio-0.9.2/django_twilio/utils.py` & `django-twilio-0.9.3/django_twilio/utils.py`

 * *Files identical despite different names*

### Comparing `django-twilio-0.9.2/django_twilio/migrations/0001_initial.py` & `django-twilio-0.9.3/django_twilio/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-twilio-0.9.2/django_twilio/request.py` & `django-twilio-0.9.3/django_twilio/request.py`

 * *Files identical despite different names*

### Comparing `django-twilio-0.9.2/PKG-INFO` & `django-twilio-0.9.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: django-twilio
-Version: 0.9.2
+Version: 0.9.3
 Summary: Build Twilio functionality into your Django apps.
 Home-page: https://github.com/rdegges/django-twilio
 Author: Randall Degges
 Author-email: rdegges@gmail.com
 License: UNLICENSE
 Description-Content-Type: UNKNOWN
 Description: =============
@@ -40,15 +40,15 @@
         
         Twilio makes it easy to send & receive SMS messages, and create & manage voice calls through software.
         
         Django-twilio makes it easy to use Twilio in your Django projects.
         
         Version 0.9.0 supports twilio 6.x and django 1.8-2.0.
         
-        Version 0.9.2 has minimal py3.7 and also allows django 2.1
+        Version 0.9.2 has minimal py3.7 support and 0.9.2 & 0.9.3 also allows django 2.1
         
         For legacy twilio (5.x SDK), please see the 0.8 version.
         
         Documentation
         -------------
         
         The documentation is hosted at ReadTheDocs. You can check out the docs
```

