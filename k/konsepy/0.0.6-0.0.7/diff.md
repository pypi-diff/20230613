# Comparing `tmp/konsepy-0.0.6.tar.gz` & `tmp/konsepy-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "konsepy-0.0.6.tar", last modified: Thu May  4 19:07:12 2023, max compression
+gzip compressed data, was "konsepy-0.0.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `konsepy-0.0.6.tar` & `konsepy-0.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      996 2023-05-04 19:07:07.877667 konsepy-0.0.6/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0        0        0       41 2023-05-04 19:07:07.877667 konsepy-0.0.6/.gitignore
--rw-r--r--   0        0        0      803 2023-05-04 19:07:07.877667 konsepy-0.0.6/CHANGELOG.md
--rw-r--r--   0        0        0      335 2023-05-04 19:07:07.877667 konsepy-0.0.6/README.md
--rw-r--r--   0        0        0      905 2023-05-04 19:07:07.877667 konsepy-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      110 2023-05-04 19:07:07.877667 konsepy-0.0.6/src/konsepy/__init__.py
--rw-r--r--   0        0        0     4116 2023-05-04 19:07:07.877667 konsepy-0.0.6/src/konsepy/bio_tag.py
--rw-r--r--   0        0        0     3056 2023-05-04 19:07:07.877667 konsepy-0.0.6/src/konsepy/cli.py
--rw-r--r--   0        0        0      104 2023-05-04 19:07:07.877667 konsepy-0.0.6/src/konsepy/constants.py
--rw-r--r--   0        0        0     4480 2023-05-04 19:07:07.877667 konsepy-0.0.6/src/konsepy/get_text_snippets.py
--rw-r--r--   0        0        0     1564 2023-05-04 19:07:07.877667 konsepy-0.0.6/src/konsepy/importer.py
--rw-r--r--   0        0        0     5284 2023-05-04 19:07:07.877667 konsepy-0.0.6/src/konsepy/regex.py
--rw-r--r--   0        0        0     2469 2023-05-04 19:07:07.877667 konsepy-0.0.6/src/konsepy/run_all.py
--rw-r--r--   0        0        0      654 2023-05-04 19:07:07.877667 konsepy-0.0.6/src/konsepy/rxutils.py
--rw-r--r--   0        0        0     5285 2023-05-04 19:07:07.877667 konsepy-0.0.6/src/konsepy/textio.py
--rw-r--r--   0        0        0      202 2023-05-04 19:07:07.877667 konsepy-0.0.6/src/konsepy/types.py
--rw-r--r--   0        0        0     1297 2023-05-04 19:07:07.877667 konsepy-0.0.6/test/build.ps1
--rw-r--r--   0        0        0     1212 1970-01-01 00:00:00.000000 konsepy-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      996 2023-06-13 19:40:44.640376 konsepy-0.0.7/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0        0        0       41 2023-06-13 19:40:44.640376 konsepy-0.0.7/.gitignore
+-rw-r--r--   0        0        0      803 2023-06-13 19:40:44.640376 konsepy-0.0.7/CHANGELOG.md
+-rw-r--r--   0        0        0      335 2023-06-13 19:40:44.640376 konsepy-0.0.7/README.md
+-rw-r--r--   0        0        0      905 2023-06-13 19:40:44.640376 konsepy-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      110 2023-06-13 19:40:44.640376 konsepy-0.0.7/src/konsepy/__init__.py
+-rw-r--r--   0        0        0     4116 2023-06-13 19:40:44.640376 konsepy-0.0.7/src/konsepy/bio_tag.py
+-rw-r--r--   0        0        0     3056 2023-06-13 19:40:44.640376 konsepy-0.0.7/src/konsepy/cli.py
+-rw-r--r--   0        0        0      104 2023-06-13 19:40:44.640376 konsepy-0.0.7/src/konsepy/constants.py
+-rw-r--r--   0        0        0     4480 2023-06-13 19:40:44.640376 konsepy-0.0.7/src/konsepy/get_text_snippets.py
+-rw-r--r--   0        0        0     1564 2023-06-13 19:40:44.640376 konsepy-0.0.7/src/konsepy/importer.py
+-rw-r--r--   0        0        0     5284 2023-06-13 19:40:44.640376 konsepy-0.0.7/src/konsepy/regex.py
+-rw-r--r--   0        0        0     2469 2023-06-13 19:40:44.640376 konsepy-0.0.7/src/konsepy/run_all.py
+-rw-r--r--   0        0        0      654 2023-06-13 19:40:44.640376 konsepy-0.0.7/src/konsepy/rxutils.py
+-rw-r--r--   0        0        0     5285 2023-06-13 19:40:44.640376 konsepy-0.0.7/src/konsepy/textio.py
+-rw-r--r--   0        0        0      202 2023-06-13 19:40:44.640376 konsepy-0.0.7/src/konsepy/types.py
+-rw-r--r--   0        0        0     1297 2023-06-13 19:40:44.640376 konsepy-0.0.7/test/build.ps1
+-rw-r--r--   0        0        0     1212 1970-01-01 00:00:00.000000 konsepy-0.0.7/PKG-INFO
```

### Comparing `konsepy-0.0.6/.github/workflows/publish-to-pypi.yml` & `konsepy-0.0.7/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `konsepy-0.0.6/CHANGELOG.md` & `konsepy-0.0.7/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `konsepy-0.0.6/pyproject.toml` & `konsepy-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `konsepy-0.0.6/src/konsepy/bio_tag.py` & `konsepy-0.0.7/src/konsepy/bio_tag.py`

 * *Files identical despite different names*

