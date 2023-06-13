# Comparing `tmp/simfin-0.9.1.tar.gz` & `tmp/simfin-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simfin-0.9.1.tar", last modified: Thu Apr 13 14:14:22 2023, max compression
+gzip compressed data, was "simfin-0.9.2.tar", last modified: Tue Jun 13 19:21:31 2023, max compression
```

## Comparing `simfin-0.9.1.tar` & `simfin-0.9.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 thomasflassbeck   (501) staff       (20)        0 2023-04-13 14:14:22.044146 simfin-0.9.1/
--rw-r--r--   0 thomasflassbeck   (501) staff       (20)     1259 2023-02-22 12:33:47.000000 simfin-0.9.1/LICENSE.txt
--rw-r--r--   0 thomasflassbeck   (501) staff       (20)      570 2023-04-13 14:14:22.043950 simfin-0.9.1/PKG-INFO
--rw-r--r--   0 thomasflassbeck   (501) staff       (20)     7352 2023-02-22 12:33:47.000000 simfin-0.9.1/README.md
--rw-r--r--   0 thomasflassbeck   (501) staff       (20)       38 2023-04-13 14:14:22.044205 simfin-0.9.1/setup.cfg
--rw-r--r--   0 thomasflassbeck   (501) staff       (20)     1008 2023-04-13 14:10:04.000000 simfin-0.9.1/setup.py
-drwxr-xr-x   0 thomasflassbeck   (501) staff       (20)        0 2023-04-13 14:14:22.042936 simfin-0.9.1/simfin/
--rw-r--r--   0 thomasflassbeck   (501) staff       (20)     1621 2023-04-13 14:11:07.000000 simfin-0.9.1/simfin/__init__.py
--rw-r--r--   0 thomasflassbeck   (501) staff       (20)    11769 2023-02-22 12:33:47.000000 simfin-0.9.1/simfin/cache.py
--rw-r--r--   0 thomasflassbeck   (501) staff       (20)     4917 2023-02-22 12:33:47.000000 simfin-0.9.1/simfin/config.py
--rw-r--r--   0 thomasflassbeck   (501) staff       (20)    10036 2023-02-22 12:33:47.000000 simfin-0.9.1/simfin/datasets.py
--rw-r--r--   0 thomasflassbeck   (501) staff       (20)     6944 2023-02-22 12:33:47.000000 simfin-0.9.1/simfin/derived.py
--rw-r--r--   0 thomasflassbeck   (501) staff       (20)    11021 2023-04-13 14:10:11.000000 simfin-0.9.1/simfin/download.py
--rw-r--r--   0 thomasflassbeck   (501) staff       (20)      743 2023-02-22 12:33:47.000000 simfin-0.9.1/simfin/exceptions.py
--rw-r--r--   0 thomasflassbeck   (501) staff       (20)    31133 2023-02-22 12:33:47.000000 simfin-0.9.1/simfin/hubs.py
--rw-r--r--   0 thomasflassbeck   (501) staff       (20)     8872 2023-02-22 12:33:47.000000 simfin-0.9.1/simfin/info.py
--rw-r--r--   0 thomasflassbeck   (501) staff       (20)    11940 2023-04-13 14:10:11.000000 simfin-0.9.1/simfin/load.py
--rw-r--r--   0 thomasflassbeck   (501) staff       (20)     2925 2023-02-22 12:33:47.000000 simfin-0.9.1/simfin/load_info.py
--rw-r--r--   0 thomasflassbeck   (501) staff       (20)    19450 2023-02-22 12:33:47.000000 simfin-0.9.1/simfin/names.py
--rw-r--r--   0 thomasflassbeck   (501) staff       (20)     7990 2023-02-22 13:21:56.000000 simfin-0.9.1/simfin/names_extra.py
--rw-r--r--   0 thomasflassbeck   (501) staff       (20)     3830 2023-02-22 12:33:47.000000 simfin-0.9.1/simfin/paths.py
--rw-r--r--   0 thomasflassbeck   (501) staff       (20)    17189 2023-02-22 12:33:47.000000 simfin-0.9.1/simfin/rel_change.py
--rw-r--r--   0 thomasflassbeck   (501) staff       (20)    14284 2023-02-22 12:33:47.000000 simfin-0.9.1/simfin/resample.py
--rw-r--r--   0 thomasflassbeck   (501) staff       (20)    37350 2023-02-22 12:33:47.000000 simfin-0.9.1/simfin/signals.py
--rw-r--r--   0 thomasflassbeck   (501) staff       (20)    14331 2023-02-22 12:33:47.000000 simfin-0.9.1/simfin/transform.py
--rw-r--r--   0 thomasflassbeck   (501) staff       (20)    15933 2023-04-13 14:10:11.000000 simfin-0.9.1/simfin/utils.py
-drwxr-xr-x   0 thomasflassbeck   (501) staff       (20)        0 2023-04-13 14:14:22.043708 simfin-0.9.1/simfin.egg-info/
--rw-r--r--   0 thomasflassbeck   (501) staff       (20)      570 2023-04-13 14:14:22.000000 simfin-0.9.1/simfin.egg-info/PKG-INFO
--rw-r--r--   0 thomasflassbeck   (501) staff       (20)      521 2023-04-13 14:14:22.000000 simfin-0.9.1/simfin.egg-info/SOURCES.txt
--rw-r--r--   0 thomasflassbeck   (501) staff       (20)        1 2023-04-13 14:14:22.000000 simfin-0.9.1/simfin.egg-info/dependency_links.txt
--rw-r--r--   0 thomasflassbeck   (501) staff       (20)       22 2023-04-13 14:14:22.000000 simfin-0.9.1/simfin.egg-info/requires.txt
--rw-r--r--   0 thomasflassbeck   (501) staff       (20)        7 2023-04-13 14:14:22.000000 simfin-0.9.1/simfin.egg-info/top_level.txt
+drwxr-xr-x   0 thomasflassbeck   (501) staff       (20)        0 2023-06-13 19:21:31.898093 simfin-0.9.2/
+-rw-r--r--   0 thomasflassbeck   (501) staff       (20)     1259 2023-02-22 12:33:47.000000 simfin-0.9.2/LICENSE.txt
+-rw-r--r--   0 thomasflassbeck   (501) staff       (20)      570 2023-06-13 19:21:31.897907 simfin-0.9.2/PKG-INFO
+-rw-r--r--   0 thomasflassbeck   (501) staff       (20)     7352 2023-02-22 12:33:47.000000 simfin-0.9.2/README.md
+-rw-r--r--   0 thomasflassbeck   (501) staff       (20)       38 2023-06-13 19:21:31.898138 simfin-0.9.2/setup.cfg
+-rw-r--r--   0 thomasflassbeck   (501) staff       (20)     1008 2023-06-13 19:20:51.000000 simfin-0.9.2/setup.py
+drwxr-xr-x   0 thomasflassbeck   (501) staff       (20)        0 2023-06-13 19:21:31.896684 simfin-0.9.2/simfin/
+-rw-r--r--   0 thomasflassbeck   (501) staff       (20)     1621 2023-04-13 14:11:07.000000 simfin-0.9.2/simfin/__init__.py
+-rw-r--r--   0 thomasflassbeck   (501) staff       (20)    11769 2023-02-22 12:33:47.000000 simfin-0.9.2/simfin/cache.py
+-rw-r--r--   0 thomasflassbeck   (501) staff       (20)     4917 2023-02-22 12:33:47.000000 simfin-0.9.2/simfin/config.py
+-rw-r--r--   0 thomasflassbeck   (501) staff       (20)    10036 2023-02-22 12:33:47.000000 simfin-0.9.2/simfin/datasets.py
+-rw-r--r--   0 thomasflassbeck   (501) staff       (20)     6944 2023-02-22 12:33:47.000000 simfin-0.9.2/simfin/derived.py
+-rw-r--r--   0 thomasflassbeck   (501) staff       (20)    11027 2023-06-13 19:20:51.000000 simfin-0.9.2/simfin/download.py
+-rw-r--r--   0 thomasflassbeck   (501) staff       (20)      743 2023-02-22 12:33:47.000000 simfin-0.9.2/simfin/exceptions.py
+-rw-r--r--   0 thomasflassbeck   (501) staff       (20)    31133 2023-02-22 12:33:47.000000 simfin-0.9.2/simfin/hubs.py
+-rw-r--r--   0 thomasflassbeck   (501) staff       (20)     8872 2023-02-22 12:33:47.000000 simfin-0.9.2/simfin/info.py
+-rw-r--r--   0 thomasflassbeck   (501) staff       (20)    11940 2023-04-13 14:10:11.000000 simfin-0.9.2/simfin/load.py
+-rw-r--r--   0 thomasflassbeck   (501) staff       (20)     2925 2023-02-22 12:33:47.000000 simfin-0.9.2/simfin/load_info.py
+-rw-r--r--   0 thomasflassbeck   (501) staff       (20)    19450 2023-02-22 12:33:47.000000 simfin-0.9.2/simfin/names.py
+-rw-r--r--   0 thomasflassbeck   (501) staff       (20)     7990 2023-02-22 13:21:56.000000 simfin-0.9.2/simfin/names_extra.py
+-rw-r--r--   0 thomasflassbeck   (501) staff       (20)     3830 2023-02-22 12:33:47.000000 simfin-0.9.2/simfin/paths.py
+-rw-r--r--   0 thomasflassbeck   (501) staff       (20)    17189 2023-02-22 12:33:47.000000 simfin-0.9.2/simfin/rel_change.py
+-rw-r--r--   0 thomasflassbeck   (501) staff       (20)    14284 2023-02-22 12:33:47.000000 simfin-0.9.2/simfin/resample.py
+-rw-r--r--   0 thomasflassbeck   (501) staff       (20)    37350 2023-02-22 12:33:47.000000 simfin-0.9.2/simfin/signals.py
+-rw-r--r--   0 thomasflassbeck   (501) staff       (20)    14331 2023-02-22 12:33:47.000000 simfin-0.9.2/simfin/transform.py
+-rw-r--r--   0 thomasflassbeck   (501) staff       (20)    15933 2023-04-13 14:10:11.000000 simfin-0.9.2/simfin/utils.py
+drwxr-xr-x   0 thomasflassbeck   (501) staff       (20)        0 2023-06-13 19:21:31.897709 simfin-0.9.2/simfin.egg-info/
+-rw-r--r--   0 thomasflassbeck   (501) staff       (20)      570 2023-06-13 19:21:31.000000 simfin-0.9.2/simfin.egg-info/PKG-INFO
+-rw-r--r--   0 thomasflassbeck   (501) staff       (20)      521 2023-06-13 19:21:31.000000 simfin-0.9.2/simfin.egg-info/SOURCES.txt
+-rw-r--r--   0 thomasflassbeck   (501) staff       (20)        1 2023-06-13 19:21:31.000000 simfin-0.9.2/simfin.egg-info/dependency_links.txt
+-rw-r--r--   0 thomasflassbeck   (501) staff       (20)       22 2023-06-13 19:21:31.000000 simfin-0.9.2/simfin.egg-info/requires.txt
+-rw-r--r--   0 thomasflassbeck   (501) staff       (20)        7 2023-06-13 19:21:31.000000 simfin-0.9.2/simfin.egg-info/top_level.txt
```

### Comparing `simfin-0.9.1/LICENSE.txt` & `simfin-0.9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `simfin-0.9.1/PKG-INFO` & `simfin-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simfin
-Version: 0.9.1
+Version: 0.9.2
 Summary: Simple financial data for Python
 Home-page: https://github.com/simfin/simfin
 Author: SimFin
 Author-email: info@simfin.com
 License: MIT
 Keywords: financial data,finance
 Description-Content-Type: text/markdown
```

