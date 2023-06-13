# Comparing `tmp/dbis-relational-model-0.0.8.tar.gz` & `tmp/dbis-relational-model-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbis-relational-model-0.0.8.tar", last modified: Wed May  4 11:54:53 2022, max compression
+gzip compressed data, was "dbis-relational-model-0.0.9.tar", last modified: Wed May 11 09:14:38 2022, max compression
```

## Comparing `dbis-relational-model-0.0.8.tar` & `dbis-relational-model-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 philipph  (1000) philipph  (1000)        0 2022-05-04 11:54:53.389253 dbis-relational-model-0.0.8/
--rw-r--r--   0 philipph  (1000) philipph  (1000)    11357 2022-04-25 13:46:59.000000 dbis-relational-model-0.0.8/LICENSE
--rw-r--r--   0 philipph  (1000) philipph  (1000)      753 2022-05-04 11:54:53.385919 dbis-relational-model-0.0.8/PKG-INFO
--rw-r--r--   0 philipph  (1000) philipph  (1000)      161 2022-04-25 14:25:35.000000 dbis-relational-model-0.0.8/README.md
-drwxr-xr-x   0 philipph  (1000) philipph  (1000)        0 2022-05-04 11:54:53.385919 dbis-relational-model-0.0.8/dbis_relational_model.egg-info/
--rw-r--r--   0 philipph  (1000) philipph  (1000)      753 2022-05-04 11:54:53.000000 dbis-relational-model-0.0.8/dbis_relational_model.egg-info/PKG-INFO
--rw-r--r--   0 philipph  (1000) philipph  (1000)      272 2022-05-04 11:54:53.000000 dbis-relational-model-0.0.8/dbis_relational_model.egg-info/SOURCES.txt
--rw-r--r--   0 philipph  (1000) philipph  (1000)        1 2022-05-04 11:54:53.000000 dbis-relational-model-0.0.8/dbis_relational_model.egg-info/dependency_links.txt
--rw-r--r--   0 philipph  (1000) philipph  (1000)       17 2022-05-04 11:54:53.000000 dbis-relational-model-0.0.8/dbis_relational_model.egg-info/top_level.txt
-drwxr-xr-x   0 philipph  (1000) philipph  (1000)        0 2022-05-04 11:54:53.385919 dbis-relational-model-0.0.8/relational_model/
--rw-r--r--   0 philipph  (1000) philipph  (1000)        0 2022-04-25 13:46:59.000000 dbis-relational-model-0.0.8/relational_model/__init__.py
--rw-r--r--   0 philipph  (1000) philipph  (1000)    10862 2022-05-04 11:42:06.000000 dbis-relational-model-0.0.8/relational_model/relational_model.py
--rw-r--r--   0 philipph  (1000) philipph  (1000)       38 2022-05-04 11:54:53.389253 dbis-relational-model-0.0.8/setup.cfg
--rw-r--r--   0 philipph  (1000) philipph  (1000)     1086 2022-05-04 11:53:43.000000 dbis-relational-model-0.0.8/setup.py
+drwxr-xr-x   0 philipph  (1000) philipph  (1000)        0 2022-05-11 09:14:38.844212 dbis-relational-model-0.0.9/
+-rw-r--r--   0 philipph  (1000) philipph  (1000)    11357 2022-04-25 13:46:59.000000 dbis-relational-model-0.0.9/LICENSE
+-rw-r--r--   0 philipph  (1000) philipph  (1000)      753 2022-05-11 09:14:38.844212 dbis-relational-model-0.0.9/PKG-INFO
+-rw-r--r--   0 philipph  (1000) philipph  (1000)      161 2022-04-25 14:25:35.000000 dbis-relational-model-0.0.9/README.md
+drwxr-xr-x   0 philipph  (1000) philipph  (1000)        0 2022-05-11 09:14:38.844212 dbis-relational-model-0.0.9/dbis_relational_model.egg-info/
+-rw-r--r--   0 philipph  (1000) philipph  (1000)      753 2022-05-11 09:14:38.000000 dbis-relational-model-0.0.9/dbis_relational_model.egg-info/PKG-INFO
+-rw-r--r--   0 philipph  (1000) philipph  (1000)      272 2022-05-11 09:14:38.000000 dbis-relational-model-0.0.9/dbis_relational_model.egg-info/SOURCES.txt
+-rw-r--r--   0 philipph  (1000) philipph  (1000)        1 2022-05-11 09:14:38.000000 dbis-relational-model-0.0.9/dbis_relational_model.egg-info/dependency_links.txt
+-rw-r--r--   0 philipph  (1000) philipph  (1000)       17 2022-05-11 09:14:38.000000 dbis-relational-model-0.0.9/dbis_relational_model.egg-info/top_level.txt
+drwxr-xr-x   0 philipph  (1000) philipph  (1000)        0 2022-05-11 09:14:38.844212 dbis-relational-model-0.0.9/relational_model/
+-rw-r--r--   0 philipph  (1000) philipph  (1000)        0 2022-04-25 13:46:59.000000 dbis-relational-model-0.0.9/relational_model/__init__.py
+-rw-r--r--   0 philipph  (1000) philipph  (1000)    10831 2022-05-11 09:12:29.000000 dbis-relational-model-0.0.9/relational_model/relational_model.py
+-rw-r--r--   0 philipph  (1000) philipph  (1000)       38 2022-05-11 09:14:38.844212 dbis-relational-model-0.0.9/setup.cfg
+-rw-r--r--   0 philipph  (1000) philipph  (1000)     1086 2022-05-11 09:12:54.000000 dbis-relational-model-0.0.9/setup.py
```

### Comparing `dbis-relational-model-0.0.8/LICENSE` & `dbis-relational-model-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dbis-relational-model-0.0.8/PKG-INFO` & `dbis-relational-model-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbis-relational-model
-Version: 0.0.8
+Version: 0.0.9
 Summary: RWTH Aachen Computer Science i5/dbis assets for Lecture Datenbanken und Informationssysteme
 Home-page: https://github.com/rwth-acis/dbis-relational-model.git
 Author: Philipp Hochmann
 Author-email: hochmann@dbis.rwth-aachen.de
 License: Apache
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

