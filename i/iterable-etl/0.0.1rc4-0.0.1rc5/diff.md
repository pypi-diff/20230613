# Comparing `tmp/iterable_etl-0.0.1rc4.tar.gz` & `tmp/iterable_etl-0.0.1rc5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iterable_etl-0.0.1rc4.tar", last modified: Thu Jun  8 19:00:32 2023, max compression
+gzip compressed data, was "iterable_etl-0.0.1rc5.tar", last modified: Tue Jun 13 19:09:20 2023, max compression
```

## Comparing `iterable_etl-0.0.1rc4.tar` & `iterable_etl-0.0.1rc5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-08 19:00:32.013533 iterable_etl-0.0.1rc4/
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      307 2023-06-07 17:51:32.000000 iterable_etl-0.0.1rc4/MANIFEST.in
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1769 2023-06-08 19:00:32.009534 iterable_etl-0.0.1rc4/PKG-INFO
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1258 2023-06-07 21:56:06.000000 iterable_etl-0.0.1rc4/README_PUBLIC.md
-drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-08 19:00:32.009534 iterable_etl-0.0.1rc4/iterable_etl/
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-06-02 15:40:55.000000 iterable_etl-0.0.1rc4/iterable_etl/__init__.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      154 2023-06-07 15:07:58.000000 iterable_etl-0.0.1rc4/iterable_etl/__main__.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      833 2023-06-07 17:20:53.000000 iterable_etl-0.0.1rc4/iterable_etl/iterable_etl.py
-drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-08 19:00:32.009534 iterable_etl-0.0.1rc4/iterable_etl/libs/
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-06-06 22:36:56.000000 iterable_etl-0.0.1rc4/iterable_etl/libs/__init__.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      516 2023-06-07 15:37:52.000000 iterable_etl-0.0.1rc4/iterable_etl/libs/cnst.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1629 2023-06-07 19:19:44.000000 iterable_etl-0.0.1rc4/iterable_etl/libs/dbg.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      524 2023-06-07 19:21:02.000000 iterable_etl-0.0.1rc4/iterable_etl/libs/network.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      636 2023-06-07 19:11:13.000000 iterable_etl-0.0.1rc4/iterable_etl/libs/spark.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      463 2023-06-07 19:11:13.000000 iterable_etl-0.0.1rc4/iterable_etl/libs/transform.py
-drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-08 19:00:32.009534 iterable_etl-0.0.1rc4/iterable_etl/tables/
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-06-06 22:37:03.000000 iterable_etl-0.0.1rc4/iterable_etl/tables/__init__.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      832 2023-06-08 17:58:59.000000 iterable_etl-0.0.1rc4/iterable_etl/tables/campaign_history.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1359 2023-06-08 17:59:20.000000 iterable_etl-0.0.1rc4/iterable_etl/tables/campaign_list_history.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1668 2023-06-08 17:59:33.000000 iterable_etl-0.0.1rc4/iterable_etl/tables/campaign_metrics.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      758 2023-06-08 17:59:58.000000 iterable_etl-0.0.1rc4/iterable_etl/tables/list.py
-drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-08 19:00:32.009534 iterable_etl-0.0.1rc4/iterable_etl.egg-info/
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1769 2023-06-08 19:00:32.000000 iterable_etl-0.0.1rc4/iterable_etl.egg-info/PKG-INFO
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      666 2023-06-08 19:00:32.000000 iterable_etl-0.0.1rc4/iterable_etl.egg-info/SOURCES.txt
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        1 2023-06-08 19:00:32.000000 iterable_etl-0.0.1rc4/iterable_etl.egg-info/dependency_links.txt
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)       69 2023-06-08 19:00:32.000000 iterable_etl-0.0.1rc4/iterable_etl.egg-info/requires.txt
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)       13 2023-06-08 19:00:32.000000 iterable_etl-0.0.1rc4/iterable_etl.egg-info/top_level.txt
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)       38 2023-06-08 19:00:32.013533 iterable_etl-0.0.1rc4/setup.cfg
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      984 2023-06-08 19:00:09.000000 iterable_etl-0.0.1rc4/setup.py
-drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-08 19:00:32.009534 iterable_etl-0.0.1rc4/tests/
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-06-05 15:58:16.000000 iterable_etl-0.0.1rc4/tests/__init__.py
+drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-13 19:09:20.136790 iterable_etl-0.0.1rc5/
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      307 2023-06-07 17:51:32.000000 iterable_etl-0.0.1rc5/MANIFEST.in
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1769 2023-06-13 19:09:20.136790 iterable_etl-0.0.1rc5/PKG-INFO
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1258 2023-06-07 21:56:06.000000 iterable_etl-0.0.1rc5/README_PUBLIC.md
+drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-13 19:09:20.136790 iterable_etl-0.0.1rc5/iterable_etl/
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-06-02 15:40:55.000000 iterable_etl-0.0.1rc5/iterable_etl/__init__.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      154 2023-06-07 15:07:58.000000 iterable_etl-0.0.1rc5/iterable_etl/__main__.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      833 2023-06-13 17:23:12.000000 iterable_etl-0.0.1rc5/iterable_etl/iterable_etl.py
+drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-13 19:09:20.136790 iterable_etl-0.0.1rc5/iterable_etl/libs/
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-06-06 22:36:56.000000 iterable_etl-0.0.1rc5/iterable_etl/libs/__init__.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      584 2023-06-13 19:07:26.000000 iterable_etl-0.0.1rc5/iterable_etl/libs/cnst.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1629 2023-06-07 19:19:44.000000 iterable_etl-0.0.1rc5/iterable_etl/libs/dbg.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      607 2023-06-13 19:03:59.000000 iterable_etl-0.0.1rc5/iterable_etl/libs/network.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      636 2023-06-07 19:11:13.000000 iterable_etl-0.0.1rc5/iterable_etl/libs/spark.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      941 2023-06-13 19:07:15.000000 iterable_etl-0.0.1rc5/iterable_etl/libs/transform.py
+drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-13 19:09:20.136790 iterable_etl-0.0.1rc5/iterable_etl/tables/
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-06-06 22:37:03.000000 iterable_etl-0.0.1rc5/iterable_etl/tables/__init__.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      832 2023-06-08 17:58:59.000000 iterable_etl-0.0.1rc5/iterable_etl/tables/campaign_history.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1359 2023-06-08 17:59:20.000000 iterable_etl-0.0.1rc5/iterable_etl/tables/campaign_list_history.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1704 2023-06-13 19:07:15.000000 iterable_etl-0.0.1rc5/iterable_etl/tables/campaign_metrics.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      758 2023-06-08 17:59:58.000000 iterable_etl-0.0.1rc5/iterable_etl/tables/list.py
+drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-13 19:09:20.136790 iterable_etl-0.0.1rc5/iterable_etl.egg-info/
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1769 2023-06-13 19:09:20.000000 iterable_etl-0.0.1rc5/iterable_etl.egg-info/PKG-INFO
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      666 2023-06-13 19:09:20.000000 iterable_etl-0.0.1rc5/iterable_etl.egg-info/SOURCES.txt
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        1 2023-06-13 19:09:20.000000 iterable_etl-0.0.1rc5/iterable_etl.egg-info/dependency_links.txt
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)       69 2023-06-13 19:09:20.000000 iterable_etl-0.0.1rc5/iterable_etl.egg-info/requires.txt
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)       13 2023-06-13 19:09:20.000000 iterable_etl-0.0.1rc5/iterable_etl.egg-info/top_level.txt
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)       38 2023-06-13 19:09:20.136790 iterable_etl-0.0.1rc5/setup.cfg
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      984 2023-06-13 19:08:47.000000 iterable_etl-0.0.1rc5/setup.py
+drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-13 19:09:20.136790 iterable_etl-0.0.1rc5/tests/
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-06-05 15:58:16.000000 iterable_etl-0.0.1rc5/tests/__init__.py
```

### Comparing `iterable_etl-0.0.1rc4/PKG-INFO` & `iterable_etl-0.0.1rc5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iterable_etl
-Version: 0.0.1rc4
+Version: 0.0.1rc5
 Summary: Replicate iterable data in databricks
 Home-page: https://github.com/neofinancial/iterable_etl
 Author: Neo Financial
 Author-email: engineering@neofinancial.com
 License: UNLICENSED
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `iterable_etl-0.0.1rc4/README_PUBLIC.md` & `iterable_etl-0.0.1rc5/README_PUBLIC.md`

 * *Files identical despite different names*

