# Comparing `tmp/superspreader-0.2.0.tar.gz` & `tmp/superspreader-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superspreader-0.2.0.tar", last modified: Tue Jun 13 05:48:15 2023, max compression
+gzip compressed data, was "superspreader-0.2.1.tar", last modified: Tue Jun 13 07:26:27 2023, max compression
```

## Comparing `superspreader-0.2.0.tar` & `superspreader-0.2.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:48:15.514573 superspreader-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-13 05:48:05.000000 superspreader-0.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-06-13 05:48:15.514573 superspreader-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-06-13 05:48:05.000000 superspreader-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-13 05:48:05.000000 superspreader-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-13 05:48:15.514573 superspreader-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-06-13 05:48:05.000000 superspreader-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:48:15.510573 superspreader-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:48:15.514573 superspreader-0.2.0/src/superspreader/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 05:48:05.000000 superspreader-0.2.0/src/superspreader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-13 05:48:05.000000 superspreader-0.2.0/src/superspreader/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-06-13 05:48:05.000000 superspreader-0.2.0/src/superspreader/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-13 05:48:05.000000 superspreader-0.2.0/src/superspreader/i18n.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-06-13 05:48:05.000000 superspreader-0.2.0/src/superspreader/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     7986 2023-06-13 05:48:05.000000 superspreader-0.2.0/src/superspreader/sheets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:48:15.514573 superspreader-0.2.0/src/superspreader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-06-13 05:48:15.000000 superspreader-0.2.0/src/superspreader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-13 05:48:15.000000 superspreader-0.2.0/src/superspreader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 05:48:15.000000 superspreader-0.2.0/src/superspreader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-13 05:48:15.000000 superspreader-0.2.0/src/superspreader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-13 05:48:15.000000 superspreader-0.2.0/src/superspreader.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:48:15.514573 superspreader-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-06-13 05:48:05.000000 superspreader-0.2.0/tests/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-06-13 05:48:05.000000 superspreader-0.2.0/tests/test_full_import.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-13 05:48:05.000000 superspreader-0.2.0/tests/test_sheet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:26:27.606954 superspreader-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-13 07:26:18.000000 superspreader-0.2.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-06-13 07:26:27.606954 superspreader-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-06-13 07:26:18.000000 superspreader-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-13 07:26:18.000000 superspreader-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-13 07:26:27.606954 superspreader-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-06-13 07:26:18.000000 superspreader-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:26:27.602954 superspreader-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:26:27.602954 superspreader-0.2.1/src/superspreader/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 07:26:18.000000 superspreader-0.2.1/src/superspreader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-13 07:26:18.000000 superspreader-0.2.1/src/superspreader/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-06-13 07:26:18.000000 superspreader-0.2.1/src/superspreader/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-13 07:26:18.000000 superspreader-0.2.1/src/superspreader/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-06-13 07:26:18.000000 superspreader-0.2.1/src/superspreader/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8045 2023-06-13 07:26:18.000000 superspreader-0.2.1/src/superspreader/sheets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:26:27.602954 superspreader-0.2.1/src/superspreader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-06-13 07:26:27.000000 superspreader-0.2.1/src/superspreader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-13 07:26:27.000000 superspreader-0.2.1/src/superspreader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 07:26:27.000000 superspreader-0.2.1/src/superspreader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-13 07:26:27.000000 superspreader-0.2.1/src/superspreader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-13 07:26:27.000000 superspreader-0.2.1/src/superspreader.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:26:27.606954 superspreader-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-06-13 07:26:18.000000 superspreader-0.2.1/tests/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-06-13 07:26:18.000000 superspreader-0.2.1/tests/test_full_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-13 07:26:18.000000 superspreader-0.2.1/tests/test_sheet.py
```

### Comparing `superspreader-0.2.0/LICENSE.txt` & `superspreader-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `superspreader-0.2.0/PKG-INFO` & `superspreader-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superspreader
-Version: 0.2.0
+Version: 0.2.1
 Summary: Load data from spreadsheets easily
 Home-page: https://github.com/julianklotz/superspreader
 Author: Julian Klotz
 Author-email: post@julianklotz.de
 Project-URL: Source, https://github.com/julianklotz/superspreader
 Keywords: excel,spreadsheets,import,csv,tsv,openpyxl
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `superspreader-0.2.0/README.md` & `superspreader-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `superspreader-0.2.0/setup.py` & `superspreader-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages, setup
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="superspreader",
-    version="0.2.0",
+    version="0.2.1",
     description="Load data from spreadsheets easily",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/julianklotz/superspreader",
     author="Julian Klotz",
     author_email="post@julianklotz.de",
     classifiers=[
```

