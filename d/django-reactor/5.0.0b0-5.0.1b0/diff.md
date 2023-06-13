# Comparing `tmp/django-reactor-5.0.0b0.tar.gz` & `tmp/django-reactor-5.0.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-reactor-5.0.0b0.tar", last modified: Mon Jun 12 07:51:20 2023, max compression
+gzip compressed data, was "django-reactor-5.0.1b0.tar", last modified: Tue Jun 13 10:49:38 2023, max compression
```

## Comparing `django-reactor-5.0.0b0.tar` & `django-reactor-5.0.1b0.tar`

### file list

```diff
@@ -1,36 +1,39 @@
-drwxr-xr-x   0 xigurat   (1000) xigurat   (1001)        0 2023-06-12 07:51:20.094159 django-reactor-5.0.0b0/
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)       72 2023-06-01 12:00:36.000000 django-reactor-5.0.0b0/MANIFEST.in
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)    16764 2023-06-12 07:51:20.094159 django-reactor-5.0.0b0/PKG-INFO
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)    15905 2023-06-10 22:13:11.000000 django-reactor-5.0.0b0/README.md
-drwxr-xr-x   0 xigurat   (1000) xigurat   (1001)        0 2023-06-12 07:51:20.094159 django-reactor-5.0.0b0/django_reactor.egg-info/
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)    16764 2023-06-12 07:51:20.000000 django-reactor-5.0.0b0/django_reactor.egg-info/PKG-INFO
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)      684 2023-06-12 07:51:20.000000 django-reactor-5.0.0b0/django_reactor.egg-info/SOURCES.txt
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)        1 2023-06-12 07:51:20.000000 django-reactor-5.0.0b0/django_reactor.egg-info/dependency_links.txt
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)        1 2023-06-01 11:50:12.000000 django-reactor-5.0.0b0/django_reactor.egg-info/not-zip-safe
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)      180 2023-06-12 07:51:20.000000 django-reactor-5.0.0b0/django_reactor.egg-info/requires.txt
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)        8 2023-06-12 07:51:20.000000 django-reactor-5.0.0b0/django_reactor.egg-info/top_level.txt
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)      451 2023-06-10 22:13:11.000000 django-reactor-5.0.0b0/pyproject.toml
-drwxr-xr-x   0 xigurat   (1000) xigurat   (1001)        0 2023-06-12 07:51:20.094159 django-reactor-5.0.0b0/reactor/
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)        0 2023-05-31 13:32:27.000000 django-reactor-5.0.0b0/reactor/__init__.py
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)      291 2023-06-06 12:12:16.000000 django-reactor-5.0.0b0/reactor/apps.py
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)     5661 2023-06-10 22:13:11.000000 django-reactor-5.0.0b0/reactor/auto_broadcast.py
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)    13782 2023-06-10 22:13:11.000000 django-reactor-5.0.0b0/reactor/component.py
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)     6125 2023-06-10 22:13:11.000000 django-reactor-5.0.0b0/reactor/consumer.py
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)     3990 2023-06-12 07:48:44.000000 django-reactor-5.0.0b0/reactor/event_transpiler.py
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)      411 2023-05-31 13:32:27.000000 django-reactor-5.0.0b0/reactor/log.py
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)     3045 2023-06-10 22:13:11.000000 django-reactor-5.0.0b0/reactor/repository.py
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)      874 2023-06-10 22:13:11.000000 django-reactor-5.0.0b0/reactor/schemas.py
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)      765 2023-06-10 22:13:11.000000 django-reactor-5.0.0b0/reactor/serializer.py
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)      590 2023-06-12 07:48:55.000000 django-reactor-5.0.0b0/reactor/settings.py
-drwxr-xr-x   0 xigurat   (1000) xigurat   (1001)        0 2023-06-12 07:51:20.094159 django-reactor-5.0.0b0/reactor/static/
-drwxr-xr-x   0 xigurat   (1000) xigurat   (1001)        0 2023-06-12 07:51:20.094159 django-reactor-5.0.0b0/reactor/static/reactor/
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)    22594 2023-06-12 07:51:19.000000 django-reactor-5.0.0b0/reactor/static/reactor/reactor.min.js
-drwxr-xr-x   0 xigurat   (1000) xigurat   (1001)        0 2023-06-12 07:51:20.094159 django-reactor-5.0.0b0/reactor/templates/
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)      444 2022-07-30 12:06:00.000000 django-reactor-5.0.0b0/reactor/templates/reactor_header.html
-drwxr-xr-x   0 xigurat   (1000) xigurat   (1001)        0 2023-06-12 07:51:20.094159 django-reactor-5.0.0b0/reactor/templatetags/
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)        0 2022-07-30 12:06:00.000000 django-reactor-5.0.0b0/reactor/templatetags/__init__.py
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)     3524 2023-06-10 22:13:11.000000 django-reactor-5.0.0b0/reactor/templatetags/reactor.py
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)      165 2022-07-30 12:06:00.000000 django-reactor-5.0.0b0/reactor/urls.py
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)     2733 2023-06-10 22:13:11.000000 django-reactor-5.0.0b0/reactor/utils.py
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)     1336 2023-06-12 07:51:20.097492 django-reactor-5.0.0b0/setup.cfg
--rw-r--r--   0 xigurat   (1000) xigurat   (1001)       39 2023-06-01 09:29:36.000000 django-reactor-5.0.0b0/setup.py
+drwxr-xr-x   0 xigurat   (1000) xigurat   (1001)        0 2023-06-13 10:49:38.695759 django-reactor-5.0.1b0/
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)       65 2023-06-13 10:33:48.000000 django-reactor-5.0.1b0/MANIFEST.in
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)    16764 2023-06-13 10:49:38.695759 django-reactor-5.0.1b0/PKG-INFO
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)    15905 2023-06-10 22:13:11.000000 django-reactor-5.0.1b0/README.md
+drwxr-xr-x   0 xigurat   (1000) xigurat   (1001)        0 2023-06-13 10:49:38.692425 django-reactor-5.0.1b0/django_reactor.egg-info/
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)    16764 2023-06-13 10:49:38.000000 django-reactor-5.0.1b0/django_reactor.egg-info/PKG-INFO
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)      800 2023-06-13 10:49:38.000000 django-reactor-5.0.1b0/django_reactor.egg-info/SOURCES.txt
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)        1 2023-06-13 10:49:38.000000 django-reactor-5.0.1b0/django_reactor.egg-info/dependency_links.txt
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)        1 2023-06-01 11:50:12.000000 django-reactor-5.0.1b0/django_reactor.egg-info/not-zip-safe
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)      180 2023-06-13 10:49:38.000000 django-reactor-5.0.1b0/django_reactor.egg-info/requires.txt
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)        8 2023-06-13 10:49:38.000000 django-reactor-5.0.1b0/django_reactor.egg-info/top_level.txt
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)      451 2023-06-10 22:13:11.000000 django-reactor-5.0.1b0/pyproject.toml
+drwxr-xr-x   0 xigurat   (1000) xigurat   (1001)        0 2023-06-13 10:49:38.692425 django-reactor-5.0.1b0/reactor/
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)        0 2023-05-31 13:32:27.000000 django-reactor-5.0.1b0/reactor/__init__.py
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)      291 2023-06-06 12:12:16.000000 django-reactor-5.0.1b0/reactor/apps.py
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)     5661 2023-06-10 22:13:11.000000 django-reactor-5.0.1b0/reactor/auto_broadcast.py
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)    13782 2023-06-10 22:13:11.000000 django-reactor-5.0.1b0/reactor/component.py
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)     6125 2023-06-10 22:13:11.000000 django-reactor-5.0.1b0/reactor/consumer.py
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)     3990 2023-06-12 07:48:44.000000 django-reactor-5.0.1b0/reactor/event_transpiler.py
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)      411 2023-05-31 13:32:27.000000 django-reactor-5.0.1b0/reactor/log.py
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)     3045 2023-06-10 22:13:11.000000 django-reactor-5.0.1b0/reactor/repository.py
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)      874 2023-06-10 22:13:11.000000 django-reactor-5.0.1b0/reactor/schemas.py
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)      765 2023-06-10 22:13:11.000000 django-reactor-5.0.1b0/reactor/serializer.py
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)      590 2023-06-12 07:48:55.000000 django-reactor-5.0.1b0/reactor/settings.py
+drwxr-xr-x   0 xigurat   (1000) xigurat   (1001)        0 2023-06-13 10:49:38.692425 django-reactor-5.0.1b0/reactor/static/
+drwxr-xr-x   0 xigurat   (1000) xigurat   (1001)        0 2023-06-13 10:49:38.692425 django-reactor-5.0.1b0/reactor/static/reactor/
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)     4596 2023-06-10 22:13:11.000000 django-reactor-5.0.1b0/reactor/static/reactor/reactor-boost.js
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)     9536 2023-06-10 22:13:11.000000 django-reactor-5.0.1b0/reactor/static/reactor/reactor.js
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)    22594 2023-06-13 10:49:38.000000 django-reactor-5.0.1b0/reactor/static/reactor/reactor.min.js
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)    87150 2023-06-13 10:49:38.000000 django-reactor-5.0.1b0/reactor/static/reactor/reactor.min.js.map
+drwxr-xr-x   0 xigurat   (1000) xigurat   (1001)        0 2023-06-13 10:49:38.695759 django-reactor-5.0.1b0/reactor/templates/
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)      444 2022-07-30 12:06:00.000000 django-reactor-5.0.1b0/reactor/templates/reactor_header.html
+drwxr-xr-x   0 xigurat   (1000) xigurat   (1001)        0 2023-06-13 10:49:38.695759 django-reactor-5.0.1b0/reactor/templatetags/
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)        0 2022-07-30 12:06:00.000000 django-reactor-5.0.1b0/reactor/templatetags/__init__.py
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)     3524 2023-06-10 22:13:11.000000 django-reactor-5.0.1b0/reactor/templatetags/reactor.py
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)      165 2022-07-30 12:06:00.000000 django-reactor-5.0.1b0/reactor/urls.py
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)     2733 2023-06-10 22:13:11.000000 django-reactor-5.0.1b0/reactor/utils.py
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)     1336 2023-06-13 10:49:38.695759 django-reactor-5.0.1b0/setup.cfg
+-rw-r--r--   0 xigurat   (1000) xigurat   (1001)       39 2023-06-01 09:29:36.000000 django-reactor-5.0.1b0/setup.py
```

### Comparing `django-reactor-5.0.0b0/PKG-INFO` & `django-reactor-5.0.1b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-reactor
-Version: 5.0.0b0
+Version: 5.0.1b0
 Summary: Brings LiveView from Phoenix framework into Django
 Home-page: https://github.com/edelvalle/reactor
 Author: Eddy Ernesto del Valle Pino
 Author-email: eddy@edelvalle.me
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `django-reactor-5.0.0b0/README.md` & `django-reactor-5.0.1b0/README.md`

 * *Files identical despite different names*

