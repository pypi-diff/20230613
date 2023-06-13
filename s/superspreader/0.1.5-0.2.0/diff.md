# Comparing `tmp/superspreader-0.1.5.tar.gz` & `tmp/superspreader-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superspreader-0.1.5.tar", last modified: Thu Sep  1 12:41:34 2022, max compression
+gzip compressed data, was "superspreader-0.2.0.tar", last modified: Tue Jun 13 05:48:15 2023, max compression
```

## Comparing `superspreader-0.1.5.tar` & `superspreader-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 12:41:34.527619 superspreader-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (121)     1068 2022-09-01 12:41:22.000000 superspreader-0.1.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3239 2022-09-01 12:41:34.527619 superspreader-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2329 2022-09-01 12:41:22.000000 superspreader-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      230 2022-09-01 12:41:22.000000 superspreader-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       78 2022-09-01 12:41:34.527619 superspreader-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1507 2022-09-01 12:41:22.000000 superspreader-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 12:41:34.523620 superspreader-0.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 12:41:34.523620 superspreader-0.1.5/src/superspreader/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-01 12:41:22.000000 superspreader-0.1.5/src/superspreader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      414 2022-09-01 12:41:22.000000 superspreader-0.1.5/src/superspreader/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     3347 2022-09-01 12:41:22.000000 superspreader-0.1.5/src/superspreader/fields.py
--rw-r--r--   0 runner    (1001) docker     (121)      840 2022-09-01 12:41:22.000000 superspreader-0.1.5/src/superspreader/i18n.py
--rw-r--r--   0 runner    (1001) docker     (121)     1965 2022-09-01 12:41:22.000000 superspreader-0.1.5/src/superspreader/messages.py
--rw-r--r--   0 runner    (1001) docker     (121)     7939 2022-09-01 12:41:22.000000 superspreader-0.1.5/src/superspreader/sheets.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 12:41:34.527619 superspreader-0.1.5/src/superspreader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3239 2022-09-01 12:41:34.000000 superspreader-0.1.5/src/superspreader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      433 2022-09-01 12:41:34.000000 superspreader-0.1.5/src/superspreader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-01 12:41:34.000000 superspreader-0.1.5/src/superspreader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-09-01 12:41:34.000000 superspreader-0.1.5/src/superspreader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-09-01 12:41:34.000000 superspreader-0.1.5/src/superspreader.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:48:15.514573 superspreader-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-13 05:48:05.000000 superspreader-0.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-06-13 05:48:15.514573 superspreader-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-06-13 05:48:05.000000 superspreader-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-13 05:48:05.000000 superspreader-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-13 05:48:15.514573 superspreader-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-06-13 05:48:05.000000 superspreader-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:48:15.510573 superspreader-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:48:15.514573 superspreader-0.2.0/src/superspreader/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 05:48:05.000000 superspreader-0.2.0/src/superspreader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-13 05:48:05.000000 superspreader-0.2.0/src/superspreader/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-06-13 05:48:05.000000 superspreader-0.2.0/src/superspreader/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-13 05:48:05.000000 superspreader-0.2.0/src/superspreader/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-06-13 05:48:05.000000 superspreader-0.2.0/src/superspreader/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7986 2023-06-13 05:48:05.000000 superspreader-0.2.0/src/superspreader/sheets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:48:15.514573 superspreader-0.2.0/src/superspreader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-06-13 05:48:15.000000 superspreader-0.2.0/src/superspreader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-13 05:48:15.000000 superspreader-0.2.0/src/superspreader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 05:48:15.000000 superspreader-0.2.0/src/superspreader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-13 05:48:15.000000 superspreader-0.2.0/src/superspreader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-13 05:48:15.000000 superspreader-0.2.0/src/superspreader.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:48:15.514573 superspreader-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-06-13 05:48:05.000000 superspreader-0.2.0/tests/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-06-13 05:48:05.000000 superspreader-0.2.0/tests/test_full_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-13 05:48:05.000000 superspreader-0.2.0/tests/test_sheet.py
```

### Comparing `superspreader-0.1.5/LICENSE.txt` & `superspreader-0.2.0/LICENSE.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 julianklotz
+Copyright (c) 2022, 2023 julianklotz
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `superspreader-0.1.5/PKG-INFO` & `superspreader-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superspreader
-Version: 0.1.5
+Version: 0.2.0
 Summary: Load data from spreadsheets easily
 Home-page: https://github.com/julianklotz/superspreader
 Author: Julian Klotz
 Author-email: post@julianklotz.de
 Project-URL: Source, https://github.com/julianklotz/superspreader
 Keywords: excel,spreadsheets,import,csv,tsv,openpyxl
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `superspreader-0.1.5/README.md` & `superspreader-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `superspreader-0.1.5/setup.py` & `superspreader-0.2.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,17 @@
-"""A setuptools based setup module.
-
-See:
-https://packaging.python.org/guides/distributing-packages-using-setuptools/
-https://github.com/pypa/sampleproject
-"""
-
 import pathlib
 
 from setuptools import find_packages, setup
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="superspreader",
-    version="0.1.5",
+    version="0.2.0",
     description="Load data from spreadsheets easily",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/julianklotz/superspreader",
     author="Julian Klotz",
     author_email="post@julianklotz.de",
     classifiers=[
```

### Comparing `superspreader-0.1.5/src/superspreader/fields.py` & `superspreader-0.2.0/src/superspreader/fields.py`

 * *Files identical despite different names*

### Comparing `superspreader-0.1.5/src/superspreader/i18n.py` & `superspreader-0.2.0/src/superspreader/i18n.py`

 * *Files identical despite different names*

### Comparing `superspreader-0.1.5/src/superspreader/messages.py` & `superspreader-0.2.0/src/superspreader/messages.py`

 * *Files identical despite different names*

### Comparing `superspreader-0.1.5/src/superspreader/sheets.py` & `superspreader-0.2.0/src/superspreader/sheets.py`

 * *Files 1% similar despite different names*

```diff
@@ -244,14 +244,15 @@
         """
         column_map = {}
         label_row = self.get_label_row()
 
         for index, column in enumerate(
             sheet.iter_cols(0, sheet.max_column, min_row=label_row, max_row=label_row)
         ):
+            key = str(column[0].value).strip()
             column_map[column[0].value] = index
 
         return column_map
 
     def __check_columns_present(self, column_map) -> None:
         """
         Checks whether the columns (described by the source attribute of fields) are present.
```

### Comparing `superspreader-0.1.5/src/superspreader.egg-info/PKG-INFO` & `superspreader-0.2.0/src/superspreader.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superspreader
-Version: 0.1.5
+Version: 0.2.0
 Summary: Load data from spreadsheets easily
 Home-page: https://github.com/julianklotz/superspreader
 Author: Julian Klotz
 Author-email: post@julianklotz.de
 Project-URL: Source, https://github.com/julianklotz/superspreader
 Keywords: excel,spreadsheets,import,csv,tsv,openpyxl
 Classifier: Development Status :: 3 - Alpha
```

