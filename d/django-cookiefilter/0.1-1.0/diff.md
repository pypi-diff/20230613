# Comparing `tmp/django-cookiefilter-0.1.tar.gz` & `tmp/django-cookiefilter-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-cookiefilter-0.1.tar", last modified: Mon Jan  7 13:35:22 2019, max compression
+gzip compressed data, was "django-cookiefilter-1.0.tar", last modified: Tue Jun 13 10:45:17 2023, max compression
```

## Comparing `django-cookiefilter-0.1.tar` & `django-cookiefilter-1.0.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxr-xr-x   0 tomkins    (501) staff       (20)        0 2019-01-07 13:35:22.000000 django-cookiefilter-0.1/
--rw-r--r--   0 tomkins    (501) staff       (20)     1503 2019-01-06 15:05:06.000000 django-cookiefilter-0.1/LICENSE
--rw-r--r--   0 tomkins    (501) staff       (20)      130 2019-01-06 15:19:18.000000 django-cookiefilter-0.1/MANIFEST.in
--rw-r--r--   0 tomkins    (501) staff       (20)      931 2019-01-07 13:35:22.000000 django-cookiefilter-0.1/PKG-INFO
--rw-r--r--   0 tomkins    (501) staff       (20)     1155 2019-01-06 22:47:11.000000 django-cookiefilter-0.1/README.rst
-drwxr-xr-x   0 tomkins    (501) staff       (20)        0 2019-01-07 13:35:22.000000 django-cookiefilter-0.1/cookiefilter/
--rw-r--r--   0 tomkins    (501) staff       (20)       20 2019-01-07 13:34:14.000000 django-cookiefilter-0.1/cookiefilter/__init__.py
--rw-r--r--   0 tomkins    (501) staff       (20)     2186 2019-01-06 22:47:11.000000 django-cookiefilter-0.1/cookiefilter/middleware.py
-drwxr-xr-x   0 tomkins    (501) staff       (20)        0 2019-01-07 13:35:22.000000 django-cookiefilter-0.1/django_cookiefilter.egg-info/
--rw-r--r--   0 tomkins    (501) staff       (20)      931 2019-01-07 13:35:22.000000 django-cookiefilter-0.1/django_cookiefilter.egg-info/PKG-INFO
--rw-r--r--   0 tomkins    (501) staff       (20)      315 2019-01-07 13:35:22.000000 django-cookiefilter-0.1/django_cookiefilter.egg-info/SOURCES.txt
--rw-r--r--   0 tomkins    (501) staff       (20)        1 2019-01-07 13:35:22.000000 django-cookiefilter-0.1/django_cookiefilter.egg-info/dependency_links.txt
--rw-r--r--   0 tomkins    (501) staff       (20)       12 2019-01-07 13:35:22.000000 django-cookiefilter-0.1/django_cookiefilter.egg-info/requires.txt
--rw-r--r--   0 tomkins    (501) staff       (20)       13 2019-01-07 13:35:22.000000 django-cookiefilter-0.1/django_cookiefilter.egg-info/top_level.txt
--rw-r--r--   0 tomkins    (501) staff       (20)       67 2019-01-07 13:35:22.000000 django-cookiefilter-0.1/setup.cfg
--rw-r--r--   0 tomkins    (501) staff       (20)     1179 2019-01-07 13:34:14.000000 django-cookiefilter-0.1/setup.py
+drwxr-xr-x   0 tomkins    (501) staff       (20)        0 2023-06-13 10:45:17.057679 django-cookiefilter-1.0/
+-rw-r--r--   0 tomkins    (501) staff       (20)     1508 2023-06-13 10:38:06.000000 django-cookiefilter-1.0/LICENSE
+-rw-r--r--   0 tomkins    (501) staff       (20)      130 2020-10-05 00:00:12.000000 django-cookiefilter-1.0/MANIFEST.in
+-rw-r--r--   0 tomkins    (501) staff       (20)     2127 2023-06-13 10:45:17.057776 django-cookiefilter-1.0/PKG-INFO
+-rw-r--r--   0 tomkins    (501) staff       (20)     1158 2023-06-11 18:29:47.000000 django-cookiefilter-1.0/README.rst
+drwxr-xr-x   0 tomkins    (501) staff       (20)        0 2023-06-13 10:45:17.056659 django-cookiefilter-1.0/cookiefilter/
+-rw-r--r--   0 tomkins    (501) staff       (20)       20 2023-06-13 10:39:26.000000 django-cookiefilter-1.0/cookiefilter/__init__.py
+-rw-r--r--   0 tomkins    (501) staff       (20)     2297 2020-10-15 15:47:34.000000 django-cookiefilter-1.0/cookiefilter/middleware.py
+drwxr-xr-x   0 tomkins    (501) staff       (20)        0 2023-06-13 10:45:17.057329 django-cookiefilter-1.0/django_cookiefilter.egg-info/
+-rw-r--r--   0 tomkins    (501) staff       (20)     2127 2023-06-13 10:45:17.000000 django-cookiefilter-1.0/django_cookiefilter.egg-info/PKG-INFO
+-rw-r--r--   0 tomkins    (501) staff       (20)      355 2023-06-13 10:45:17.000000 django-cookiefilter-1.0/django_cookiefilter.egg-info/SOURCES.txt
+-rw-r--r--   0 tomkins    (501) staff       (20)        1 2023-06-13 10:45:17.000000 django-cookiefilter-1.0/django_cookiefilter.egg-info/dependency_links.txt
+-rw-r--r--   0 tomkins    (501) staff       (20)       12 2023-06-13 10:45:17.000000 django-cookiefilter-1.0/django_cookiefilter.egg-info/requires.txt
+-rw-r--r--   0 tomkins    (501) staff       (20)       13 2023-06-13 10:45:17.000000 django-cookiefilter-1.0/django_cookiefilter.egg-info/top_level.txt
+-rw-r--r--   0 tomkins    (501) staff       (20)      366 2023-06-13 10:38:06.000000 django-cookiefilter-1.0/pyproject.toml
+-rw-r--r--   0 tomkins    (501) staff       (20)       70 2023-06-13 10:45:17.058296 django-cookiefilter-1.0/setup.cfg
+-rw-r--r--   0 tomkins    (501) staff       (20)     1363 2023-06-13 10:39:26.000000 django-cookiefilter-1.0/setup.py
+drwxr-xr-x   0 tomkins    (501) staff       (20)        0 2023-06-13 10:45:17.057437 django-cookiefilter-1.0/tests/
+-rw-r--r--   0 tomkins    (501) staff       (20)     1702 2020-10-15 15:47:34.000000 django-cookiefilter-1.0/tests/test_middleware.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-cookiefilter-0.1/LICENSE` & `django-cookiefilter-1.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2019, Developer Society Limited
+Copyright (c) 2019-2023, Developer Society Limited
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright notice, this
   list of conditions and the following disclaimer.
