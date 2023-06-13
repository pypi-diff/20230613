# Comparing `tmp/mongo_to_s3-0.0.4.tar.gz` & `tmp/mongo_to_s3-0.0.5.tar.gz`

## Comparing `mongo_to_s3-0.0.4.tar` & `mongo_to_s3-0.0.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mongo_to_s3-0.0.4/src/mongo-to-s3/__init__.py
--rw-r--r--   0        0        0     5884 2020-02-02 00:00:00.000000 mongo_to_s3-0.0.4/src/mongo-to-s3/mongo-to-s3.py
--rw-r--r--   0        0        0     3253 2020-02-02 00:00:00.000000 mongo_to_s3-0.0.4/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 mongo_to_s3-0.0.4/LICENSE.txt
--rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 mongo_to_s3-0.0.4/README.md
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 mongo_to_s3-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     4071 2020-02-02 00:00:00.000000 mongo_to_s3-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mongo_to_s3-0.0.5/src/mongo_to_s3/__init__.py
+-rw-r--r--   0        0        0     5884 2020-02-02 00:00:00.000000 mongo_to_s3-0.0.5/src/mongo_to_s3/mongo_to_s3.py
+-rw-r--r--   0        0        0     3253 2020-02-02 00:00:00.000000 mongo_to_s3-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 mongo_to_s3-0.0.5/LICENSE.txt
+-rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 mongo_to_s3-0.0.5/README.md
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 mongo_to_s3-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     4071 2020-02-02 00:00:00.000000 mongo_to_s3-0.0.5/PKG-INFO
```

### Comparing `mongo_to_s3-0.0.4/src/mongo-to-s3/mongo-to-s3.py` & `mongo_to_s3-0.0.5/src/mongo_to_s3/mongo_to_s3.py`

 * *Files identical despite different names*

### Comparing `mongo_to_s3-0.0.4/.gitignore` & `mongo_to_s3-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `mongo_to_s3-0.0.4/LICENSE.txt` & `mongo_to_s3-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mongo_to_s3-0.0.4/README.md` & `mongo_to_s3-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `mongo_to_s3-0.0.4/pyproject.toml` & `mongo_to_s3-0.0.5/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "mongo-to-s3"
-version = "0.0.4"
+version = "0.0.5"
 dependencies = [
     "boto3",
 ]
 authors = [
   { name="S M Mahmudul Hasan", email="thegeek@iamlizu.com" },
 ]
 description = "Automated script generator to backup MongoDB databases to Amazon S3."
@@ -22,8 +22,8 @@
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/IamLizu/mongo-to-s3"
 "Bug Tracker" = "https://github.com/IamLizu/mongo-to-s3/issues"
 
 [project.scripts]
-mongo-to-s3 = "mongo-to-s3.main:main"
+mongo-to-s3 = "mongo_to_s3.main:main"
```

### Comparing `mongo_to_s3-0.0.4/PKG-INFO` & `mongo_to_s3-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongo-to-s3
-Version: 0.0.4
+Version: 0.0.5
 Summary: Automated script generator to backup MongoDB databases to Amazon S3.
 Project-URL: Homepage, https://github.com/IamLizu/mongo-to-s3
 Project-URL: Bug Tracker, https://github.com/IamLizu/mongo-to-s3/issues
 Author-email: S M Mahmudul Hasan <thegeek@iamlizu.com>
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

