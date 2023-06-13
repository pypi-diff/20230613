# Comparing `tmp/politikontroller_py-1.1.0.tar.gz` & `tmp/politikontroller_py-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "politikontroller_py-1.1.0.tar", max compression
+gzip compressed data, was "politikontroller_py-1.2.0.tar", max compression
```

## Comparing `politikontroller_py-1.1.0.tar` & `politikontroller_py-1.2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1070 2023-06-11 23:05:05.810836 politikontroller_py-1.1.0/LICENSE
--rw-r--r--   0        0        0     1018 2023-06-13 00:09:17.352013 politikontroller_py-1.1.0/README.md
--rw-r--r--   0        0        0       78 2023-06-11 23:05:05.814836 politikontroller_py-1.1.0/politikontroller_py/__init__.py
--rw-r--r--   0        0        0     2382 2023-06-11 23:05:05.814836 politikontroller_py-1.1.0/politikontroller_py/cli.py
--rw-r--r--   0        0        0     5265 2023-06-13 00:04:29.550179 politikontroller_py-1.1.0/politikontroller_py/client.py
--rw-r--r--   0        0        0      441 2023-06-12 23:56:29.371118 politikontroller_py-1.1.0/politikontroller_py/constants.py
--rw-r--r--   0        0        0       96 2023-06-11 23:05:05.810836 politikontroller_py-1.1.0/politikontroller_py/exceptions.py
--rw-r--r--   0        0        0     3390 2023-06-13 00:07:44.003418 politikontroller_py-1.1.0/politikontroller_py/models.py
--rw-r--r--   0        0        0     4097 2023-06-11 23:05:05.814836 politikontroller_py-1.1.0/politikontroller_py/utils.py
--rw-r--r--   0        0        0      679 2023-06-13 00:11:32.376874 politikontroller_py-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     1765 1970-01-01 00:00:00.000000 politikontroller_py-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-11 23:05:05.810836 politikontroller_py-1.2.0/LICENSE
+-rw-r--r--   0        0        0     1018 2023-06-13 00:09:17.352013 politikontroller_py-1.2.0/README.md
+-rw-r--r--   0        0        0       78 2023-06-11 23:05:05.814836 politikontroller_py-1.2.0/politikontroller_py/__init__.py
+-rw-r--r--   0        0        0     2382 2023-06-11 23:05:05.814836 politikontroller_py-1.2.0/politikontroller_py/cli.py
+-rw-r--r--   0        0        0     5265 2023-06-13 00:04:29.550179 politikontroller_py-1.2.0/politikontroller_py/client.py
+-rw-r--r--   0        0        0      441 2023-06-12 23:56:29.371118 politikontroller_py-1.2.0/politikontroller_py/constants.py
+-rw-r--r--   0        0        0       96 2023-06-11 23:05:05.810836 politikontroller_py-1.2.0/politikontroller_py/exceptions.py
+-rw-r--r--   0        0        0     3508 2023-06-13 00:58:46.405264 politikontroller_py-1.2.0/politikontroller_py/models.py
+-rw-r--r--   0        0        0     4097 2023-06-11 23:05:05.814836 politikontroller_py-1.2.0/politikontroller_py/utils.py
+-rw-r--r--   0        0        0      679 2023-06-13 01:00:03.385889 politikontroller_py-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1765 1970-01-01 00:00:00.000000 politikontroller_py-1.2.0/PKG-INFO
```

### Comparing `politikontroller_py-1.1.0/LICENSE` & `politikontroller_py-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `politikontroller_py-1.1.0/README.md` & `politikontroller_py-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `politikontroller_py-1.1.0/politikontroller_py/cli.py` & `politikontroller_py-1.2.0/politikontroller_py/cli.py`

 * *Files identical despite different names*

### Comparing `politikontroller_py-1.1.0/politikontroller_py/client.py` & `politikontroller_py-1.2.0/politikontroller_py/client.py`

 * *Files identical despite different names*

### Comparing `politikontroller_py-1.1.0/politikontroller_py/models.py` & `politikontroller_py-1.2.0/politikontroller_py/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,26 +65,31 @@
 class PoliceControlType(BaseModel):
     id: int
     name: PoliceControlTypeEnum
     slug: str
 
 
 class PoliceControlPoint:
+    type: str = "Point"
     lat: float
     lng: float
 
     def __init__(self, lat, lng):
         self.lat = lat
         self.lng = lng
 
     @property
+    def coordinates(self):
+        return (self.lat, self.lng)
+
+    @property
     def __geo_interface__(self):
         return {
-            'type': 'Point',
-            'coordinates': (self.lat, self.lng),
+            'type': self.type,
+            'coordinates': self.coordinates,
         }
 
 
 class PoliceControl(BaseModel):
     id: int
     type: PoliceControlTypeEnum
     county: str
@@ -123,15 +128,15 @@
     def _geometry(self):
         return PoliceControlPoint(self.lat, self.lng)
 
     @property
     def __geo_interface__(self):
         return {
             "type": "Feature",
-            "geometry": self._geometry,
+            "geometry": self._geometry.__geo_interface__,
             "properties": {
                 "title": self.title,
                 "description": self.description,
                 "type": self.type,
             },
         }
```

### Comparing `politikontroller_py-1.1.0/politikontroller_py/utils.py` & `politikontroller_py-1.2.0/politikontroller_py/utils.py`

 * *Files identical despite different names*

### Comparing `politikontroller_py-1.1.0/pyproject.toml` & `politikontroller_py-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "politikontroller-py"
-version = "1.1.0"
+version = "1.2.0"
 description = "Unofficial client for politikontroller.no"
 authors = ["Bendik R. Brenne <bendik@konstant.no>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "politikontroller_py" },
 ]
```

### Comparing `politikontroller_py-1.1.0/PKG-INFO` & `politikontroller_py-1.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: politikontroller-py
-Version: 1.1.0
+Version: 1.2.0
 Summary: Unofficial client for politikontroller.no
 License: MIT
 Author: Bendik R. Brenne
 Author-email: bendik@konstant.no
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

