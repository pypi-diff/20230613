# Comparing `tmp/django-better-migrations-0.0.3.tar.gz` & `tmp/django-better-migrations-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-better-migrations-0.0.3.tar", last modified: Fri May 18 19:48:23 2018, max compression
+gzip compressed data, was "dist/django-better-migrations-0.0.4.tar", last modified: Thu Aug 16 15:34:17 2018, max compression
```

## Comparing `django-better-migrations-0.0.3.tar` & `django-better-migrations-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 jbbarth    (501) staff       (20)        0 2018-05-18 19:48:23.000000 django-better-migrations-0.0.3/
--rw-r--r--   0 jbbarth    (501) staff       (20)     2464 2018-05-18 19:48:23.000000 django-better-migrations-0.0.3/PKG-INFO
--rw-r--r--   0 jbbarth    (501) staff       (20)     1088 2017-12-18 08:58:28.000000 django-better-migrations-0.0.3/LICENSE
-drwxr-xr-x   0 jbbarth    (501) staff       (20)        0 2018-05-18 19:48:23.000000 django-better-migrations-0.0.3/django_better_migrations.egg-info/
--rw-r--r--   0 jbbarth    (501) staff       (20)     2464 2018-05-18 19:48:23.000000 django-better-migrations-0.0.3/django_better_migrations.egg-info/PKG-INFO
--rw-r--r--   0 jbbarth    (501) staff       (20)      397 2018-05-18 19:48:23.000000 django-better-migrations-0.0.3/django_better_migrations.egg-info/SOURCES.txt
--rw-r--r--   0 jbbarth    (501) staff       (20)       25 2018-05-18 19:48:23.000000 django-better-migrations-0.0.3/django_better_migrations.egg-info/top_level.txt
--rw-r--r--   0 jbbarth    (501) staff       (20)        1 2018-05-18 19:48:23.000000 django-better-migrations-0.0.3/django_better_migrations.egg-info/dependency_links.txt
--rw-r--r--   0 jbbarth    (501) staff       (20)       27 2017-12-18 08:58:28.000000 django-better-migrations-0.0.3/MANIFEST.in
--rw-r--r--   0 jbbarth    (501) staff       (20)     1412 2017-12-18 11:15:10.000000 django-better-migrations-0.0.3/README.md
--rw-r--r--   0 jbbarth    (501) staff       (20)     1052 2017-12-18 08:58:28.000000 django-better-migrations-0.0.3/setup.py
--rw-r--r--   0 jbbarth    (501) staff       (20)      252 2018-05-18 19:48:23.000000 django-better-migrations-0.0.3/setup.cfg
-drwxr-xr-x   0 jbbarth    (501) staff       (20)        0 2018-05-18 19:48:23.000000 django-better-migrations-0.0.3/django_better_migrations/
--rw-r--r--   0 jbbarth    (501) staff       (20)      789 2018-05-18 19:47:49.000000 django-better-migrations-0.0.3/django_better_migrations/config.py
--rw-r--r--   0 jbbarth    (501) staff       (20)       95 2018-05-18 19:47:55.000000 django-better-migrations-0.0.3/django_better_migrations/__init__.py
--rw-r--r--   0 jbbarth    (501) staff       (20)      394 2017-12-18 11:06:22.000000 django-better-migrations-0.0.3/django_better_migrations/rules.py
--rw-r--r--   0 jbbarth    (501) staff       (20)     2541 2018-05-18 19:47:49.000000 django-better-migrations-0.0.3/django_better_migrations/migration_writer_patch.py
+drwxr-xr-x   0 jbbarth    (501) staff       (20)        0 2018-08-16 15:34:17.000000 django-better-migrations-0.0.4/
+-rw-r--r--   0 jbbarth    (501) staff       (20)     2472 2018-08-16 15:34:17.000000 django-better-migrations-0.0.4/PKG-INFO
+-rw-r--r--   0 jbbarth    (501) staff       (20)     1088 2017-12-18 08:58:28.000000 django-better-migrations-0.0.4/LICENSE
+drwxr-xr-x   0 jbbarth    (501) staff       (20)        0 2018-08-16 15:34:17.000000 django-better-migrations-0.0.4/django_better_migrations.egg-info/
+-rw-r--r--   0 jbbarth    (501) staff       (20)     2472 2018-08-16 15:34:17.000000 django-better-migrations-0.0.4/django_better_migrations.egg-info/PKG-INFO
+-rw-r--r--   0 jbbarth    (501) staff       (20)      397 2018-08-16 15:34:17.000000 django-better-migrations-0.0.4/django_better_migrations.egg-info/SOURCES.txt
+-rw-r--r--   0 jbbarth    (501) staff       (20)       25 2018-08-16 15:34:17.000000 django-better-migrations-0.0.4/django_better_migrations.egg-info/top_level.txt
+-rw-r--r--   0 jbbarth    (501) staff       (20)        1 2018-08-16 15:34:17.000000 django-better-migrations-0.0.4/django_better_migrations.egg-info/dependency_links.txt
+-rw-r--r--   0 jbbarth    (501) staff       (20)       27 2017-12-18 08:58:28.000000 django-better-migrations-0.0.4/MANIFEST.in
+-rw-r--r--   0 jbbarth    (501) staff       (20)     1420 2018-08-16 15:29:40.000000 django-better-migrations-0.0.4/README.md
+-rw-r--r--   0 jbbarth    (501) staff       (20)     1052 2017-12-18 08:58:28.000000 django-better-migrations-0.0.4/setup.py
+-rw-r--r--   0 jbbarth    (501) staff       (20)      231 2018-08-16 15:34:17.000000 django-better-migrations-0.0.4/setup.cfg
+drwxr-xr-x   0 jbbarth    (501) staff       (20)        0 2018-08-16 15:34:17.000000 django-better-migrations-0.0.4/django_better_migrations/
+-rw-r--r--   0 jbbarth    (501) staff       (20)      789 2018-05-18 19:47:49.000000 django-better-migrations-0.0.4/django_better_migrations/config.py
+-rw-r--r--   0 jbbarth    (501) staff       (20)       95 2018-08-16 15:29:48.000000 django-better-migrations-0.0.4/django_better_migrations/__init__.py
+-rw-r--r--   0 jbbarth    (501) staff       (20)      465 2018-08-16 15:29:40.000000 django-better-migrations-0.0.4/django_better_migrations/rules.py
+-rw-r--r--   0 jbbarth    (501) staff       (20)     2541 2018-05-18 19:47:49.000000 django-better-migrations-0.0.4/django_better_migrations/migration_writer_patch.py
```

### Comparing `django-better-migrations-0.0.3/PKG-INFO` & `django-better-migrations-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 1.1
 Name: django-better-migrations
