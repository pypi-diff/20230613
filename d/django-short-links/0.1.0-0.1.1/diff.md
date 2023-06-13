# Comparing `tmp/django_short_links-0.1.0.tar.gz` & `tmp/django_short_links-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_short_links-0.1.0.tar", max compression
+gzip compressed data, was "django_short_links-0.1.1.tar", max compression
```

## Comparing `django_short_links-0.1.0.tar` & `django_short_links-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1095 2022-08-21 12:14:58.898018 django_short_links-0.1.0/LICENSE
--rw-r--r--   0        0        0        0 2022-08-21 12:10:59.901587 django_short_links-0.1.0/links/__init__.py
--rw-r--r--   0        0        0      167 2023-06-12 11:03:25.902464 django_short_links-0.1.0/links/admin.py
--rw-r--r--   0        0        0      218 2023-06-12 13:20:44.527009 django_short_links-0.1.0/links/apps.py
--rw-r--r--   0        0        0      228 2023-06-12 11:03:47.298696 django_short_links-0.1.0/links/forms.py
--rw-r--r--   0        0        0      849 2023-06-13 10:30:17.657675 django_short_links-0.1.0/links/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-06-12 10:57:28.904816 django_short_links-0.1.0/links/migrations/__init__.py
--rw-r--r--   0        0        0      654 2023-06-13 10:25:49.830518 django_short_links-0.1.0/links/models.py
--rw-r--r--   0        0        0      982 2023-06-12 12:33:21.684915 django_short_links-0.1.0/links/templates/links/base.html
--rw-r--r--   0        0        0     1719 2023-06-13 10:46:10.589864 django_short_links-0.1.0/links/templates/links/detail.html
--rw-r--r--   0        0        0     1860 2023-06-13 10:27:05.850608 django_short_links-0.1.0/links/templates/links/index.html
--rw-r--r--   0        0        0     1498 2023-06-12 13:21:10.628098 django_short_links-0.1.0/links/templates/registration/login.html
--rw-r--r--   0        0        0       84 2023-02-06 09:50:24.122941 django_short_links-0.1.0/links/tests.py
--rw-r--r--   0        0        0      416 2023-06-12 13:18:46.120022 django_short_links-0.1.0/links/urls.py
--rw-r--r--   0        0        0     1974 2023-06-13 10:44:53.464487 django_short_links-0.1.0/links/views.py
--rw-r--r--   0        0        0      512 2023-06-13 11:21:05.610449 django_short_links-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      796 2023-06-13 11:21:26.193848 django_short_links-0.1.0/README.md
--rw-r--r--   0        0        0     1403 1970-01-01 00:00:00.000000 django_short_links-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1095 2022-08-21 12:14:58.898018 django_short_links-0.1.1/LICENSE
+-rw-r--r--   0        0        0        0 2022-08-21 12:10:59.901587 django_short_links-0.1.1/links/__init__.py
+-rw-r--r--   0        0        0      167 2023-06-12 11:03:25.902464 django_short_links-0.1.1/links/admin.py
+-rw-r--r--   0        0        0      218 2023-06-12 13:20:44.527009 django_short_links-0.1.1/links/apps.py
+-rw-r--r--   0        0        0      228 2023-06-12 11:03:47.298696 django_short_links-0.1.1/links/forms.py
+-rw-r--r--   0        0        0      849 2023-06-13 10:30:17.657675 django_short_links-0.1.1/links/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-06-12 10:57:28.904816 django_short_links-0.1.1/links/migrations/__init__.py
+-rw-r--r--   0        0        0      654 2023-06-13 10:25:49.830518 django_short_links-0.1.1/links/models.py
+-rw-r--r--   0        0        0      982 2023-06-12 12:33:21.684915 django_short_links-0.1.1/links/templates/links/base.html
+-rw-r--r--   0        0        0     1719 2023-06-13 10:46:10.589864 django_short_links-0.1.1/links/templates/links/detail.html
+-rw-r--r--   0        0        0     1860 2023-06-13 10:27:05.850608 django_short_links-0.1.1/links/templates/links/index.html
+-rw-r--r--   0        0        0     1498 2023-06-12 13:21:10.628098 django_short_links-0.1.1/links/templates/registration/login.html
+-rw-r--r--   0        0        0       84 2023-02-06 09:50:24.122941 django_short_links-0.1.1/links/tests.py
+-rw-r--r--   0        0        0      416 2023-06-12 13:18:46.120022 django_short_links-0.1.1/links/urls.py
+-rw-r--r--   0        0        0     1974 2023-06-13 10:44:53.464487 django_short_links-0.1.1/links/views.py
+-rw-r--r--   0        0        0      512 2023-06-13 11:23:30.375363 django_short_links-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      802 2023-06-13 11:22:22.510332 django_short_links-0.1.1/README.md
+-rw-r--r--   0        0        0     1409 1970-01-01 00:00:00.000000 django_short_links-0.1.1/PKG-INFO
```

### Comparing `django_short_links-0.1.0/LICENSE` & `django_short_links-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_short_links-0.1.0/links/migrations/0001_initial.py` & `django_short_links-0.1.1/links/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_short_links-0.1.0/links/models.py` & `django_short_links-0.1.1/links/models.py`

 * *Files identical despite different names*

### Comparing `django_short_links-0.1.0/links/templates/links/base.html` & `django_short_links-0.1.1/links/templates/links/base.html`

 * *Files identical despite different names*

### Comparing `django_short_links-0.1.0/links/templates/links/detail.html` & `django_short_links-0.1.1/links/templates/links/detail.html`

 * *Files identical despite different names*

### Comparing `django_short_links-0.1.0/links/templates/links/index.html` & `django_short_links-0.1.1/links/templates/links/index.html`

 * *Files identical despite different names*

### Comparing `django_short_links-0.1.0/links/templates/registration/login.html` & `django_short_links-0.1.1/links/templates/registration/login.html`

 * *Files identical despite different names*

### Comparing `django_short_links-0.1.0/links/views.py` & `django_short_links-0.1.1/links/views.py`

 * *Files identical despite different names*

### Comparing `django_short_links-0.1.0/pyproject.toml` & `django_short_links-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-short-links"
-version = "0.1.0"
+version = "0.1.1"
 description = "URL shortener Django app"
 authors = ["Yousef Abu Shanab <josephyousef249@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "links" }]
 homepage = "https://github.com/youzarsiph/django-links/"
 repository = "https://github.com/youzarsiph/django-links/"
```

### Comparing `django_short_links-0.1.0/README.md` & `django_short_links-0.1.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 URL / Link shortener web app.
 
 ## Getting Started
 
 Install `links`:
 
 ```shell
-pip install django-links
+pip install django-short-links
 ```
 
 Add `links` to `INSTALLED_APPS` and add a new setting `LINKS_SITE_NAME`, in `settings.py`:
 
 ```python
 # settings.py
```

### Comparing `django_short_links-0.1.0/PKG-INFO` & `django_short_links-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-short-links
-Version: 0.1.0
+Version: 0.1.1
 Summary: URL shortener Django app
 Home-page: https://github.com/youzarsiph/django-links/
 License: MIT
 Author: Yousef Abu Shanab
 Author-email: josephyousef249@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -21,15 +21,15 @@
 URL / Link shortener web app.
 
 ## Getting Started
 
 Install `links`:
 
 ```shell
-pip install django-links
+pip install django-short-links
 ```
 
 Add `links` to `INSTALLED_APPS` and add a new setting `LINKS_SITE_NAME`, in `settings.py`:
 
 ```python
 # settings.py
```

