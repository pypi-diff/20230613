# Comparing `tmp/automongobackup-0.0.2.tar.gz` & `tmp/automongobackup-0.0.3.tar.gz`

## Comparing `automongobackup-0.0.2.tar` & `automongobackup-0.0.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 automongobackup-0.0.2/src/automongobackup/__init__.py
--rw-r--r--   0        0        0     5884 2020-02-02 00:00:00.000000 automongobackup-0.0.2/src/automongobackup/automongobackup.py
--rw-r--r--   0        0        0     3253 2020-02-02 00:00:00.000000 automongobackup-0.0.2/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 automongobackup-0.0.2/LICENSE.txt
--rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 automongobackup-0.0.2/README.md
--rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 automongobackup-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     4083 2020-02-02 00:00:00.000000 automongobackup-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 automongobackup-0.0.3/src/automongobackup/__init__.py
+-rw-r--r--   0        0        0     5884 2020-02-02 00:00:00.000000 automongobackup-0.0.3/src/automongobackup/__main__.py
+-rw-r--r--   0        0        0     3253 2020-02-02 00:00:00.000000 automongobackup-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 automongobackup-0.0.3/LICENSE.txt
+-rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 automongobackup-0.0.3/README.md
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 automongobackup-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     4083 2020-02-02 00:00:00.000000 automongobackup-0.0.3/PKG-INFO
```

### Comparing `automongobackup-0.0.2/src/automongobackup/automongobackup.py` & `automongobackup-0.0.3/src/automongobackup/__main__.py`

 * *Files identical despite different names*

### Comparing `automongobackup-0.0.2/.gitignore` & `automongobackup-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `automongobackup-0.0.2/LICENSE.txt` & `automongobackup-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `automongobackup-0.0.2/README.md` & `automongobackup-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `automongobackup-0.0.2/pyproject.toml` & `automongobackup-0.0.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "automongobackup"
-version = "0.0.2"
+version = "0.0.3"
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
 "Homepage" = "https://github.com/IamLizu/automongobackup"
 "Bug Tracker" = "https://github.com/IamLizu/automongobackup/issues"
 
 [project.scripts]
-automongobackup = "automongobackup:main"
+automongobackup = "automongobackup:__main__"
```

### Comparing `automongobackup-0.0.2/PKG-INFO` & `automongobackup-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automongobackup
-Version: 0.0.2
+Version: 0.0.3
 Summary: Automated script generator to backup MongoDB databases to Amazon S3.
 Project-URL: Homepage, https://github.com/IamLizu/automongobackup
 Project-URL: Bug Tracker, https://github.com/IamLizu/automongobackup/issues
 Author-email: S M Mahmudul Hasan <thegeek@iamlizu.com>
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

