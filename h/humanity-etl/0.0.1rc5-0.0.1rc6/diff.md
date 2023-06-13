# Comparing `tmp/humanity_etl-0.0.1rc5.tar.gz` & `tmp/humanity_etl-0.0.1rc6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "humanity_etl-0.0.1rc5.tar", last modified: Mon Jun 12 20:31:05 2023, max compression
+gzip compressed data, was "humanity_etl-0.0.1rc6.tar", last modified: Tue Jun 13 15:40:06 2023, max compression
```

## Comparing `humanity_etl-0.0.1rc5.tar` & `humanity_etl-0.0.1rc6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-12 20:31:05.796217 humanity_etl-0.0.1rc5/
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      307 2023-06-07 17:51:32.000000 humanity_etl-0.0.1rc5/MANIFEST.in
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1495 2023-06-12 20:31:05.796217 humanity_etl-0.0.1rc5/PKG-INFO
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      984 2023-06-08 17:49:58.000000 humanity_etl-0.0.1rc5/README_PUBLIC.md
-drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-12 20:31:05.792217 humanity_etl-0.0.1rc5/humanity_etl/
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-06-02 15:40:55.000000 humanity_etl-0.0.1rc5/humanity_etl/__init__.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      154 2023-06-08 17:37:37.000000 humanity_etl-0.0.1rc5/humanity_etl/__main__.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      328 2023-06-08 17:11:05.000000 humanity_etl-0.0.1rc5/humanity_etl/humanity_etl.py
-drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-12 20:31:05.796217 humanity_etl-0.0.1rc5/humanity_etl/libs/
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-06-06 22:36:56.000000 humanity_etl-0.0.1rc5/humanity_etl/libs/__init__.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     4841 2023-06-12 19:40:35.000000 humanity_etl-0.0.1rc5/humanity_etl/libs/cnst.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1629 2023-06-07 19:19:44.000000 humanity_etl-0.0.1rc5/humanity_etl/libs/dbg.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      547 2023-06-12 20:29:22.000000 humanity_etl-0.0.1rc5/humanity_etl/libs/network.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     5966 2023-06-08 18:01:30.000000 humanity_etl-0.0.1rc5/humanity_etl/libs/transform.py
-drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-12 20:31:05.796217 humanity_etl-0.0.1rc5/humanity_etl/tables/
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-06-06 22:37:03.000000 humanity_etl-0.0.1rc5/humanity_etl/tables/__init__.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     4489 2023-06-12 20:29:08.000000 humanity_etl-0.0.1rc5/humanity_etl/tables/timeclocks.py
-drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-12 20:31:05.792217 humanity_etl-0.0.1rc5/humanity_etl.egg-info/
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1495 2023-06-12 20:31:05.000000 humanity_etl-0.0.1rc5/humanity_etl.egg-info/PKG-INFO
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      520 2023-06-12 20:31:05.000000 humanity_etl-0.0.1rc5/humanity_etl.egg-info/SOURCES.txt
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        1 2023-06-12 20:31:05.000000 humanity_etl-0.0.1rc5/humanity_etl.egg-info/dependency_links.txt
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)       75 2023-06-12 20:31:05.000000 humanity_etl-0.0.1rc5/humanity_etl.egg-info/requires.txt
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)       13 2023-06-12 20:31:05.000000 humanity_etl-0.0.1rc5/humanity_etl.egg-info/top_level.txt
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)       38 2023-06-12 20:31:05.796217 humanity_etl-0.0.1rc5/setup.cfg
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      990 2023-06-12 20:30:51.000000 humanity_etl-0.0.1rc5/setup.py
-drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-12 20:31:05.796217 humanity_etl-0.0.1rc5/tests/
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-06-05 15:58:16.000000 humanity_etl-0.0.1rc5/tests/__init__.py
+drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-13 15:40:06.843053 humanity_etl-0.0.1rc6/
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      307 2023-06-07 17:51:32.000000 humanity_etl-0.0.1rc6/MANIFEST.in
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1495 2023-06-13 15:40:06.843053 humanity_etl-0.0.1rc6/PKG-INFO
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      984 2023-06-08 17:49:58.000000 humanity_etl-0.0.1rc6/README_PUBLIC.md
+drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-13 15:40:06.839053 humanity_etl-0.0.1rc6/humanity_etl/
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-06-02 15:40:55.000000 humanity_etl-0.0.1rc6/humanity_etl/__init__.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      154 2023-06-08 17:37:37.000000 humanity_etl-0.0.1rc6/humanity_etl/__main__.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      328 2023-06-08 17:11:05.000000 humanity_etl-0.0.1rc6/humanity_etl/humanity_etl.py
+drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-13 15:40:06.843053 humanity_etl-0.0.1rc6/humanity_etl/libs/
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-06-06 22:36:56.000000 humanity_etl-0.0.1rc6/humanity_etl/libs/__init__.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     4841 2023-06-12 19:40:35.000000 humanity_etl-0.0.1rc6/humanity_etl/libs/cnst.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1629 2023-06-07 19:19:44.000000 humanity_etl-0.0.1rc6/humanity_etl/libs/dbg.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      547 2023-06-12 20:29:22.000000 humanity_etl-0.0.1rc6/humanity_etl/libs/network.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     5966 2023-06-08 18:01:30.000000 humanity_etl-0.0.1rc6/humanity_etl/libs/transform.py
+drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-13 15:40:06.843053 humanity_etl-0.0.1rc6/humanity_etl/tables/
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-06-06 22:37:03.000000 humanity_etl-0.0.1rc6/humanity_etl/tables/__init__.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     4489 2023-06-13 15:39:00.000000 humanity_etl-0.0.1rc6/humanity_etl/tables/timeclocks.py
+drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-13 15:40:06.839053 humanity_etl-0.0.1rc6/humanity_etl.egg-info/
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1495 2023-06-13 15:40:06.000000 humanity_etl-0.0.1rc6/humanity_etl.egg-info/PKG-INFO
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      520 2023-06-13 15:40:06.000000 humanity_etl-0.0.1rc6/humanity_etl.egg-info/SOURCES.txt
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        1 2023-06-13 15:40:06.000000 humanity_etl-0.0.1rc6/humanity_etl.egg-info/dependency_links.txt
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)       75 2023-06-13 15:40:06.000000 humanity_etl-0.0.1rc6/humanity_etl.egg-info/requires.txt
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)       13 2023-06-13 15:40:06.000000 humanity_etl-0.0.1rc6/humanity_etl.egg-info/top_level.txt
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)       38 2023-06-13 15:40:06.843053 humanity_etl-0.0.1rc6/setup.cfg
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      990 2023-06-13 15:39:38.000000 humanity_etl-0.0.1rc6/setup.py
+drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-13 15:40:06.843053 humanity_etl-0.0.1rc6/tests/
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-06-05 15:58:16.000000 humanity_etl-0.0.1rc6/tests/__init__.py
```

### Comparing `humanity_etl-0.0.1rc5/PKG-INFO` & `humanity_etl-0.0.1rc6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: humanity_etl
-Version: 0.0.1rc5
+Version: 0.0.1rc6
 Summary: Replicate humanity data in databricks
 Home-page: https://github.com/neofinancial/humanity_etl
 Author: Neo Financial
 Author-email: engineering@neofinancial.com
 License: UNLICENSED
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `humanity_etl-0.0.1rc5/README_PUBLIC.md` & `humanity_etl-0.0.1rc6/README_PUBLIC.md`

 * *Files identical despite different names*

