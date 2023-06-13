# Comparing `tmp/pylicensing-0.0.2.tar.gz` & `tmp/pylicensing-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylicensing-0.0.2.tar", last modified: Tue Jun 13 20:38:58 2023, max compression
+gzip compressed data, was "pylicensing-0.0.3.tar", last modified: Tue Jun 13 20:48:16 2023, max compression
```

## Comparing `pylicensing-0.0.2.tar` & `pylicensing-0.0.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 20:38:58.541088 pylicensing-0.0.2/
--rw-rw-rw-   0        0        0     1083 2023-03-06 20:13:43.000000 pylicensing-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     2714 2023-06-13 20:38:58.541088 pylicensing-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2177 2023-03-11 06:33:33.000000 pylicensing-0.0.2/README.md
--rw-rw-rw-   0        0        0      617 2023-06-13 20:38:20.000000 pylicensing-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0      335 2023-06-13 20:38:58.545592 pylicensing-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0       63 2023-02-02 18:28:58.000000 pylicensing-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-13 20:38:58.503056 pylicensing-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-06-13 20:38:58.517068 pylicensing-0.0.2/src/pylicensing/
--rw-rw-rw-   0        0        0       91 2023-05-03 14:43:54.000000 pylicensing-0.0.2/src/pylicensing/__init__.py
--rw-rw-rw-   0        0        0     4239 2023-05-13 12:42:02.000000 pylicensing-0.0.2/src/pylicensing/database.py
--rw-rw-rw-   0        0        0     1549 2023-03-10 22:50:24.000000 pylicensing-0.0.2/src/pylicensing/exceptions.py
--rw-rw-rw-   0        0        0     1541 2023-05-14 14:55:02.000000 pylicensing-0.0.2/src/pylicensing/hwid_tools.py
-drwxrwxrwx   0        0        0        0 2023-06-13 20:38:58.536585 pylicensing-0.0.2/src/pylicensing/key/
--rw-rw-rw-   0        0        0       51 2023-05-11 19:29:20.000000 pylicensing-0.0.2/src/pylicensing/key/__init__.py
--rw-rw-rw-   0        0        0     2736 2023-03-09 20:14:13.000000 pylicensing-0.0.2/src/pylicensing/key/_generate.py
--rw-rw-rw-   0        0        0     1933 2023-03-10 00:40:15.000000 pylicensing-0.0.2/src/pylicensing/key/format.py
--rw-rw-rw-   0        0        0     2413 2023-05-13 12:44:07.000000 pylicensing-0.0.2/src/pylicensing/key/key.py
--rw-rw-rw-   0        0        0     3679 2023-03-10 22:58:51.000000 pylicensing-0.0.2/src/pylicensing/validation.py
-drwxrwxrwx   0        0        0        0 2023-06-13 20:38:58.533081 pylicensing-0.0.2/src/pylicensing.egg-info/
--rw-rw-rw-   0        0        0     2714 2023-06-13 20:38:58.000000 pylicensing-0.0.2/src/pylicensing.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      652 2023-06-13 20:38:58.000000 pylicensing-0.0.2/src/pylicensing.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 20:38:58.000000 pylicensing-0.0.2/src/pylicensing.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-03-07 20:19:34.000000 pylicensing-0.0.2/src/pylicensing.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       35 2023-06-13 20:38:58.000000 pylicensing-0.0.2/src/pylicensing.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-13 20:38:58.000000 pylicensing-0.0.2/src/pylicensing.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-13 20:38:58.540088 pylicensing-0.0.2/tests/
--rw-rw-rw-   0        0        0     3027 2023-03-10 01:49:58.000000 pylicensing-0.0.2/tests/test_database.py
--rw-rw-rw-   0        0        0     1447 2023-03-10 18:51:18.000000 pylicensing-0.0.2/tests/test_format_validation.py
--rw-rw-rw-   0        0        0     1109 2023-03-10 18:51:39.000000 pylicensing-0.0.2/tests/test_hwid.py
--rw-rw-rw-   0        0        0     1281 2023-03-10 01:49:28.000000 pylicensing-0.0.2/tests/test_key_creation.py
+drwxrwxrwx   0        0        0        0 2023-06-13 20:48:16.651414 pylicensing-0.0.3/
+-rw-rw-rw-   0        0        0     1083 2023-03-06 20:13:43.000000 pylicensing-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     2714 2023-06-13 20:48:16.651915 pylicensing-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2177 2023-03-11 06:33:33.000000 pylicensing-0.0.3/README.md
+-rw-rw-rw-   0        0        0      617 2023-06-13 20:48:02.000000 pylicensing-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0      335 2023-06-13 20:48:16.656918 pylicensing-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0       63 2023-02-02 18:28:58.000000 pylicensing-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 20:48:16.615883 pylicensing-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-06-13 20:48:16.627393 pylicensing-0.0.3/src/pylicensing/
+-rw-rw-rw-   0        0        0       91 2023-05-03 14:43:54.000000 pylicensing-0.0.3/src/pylicensing/__init__.py
+-rw-rw-rw-   0        0        0     4239 2023-05-13 12:42:02.000000 pylicensing-0.0.3/src/pylicensing/database.py
+-rw-rw-rw-   0        0        0     1549 2023-03-10 22:50:24.000000 pylicensing-0.0.3/src/pylicensing/exceptions.py
+-rw-rw-rw-   0        0        0     1541 2023-05-14 14:55:02.000000 pylicensing-0.0.3/src/pylicensing/hwid_tools.py
+drwxrwxrwx   0        0        0        0 2023-06-13 20:48:16.646409 pylicensing-0.0.3/src/pylicensing/key/
+-rw-rw-rw-   0        0        0       51 2023-05-11 19:29:20.000000 pylicensing-0.0.3/src/pylicensing/key/__init__.py
+-rw-rw-rw-   0        0        0     2736 2023-03-09 20:14:13.000000 pylicensing-0.0.3/src/pylicensing/key/_generate.py
+-rw-rw-rw-   0        0        0     1933 2023-03-10 00:40:15.000000 pylicensing-0.0.3/src/pylicensing/key/format.py
+-rw-rw-rw-   0        0        0     2521 2023-06-13 20:47:07.000000 pylicensing-0.0.3/src/pylicensing/key/key.py
+-rw-rw-rw-   0        0        0     3679 2023-03-10 22:58:51.000000 pylicensing-0.0.3/src/pylicensing/validation.py
+drwxrwxrwx   0        0        0        0 2023-06-13 20:48:16.641905 pylicensing-0.0.3/src/pylicensing.egg-info/
+-rw-rw-rw-   0        0        0     2714 2023-06-13 20:48:16.000000 pylicensing-0.0.3/src/pylicensing.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      652 2023-06-13 20:48:16.000000 pylicensing-0.0.3/src/pylicensing.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 20:48:16.000000 pylicensing-0.0.3/src/pylicensing.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-03-07 20:19:34.000000 pylicensing-0.0.3/src/pylicensing.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       35 2023-06-13 20:48:16.000000 pylicensing-0.0.3/src/pylicensing.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-13 20:48:16.000000 pylicensing-0.0.3/src/pylicensing.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-13 20:48:16.650913 pylicensing-0.0.3/tests/
+-rw-rw-rw-   0        0        0     3027 2023-03-10 01:49:58.000000 pylicensing-0.0.3/tests/test_database.py
+-rw-rw-rw-   0        0        0     1447 2023-03-10 18:51:18.000000 pylicensing-0.0.3/tests/test_format_validation.py
+-rw-rw-rw-   0        0        0     1109 2023-03-10 18:51:39.000000 pylicensing-0.0.3/tests/test_hwid.py
+-rw-rw-rw-   0        0        0     1281 2023-03-10 01:49:28.000000 pylicensing-0.0.3/tests/test_key_creation.py
```

### Comparing `pylicensing-0.0.2/LICENSE` & `pylicensing-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pylicensing-0.0.2/PKG-INFO` & `pylicensing-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylicensing
-Version: 0.0.2
+Version: 0.0.3
 Summary: Simple licensing helper using mongodb
 Author-email: Kenny Hommel <kennyhommel36@gmail.com>
 Project-URL: Homepage, https://github.com/kennyhml/pylicensing
 Project-URL: Bug Tracker, https://github.com/kennyhml/pylicensing/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pylicensing-0.0.2/README.md` & `pylicensing-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pylicensing-0.0.2/pyproject.toml` & `pylicensing-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pylicensing"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Kenny Hommel", email="kennyhommel36@gmail.com" },
 ]
 description = "Simple licensing helper using mongodb"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `pylicensing-0.0.2/src/pylicensing/database.py` & `pylicensing-0.0.3/src/pylicensing/database.py`

 * *Files identical despite different names*

