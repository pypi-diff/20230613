# Comparing `tmp/django-htmx-1.8.0.tar.gz` & `tmp/django-htmx-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-htmx-1.8.0.tar", last modified: Mon Jan 10 16:52:43 2022, max compression
+gzip compressed data, was "django-htmx-1.9.0.tar", last modified: Wed Mar  2 08:46:00 2022, max compression
```

## Comparing `django-htmx-1.8.0.tar` & `django-htmx-1.9.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 chainz     (501) staff       (20)        0 2022-01-10 16:52:43.327699 django-htmx-1.8.0/
--rw-r--r--   0 chainz     (501) staff       (20)     3374 2022-01-10 16:52:36.000000 django-htmx-1.8.0/HISTORY.rst
--rw-r--r--   0 chainz     (501) staff       (20)     1061 2021-02-07 13:10:39.000000 django-htmx-1.8.0/LICENSE
--rw-r--r--   0 chainz     (501) staff       (20)      286 2021-12-28 23:48:50.000000 django-htmx-1.8.0/MANIFEST.in
--rw-r--r--   0 chainz     (501) staff       (20)    11312 2022-01-10 16:52:43.327968 django-htmx-1.8.0/PKG-INFO
--rw-r--r--   0 chainz     (501) staff       (20)    10097 2022-01-10 16:13:36.000000 django-htmx-1.8.0/README.rst
--rw-r--r--   0 chainz     (501) staff       (20)      636 2022-01-10 16:13:36.000000 django-htmx-1.8.0/pyproject.toml
--rw-r--r--   0 chainz     (501) staff       (20)     1482 2022-01-10 16:52:43.328844 django-htmx-1.8.0/setup.cfg
--rw-r--r--   0 chainz     (501) staff       (20)       38 2021-02-07 13:10:39.000000 django-htmx-1.8.0/setup.py
-drwxr-xr-x   0 chainz     (501) staff       (20)        0 2022-01-10 16:52:43.322209 django-htmx-1.8.0/src/
-drwxr-xr-x   0 chainz     (501) staff       (20)        0 2022-01-10 16:52:43.325299 django-htmx-1.8.0/src/django_htmx/
--rw-r--r--   0 chainz     (501) staff       (20)        0 2021-02-05 10:18:49.000000 django-htmx-1.8.0/src/django_htmx/__init__.py
--rw-r--r--   0 chainz     (501) staff       (20)     1759 2022-01-10 14:33:04.000000 django-htmx-1.8.0/src/django_htmx/http.py
--rw-r--r--   0 chainz     (501) staff       (20)      498 2022-01-05 10:17:10.000000 django-htmx-1.8.0/src/django_htmx/jinja.py
--rw-r--r--   0 chainz     (501) staff       (20)     2110 2021-10-06 15:15:55.000000 django-htmx-1.8.0/src/django_htmx/middleware.py
--rw-r--r--   0 chainz     (501) staff       (20)        0 2021-08-04 15:28:07.000000 django-htmx-1.8.0/src/django_htmx/py.typed
-drwxr-xr-x   0 chainz     (501) staff       (20)        0 2022-01-10 16:52:43.326951 django-htmx-1.8.0/src/django_htmx/static/
--rw-r--r--   0 chainz     (501) staff       (20)      741 2021-07-09 14:31:16.000000 django-htmx-1.8.0/src/django_htmx/static/django-htmx.js
-drwxr-xr-x   0 chainz     (501) staff       (20)        0 2022-01-10 16:52:43.327395 django-htmx-1.8.0/src/django_htmx/templatetags/
--rw-r--r--   0 chainz     (501) staff       (20)        0 2021-07-08 09:06:55.000000 django-htmx-1.8.0/src/django_htmx/templatetags/__init__.py
--rw-r--r--   0 chainz     (501) staff       (20)      149 2021-07-08 09:06:55.000000 django-htmx-1.8.0/src/django_htmx/templatetags/django_htmx.py
-drwxr-xr-x   0 chainz     (501) staff       (20)        0 2022-01-10 16:52:43.326712 django-htmx-1.8.0/src/django_htmx.egg-info/
--rw-r--r--   0 chainz     (501) staff       (20)    11312 2022-01-10 16:52:43.000000 django-htmx-1.8.0/src/django_htmx.egg-info/PKG-INFO
--rw-r--r--   0 chainz     (501) staff       (20)      563 2022-01-10 16:52:43.000000 django-htmx-1.8.0/src/django_htmx.egg-info/SOURCES.txt
--rw-r--r--   0 chainz     (501) staff       (20)        1 2022-01-10 16:52:43.000000 django-htmx-1.8.0/src/django_htmx.egg-info/dependency_links.txt
--rw-r--r--   0 chainz     (501) staff       (20)        1 2022-01-10 16:52:43.000000 django-htmx-1.8.0/src/django_htmx.egg-info/not-zip-safe
--rw-r--r--   0 chainz     (501) staff       (20)       12 2022-01-10 16:52:43.000000 django-htmx-1.8.0/src/django_htmx.egg-info/requires.txt
--rw-r--r--   0 chainz     (501) staff       (20)       12 2022-01-10 16:52:43.000000 django-htmx-1.8.0/src/django_htmx.egg-info/top_level.txt
+drwxr-xr-x   0 chainz     (501) staff       (20)        0 2022-03-02 08:46:00.172407 django-htmx-1.9.0/
+-rw-r--r--   0 chainz     (501) staff       (20)     3866 2022-03-02 08:45:50.000000 django-htmx-1.9.0/HISTORY.rst
+-rw-r--r--   0 chainz     (501) staff       (20)     1069 2022-01-19 15:27:56.000000 django-htmx-1.9.0/LICENSE
+-rw-r--r--   0 chainz     (501) staff       (20)      323 2022-03-02 08:08:57.000000 django-htmx-1.9.0/MANIFEST.in
+-rw-r--r--   0 chainz     (501) staff       (20)     2591 2022-03-02 08:46:00.172571 django-htmx-1.9.0/PKG-INFO
+-rw-r--r--   0 chainz     (501) staff       (20)     1312 2022-03-02 08:08:57.000000 django-htmx-1.9.0/README.rst
+-rw-r--r--   0 chainz     (501) staff       (20)      687 2022-03-01 11:54:31.000000 django-htmx-1.9.0/pyproject.toml
+-rw-r--r--   0 chainz     (501) staff       (20)     1544 2022-03-02 08:46:00.173360 django-htmx-1.9.0/setup.cfg
+-rw-r--r--   0 chainz     (501) staff       (20)       74 2022-01-19 11:13:52.000000 django-htmx-1.9.0/setup.py
+drwxr-xr-x   0 chainz     (501) staff       (20)        0 2022-03-02 08:46:00.166183 django-htmx-1.9.0/src/
+drwxr-xr-x   0 chainz     (501) staff       (20)        0 2022-03-02 08:46:00.169762 django-htmx-1.9.0/src/django_htmx/
+-rw-r--r--   0 chainz     (501) staff       (20)        0 2021-02-05 10:18:49.000000 django-htmx-1.9.0/src/django_htmx/__init__.py
+-rw-r--r--   0 chainz     (501) staff       (20)     1927 2022-03-02 08:27:24.000000 django-htmx-1.9.0/src/django_htmx/http.py
+-rw-r--r--   0 chainz     (501) staff       (20)      534 2022-01-19 11:13:52.000000 django-htmx-1.9.0/src/django_htmx/jinja.py
+-rw-r--r--   0 chainz     (501) staff       (20)     2118 2022-01-19 11:13:52.000000 django-htmx-1.9.0/src/django_htmx/middleware.py
+-rw-r--r--   0 chainz     (501) staff       (20)        0 2021-08-04 15:28:07.000000 django-htmx-1.9.0/src/django_htmx/py.typed
+drwxr-xr-x   0 chainz     (501) staff       (20)        0 2022-03-02 08:46:00.171665 django-htmx-1.9.0/src/django_htmx/static/
+-rw-r--r--   0 chainz     (501) staff       (20)      741 2021-07-09 14:31:16.000000 django-htmx-1.9.0/src/django_htmx/static/django-htmx.js
+drwxr-xr-x   0 chainz     (501) staff       (20)        0 2022-03-02 08:46:00.172129 django-htmx-1.9.0/src/django_htmx/templatetags/
+-rw-r--r--   0 chainz     (501) staff       (20)        0 2021-07-08 09:06:55.000000 django-htmx-1.9.0/src/django_htmx/templatetags/__init__.py
+-rw-r--r--   0 chainz     (501) staff       (20)      185 2022-01-19 11:13:52.000000 django-htmx-1.9.0/src/django_htmx/templatetags/django_htmx.py
+drwxr-xr-x   0 chainz     (501) staff       (20)        0 2022-03-02 08:46:00.171399 django-htmx-1.9.0/src/django_htmx.egg-info/
+-rw-r--r--   0 chainz     (501) staff       (20)     2591 2022-03-02 08:45:59.000000 django-htmx-1.9.0/src/django_htmx.egg-info/PKG-INFO
+-rw-r--r--   0 chainz     (501) staff       (20)      563 2022-03-02 08:46:00.000000 django-htmx-1.9.0/src/django_htmx.egg-info/SOURCES.txt
+-rw-r--r--   0 chainz     (501) staff       (20)        1 2022-03-02 08:45:59.000000 django-htmx-1.9.0/src/django_htmx.egg-info/dependency_links.txt
+-rw-r--r--   0 chainz     (501) staff       (20)        1 2022-03-02 08:45:59.000000 django-htmx-1.9.0/src/django_htmx.egg-info/not-zip-safe
+-rw-r--r--   0 chainz     (501) staff       (20)       12 2022-03-02 08:46:00.000000 django-htmx-1.9.0/src/django_htmx.egg-info/requires.txt
+-rw-r--r--   0 chainz     (501) staff       (20)       12 2022-03-02 08:46:00.000000 django-htmx-1.9.0/src/django_htmx.egg-info/top_level.txt
```

### Comparing `django-htmx-1.8.0/HISTORY.rst` & `django-htmx-1.9.0/HISTORY.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,23 @@
 =======
 History
 =======
 