### Comparing `simfin-0.9.1/README.md` & `simfin-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `simfin-0.9.1/setup.py` & `simfin-0.9.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 # This is also defined in simfin/__init__.py and must be
 # updated in both places.
-MY_VERSION = '0.9.1'
+MY_VERSION = '0.9.2'
 
 setup(
     name='simfin',
     packages=['simfin'],
     version=MY_VERSION,
     description='Simple financial data for Python',
     long_description='SimFin makes it easy to obtain and use financial and '
```

### Comparing `simfin-0.9.1/simfin/__init__.py` & `simfin-0.9.2/simfin/__init__.py`

 * *Files identical despite different names*

### Comparing `simfin-0.9.1/simfin/cache.py` & `simfin-0.9.2/simfin/cache.py`

 * *Files identical despite different names*

### Comparing `simfin-0.9.1/simfin/config.py` & `simfin-0.9.2/simfin/config.py`

 * *Files identical despite different names*

### Comparing `simfin-0.9.1/simfin/datasets.py` & `simfin-0.9.2/simfin/datasets.py`

 * *Files identical despite different names*

### Comparing `simfin-0.9.1/simfin/derived.py` & `simfin-0.9.2/simfin/derived.py`

 * *Files identical despite different names*

### Comparing `simfin-0.9.1/simfin/download.py` & `simfin-0.9.2/simfin/download.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         args += '&variant=' + variant
 
     # Market.
     if market is not None:
         args += '&market=' + market
 
     # Base URL for the bulk-download API on the SimFin server.
-    base_url = 'https://backend.simfin.com/api/bulk-download?'
+    base_url = 'https://bulk-download.simfin.com/api/bulk-download?'
     # Combine base URL and arguments.
     url = base_url + args
 
     return url
 
 
 def _url_info(name):
```

### Comparing `simfin-0.9.1/simfin/exceptions.py` & `simfin-0.9.2/simfin/exceptions.py`

 * *Files identical despite different names*

### Comparing `simfin-0.9.1/simfin/hubs.py` & `simfin-0.9.2/simfin/hubs.py`

 * *Files identical despite different names*

### Comparing `simfin-0.9.1/simfin/info.py` & `simfin-0.9.2/simfin/info.py`

 * *Files identical despite different names*

### Comparing `simfin-0.9.1/simfin/load.py` & `simfin-0.9.2/simfin/load.py`

 * *Files identical despite different names*

### Comparing `simfin-0.9.1/simfin/load_info.py` & `simfin-0.9.2/simfin/load_info.py`

 * *Files identical despite different names*

### Comparing `simfin-0.9.1/simfin/names.py` & `simfin-0.9.2/simfin/names.py`

 * *Files identical despite different names*

### Comparing `simfin-0.9.1/simfin/names_extra.py` & `simfin-0.9.2/simfin/names_extra.py`

 * *Files identical despite different names*

### Comparing `simfin-0.9.1/simfin/paths.py` & `simfin-0.9.2/simfin/paths.py`

 * *Files identical despite different names*

### Comparing `simfin-0.9.1/simfin/rel_change.py` & `simfin-0.9.2/simfin/rel_change.py`

 * *Files identical despite different names*

### Comparing `simfin-0.9.1/simfin/resample.py` & `simfin-0.9.2/simfin/resample.py`

 * *Files identical despite different names*

### Comparing `simfin-0.9.1/simfin/signals.py` & `simfin-0.9.2/simfin/signals.py`

 * *Files identical despite different names*

### Comparing `simfin-0.9.1/simfin/transform.py` & `simfin-0.9.2/simfin/transform.py`

 * *Files identical despite different names*

### Comparing `simfin-0.9.1/simfin/utils.py` & `simfin-0.9.2/simfin/utils.py`

 * *Files identical despite different names*

### Comparing `simfin-0.9.1/simfin.egg-info/PKG-INFO` & `simfin-0.9.2/simfin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simfin
-Version: 0.9.1
+Version: 0.9.2
 Summary: Simple financial data for Python
 Home-page: https://github.com/simfin/simfin
 Author: SimFin
 Author-email: info@simfin.com
 License: MIT
 Keywords: financial data,finance
 Description-Content-Type: text/markdown
```

### Comparing `simfin-0.9.1/simfin.egg-info/SOURCES.txt` & `simfin-0.9.2/simfin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

