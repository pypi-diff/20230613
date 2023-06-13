# Comparing `tmp/django-easy-audit-1.3.4b2.tar.gz` & `tmp/django-easy-audit-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-easy-audit-1.3.4b2.tar", last modified: Wed Apr 19 15:38:19 2023, max compression
+gzip compressed data, was "django-easy-audit-1.3.5.tar", last modified: Tue Jun 13 14:39:01 2023, max compression
```

## Comparing `django-easy-audit-1.3.4b2.tar` & `django-easy-audit-1.3.5.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2023-04-19 15:38:19.049323 django-easy-audit-1.3.4b2/
--rw-r--r--   0 jason     (1000) jason     (1000)    35141 2020-02-02 14:58:04.000000 django-easy-audit-1.3.4b2/LICENSE
--rw-r--r--   0 jason     (1000) jason     (1000)      112 2020-02-02 14:58:04.000000 django-easy-audit-1.3.4b2/MANIFEST.in
--rw-rw-r--   0 jason     (1000) jason     (1000)     2030 2023-04-19 15:38:19.049323 django-easy-audit-1.3.4b2/PKG-INFO
--rw-r--r--   0 jason     (1000) jason     (1000)      787 2020-02-02 14:58:04.000000 django-easy-audit-1.3.4b2/README.rst
-drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2023-04-19 15:38:19.045323 django-easy-audit-1.3.4b2/django_easy_audit.egg-info/
--rw-rw-r--   0 jason     (1000) jason     (1000)     2030 2023-04-19 15:38:18.000000 django-easy-audit-1.3.4b2/django_easy_audit.egg-info/PKG-INFO
--rw-rw-r--   0 jason     (1000) jason     (1000)     1630 2023-04-19 15:38:19.000000 django-easy-audit-1.3.4b2/django_easy_audit.egg-info/SOURCES.txt
--rw-rw-r--   0 jason     (1000) jason     (1000)        1 2023-04-19 15:38:18.000000 django-easy-audit-1.3.4b2/django_easy_audit.egg-info/dependency_links.txt
--rw-rw-r--   0 jason     (1000) jason     (1000)       32 2023-04-19 15:38:18.000000 django-easy-audit-1.3.4b2/django_easy_audit.egg-info/requires.txt
--rw-rw-r--   0 jason     (1000) jason     (1000)       10 2023-04-19 15:38:19.000000 django-easy-audit-1.3.4b2/django_easy_audit.egg-info/top_level.txt
-drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2023-04-19 15:38:19.045323 django-easy-audit-1.3.4b2/easyaudit/
--rw-rw-r--   0 jason     (1000) jason     (1000)      101 2022-04-07 03:31:02.000000 django-easy-audit-1.3.4b2/easyaudit/__init__.py
--rw-rw-r--   0 jason     (1000) jason     (1000)     4461 2020-08-04 01:44:58.000000 django-easy-audit-1.3.4b2/easyaudit/admin.py
--rw-rw-r--   0 jason     (1000) jason     (1000)     5159 2022-05-24 18:10:15.000000 django-easy-audit-1.3.4b2/easyaudit/admin_helpers.py
--rw-rw-r--   0 jason     (1000) jason     (1000)      294 2022-02-25 18:56:54.000000 django-easy-audit-1.3.4b2/easyaudit/apps.py
--rw-rw-r--   0 jason     (1000) jason     (1000)      410 2020-08-04 01:44:58.000000 django-easy-audit-1.3.4b2/easyaudit/backends.py
--rw-rw-r--   0 jason     (1000) jason     (1000)     3693 2022-09-04 03:01:59.000000 django-easy-audit-1.3.4b2/easyaudit/crudhistory_admin_mixin.py
-drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2023-04-19 15:38:19.045323 django-easy-audit-1.3.4b2/easyaudit/middleware/
--rw-r--r--   0 jason     (1000) jason     (1000)        0 2020-02-02 14:58:04.000000 django-easy-audit-1.3.4b2/easyaudit/middleware/__init__.py
--rw-rw-r--   0 jason     (1000) jason     (1000)     1912 2020-08-07 17:56:33.000000 django-easy-audit-1.3.4b2/easyaudit/middleware/easyaudit.py
-drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2023-04-19 15:38:19.049323 django-easy-audit-1.3.4b2/easyaudit/migrations/
--rw-r--r--   0 jason     (1000) jason     (1000)     2290 2020-02-02 14:58:04.000000 django-easy-audit-1.3.4b2/easyaudit/migrations/0001_initial.py
--rw-r--r--   0 jason     (1000) jason     (1000)      812 2020-02-02 14:58:04.000000 django-easy-audit-1.3.4b2/easyaudit/migrations/0002_auto_20170125_0759.py
--rw-r--r--   0 jason     (1000) jason     (1000)      837 2020-02-02 14:58:04.000000 django-easy-audit-1.3.4b2/easyaudit/migrations/0003_auto_20170228_1505.py
--rw-r--r--   0 jason     (1000) jason     (1000)      496 2020-02-02 14:58:04.000000 django-easy-audit-1.3.4b2/easyaudit/migrations/0004_auto_20170620_1354.py
--rw-r--r--   0 jason     (1000) jason     (1000)      577 2020-02-02 14:58:04.000000 django-easy-audit-1.3.4b2/easyaudit/migrations/0005_auto_20170713_1155.py
--rw-r--r--   0 jason     (1000) jason     (1000)     1563 2020-02-02 14:58:04.000000 django-easy-audit-1.3.4b2/easyaudit/migrations/0006_auto_20171018_1242.py
--rw-r--r--   0 jason     (1000) jason     (1000)     1020 2020-02-02 14:58:04.000000 django-easy-audit-1.3.4b2/easyaudit/migrations/0007_auto_20180105_0838.py
--rw-r--r--   0 jason     (1000) jason     (1000)      704 2020-02-02 14:58:04.000000 django-easy-audit-1.3.4b2/easyaudit/migrations/0008_auto_20180220_1908.py
--rw-r--r--   0 jason     (1000) jason     (1000)      634 2020-02-02 14:58:04.000000 django-easy-audit-1.3.4b2/easyaudit/migrations/0009_auto_20180314_2225.py
--rw-r--r--   0 jason     (1000) jason     (1000)      404 2020-02-02 14:58:04.000000 django-easy-audit-1.3.4b2/easyaudit/migrations/0010_repr_text.py
--rw-r--r--   0 jason     (1000) jason     (1000)      432 2020-02-02 14:58:04.000000 django-easy-audit-1.3.4b2/easyaudit/migrations/0011_auto_20181101_1339.py
--rw-r--r--   0 jason     (1000) jason     (1000)     1519 2020-02-02 14:58:04.000000 django-easy-audit-1.3.4b2/easyaudit/migrations/0012_auto_20181018_0012.py
--rw-rw-r--   0 jason     (1000) jason     (1000)      700 2022-09-04 03:01:59.000000 django-easy-audit-1.3.4b2/easyaudit/migrations/0013_auto_20190723_0126.py
--rw-rw-r--   0 jason     (1000) jason     (1000)      395 2020-08-04 01:44:58.000000 django-easy-audit-1.3.4b2/easyaudit/migrations/0014_auto_20200513_0008.py
--rw-rw-r--   0 jason     (1000) jason     (1000)     5081 2020-11-07 19:27:56.000000 django-easy-audit-1.3.4b2/easyaudit/migrations/0015_auto_20201019_1217.py
--rw-rw-r--   0 jason     (1000) jason     (1000)      721 2022-02-12 03:50:51.000000 django-easy-audit-1.3.4b2/easyaudit/migrations/0016_alter_crudevent_event_type.py
--rw-rw-r--   0 jason     (1000) jason     (1000)      453 2023-01-26 14:03:29.000000 django-easy-audit-1.3.4b2/easyaudit/migrations/0017_alter_requestevent_datetime.py
--rw-r--r--   0 jason     (1000) jason     (1000)        0 2020-02-02 14:58:04.000000 django-easy-audit-1.3.4b2/easyaudit/migrations/__init__.py
--rw-rw-r--   0 jason     (1000) jason     (1000)     4221 2023-01-26 14:03:29.000000 django-easy-audit-1.3.4b2/easyaudit/models.py
--rw-rw-r--   0 jason     (1000) jason     (1000)     6277 2020-08-04 01:44:58.000000 django-easy-audit-1.3.4b2/easyaudit/settings.py
-drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2023-04-19 15:38:19.049323 django-easy-audit-1.3.4b2/easyaudit/signals/
--rw-r--r--   0 jason     (1000) jason     (1000)        0 2020-02-02 14:58:04.000000 django-easy-audit-1.3.4b2/easyaudit/signals/__init__.py
--rw-rw-r--   0 jason     (1000) jason     (1000)     2348 2023-04-19 15:36:04.000000 django-easy-audit-1.3.4b2/easyaudit/signals/auth_signals.py
--rw-rw-r--   0 jason     (1000) jason     (1000)    14865 2023-04-19 15:36:04.000000 django-easy-audit-1.3.4b2/easyaudit/signals/model_signals.py
--rw-rw-r--   0 jason     (1000) jason     (1000)     3267 2022-09-04 03:25:59.000000 django-easy-audit-1.3.4b2/easyaudit/signals/request_signals.py
-drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2023-04-19 15:38:19.045323 django-easy-audit-1.3.4b2/easyaudit/templates/
-drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2023-04-19 15:38:19.045323 django-easy-audit-1.3.4b2/easyaudit/templates/admin/
-drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2023-04-19 15:38:19.049323 django-easy-audit-1.3.4b2/easyaudit/templates/admin/easyaudit/
--rw-r--r--   0 jason     (1000) jason     (1000)      508 2020-02-02 14:58:04.000000 django-easy-audit-1.3.4b2/easyaudit/templates/admin/easyaudit/change_list.html
--rw-r--r--   0 jason     (1000) jason     (1000)     1215 2020-02-02 14:58:04.000000 django-easy-audit-1.3.4b2/easyaudit/templates/admin/easyaudit/purge_confirmation.html
--rw-rw-r--   0 jason     (1000) jason     (1000)     2893 2023-04-19 15:36:04.000000 django-easy-audit-1.3.4b2/easyaudit/utils.py
--rw-r--r--   0 jason     (1000) jason     (1000)       63 2020-02-02 14:58:04.000000 django-easy-audit-1.3.4b2/easyaudit/views.py
--rw-rw-r--   0 jason     (1000) jason     (1000)       38 2023-04-19 15:38:19.049323 django-easy-audit-1.3.4b2/setup.cfg
--rw-rw-r--   0 jason     (1000) jason     (1000)     1719 2023-04-19 15:37:59.000000 django-easy-audit-1.3.4b2/setup.py
+drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2023-06-13 14:39:01.913755 django-easy-audit-1.3.5/
+-rw-r--r--   0 jason     (1000) jason     (1000)    35141 2020-02-02 14:58:04.000000 django-easy-audit-1.3.5/LICENSE
+-rw-r--r--   0 jason     (1000) jason     (1000)      112 2020-02-02 14:58:04.000000 django-easy-audit-1.3.5/MANIFEST.in
+-rw-rw-r--   0 jason     (1000) jason     (1000)     2008 2023-06-13 14:39:01.909755 django-easy-audit-1.3.5/PKG-INFO
+-rw-r--r--   0 jason     (1000) jason     (1000)      787 2020-02-02 14:58:04.000000 django-easy-audit-1.3.5/README.rst
+drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2023-06-13 14:39:01.905755 django-easy-audit-1.3.5/django_easy_audit.egg-info/
+-rw-rw-r--   0 jason     (1000) jason     (1000)     2008 2023-06-13 14:39:01.000000 django-easy-audit-1.3.5/django_easy_audit.egg-info/PKG-INFO
+-rw-rw-r--   0 jason     (1000) jason     (1000)     1630 2023-06-13 14:39:01.000000 django-easy-audit-1.3.5/django_easy_audit.egg-info/SOURCES.txt
+-rw-rw-r--   0 jason     (1000) jason     (1000)        1 2023-06-13 14:39:01.000000 django-easy-audit-1.3.5/django_easy_audit.egg-info/dependency_links.txt
+-rw-rw-r--   0 jason     (1000) jason     (1000)       32 2023-06-13 14:39:01.000000 django-easy-audit-1.3.5/django_easy_audit.egg-info/requires.txt
+-rw-rw-r--   0 jason     (1000) jason     (1000)       10 2023-06-13 14:39:01.000000 django-easy-audit-1.3.5/django_easy_audit.egg-info/top_level.txt
+drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2023-06-13 14:39:01.909755 django-easy-audit-1.3.5/easyaudit/
+-rw-rw-r--   0 jason     (1000) jason     (1000)      101 2022-04-07 03:31:02.000000 django-easy-audit-1.3.5/easyaudit/__init__.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)     5532 2023-06-13 14:36:17.000000 django-easy-audit-1.3.5/easyaudit/admin.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)     5159 2022-05-24 18:10:15.000000 django-easy-audit-1.3.5/easyaudit/admin_helpers.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)      294 2022-02-25 18:56:54.000000 django-easy-audit-1.3.5/easyaudit/apps.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)      410 2020-08-04 01:44:58.000000 django-easy-audit-1.3.5/easyaudit/backends.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)     3693 2022-09-04 03:01:59.000000 django-easy-audit-1.3.5/easyaudit/crudhistory_admin_mixin.py
+drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2023-06-13 14:39:01.909755 django-easy-audit-1.3.5/easyaudit/middleware/
+-rw-r--r--   0 jason     (1000) jason     (1000)        0 2020-02-02 14:58:04.000000 django-easy-audit-1.3.5/easyaudit/middleware/__init__.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)     1912 2020-08-07 17:56:33.000000 django-easy-audit-1.3.5/easyaudit/middleware/easyaudit.py
+drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2023-06-13 14:39:01.909755 django-easy-audit-1.3.5/easyaudit/migrations/
+-rw-r--r--   0 jason     (1000) jason     (1000)     2290 2020-02-02 14:58:04.000000 django-easy-audit-1.3.5/easyaudit/migrations/0001_initial.py
+-rw-r--r--   0 jason     (1000) jason     (1000)      812 2020-02-02 14:58:04.000000 django-easy-audit-1.3.5/easyaudit/migrations/0002_auto_20170125_0759.py
+-rw-r--r--   0 jason     (1000) jason     (1000)      837 2020-02-02 14:58:04.000000 django-easy-audit-1.3.5/easyaudit/migrations/0003_auto_20170228_1505.py
+-rw-r--r--   0 jason     (1000) jason     (1000)      496 2020-02-02 14:58:04.000000 django-easy-audit-1.3.5/easyaudit/migrations/0004_auto_20170620_1354.py
+-rw-r--r--   0 jason     (1000) jason     (1000)      577 2020-02-02 14:58:04.000000 django-easy-audit-1.3.5/easyaudit/migrations/0005_auto_20170713_1155.py
+-rw-r--r--   0 jason     (1000) jason     (1000)     1563 2020-02-02 14:58:04.000000 django-easy-audit-1.3.5/easyaudit/migrations/0006_auto_20171018_1242.py
+-rw-r--r--   0 jason     (1000) jason     (1000)     1020 2020-02-02 14:58:04.000000 django-easy-audit-1.3.5/easyaudit/migrations/0007_auto_20180105_0838.py
+-rw-r--r--   0 jason     (1000) jason     (1000)      704 2020-02-02 14:58:04.000000 django-easy-audit-1.3.5/easyaudit/migrations/0008_auto_20180220_1908.py
+-rw-r--r--   0 jason     (1000) jason     (1000)      634 2020-02-02 14:58:04.000000 django-easy-audit-1.3.5/easyaudit/migrations/0009_auto_20180314_2225.py
+-rw-r--r--   0 jason     (1000) jason     (1000)      404 2020-02-02 14:58:04.000000 django-easy-audit-1.3.5/easyaudit/migrations/0010_repr_text.py
+-rw-r--r--   0 jason     (1000) jason     (1000)      432 2020-02-02 14:58:04.000000 django-easy-audit-1.3.5/easyaudit/migrations/0011_auto_20181101_1339.py
+-rw-r--r--   0 jason     (1000) jason     (1000)     1519 2020-02-02 14:58:04.000000 django-easy-audit-1.3.5/easyaudit/migrations/0012_auto_20181018_0012.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)      700 2022-09-04 03:01:59.000000 django-easy-audit-1.3.5/easyaudit/migrations/0013_auto_20190723_0126.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)      395 2020-08-04 01:44:58.000000 django-easy-audit-1.3.5/easyaudit/migrations/0014_auto_20200513_0008.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)     5081 2020-11-07 19:27:56.000000 django-easy-audit-1.3.5/easyaudit/migrations/0015_auto_20201019_1217.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)      721 2022-02-12 03:50:51.000000 django-easy-audit-1.3.5/easyaudit/migrations/0016_alter_crudevent_event_type.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)      453 2023-01-26 14:03:29.000000 django-easy-audit-1.3.5/easyaudit/migrations/0017_alter_requestevent_datetime.py
+-rw-r--r--   0 jason     (1000) jason     (1000)        0 2020-02-02 14:58:04.000000 django-easy-audit-1.3.5/easyaudit/migrations/__init__.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)     4221 2023-01-26 14:03:29.000000 django-easy-audit-1.3.5/easyaudit/models.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)     6277 2020-08-04 01:44:58.000000 django-easy-audit-1.3.5/easyaudit/settings.py
+drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2023-06-13 14:39:01.909755 django-easy-audit-1.3.5/easyaudit/signals/
+-rw-r--r--   0 jason     (1000) jason     (1000)        0 2020-02-02 14:58:04.000000 django-easy-audit-1.3.5/easyaudit/signals/__init__.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)     2348 2023-04-19 15:36:04.000000 django-easy-audit-1.3.5/easyaudit/signals/auth_signals.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)    14865 2023-04-19 15:36:04.000000 django-easy-audit-1.3.5/easyaudit/signals/model_signals.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)     3267 2022-09-04 03:25:59.000000 django-easy-audit-1.3.5/easyaudit/signals/request_signals.py
+drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2023-06-13 14:39:01.905755 django-easy-audit-1.3.5/easyaudit/templates/
+drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2023-06-13 14:39:01.905755 django-easy-audit-1.3.5/easyaudit/templates/admin/
+drwxrwxr-x   0 jason     (1000) jason     (1000)        0 2023-06-13 14:39:01.909755 django-easy-audit-1.3.5/easyaudit/templates/admin/easyaudit/
+-rw-r--r--   0 jason     (1000) jason     (1000)      508 2020-02-02 14:58:04.000000 django-easy-audit-1.3.5/easyaudit/templates/admin/easyaudit/change_list.html
+-rw-r--r--   0 jason     (1000) jason     (1000)     1215 2020-02-02 14:58:04.000000 django-easy-audit-1.3.5/easyaudit/templates/admin/easyaudit/purge_confirmation.html
+-rw-rw-r--   0 jason     (1000) jason     (1000)     2893 2023-04-19 15:36:04.000000 django-easy-audit-1.3.5/easyaudit/utils.py
+-rw-r--r--   0 jason     (1000) jason     (1000)       63 2020-02-02 14:58:04.000000 django-easy-audit-1.3.5/easyaudit/views.py
+-rw-rw-r--   0 jason     (1000) jason     (1000)       38 2023-06-13 14:39:01.913755 django-easy-audit-1.3.5/setup.cfg
+-rw-rw-r--   0 jason     (1000) jason     (1000)     1716 2023-06-13 14:37:11.000000 django-easy-audit-1.3.5/setup.py
```

### Comparing `django-easy-audit-1.3.4b2/LICENSE` & `django-easy-audit-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `django-easy-audit-1.3.4b2/PKG-INFO` & `django-easy-audit-1.3.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: django-easy-audit
-Version: 1.3.4b2
+Version: 1.3.5
 Summary: Yet another Django audit log app, hopefully the simplest one.
 Home-page: https://github.com/soynatan/django-easy-audit
 Author: Natán Calzolari
 Author-email: natancalzolari@gmail.com
 License: GPL3
-Platform: UNKNOWN
 Classifier: Environment :: Plugins
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
@@ -51,9 +50,7 @@
         ...
         'easyaudit.middleware.easyaudit.EasyAuditMiddleware',
     )
 
 3. Run 'python manage.py migrate easyaudit' to create the audit models.
 
 4. That's it! Now every CRUD event on your whole project will be registered in the audit models, which you will be able to query from the Django admin app. Additionally, this app will also log all authentication events and all URLs requested.
-
-
```