### Comparing `humanity_etl-0.0.1rc5/humanity_etl/libs/cnst.py` & `humanity_etl-0.0.1rc6/humanity_etl/libs/cnst.py`

 * *Files identical despite different names*

### Comparing `humanity_etl-0.0.1rc5/humanity_etl/libs/dbg.py` & `humanity_etl-0.0.1rc6/humanity_etl/libs/dbg.py`

 * *Files identical despite different names*

### Comparing `humanity_etl-0.0.1rc5/humanity_etl/libs/network.py` & `humanity_etl-0.0.1rc6/humanity_etl/libs/network.py`

 * *Files identical despite different names*

### Comparing `humanity_etl-0.0.1rc5/humanity_etl/libs/transform.py` & `humanity_etl-0.0.1rc6/humanity_etl/libs/transform.py`

 * *Files identical despite different names*

### Comparing `humanity_etl-0.0.1rc5/humanity_etl/tables/timeclocks.py` & `humanity_etl-0.0.1rc6/humanity_etl/tables/timeclocks.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,15 +103,15 @@
     ott_program_df = merger(
         ott_timeclocks_df, ott_positions_df, ott_employees_df, ott_shifts_df, "OTT"
     )
     edm_program_df = merger(
         edm_timeclocks_df, edm_positions_df, edm_employees_df, edm_shifts_df, "EDM"
     )
     mtl_program_df = merger(
-        mtl_timeclocks_df, mtl_positions_df, mtl_employees_df, mtl_shifts_df, "EDM"
+        mtl_timeclocks_df, mtl_positions_df, mtl_employees_df, mtl_shifts_df, "MTL"
     )
 
     # "UNION" all region dataframes
     humanity_df = pd.concat(
         [gta_program_df, cgy_program_df, wpg_program_df, edm_program_df, ott_program_df, mtl_program_df]
     )
     humanity_final_df = humanity_df.merge(
```

### Comparing `humanity_etl-0.0.1rc5/humanity_etl.egg-info/PKG-INFO` & `humanity_etl-0.0.1rc6/humanity_etl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: humanity-etl
-Version: 0.0.1rc5
+Version: 0.0.1rc6
 Summary: Replicate humanity data in databricks
 Home-page: https://github.com/neofinancial/humanity_etl
 Author: Neo Financial
 Author-email: engineering@neofinancial.com
 License: UNLICENSED
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `humanity_etl-0.0.1rc5/humanity_etl.egg-info/SOURCES.txt` & `humanity_etl-0.0.1rc6/humanity_etl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `humanity_etl-0.0.1rc5/setup.py` & `humanity_etl-0.0.1rc6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     long_description = fh.read()
 
 setup(
     author="Neo Financial",
     author_email="engineering@neofinancial.com",
     python_requires=">=3.6",
     name="humanity_etl",
-    version="0.0.1rc5",
+    version="0.0.1rc6",
     description="Replicate humanity data in databricks",
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
         "Intended Audience :: Developers",
         "Natural Language :: English",
         "Programming Language :: Python :: 3",
     ],
```

