# Comparing `tmp/gli99-1.1.5.tar.gz` & `tmp/gli99-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gli99-1.1.5.tar", last modified: Fri Mar 10 19:13:27 2023, max compression
+gzip compressed data, was "gli99-1.1.6.tar", last modified: Tue Jun 13 18:41:06 2023, max compression
```

## Comparing `gli99-1.1.5.tar` & `gli99-1.1.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-03-10 19:13:27.146415 gli99-1.1.5/
--rw-rw-rw-   0        0        0     1085 2023-03-04 20:16:16.000000 gli99-1.1.5/LICENSE.txt
--rw-rw-rw-   0        0        0       24 2023-03-07 22:58:15.000000 gli99-1.1.5/MANIFEST.in
--rw-rw-rw-   0        0        0      791 2023-03-10 19:13:27.145457 gli99-1.1.5/PKG-INFO
--rw-rw-rw-   0        0        0      302 2023-03-10 19:13:25.000000 gli99-1.1.5/README.md
--rw-rw-rw-   0        0        0       42 2023-03-10 19:13:27.147412 gli99-1.1.5/setup.cfg
--rw-rw-rw-   0        0        0      881 2023-03-10 19:13:18.000000 gli99-1.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-10 19:13:27.084983 gli99-1.1.5/src/
-drwxrwxrwx   0        0        0        0 2023-03-10 19:13:27.107924 gli99-1.1.5/src/gli99/
--rw-rw-rw-   0        0        0        0 2023-03-06 23:39:49.000000 gli99-1.1.5/src/gli99/__init__.py
--rw-rw-rw-   0        0        0     2096 2023-03-09 03:29:00.000000 gli99-1.1.5/src/gli99/browser_options.json
--rw-rw-rw-   0        0        0     4892 2023-03-10 18:03:13.000000 gli99-1.1.5/src/gli99/tools.py
-drwxrwxrwx   0        0        0        0 2023-03-10 19:13:27.141726 gli99-1.1.5/src/gli99.egg-info/
--rw-rw-rw-   0        0        0      791 2023-03-10 19:13:26.000000 gli99-1.1.5/src/gli99.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      278 2023-03-10 19:13:26.000000 gli99-1.1.5/src/gli99.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-10 19:13:26.000000 gli99-1.1.5/src/gli99.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-03-10 19:13:26.000000 gli99-1.1.5/src/gli99.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-03-10 19:13:26.000000 gli99-1.1.5/src/gli99.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-13 18:41:06.261517 gli99-1.1.6/
+-rw-rw-rw-   0        0        0     1085 2023-03-04 20:16:16.000000 gli99-1.1.6/LICENSE.txt
+-rw-rw-rw-   0        0        0       24 2023-03-07 22:58:15.000000 gli99-1.1.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     1082 2023-06-13 18:41:06.261517 gli99-1.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0      593 2023-06-13 18:41:05.000000 gli99-1.1.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-13 18:41:06.262518 gli99-1.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      881 2023-06-13 18:40:58.000000 gli99-1.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 18:41:06.235669 gli99-1.1.6/src/
+drwxrwxrwx   0        0        0        0 2023-06-13 18:41:06.243650 gli99-1.1.6/src/gli99/
+-rw-rw-rw-   0        0        0        0 2023-03-06 23:39:49.000000 gli99-1.1.6/src/gli99/__init__.py
+-rw-rw-rw-   0        0        0     2096 2023-03-09 03:29:00.000000 gli99-1.1.6/src/gli99/browser_options.json
+-rw-rw-rw-   0        0        0     4892 2023-03-10 19:25:37.000000 gli99-1.1.6/src/gli99/tools.py
+drwxrwxrwx   0        0        0        0 2023-06-13 18:41:06.259611 gli99-1.1.6/src/gli99.egg-info/
+-rw-rw-rw-   0        0        0     1082 2023-06-13 18:41:06.000000 gli99-1.1.6/src/gli99.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      278 2023-06-13 18:41:06.000000 gli99-1.1.6/src/gli99.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 18:41:06.000000 gli99-1.1.6/src/gli99.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-06-13 18:41:06.000000 gli99-1.1.6/src/gli99.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-13 18:41:06.000000 gli99-1.1.6/src/gli99.egg-info/top_level.txt
```

### Comparing `gli99-1.1.5/LICENSE.txt` & `gli99-1.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gli99-1.1.5/setup.py` & `gli99-1.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="gli99",
-    version='1.1.5',
+    version='1.1.6',
     description="Web scraper for gifcities.org",
     package_dir={'':'src'},
     packages=setuptools.find_packages(where="src"),
     include_package_data=True,
     python_requires=">3.10.0",
     classifiers=[
         "Programming Language :: Python",
```

### Comparing `gli99-1.1.5/src/gli99/browser_options.json` & `gli99-1.1.6/src/gli99/browser_options.json`

 * *Files identical despite different names*

### Comparing `gli99-1.1.5/src/gli99/tools.py` & `gli99-1.1.6/src/gli99/tools.py`

 * *Files identical despite different names*

