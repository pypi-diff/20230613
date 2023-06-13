# Comparing `tmp/skulk-2.1.0-py2.py3-none-any.whl.zip` & `tmp/skulk-2.1.1-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 10429 bytes, number of entries: 11
--rw-r--r--  2.0 unx        5 b- defN 23-Jun-13 17:57 skulk/VERSION
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-13 17:56 skulk/__init__.py
--rw-r--r--  2.0 unx    11487 b- defN 23-Jun-13 17:56 skulk/bumper.py
--rw-r--r--  2.0 unx     2325 b- defN 23-Jun-13 17:56 skulk/questions.py
--rw-r--r--  2.0 unx    10044 b- defN 23-Jun-13 17:56 skulk/skulk.py
--rw-r--r--  2.0 unx     3586 b- defN 23-Jun-13 17:56 skulk/util.py
--rw-r--r--  2.0 unx      609 b- defN 23-Jun-13 17:57 skulk-2.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Jun-13 17:57 skulk-2.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       43 b- defN 23-Jun-13 17:57 skulk-2.1.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        6 b- defN 23-Jun-13 17:57 skulk-2.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      810 b- defN 23-Jun-13 17:57 skulk-2.1.0.dist-info/RECORD
-11 files, 29025 bytes uncompressed, 9075 bytes compressed:  68.7%
+Zip file size: 10443 bytes, number of entries: 11
+-rw-r--r--  2.0 unx        5 b- defN 23-Jun-13 18:22 skulk/VERSION
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-13 18:22 skulk/__init__.py
+-rw-r--r--  2.0 unx    11487 b- defN 23-Jun-13 18:22 skulk/bumper.py
+-rw-r--r--  2.0 unx     2325 b- defN 23-Jun-13 18:22 skulk/questions.py
+-rw-r--r--  2.0 unx    10044 b- defN 23-Jun-13 18:22 skulk/skulk.py
+-rw-r--r--  2.0 unx     3586 b- defN 23-Jun-13 18:22 skulk/util.py
+-rw-r--r--  2.0 unx      641 b- defN 23-Jun-13 18:22 skulk-2.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Jun-13 18:22 skulk-2.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       43 b- defN 23-Jun-13 18:22 skulk-2.1.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-13 18:22 skulk-2.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      810 b- defN 23-Jun-13 18:22 skulk-2.1.1.dist-info/RECORD
+11 files, 29057 bytes uncompressed, 9089 bytes compressed:  68.7%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: skulk/skulk.py
 Comment: 
 
 Filename: skulk/util.py
 Comment: 
 
-Filename: skulk-2.1.0.dist-info/METADATA
+Filename: skulk-2.1.1.dist-info/METADATA
 Comment: 
 
-Filename: skulk-2.1.0.dist-info/WHEEL
+Filename: skulk-2.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: skulk-2.1.0.dist-info/entry_points.txt
+Filename: skulk-2.1.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: skulk-2.1.0.dist-info/top_level.txt
+Filename: skulk-2.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: skulk-2.1.0.dist-info/RECORD
+Filename: skulk-2.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## skulk/VERSION

```diff
@@ -1 +1 @@
-2.1.0
+2.1.1
```

## Comparing `skulk-2.1.0.dist-info/METADATA` & `skulk-2.1.1.dist-info/METADATA`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: skulk
-Version: 2.1.0
+Version: 2.1.1
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
+Requires-Dist: bullet (>=2.2.0)
 
 Streamline release for Conductor client tools and others
```

## Comparing `skulk-2.1.0.dist-info/RECORD` & `skulk-2.1.1.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-skulk/VERSION,sha256=gkj3dyaHr_CxA7NomJCN64ISYzf5M-SaWsBIKQk8WP8,5
+skulk/VERSION,sha256=NaRqRC3vqCyjYmWIns3nfRidkEDoDHRq_xdeNPkac1w,5
 skulk/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 skulk/bumper.py,sha256=lIg6y4Nrzf7-in1kqnZP9XosjqK0BhprgImejvGdsks,11487
 skulk/questions.py,sha256=08ujtmpZss7VmNwlFMYVJZx_sJG_GsCjloURUrFG1ok,2325
 skulk/skulk.py,sha256=4Ytv48qPDy_uAucHz1mTZv9ew2RsHN3IY98hDVbESdo,10044
 skulk/util.py,sha256=uBlyNpq_8RsuD2oOKxk4cL7-2zqXotcBPjI-QHacsHo,3586
-skulk-2.1.0.dist-info/METADATA,sha256=n-oQx32o3nV-e7M6erQtd6wDOd4yd3e2U9D7-lem_j4,609
-skulk-2.1.0.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
-skulk-2.1.0.dist-info/entry_points.txt,sha256=8DGRFZ3C46ZQBYFsfNj4eYw5ZGq8NWW8uKe-2xC-c34,43
-skulk-2.1.0.dist-info/top_level.txt,sha256=EOnQuA1Vdf2WjOz9xLTPLCynTq2IdzLPGQ54LdhP7oY,6
-skulk-2.1.0.dist-info/RECORD,,
+skulk-2.1.1.dist-info/METADATA,sha256=auOZmGoG8iSne8gVdTEAZk2fsPqxvkfsGzclbOm9Jjw,641
+skulk-2.1.1.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+skulk-2.1.1.dist-info/entry_points.txt,sha256=8DGRFZ3C46ZQBYFsfNj4eYw5ZGq8NWW8uKe-2xC-c34,43
+skulk-2.1.1.dist-info/top_level.txt,sha256=EOnQuA1Vdf2WjOz9xLTPLCynTq2IdzLPGQ54LdhP7oY,6
+skulk-2.1.1.dist-info/RECORD,,
```