+1.9.0 (2022-03-02)
+------------------
+
+* Move documentation from the README to `Read the Docs <https://django-htmx.readthedocs.io/>`__.
+  Also expand it with sections on installing htmx, and configuring CSRF.
+
+  Thanks to Ben Beecher for intial setup in `PR #194 <https://github.com/adamchainz/django-htmx/pull/194>`__.
+
+* Add ``HttpResponseClientRefresh`` for telling htmx to reload the page.
+
+  Thanks to Bogumil Schube in `PR #193 <https://github.com/adamchainz/django-htmx/pull/193>`__.
+
 1.8.0 (2022-01-10)
 ------------------
 
 * Drop Python 3.6 support.
 
 1.7.0 (2022-01-10)
 ------------------
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_4gsfgmhc_/tmpwxxbb01h_TarContainer/0/1.rst", line 107, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_4gsfgmhc_/tmpwxxbb01h_TarContainer/0/1.rst", line 107, column 0: CDATA terminal not found*

```diff
@@ -1,5 +1,13 @@
-======= History ======= 1.8.0 (2022-01-10) ------------------ * Drop Python 3.6
-support. 1.7.0 (2022-01-10) ------------------ * Use ``DjangoJSONEncoder`` for
-encoding the ``HX-Trigger`` event. Thanks to Cleiton de Lima in `PR #182
+======= History ======= 1.9.0 (2022-03-02) ------------------ * Move
+documentation from the README to `Read the Docs
+django-htmx.readthedocs.io/>`__. Also expand it with sections on installing
+htmx, and configuring CSRF. Thanks to Ben Beecher for intial setup in `PR #194
+github.com/adamchainz/django-htmx/pull/194>`__. * Add
+``HttpResponseClientRefresh`` for telling htmx to reload the page. Thanks to
+Bogumil Schube in `PR #193
+github.com/adamchainz/django-htmx/pull/193>`__. 1.8.0 (2022-01-10) ------------
+------ * Drop Python 3.6 support. 1.7.0 (2022-01-10) ------------------ * Use
+``DjangoJSONEncoder`` for encoding the ``HX-Trigger`` event. Thanks to Cleiton
+de Lima in `PR #182
 github.com/adamchainz/django-htmx/pull/182>`__. * Drop redundant 'async' from
 debug ``
