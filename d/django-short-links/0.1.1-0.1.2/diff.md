# Comparing `tmp/django_short_links-0.1.1.tar.gz` & `tmp/django_short_links-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_short_links-0.1.1.tar", max compression
+gzip compressed data, was "django_short_links-0.1.2.tar", max compression
```

## Comparing `django_short_links-0.1.1.tar` & `django_short_links-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,17 @@
--rw-r--r--   0        0        0     1095 2022-08-21 12:14:58.898018 django_short_links-0.1.1/LICENSE
--rw-r--r--   0        0        0        0 2022-08-21 12:10:59.901587 django_short_links-0.1.1/links/__init__.py
--rw-r--r--   0        0        0      167 2023-06-12 11:03:25.902464 django_short_links-0.1.1/links/admin.py
--rw-r--r--   0        0        0      218 2023-06-12 13:20:44.527009 django_short_links-0.1.1/links/apps.py
--rw-r--r--   0        0        0      228 2023-06-12 11:03:47.298696 django_short_links-0.1.1/links/forms.py
--rw-r--r--   0        0        0      849 2023-06-13 10:30:17.657675 django_short_links-0.1.1/links/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-06-12 10:57:28.904816 django_short_links-0.1.1/links/migrations/__init__.py
--rw-r--r--   0        0        0      654 2023-06-13 10:25:49.830518 django_short_links-0.1.1/links/models.py
--rw-r--r--   0        0        0      982 2023-06-12 12:33:21.684915 django_short_links-0.1.1/links/templates/links/base.html
--rw-r--r--   0        0        0     1719 2023-06-13 10:46:10.589864 django_short_links-0.1.1/links/templates/links/detail.html
--rw-r--r--   0        0        0     1860 2023-06-13 10:27:05.850608 django_short_links-0.1.1/links/templates/links/index.html
--rw-r--r--   0        0        0     1498 2023-06-12 13:21:10.628098 django_short_links-0.1.1/links/templates/registration/login.html
--rw-r--r--   0        0        0       84 2023-02-06 09:50:24.122941 django_short_links-0.1.1/links/tests.py
--rw-r--r--   0        0        0      416 2023-06-12 13:18:46.120022 django_short_links-0.1.1/links/urls.py
--rw-r--r--   0        0        0     1974 2023-06-13 10:44:53.464487 django_short_links-0.1.1/links/views.py
--rw-r--r--   0        0        0      512 2023-06-13 11:23:30.375363 django_short_links-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      802 2023-06-13 11:22:22.510332 django_short_links-0.1.1/README.md
--rw-r--r--   0        0        0     1409 1970-01-01 00:00:00.000000 django_short_links-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1095 2022-08-21 12:14:58.898018 django_short_links-0.1.2/LICENSE
+-rw-r--r--   0        0        0        0 2022-08-21 12:10:59.901587 django_short_links-0.1.2/links/__init__.py
+-rw-r--r--   0        0        0      167 2023-06-12 11:03:25.902464 django_short_links-0.1.2/links/admin.py
+-rw-r--r--   0        0        0      218 2023-06-12 13:20:44.527009 django_short_links-0.1.2/links/apps.py
+-rw-r--r--   0        0        0      228 2023-06-12 11:03:47.298696 django_short_links-0.1.2/links/forms.py
+-rw-r--r--   0        0        0      849 2023-06-13 10:30:17.657675 django_short_links-0.1.2/links/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-06-12 10:57:28.904816 django_short_links-0.1.2/links/migrations/__init__.py
+-rw-r--r--   0        0        0      654 2023-06-13 10:25:49.830518 django_short_links-0.1.2/links/models.py
+-rw-r--r--   0        0        0      982 2023-06-12 12:33:21.684915 django_short_links-0.1.2/links/templates/links/base.html
+-rw-r--r--   0        0        0     1719 2023-06-13 10:46:10.589864 django_short_links-0.1.2/links/templates/links/detail.html
+-rw-r--r--   0        0        0     1879 2023-06-13 14:23:34.656752 django_short_links-0.1.2/links/templates/links/index.html
+-rw-r--r--   0        0        0       84 2023-02-06 09:50:24.122941 django_short_links-0.1.2/links/tests.py
+-rw-r--r--   0        0        0      416 2023-06-12 13:18:46.120022 django_short_links-0.1.2/links/urls.py
+-rw-r--r--   0        0        0     1974 2023-06-13 10:44:53.464487 django_short_links-0.1.2/links/views.py
+-rw-r--r--   0        0        0      524 2023-06-13 12:23:10.526038 django_short_links-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      753 2023-06-13 12:22:40.155650 django_short_links-0.1.2/README.md
+-rw-r--r--   0        0        0     1372 1970-01-01 00:00:00.000000 django_short_links-0.1.2/PKG-INFO
```

### Comparing `django_short_links-0.1.1/LICENSE` & `django_short_links-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_short_links-0.1.1/links/migrations/0001_initial.py` & `django_short_links-0.1.2/links/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_short_links-0.1.1/links/models.py` & `django_short_links-0.1.2/links/models.py`

 * *Files identical despite different names*

### Comparing `django_short_links-0.1.1/links/templates/links/base.html` & `django_short_links-0.1.2/links/templates/links/base.html`

 * *Files identical despite different names*

### Comparing `django_short_links-0.1.1/links/templates/links/detail.html` & `django_short_links-0.1.2/links/templates/links/detail.html`

 * *Files identical despite different names*

### Comparing `django_short_links-0.1.1/links/templates/links/index.html` & `django_short_links-0.1.2/links/templates/links/index.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 {% extends 'links/base.html' %} {% load i18n %}
-{% block title %}{% translate 'Links | URL shortener web app' %}{% endblock %}
+{% block title %}{% translate 'Links | URL shortener' %}{% endblock %}
 {% block body_attrs %}class="overflow-hidden"{% endblock %}
 {% block main %}
 <div class="container d-flex align-items-center justify-content-between overflow-hidden" style="height: 100vh">
   <div class="w-100">
     <h1 class="display-1 fw-bold mb-4">
       <a href="{% url 'links:index' %}" class="text-decoration-none">
         {% translate 'Links' %}
       </a>
     </h1>
     {% block content %}
     <p class="lead mb-4">
       {% blocktranslate %}