### Comparing `django-reactor-5.0.0b0/django_reactor.egg-info/PKG-INFO` & `django-reactor-5.0.1b0/django_reactor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-reactor
-Version: 5.0.0b0
+Version: 5.0.1b0
 Summary: Brings LiveView from Phoenix framework into Django
 Home-page: https://github.com/edelvalle/reactor
 Author: Eddy Ernesto del Valle Pino
 Author-email: eddy@edelvalle.me
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `django-reactor-5.0.0b0/reactor/auto_broadcast.py` & `django-reactor-5.0.1b0/reactor/auto_broadcast.py`

 * *Files identical despite different names*

### Comparing `django-reactor-5.0.0b0/reactor/component.py` & `django-reactor-5.0.1b0/reactor/component.py`

 * *Files identical despite different names*

### Comparing `django-reactor-5.0.0b0/reactor/consumer.py` & `django-reactor-5.0.1b0/reactor/consumer.py`

 * *Files identical despite different names*

### Comparing `django-reactor-5.0.0b0/reactor/event_transpiler.py` & `django-reactor-5.0.1b0/reactor/event_transpiler.py`

 * *Files identical despite different names*

### Comparing `django-reactor-5.0.0b0/reactor/repository.py` & `django-reactor-5.0.1b0/reactor/repository.py`

 * *Files identical despite different names*