### Comparing `iterable_etl-0.0.1rc4/iterable_etl/iterable_etl.py` & `iterable_etl-0.0.1rc5/iterable_etl/iterable_etl.py`

 * *Files identical despite different names*

### Comparing `iterable_etl-0.0.1rc4/iterable_etl/libs/dbg.py` & `iterable_etl-0.0.1rc5/iterable_etl/libs/dbg.py`

 * *Files identical despite different names*

### Comparing `iterable_etl-0.0.1rc4/iterable_etl/libs/spark.py` & `iterable_etl-0.0.1rc5/iterable_etl/libs/spark.py`

 * *Files identical despite different names*

### Comparing `iterable_etl-0.0.1rc4/iterable_etl/tables/campaign_history.py` & `iterable_etl-0.0.1rc5/iterable_etl/tables/campaign_history.py`

 * *Files identical despite different names*

### Comparing `iterable_etl-0.0.1rc4/iterable_etl/tables/campaign_list_history.py` & `iterable_etl-0.0.1rc5/iterable_etl/tables/campaign_list_history.py`

 * *Files identical despite different names*

### Comparing `iterable_etl-0.0.1rc4/iterable_etl/tables/list.py` & `iterable_etl-0.0.1rc5/iterable_etl/tables/list.py`

 * *Files identical despite different names*

### Comparing `iterable_etl-0.0.1rc4/iterable_etl.egg-info/PKG-INFO` & `iterable_etl-0.0.1rc5/iterable_etl.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iterable-etl
-Version: 0.0.1rc4
+Version: 0.0.1rc5
 Summary: Replicate iterable data in databricks
 Home-page: https://github.com/neofinancial/iterable_etl
 Author: Neo Financial
 Author-email: engineering@neofinancial.com
 License: UNLICENSED
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `iterable_etl-0.0.1rc4/iterable_etl.egg-info/SOURCES.txt` & `iterable_etl-0.0.1rc5/iterable_etl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iterable_etl-0.0.1rc4/setup.py` & `iterable_etl-0.0.1rc5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     long_description = fh.read()
 
 setup(
     author="Neo Financial",
     author_email="engineering@neofinancial.com",
     python_requires=">=3.6",
     name="iterable_etl",
-    version="0.0.1rc4",
+    version="0.0.1rc5",
     description="Replicate iterable data in databricks",
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
         "Intended Audience :: Developers",
         "Natural Language :: English",
         "Programming Language :: Python :: 3",
     ],
```

