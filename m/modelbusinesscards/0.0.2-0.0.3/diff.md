# Comparing `tmp/modelbusinesscards-0.0.2.tar.gz` & `tmp/modelbusinesscards-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelbusinesscards-0.0.2.tar", last modified: Tue Jun 13 17:20:54 2023, max compression
+gzip compressed data, was "modelbusinesscards-0.0.3.tar", last modified: Tue Jun 13 17:26:13 2023, max compression
```

## Comparing `modelbusinesscards-0.0.2.tar` & `modelbusinesscards-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 upsolver   (501) staff       (20)        0 2023-06-13 17:20:54.176463 modelbusinesscards-0.0.2/
--rw-r--r--   0 upsolver   (501) staff       (20)     1067 2023-06-13 17:07:56.000000 modelbusinesscards-0.0.2/LICENSE
--rw-r--r--   0 upsolver   (501) staff       (20)      247 2023-06-13 17:20:54.176113 modelbusinesscards-0.0.2/PKG-INFO
--rw-r--r--   0 upsolver   (501) staff       (20)     4697 2023-06-13 17:19:04.000000 modelbusinesscards-0.0.2/README.md
--rw-r--r--   0 upsolver   (501) staff       (20)       38 2023-06-13 17:20:54.176591 modelbusinesscards-0.0.2/setup.cfg
--rw-r--r--   0 upsolver   (501) staff       (20)      625 2023-06-13 17:20:10.000000 modelbusinesscards-0.0.2/setup.py
-drwxr-xr-x   0 upsolver   (501) staff       (20)        0 2023-06-13 17:20:54.170421 modelbusinesscards-0.0.2/src/
-drwxr-xr-x   0 upsolver   (501) staff       (20)        0 2023-06-13 17:20:54.173897 modelbusinesscards-0.0.2/src/modelbusinesscards/
--rw-r--r--   0 upsolver   (501) staff       (20)       48 2023-06-09 22:06:30.000000 modelbusinesscards-0.0.2/src/modelbusinesscards/__init__.py
--rw-r--r--   0 upsolver   (501) staff       (20)      198 2023-06-10 01:15:47.000000 modelbusinesscards-0.0.2/src/modelbusinesscards/__main__.py
--rw-r--r--   0 upsolver   (501) staff       (20)      549 2023-06-09 22:06:51.000000 modelbusinesscards-0.0.2/src/modelbusinesscards/entities.py
--rw-r--r--   0 upsolver   (501) staff       (20)     1200 2023-06-10 01:13:37.000000 modelbusinesscards-0.0.2/src/modelbusinesscards/main.py
--rw-r--r--   0 upsolver   (501) staff       (20)     3721 2023-06-10 01:38:59.000000 modelbusinesscards-0.0.2/src/modelbusinesscards/parser.py
--rw-r--r--   0 upsolver   (501) staff       (20)     2000 2023-06-10 02:27:24.000000 modelbusinesscards-0.0.2/src/modelbusinesscards/writer.py
-drwxr-xr-x   0 upsolver   (501) staff       (20)        0 2023-06-13 17:20:54.175737 modelbusinesscards-0.0.2/src/modelbusinesscards.egg-info/
--rw-r--r--   0 upsolver   (501) staff       (20)      247 2023-06-13 17:20:54.000000 modelbusinesscards-0.0.2/src/modelbusinesscards.egg-info/PKG-INFO
--rw-r--r--   0 upsolver   (501) staff       (20)      457 2023-06-13 17:20:54.000000 modelbusinesscards-0.0.2/src/modelbusinesscards.egg-info/SOURCES.txt
--rw-r--r--   0 upsolver   (501) staff       (20)        1 2023-06-13 17:20:54.000000 modelbusinesscards-0.0.2/src/modelbusinesscards.egg-info/dependency_links.txt
--rw-r--r--   0 upsolver   (501) staff       (20)        1 2023-06-10 00:57:20.000000 modelbusinesscards-0.0.2/src/modelbusinesscards.egg-info/not-zip-safe
--rw-r--r--   0 upsolver   (501) staff       (20)       19 2023-06-13 17:20:54.000000 modelbusinesscards-0.0.2/src/modelbusinesscards.egg-info/top_level.txt
+drwxr-xr-x   0 upsolver   (501) staff       (20)        0 2023-06-13 17:26:13.652699 modelbusinesscards-0.0.3/
+-rw-r--r--   0 upsolver   (501) staff       (20)     1067 2023-06-13 17:07:56.000000 modelbusinesscards-0.0.3/LICENSE
+-rw-r--r--   0 upsolver   (501) staff       (20)       15 2023-06-13 17:25:03.000000 modelbusinesscards-0.0.3/MANIFEST.in
+-rw-r--r--   0 upsolver   (501) staff       (20)      247 2023-06-13 17:26:13.652154 modelbusinesscards-0.0.3/PKG-INFO
+-rw-r--r--   0 upsolver   (501) staff       (20)     4697 2023-06-13 17:19:04.000000 modelbusinesscards-0.0.3/README.md
+-rw-r--r--   0 upsolver   (501) staff       (20)       38 2023-06-13 17:26:13.652837 modelbusinesscards-0.0.3/setup.cfg
+-rw-r--r--   0 upsolver   (501) staff       (20)      656 2023-06-13 17:26:03.000000 modelbusinesscards-0.0.3/setup.py
+drwxr-xr-x   0 upsolver   (501) staff       (20)        0 2023-06-13 17:26:13.644277 modelbusinesscards-0.0.3/src/
+drwxr-xr-x   0 upsolver   (501) staff       (20)        0 2023-06-13 17:26:13.648884 modelbusinesscards-0.0.3/src/modelbusinesscards/
+-rw-r--r--   0 upsolver   (501) staff       (20)       48 2023-06-09 22:06:30.000000 modelbusinesscards-0.0.3/src/modelbusinesscards/__init__.py
+-rw-r--r--   0 upsolver   (501) staff       (20)      198 2023-06-10 01:15:47.000000 modelbusinesscards-0.0.3/src/modelbusinesscards/__main__.py
+-rw-r--r--   0 upsolver   (501) staff       (20)      549 2023-06-09 22:06:51.000000 modelbusinesscards-0.0.3/src/modelbusinesscards/entities.py
+-rw-r--r--   0 upsolver   (501) staff       (20)     1200 2023-06-10 01:13:37.000000 modelbusinesscards-0.0.3/src/modelbusinesscards/main.py
+-rw-r--r--   0 upsolver   (501) staff       (20)     3721 2023-06-10 01:38:59.000000 modelbusinesscards-0.0.3/src/modelbusinesscards/parser.py
+-rw-r--r--   0 upsolver   (501) staff       (20)     2000 2023-06-10 02:27:24.000000 modelbusinesscards-0.0.3/src/modelbusinesscards/writer.py
+drwxr-xr-x   0 upsolver   (501) staff       (20)        0 2023-06-13 17:26:13.651362 modelbusinesscards-0.0.3/src/modelbusinesscards.egg-info/
+-rw-r--r--   0 upsolver   (501) staff       (20)      247 2023-06-13 17:26:13.000000 modelbusinesscards-0.0.3/src/modelbusinesscards.egg-info/PKG-INFO
+-rw-r--r--   0 upsolver   (501) staff       (20)      469 2023-06-13 17:26:13.000000 modelbusinesscards-0.0.3/src/modelbusinesscards.egg-info/SOURCES.txt
+-rw-r--r--   0 upsolver   (501) staff       (20)        1 2023-06-13 17:26:13.000000 modelbusinesscards-0.0.3/src/modelbusinesscards.egg-info/dependency_links.txt
+-rw-r--r--   0 upsolver   (501) staff       (20)        1 2023-06-10 00:57:20.000000 modelbusinesscards-0.0.3/src/modelbusinesscards.egg-info/not-zip-safe
+-rw-r--r--   0 upsolver   (501) staff       (20)       19 2023-06-13 17:26:13.000000 modelbusinesscards-0.0.3/src/modelbusinesscards.egg-info/top_level.txt
```

### Comparing `modelbusinesscards-0.0.2/LICENSE` & `modelbusinesscards-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `modelbusinesscards-0.0.2/README.md` & `modelbusinesscards-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `modelbusinesscards-0.0.2/setup.py` & `modelbusinesscards-0.0.3/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from setuptools import setup, find_packages
 
 # package info/config (use "pip install -e ." to instal locally for dev)
 setup(
     name='modelbusinesscards',
-    version='0.0.2',
+    version='0.0.3',
     description='Generating documentation of AI model usage to increase visibility and safety',
     url='https://github.com/youmustfight/model-business-cards',
     package_dir={ '': 'src' }, # This tells setuptools to look for packages in the 'src' directory.
     packages=find_packages(where='src'), # find_packages() will find packages in the 'src' directory because of the above.
     install_requires=[],
+    include_package_data=True,
     license='MIT',
     zip_safe=False
 )
```

### Comparing `modelbusinesscards-0.0.2/src/modelbusinesscards/entities.py` & `modelbusinesscards-0.0.3/src/modelbusinesscards/entities.py`

 * *Files identical despite different names*

### Comparing `modelbusinesscards-0.0.2/src/modelbusinesscards/main.py` & `modelbusinesscards-0.0.3/src/modelbusinesscards/main.py`

 * *Files identical despite different names*

### Comparing `modelbusinesscards-0.0.2/src/modelbusinesscards/parser.py` & `modelbusinesscards-0.0.3/src/modelbusinesscards/parser.py`

 * *Files identical despite different names*

### Comparing `modelbusinesscards-0.0.2/src/modelbusinesscards/writer.py` & `modelbusinesscards-0.0.3/src/modelbusinesscards/writer.py`

 * *Files identical despite different names*

