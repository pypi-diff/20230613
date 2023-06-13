# Comparing `tmp/lifeguard-tinydb-1.0.0.tar.gz` & `tmp/lifeguard-tinydb-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lifeguard-tinydb-1.0.0.tar", last modified: Fri May 26 20:08:48 2023, max compression
+gzip compressed data, was "lifeguard-tinydb-1.2.0.tar", last modified: Tue Jun 13 13:49:27 2023, max compression
```

## Comparing `lifeguard-tinydb-1.0.0.tar` & `lifeguard-tinydb-1.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:08:48.575727 lifeguard-tinydb-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-26 20:08:48.575727 lifeguard-tinydb-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-26 20:08:27.000000 lifeguard-tinydb-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:08:48.575727 lifeguard-tinydb-1.0.0/lifeguard_tinydb/
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-26 20:08:27.000000 lifeguard-tinydb-1.0.0/lifeguard_tinydb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-05-26 20:08:27.000000 lifeguard-tinydb-1.0.0/lifeguard_tinydb/repositories.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-26 20:08:27.000000 lifeguard-tinydb-1.0.0/lifeguard_tinydb/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:08:48.575727 lifeguard-tinydb-1.0.0/lifeguard_tinydb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-26 20:08:48.000000 lifeguard-tinydb-1.0.0/lifeguard_tinydb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-26 20:08:48.000000 lifeguard-tinydb-1.0.0/lifeguard_tinydb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 20:08:48.000000 lifeguard-tinydb-1.0.0/lifeguard_tinydb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-26 20:08:48.000000 lifeguard-tinydb-1.0.0/lifeguard_tinydb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-26 20:08:48.000000 lifeguard-tinydb-1.0.0/lifeguard_tinydb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 20:08:48.575727 lifeguard-tinydb-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-05-26 20:08:27.000000 lifeguard-tinydb-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:49:27.036540 lifeguard-tinydb-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-13 13:49:27.036540 lifeguard-tinydb-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-13 13:49:02.000000 lifeguard-tinydb-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:49:27.036540 lifeguard-tinydb-1.2.0/lifeguard_tinydb/
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-13 13:49:02.000000 lifeguard-tinydb-1.2.0/lifeguard_tinydb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-06-13 13:49:02.000000 lifeguard-tinydb-1.2.0/lifeguard_tinydb/repositories.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-13 13:49:02.000000 lifeguard-tinydb-1.2.0/lifeguard_tinydb/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:49:27.036540 lifeguard-tinydb-1.2.0/lifeguard_tinydb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-13 13:49:26.000000 lifeguard-tinydb-1.2.0/lifeguard_tinydb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-13 13:49:27.000000 lifeguard-tinydb-1.2.0/lifeguard_tinydb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 13:49:26.000000 lifeguard-tinydb-1.2.0/lifeguard_tinydb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-13 13:49:26.000000 lifeguard-tinydb-1.2.0/lifeguard_tinydb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-13 13:49:26.000000 lifeguard-tinydb-1.2.0/lifeguard_tinydb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 13:49:27.036540 lifeguard-tinydb-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-13 13:49:02.000000 lifeguard-tinydb-1.2.0/setup.py
```

### Comparing `lifeguard-tinydb-1.0.0/PKG-INFO` & `lifeguard-tinydb-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lifeguard-tinydb
-Version: 1.0.0
+Version: 1.2.0
 Summary: Lifeguard integration with TinyDB
 Home-page: https://github.com/LifeguardSystem/lifeguard-tinydb
 Author: Diego Rubin
 Author-email: contact@diegorubin.dev
 License: GPL2
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
```

### Comparing `lifeguard-tinydb-1.0.0/lifeguard_tinydb/__init__.py` & `lifeguard-tinydb-1.2.0/lifeguard_tinydb/__init__.py`

 * *Files identical despite different names*

### Comparing `lifeguard-tinydb-1.0.0/lifeguard_tinydb/repositories.py` & `lifeguard-tinydb-1.2.0/lifeguard_tinydb/repositories.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,14 +60,17 @@
     def fetch_all_validation_results(self):
         results = []
         for result in self.table.all():
             results.append(self.__convert_to_validation(result))
 
         return results
 
+    def delete_validation_result(self, validation_name):
+        self.table.remove(self.__get_key(validation_name))
+
     def __convert_to_validation(self, entry):
         last_execution = entry["last_execution"]
 
         if last_execution:
             last_execution = datetime.strptime(last_execution, DATE_FORMAT)
 
         return ValidationResponse(
```

### Comparing `lifeguard-tinydb-1.0.0/lifeguard_tinydb.egg-info/PKG-INFO` & `lifeguard-tinydb-1.2.0/lifeguard_tinydb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lifeguard-tinydb
-Version: 1.0.0
+Version: 1.2.0
 Summary: Lifeguard integration with TinyDB
 Home-page: https://github.com/LifeguardSystem/lifeguard-tinydb
 Author: Diego Rubin
 Author-email: contact@diegorubin.dev
 License: GPL2
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
```

### Comparing `lifeguard-tinydb-1.0.0/setup.py` & `lifeguard-tinydb-1.2.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="lifeguard-tinydb",
-    version="1.0.0",
+    version="1.2.0",
     url="https://github.com/LifeguardSystem/lifeguard-tinydb",
     author="Diego Rubin",
     author_email="contact@diegorubin.dev",
     license="GPL2",
     scripts=[],
     include_package_data=True,
     description="Lifeguard integration with TinyDB",
```

