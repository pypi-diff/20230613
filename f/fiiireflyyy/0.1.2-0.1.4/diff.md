# Comparing `tmp/fiiireflyyy-0.1.2.tar.gz` & `tmp/fiiireflyyy-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fiiireflyyy-0.1.2.tar", last modified: Tue Jun 13 12:17:05 2023, max compression
+gzip compressed data, was "fiiireflyyy-0.1.4.tar", last modified: Tue Jun 13 13:02:42 2023, max compression
```

## Comparing `fiiireflyyy-0.1.2.tar` & `fiiireflyyy-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 12:17:05.458712 fiiireflyyy-0.1.2/
--rw-rw-rw-   0        0        0      669 2023-06-13 12:17:05.459711 fiiireflyyy-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     6290 2023-06-13 09:58:55.000000 fiiireflyyy-0.1.2/README.txt
-drwxrwxrwx   0        0        0        0 2023-06-13 12:17:05.453710 fiiireflyyy-0.1.2/fiiireflyyy/
--rw-rw-rw-   0        0        0      153 2023-06-13 12:11:31.000000 fiiireflyyy-0.1.2/fiiireflyyy/__init__.py
--rw-rw-rw-   0        0        0     4312 2023-06-13 09:58:55.000000 fiiireflyyy-0.1.2/fiiireflyyy/firefiles.py
--rw-rw-rw-   0        0        0    51273 2023-06-13 09:58:55.000000 fiiireflyyy-0.1.2/fiiireflyyy/firelearn.py
--rw-rw-rw-   0        0        0    14713 2023-06-13 09:58:55.000000 fiiireflyyy-0.1.2/fiiireflyyy/fireprocess.py
--rw-rw-rw-   0        0        0    15817 2023-06-13 09:58:55.000000 fiiireflyyy-0.1.2/fiiireflyyy/flimage.py
--rw-rw-rw-   0        0        0      649 2023-06-13 12:15:44.000000 fiiireflyyy-0.1.2/fiiireflyyy/logic_gates.py
-drwxrwxrwx   0        0        0        0 2023-06-13 12:17:05.458712 fiiireflyyy-0.1.2/fiiireflyyy.egg-info/
--rw-rw-rw-   0        0        0      669 2023-06-13 12:17:05.000000 fiiireflyyy-0.1.2/fiiireflyyy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      354 2023-06-13 12:17:05.000000 fiiireflyyy-0.1.2/fiiireflyyy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 12:17:05.000000 fiiireflyyy-0.1.2/fiiireflyyy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      116 2023-06-13 12:17:05.000000 fiiireflyyy-0.1.2/fiiireflyyy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-13 12:17:05.000000 fiiireflyyy-0.1.2/fiiireflyyy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-13 12:17:05.462712 fiiireflyyy-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1113 2023-06-13 12:06:42.000000 fiiireflyyy-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 13:02:42.059917 fiiireflyyy-0.1.4/
+-rw-rw-rw-   0        0        0      669 2023-06-13 13:02:42.059917 fiiireflyyy-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     6290 2023-06-13 09:58:55.000000 fiiireflyyy-0.1.4/README.txt
+drwxrwxrwx   0        0        0        0 2023-06-13 13:02:42.054916 fiiireflyyy-0.1.4/fiiireflyyy/
+-rw-rw-rw-   0        0        0      153 2023-06-13 12:11:31.000000 fiiireflyyy-0.1.4/fiiireflyyy/__init__.py
+-rw-rw-rw-   0        0        0     4312 2023-06-13 09:58:55.000000 fiiireflyyy-0.1.4/fiiireflyyy/firefiles.py
+-rw-rw-rw-   0        0        0    51273 2023-06-13 09:58:55.000000 fiiireflyyy-0.1.4/fiiireflyyy/firelearn.py
+-rw-rw-rw-   0        0        0    14713 2023-06-13 09:58:55.000000 fiiireflyyy-0.1.4/fiiireflyyy/fireprocess.py
+-rw-rw-rw-   0        0        0    15817 2023-06-13 09:58:55.000000 fiiireflyyy-0.1.4/fiiireflyyy/flimage.py
+-rw-rw-rw-   0        0        0      649 2023-06-13 12:15:44.000000 fiiireflyyy-0.1.4/fiiireflyyy/logic_gates.py
+drwxrwxrwx   0        0        0        0 2023-06-13 13:02:42.058917 fiiireflyyy-0.1.4/fiiireflyyy.egg-info/
+-rw-rw-rw-   0        0        0      669 2023-06-13 13:02:41.000000 fiiireflyyy-0.1.4/fiiireflyyy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      354 2023-06-13 13:02:42.000000 fiiireflyyy-0.1.4/fiiireflyyy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 13:02:41.000000 fiiireflyyy-0.1.4/fiiireflyyy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      116 2023-06-13 13:02:41.000000 fiiireflyyy-0.1.4/fiiireflyyy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-13 13:02:41.000000 fiiireflyyy-0.1.4/fiiireflyyy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-13 13:02:42.063918 fiiireflyyy-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1113 2023-06-13 13:01:52.000000 fiiireflyyy-0.1.4/setup.py
```

### Comparing `fiiireflyyy-0.1.2/PKG-INFO` & `fiiireflyyy-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiiireflyyy
-Version: 0.1.2
+Version: 0.1.4
 Summary: A python package covering miscellaneous uses, from system management to machine learning and image or data processing. Developed for personal uses.
 Author: fiiireflyyy (Willy Lutz)
 Author-email: <lutz0willy@gmail.com>
 Keywords: python,machine learning,deep learning,data analysis,system management,data processing
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fiiireflyyy-0.1.2/README.txt` & `fiiireflyyy-0.1.4/README.txt`

 * *Files identical despite different names*

### Comparing `fiiireflyyy-0.1.2/fiiireflyyy/firefiles.py` & `fiiireflyyy-0.1.4/fiiireflyyy/firefiles.py`

 * *Files identical despite different names*

### Comparing `fiiireflyyy-0.1.2/fiiireflyyy/firelearn.py` & `fiiireflyyy-0.1.4/fiiireflyyy/firelearn.py`

 * *Files identical despite different names*

### Comparing `fiiireflyyy-0.1.2/fiiireflyyy/fireprocess.py` & `fiiireflyyy-0.1.4/fiiireflyyy/fireprocess.py`

 * *Files identical despite different names*

### Comparing `fiiireflyyy-0.1.2/fiiireflyyy/flimage.py` & `fiiireflyyy-0.1.4/fiiireflyyy/flimage.py`

 * *Files identical despite different names*

### Comparing `fiiireflyyy-0.1.2/fiiireflyyy/logic_gates.py` & `fiiireflyyy-0.1.4/fiiireflyyy/logic_gates.py`

 * *Files identical despite different names*

### Comparing `fiiireflyyy-0.1.2/fiiireflyyy.egg-info/PKG-INFO` & `fiiireflyyy-0.1.4/fiiireflyyy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiiireflyyy
-Version: 0.1.2
+Version: 0.1.4
 Summary: A python package covering miscellaneous uses, from system management to machine learning and image or data processing. Developed for personal uses.
 Author: fiiireflyyy (Willy Lutz)
 Author-email: <lutz0willy@gmail.com>
 Keywords: python,machine learning,deep learning,data analysis,system management,data processing
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fiiireflyyy-0.1.2/setup.py` & `fiiireflyyy-0.1.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.1.2'
+VERSION = '0.1.4'
 DESCRIPTION = 'A python package covering miscellaneous uses, from system management to machine learning and image or' \
               ' data processing. Developed for personal uses.'
 
 # Setting up
 setup(
     name="fiiireflyyy",
     version=VERSION,
```