### Comparing `pylicensing-0.0.2/src/pylicensing/exceptions.py` & `pylicensing-0.0.3/src/pylicensing/exceptions.py`

 * *Files identical despite different names*

### Comparing `pylicensing-0.0.2/src/pylicensing/hwid_tools.py` & `pylicensing-0.0.3/src/pylicensing/hwid_tools.py`

 * *Files identical despite different names*

### Comparing `pylicensing-0.0.2/src/pylicensing/key/_generate.py` & `pylicensing-0.0.3/src/pylicensing/key/_generate.py`

 * *Files identical despite different names*

### Comparing `pylicensing-0.0.2/src/pylicensing/key/format.py` & `pylicensing-0.0.3/src/pylicensing/key/format.py`

 * *Files identical despite different names*

### Comparing `pylicensing-0.0.2/src/pylicensing/key/key.py` & `pylicensing-0.0.3/src/pylicensing/key/key.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 from dataclasses import dataclass, field
 from datetime import datetime, timedelta
+from typing import Optional
 
 from bson.objectid import ObjectId
 
 from ._generate import generate_key
 from .format import KeyFormat
 
 
@@ -31,35 +32,38 @@
 
     key: str
     owner: str
     hwid_limit: int
     created: datetime
     valid_until: datetime
     hwids: list = field(default_factory=list)
