# Comparing `tmp/skulk-2.1.1-py2.py3-none-any.whl.zip` & `tmp/skulk-2.1.2-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 10443 bytes, number of entries: 11
--rw-r--r--  2.0 unx        5 b- defN 23-Jun-13 18:22 skulk/VERSION
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-13 18:22 skulk/__init__.py
--rw-r--r--  2.0 unx    11487 b- defN 23-Jun-13 18:22 skulk/bumper.py
--rw-r--r--  2.0 unx     2325 b- defN 23-Jun-13 18:22 skulk/questions.py
--rw-r--r--  2.0 unx    10044 b- defN 23-Jun-13 18:22 skulk/skulk.py
--rw-r--r--  2.0 unx     3586 b- defN 23-Jun-13 18:22 skulk/util.py
--rw-r--r--  2.0 unx      641 b- defN 23-Jun-13 18:22 skulk-2.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Jun-13 18:22 skulk-2.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       43 b- defN 23-Jun-13 18:22 skulk-2.1.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        6 b- defN 23-Jun-13 18:22 skulk-2.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      810 b- defN 23-Jun-13 18:22 skulk-2.1.1.dist-info/RECORD
-11 files, 29057 bytes uncompressed, 9089 bytes compressed:  68.7%
+Zip file size: 10450 bytes, number of entries: 11
+-rw-r--r--  2.0 unx        5 b- defN 23-Jun-13 18:26 skulk/VERSION
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-13 18:25 skulk/__init__.py
+-rw-r--r--  2.0 unx    11487 b- defN 23-Jun-13 18:25 skulk/bumper.py
+-rw-r--r--  2.0 unx     2325 b- defN 23-Jun-13 18:25 skulk/questions.py
+-rw-r--r--  2.0 unx    10044 b- defN 23-Jun-13 18:25 skulk/skulk.py
+-rw-r--r--  2.0 unx     3586 b- defN 23-Jun-13 18:25 skulk/util.py
+-rw-r--r--  2.0 unx      675 b- defN 23-Jun-13 18:26 skulk-2.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Jun-13 18:26 skulk-2.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       43 b- defN 23-Jun-13 18:26 skulk-2.1.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-13 18:26 skulk-2.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      810 b- defN 23-Jun-13 18:26 skulk-2.1.2.dist-info/RECORD
+11 files, 29091 bytes uncompressed, 9096 bytes compressed:  68.7%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: skulk/skulk.py
 Comment: 
 
 Filename: skulk/util.py
 Comment: 
 
-Filename: skulk-2.1.1.dist-info/METADATA
+Filename: skulk-2.1.2.dist-info/METADATA
 Comment: 
 
-Filename: skulk-2.1.1.dist-info/WHEEL
+Filename: skulk-2.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: skulk-2.1.1.dist-info/entry_points.txt
+Filename: skulk-2.1.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: skulk-2.1.1.dist-info/top_level.txt
+Filename: skulk-2.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: skulk-2.1.1.dist-info/RECORD
+Filename: skulk-2.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## skulk/VERSION

```diff
@@ -1 +1 @@
-2.1.1
+2.1.2
```

## Comparing `skulk-2.1.1.dist-info/METADATA` & `skulk-2.1.2.dist-info/METADATA`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: skulk
-Version: 2.1.1
+Version: 2.1.2
 Summary: Streamline release for Conductor client tools and others
 Home-page: https://github.com/ConductorTechnologies/skulk
 Author: Julian Mann
 Author-email: julian@conductortech.com
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
 Requires-Dist: GitPython (<4.0.0,>=3.1.31)
 Requires-Dist: semver (<4.0.0,>=3.0.0)
 Requires-Dist: twine (>=4.0.2)
 Requires-Dist: future (>=0.18.3)
 Requires-Dist: bullet (>=2.2.0)
+Requires-Dist: tabulate (>=0.9.0)
 
 Streamline release for Conductor client tools and others
```

