# Comparing `tmp/aflabs_test_app-0.1.0.tar.gz` & `tmp/aflabs_test_app-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aflabs_test_app-0.1.0.tar", max compression
+gzip compressed data, was "aflabs_test_app-0.1.1.tar", max compression
```

## Comparing `aflabs_test_app-0.1.0.tar` & `aflabs_test_app-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0       28 2023-06-13 07:10:38.510387 aflabs_test_app-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-06-13 07:06:35.380152 aflabs_test_app-0.1.0/books/__init__.py
--rw-r--r--   0        0        0       90 2023-06-13 07:06:35.380152 aflabs_test_app-0.1.0/books/admin.py
--rw-r--r--   0        0        0       85 2023-06-13 07:06:35.380152 aflabs_test_app-0.1.0/books/apps.py
--rw-r--r--   0        0        0      164 2023-06-13 07:06:35.380152 aflabs_test_app-0.1.0/books/forms.py
--rw-r--r--   0        0        0      938 2023-06-13 07:06:35.380152 aflabs_test_app-0.1.0/books/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-06-13 07:06:35.380152 aflabs_test_app-0.1.0/books/migrations/__init__.py
--rw-r--r--   0        0        0      887 2023-06-13 07:06:35.380152 aflabs_test_app-0.1.0/books/migrations/__pycache__/0001_initial.cpython-39.pyc
--rw-r--r--   0        0        0      146 2023-06-13 07:06:35.380152 aflabs_test_app-0.1.0/books/migrations/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      559 2023-06-13 07:06:35.380152 aflabs_test_app-0.1.0/books/models.py
--rw-r--r--   0        0        0     1226 2023-06-13 07:06:35.384153 aflabs_test_app-0.1.0/books/templates/author_books_edit.html
--rw-r--r--   0        0        0      723 2023-06-13 07:06:35.384153 aflabs_test_app-0.1.0/books/templates/author_create.html
--rw-r--r--   0        0        0      905 2023-06-13 07:06:35.384153 aflabs_test_app-0.1.0/books/templates/author_detail.html
--rw-r--r--   0        0        0      600 2023-06-13 07:06:35.384153 aflabs_test_app-0.1.0/books/templates/author_list.html
--rw-r--r--   0        0        0      769 2023-06-13 07:06:35.384153 aflabs_test_app-0.1.0/books/templates/base.html
--rw-r--r--   0        0        0      364 2023-06-13 07:06:35.384153 aflabs_test_app-0.1.0/books/templates/home.html
--rw-r--r--   0        0        0       60 2023-06-13 07:06:35.384153 aflabs_test_app-0.1.0/books/tests.py
--rw-r--r--   0        0        0      485 2023-06-13 07:06:35.384153 aflabs_test_app-0.1.0/books/urls.py
--rw-r--r--   0        0        0     1897 2023-06-13 07:06:35.384153 aflabs_test_app-0.1.0/books/views.py
--rw-r--r--   0        0        0      360 2023-06-13 07:16:12.947260 aflabs_test_app-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      416 1970-01-01 00:00:00.000000 aflabs_test_app-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       28 2023-06-13 07:10:38.510387 aflabs_test_app-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-13 07:06:35.380152 aflabs_test_app-0.1.1/books/__init__.py
+-rw-r--r--   0        0        0       90 2023-06-13 07:06:35.380152 aflabs_test_app-0.1.1/books/admin.py
+-rw-r--r--   0        0        0       85 2023-06-13 07:06:35.380152 aflabs_test_app-0.1.1/books/apps.py
+-rw-r--r--   0        0        0      164 2023-06-13 07:06:35.380152 aflabs_test_app-0.1.1/books/forms.py
+-rw-r--r--   0        0        0      938 2023-06-13 07:06:35.380152 aflabs_test_app-0.1.1/books/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-06-13 07:06:35.380152 aflabs_test_app-0.1.1/books/migrations/__init__.py
+-rw-r--r--   0        0        0      887 2023-06-13 07:06:35.380152 aflabs_test_app-0.1.1/books/migrations/__pycache__/0001_initial.cpython-39.pyc
+-rw-r--r--   0        0        0      146 2023-06-13 07:06:35.380152 aflabs_test_app-0.1.1/books/migrations/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      559 2023-06-13 07:06:35.380152 aflabs_test_app-0.1.1/books/models.py
+-rw-r--r--   0        0        0     1226 2023-06-13 07:06:35.384153 aflabs_test_app-0.1.1/books/templates/author_books_edit.html
+-rw-r--r--   0        0        0      723 2023-06-13 07:06:35.384153 aflabs_test_app-0.1.1/books/templates/author_create.html
+-rw-r--r--   0        0        0      905 2023-06-13 07:06:35.384153 aflabs_test_app-0.1.1/books/templates/author_detail.html
+-rw-r--r--   0        0        0      600 2023-06-13 07:06:35.384153 aflabs_test_app-0.1.1/books/templates/author_list.html
+-rw-r--r--   0        0        0      769 2023-06-13 07:06:35.384153 aflabs_test_app-0.1.1/books/templates/base.html
+-rw-r--r--   0        0        0      364 2023-06-13 07:06:35.384153 aflabs_test_app-0.1.1/books/templates/home.html
+-rw-r--r--   0        0        0       60 2023-06-13 07:06:35.384153 aflabs_test_app-0.1.1/books/tests.py
+-rw-r--r--   0        0        0      485 2023-06-13 07:06:35.384153 aflabs_test_app-0.1.1/books/urls.py
+-rw-r--r--   0        0        0     1897 2023-06-13 07:06:35.384153 aflabs_test_app-0.1.1/books/views.py
+-rw-r--r--   0        0        0      343 2023-06-13 07:19:15.228479 aflabs_test_app-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      378 1970-01-01 00:00:00.000000 aflabs_test_app-0.1.1/PKG-INFO
```

### Comparing `aflabs_test_app-0.1.0/books/migrations/0001_initial.py` & `aflabs_test_app-0.1.1/books/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aflabs_test_app-0.1.0/books/migrations/__pycache__/0001_initial.cpython-39.pyc` & `aflabs_test_app-0.1.1/books/migrations/__pycache__/0001_initial.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aflabs_test_app-0.1.0/books/models.py` & `aflabs_test_app-0.1.1/books/models.py`

 * *Files identical despite different names*

### Comparing `aflabs_test_app-0.1.0/books/templates/author_books_edit.html` & `aflabs_test_app-0.1.1/books/templates/author_books_edit.html`

 * *Files identical despite different names*

### Comparing `aflabs_test_app-0.1.0/books/templates/author_create.html` & `aflabs_test_app-0.1.1/books/templates/author_create.html`

 * *Files identical despite different names*

### Comparing `aflabs_test_app-0.1.0/books/templates/author_detail.html` & `aflabs_test_app-0.1.1/books/templates/author_detail.html`

 * *Files identical despite different names*

### Comparing `aflabs_test_app-0.1.0/books/templates/author_list.html` & `aflabs_test_app-0.1.1/books/templates/author_list.html`

 * *Files identical despite different names*

### Comparing `aflabs_test_app-0.1.0/books/templates/base.html` & `aflabs_test_app-0.1.1/books/templates/base.html`

 * *Files identical despite different names*

### Comparing `aflabs_test_app-0.1.0/books/views.py` & `aflabs_test_app-0.1.1/books/views.py`

 * *Files identical despite different names*

