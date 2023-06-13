# Comparing `tmp/automongobackup-0.0.4.tar.gz` & `tmp/automongobackup-0.0.5.tar.gz`

## Comparing `automongobackup-0.0.4.tar` & `automongobackup-0.0.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 automongobackup-0.0.4/src/automongobackup/__init__.py
--rw-r--r--   0        0        0     5884 2020-02-02 00:00:00.000000 automongobackup-0.0.4/src/automongobackup/automongobackup.py
--rw-r--r--   0        0        0     3253 2020-02-02 00:00:00.000000 automongobackup-0.0.4/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 automongobackup-0.0.4/LICENSE.txt
--rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 automongobackup-0.0.4/README.md
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 automongobackup-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     4083 2020-02-02 00:00:00.000000 automongobackup-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 automongobackup-0.0.5/src/automongobackup/__init__.py
+-rw-r--r--   0        0        0     5884 2020-02-02 00:00:00.000000 automongobackup-0.0.5/src/automongobackup/automongobackup.py
+-rw-r--r--   0        0        0     3253 2020-02-02 00:00:00.000000 automongobackup-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 automongobackup-0.0.5/LICENSE.txt
+-rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 automongobackup-0.0.5/README.md
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 automongobackup-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     4083 2020-02-02 00:00:00.000000 automongobackup-0.0.5/PKG-INFO
```

### Comparing `automongobackup-0.0.4/src/automongobackup/automongobackup.py` & `automongobackup-0.0.5/src/automongobackup/automongobackup.py`

 * *Files identical despite different names*

### Comparing `automongobackup-0.0.4/.gitignore` & `automongobackup-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `automongobackup-0.0.4/LICENSE.txt` & `automongobackup-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `automongobackup-0.0.4/README.md` & `automongobackup-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `automongobackup-0.0.4/pyproject.toml` & `automongobackup-0.0.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "automongobackup"
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
 "Homepage" = "https://github.com/IamLizu/automongobackup"
 "Bug Tracker" = "https://github.com/IamLizu/automongobackup/issues"
 
 [project.scripts]
-automongobackup = "automongobackup.automongobackup:__main__"
+automongobackup = "automongobackup.automongobackup:main"
```

### Comparing `automongobackup-0.0.4/PKG-INFO` & `automongobackup-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automongobackup
-Version: 0.0.4
+Version: 0.0.5
 Summary: Automated script generator to backup MongoDB databases to Amazon S3.
 Project-URL: Homepage, https://github.com/IamLizu/automongobackup
 Project-URL: Bug Tracker, https://github.com/IamLizu/automongobackup/issues
 Author-email: S M Mahmudul Hasan <thegeek@iamlizu.com>
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

