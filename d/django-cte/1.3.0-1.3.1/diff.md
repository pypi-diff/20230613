# Comparing `tmp/django-cte-1.3.0.tar.gz` & `tmp/django-cte-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-cte-1.3.0.tar", last modified: Wed May 24 15:12:20 2023, max compression
+gzip compressed data, was "django-cte-1.3.1.tar", last modified: Tue Jun 13 20:00:24 2023, max compression
```

## Comparing `django-cte-1.3.0.tar` & `django-cte-1.3.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 dimagi    (1001) dimagi    (1001)        0 2023-05-24 15:12:20.696809 django-cte-1.3.0/
--rw-r--r--   0 dimagi    (1001) dimagi    (1001)     1508 2018-02-21 14:28:44.000000 django-cte-1.3.0/LICENSE
--rw-r--r--   0 dimagi    (1001) dimagi    (1001)     2134 2023-05-24 15:12:20.696809 django-cte-1.3.0/PKG-INFO
--rw-r--r--   0 dimagi    (1001) dimagi    (1001)      850 2022-04-26 20:01:12.000000 django-cte-1.3.0/README.md
-drwxr-xr-x   0 dimagi    (1001) dimagi    (1001)        0 2023-05-24 15:12:20.696809 django-cte-1.3.0/django_cte/
--rw-r--r--   0 dimagi    (1001) dimagi    (1001)      158 2023-05-24 15:06:01.000000 django-cte-1.3.0/django_cte/__init__.py
--rw-r--r--   0 dimagi    (1001) dimagi    (1001)     6574 2023-05-24 15:06:01.000000 django-cte-1.3.0/django_cte/cte.py
--rw-r--r--   0 dimagi    (1001) dimagi    (1001)     1930 2022-07-07 11:23:10.000000 django-cte-1.3.0/django_cte/expressions.py
--rw-r--r--   0 dimagi    (1001) dimagi    (1001)     3243 2023-05-24 15:05:55.000000 django-cte-1.3.0/django_cte/join.py
--rw-r--r--   0 dimagi    (1001) dimagi    (1001)     3615 2023-05-24 15:05:55.000000 django-cte-1.3.0/django_cte/meta.py
--rw-r--r--   0 dimagi    (1001) dimagi    (1001)     5642 2023-05-24 15:06:01.000000 django-cte-1.3.0/django_cte/query.py
--rw-r--r--   0 dimagi    (1001) dimagi    (1001)     1137 2021-09-22 11:08:48.000000 django-cte-1.3.0/django_cte/raw.py
-drwxr-xr-x   0 dimagi    (1001) dimagi    (1001)        0 2023-05-24 15:12:20.696809 django-cte-1.3.0/django_cte.egg-info/
--rw-r--r--   0 dimagi    (1001) dimagi    (1001)     2134 2023-05-24 15:12:20.000000 django-cte-1.3.0/django_cte.egg-info/PKG-INFO
--rw-r--r--   0 dimagi    (1001) dimagi    (1001)      315 2023-05-24 15:12:20.000000 django-cte-1.3.0/django_cte.egg-info/SOURCES.txt
--rw-r--r--   0 dimagi    (1001) dimagi    (1001)        1 2023-05-24 15:12:20.000000 django-cte-1.3.0/django_cte.egg-info/dependency_links.txt
--rw-r--r--   0 dimagi    (1001) dimagi    (1001)       11 2023-05-24 15:12:20.000000 django-cte-1.3.0/django_cte.egg-info/top_level.txt
--rw-r--r--   0 dimagi    (1001) dimagi    (1001)      130 2023-05-24 15:12:20.696809 django-cte-1.3.0/setup.cfg
--rw-r--r--   0 dimagi    (1001) dimagi    (1001)     2002 2022-04-26 13:51:48.000000 django-cte-1.3.0/setup.py
+drwxr-xr-x   0 dimagi    (1001) dimagi    (1001)        0 2023-06-13 20:00:24.707505 django-cte-1.3.1/
+-rw-r--r--   0 dimagi    (1001) dimagi    (1001)     1508 2018-02-21 14:28:44.000000 django-cte-1.3.1/LICENSE
+-rw-r--r--   0 dimagi    (1001) dimagi    (1001)     2134 2023-06-13 20:00:24.707505 django-cte-1.3.1/PKG-INFO
+-rw-r--r--   0 dimagi    (1001) dimagi    (1001)      850 2022-04-26 20:01:12.000000 django-cte-1.3.1/README.md
+drwxr-xr-x   0 dimagi    (1001) dimagi    (1001)        0 2023-06-13 20:00:24.703505 django-cte-1.3.1/django_cte/
+-rw-r--r--   0 dimagi    (1001) dimagi    (1001)      158 2023-06-13 19:46:37.000000 django-cte-1.3.1/django_cte/__init__.py
+-rw-r--r--   0 dimagi    (1001) dimagi    (1001)     6574 2023-05-24 15:06:01.000000 django-cte-1.3.1/django_cte/cte.py
+-rw-r--r--   0 dimagi    (1001) dimagi    (1001)     1930 2022-07-07 11:23:10.000000 django-cte-1.3.1/django_cte/expressions.py
+-rw-r--r--   0 dimagi    (1001) dimagi    (1001)     3243 2023-05-24 15:05:55.000000 django-cte-1.3.1/django_cte/join.py
+-rw-r--r--   0 dimagi    (1001) dimagi    (1001)     3615 2023-05-24 15:05:55.000000 django-cte-1.3.1/django_cte/meta.py
+-rw-r--r--   0 dimagi    (1001) dimagi    (1001)     5663 2023-06-13 19:46:13.000000 django-cte-1.3.1/django_cte/query.py
+-rw-r--r--   0 dimagi    (1001) dimagi    (1001)     1137 2021-09-22 11:08:48.000000 django-cte-1.3.1/django_cte/raw.py
+drwxr-xr-x   0 dimagi    (1001) dimagi    (1001)        0 2023-06-13 20:00:24.707505 django-cte-1.3.1/django_cte.egg-info/
+-rw-r--r--   0 dimagi    (1001) dimagi    (1001)     2134 2023-06-13 20:00:24.000000 django-cte-1.3.1/django_cte.egg-info/PKG-INFO
+-rw-r--r--   0 dimagi    (1001) dimagi    (1001)      315 2023-06-13 20:00:24.000000 django-cte-1.3.1/django_cte.egg-info/SOURCES.txt
+-rw-r--r--   0 dimagi    (1001) dimagi    (1001)        1 2023-06-13 20:00:24.000000 django-cte-1.3.1/django_cte.egg-info/dependency_links.txt
+-rw-r--r--   0 dimagi    (1001) dimagi    (1001)       11 2023-06-13 20:00:24.000000 django-cte-1.3.1/django_cte.egg-info/top_level.txt
+-rw-r--r--   0 dimagi    (1001) dimagi    (1001)      130 2023-06-13 20:00:24.707505 django-cte-1.3.1/setup.cfg
+-rw-r--r--   0 dimagi    (1001) dimagi    (1001)     2002 2022-04-26 13:51:48.000000 django-cte-1.3.1/setup.py
```

### Comparing `django-cte-1.3.0/LICENSE` & `django-cte-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-cte-1.3.0/PKG-INFO` & `django-cte-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-cte
-Version: 1.3.0
+Version: 1.3.1
 Summary: Common Table Expressions (CTE) for Django
 Home-page: https://github.com/dimagi/django-cte
 Maintainer: Daniel Miller
 Maintainer-email: millerdev@gmail.com
 License: BSD License
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `django-cte-1.3.0/README.md` & `django-cte-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `django-cte-1.3.0/django_cte/cte.py` & `django-cte-1.3.1/django_cte/cte.py`

 * *Files identical despite different names*

### Comparing `django-cte-1.3.0/django_cte/expressions.py` & `django-cte-1.3.1/django_cte/expressions.py`

 * *Files identical despite different names*

### Comparing `django-cte-1.3.0/django_cte/join.py` & `django-cte-1.3.1/django_cte/join.py`

 * *Files identical despite different names*

### Comparing `django-cte-1.3.0/django_cte/meta.py` & `django-cte-1.3.1/django_cte/meta.py`

 * *Files identical despite different names*

### Comparing `django-cte-1.3.0/django_cte/query.py` & `django-cte-1.3.1/django_cte/query.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,14 +121,15 @@
 
 
 class CTEDeleteQuery(DeleteQuery, CTEQuery):
     pass
 
 
 QUERY_TYPES = {
+    Query: CTEQuery,
     UpdateQuery: CTEUpdateQuery,
     DeleteQuery: CTEDeleteQuery,
 }
 
 
 class CTEQueryCompiler(SQLCompiler):
```

### Comparing `django-cte-1.3.0/django_cte/raw.py` & `django-cte-1.3.1/django_cte/raw.py`

 * *Files identical despite different names*

### Comparing `django-cte-1.3.0/django_cte.egg-info/PKG-INFO` & `django-cte-1.3.1/django_cte.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-cte
-Version: 1.3.0
+Version: 1.3.1
 Summary: Common Table Expressions (CTE) for Django
 Home-page: https://github.com/dimagi/django-cte
 Maintainer: Daniel Miller
 Maintainer-email: millerdev@gmail.com
 License: BSD License
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `django-cte-1.3.0/setup.py` & `django-cte-1.3.1/setup.py`

 * *Files identical despite different names*

