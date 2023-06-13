# Comparing `tmp/django-sweet-utils-1.3.4.tar.gz` & `tmp/django-sweet-utils-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-sweet-utils-1.3.4.tar", last modified: Thu May 25 16:25:25 2023, max compression
+gzip compressed data, was "django-sweet-utils-1.4.0.tar", last modified: Tue Jun 13 12:00:11 2023, max compression
```

## Comparing `django-sweet-utils-1.3.4.tar` & `django-sweet-utils-1.4.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-05-25 16:25:25.633954 django-sweet-utils-1.3.4/
--rw-r--r--   0 rustam     (501) staff       (20)     1545 2022-11-29 11:14:37.000000 django-sweet-utils-1.3.4/LICENSE
--rw-r--r--   0 rustam     (501) staff       (20)       58 2022-11-29 11:14:37.000000 django-sweet-utils-1.3.4/MANIFEST.in
--rw-r--r--   0 rustam     (501) staff       (20)     3043 2023-05-25 16:25:25.634158 django-sweet-utils-1.3.4/PKG-INFO
--rw-r--r--   0 rustam     (501) staff       (20)     1677 2022-11-29 11:14:37.000000 django-sweet-utils-1.3.4/README.md
-drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-05-25 16:25:25.623589 django-sweet-utils-1.3.4/django_sweet_utils/
--rw-r--r--   0 rustam     (501) staff       (20)        0 2022-11-29 11:14:37.000000 django-sweet-utils-1.3.4/django_sweet_utils/__init__.py
-drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-05-25 16:25:25.625658 django-sweet-utils-1.3.4/django_sweet_utils/admin/
--rw-r--r--   0 rustam     (501) staff       (20)        0 2023-05-25 16:24:12.000000 django-sweet-utils-1.3.4/django_sweet_utils/admin/__init__.py
--rw-r--r--   0 rustam     (501) staff       (20)      253 2023-05-25 16:25:07.000000 django-sweet-utils-1.3.4/django_sweet_utils/admin/actions.py
-drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-05-25 16:25:25.627898 django-sweet-utils-1.3.4/django_sweet_utils/api/
--rw-r--r--   0 rustam     (501) staff       (20)        0 2022-11-29 11:14:37.000000 django-sweet-utils-1.3.4/django_sweet_utils/api/__init__.py
--rw-r--r--   0 rustam     (501) staff       (20)     1438 2023-02-24 11:38:03.000000 django-sweet-utils-1.3.4/django_sweet_utils/api/metadata.py
--rw-r--r--   0 rustam     (501) staff       (20)      246 2023-02-24 12:25:50.000000 django-sweet-utils-1.3.4/django_sweet_utils/api/permissions.py
--rw-r--r--   0 rustam     (501) staff       (20)      962 2022-11-29 11:14:37.000000 django-sweet-utils-1.3.4/django_sweet_utils/api/views.py
--rw-r--r--   0 rustam     (501) staff       (20)      166 2022-11-29 11:14:37.000000 django-sweet-utils-1.3.4/django_sweet_utils/apps.py
-drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-05-25 16:25:25.628599 django-sweet-utils-1.3.4/django_sweet_utils/db/
--rw-r--r--   0 rustam     (501) staff       (20)        0 2022-11-29 11:14:37.000000 django-sweet-utils-1.3.4/django_sweet_utils/db/__init__.py
--rw-r--r--   0 rustam     (501) staff       (20)     2232 2023-05-25 16:16:51.000000 django-sweet-utils-1.3.4/django_sweet_utils/db/models.py
-drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-05-25 16:25:25.630290 django-sweet-utils-1.3.4/django_sweet_utils/misc/
--rw-r--r--   0 rustam     (501) staff       (20)        0 2022-11-29 11:14:37.000000 django-sweet-utils-1.3.4/django_sweet_utils/misc/__init__.py
--rw-r--r--   0 rustam     (501) staff       (20)      342 2022-12-22 11:02:57.000000 django-sweet-utils-1.3.4/django_sweet_utils/misc/json.py
--rw-r--r--   0 rustam     (501) staff       (20)     1465 2022-12-20 04:47:46.000000 django-sweet-utils-1.3.4/django_sweet_utils/misc/logging.py
-drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-05-25 16:25:25.631196 django-sweet-utils-1.3.4/django_sweet_utils/serializers/
--rw-r--r--   0 rustam     (501) staff       (20)        0 2023-01-26 10:20:33.000000 django-sweet-utils-1.3.4/django_sweet_utils/serializers/__init__.py
--rw-r--r--   0 rustam     (501) staff       (20)     1213 2023-02-10 07:18:14.000000 django-sweet-utils-1.3.4/django_sweet_utils/serializers/fields.py
-drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-05-25 16:25:25.633162 django-sweet-utils-1.3.4/django_sweet_utils/templatetags/
--rw-r--r--   0 rustam     (501) staff       (20)        0 2022-11-25 06:53:25.000000 django-sweet-utils-1.3.4/django_sweet_utils/templatetags/__init__.py
--rw-r--r--   0 rustam     (501) staff       (20)      169 2022-11-25 06:53:25.000000 django-sweet-utils-1.3.4/django_sweet_utils/templatetags/format_str.py
--rw-r--r--   0 rustam     (501) staff       (20)     4670 2022-11-25 06:53:25.000000 django-sweet-utils-1.3.4/django_sweet_utils/templatetags/query_string.py
-drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-05-25 16:25:25.625140 django-sweet-utils-1.3.4/django_sweet_utils.egg-info/
--rw-r--r--   0 rustam     (501) staff       (20)     3043 2023-05-25 16:25:25.000000 django-sweet-utils-1.3.4/django_sweet_utils.egg-info/PKG-INFO
--rw-r--r--   0 rustam     (501) staff       (20)      919 2023-05-25 16:25:25.000000 django-sweet-utils-1.3.4/django_sweet_utils.egg-info/SOURCES.txt
--rw-r--r--   0 rustam     (501) staff       (20)        1 2023-05-25 16:25:25.000000 django-sweet-utils-1.3.4/django_sweet_utils.egg-info/dependency_links.txt
--rw-r--r--   0 rustam     (501) staff       (20)       32 2023-05-25 16:25:25.000000 django-sweet-utils-1.3.4/django_sweet_utils.egg-info/requires.txt
--rw-r--r--   0 rustam     (501) staff       (20)       19 2023-05-25 16:25:25.000000 django-sweet-utils-1.3.4/django_sweet_utils.egg-info/top_level.txt
--rw-r--r--   0 rustam     (501) staff       (20)     1212 2023-05-25 16:25:25.634909 django-sweet-utils-1.3.4/setup.cfg
--rw-r--r--   0 rustam     (501) staff       (20)      195 2022-11-29 11:14:37.000000 django-sweet-utils-1.3.4/setup.py
+drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-06-13 12:00:11.711107 django-sweet-utils-1.4.0/
+-rw-r--r--   0 rustam     (501) staff       (20)     1063 2023-06-13 11:36:27.000000 django-sweet-utils-1.4.0/LICENSE
+-rw-r--r--   0 rustam     (501) staff       (20)       58 2022-11-29 11:14:37.000000 django-sweet-utils-1.4.0/MANIFEST.in
+-rw-r--r--   0 rustam     (501) staff       (20)     6484 2023-06-13 12:00:11.711296 django-sweet-utils-1.4.0/PKG-INFO
+-rw-r--r--   0 rustam     (501) staff       (20)     5119 2023-06-13 11:58:13.000000 django-sweet-utils-1.4.0/README.md
+drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-06-13 12:00:11.684834 django-sweet-utils-1.4.0/django_sweet_utils/
+-rw-r--r--   0 rustam     (501) staff       (20)        0 2022-11-29 11:14:37.000000 django-sweet-utils-1.4.0/django_sweet_utils/__init__.py
+drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-06-13 12:00:11.687579 django-sweet-utils-1.4.0/django_sweet_utils/admin/
+-rw-r--r--   0 rustam     (501) staff       (20)        0 2023-05-25 16:24:12.000000 django-sweet-utils-1.4.0/django_sweet_utils/admin/__init__.py
+-rw-r--r--   0 rustam     (501) staff       (20)      253 2023-05-25 16:25:07.000000 django-sweet-utils-1.4.0/django_sweet_utils/admin/actions.py
+drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-06-13 12:00:11.689773 django-sweet-utils-1.4.0/django_sweet_utils/api/
+-rw-r--r--   0 rustam     (501) staff       (20)        0 2022-11-29 11:14:37.000000 django-sweet-utils-1.4.0/django_sweet_utils/api/__init__.py
+-rw-r--r--   0 rustam     (501) staff       (20)     1438 2023-02-24 11:38:03.000000 django-sweet-utils-1.4.0/django_sweet_utils/api/metadata.py
+-rw-r--r--   0 rustam     (501) staff       (20)      246 2023-02-24 12:25:50.000000 django-sweet-utils-1.4.0/django_sweet_utils/api/permissions.py
+-rw-r--r--   0 rustam     (501) staff       (20)      962 2023-06-13 11:41:06.000000 django-sweet-utils-1.4.0/django_sweet_utils/api/views.py
+-rw-r--r--   0 rustam     (501) staff       (20)      166 2022-11-29 11:14:37.000000 django-sweet-utils-1.4.0/django_sweet_utils/apps.py
+drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-06-13 12:00:11.690592 django-sweet-utils-1.4.0/django_sweet_utils/db/
+-rw-r--r--   0 rustam     (501) staff       (20)        0 2022-11-29 11:14:37.000000 django-sweet-utils-1.4.0/django_sweet_utils/db/__init__.py
+-rw-r--r--   0 rustam     (501) staff       (20)     2232 2023-05-25 16:16:51.000000 django-sweet-utils-1.4.0/django_sweet_utils/db/models.py
+drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-06-13 12:00:11.692247 django-sweet-utils-1.4.0/django_sweet_utils/misc/
+-rw-r--r--   0 rustam     (501) staff       (20)        0 2022-11-29 11:14:37.000000 django-sweet-utils-1.4.0/django_sweet_utils/misc/__init__.py
+-rw-r--r--   0 rustam     (501) staff       (20)      342 2022-12-22 11:02:57.000000 django-sweet-utils-1.4.0/django_sweet_utils/misc/json.py
+-rw-r--r--   0 rustam     (501) staff       (20)     1462 2023-06-13 11:58:13.000000 django-sweet-utils-1.4.0/django_sweet_utils/misc/logging.py
+drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-06-13 12:00:11.693118 django-sweet-utils-1.4.0/django_sweet_utils/serializers/
+-rw-r--r--   0 rustam     (501) staff       (20)        0 2023-01-26 10:20:33.000000 django-sweet-utils-1.4.0/django_sweet_utils/serializers/__init__.py
+-rw-r--r--   0 rustam     (501) staff       (20)     1213 2023-02-10 07:18:14.000000 django-sweet-utils-1.4.0/django_sweet_utils/serializers/fields.py
+drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-06-13 12:00:11.710645 django-sweet-utils-1.4.0/django_sweet_utils/templatetags/
+-rw-r--r--   0 rustam     (501) staff       (20)        0 2022-11-25 06:53:25.000000 django-sweet-utils-1.4.0/django_sweet_utils/templatetags/__init__.py
+-rw-r--r--   0 rustam     (501) staff       (20)      169 2022-11-25 06:53:25.000000 django-sweet-utils-1.4.0/django_sweet_utils/templatetags/format_str.py
+-rw-r--r--   0 rustam     (501) staff       (20)     4670 2022-11-25 06:53:25.000000 django-sweet-utils-1.4.0/django_sweet_utils/templatetags/query_string.py
+drwxr-xr-x   0 rustam     (501) staff       (20)        0 2023-06-13 12:00:11.687003 django-sweet-utils-1.4.0/django_sweet_utils.egg-info/
+-rw-r--r--   0 rustam     (501) staff       (20)     6484 2023-06-13 12:00:11.000000 django-sweet-utils-1.4.0/django_sweet_utils.egg-info/PKG-INFO
+-rw-r--r--   0 rustam     (501) staff       (20)      919 2023-06-13 12:00:11.000000 django-sweet-utils-1.4.0/django_sweet_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 rustam     (501) staff       (20)        1 2023-06-13 12:00:11.000000 django-sweet-utils-1.4.0/django_sweet_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 rustam     (501) staff       (20)       32 2023-06-13 12:00:11.000000 django-sweet-utils-1.4.0/django_sweet_utils.egg-info/requires.txt
+-rw-r--r--   0 rustam     (501) staff       (20)       19 2023-06-13 12:00:11.000000 django-sweet-utils-1.4.0/django_sweet_utils.egg-info/top_level.txt
+-rw-r--r--   0 rustam     (501) staff       (20)     1211 2023-06-13 12:00:11.712115 django-sweet-utils-1.4.0/setup.cfg
+-rw-r--r--   0 rustam     (501) staff       (20)      195 2022-11-29 11:14:37.000000 django-sweet-utils-1.4.0/setup.py
```

### Comparing `django-sweet-utils-1.3.4/django_sweet_utils/api/metadata.py` & `django-sweet-utils-1.4.0/django_sweet_utils/api/metadata.py`

 * *Files identical despite different names*

### Comparing `django-sweet-utils-1.3.4/django_sweet_utils/api/views.py` & `django-sweet-utils-1.4.0/django_sweet_utils/api/views.py`

 * *Files identical despite different names*

### Comparing `django-sweet-utils-1.3.4/django_sweet_utils/db/models.py` & `django-sweet-utils-1.4.0/django_sweet_utils/db/models.py`

 * *Files identical despite different names*

### Comparing `django-sweet-utils-1.3.4/django_sweet_utils/misc/logging.py` & `django-sweet-utils-1.4.0/django_sweet_utils/misc/logging.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,15 +14,15 @@
             context.pop('request')
         except KeyError:
             pass
 
         return {
             'message': message,
             'level': record.levelname,
-            'app': settings.APP_LABEL + '_' + settings.RUNNING_BRANCH,
+            'app': settings.APP_LABEL + '_' + settings.ENVIRONMENT,
             **context
         }
 
 
 class CustomFilter(logging.Filter):
 
     def filter(self, record):
