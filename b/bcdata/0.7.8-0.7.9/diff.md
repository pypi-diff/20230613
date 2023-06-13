# Comparing `tmp/bcdata-0.7.8.tar.gz` & `tmp/bcdata-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bcdata-0.7.8.tar", last modified: Fri Jun  2 00:01:56 2023, max compression
+gzip compressed data, was "bcdata-0.7.9.tar", last modified: Tue Jun 13 20:15:14 2023, max compression
```

## Comparing `bcdata-0.7.8.tar` & `bcdata-0.7.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 snorris    (501) staff       (20)        0 2023-06-02 00:01:56.715017 bcdata-0.7.8/
--rw-r--r--   0 snorris    (501) staff       (20)     6388 2023-06-02 00:00:04.000000 bcdata-0.7.8/CHANGES.txt
--rw-r--r--   0 snorris    (501) staff       (20)     1080 2018-01-17 01:59:21.000000 bcdata-0.7.8/LICENSE.txt
--rw-r--r--   0 snorris    (501) staff       (20)    16453 2023-06-02 00:01:56.714888 bcdata-0.7.8/PKG-INFO
--rw-r--r--   0 snorris    (501) staff       (20)    15633 2023-06-02 00:00:04.000000 bcdata-0.7.8/README.md
-drwxr-xr-x   0 snorris    (501) staff       (20)        0 2023-06-02 00:01:56.712977 bcdata-0.7.8/bcdata/
--rw-r--r--   0 snorris    (501) staff       (20)      349 2023-06-02 00:00:04.000000 bcdata-0.7.8/bcdata/__init__.py
--rw-r--r--   0 snorris    (501) staff       (20)     5267 2022-09-26 21:48:59.000000 bcdata-0.7.8/bcdata/bc2pg.py
--rw-r--r--   0 snorris    (501) staff       (20)     3876 2022-11-18 22:34:58.000000 bcdata-0.7.8/bcdata/bcdc.py
--rw-r--r--   0 snorris    (501) staff       (20)     9795 2023-04-13 19:53:56.000000 bcdata-0.7.8/bcdata/cli.py
--rw-r--r--   0 snorris    (501) staff       (20)     6342 2022-09-29 00:22:24.000000 bcdata-0.7.8/bcdata/database.py
--rw-r--r--   0 snorris    (501) staff       (20)     3034 2022-11-18 22:34:58.000000 bcdata-0.7.8/bcdata/wcs.py
--rw-r--r--   0 snorris    (501) staff       (20)    11387 2023-04-13 19:53:56.000000 bcdata-0.7.8/bcdata/wfs.py
-drwxr-xr-x   0 snorris    (501) staff       (20)        0 2023-06-02 00:01:56.713909 bcdata-0.7.8/bcdata.egg-info/
--rw-r--r--   0 snorris    (501) staff       (20)    16453 2023-06-02 00:01:56.000000 bcdata-0.7.8/bcdata.egg-info/PKG-INFO
--rw-r--r--   0 snorris    (501) staff       (20)      474 2023-06-02 00:01:56.000000 bcdata-0.7.8/bcdata.egg-info/SOURCES.txt
--rw-r--r--   0 snorris    (501) staff       (20)        1 2023-06-02 00:01:56.000000 bcdata-0.7.8/bcdata.egg-info/dependency_links.txt
--rw-r--r--   0 snorris    (501) staff       (20)       42 2023-06-02 00:01:56.000000 bcdata-0.7.8/bcdata.egg-info/entry_points.txt
--rw-r--r--   0 snorris    (501) staff       (20)        1 2019-11-08 06:25:25.000000 bcdata-0.7.8/bcdata.egg-info/not-zip-safe
--rw-r--r--   0 snorris    (501) staff       (20)      121 2023-06-02 00:01:56.000000 bcdata-0.7.8/bcdata.egg-info/requires.txt
--rw-r--r--   0 snorris    (501) staff       (20)        7 2023-06-02 00:01:56.000000 bcdata-0.7.8/bcdata.egg-info/top_level.txt
--rw-r--r--   0 snorris    (501) staff       (20)      173 2022-07-16 00:28:03.000000 bcdata-0.7.8/pyproject.toml
--rw-r--r--   0 snorris    (501) staff       (20)      102 2023-05-29 23:57:06.000000 bcdata-0.7.8/requirements.txt
--rw-r--r--   0 snorris    (501) staff       (20)       38 2023-06-02 00:01:56.715048 bcdata-0.7.8/setup.cfg
--rw-r--r--   0 snorris    (501) staff       (20)     1732 2022-07-20 16:54:44.000000 bcdata-0.7.8/setup.py
-drwxr-xr-x   0 snorris    (501) staff       (20)        0 2023-06-02 00:01:56.714644 bcdata-0.7.8/tests/
--rw-r--r--   0 snorris    (501) staff       (20)     3851 2022-11-18 21:53:34.000000 bcdata-0.7.8/tests/test_bc2pg.py
--rw-r--r--   0 snorris    (501) staff       (20)     6049 2023-04-13 19:53:56.000000 bcdata-0.7.8/tests/test_bcdata.py
--rw-r--r--   0 snorris    (501) staff       (20)    11548 2022-07-20 16:54:44.000000 bcdata-0.7.8/tests/test_bcdc.py
--rw-r--r--   0 snorris    (501) staff       (20)     2393 2022-07-20 16:54:44.000000 bcdata-0.7.8/tests/test_cli.py
+drwxr-xr-x   0 snorris    (501) staff       (20)        0 2023-06-13 20:15:14.292203 bcdata-0.7.9/
+-rw-r--r--   0 snorris    (501) staff       (20)     6511 2023-06-13 20:13:50.000000 bcdata-0.7.9/CHANGES.txt
+-rw-r--r--   0 snorris    (501) staff       (20)     1080 2018-01-17 01:59:21.000000 bcdata-0.7.9/LICENSE.txt
+-rw-r--r--   0 snorris    (501) staff       (20)    16453 2023-06-13 20:15:14.292054 bcdata-0.7.9/PKG-INFO
+-rw-r--r--   0 snorris    (501) staff       (20)    15633 2023-06-02 00:00:04.000000 bcdata-0.7.9/README.md
+drwxr-xr-x   0 snorris    (501) staff       (20)        0 2023-06-13 20:15:14.290510 bcdata-0.7.9/bcdata/
+-rw-r--r--   0 snorris    (501) staff       (20)      349 2023-06-13 20:13:50.000000 bcdata-0.7.9/bcdata/__init__.py
+-rw-r--r--   0 snorris    (501) staff       (20)     5267 2022-09-26 21:48:59.000000 bcdata-0.7.9/bcdata/bc2pg.py
+-rw-r--r--   0 snorris    (501) staff       (20)     3876 2022-11-18 22:34:58.000000 bcdata-0.7.9/bcdata/bcdc.py
+-rw-r--r--   0 snorris    (501) staff       (20)     9795 2023-04-13 19:53:56.000000 bcdata-0.7.9/bcdata/cli.py
+-rw-r--r--   0 snorris    (501) staff       (20)     6342 2022-09-29 00:22:24.000000 bcdata-0.7.9/bcdata/database.py
+-rw-r--r--   0 snorris    (501) staff       (20)     3034 2022-11-18 22:34:58.000000 bcdata-0.7.9/bcdata/wcs.py
+-rw-r--r--   0 snorris    (501) staff       (20)    11297 2023-06-13 20:13:50.000000 bcdata-0.7.9/bcdata/wfs.py
+drwxr-xr-x   0 snorris    (501) staff       (20)        0 2023-06-13 20:15:14.291456 bcdata-0.7.9/bcdata.egg-info/
+-rw-r--r--   0 snorris    (501) staff       (20)    16453 2023-06-13 20:15:14.000000 bcdata-0.7.9/bcdata.egg-info/PKG-INFO
+-rw-r--r--   0 snorris    (501) staff       (20)      474 2023-06-13 20:15:14.000000 bcdata-0.7.9/bcdata.egg-info/SOURCES.txt
+-rw-r--r--   0 snorris    (501) staff       (20)        1 2023-06-13 20:15:14.000000 bcdata-0.7.9/bcdata.egg-info/dependency_links.txt
+-rw-r--r--   0 snorris    (501) staff       (20)       42 2023-06-13 20:15:14.000000 bcdata-0.7.9/bcdata.egg-info/entry_points.txt
+-rw-r--r--   0 snorris    (501) staff       (20)        1 2019-11-08 06:25:25.000000 bcdata-0.7.9/bcdata.egg-info/not-zip-safe
+-rw-r--r--   0 snorris    (501) staff       (20)      124 2023-06-13 20:15:14.000000 bcdata-0.7.9/bcdata.egg-info/requires.txt
+-rw-r--r--   0 snorris    (501) staff       (20)        7 2023-06-13 20:15:14.000000 bcdata-0.7.9/bcdata.egg-info/top_level.txt
+-rw-r--r--   0 snorris    (501) staff       (20)      173 2022-07-16 00:28:03.000000 bcdata-0.7.9/pyproject.toml
+-rw-r--r--   0 snorris    (501) staff       (20)      105 2023-06-13 20:13:50.000000 bcdata-0.7.9/requirements.txt
+-rw-r--r--   0 snorris    (501) staff       (20)       38 2023-06-13 20:15:14.292240 bcdata-0.7.9/setup.cfg
+-rw-r--r--   0 snorris    (501) staff       (20)     1732 2022-07-20 16:54:44.000000 bcdata-0.7.9/setup.py
+drwxr-xr-x   0 snorris    (501) staff       (20)        0 2023-06-13 20:15:14.291879 bcdata-0.7.9/tests/
+-rw-r--r--   0 snorris    (501) staff       (20)     3851 2022-11-18 21:53:34.000000 bcdata-0.7.9/tests/test_bc2pg.py
+-rw-r--r--   0 snorris    (501) staff       (20)     6049 2023-04-13 19:53:56.000000 bcdata-0.7.9/tests/test_bcdata.py
+-rw-r--r--   0 snorris    (501) staff       (20)    11548 2022-07-20 16:54:44.000000 bcdata-0.7.9/tests/test_bcdc.py
+-rw-r--r--   0 snorris    (501) staff       (20)     2393 2022-07-20 16:54:44.000000 bcdata-0.7.9/tests/test_cli.py
```

### Comparing `bcdata-0.7.8/CHANGES.txt` & `bcdata-0.7.9/CHANGES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 Changes
 =======
 
