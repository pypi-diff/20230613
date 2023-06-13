# Comparing `tmp/mail-cleaner-1.1.0.tar.gz` & `tmp/mail-cleaner-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mail-cleaner-1.1.0.tar", last modified: Wed Jan 18 13:24:54 2023, max compression
+gzip compressed data, was "mail-cleaner-1.2.0.tar", last modified: Tue Jun 13 16:59:45 2023, max compression
```

## Comparing `mail-cleaner-1.1.0.tar` & `mail-cleaner-1.2.0.tar`

### file list

```diff
@@ -1,25 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 13:24:54.396948 mail-cleaner-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-01-18 13:24:47.000000 mail-cleaner-1.1.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-01-18 13:24:47.000000 mail-cleaner-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-01-18 13:24:47.000000 mail-cleaner-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-01-18 13:24:54.396948 mail-cleaner-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-01-18 13:24:47.000000 mail-cleaner-1.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 13:24:54.392948 mail-cleaner-1.1.0/mail_cleaner/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-18 13:24:47.000000 mail-cleaner-1.1.0/mail_cleaner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-01-18 13:24:47.000000 mail-cleaner-1.1.0/mail_cleaner/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-01-18 13:24:47.000000 mail-cleaner-1.1.0/mail_cleaner/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-01-18 13:24:47.000000 mail-cleaner-1.1.0/mail_cleaner/mail.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-18 13:24:47.000000 mail-cleaner-1.1.0/mail_cleaner/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-01-18 13:24:47.000000 mail-cleaner-1.1.0/mail_cleaner/sanitizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-01-18 13:24:47.000000 mail-cleaner-1.1.0/mail_cleaner/text.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-01-18 13:24:47.000000 mail-cleaner-1.1.0/mail_cleaner/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 13:24:54.396948 mail-cleaner-1.1.0/mail_cleaner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-01-18 13:24:54.000000 mail-cleaner-1.1.0/mail_cleaner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-01-18 13:24:54.000000 mail-cleaner-1.1.0/mail_cleaner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-18 13:24:54.000000 mail-cleaner-1.1.0/mail_cleaner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-18 13:24:54.000000 mail-cleaner-1.1.0/mail_cleaner.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-01-18 13:24:54.000000 mail-cleaner-1.1.0/mail_cleaner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-01-18 13:24:54.000000 mail-cleaner-1.1.0/mail_cleaner.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-01-18 13:24:47.000000 mail-cleaner-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-01-18 13:24:54.396948 mail-cleaner-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-18 13:24:47.000000 mail-cleaner-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:59:45.219887 mail-cleaner-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-06-13 16:59:40.000000 mail-cleaner-1.2.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-06-13 16:59:40.000000 mail-cleaner-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-13 16:59:40.000000 mail-cleaner-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-06-13 16:59:45.219887 mail-cleaner-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-06-13 16:59:40.000000 mail-cleaner-1.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:59:45.219887 mail-cleaner-1.2.0/mail_cleaner/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 16:59:40.000000 mail-cleaner-1.2.0/mail_cleaner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-13 16:59:40.000000 mail-cleaner-1.2.0/mail_cleaner/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-06-13 16:59:40.000000 mail-cleaner-1.2.0/mail_cleaner/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-06-13 16:59:40.000000 mail-cleaner-1.2.0/mail_cleaner/mail.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 16:59:40.000000 mail-cleaner-1.2.0/mail_cleaner/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-06-13 16:59:40.000000 mail-cleaner-1.2.0/mail_cleaner/sanitizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-06-13 16:59:40.000000 mail-cleaner-1.2.0/mail_cleaner/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-13 16:59:40.000000 mail-cleaner-1.2.0/mail_cleaner/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:59:45.219887 mail-cleaner-1.2.0/mail_cleaner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-06-13 16:59:45.000000 mail-cleaner-1.2.0/mail_cleaner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-13 16:59:45.000000 mail-cleaner-1.2.0/mail_cleaner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 16:59:45.000000 mail-cleaner-1.2.0/mail_cleaner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 16:59:45.000000 mail-cleaner-1.2.0/mail_cleaner.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-13 16:59:45.000000 mail-cleaner-1.2.0/mail_cleaner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-13 16:59:45.000000 mail-cleaner-1.2.0/mail_cleaner.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-13 16:59:40.000000 mail-cleaner-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-06-13 16:59:45.219887 mail-cleaner-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 16:59:40.000000 mail-cleaner-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:59:45.219887 mail-cleaner-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-06-13 16:59:40.000000 mail-cleaner-1.2.0/tests/test_replace_data_uris.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-13 16:59:40.000000 mail-cleaner-1.2.0/tests/test_sanitizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-06-13 16:59:40.000000 mail-cleaner-1.2.0/tests/test_send_mail_plus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-06-13 16:59:40.000000 mail-cleaner-1.2.0/tests/test_strip_tags_plus.py
```

### Comparing `mail-cleaner-1.1.0/CHANGELOG.rst` & `mail-cleaner-1.2.0/CHANGELOG.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 =========
 Changelog
 =========
 
