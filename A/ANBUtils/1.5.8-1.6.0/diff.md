# Comparing `tmp/ANBUtils-1.5.8.tar.gz` & `tmp/ANBUtils-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ANBUtils-1.5.8.tar", last modified: Tue Jun 13 06:11:14 2023, max compression
+gzip compressed data, was "dist/ANBUtils-1.6.0.tar", last modified: Tue Jun 13 06:24:35 2023, max compression
```

## Comparing `ANBUtils-1.5.8.tar` & `ANBUtils-1.6.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 redbson    (501) staff       (20)        0 2023-06-13 06:11:14.311587 ANBUtils-1.5.8/
-drwxr-xr-x   0 redbson    (501) staff       (20)        0 2023-06-13 06:11:14.310127 ANBUtils-1.5.8/ANBUtils/
--rw-r--r--   0 redbson    (501) staff       (20)      881 2023-06-13 06:10:43.000000 ANBUtils-1.5.8/ANBUtils/__init__.py
--rw-r--r--   0 redbson    (501) staff       (20)     2484 2023-06-13 05:24:45.000000 ANBUtils-1.5.8/ANBUtils/a.py
--rw-r--r--   0 redbson    (501) staff       (20)    11142 2023-06-12 14:50:29.000000 ANBUtils-1.5.8/ANBUtils/db_worker.py
--rw-r--r--   0 redbson    (501) staff       (20)      932 2023-06-06 05:14:52.000000 ANBUtils-1.5.8/ANBUtils/easy_pickle.py
--rw-r--r--   0 redbson    (501) staff       (20)      917 2023-06-13 04:40:10.000000 ANBUtils-1.5.8/ANBUtils/environ_cheker.py
--rw-r--r--   0 redbson    (501) staff       (20)     3509 2023-06-06 05:12:32.000000 ANBUtils-1.5.8/ANBUtils/id_work.py
--rw-r--r--   0 redbson    (501) staff       (20)     1954 2023-06-13 04:36:50.000000 ANBUtils-1.5.8/ANBUtils/messenger.py
--rw-r--r--   0 redbson    (501) staff       (20)     4021 2023-06-06 05:17:20.000000 ANBUtils-1.5.8/ANBUtils/tbox.py
-drwxr-xr-x   0 redbson    (501) staff       (20)        0 2023-06-13 06:11:14.311116 ANBUtils-1.5.8/ANBUtils.egg-info/
--rw-r--r--   0 redbson    (501) staff       (20)     5094 2023-06-13 06:11:14.000000 ANBUtils-1.5.8/ANBUtils.egg-info/PKG-INFO
--rw-r--r--   0 redbson    (501) staff       (20)      344 2023-06-13 06:11:14.000000 ANBUtils-1.5.8/ANBUtils.egg-info/SOURCES.txt
--rw-r--r--   0 redbson    (501) staff       (20)        1 2023-06-13 06:11:14.000000 ANBUtils-1.5.8/ANBUtils.egg-info/dependency_links.txt
--rw-r--r--   0 redbson    (501) staff       (20)       94 2023-06-13 06:11:14.000000 ANBUtils-1.5.8/ANBUtils.egg-info/requires.txt
--rw-r--r--   0 redbson    (501) staff       (20)        9 2023-06-13 06:11:14.000000 ANBUtils-1.5.8/ANBUtils.egg-info/top_level.txt
--rw-r--r--   0 redbson    (501) staff       (20)     5094 2023-06-13 06:11:14.311379 ANBUtils-1.5.8/PKG-INFO
--rw-r--r--   0 redbson    (501) staff       (20)     4704 2023-06-13 06:05:52.000000 ANBUtils-1.5.8/README.md
--rw-r--r--   0 redbson    (501) staff       (20)       38 2023-06-13 06:11:14.311676 ANBUtils-1.5.8/setup.cfg
--rw-r--r--   0 redbson    (501) staff       (20)      892 2023-06-13 06:07:13.000000 ANBUtils-1.5.8/setup.py
+drwxr-xr-x   0 redbson    (501) staff       (20)        0 2023-06-13 06:24:35.083709 ANBUtils-1.6.0/
+drwxr-xr-x   0 redbson    (501) staff       (20)        0 2023-06-13 06:24:35.082434 ANBUtils-1.6.0/ANBUtils/
+-rw-r--r--   0 redbson    (501) staff       (20)      881 2023-06-13 06:10:43.000000 ANBUtils-1.6.0/ANBUtils/__init__.py
+-rw-r--r--   0 redbson    (501) staff       (20)     2484 2023-06-13 05:24:45.000000 ANBUtils-1.6.0/ANBUtils/a.py
+-rw-r--r--   0 redbson    (501) staff       (20)    11142 2023-06-12 14:50:29.000000 ANBUtils-1.6.0/ANBUtils/db_worker.py
+-rw-r--r--   0 redbson    (501) staff       (20)      932 2023-06-06 05:14:52.000000 ANBUtils-1.6.0/ANBUtils/easy_pickle.py
+-rw-r--r--   0 redbson    (501) staff       (20)      889 2023-06-13 06:22:36.000000 ANBUtils-1.6.0/ANBUtils/environ_cheker.py
+-rw-r--r--   0 redbson    (501) staff       (20)     3509 2023-06-06 05:12:32.000000 ANBUtils-1.6.0/ANBUtils/id_work.py
+-rw-r--r--   0 redbson    (501) staff       (20)     1954 2023-06-13 04:36:50.000000 ANBUtils-1.6.0/ANBUtils/messenger.py
+-rw-r--r--   0 redbson    (501) staff       (20)     4021 2023-06-06 05:17:20.000000 ANBUtils-1.6.0/ANBUtils/tbox.py
+drwxr-xr-x   0 redbson    (501) staff       (20)        0 2023-06-13 06:24:35.083292 ANBUtils-1.6.0/ANBUtils.egg-info/
+-rw-r--r--   0 redbson    (501) staff       (20)     5094 2023-06-13 06:24:35.000000 ANBUtils-1.6.0/ANBUtils.egg-info/PKG-INFO
+-rw-r--r--   0 redbson    (501) staff       (20)      344 2023-06-13 06:24:35.000000 ANBUtils-1.6.0/ANBUtils.egg-info/SOURCES.txt
+-rw-r--r--   0 redbson    (501) staff       (20)        1 2023-06-13 06:24:35.000000 ANBUtils-1.6.0/ANBUtils.egg-info/dependency_links.txt
+-rw-r--r--   0 redbson    (501) staff       (20)       94 2023-06-13 06:24:35.000000 ANBUtils-1.6.0/ANBUtils.egg-info/requires.txt
+-rw-r--r--   0 redbson    (501) staff       (20)        9 2023-06-13 06:24:35.000000 ANBUtils-1.6.0/ANBUtils.egg-info/top_level.txt
+-rw-r--r--   0 redbson    (501) staff       (20)     5094 2023-06-13 06:24:35.083513 ANBUtils-1.6.0/PKG-INFO
+-rw-r--r--   0 redbson    (501) staff       (20)     4704 2023-06-13 06:05:52.000000 ANBUtils-1.6.0/README.md
+-rw-r--r--   0 redbson    (501) staff       (20)       38 2023-06-13 06:24:35.083789 ANBUtils-1.6.0/setup.cfg
+-rw-r--r--   0 redbson    (501) staff       (20)      892 2023-06-13 06:07:13.000000 ANBUtils-1.6.0/setup.py
```

### Comparing `ANBUtils-1.5.8/ANBUtils/__init__.py` & `ANBUtils-1.6.0/ANBUtils/__init__.py`

 * *Files identical despite different names*

### Comparing `ANBUtils-1.5.8/ANBUtils/a.py` & `ANBUtils-1.6.0/ANBUtils/a.py`

 * *Files identical despite different names*

### Comparing `ANBUtils-1.5.8/ANBUtils/db_worker.py` & `ANBUtils-1.6.0/ANBUtils/db_worker.py`

 * *Files identical despite different names*

### Comparing `ANBUtils-1.5.8/ANBUtils/easy_pickle.py` & `ANBUtils-1.6.0/ANBUtils/easy_pickle.py`

 * *Files identical despite different names*

### Comparing `ANBUtils-1.5.8/ANBUtils/environ_cheker.py` & `ANBUtils-1.6.0/ANBUtils/environ_cheker.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,11 +18,11 @@
         无
 
     返回:
         无
     """
     for k in ['MONGODB_URL', 'MONGODB_PUB_URI', 'DINGTALK_WEBHOOK','QYWECHAT_WEBHOOK']:
         if k not in os.environ:
-            warnings.warn( '\nPlease set %s in environment variable' % k )
             if k == 'MONGODB_URL':
-                warnings.warn(
-                    'see <Setting Up DBWorker> https://second-cloche-446.notion.site/ANBUtils-Wiki-f3ba5d99b6904a56a3335aff927492ee' )
+                print('see <Setting Up DBWorker> https://second-cloche-446.notion.site/ANBUtils-Wiki-f3ba5d99b6904a56a3335aff927492ee' )
+            warnings.warn( '\nPlease set %s in environment variable' % k )
+
```

### Comparing `ANBUtils-1.5.8/ANBUtils/id_work.py` & `ANBUtils-1.6.0/ANBUtils/id_work.py`

 * *Files identical despite different names*

### Comparing `ANBUtils-1.5.8/ANBUtils/messenger.py` & `ANBUtils-1.6.0/ANBUtils/messenger.py`

 * *Files identical despite different names*

### Comparing `ANBUtils-1.5.8/ANBUtils/tbox.py` & `ANBUtils-1.6.0/ANBUtils/tbox.py`

 * *Files identical despite different names*

### Comparing `ANBUtils-1.5.8/ANBUtils.egg-info/PKG-INFO` & `ANBUtils-1.6.0/ANBUtils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ANBUtils
-Version: 1.5.8
+Version: 1.6.0
 Summary: ANBUilts is a versatile Python package that offers a comprehensive set of utility functions and tools for data analysis, database operations, and messaging integration.
 Home-page: https://github.com/redbson/ANBUtils
 Author: redbson
 Author-email: redbson@gmail.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `ANBUtils-1.5.8/PKG-INFO` & `ANBUtils-1.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ANBUtils
-Version: 1.5.8
+Version: 1.6.0
 Summary: ANBUilts is a versatile Python package that offers a comprehensive set of utility functions and tools for data analysis, database operations, and messaging integration.
 Home-page: https://github.com/redbson/ANBUtils
 Author: redbson
 Author-email: redbson@gmail.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `ANBUtils-1.5.8/README.md` & `ANBUtils-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `ANBUtils-1.5.8/setup.py` & `ANBUtils-1.6.0/setup.py`

 * *Files identical despite different names*