```

### Comparing `django-htmx-1.8.0/LICENSE` & `django-htmx-1.9.0/LICENSE`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2020-2021
+Copyright (c) 2020 Adam Johnson
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `django-htmx-1.8.0/pyproject.toml` & `django-htmx-1.9.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.black]
 target-version = ['py37']
 
 [tool.isort]
 profile = "black"
+add_imports = "from __future__ import annotations"
 
 [tool.mypy]
 check_untyped_defs = true
 disallow_any_generics = true
 disallow_incomplete_defs = true
 disallow_untyped_defs = true
 mypy_path = "src/"
```

### Comparing `django-htmx-1.8.0/setup.cfg` & `django-htmx-1.9.0/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 [metadata]
 name = django-htmx
-version = 1.8.0
+version = 1.9.0
 description = Extensions for using Django with htmx.
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 author = Adam Johnson
 author_email = me@adamj.eu
 url = https://github.com/adamchainz/django-htmx
 project_urls = 
+	Documentation = https://django-htmx.readthedocs.io/
 	Changelog = https://github.com/adamchainz/django-htmx/blob/main/HISTORY.rst
 	Twitter = https://twitter.com/adamchainz
 license = MIT
 keywords = Django
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Framework :: Django :: 2.2
@@ -43,15 +44,17 @@
 
 [options.packages.find]
 where = src
 
 [coverage:run]
 branch = True
 parallel = True
