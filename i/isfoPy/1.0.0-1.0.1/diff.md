# Comparing `tmp/isfoPy-1.0.0.tar.gz` & `tmp/isfoPy-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isfoPy-1.0.0.tar", last modified: Tue Jun 13 18:20:37 2023, max compression
+gzip compressed data, was "isfoPy-1.0.1.tar", last modified: Tue Jun 13 18:58:06 2023, max compression
```

## Comparing `isfoPy-1.0.0.tar` & `isfoPy-1.0.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 18:20:37.387868 isfoPy-1.0.0/
--rw-rw-rw-   0        0        0      575 2023-06-13 18:20:37.387868 isfoPy-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-13 18:20:37.331678 isfoPy-1.0.0/isfoPy/
--rw-rw-rw-   0        0        0     6212 2023-06-13 18:11:11.000000 isfoPy-1.0.0/isfoPy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 18:20:37.387868 isfoPy-1.0.0/isfoPy.egg-info/
--rw-rw-rw-   0        0        0      575 2023-06-13 18:20:37.000000 isfoPy-1.0.0/isfoPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      147 2023-06-13 18:20:37.000000 isfoPy-1.0.0/isfoPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 18:20:37.000000 isfoPy-1.0.0/isfoPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-13 18:20:37.000000 isfoPy-1.0.0/isfoPy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-13 18:20:37.387868 isfoPy-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      674 2023-06-13 18:18:10.000000 isfoPy-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 18:58:06.685383 isfoPy-1.0.1/
+-rw-rw-rw-   0        0        0      575 2023-06-13 18:58:06.677346 isfoPy-1.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-13 18:58:06.653383 isfoPy-1.0.1/isfoPy/
+-rw-rw-rw-   0        0        0    11592 2023-06-13 18:53:42.000000 isfoPy-1.0.1/isfoPy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 18:58:06.677346 isfoPy-1.0.1/isfoPy.egg-info/
+-rw-rw-rw-   0        0        0      575 2023-06-13 18:58:06.000000 isfoPy-1.0.1/isfoPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      147 2023-06-13 18:58:06.000000 isfoPy-1.0.1/isfoPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 18:58:06.000000 isfoPy-1.0.1/isfoPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-13 18:58:06.000000 isfoPy-1.0.1/isfoPy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-13 18:58:06.685383 isfoPy-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      674 2023-06-13 18:46:59.000000 isfoPy-1.0.1/setup.py
```

### Comparing `isfoPy-1.0.0/PKG-INFO` & `isfoPy-1.0.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isfoPy
-Version: 1.0.0
+Version: 1.0.1
 Summary: an all in one library for gui application creation
 Author: Aland Salam
 Author-email: isfoedu@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `isfoPy-1.0.0/isfoPy.egg-info/PKG-INFO` & `isfoPy-1.0.1/isfoPy.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isfoPy
-Version: 1.0.0
+Version: 1.0.1
 Summary: an all in one library for gui application creation
 Author: Aland Salam
 Author-email: isfoedu@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `isfoPy-1.0.0/setup.py` & `isfoPy-1.0.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='isfoPy',
-    version='1.0.0',
+    version='1.0.1',
     description='an all in one library for gui application creation',
     author='Aland Salam',
     author_email='isfoedu@gmail.com',
     packages=['isfoPy'],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
```