-0.7.8 ()
+0.7.9 (2023-06-13)
+------------------
+- fix geometry type checking (#131)
+- update geopandas requirement (#129)
+
+0.7.8 (2023-06-01)
 ------------------
 - pin geopandas requirement to <v0.13 (#129)
 
 0.7.7 (2023-04-13)
 ------------------
 - add option to lowercasify properties keys / column names (#126)
```

### Comparing `bcdata-0.7.8/LICENSE.txt` & `bcdata-0.7.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bcdata-0.7.8/PKG-INFO` & `bcdata-0.7.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bcdata
-Version: 0.7.8
+Version: 0.7.9
 Summary: Python tools for quick access to DataBC geo-data available via WFS
 Home-page: https://github.com/smnorris/bcdata
 Author: Simon Norris
 Author-email: snorris@hillcrestgeo.ca
 License: Apache
 Keywords: gis geospatial data BC DataBC download "Britsh Columbia"
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `bcdata-0.7.8/README.md` & `bcdata-0.7.9/README.md`

 * *Files identical despite different names*

### Comparing `bcdata-0.7.8/bcdata/bc2pg.py` & `bcdata-0.7.9/bcdata/bc2pg.py`

 * *Files identical despite different names*

### Comparing `bcdata-0.7.8/bcdata/bcdc.py` & `bcdata-0.7.9/bcdata/bcdc.py`

 * *Files identical despite different names*

### Comparing `bcdata-0.7.8/bcdata/cli.py` & `bcdata-0.7.9/bcdata/cli.py`

 * *Files identical despite different names*

### Comparing `bcdata-0.7.8/bcdata/database.py` & `bcdata-0.7.9/bcdata/database.py`

 * *Files identical despite different names*

### Comparing `bcdata-0.7.8/bcdata/wcs.py` & `bcdata-0.7.9/bcdata/wcs.py`

 * *Files identical despite different names*

### Comparing `bcdata-0.7.8/bcdata/wfs.py` & `bcdata-0.7.9/bcdata/wfs.py`

 * *Files 3% similar despite different names*

```diff
@@ -296,51 +296,46 @@
 
 
 def get_types(dataset, count=10):
     """Return distinct types within the first n features"""
     # validate the table name
     table = validate_name(dataset)
     log.info("Getting feature geometry type")
-    # get features and find distinct types where geom is not empty
-    features = [f for f in get_features(table, count=count)]
-    geom_types = list(
-        set([f["geometry"]["type"].upper() for f in features if f["geometry"]])
-    )
+    # get first n features, examine the feature geometry type (where geometry is not empty)
+    geom_types = []
+    for f in get_features(table, count=count):
+        if f["geometry"]:
+            geom_type = f["geometry"]["type"].upper()
+            # only these geometry types are expected/supported
+            if geom_type not in (
+                "POINT",
+                "LINESTRING",
+                "POLYGON",
+                "MULTIPOINT",
+                "MULTILINESTRING",
+                "MULTIPOLYGON",
+            ):
+                raise ValueError("Geometry type {geomtype} is not supported")
+            # look for z dimension, modify type if found
+            if (
+                (geom_type == "POINT" and len(f["geometry"]["coordinates"]) == 3)
+                or (
+                    geom_type == "MULTIPOINT"
+                    and len(f["geometry"]["coordinates"][0]) == 3
+                )
+                or (
+                    geom_type == "LINESTRING"
+                    and len(f["geometry"]["coordinates"][0]) == 3
+                )
+                or (
+                    geom_type == "MULTILINESTRING"
+                    and len(f["geometry"]["coordinates"][0][0]) == 3
+                )
+            ):
+                geom_type = geom_type + "Z"
+            geom_types.append(geom_type)
+    geom_types = list(set(geom_types))
+    # issue warning if types are mixed
     if len(geom_types) > 1:
         typestring = ",".join(geom_types)
         log.warning(f"Dataset {dataset} has multiple geometry types: {typestring}")
-    # validate the type (shouldn't be necessary)
-    for geom_type in geom_types:
-        if geom_type not in (
-            "POINT",
-            "LINESTRING",
-            "POLYGON",
-            "MULTIPOINT",
-            "MULTILINESTRING",
-            "MULTIPOLYGON",
-        ):
-            raise ValueError("Geometry type {geomtype} is not supported")
-    # if Z coordinates are supplied, modify the type accordingly
-    # (presuming that all )
-    # (points and lines only, presumably there are no 3d polygon features)
-    for i in range(len(geom_types)):
-        if (
-            geom_types[i] == "POINT"
-            and len(features[0]["geometry"]["coordinates"]) == 3
-        ):
-            geom_types[i] = "POINTZ"
-        if (
-            geom_types[i] == "MULTIPOINT"
-            and len(features[0]["geometry"]["coordinates"][0]) == 3
-        ):
-            geom_types[i] = "POINTZ"
-        if (
-            geom_types[i] == "LINESTRING"
-            and len(features[0]["geometry"]["coordinates"][0]) == 3
-        ):
-            geom_types[i] = "LINESTRINGZ"
-        if (
-            geom_types[i] == "MULTILINESTRING"
-            and len(features[0]["geometry"]["coordinates"][0][0]) == 3
-        ):
-            geom_types[i] = "MULTILINESTRINGZ"
     return geom_types
```

### Comparing `bcdata-0.7.8/bcdata.egg-info/PKG-INFO` & `bcdata-0.7.9/bcdata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bcdata
-Version: 0.7.8
+Version: 0.7.9
 Summary: Python tools for quick access to DataBC geo-data available via WFS
 Home-page: https://github.com/smnorris/bcdata
 Author: Simon Norris
 Author-email: snorris@hillcrestgeo.ca
 License: Apache
 Keywords: gis geospatial data BC DataBC download "Britsh Columbia"
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `bcdata-0.7.8/setup.py` & `bcdata-0.7.9/setup.py`

 * *Files identical despite different names*

### Comparing `bcdata-0.7.8/tests/test_bc2pg.py` & `bcdata-0.7.9/tests/test_bc2pg.py`

 * *Files identical despite different names*

### Comparing `bcdata-0.7.8/tests/test_bcdata.py` & `bcdata-0.7.9/tests/test_bcdata.py`

 * *Files identical despite different names*

### Comparing `bcdata-0.7.8/tests/test_bcdc.py` & `bcdata-0.7.9/tests/test_bcdc.py`

 * *Files identical despite different names*

### Comparing `bcdata-0.7.8/tests/test_cli.py` & `bcdata-0.7.9/tests/test_cli.py`

 * *Files identical despite different names*

