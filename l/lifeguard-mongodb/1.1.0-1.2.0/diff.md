# Comparing `tmp/lifeguard-mongodb-1.1.0.tar.gz` & `tmp/lifeguard-mongodb-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lifeguard-mongodb-1.1.0.tar", last modified: Fri May 26 15:18:12 2023, max compression
+gzip compressed data, was "lifeguard-mongodb-1.2.0.tar", last modified: Tue Jun 13 13:12:44 2023, max compression
```

## Comparing `lifeguard-mongodb-1.1.0.tar` & `lifeguard-mongodb-1.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:18:12.003502 lifeguard-mongodb-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-26 15:18:12.003502 lifeguard-mongodb-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-26 15:17:42.000000 lifeguard-mongodb-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:18:12.003502 lifeguard-mongodb-1.1.0/lifeguard_mongodb/
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-26 15:17:42.000000 lifeguard-mongodb-1.1.0/lifeguard_mongodb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-05-26 15:17:42.000000 lifeguard-mongodb-1.1.0/lifeguard_mongodb/repositories.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-26 15:17:42.000000 lifeguard-mongodb-1.1.0/lifeguard_mongodb/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:18:12.003502 lifeguard-mongodb-1.1.0/lifeguard_mongodb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-26 15:18:11.000000 lifeguard-mongodb-1.1.0/lifeguard_mongodb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-26 15:18:11.000000 lifeguard-mongodb-1.1.0/lifeguard_mongodb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 15:18:11.000000 lifeguard-mongodb-1.1.0/lifeguard_mongodb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-26 15:18:11.000000 lifeguard-mongodb-1.1.0/lifeguard_mongodb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-26 15:18:11.000000 lifeguard-mongodb-1.1.0/lifeguard_mongodb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 15:18:12.003502 lifeguard-mongodb-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-26 15:17:42.000000 lifeguard-mongodb-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:12:44.795171 lifeguard-mongodb-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-13 13:12:44.795171 lifeguard-mongodb-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-13 13:12:14.000000 lifeguard-mongodb-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:12:44.795171 lifeguard-mongodb-1.2.0/lifeguard_mongodb/
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-13 13:12:14.000000 lifeguard-mongodb-1.2.0/lifeguard_mongodb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-06-13 13:12:14.000000 lifeguard-mongodb-1.2.0/lifeguard_mongodb/repositories.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-13 13:12:14.000000 lifeguard-mongodb-1.2.0/lifeguard_mongodb/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:12:44.795171 lifeguard-mongodb-1.2.0/lifeguard_mongodb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-13 13:12:44.000000 lifeguard-mongodb-1.2.0/lifeguard_mongodb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-13 13:12:44.000000 lifeguard-mongodb-1.2.0/lifeguard_mongodb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 13:12:44.000000 lifeguard-mongodb-1.2.0/lifeguard_mongodb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-13 13:12:44.000000 lifeguard-mongodb-1.2.0/lifeguard_mongodb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-13 13:12:44.000000 lifeguard-mongodb-1.2.0/lifeguard_mongodb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 13:12:44.795171 lifeguard-mongodb-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-13 13:12:14.000000 lifeguard-mongodb-1.2.0/setup.py
```

### Comparing `lifeguard-mongodb-1.1.0/PKG-INFO` & `lifeguard-mongodb-1.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lifeguard-mongodb
-Version: 1.1.0
+Version: 1.2.0
 Summary: Lifeguard integration with MongoDB
 Home-page: https://github.com/LifeguardSystem/lifeguard-mongodb
 Author: Diego Rubin
 Author-email: contact@diegorubin.dev
 License: GPL2
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
@@ -13,9 +13,7 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: System :: Monitoring
 Description-Content-Type: text/markdown
 
 # Lifeguard MongoDB
 
-[![SourceLevel](https://app.sourcelevel.io/github/LifeguardSystem/-/lifeguard-mongodb.svg)](https://app.sourcelevel.io/github/LifeguardSystem/-/lifeguard-mongodb)
-
```

### Comparing `lifeguard-mongodb-1.1.0/lifeguard_mongodb/__init__.py` & `lifeguard-mongodb-1.2.0/lifeguard_mongodb/__init__.py`

 * *Files identical despite different names*

### Comparing `lifeguard-mongodb-1.1.0/lifeguard_mongodb/repositories.py` & `lifeguard-mongodb-1.2.0/lifeguard_mongodb/repositories.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,14 +91,17 @@
     def fetch_all_validation_results(self):
         results = []
         for result in self.collection.find():
             results.append(self.__convert_to_validation(result))
 
         return results
 
+    def delete_validation_result(self, validation_name):
+        self.collection.delete_one({"validation_name": validation_name})
+
     def __convert_to_validation(self, validation_document):
         return ValidationResponse(
             validation_document["status"],
             validation_document["details"],
             validation_document["settings"],
             last_execution=validation_document["last_execution"],
             validation_name=validation_document["validation_name"],
```

### Comparing `lifeguard-mongodb-1.1.0/lifeguard_mongodb/settings.py` & `lifeguard-mongodb-1.2.0/lifeguard_mongodb/settings.py`

 * *Files identical despite different names*

### Comparing `lifeguard-mongodb-1.1.0/lifeguard_mongodb.egg-info/PKG-INFO` & `lifeguard-mongodb-1.2.0/lifeguard_mongodb.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lifeguard-mongodb
-Version: 1.1.0
+Version: 1.2.0
 Summary: Lifeguard integration with MongoDB
 Home-page: https://github.com/LifeguardSystem/lifeguard-mongodb
 Author: Diego Rubin
 Author-email: contact@diegorubin.dev
 License: GPL2
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
@@ -13,9 +13,7 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: System :: Monitoring
 Description-Content-Type: text/markdown
 
 # Lifeguard MongoDB
 
-[![SourceLevel](https://app.sourcelevel.io/github/LifeguardSystem/-/lifeguard-mongodb.svg)](https://app.sourcelevel.io/github/LifeguardSystem/-/lifeguard-mongodb)
-
```

### Comparing `lifeguard-mongodb-1.1.0/setup.py` & `lifeguard-mongodb-1.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="lifeguard-mongodb",
-    version="1.1.0",
+    version="1.2.0",
     url="https://github.com/LifeguardSystem/lifeguard-mongodb",
     author="Diego Rubin",
     author_email="contact@diegorubin.dev",
     license="GPL2",
     scripts=[],
     include_package_data=True,
     description="Lifeguard integration with MongoDB",
```