### Comparing `django-easy-audit-1.3.4b2/README.rst` & `django-easy-audit-1.3.5/README.rst`

 * *Files identical despite different names*

### Comparing `django-easy-audit-1.3.4b2/django_easy_audit.egg-info/PKG-INFO` & `django-easy-audit-1.3.5/django_easy_audit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: django-easy-audit
-Version: 1.3.4b2
+Version: 1.3.5
 Summary: Yet another Django audit log app, hopefully the simplest one.
 Home-page: https://github.com/soynatan/django-easy-audit
 Author: Natán Calzolari
 Author-email: natancalzolari@gmail.com
 License: GPL3
-Platform: UNKNOWN
 Classifier: Environment :: Plugins
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
@@ -51,9 +50,7 @@
         ...
         'easyaudit.middleware.easyaudit.EasyAuditMiddleware',
     )
 
 3. Run 'python manage.py migrate easyaudit' to create the audit models.
 
 4. That's it! Now every CRUD event on your whole project will be registered in the audit models, which you will be able to query from the Django admin app. Additionally, this app will also log all authentication events and all URLs requested.
-
-
```

### Comparing `django-easy-audit-1.3.4b2/django_easy_audit.egg-info/SOURCES.txt` & `django-easy-audit-1.3.5/django_easy_audit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-easy-audit-1.3.4b2/easyaudit/admin.py` & `django-easy-audit-1.3.5/easyaudit/admin.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from django.contrib import admin
 from django.contrib.auth import get_user_model
 from django.contrib.contenttypes.models import ContentType