```

### Comparing `django-sweet-utils-1.3.4/django_sweet_utils/serializers/fields.py` & `django-sweet-utils-1.4.0/django_sweet_utils/serializers/fields.py`

 * *Files identical despite different names*

### Comparing `django-sweet-utils-1.3.4/django_sweet_utils/templatetags/query_string.py` & `django-sweet-utils-1.4.0/django_sweet_utils/templatetags/query_string.py`

 * *Files identical despite different names*

### Comparing `django-sweet-utils-1.3.4/django_sweet_utils.egg-info/SOURCES.txt` & `django-sweet-utils-1.4.0/django_sweet_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-sweet-utils-1.3.4/setup.cfg` & `django-sweet-utils-1.4.0/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [metadata]
 name = django-sweet-utils
-version = 1.3.4
+version = 1.4.0
 description = A little django code sugar.
-url = https://github.com/HarleyK1ng/django-sweet-utils
+url = https://github.com/AllYouZombies/django-sweet-utils
 author = Astafeev Rustam
-author_email = astafeev0308@gmail.com
-license = BSD-3-Clause
+author_email = rustam@astafeev.dev
+license = MIT License
 classifiers = 
 	Environment :: Web Environment
 	Framework :: Django
 	Framework :: Django :: 3
 	Framework :: Django :: 3.0
 	Framework :: Django :: 3.1
 	Framework :: Django :: 3.2
 	Framework :: Django :: 4
 	Framework :: Django :: 4.0
 	Framework :: Django :: 4.1
 	Intended Audience :: Developers
-	License :: OSI Approved :: BSD License
+	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
```

