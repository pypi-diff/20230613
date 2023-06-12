# Comparing `tmp/azdsdr-1.230505.2.tar.gz` & `tmp/azdsdr-1.230612.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azdsdr-1.230505.2.tar", last modified: Fri May  5 17:10:45 2023, max compression
+gzip compressed data, was "azdsdr-1.230612.2.tar", last modified: Mon Jun 12 22:01:36 2023, max compression
```

## Comparing `azdsdr-1.230505.2.tar` & `azdsdr-1.230612.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 17:10:45.370000 azdsdr-1.230505.2/
--rw-rw-rw-   0        0        0    12797 2023-05-05 17:10:46.000000 azdsdr-1.230505.2/PKG-INFO
--rw-rw-rw-   0        0        0    12457 2023-04-20 21:11:06.000000 azdsdr-1.230505.2/README.md
--rw-rw-rw-   0        0        0      198 2023-05-05 17:10:46.000000 azdsdr-1.230505.2/setup.cfg
--rw-rw-rw-   0        0        0      726 2023-05-05 17:10:34.000000 azdsdr-1.230505.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-05 17:10:45.510000 azdsdr-1.230505.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-05 17:10:45.520000 azdsdr-1.230505.2/src/azdsdr/
--rw-rw-rw-   0        0        0        0 2022-09-29 16:46:06.000000 azdsdr-1.230505.2/src/azdsdr/__init__.py
--rw-rw-rw-   0        0        0    35840 2023-03-04 19:26:56.000000 azdsdr-1.230505.2/src/azdsdr/readers.py
--rw-rw-rw-   0        0        0    10272 2023-05-05 17:10:26.000000 azdsdr-1.230505.2/src/azdsdr/tools.py
-drwxrwxrwx   0        0        0        0 2023-05-05 17:10:45.530000 azdsdr-1.230505.2/src/azdsdr.egg-info/
--rw-rw-rw-   0        0        0    12797 2023-05-05 17:10:46.000000 azdsdr-1.230505.2/src/azdsdr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      282 2023-05-05 17:10:46.000000 azdsdr-1.230505.2/src/azdsdr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 17:10:46.000000 azdsdr-1.230505.2/src/azdsdr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      125 2023-05-05 17:10:46.000000 azdsdr-1.230505.2/src/azdsdr.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-05 17:10:46.000000 azdsdr-1.230505.2/src/azdsdr.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-05 17:10:45.550000 azdsdr-1.230505.2/test/
--rw-rw-rw-   0        0        0    17848 2023-03-04 19:42:34.000000 azdsdr-1.230505.2/test/test.py
+drwxrwxrwx   0        0        0        0 2023-06-12 22:01:36.750000 azdsdr-1.230612.2/
+-rw-rw-rw-   0        0        0    12797 2023-06-12 22:01:38.000000 azdsdr-1.230612.2/PKG-INFO
+-rw-rw-rw-   0        0        0    12457 2023-04-20 21:11:06.000000 azdsdr-1.230612.2/README.md
+-rw-rw-rw-   0        0        0      198 2023-06-12 22:01:38.000000 azdsdr-1.230612.2/setup.cfg
+-rw-rw-rw-   0        0        0      726 2023-06-12 22:00:02.000000 azdsdr-1.230612.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 22:01:36.760000 azdsdr-1.230612.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-12 22:01:36.760000 azdsdr-1.230612.2/src/azdsdr/
+-rw-rw-rw-   0        0        0        0 2022-09-29 16:46:06.000000 azdsdr-1.230612.2/src/azdsdr/__init__.py
+-rw-rw-rw-   0        0        0    35845 2023-06-12 21:59:42.000000 azdsdr-1.230612.2/src/azdsdr/readers.py
+-rw-rw-rw-   0        0        0    10272 2023-05-05 17:10:26.000000 azdsdr-1.230612.2/src/azdsdr/tools.py
+drwxrwxrwx   0        0        0        0 2023-06-12 22:01:36.760000 azdsdr-1.230612.2/src/azdsdr.egg-info/
+-rw-rw-rw-   0        0        0    12797 2023-06-12 22:01:38.000000 azdsdr-1.230612.2/src/azdsdr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2023-06-12 22:01:38.000000 azdsdr-1.230612.2/src/azdsdr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 22:01:38.000000 azdsdr-1.230612.2/src/azdsdr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      125 2023-06-12 22:01:38.000000 azdsdr-1.230612.2/src/azdsdr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-12 22:01:38.000000 azdsdr-1.230612.2/src/azdsdr.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-12 22:01:36.760000 azdsdr-1.230612.2/test/
+-rw-rw-rw-   0        0        0    17848 2023-03-04 19:42:34.000000 azdsdr-1.230612.2/test/test.py
```

### Comparing `azdsdr-1.230505.2/PKG-INFO` & `azdsdr-1.230612.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azdsdr
-Version: 1.230505.2
+Version: 1.230612.2
 Summary: This package provide functions and tools for accessing data in a easy way.
 Home-page: https://github.com/xhinker/azdsdr
 Author: Andrew Zhu
 Author-email: xhinker@hotmail.com
 License: Apache License
 Keywords: DS Data Reader
 Description-Content-Type: text/markdown