### Comparing `superspreader-0.2.0/src/superspreader/fields.py` & `superspreader-0.2.1/src/superspreader/fields.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,39 +4,61 @@
 
 from .exceptions import ImproperlyConfigured, ValidationException
 from .i18n import translate as _
 
 
 class BaseField(ABC):
     target_type = None
-    check_type = True
+    default = None
+    cast_type = True
 
-    def __init__(self, source, required=True):
+    def __init__(self, source, required=True, default=None):
         self.source = source
         self.required = required
         self.language = None
         self.extra_context = None
 
-    def __call__(self, value, language, extra_context={}):
+        if default is not None:
+            self.default = default
+
+    def __call__(self, value, language, extra_context=None):
+        if extra_context is None:
+            extra_context = {}
+
         self.extra_context = extra_context
         self.language = language
+
+        if value is None:
+            value = self.get_default()
+
         if value is None and self.required is True:
             msg = _("field.is_required", params={"field": self.source})
             raise ValidationException(msg)
 
         return self.clean(value)
 
     def get_target_type(self):
+        """
+        The field value’s desired type, used for casting primitive types.
+        In more advanced cases, disable type casting (cast_type=False) and implement
+        your own logic in `clean`.
+        """
         return self.target_type
 
+    def get_default(self):
+        """
+        Gets the default value for the field
+        """
+        return self.default
+
     def clean(self, value):
         if value is None:
             return
 
-        if self.check_type:
+        if self.cast_type:
             desired_type = self.get_target_type()
             if desired_type is None:
                 raise ImproperlyConfigured(
                     f"You have to specify a target type for"
                     f" {self.__class__.__name__}"
                 )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `superspreader-0.2.0/src/superspreader/i18n.py` & `superspreader-0.2.1/src/superspreader/i18n.py`

 * *Files identical despite different names*

### Comparing `superspreader-0.2.0/src/superspreader/messages.py` & `superspreader-0.2.1/src/superspreader/messages.py`

 * *Files identical despite different names*

### Comparing `superspreader-0.2.0/src/superspreader/sheets.py` & `superspreader-0.2.1/src/superspreader/sheets.py`

 * *Files 1% similar despite different names*

```diff
@@ -244,16 +244,17 @@
         """
         column_map = {}
         label_row = self.get_label_row()
 
         for index, column in enumerate(
             sheet.iter_cols(0, sheet.max_column, min_row=label_row, max_row=label_row)
         ):
+            # Retrieve and sanitize the column name from a header cell
             key = str(column[0].value).strip()
-            column_map[column[0].value] = index
+            column_map[key] = index
 
         return column_map
 
     def __check_columns_present(self, column_map) -> None:
         """
         Checks whether the columns (described by the source attribute of fields) are present.
         Missing columns are added to error list.
```

### Comparing `superspreader-0.2.0/src/superspreader.egg-info/PKG-INFO` & `superspreader-0.2.1/src/superspreader.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superspreader
-Version: 0.2.0
+Version: 0.2.1
 Summary: Load data from spreadsheets easily
 Home-page: https://github.com/julianklotz/superspreader
 Author: Julian Klotz
 Author-email: post@julianklotz.de
 Project-URL: Source, https://github.com/julianklotz/superspreader
 Keywords: excel,spreadsheets,import,csv,tsv,openpyxl
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `superspreader-0.2.0/tests/test_fields.py` & `superspreader-0.2.1/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `superspreader-0.2.0/tests/test_full_import.py` & `superspreader-0.2.1/tests/test_full_import.py`

 * *Files identical despite different names*

### Comparing `superspreader-0.2.0/tests/test_sheet.py` & `superspreader-0.2.1/tests/test_sheet.py`

 * *Files identical despite different names*

