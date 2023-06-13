# Comparing `tmp/makaonion-0.0.2.tar.gz` & `tmp/makaonion-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "makaonion-0.0.2.tar", last modified: Tue Jun 13 03:45:25 2023, max compression
+gzip compressed data, was "makaonion-0.0.3.tar", last modified: Tue Jun 13 03:54:36 2023, max compression
```

## Comparing `makaonion-0.0.2.tar` & `makaonion-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-06-13 03:45:25.426489 makaonion-0.0.2/
--rwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)      104 2023-06-13 01:23:57.000000 makaonion-0.0.2/CHANGELOG.md
--rwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)     1065 2023-06-13 01:15:27.000000 makaonion-0.0.2/LICENCE.txt
--rwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)       31 2023-06-13 01:16:12.000000 makaonion-0.0.2/MANIFEST.in
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)      982 2023-06-13 03:45:25.426489 makaonion-0.0.2/PKG-INFO
--rwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)      363 2023-06-13 02:48:06.000000 makaonion-0.0.2/README.md
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)    15773 2023-06-13 03:17:52.000000 makaonion-0.0.2/__init__.py
-drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-06-13 03:45:25.426489 makaonion-0.0.2/makaonion.egg-info/
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)      982 2023-06-13 03:45:24.000000 makaonion-0.0.2/makaonion.egg-info/PKG-INFO
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)      267 2023-06-13 03:45:25.000000 makaonion-0.0.2/makaonion.egg-info/SOURCES.txt
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)        1 2023-06-13 03:45:24.000000 makaonion-0.0.2/makaonion.egg-info/dependency_links.txt
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       42 2023-06-13 03:45:24.000000 makaonion-0.0.2/makaonion.egg-info/entry_points.txt
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)        9 2023-06-13 03:45:24.000000 makaonion-0.0.2/makaonion.egg-info/requires.txt
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       10 2023-06-13 03:45:24.000000 makaonion-0.0.2/makaonion.egg-info/top_level.txt
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       38 2023-06-13 03:45:25.426489 makaonion-0.0.2/setup.cfg
--rwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)     1202 2023-06-13 03:45:04.000000 makaonion-0.0.2/setup.py
+drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-06-13 03:54:36.255886 makaonion-0.0.3/
+-rwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)      104 2023-06-13 01:23:57.000000 makaonion-0.0.3/CHANGELOG.md
+-rwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)     1065 2023-06-13 01:15:27.000000 makaonion-0.0.3/LICENCE.txt
+-rwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)       31 2023-06-13 01:16:12.000000 makaonion-0.0.3/MANIFEST.in
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)      982 2023-06-13 03:54:36.255886 makaonion-0.0.3/PKG-INFO
+-rwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)      363 2023-06-13 02:48:06.000000 makaonion-0.0.3/README.md
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)    15773 2023-06-13 03:17:52.000000 makaonion-0.0.3/__init__.py
+drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-06-13 03:54:36.255886 makaonion-0.0.3/makaonion.egg-info/
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)      982 2023-06-13 03:54:36.000000 makaonion-0.0.3/makaonion.egg-info/PKG-INFO
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)      280 2023-06-13 03:54:36.000000 makaonion-0.0.3/makaonion.egg-info/SOURCES.txt
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)        1 2023-06-13 03:54:36.000000 makaonion-0.0.3/makaonion.egg-info/dependency_links.txt
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       42 2023-06-13 03:54:36.000000 makaonion-0.0.3/makaonion.egg-info/entry_points.txt
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)        9 2023-06-13 03:54:36.000000 makaonion-0.0.3/makaonion.egg-info/requires.txt
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       10 2023-06-13 03:54:36.000000 makaonion-0.0.3/makaonion.egg-info/top_level.txt
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)    15773 2023-06-13 03:54:27.000000 makaonion-0.0.3/makaonion.py
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       38 2023-06-13 03:54:36.255886 makaonion-0.0.3/setup.cfg
+-rwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)     1202 2023-06-13 03:52:36.000000 makaonion-0.0.3/setup.py
```

### Comparing `makaonion-0.0.2/LICENCE.txt` & `makaonion-0.0.3/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `makaonion-0.0.2/PKG-INFO` & `makaonion-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: makaonion
-Version: 0.0.2
+Version: 0.0.3
 Summary: Dot-Onion Services Manager Client
 Author: Erasmus A. Junior
 Author-email: eirasmx@pm.me
 License: MIT
 Keywords: tor,hosting,onion,hidden,services
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `makaonion-0.0.2/__init__.py` & `makaonion-0.0.3/__init__.py`

 * *Files identical despite different names*

### Comparing `makaonion-0.0.2/makaonion.egg-info/PKG-INFO` & `makaonion-0.0.3/makaonion.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: makaonion
-Version: 0.0.2
+Version: 0.0.3
 Summary: Dot-Onion Services Manager Client
 Author: Erasmus A. Junior
 Author-email: eirasmx@pm.me
 License: MIT
 Keywords: tor,hosting,onion,hidden,services
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `makaonion-0.0.2/setup.py` & `makaonion-0.0.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as readme:
     with codecs.open(os.path.join(here, "CHANGELOG.md"), encoding="utf-8") as changelog:
         LONG_DESCRIPTION = readme.read() + '\n\n\n' + changelog.read()
 
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'Dot-Onion Services Manager Client'
 KEYWORDS = ['tor', 'hosting', 'onion', 'hidden', 'services']
 
 
 CLASSIFIERS = [
     'Development Status :: 3 - Alpha',
     'Environment :: Console',
```

