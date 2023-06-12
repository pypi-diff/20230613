# Comparing `tmp/mlplatformutils-0.9.5.5.tar.gz` & `tmp/mlplatformutils-0.9.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mlplatformutils-0.9.5.5.tar", last modified: Mon Jun 12 23:17:47 2023, max compression
+gzip compressed data, was "dist\mlplatformutils-0.9.5.6.tar", last modified: Mon Jun 12 23:43:46 2023, max compression
```

## Comparing `mlplatformutils-0.9.5.5.tar` & `mlplatformutils-0.9.5.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 23:17:47.606733 mlplatformutils-0.9.5.5/
--rw-rw-rw-   0        0        0     6719 2023-06-12 23:17:47.607732 mlplatformutils-0.9.5.5/PKG-INFO
--rw-rw-rw-   0        0        0      420 2023-06-04 22:07:41.000000 mlplatformutils-0.9.5.5/README.rst
--rw-rw-rw-   0        0        0      115 2023-06-12 23:17:47.613729 mlplatformutils-0.9.5.5/setup.cfg
--rw-rw-rw-   0        0        0      825 2023-06-12 23:17:37.000000 mlplatformutils-0.9.5.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-12 23:17:47.421530 mlplatformutils-0.9.5.5/src/
-drwxrwxrwx   0        0        0        0 2023-06-12 23:17:47.444535 mlplatformutils-0.9.5.5/src/mlplatformutils/
--rw-rw-rw-   0        0        0        0 2023-06-04 21:52:02.000000 mlplatformutils-0.9.5.5/src/mlplatformutils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 23:17:47.602728 mlplatformutils-0.9.5.5/src/mlplatformutils/core/
--rw-rw-rw-   0        0        0        0 2023-06-03 20:39:09.000000 mlplatformutils-0.9.5.5/src/mlplatformutils/core/__init__.py
--rw-rw-rw-   0        0        0     5868 2023-06-03 20:42:19.000000 mlplatformutils-0.9.5.5/src/mlplatformutils/core/app_insights_logger.py
--rw-rw-rw-   0        0        0     1418 2023-06-12 20:54:48.000000 mlplatformutils-0.9.5.5/src/mlplatformutils/core/freshnessutils.py
--rw-rw-rw-   0        0        0    10096 2023-06-12 23:17:29.000000 mlplatformutils-0.9.5.5/src/mlplatformutils/core/lineagegraph.py
--rw-rw-rw-   0        0        0     6140 2023-06-08 20:01:59.000000 mlplatformutils-0.9.5.5/src/mlplatformutils/core/pandascoreutils.py
--rw-rw-rw-   0        0        0    12536 2023-06-10 01:10:09.000000 mlplatformutils-0.9.5.5/src/mlplatformutils/core/pandasutils.py
--rw-rw-rw-   0        0        0     3129 2023-06-04 21:06:24.000000 mlplatformutils-0.9.5.5/src/mlplatformutils/core/platformutils.py
--rw-rw-rw-   0        0        0     4675 2023-06-08 20:00:19.000000 mlplatformutils-0.9.5.5/src/mlplatformutils/core/sparkcoreutils.py
--rw-rw-rw-   0        0        0    10171 2023-06-10 01:11:28.000000 mlplatformutils-0.9.5.5/src/mlplatformutils/core/sparkutils.py
--rw-rw-rw-   0        0        0       23 2023-06-12 23:17:41.000000 mlplatformutils-0.9.5.5/src/mlplatformutils/core/version.py
-drwxrwxrwx   0        0        0        0 2023-06-12 23:17:47.501166 mlplatformutils-0.9.5.5/src/mlplatformutils.egg-info/
--rw-rw-rw-   0        0        0     6719 2023-06-12 23:17:47.000000 mlplatformutils-0.9.5.5/src/mlplatformutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      688 2023-06-12 23:17:47.000000 mlplatformutils-0.9.5.5/src/mlplatformutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 23:17:47.000000 mlplatformutils-0.9.5.5/src/mlplatformutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      103 2023-06-12 23:17:47.000000 mlplatformutils-0.9.5.5/src/mlplatformutils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-12 23:17:47.000000 mlplatformutils-0.9.5.5/src/mlplatformutils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-12 23:43:46.027120 mlplatformutils-0.9.5.6/
+-rw-rw-rw-   0        0        0     6719 2023-06-12 23:43:46.028120 mlplatformutils-0.9.5.6/PKG-INFO
+-rw-rw-rw-   0        0        0      420 2023-06-04 22:07:41.000000 mlplatformutils-0.9.5.6/README.rst
+-rw-rw-rw-   0        0        0      115 2023-06-12 23:43:46.036653 mlplatformutils-0.9.5.6/setup.cfg
+-rw-rw-rw-   0        0        0      825 2023-06-12 23:43:34.000000 mlplatformutils-0.9.5.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 23:43:45.591922 mlplatformutils-0.9.5.6/src/
+drwxrwxrwx   0        0        0        0 2023-06-12 23:43:45.639466 mlplatformutils-0.9.5.6/src/mlplatformutils/
+-rw-rw-rw-   0        0        0        0 2023-06-04 21:52:02.000000 mlplatformutils-0.9.5.6/src/mlplatformutils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 23:43:46.025119 mlplatformutils-0.9.5.6/src/mlplatformutils/core/
+-rw-rw-rw-   0        0        0        0 2023-06-03 20:39:09.000000 mlplatformutils-0.9.5.6/src/mlplatformutils/core/__init__.py
+-rw-rw-rw-   0        0        0     5868 2023-06-03 20:42:19.000000 mlplatformutils-0.9.5.6/src/mlplatformutils/core/app_insights_logger.py
+-rw-rw-rw-   0        0        0     1418 2023-06-12 20:54:48.000000 mlplatformutils-0.9.5.6/src/mlplatformutils/core/freshnessutils.py
+-rw-rw-rw-   0        0        0    10096 2023-06-12 23:17:29.000000 mlplatformutils-0.9.5.6/src/mlplatformutils/core/lineagegraph.py
+-rw-rw-rw-   0        0        0     6140 2023-06-08 20:01:59.000000 mlplatformutils-0.9.5.6/src/mlplatformutils/core/pandascoreutils.py
+-rw-rw-rw-   0        0        0    12539 2023-06-12 23:43:27.000000 mlplatformutils-0.9.5.6/src/mlplatformutils/core/pandasutils.py
+-rw-rw-rw-   0        0        0     3129 2023-06-04 21:06:24.000000 mlplatformutils-0.9.5.6/src/mlplatformutils/core/platformutils.py
+-rw-rw-rw-   0        0        0     4675 2023-06-08 20:00:19.000000 mlplatformutils-0.9.5.6/src/mlplatformutils/core/sparkcoreutils.py
+-rw-rw-rw-   0        0        0    10174 2023-06-12 23:42:09.000000 mlplatformutils-0.9.5.6/src/mlplatformutils/core/sparkutils.py
+-rw-rw-rw-   0        0        0       23 2023-06-12 23:43:37.000000 mlplatformutils-0.9.5.6/src/mlplatformutils/core/version.py
+drwxrwxrwx   0        0        0        0 2023-06-12 23:43:45.720479 mlplatformutils-0.9.5.6/src/mlplatformutils.egg-info/
+-rw-rw-rw-   0        0        0     6719 2023-06-12 23:43:45.000000 mlplatformutils-0.9.5.6/src/mlplatformutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      688 2023-06-12 23:43:45.000000 mlplatformutils-0.9.5.6/src/mlplatformutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 23:43:45.000000 mlplatformutils-0.9.5.6/src/mlplatformutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      103 2023-06-12 23:43:45.000000 mlplatformutils-0.9.5.6/src/mlplatformutils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-12 23:43:45.000000 mlplatformutils-0.9.5.6/src/mlplatformutils.egg-info/top_level.txt
```

### Comparing `mlplatformutils-0.9.5.5/PKG-INFO` & `mlplatformutils-0.9.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlplatformutils
-Version: 0.9.5.5
+Version: 0.9.5.6
 Author: Keshav Singh
 Author-email: keshav_singh@hotmail.com
 License: MIT
 Keywords: mlplatformutils
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
```

### Comparing `mlplatformutils-0.9.5.5/setup.py` & `mlplatformutils-0.9.5.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 else:
     long_description="#DESC"
 
 setup(
     name='mlplatformutils',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='0.9.5.5',
+    version='0.9.5.6',
     license='MIT',
     classifiers=[
         'Programming Language :: Python :: 3.8'
     ],
     author='Keshav Singh',
     author_email='keshav_singh@hotmail.com',
     packages=find_packages('src'),
```

### Comparing `mlplatformutils-0.9.5.5/src/mlplatformutils/core/app_insights_logger.py` & `mlplatformutils-0.9.5.6/src/mlplatformutils/core/app_insights_logger.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.9.5.5/src/mlplatformutils/core/freshnessutils.py` & `mlplatformutils-0.9.5.6/src/mlplatformutils/core/freshnessutils.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.9.5.5/src/mlplatformutils/core/lineagegraph.py` & `mlplatformutils-0.9.5.6/src/mlplatformutils/core/lineagegraph.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.9.5.5/src/mlplatformutils/core/pandascoreutils.py` & `mlplatformutils-0.9.5.6/src/mlplatformutils/core/pandascoreutils.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.9.5.5/src/mlplatformutils/core/pandasutils.py` & `mlplatformutils-0.9.5.6/src/mlplatformutils/core/pandasutils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 def get_max_properties_starting_with(id, prefix,dataprop,LineageLogger):
 
-    document=LineageLogger.query_graph("g.V().hasLabel('amlrun').has('id', '"+id+"')")
+    document=LineageLogger.query_graph("g.V().hasLabel('amlrun').has('id', '"+id+"')")[0]
     jsondump = json.dumps(document)
     jsonload = json.loads(jsondump)
     for item in jsonload:
         properties = item.get('properties')
     if properties:
         matching_props = [prop[-1] for prop in properties.keys() if prop.startswith(prefix)]
         max_val = max(int(prop) for prop in matching_props) if matching_props else 0
```

### Comparing `mlplatformutils-0.9.5.5/src/mlplatformutils/core/platformutils.py` & `mlplatformutils-0.9.5.6/src/mlplatformutils/core/platformutils.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.9.5.5/src/mlplatformutils/core/sparkcoreutils.py` & `mlplatformutils-0.9.5.6/src/mlplatformutils/core/sparkcoreutils.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.9.5.5/src/mlplatformutils/core/sparkutils.py` & `mlplatformutils-0.9.5.6/src/mlplatformutils/core/sparkutils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 def get_max_properties_starting_with(id, prefix,dataprop,LineageLogger):
 
-    document=LineageLogger.query_graph("g.V().hasLabel('amlrun').has('id', '"+id+"')")
+    document=LineageLogger.query_graph("g.V().hasLabel('amlrun').has('id', '"+id+"')")[0]
     jsondump = json.dumps(document)
     jsonload = json.loads(jsondump)
     for item in jsonload:
         properties = item.get('properties')
     if properties:
         matching_props = [prop[-1] for prop in properties.keys() if prop.startswith(prefix)]
         max_val = max(int(prop) for prop in matching_props) if matching_props else 0
```

### Comparing `mlplatformutils-0.9.5.5/src/mlplatformutils.egg-info/PKG-INFO` & `mlplatformutils-0.9.5.6/src/mlplatformutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlplatformutils
-Version: 0.9.5.5
+Version: 0.9.5.6
 Author: Keshav Singh
 Author-email: keshav_singh@hotmail.com
 License: MIT
 Keywords: mlplatformutils
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
```

### Comparing `mlplatformutils-0.9.5.5/src/mlplatformutils.egg-info/SOURCES.txt` & `mlplatformutils-0.9.5.6/src/mlplatformutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

