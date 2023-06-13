# Comparing `tmp/mongo_to_s3-0.0.1.tar.gz` & `tmp/mongo_to_s3-0.0.2.tar.gz`

## Comparing `mongo_to_s3-0.0.1.tar` & `mongo_to_s3-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mongo_to_s3-0.0.1/src/mongo-to-s3/__init__.py
--rw-r--r--   0        0        0     5884 2020-02-02 00:00:00.000000 mongo_to_s3-0.0.1/src/mongo-to-s3/mongo-to-s3.py
--rw-r--r--   0        0        0     3253 2020-02-02 00:00:00.000000 mongo_to_s3-0.0.1/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 mongo_to_s3-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 mongo_to_s3-0.0.1/README.md
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 mongo_to_s3-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     4071 2020-02-02 00:00:00.000000 mongo_to_s3-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mongo_to_s3-0.0.2/src/mongo-to-s3/__init__.py
+-rw-r--r--   0        0        0     5884 2020-02-02 00:00:00.000000 mongo_to_s3-0.0.2/src/mongo-to-s3/mongo-to-s3.py
+-rw-r--r--   0        0        0     3253 2020-02-02 00:00:00.000000 mongo_to_s3-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 mongo_to_s3-0.0.2/LICENSE.txt
+-rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 mongo_to_s3-0.0.2/README.md
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 mongo_to_s3-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4071 2020-02-02 00:00:00.000000 mongo_to_s3-0.0.2/PKG-INFO
```

### Comparing `mongo_to_s3-0.0.1/src/mongo-to-s3/mongo-to-s3.py` & `mongo_to_s3-0.0.2/src/mongo-to-s3/mongo-to-s3.py`

 * *Files identical despite different names*

### Comparing `mongo_to_s3-0.0.1/.gitignore` & `mongo_to_s3-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `mongo_to_s3-0.0.1/LICENSE.txt` & `mongo_to_s3-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mongo_to_s3-0.0.1/README.md` & `mongo_to_s3-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `mongo_to_s3-0.0.1/PKG-INFO` & `mongo_to_s3-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongo-to-s3
-Version: 0.0.1
+Version: 0.0.2
 Summary: Automated script generator to backup MongoDB databases to Amazon S3.
 Project-URL: Homepage, https://github.com/IamLizu/mongo-to-s3
 Project-URL: Bug Tracker, https://github.com/IamLizu/mongo-to-s3/issues
 Author-email: S M Mahmudul Hasan <thegeek@iamlizu.com>
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