-source = django_htmx
+source = 
+	django_htmx
+	tests
 
 [coverage:paths]
 source = 
 	src
 	.tox/*/site-packages
 
 [coverage:report]
```

### Comparing `django-htmx-1.8.0/src/django_htmx/http.py` & `django-htmx-1.9.0/src/django_htmx/http.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+from __future__ import annotations
+
 import json
 import sys
-from typing import Any, Dict
+from typing import Any
 
 from django.core.serializers.json import DjangoJSONEncoder
 from django.http import HttpResponse
 from django.http.response import HttpResponseRedirectBase
 
 if sys.version_info >= (3, 8):
     from typing import Literal
@@ -15,32 +17,38 @@
 
 HTMX_STOP_POLLING = 286
 
 
 class HttpResponseStopPolling(HttpResponse):
     status_code = HTMX_STOP_POLLING
 
-    def __init__(self, *args: object, **kwargs: object) -> None:
+    def __init__(self, *args: Any, **kwargs: Any) -> None:
         super().__init__(*args, **kwargs)
         self._reason_phrase = "Stop Polling"
 
 
 class HttpResponseClientRedirect(HttpResponseRedirectBase):
     status_code = 200
 
     def __init__(self, redirect_to: str, *args: Any, **kwargs: Any) -> None:
         super().__init__(redirect_to, *args, **kwargs)
         self["HX-Redirect"] = self["Location"]
         del self["Location"]
 
 
+class HttpResponseClientRefresh(HttpResponse):
+    def __init__(self) -> None:
+        super().__init__()
+        self["HX-Refresh"] = "true"
+
+
 def trigger_client_event(
     response: HttpResponse,
     name: str,
-    params: Dict[str, Any],
+    params: dict[str, Any],
     *,
     after: EventAfterType = "receive",
 ) -> None:
     if after == "receive":
         header = "HX-Trigger"
     elif after == "settle":
         header = "HX-Trigger-After-Settle"
```

### Comparing `django-htmx-1.8.0/src/django_htmx/middleware.py` & `django-htmx-1.9.0/src/django_htmx/middleware.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+from __future__ import annotations
+
 import json
-from typing import Any, Callable, Optional
+from typing import Any, Callable
 from urllib.parse import unquote
 
 from django.http import HttpRequest, HttpResponse
 from django.utils.functional import cached_property
 
 
 class HtmxMiddleware:
@@ -15,50 +17,50 @@
         return self.get_response(request)
 
 
 class HtmxDetails:
     def __init__(self, request: HttpRequest) -> None:
         self.request = request
 
-    def _get_header_value(self, name: str) -> Optional[str]:
+    def _get_header_value(self, name: str) -> str | None:
         value = self.request.headers.get(name) or None
         if value:
             if self.request.headers.get(f"{name}-URI-AutoEncoded") == "true":
                 value = unquote(value)
         return value
 
     def __bool__(self) -> bool:
         return self._get_header_value("HX-Request") == "true"
 
     @cached_property
     def boosted(self) -> bool:
         return self._get_header_value("HX-Boosted") == "true"
 
     @cached_property
-    def current_url(self) -> Optional[str]:
+    def current_url(self) -> str | None:
         return self._get_header_value("HX-Current-URL")
 
     @cached_property
     def history_restore_request(self) -> bool:
         return self._get_header_value("HX-History-Restore-Request") == "true"
 
     @cached_property
-    def prompt(self) -> Optional[str]:
+    def prompt(self) -> str | None:
         return self._get_header_value("HX-Prompt")
 
     @cached_property
-    def target(self) -> Optional[str]:
+    def target(self) -> str | None:
         return self._get_header_value("HX-Target")
 
     @cached_property
-    def trigger(self) -> Optional[str]:
+    def trigger(self) -> str | None:
         return self._get_header_value("HX-Trigger")
 
     @cached_property
-    def trigger_name(self) -> Optional[str]:
+    def trigger_name(self) -> str | None:
         return self._get_header_value("HX-Trigger-Name")
 
     @cached_property
     def triggering_event(self) -> Any:
         value = self._get_header_value("Triggering-Event")
         if value is not None:
             try:
```

### Comparing `django-htmx-1.8.0/src/django_htmx/static/django-htmx.js` & `django-htmx-1.9.0/src/django_htmx/static/django-htmx.js`

 * *Files identical despite different names*

### Comparing `django-htmx-1.8.0/src/django_htmx.egg-info/SOURCES.txt` & `django-htmx-1.9.0/src/django_htmx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