```

### Comparing `django-cookiefilter-0.1/README.rst` & `django-cookiefilter-1.0/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -13,21 +13,20 @@
 
 .. _pip: https://pip.pypa.io/
 
 .. code-block:: console
 
     $ pip install django-cookiefilter
 
-Edit your Django project's settings module, and add the middleware to the start of  ``MIDDLEWARE``
-(or ``MIDDLEWARE_CLASSES`` for Django 1.8):
+Edit your Django project's settings module, and add the middleware to the start of ``MIDDLEWARE``:
 
 .. code-block:: python
 
     MIDDLEWARE = [
-        'cookiefilter.middleware.CookieFilterMiddleware',
+        "cookiefilter.middleware.CookieFilterMiddleware",
         # ...
     ]
 
 .. note::
 
     The middleware should be added before ``UpdateCacheMiddleware``, as it uses the value of
     HTTP_COOKIES which needs to be modified.
@@ -38,11 +37,13 @@
 Out of the box the standard Django cookie names will work without any other configuration. However
 if your project uses different or additional cookie names, edit ``COOKIEFILTER_ALLOWED`` in your
 project's settings module:
 
 .. code-block:: python
 
     COOKIEFILTER_ALLOWED = [
-        'analytics',
-        'csrftoken',
-        'sessionid',
+        "analytics",
+        "csrftoken",
+        "django_language",
+        "messages",
+        "sessionid",
     ]
```

### Comparing `django-cookiefilter-0.1/cookiefilter/middleware.py` & `django-cookiefilter-1.0/cookiefilter/middleware.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,58 +1,63 @@
 import logging
 from http.cookies import SimpleCookie
 
 from django.conf import settings
 from django.contrib.messages.storage.cookie import CookieStorage
 
-try:
-    from django.utils.deprecation import MiddlewareMixin
-except ImportError:
-    MiddlewareMixin = object
-
 logger = logging.getLogger(__name__)
 
 
-class CookieFilterMiddleware(MiddlewareMixin):
+class CookieFilterMiddleware:
     """
     Middleware which removes all unwanted cookies.
 
     By default standard Django cookies are allowed. This setting can be changed either in the
     Django project settings, or by extending this class.
     """
+
     allowed_cookies = set(
         getattr(
-            settings, 'COOKIEFILTER_ALLOWED', [
+            settings,
+            "COOKIEFILTER_ALLOWED",
+            [
                 settings.CSRF_COOKIE_NAME,
                 settings.LANGUAGE_COOKIE_NAME,
                 settings.SESSION_COOKIE_NAME,
                 CookieStorage.cookie_name,
-            ]
+            ],
         )
     )
 
-    def process_request(self, request):
+    def __init__(self, get_response):
+        self.get_response = get_response
+
+    def __call__(self, request):
         # First step - find out if there are any unwanted cookies being set
         current_cookies = set(request.COOKIES.keys())
         unwanted_cookies = current_cookies.difference(self.allowed_cookies)
 
         if unwanted_cookies:
             # There are some unwanted cookies, so we create a new COOKIES dict containing only the
             # cookies we want
             wanted_cookies = current_cookies.intersection(self.allowed_cookies)
 
-            logger.debug('Deleted %d cookie(s)', len(unwanted_cookies))
+            logger.debug("Deleted %d cookie(s)", len(unwanted_cookies))
 
             request.COOKIES = {key: request.COOKIES[key] for key in wanted_cookies}
 
             # Other code in Django will inspect HTTP_COOKIES, so we need to recreate this as if the
             # browser only sent these cookies in the first place
             cookies = SimpleCookie(input=request.COOKIES)
-            cookie_string = cookies.output(header='', sep=';')
+            cookie_string = cookies.output(header="", sep=";")
             # cookies.output is usually for output headers, so we need to left strip whitespace
             cookie_string = cookie_string.lstrip()
 
             if cookie_string:
-                request.META['HTTP_COOKIE'] = cookie_string
+                request.META["HTTP_COOKIE"] = cookie_string
             else:
                 # If there aren't any cookies left, then just remove the header
-                del request.META['HTTP_COOKIE']
+                del request.META["HTTP_COOKIE"]
+
+        # Now let remaining middleware or the view handle the request
+        response = self.get_response(request)
+        return response
```