+    ip: Optional[str] = None
     _id: ObjectId | None = None
 
     @classmethod
     def create(
         cls,
         format: KeyFormat,
         owner: str,
         hwid_limit: int,
         valid_for: timedelta,
+        ip: Optional[str] = None
     ) -> Key:
         """Returns a `Key` created from a `KeyFormat` and other details.\n
         The key will be randomly generated using said format during creation.
         """
         return cls(
             generate_key(format),
             owner,
             hwid_limit,
             created=datetime.now().replace(microsecond=0),
             valid_until=(datetime.now() + valid_for).replace(microsecond=0),
+            ip=ip
         )
-    
+
     @property
     def expired(self) -> bool:
         return datetime.now() >= self.valid_until
 
     def to_database_data(self) -> dict:
         """Turns a `Key` into the data that is valuable for the database.
```

### Comparing `pylicensing-0.0.2/src/pylicensing/validation.py` & `pylicensing-0.0.3/src/pylicensing/validation.py`

 * *Files identical despite different names*

### Comparing `pylicensing-0.0.2/src/pylicensing.egg-info/PKG-INFO` & `pylicensing-0.0.3/src/pylicensing.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylicensing
-Version: 0.0.2
+Version: 0.0.3
 Summary: Simple licensing helper using mongodb
 Author-email: Kenny Hommel <kennyhommel36@gmail.com>
 Project-URL: Homepage, https://github.com/kennyhml/pylicensing
 Project-URL: Bug Tracker, https://github.com/kennyhml/pylicensing/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pylicensing-0.0.2/src/pylicensing.egg-info/SOURCES.txt` & `pylicensing-0.0.3/src/pylicensing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pylicensing-0.0.2/tests/test_database.py` & `pylicensing-0.0.3/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `pylicensing-0.0.2/tests/test_format_validation.py` & `pylicensing-0.0.3/tests/test_format_validation.py`

 * *Files identical despite different names*

### Comparing `pylicensing-0.0.2/tests/test_hwid.py` & `pylicensing-0.0.3/tests/test_hwid.py`

 * *Files identical despite different names*

### Comparing `pylicensing-0.0.2/tests/test_key_creation.py` & `pylicensing-0.0.3/tests/test_key_creation.py`

 * *Files identical despite different names*

