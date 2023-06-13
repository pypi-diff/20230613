# Comparing `tmp/fileformats-0.6.1.tar.gz` & `tmp/fileformats-0.6.2.tar.gz`

## Comparing `fileformats-0.6.1.tar` & `fileformats-0.6.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 fileformats-0.6.1/fileformats/archive/__init__.py
--rw-r--r--   0        0        0     8869 2020-02-02 00:00:00.000000 fileformats-0.6.1/fileformats/archive/converters.py
--rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 fileformats-0.6.1/fileformats/archive/tests/test_archive_converters.py
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 fileformats-0.6.1/fileformats/audio/__init__.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 fileformats-0.6.1/fileformats/core/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 fileformats-0.6.1/fileformats/core/_version.py
--rw-r--r--   0        0        0    41153 2020-02-02 00:00:00.000000 fileformats-0.6.1/fileformats/core/base.py
--rw-r--r--   0        0        0     5584 2020-02-02 00:00:00.000000 fileformats-0.6.1/fileformats/core/converter.py
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 fileformats-0.6.1/fileformats/core/exceptions.py
--rw-r--r--   0        0        0     4609 2020-02-02 00:00:00.000000 fileformats-0.6.1/fileformats/core/mark.py
--rw-r--r--   0        0        0    24541 2020-02-02 00:00:00.000000 fileformats-0.6.1/fileformats/core/mixin.py
--rw-r--r--   0        0        0    10881 2020-02-02 00:00:00.000000 fileformats-0.6.1/fileformats/core/utils.py
--rw-r--r--   0        0        0     8171 2020-02-02 00:00:00.000000 fileformats-0.6.1/fileformats/core/tests/test_classifiers.py
--rw-r--r--   0        0        0     3990 2020-02-02 00:00:00.000000 fileformats-0.6.1/fileformats/core/tests/test_converter.py
--rw-r--r--   0        0        0     5998 2020-02-02 00:00:00.000000 fileformats-0.6.1/fileformats/core/tests/test_detection.py
--rw-r--r--   0        0        0     3336 2020-02-02 00:00:00.000000 fileformats-0.6.1/fileformats/core/tests/test_general.py
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 fileformats-0.6.1/fileformats/core/tests/test_mime.py
--rw-r--r--   0        0        0     7043 2020-02-02 00:00:00.000000 fileformats-0.6.1/fileformats/core/tests/test_mixin.py
--rw-r--r--   0        0        0     5884 2020-02-02 00:00:00.000000 fileformats-0.6.1/fileformats/core/tests/test_utils.py
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 fileformats-0.6.1/fileformats/document/__init__.py
--rw-r--r--   0        0        0     4843 2020-02-02 00:00:00.000000 fileformats-0.6.1/fileformats/field/__init__.py
--rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 fileformats-0.6.1/fileformats/field/tests/test_fields.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 fileformats-0.6.1/fileformats/field/tests/test_fields_mime.py
--rw-r--r--   0        0        0     7937 2020-02-02 00:00:00.000000 fileformats-0.6.1/fileformats/generic/__init__.py
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 fileformats-0.6.1/fileformats/image/__init__.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 fileformats-0.6.1/fileformats/image/base.py
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 fileformats-0.6.1/fileformats/image/converters.py
--rw-r--r--   0        0        0     1893 2020-02-02 00:00:00.000000 fileformats-0.6.1/fileformats/image/raster.py
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 fileformats-0.6.1/fileformats/image/vector.py
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 fileformats-0.6.1/fileformats/image/tests/test_image_converters.py
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 fileformats-0.6.1/fileformats/image/tests/test_image_raster.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 fileformats-0.6.1/fileformats/misc/__init__.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 fileformats-0.6.1/fileformats/misc/medical.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 fileformats-0.6.1/fileformats/numeric/__init__.py
--rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 fileformats-0.6.1/fileformats/serialization/__init__.py
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 fileformats-0.6.1/fileformats/serialization/converters.py
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 fileformats-0.6.1/fileformats/serialization/tests/test_serialization_converters.py
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 fileformats-0.6.1/fileformats/text/__init__.py
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 fileformats-0.6.1/fileformats/video/__init__.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 fileformats-0.6.1/.gitignore
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 fileformats-0.6.1/AUTHORS
--rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 fileformats-0.6.1/LICENSE
--rw-r--r--   0        0        0     5235 2020-02-02 00:00:00.000000 fileformats-0.6.1/README.rst
--rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 fileformats-0.6.1/pyproject.toml
--rw-r--r--   0        0        0    22512 2020-02-02 00:00:00.000000 fileformats-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 fileformats-0.6.2/fileformats/archive/__init__.py
+-rw-r--r--   0        0        0     8869 2020-02-02 00:00:00.000000 fileformats-0.6.2/fileformats/archive/converters.py
+-rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 fileformats-0.6.2/fileformats/archive/tests/test_archive_converters.py
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 fileformats-0.6.2/fileformats/audio/__init__.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 fileformats-0.6.2/fileformats/core/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 fileformats-0.6.2/fileformats/core/_version.py
+-rw-r--r--   0        0        0    41153 2020-02-02 00:00:00.000000 fileformats-0.6.2/fileformats/core/base.py
+-rw-r--r--   0        0        0     5584 2020-02-02 00:00:00.000000 fileformats-0.6.2/fileformats/core/converter.py
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 fileformats-0.6.2/fileformats/core/exceptions.py
+-rw-r--r--   0        0        0     4609 2020-02-02 00:00:00.000000 fileformats-0.6.2/fileformats/core/mark.py
+-rw-r--r--   0        0        0    24541 2020-02-02 00:00:00.000000 fileformats-0.6.2/fileformats/core/mixin.py
+-rw-r--r--   0        0        0    10881 2020-02-02 00:00:00.000000 fileformats-0.6.2/fileformats/core/utils.py
+-rw-r--r--   0        0        0     8171 2020-02-02 00:00:00.000000 fileformats-0.6.2/fileformats/core/tests/test_classifiers.py
+-rw-r--r--   0        0        0     3990 2020-02-02 00:00:00.000000 fileformats-0.6.2/fileformats/core/tests/test_converter.py
+-rw-r--r--   0        0        0     5998 2020-02-02 00:00:00.000000 fileformats-0.6.2/fileformats/core/tests/test_detection.py
+-rw-r--r--   0        0        0     3336 2020-02-02 00:00:00.000000 fileformats-0.6.2/fileformats/core/tests/test_general.py
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 fileformats-0.6.2/fileformats/core/tests/test_mime.py
+-rw-r--r--   0        0        0     7043 2020-02-02 00:00:00.000000 fileformats-0.6.2/fileformats/core/tests/test_mixin.py
+-rw-r--r--   0        0        0     5884 2020-02-02 00:00:00.000000 fileformats-0.6.2/fileformats/core/tests/test_utils.py
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 fileformats-0.6.2/fileformats/document/__init__.py
+-rw-r--r--   0        0        0     4843 2020-02-02 00:00:00.000000 fileformats-0.6.2/fileformats/field/__init__.py
+-rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 fileformats-0.6.2/fileformats/field/tests/test_fields.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 fileformats-0.6.2/fileformats/field/tests/test_fields_mime.py
+-rw-r--r--   0        0        0     7937 2020-02-02 00:00:00.000000 fileformats-0.6.2/fileformats/generic/__init__.py
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 fileformats-0.6.2/fileformats/image/__init__.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 fileformats-0.6.2/fileformats/image/base.py
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 fileformats-0.6.2/fileformats/image/converters.py
+-rw-r--r--   0        0        0     1893 2020-02-02 00:00:00.000000 fileformats-0.6.2/fileformats/image/raster.py
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 fileformats-0.6.2/fileformats/image/vector.py
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 fileformats-0.6.2/fileformats/image/tests/test_image_converters.py
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 fileformats-0.6.2/fileformats/image/tests/test_image_raster.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 fileformats-0.6.2/fileformats/misc/__init__.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 fileformats-0.6.2/fileformats/misc/medical.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 fileformats-0.6.2/fileformats/numeric/__init__.py
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 fileformats-0.6.2/fileformats/serialization/__init__.py
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 fileformats-0.6.2/fileformats/serialization/converters.py
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 fileformats-0.6.2/fileformats/serialization/tests/test_serialization_converters.py
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 fileformats-0.6.2/fileformats/text/__init__.py
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 fileformats-0.6.2/fileformats/video/__init__.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 fileformats-0.6.2/.gitignore
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 fileformats-0.6.2/AUTHORS
+-rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 fileformats-0.6.2/LICENSE
+-rw-r--r--   0        0        0     5235 2020-02-02 00:00:00.000000 fileformats-0.6.2/README.rst
+-rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 fileformats-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0    22512 2020-02-02 00:00:00.000000 fileformats-0.6.2/PKG-INFO
```

### Comparing `fileformats-0.6.1/fileformats/archive/__init__.py` & `fileformats-0.6.2/fileformats/archive/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.1/fileformats/archive/converters.py` & `fileformats-0.6.2/fileformats/archive/converters.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.1/fileformats/archive/tests/test_archive_converters.py` & `fileformats-0.6.2/fileformats/archive/tests/test_archive_converters.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.1/fileformats/audio/__init__.py` & `fileformats-0.6.2/fileformats/audio/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.1/fileformats/core/base.py` & `fileformats-0.6.2/fileformats/core/base.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.1/fileformats/core/converter.py` & `fileformats-0.6.2/fileformats/core/converter.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.1/fileformats/core/mark.py` & `fileformats-0.6.2/fileformats/core/mark.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.1/fileformats/core/mixin.py` & `fileformats-0.6.2/fileformats/core/mixin.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.1/fileformats/core/utils.py` & `fileformats-0.6.2/fileformats/core/utils.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.1/fileformats/core/tests/test_classifiers.py` & `fileformats-0.6.2/fileformats/core/tests/test_classifiers.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.1/fileformats/core/tests/test_converter.py` & `fileformats-0.6.2/fileformats/core/tests/test_converter.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.1/fileformats/core/tests/test_detection.py` & `fileformats-0.6.2/fileformats/core/tests/test_detection.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.1/fileformats/core/tests/test_general.py` & `fileformats-0.6.2/fileformats/core/tests/test_general.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.1/fileformats/core/tests/test_mime.py` & `fileformats-0.6.2/fileformats/core/tests/test_mime.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.1/fileformats/core/tests/test_mixin.py` & `fileformats-0.6.2/fileformats/core/tests/test_mixin.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.1/fileformats/core/tests/test_utils.py` & `fileformats-0.6.2/fileformats/core/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.1/fileformats/document/__init__.py` & `fileformats-0.6.2/fileformats/document/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.1/fileformats/field/__init__.py` & `fileformats-0.6.2/fileformats/field/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.1/fileformats/field/tests/test_fields.py` & `fileformats-0.6.2/fileformats/field/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.1/fileformats/field/tests/test_fields_mime.py` & `fileformats-0.6.2/fileformats/field/tests/test_fields_mime.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.1/fileformats/generic/__init__.py` & `fileformats-0.6.2/fileformats/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.1/fileformats/image/converters.py` & `fileformats-0.6.2/fileformats/image/converters.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.1/fileformats/image/raster.py` & `fileformats-0.6.2/fileformats/image/raster.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.1/fileformats/image/tests/test_image_converters.py` & `fileformats-0.6.2/fileformats/image/tests/test_image_converters.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.1/fileformats/image/tests/test_image_raster.py` & `fileformats-0.6.2/fileformats/image/tests/test_image_raster.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.1/fileformats/serialization/__init__.py` & `fileformats-0.6.2/fileformats/serialization/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.1/fileformats/serialization/converters.py` & `fileformats-0.6.2/fileformats/serialization/converters.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.1/fileformats/serialization/tests/test_serialization_converters.py` & `fileformats-0.6.2/fileformats/serialization/tests/test_serialization_converters.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.1/fileformats/text/__init__.py` & `fileformats-0.6.2/fileformats/text/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.1/LICENSE` & `fileformats-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.1/README.rst` & `fileformats-0.6.2/README.rst`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.1/pyproject.toml` & `fileformats-0.6.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.1/PKG-INFO` & `fileformats-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fileformats
-Version: 0.6.1
+Version: 0.6.2
 Summary: Classes for representing different file formats in Python classes for use in type hinting in data workflows
 Project-URL: repository, https://github.com/ArcanaFramework/fileformats
 Author-email: "Thomas G. Close" <tom.g.close@gmail.com>
 Maintainer-email: "Thomas G. Close" <tom.g.close@gmail.com>
 License: Creative Commons Attribution 4.0 International Public License
         By exercising the Licensed Rights (defined below), You accept and agree to be bound by the terms and conditions of this Creative Commons Attribution 4.0 International Public License ("Public License"). To the extent this Public License may be interpreted as a contract, You are granted the Licensed Rights in consideration of Your acceptance of these terms and conditions, and the Licensor grants You such rights in consideration of benefits the Licensor receives from making the Licensed Material available under these terms and conditions.
```