-Version: 0.0.3
+Version: 0.0.4
 Summary: Improves Django migration system.
 Home-page: http://github.com/botify-labs/django-better-migrations
 Author: Jean-Baptiste Barth
 Author-email: jeanbaptiste.barth@gmail.com
 License: MIT
 Description: Django Better Migrations
         ========================
         
-        [![Build Status](https://travis-ci.org/jbbarth/django-better-migrations.svg?branch=master)](https://travis-ci.org/jbbarth/django-better-migrations)
+        [![Build Status](https://travis-ci.org/botify-labs/django-better-migrations.svg?branch=master)](https://travis-ci.org/botify-labs/django-better-migrations)
         
         This project aims at providing improvements to Django's default migration system.
         The default migration system is over-engineered, sometimes dangerous, and not
         team work friendly.
         
         
         More informations in the documentation, see "docs/" folder.
```

### Comparing `django-better-migrations-0.0.3/LICENSE` & `django-better-migrations-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django-better-migrations-0.0.3/django_better_migrations.egg-info/PKG-INFO` & `django-better-migrations-0.0.4/django_better_migrations.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 1.1
 Name: django-better-migrations
-Version: 0.0.3
+Version: 0.0.4
 Summary: Improves Django migration system.
 Home-page: http://github.com/botify-labs/django-better-migrations
 Author: Jean-Baptiste Barth
 Author-email: jeanbaptiste.barth@gmail.com
 License: MIT
 Description: Django Better Migrations
         ========================
         
-        [![Build Status](https://travis-ci.org/jbbarth/django-better-migrations.svg?branch=master)](https://travis-ci.org/jbbarth/django-better-migrations)
+        [![Build Status](https://travis-ci.org/botify-labs/django-better-migrations.svg?branch=master)](https://travis-ci.org/botify-labs/django-better-migrations)
         
         This project aims at providing improvements to Django's default migration system.
         The default migration system is over-engineered, sometimes dangerous, and not
         team work friendly.
         
         
         More informations in the documentation, see "docs/" folder.
```

### Comparing `django-better-migrations-0.0.3/README.md` & `django-better-migrations-0.0.4/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Django Better Migrations
 ========================
 
-[![Build Status](https://travis-ci.org/jbbarth/django-better-migrations.svg?branch=master)](https://travis-ci.org/jbbarth/django-better-migrations)
+[![Build Status](https://travis-ci.org/botify-labs/django-better-migrations.svg?branch=master)](https://travis-ci.org/botify-labs/django-better-migrations)
 
 This project aims at providing improvements to Django's default migration system.
 The default migration system is over-engineered, sometimes dangerous, and not
 team work friendly.
 
 
 More informations in the documentation, see "docs/" folder.
```

### Comparing `django-better-migrations-0.0.3/setup.py` & `django-better-migrations-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `django-better-migrations-0.0.3/django_better_migrations/config.py` & `django-better-migrations-0.0.4/django_better_migrations/config.py`

 * *Files identical despite different names*

### Comparing `django-better-migrations-0.0.3/django_better_migrations/migration_writer_patch.py` & `django-better-migrations-0.0.4/django_better_migrations/migration_writer_patch.py`

 * *Files identical despite different names*

