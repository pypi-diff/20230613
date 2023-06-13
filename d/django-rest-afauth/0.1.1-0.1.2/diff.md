# Comparing `tmp/django_rest_afauth-0.1.1.tar.gz` & `tmp/django_rest_afauth-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_rest_afauth-0.1.1.tar", max compression
+gzip compressed data, was "django_rest_afauth-0.1.2.tar", max compression
```

## Comparing `django_rest_afauth-0.1.1.tar` & `django_rest_afauth-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      289 2023-06-13 08:31:24.238614 django_rest_afauth-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-06-13 09:15:09.119768 django_rest_afauth-0.1.1/drf_afauth/__init__.py
--rw-r--r--   0        0        0       63 2023-06-13 09:15:09.119768 django_rest_afauth-0.1.1/drf_afauth/admin.py
--rw-r--r--   0        0        0      158 2023-06-13 12:30:00.793469 django_rest_afauth-0.1.1/drf_afauth/apps.py
--rw-r--r--   0        0        0        0 2023-06-13 09:15:09.119768 django_rest_afauth-0.1.1/drf_afauth/migrations/__init__.py
--rw-r--r--   0        0        0       57 2023-06-13 09:15:09.119768 django_rest_afauth-0.1.1/drf_afauth/models.py
--rw-r--r--   0        0        0        0 2023-06-13 11:13:25.337664 django_rest_afauth-0.1.1/drf_afauth/serializer.py
--rw-r--r--   0        0        0      607 2023-06-13 11:33:42.050907 django_rest_afauth-0.1.1/drf_afauth/settings.py
--rw-r--r--   0        0        0      908 2023-06-13 12:15:47.425026 django_rest_afauth-0.1.1/drf_afauth/settings_fields.py
--rw-r--r--   0        0        0       60 2023-06-13 09:15:09.119768 django_rest_afauth-0.1.1/drf_afauth/tests.py
--rw-r--r--   0        0        0        0 2023-06-13 11:32:04.338631 django_rest_afauth-0.1.1/drf_afauth/utils/__init__.py
--rw-r--r--   0        0        0     1996 2023-06-13 11:32:44.774744 django_rest_afauth-0.1.1/drf_afauth/utils/nested_settings.py
--rw-r--r--   0        0        0       63 2023-06-13 09:15:09.119768 django_rest_afauth-0.1.1/drf_afauth/views.py
--rw-r--r--   0        0        0      375 2023-06-13 12:30:39.701502 django_rest_afauth-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      687 1970-01-01 00:00:00.000000 django_rest_afauth-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      289 2023-06-13 08:31:24.238614 django_rest_afauth-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-06-13 09:15:09.119768 django_rest_afauth-0.1.2/drf_afauth/__init__.py
+-rw-r--r--   0        0        0       63 2023-06-13 09:15:09.119768 django_rest_afauth-0.1.2/drf_afauth/admin.py
+-rw-r--r--   0        0        0      158 2023-06-13 12:30:00.793469 django_rest_afauth-0.1.2/drf_afauth/apps.py
+-rw-r--r--   0        0        0        0 2023-06-13 09:15:09.119768 django_rest_afauth-0.1.2/drf_afauth/migrations/__init__.py
+-rw-r--r--   0        0        0       57 2023-06-13 09:15:09.119768 django_rest_afauth-0.1.2/drf_afauth/models.py
+-rw-r--r--   0        0        0        0 2023-06-13 11:13:25.337664 django_rest_afauth-0.1.2/drf_afauth/serializer.py
+-rw-r--r--   0        0        0      607 2023-06-13 11:33:42.050907 django_rest_afauth-0.1.2/drf_afauth/settings.py
+-rw-r--r--   0        0        0      989 2023-06-13 12:34:58.393915 django_rest_afauth-0.1.2/drf_afauth/settings_fields.py
+-rw-r--r--   0        0        0       60 2023-06-13 09:15:09.119768 django_rest_afauth-0.1.2/drf_afauth/tests.py
+-rw-r--r--   0        0        0        0 2023-06-13 11:32:04.338631 django_rest_afauth-0.1.2/drf_afauth/utils/__init__.py
+-rw-r--r--   0        0        0     1996 2023-06-13 11:32:44.774744 django_rest_afauth-0.1.2/drf_afauth/utils/nested_settings.py
+-rw-r--r--   0        0        0       63 2023-06-13 09:15:09.119768 django_rest_afauth-0.1.2/drf_afauth/views.py
+-rw-r--r--   0        0        0      375 2023-06-13 12:35:08.357936 django_rest_afauth-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      687 1970-01-01 00:00:00.000000 django_rest_afauth-0.1.2/PKG-INFO
```

### Comparing `django_rest_afauth-0.1.1/drf_afauth/settings.py` & `django_rest_afauth-0.1.2/drf_afauth/settings.py`

 * *Files identical despite different names*

### Comparing `django_rest_afauth-0.1.1/drf_afauth/settings_fields.py` & `django_rest_afauth-0.1.2/drf_afauth/settings_fields.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,15 +23,19 @@
         return super().__new__(
             cls, name=name, default=default,
             type_signature=type_signature,
             help=help, import_string=import_string)
 
 
 USER_SETTINGS_FIELDS = [
-    "example field"
+    Field(
+        "EXAMPLE_FIELD",
+        type_signature=str,
+        default="Lorem ipsum",
+    )
 ]
 
 SETTINGS_FIELDS_GROUPS_MAP = OrderedDict([
     ('user', USER_SETTINGS_FIELDS),
 ])
 
 SETTINGS_FIELDS_GROUPS = list(SETTINGS_FIELDS_GROUPS_MAP.values())
```

### Comparing `django_rest_afauth-0.1.1/drf_afauth/utils/nested_settings.py` & `django_rest_afauth-0.1.2/drf_afauth/utils/nested_settings.py`

 * *Files identical despite different names*

### Comparing `django_rest_afauth-0.1.1/PKG-INFO` & `django_rest_afauth-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-rest-afauth
-Version: 0.1.1
+Version: 0.1.2
 Summary: This is afauth app
 Author: Your Name
 Author-email: you@aflabs.si
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Django (>=4.2.2,<5.0.0)
```