### Comparing `dbis-relational-model-0.0.8/dbis_relational_model.egg-info/PKG-INFO` & `dbis-relational-model-0.0.9/dbis_relational_model.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbis-relational-model
-Version: 0.0.8
+Version: 0.0.9
 Summary: RWTH Aachen Computer Science i5/dbis assets for Lecture Datenbanken und Informationssysteme
 Home-page: https://github.com/rwth-acis/dbis-relational-model.git
 Author: Philipp Hochmann
 Author-email: hochmann@dbis.rwth-aachen.de
 License: Apache
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

### Comparing `dbis-relational-model-0.0.8/relational_model/relational_model.py` & `dbis-relational-model-0.0.9/relational_model/relational_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,16 +73,15 @@
         if (len(self.relations) + len(self.subsets) + len(self.intersections) == 0):
             display(Markdown("(empty Relation)"))
 
 
     def get_scaled_score(self, rm, scores, max_points, debug=False):
         worst_score = self.compare_against(RM(), scores, False)
         score = self.compare_against(rm, scores, debug)
-        penalty = (score / worst_score) * max_points
-        penalty = math.floor(penalty)
+        penalty = round((score / worst_score) * max_points)
         result = max(0, max_points - penalty)
         print(f"Scale deducted points to exercise's total points: {penalty}")
         print(f"Result: {result} / {max_points} points achieved")
         return result
 
     def compare_against(self, rm, scores, debug=False):
         score = 0
```

### Comparing `dbis-relational-model-0.0.8/setup.py` & `dbis-relational-model-0.0.9/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pathlib
 from setuptools import setup
 
 class Version(object):
     name="relational_model"
     description="RWTH Aachen Computer Science i5/dbis assets for Lecture Datenbanken und Informationssysteme"
-    version='0.0.8'
+    version='0.0.9'
 
 # The directory containing this file
 HERE = pathlib.Path(__file__).parent.resolve()
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
```