+from django.http import HttpResponse
+import csv, datetime
 
 try: # Django 2.0
     from django.urls import reverse
 except: # Django < 2.0
     from django.core.urlresolvers import reverse
 
 from django.utils.safestring import mark_safe
@@ -12,14 +14,38 @@
 from . import settings
 from .models import CRUDEvent, LoginEvent, RequestEvent
 from .admin_helpers import prettify_json, EasyAuditModelAdmin
 from .settings import (CRUD_EVENT_LIST_FILTER, LOGIN_EVENT_LIST_FILTER, REQUEST_EVENT_LIST_FILTER,
                        CRUD_EVENT_SEARCH_FIELDS, LOGIN_EVENT_SEARCH_FIELDS, REQUEST_EVENT_SEARCH_FIELDS,
                        READONLY_EVENTS)
 
+# Export event audits to csv
+def export_to_csv(modeladmin, request, queryset):
+    opts = modeladmin.model._meta
+    response = HttpResponse(content_type='text/csv')
+    response['Content-Disposition'] = 'attachment;' 'filename={}.csv'.format(opts.verbose_name)
+    writer = csv.writer(response)
+    fields = [field for field in opts.get_fields() if not field.many_to_many and not field.one_to_many]
+    # Write a first row with header information
+    writer.writerow([field.verbose_name for field in fields])
+    # Write data rows
+    for obj in queryset:
+        data_row = []
+        for field in fields:
+            value = getattr(obj, field.name)
+            if isinstance(value, datetime.datetime):
+                value = value.strftime('%d/%m/%Y')
+            data_row.append(value)
+        writer.writerow(data_row)
+
+    return response
+
+export_to_csv.short_description = 'Export to CSV'  #short description
+
+
 # CRUD events
 class CRUDEventAdmin(EasyAuditModelAdmin):
     list_display = ['get_event_type_display', 'get_content_type', 'object_id', 'object_repr_link', 'user_link', 'datetime']
     date_hierarchy = 'datetime'
     list_filter = CRUD_EVENT_LIST_FILTER
     search_fields = CRUD_EVENT_SEARCH_FIELDS
     readonly_fields = ['event_type', 'object_id', 'get_content_type',
@@ -67,14 +93,15 @@
     object_json_repr_prettified.short_description = 'object json repr'
 
     def changed_fields_prettified(self, obj):
         return prettify_json(obj.changed_fields)
 
     changed_fields_prettified.short_description = 'changed fields'
 
+    actions = [export_to_csv] 
 
 if settings.ADMIN_SHOW_MODEL_EVENTS:
     admin.site.register(CRUDEvent, CRUDEventAdmin)
 
 
 # Login events
 class LoginEventAdmin(EasyAuditModelAdmin):
@@ -92,14 +119,15 @@
     def get_username(self, obj):
         user = self.get_user(obj)
         username = user.get_username() if user else None
         return username
 
     get_username.short_description = "User name"
 
+    actions = [export_to_csv] 
 
 if settings.ADMIN_SHOW_AUTH_EVENTS:
     admin.site.register(LoginEvent, LoginEventAdmin)
 
 
 # Request events
 class RequestEventAdmin(EasyAuditModelAdmin):
@@ -110,10 +138,11 @@
     readonly_fields = ['url', 'method', 'query_string', 'get_user', 'remote_ip', 'datetime', ]
 
     def get_user(self, obj):
         return self.users_by_id.get(obj.user_id)
 
     get_user.short_description = "User"
 
+    actions = [export_to_csv] 
 
 if settings.ADMIN_SHOW_REQUEST_EVENTS:
     admin.site.register(RequestEvent, RequestEventAdmin)
```

### Comparing `django-easy-audit-1.3.4b2/easyaudit/admin_helpers.py` & `django-easy-audit-1.3.5/easyaudit/admin_helpers.py`

 * *Files identical despite different names*

### Comparing `django-easy-audit-1.3.4b2/easyaudit/crudhistory_admin_mixin.py` & `django-easy-audit-1.3.5/easyaudit/crudhistory_admin_mixin.py`

 * *Files identical despite different names*

### Comparing `django-easy-audit-1.3.4b2/easyaudit/middleware/easyaudit.py` & `django-easy-audit-1.3.5/easyaudit/middleware/easyaudit.py`

 * *Files identical despite different names*

### Comparing `django-easy-audit-1.3.4b2/easyaudit/migrations/0001_initial.py` & `django-easy-audit-1.3.5/easyaudit/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-easy-audit-1.3.4b2/easyaudit/migrations/0002_auto_20170125_0759.py` & `django-easy-audit-1.3.5/easyaudit/migrations/0002_auto_20170125_0759.py`

 * *Files identical despite different names*

### Comparing `django-easy-audit-1.3.4b2/easyaudit/migrations/0003_auto_20170228_1505.py` & `django-easy-audit-1.3.5/easyaudit/migrations/0003_auto_20170228_1505.py`

 * *Files identical despite different names*

### Comparing `django-easy-audit-1.3.4b2/easyaudit/migrations/0005_auto_20170713_1155.py` & `django-easy-audit-1.3.5/easyaudit/migrations/0005_auto_20170713_1155.py`

 * *Files identical despite different names*

### Comparing `django-easy-audit-1.3.4b2/easyaudit/migrations/0006_auto_20171018_1242.py` & `django-easy-audit-1.3.5/easyaudit/migrations/0006_auto_20171018_1242.py`

 * *Files identical despite different names*

### Comparing `django-easy-audit-1.3.4b2/easyaudit/migrations/0007_auto_20180105_0838.py` & `django-easy-audit-1.3.5/easyaudit/migrations/0007_auto_20180105_0838.py`

 * *Files identical despite different names*

### Comparing `django-easy-audit-1.3.4b2/easyaudit/migrations/0008_auto_20180220_1908.py` & `django-easy-audit-1.3.5/easyaudit/migrations/0008_auto_20180220_1908.py`

 * *Files identical despite different names*

### Comparing `django-easy-audit-1.3.4b2/easyaudit/migrations/0009_auto_20180314_2225.py` & `django-easy-audit-1.3.5/easyaudit/migrations/0009_auto_20180314_2225.py`

 * *Files identical despite different names*

### Comparing `django-easy-audit-1.3.4b2/easyaudit/migrations/0012_auto_20181018_0012.py` & `django-easy-audit-1.3.5/easyaudit/migrations/0012_auto_20181018_0012.py`

 * *Files identical despite different names*

### Comparing `django-easy-audit-1.3.4b2/easyaudit/migrations/0013_auto_20190723_0126.py` & `django-easy-audit-1.3.5/easyaudit/migrations/0013_auto_20190723_0126.py`

 * *Files identical despite different names*

### Comparing `django-easy-audit-1.3.4b2/easyaudit/migrations/0015_auto_20201019_1217.py` & `django-easy-audit-1.3.5/easyaudit/migrations/0015_auto_20201019_1217.py`

 * *Files identical despite different names*

### Comparing `django-easy-audit-1.3.4b2/easyaudit/migrations/0016_alter_crudevent_event_type.py` & `django-easy-audit-1.3.5/easyaudit/migrations/0016_alter_crudevent_event_type.py`

 * *Files identical despite different names*

### Comparing `django-easy-audit-1.3.4b2/easyaudit/models.py` & `django-easy-audit-1.3.5/easyaudit/models.py`

 * *Files identical despite different names*

### Comparing `django-easy-audit-1.3.4b2/easyaudit/settings.py` & `django-easy-audit-1.3.5/easyaudit/settings.py`

 * *Files identical despite different names*

### Comparing `django-easy-audit-1.3.4b2/easyaudit/signals/auth_signals.py` & `django-easy-audit-1.3.5/easyaudit/signals/auth_signals.py`

 * *Files identical despite different names*

### Comparing `django-easy-audit-1.3.4b2/easyaudit/signals/model_signals.py` & `django-easy-audit-1.3.5/easyaudit/signals/model_signals.py`

 * *Files identical despite different names*

### Comparing `django-easy-audit-1.3.4b2/easyaudit/signals/request_signals.py` & `django-easy-audit-1.3.5/easyaudit/signals/request_signals.py`

 * *Files identical despite different names*

### Comparing `django-easy-audit-1.3.4b2/easyaudit/templates/admin/easyaudit/purge_confirmation.html` & `django-easy-audit-1.3.5/easyaudit/templates/admin/easyaudit/purge_confirmation.html`

 * *Files identical despite different names*

### Comparing `django-easy-audit-1.3.4b2/easyaudit/utils.py` & `django-easy-audit-1.3.5/easyaudit/utils.py`

 * *Files identical despite different names*

### Comparing `django-easy-audit-1.3.4b2/setup.py` & `django-easy-audit-1.3.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='django-easy-audit',
-    version='1.3.4.b2',
+    version='1.3.5',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         "beautifulsoup4",
         "django>=2.2,<5.0"
     ],
     python_requires=">=3.5",
```

