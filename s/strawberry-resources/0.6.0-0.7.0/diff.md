# Comparing `tmp/strawberry_resources-0.6.0.tar.gz` & `tmp/strawberry_resources-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strawberry_resources-0.6.0.tar", max compression
+gzip compressed data, was "strawberry_resources-0.7.0.tar", max compression
```

## Comparing `strawberry_resources-0.6.0.tar` & `strawberry_resources-0.7.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1069 2023-05-10 21:14:53.479685 strawberry_resources-0.6.0/LICENSE
--rw-r--r--   0        0        0     9125 2023-05-10 21:14:53.479685 strawberry_resources-0.6.0/README.md
--rw-r--r--   0        0        0     4057 2023-05-10 21:14:53.479685 strawberry_resources-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     1174 2023-05-10 21:14:53.479685 strawberry_resources-0.6.0/strawberry_resources/__init__.py
--rw-r--r--   0        0        0       59 2023-05-10 21:14:53.479685 strawberry_resources-0.6.0/strawberry_resources/__main__.py
--rw-r--r--   0        0        0      123 2023-05-10 21:14:53.479685 strawberry_resources-0.6.0/strawberry_resources/cli/__init__.py
--rw-r--r--   0        0        0     1268 2023-05-10 21:14:53.479685 strawberry_resources-0.6.0/strawberry_resources/cli/export.py
--rw-r--r--   0        0        0     2828 2023-05-10 21:14:53.479685 strawberry_resources-0.6.0/strawberry_resources/exporter.py
--rw-r--r--   0        0        0      124 2023-05-10 21:14:53.479685 strawberry_resources-0.6.0/strawberry_resources/integrations/__init__.py
--rw-r--r--   0        0        0     1660 2023-05-10 21:14:53.479685 strawberry_resources-0.6.0/strawberry_resources/integrations/base.py
--rw-r--r--   0        0        0    10066 2023-05-10 21:14:53.479685 strawberry_resources-0.6.0/strawberry_resources/integrations/django.py
--rw-r--r--   0        0        0        0 2023-05-10 21:14:53.479685 strawberry_resources-0.6.0/strawberry_resources/py.typed
--rw-r--r--   0        0        0      628 2023-05-10 21:14:53.479685 strawberry_resources-0.6.0/strawberry_resources/queries.py
--rw-r--r--   0        0        0     7741 2023-05-10 21:14:53.479685 strawberry_resources-0.6.0/strawberry_resources/resolver.py
--rw-r--r--   0        0        0     7143 2023-05-10 21:14:53.479685 strawberry_resources-0.6.0/strawberry_resources/types.py
--rw-r--r--   0        0        0        0 2023-05-10 21:14:53.483685 strawberry_resources-0.6.0/strawberry_resources/utils/__init__.py
--rw-r--r--   0        0        0     2033 2023-05-10 21:14:53.483685 strawberry_resources-0.6.0/strawberry_resources/utils/inspect.py
--rw-r--r--   0        0        0      662 2023-05-10 21:14:53.483685 strawberry_resources-0.6.0/strawberry_resources/utils/pyutils.py
--rw-r--r--   0        0        0    10950 1970-01-01 00:00:00.000000 strawberry_resources-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-13 19:38:27.583874 strawberry_resources-0.7.0/LICENSE
+-rw-r--r--   0        0        0     9125 2023-06-13 19:38:27.583874 strawberry_resources-0.7.0/README.md
+-rw-r--r--   0        0        0     4034 2023-06-13 19:38:27.583874 strawberry_resources-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     1174 2023-06-13 19:38:27.583874 strawberry_resources-0.7.0/strawberry_resources/__init__.py
+-rw-r--r--   0        0        0       59 2023-06-13 19:38:27.583874 strawberry_resources-0.7.0/strawberry_resources/__main__.py
+-rw-r--r--   0        0        0      123 2023-06-13 19:38:27.583874 strawberry_resources-0.7.0/strawberry_resources/cli/__init__.py
+-rw-r--r--   0        0        0     1268 2023-06-13 19:38:27.583874 strawberry_resources-0.7.0/strawberry_resources/cli/export.py
+-rw-r--r--   0        0        0     2828 2023-06-13 19:38:27.583874 strawberry_resources-0.7.0/strawberry_resources/exporter.py
+-rw-r--r--   0        0        0      124 2023-06-13 19:38:27.583874 strawberry_resources-0.7.0/strawberry_resources/integrations/__init__.py
+-rw-r--r--   0        0        0     1660 2023-06-13 19:38:27.583874 strawberry_resources-0.7.0/strawberry_resources/integrations/base.py
+-rw-r--r--   0        0        0    10066 2023-06-13 19:38:27.583874 strawberry_resources-0.7.0/strawberry_resources/integrations/django.py
+-rw-r--r--   0        0        0        0 2023-06-13 19:38:27.583874 strawberry_resources-0.7.0/strawberry_resources/py.typed
+-rw-r--r--   0        0        0      628 2023-06-13 19:38:27.583874 strawberry_resources-0.7.0/strawberry_resources/queries.py
+-rw-r--r--   0        0        0     7741 2023-06-13 19:38:27.583874 strawberry_resources-0.7.0/strawberry_resources/resolver.py
+-rw-r--r--   0        0        0     7169 2023-06-13 19:38:27.583874 strawberry_resources-0.7.0/strawberry_resources/types.py
+-rw-r--r--   0        0        0        0 2023-06-13 19:38:27.583874 strawberry_resources-0.7.0/strawberry_resources/utils/__init__.py
+-rw-r--r--   0        0        0     2033 2023-06-13 19:38:27.583874 strawberry_resources-0.7.0/strawberry_resources/utils/inspect.py
+-rw-r--r--   0        0        0      662 2023-06-13 19:38:27.583874 strawberry_resources-0.7.0/strawberry_resources/utils/pyutils.py
+-rw-r--r--   0        0        0    10700 1970-01-01 00:00:00.000000 strawberry_resources-0.7.0/PKG-INFO
```

### Comparing `strawberry_resources-0.6.0/LICENSE` & `strawberry_resources-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `strawberry_resources-0.6.0/README.md` & `strawberry_resources-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `strawberry_resources-0.6.0/pyproject.toml` & `strawberry_resources-0.7.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "strawberry-resources"
-version = "0.6.0"
+version = "0.7.0"
 description = "Introspection utilities to extract data from strawberry graphql"
 authors = ["Thiago Bellini Ribeiro <thiago@bellini.dev>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/blb-ventures/strawberry-resources"
 repository = "https://github.com/blb-ventures/strawberry-resources"
 documentation = "https://github.com/blb-ventures/strawberry-resources"
@@ -47,15 +47,15 @@
 django-types = "^0.17.0"
 django-phonenumber-field = "^7.0.0"
 codecov = "^2.1.12"
 pytest = "^7.1.2"
 pytest-cov = "^4.0.0"
 ipython = "^8.4.0"
 pytest-asyncio = "^0.21.0"
-ruff = "^0.0.263"
+ruff = "^0.0.272"
 pytest-django = "^4.5.2"
 
 [tool.poetry.extras]
 django = ["django", "strawberry-graphql-django"]
 django-plus = [
   "django",
   "strawberry-graphql-django",
@@ -131,16 +131,14 @@
   "__pycached__",
   "_build",
   "buck-out",
   "build",
   "dist",
 ]
 
-[tool.ruff.pyupgrade]
-
 [tool.ruff.isort]
 known-first-party = ["strawberry-django-plus"]
 
 [tool.black]
 line-length = 100
 target-version = ['py38', 'py39', 'py310', 'py311']
 preview = true
```

### Comparing `strawberry_resources-0.6.0/strawberry_resources/__init__.py` & `strawberry_resources-0.7.0/strawberry_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `strawberry_resources-0.6.0/strawberry_resources/cli/export.py` & `strawberry_resources-0.7.0/strawberry_resources/cli/export.py`

 * *Files identical despite different names*

### Comparing `strawberry_resources-0.6.0/strawberry_resources/exporter.py` & `strawberry_resources-0.7.0/strawberry_resources/exporter.py`

 * *Files identical despite different names*

### Comparing `strawberry_resources-0.6.0/strawberry_resources/integrations/base.py` & `strawberry_resources-0.7.0/strawberry_resources/integrations/base.py`

 * *Files identical despite different names*

### Comparing `strawberry_resources-0.6.0/strawberry_resources/integrations/django.py` & `strawberry_resources-0.7.0/strawberry_resources/integrations/django.py`

 * *Files identical despite different names*

### Comparing `strawberry_resources-0.6.0/strawberry_resources/queries.py` & `strawberry_resources-0.7.0/strawberry_resources/queries.py`

 * *Files identical despite different names*

### Comparing `strawberry_resources-0.6.0/strawberry_resources/resolver.py` & `strawberry_resources-0.7.0/strawberry_resources/resolver.py`

 * *Files identical despite different names*

### Comparing `strawberry_resources-0.6.0/strawberry_resources/types.py` & `strawberry_resources-0.7.0/strawberry_resources/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,14 +63,15 @@
     TIME = "time"
     URL = "url"
     UUID = "uuid"
     POINT = "point"
     GEOPOINT = "geopoint"
     POLYGON = "polygon"
     DISTANCE = "distance"
+    MARKDOWN = "markdown"
 
 
 @strawberry.enum
 class FieldObjectKind(enum.Enum):
     """The kind of the nested object.
 
     The options here are:
```

### Comparing `strawberry_resources-0.6.0/strawberry_resources/utils/inspect.py` & `strawberry_resources-0.7.0/strawberry_resources/utils/inspect.py`

 * *Files identical despite different names*

### Comparing `strawberry_resources-0.6.0/strawberry_resources/utils/pyutils.py` & `strawberry_resources-0.7.0/strawberry_resources/utils/pyutils.py`

 * *Files identical despite different names*

### Comparing `strawberry_resources-0.6.0/PKG-INFO` & `strawberry_resources-0.7.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strawberry-resources
-Version: 0.6.0
+Version: 0.7.0
 Summary: Introspection utilities to extract data from strawberry graphql
 Home-page: https://github.com/blb-ventures/strawberry-resources
 License: MIT
 Keywords: strawberry,django,graphql,resources,forms
 Author: Thiago Bellini Ribeiro
 Author-email: thiago@bellini.dev
 Requires-Python: >=3.8,<4.0
@@ -15,19 +15,14 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: django
 Provides-Extra: django-plus
 Requires-Dist: click (>=8.1.3)
 Requires-Dist: django (>=3.2) ; extra == "django" or extra == "django-plus"
 Requires-Dist: django-choices-field (>=2.0) ; extra == "django-plus"
 Requires-Dist: strawberry-django-plus (>=2.0) ; extra == "django-plus"
 Requires-Dist: strawberry-graphql (>=0.140.3)
```