### Comparing `konsepy-0.0.6/src/konsepy/cli.py` & `konsepy-0.0.7/src/konsepy/cli.py`

 * *Files identical despite different names*

### Comparing `konsepy-0.0.6/src/konsepy/get_text_snippets.py` & `konsepy-0.0.7/src/konsepy/get_text_snippets.py`

 * *Files identical despite different names*

### Comparing `konsepy-0.0.6/src/konsepy/importer.py` & `konsepy-0.0.7/src/konsepy/importer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import importlib
 import pkgutil
-from enum import EnumType
+from enum import EnumMeta
 from pathlib import Path
 
 from loguru import logger
 
 
 class ConceptImport:
 
@@ -24,15 +24,15 @@
 
     @property
     def categories(self):
         return [category.name for category in self.category_enum]
 
     def _get_category(self):
         for name, value in self.imp.__dict__.items():
-            if isinstance(value, EnumType):
+            if isinstance(value, EnumMeta):
                 return value
         raise ValueError(f'Unable to identify category enum for concept "{self.name}".')
 
     def __str__(self):
         return f'ConceptImport<{self.name}>'
```

### Comparing `konsepy-0.0.6/src/konsepy/regex.py` & `konsepy-0.0.7/src/konsepy/regex.py`

 * *Files identical despite different names*

### Comparing `konsepy-0.0.6/src/konsepy/run_all.py` & `konsepy-0.0.7/src/konsepy/run_all.py`

 * *Files identical despite different names*

### Comparing `konsepy-0.0.6/src/konsepy/rxutils.py` & `konsepy-0.0.7/src/konsepy/rxutils.py`

 * *Files identical despite different names*

### Comparing `konsepy-0.0.6/src/konsepy/textio.py` & `konsepy-0.0.7/src/konsepy/textio.py`

 * *Files identical despite different names*

### Comparing `konsepy-0.0.6/test/build.ps1` & `konsepy-0.0.7/test/build.ps1`

 * *Files identical despite different names*

### Comparing `konsepy-0.0.6/PKG-INFO` & `konsepy-0.0.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: konsepy
-Version: 0.0.6
+Version: 0.0.7
 Summary: Framework for build NLP information extraction systems using regular expressions.
 Keywords: nlp
 Author-email: dcronkite <dcronkite+pypi@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