-      URL shortener Django app.
+      A Django app that allows users to shorten long urls.
       {% endblocktranslate %}
     </p>
     {% if form.errors %}
     <div class="text-white p-3 border rounded-3" role="alert">
       {{ form.errors }}
     </div>
     {% endif %}
```

#### html2text {}

```diff
@@ -1,13 +1,14 @@
 {% extends 'links/base.html' %} {% load i18n %} {% block title %}{% translate
-'Links | URL shortener web app' %}{% endblock %} {% block body_attrs
-%}class="overflow-hidden"{% endblock %} {% block main %}
+'Links | URL shortener' %}{% endblock %} {% block body_attrs %}class="overflow-
+hidden"{% endblock %} {% block main %}
 ****** {%_translate_'Links'_%} ******
 {% block content %}
-{% blocktranslate %} URL shortener Django app. {% endblocktranslate %}
+{% blocktranslate %} A Django app that allows users to shorten long urls. {%
+endblocktranslate %}
 {% if form.errors %}
 {{ form.errors }}
 {% endif %}
 ***** Shorten URL *****
 {% csrf_token %}
 [Unknown INPUT type]  {% translate 'URL' %}  {% translate 'The URL to be
 shortened' %}
```

### Comparing `django_short_links-0.1.1/links/views.py` & `django_short_links-0.1.2/links/views.py`

 * *Files identical despite different names*

### Comparing `django_short_links-0.1.1/pyproject.toml` & `django_short_links-0.1.2/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "django-short-links"
-version = "0.1.1"
+version = "0.1.2"
 description = "URL shortener Django app"
 authors = ["Yousef Abu Shanab <josephyousef249@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "links" }]
-homepage = "https://github.com/youzarsiph/django-links/"
-repository = "https://github.com/youzarsiph/django-links/"
+homepage = "https://github.com/youzarsiph/django-short-links/"
+repository = "https://github.com/youzarsiph/django-short-links/"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 django = "^4.2"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `django_short_links-0.1.1/README.md` & `django_short_links-0.1.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 
 INSTALLED_APPS = [
     ...
     'links',
     ...
 ]
 
-# Your server's IP address with route of 'links.urls' appended to the end without trailing slash
-LINKS_SITE_URL = 'https://your.domain.com/l'
+# Your server's IP address without trailing slash
+LINKS_SITE_URL = 'https://your.domain.com'
 ```
 
 Include `links` URLConf, in project's `urls.py`:
 
 ```python
 # urls.py
```

### Comparing `django_short_links-0.1.1/PKG-INFO` & `django_short_links-0.1.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: django-short-links
-Version: 0.1.1
+Version: 0.1.2
 Summary: URL shortener Django app
-Home-page: https://github.com/youzarsiph/django-links/
+Home-page: https://github.com/youzarsiph/django-short-links/
 License: MIT
 Author: Yousef Abu Shanab
 Author-email: josephyousef249@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: django (>=4.2,<5.0)
-Project-URL: Repository, https://github.com/youzarsiph/django-links/
+Project-URL: Repository, https://github.com/youzarsiph/django-short-links/
 Description-Content-Type: text/markdown
 
 # django-short-links
 
 URL / Link shortener web app.
 
 ## Getting Started
@@ -35,16 +35,16 @@
 
 INSTALLED_APPS = [
     ...
     'links',
     ...
 ]
 
-# Your server's IP address with route of 'links.urls' appended to the end without trailing slash
-LINKS_SITE_URL = 'https://your.domain.com/l'
+# Your server's IP address without trailing slash
+LINKS_SITE_URL = 'https://your.domain.com'
 ```
 
 Include `links` URLConf, in project's `urls.py`:
 
 ```python
 # urls.py
```