+1.2.0 (2023-06-13)
+==================
+
+* [#2] Add support for ``CC``.
+
 1.1.0 (2023-01-18)
 ==================
 
 Adds optional ``headers`` parameter to ``send_mail_plus``. These headers will
 end up in the header section of the body of the top message, not in any
 multipart "children" of the message.
```

### Comparing `mail-cleaner-1.1.0/LICENSE` & `mail-cleaner-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mail-cleaner-1.1.0/PKG-INFO` & `mail-cleaner-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mail-cleaner
-Version: 1.1.0
+Version: 1.2.0
 Summary: Handle and sanitize HTML & text emails
 Home-page: https://github.com/maykinmedia/mail-cleaner
 Author: Maykin Media
 Author-email: support@maykinmedia.nl
 License: MIT
 Project-URL: Documentation, http://mail-cleaner.readthedocs.io/en/latest/
 Project-URL: Changelog, https://github.com/maykinmedia/mail-cleaner/blob/main/CHANGELOG.rst
@@ -31,15 +31,15 @@
 Provides-Extra: docs
 Provides-Extra: release
 License-File: LICENSE
 
 mail-cleaner
 ============
 
-:Version: 1.1.0
+:Version: 1.2.0
 :Source: https://github.com/maykinmedia/mail-cleaner
 :Keywords: django, email, sanitize
 :PythonVersion: 3.9
 
 |build-status| |code-quality| |black| |coverage| |docs|
 
 |python-versions| |django-versions| |pypi-version|
```

### Comparing `mail-cleaner-1.1.0/README.rst` & `mail-cleaner-1.2.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 mail-cleaner
 ============
 
-:Version: 1.1.0
+:Version: 1.2.0
 :Source: https://github.com/maykinmedia/mail-cleaner
 :Keywords: django, email, sanitize
 :PythonVersion: 3.9
 
 |build-status| |code-quality| |black| |coverage| |docs|
 
 |python-versions| |django-versions| |pypi-version|
```

### Comparing `mail-cleaner-1.1.0/mail_cleaner/constants.py` & `mail-cleaner-1.2.0/mail_cleaner/constants.py`

 * *Files identical despite different names*

### Comparing `mail-cleaner-1.1.0/mail_cleaner/mail.py` & `mail-cleaner-1.2.0/mail_cleaner/mail.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 
 
 def send_mail_plus(
     subject: str,
     message: str,
     from_email: Optional[str],
     recipient_list: Optional[Sequence[str]],
+    cc: Optional[Sequence[str]],
     fail_silently: bool = False,
     auth_user: Optional[str] = None,
     auth_password: Optional[str] = None,
     connection=None,
     html_message: Optional[str] = None,
     attachments: Optional[Iterable["_AttachmentTuple"]] = None,
     headers: Optional[Dict[str, str]] = None,
@@ -50,14 +51,15 @@
     )
     headers = headers or {}
     mail = EmailMultiAlternatives(
         subject,
         message,
         from_email,
         recipient_list,
+        cc=cc,
         connection=connection,
         headers=headers,
     )
     if html_message:
         html_message, mime_images = replace_datauri_images(html_message)
 
         mail.attach_alternative(html_message, "text/html")
```

### Comparing `mail-cleaner-1.1.0/mail_cleaner/sanitizer.py` & `mail-cleaner-1.2.0/mail_cleaner/sanitizer.py`

 * *Files identical despite different names*

### Comparing `mail-cleaner-1.1.0/mail_cleaner/text.py` & `mail-cleaner-1.2.0/mail_cleaner/text.py`

 * *Files identical despite different names*

### Comparing `mail-cleaner-1.1.0/mail_cleaner.egg-info/PKG-INFO` & `mail-cleaner-1.2.0/mail_cleaner.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mail-cleaner
-Version: 1.1.0
+Version: 1.2.0
 Summary: Handle and sanitize HTML & text emails
 Home-page: https://github.com/maykinmedia/mail-cleaner
 Author: Maykin Media
 Author-email: support@maykinmedia.nl
 License: MIT
 Project-URL: Documentation, http://mail-cleaner.readthedocs.io/en/latest/
 Project-URL: Changelog, https://github.com/maykinmedia/mail-cleaner/blob/main/CHANGELOG.rst
@@ -31,15 +31,15 @@
 Provides-Extra: docs
 Provides-Extra: release
 License-File: LICENSE
 
 mail-cleaner
 ============
 
-:Version: 1.1.0
+:Version: 1.2.0
 :Source: https://github.com/maykinmedia/mail-cleaner
 :Keywords: django, email, sanitize
 :PythonVersion: 3.9
 
 |build-status| |code-quality| |black| |coverage| |docs|
 
 |python-versions| |django-versions| |pypi-version|
```

### Comparing `mail-cleaner-1.1.0/setup.cfg` & `mail-cleaner-1.2.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mail-cleaner
-version = 1.1.0
+version = 1.2.0
 description = Handle and sanitize HTML & text emails
 long_description = file: README.rst
 url = https://github.com/maykinmedia/mail-cleaner
 project_urls = 
 	Documentation = http://mail-cleaner.readthedocs.io/en/latest/
 	Changelog = https://github.com/maykinmedia/mail-cleaner/blob/main/CHANGELOG.rst
 	Bug Tracker = https://github.com/maykinmedia/mail-cleaner/issues
```