```

### Comparing `azdsdr-1.230505.2/README.md` & `azdsdr-1.230612.2/README.md`

 * *Files identical despite different names*

### Comparing `azdsdr-1.230505.2/setup.py` & `azdsdr-1.230612.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup,find_packages
 
 setup(
     name='azdsdr',
-    version='1.230505.2',
+    version='1.230612.2',
     license='Apache License',
     author="Andrew Zhu",
     author_email='xhinker@hotmail.com',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     url='https://github.com/xhinker/azdsdr',
     keywords='DS Data Reader',
```

### Comparing `azdsdr-1.230505.2/src/azdsdr/readers.py` & `azdsdr-1.230612.2/src/azdsdr/readers.py`

 * *Files 1% similar despite different names*

```diff
@@ -887,20 +887,20 @@
         except:
             print('get azure blob key and connection string error')
 
         # temp name for azure blob 
         temp_name = str(uuid.uuid4())
         
         kusto_head = f'''.export async to csv(
-            h@"https://{azure_blob_account}.blob.core.windows.net:443//{self.azure_blob_container}/azdsdr;{azure_blob_key}"
+            h@"https://{azure_blob_account}.blob.core.windows.net:443/{self.azure_blob_container}/azdsdr;{azure_blob_key}"
         ) with (
             sizeLimit        = 100000000
-            ,namePrefix      = {temp_name}
-            ,includeHeaders  = all
-            ,encoding        = UTF8NoBOM
+            ,namePrefix      = "{temp_name}"
+            ,includeHeaders  = "all"
+            ,encoding        = "UTF8NoBOM"
             ,distributed     = false
         )
         <|
         '''
 
         try:
             kql = f"""{kusto_head}{input_kql}"""
```

### Comparing `azdsdr-1.230505.2/src/azdsdr/tools.py` & `azdsdr-1.230612.2/src/azdsdr/tools.py`

 * *Files identical despite different names*

### Comparing `azdsdr-1.230505.2/src/azdsdr.egg-info/PKG-INFO` & `azdsdr-1.230612.2/src/azdsdr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azdsdr
-Version: 1.230505.2
+Version: 1.230612.2
 Summary: This package provide functions and tools for accessing data in a easy way.
 Home-page: https://github.com/xhinker/azdsdr
 Author: Andrew Zhu
 Author-email: xhinker@hotmail.com
 License: Apache License
 Keywords: DS Data Reader
 Description-Content-Type: text/markdown
```

### Comparing `azdsdr-1.230505.2/test/test.py` & `azdsdr-1.230612.2/test/test.py`

 * *Files identical despite different names*