### Comparing `django-reactor-5.0.0b0/reactor/schemas.py` & `django-reactor-5.0.1b0/reactor/schemas.py`

 * *Files identical despite different names*

### Comparing `django-reactor-5.0.0b0/reactor/serializer.py` & `django-reactor-5.0.1b0/reactor/serializer.py`

 * *Files identical despite different names*

### Comparing `django-reactor-5.0.0b0/reactor/settings.py` & `django-reactor-5.0.1b0/reactor/settings.py`

 * *Files identical despite different names*

### Comparing `django-reactor-5.0.0b0/reactor/static/reactor/reactor.min.js` & `django-reactor-5.0.1b0/reactor/static/reactor/reactor.min.js`

 * *Files identical despite different names*

### Comparing `django-reactor-5.0.0b0/reactor/templatetags/reactor.py` & `django-reactor-5.0.1b0/reactor/templatetags/reactor.py`

 * *Files identical despite different names*

### Comparing `django-reactor-5.0.0b0/reactor/utils.py` & `django-reactor-5.0.1b0/reactor/utils.py`

 * *Files identical despite different names*

### Comparing `django-reactor-5.0.0b0/setup.cfg` & `django-reactor-5.0.1b0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-reactor
-version = 5.0.0b0
+version = 5.0.1b0
 description = Brings LiveView from Phoenix framework into Django
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Development Status :: 4 - Beta
 	Environment :: Web Environment
 	Framework :: Django
```

