# Comparing `tmp/cyberfame-tools-2023.6.13b0.tar.gz` & `tmp/cyberfame-tools-2023.6.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyberfame-tools-2023.6.13b0.tar", last modified: Tue Jun 13 15:37:27 2023, max compression
+gzip compressed data, was "cyberfame-tools-2023.6.14.tar", last modified: Tue Jun 13 15:38:14 2023, max compression
```

## Comparing `cyberfame-tools-2023.6.13b0.tar` & `cyberfame-tools-2023.6.14.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 kittyandrew  (1000) kittyandrew  (1000)        0 2023-06-13 15:37:27.251161 cyberfame-tools-2023.6.13b0/
--rw-rw-r--   0 kittyandrew  (1000) kittyandrew  (1000)       39 2023-02-11 15:59:23.000000 cyberfame-tools-2023.6.13b0/MANIFEST.in
--rw-rw-r--   0 kittyandrew  (1000) kittyandrew  (1000)      654 2023-06-13 15:37:27.251161 cyberfame-tools-2023.6.13b0/PKG-INFO
--rw-rw-r--   0 kittyandrew  (1000) kittyandrew  (1000)      123 2023-02-16 16:35:41.000000 cyberfame-tools-2023.6.13b0/README.md
-drwxrwxr-x   0 kittyandrew  (1000) kittyandrew  (1000)        0 2023-06-13 15:37:27.247161 cyberfame-tools-2023.6.13b0/cyberfame_tools.egg-info/
--rw-rw-r--   0 kittyandrew  (1000) kittyandrew  (1000)      654 2023-06-13 15:37:27.000000 cyberfame-tools-2023.6.13b0/cyberfame_tools.egg-info/PKG-INFO
--rw-rw-r--   0 kittyandrew  (1000) kittyandrew  (1000)      387 2023-06-13 15:37:27.000000 cyberfame-tools-2023.6.13b0/cyberfame_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 kittyandrew  (1000) kittyandrew  (1000)        1 2023-06-13 15:37:27.000000 cyberfame-tools-2023.6.13b0/cyberfame_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 kittyandrew  (1000) kittyandrew  (1000)        8 2023-06-13 15:37:27.000000 cyberfame-tools-2023.6.13b0/cyberfame_tools.egg-info/requires.txt
--rw-rw-r--   0 kittyandrew  (1000) kittyandrew  (1000)       15 2023-06-13 15:37:27.000000 cyberfame-tools-2023.6.13b0/cyberfame_tools.egg-info/top_level.txt
-drwxrwxr-x   0 kittyandrew  (1000) kittyandrew  (1000)        0 2023-06-13 15:37:27.247161 cyberfame-tools-2023.6.13b0/cyberfametools/
--rw-rw-r--   0 kittyandrew  (1000) kittyandrew  (1000)      180 2023-06-13 15:23:20.000000 cyberfame-tools-2023.6.13b0/cyberfametools/__init__.py
--rw-rw-r--   0 kittyandrew  (1000) kittyandrew  (1000)      729 2023-02-16 16:37:02.000000 cyberfame-tools-2023.6.13b0/cyberfametools/__main__.py
--rw-rw-r--   0 kittyandrew  (1000) kittyandrew  (1000)     2057 2023-04-03 14:51:16.000000 cyberfame-tools-2023.6.13b0/cyberfametools/basic.py
-drwxrwxr-x   0 kittyandrew  (1000) kittyandrew  (1000)        0 2023-06-13 15:37:27.247161 cyberfame-tools-2023.6.13b0/cyberfametools/data/
--rw-rw-r--   0 kittyandrew  (1000) kittyandrew  (1000)   341846 2023-02-13 21:39:19.000000 cyberfame-tools-2023.6.13b0/cyberfametools/data/packed.bin
--rw-rw-r--   0 kittyandrew  (1000) kittyandrew  (1000)    19090 2023-06-12 19:14:57.000000 cyberfame-tools-2023.6.13b0/cyberfametools/gh.py
--rw-rw-r--   0 kittyandrew  (1000) kittyandrew  (1000)     9008 2023-02-13 21:39:37.000000 cyberfame-tools-2023.6.13b0/cyberfametools/identification.py
--rw-rw-r--   0 kittyandrew  (1000) kittyandrew  (1000)       38 2023-06-13 15:37:27.251161 cyberfame-tools-2023.6.13b0/setup.cfg
--rw-rw-r--   0 kittyandrew  (1000) kittyandrew  (1000)     1093 2023-06-13 15:37:18.000000 cyberfame-tools-2023.6.13b0/setup.py
+drwxrwxr-x   0 kittyandrew  (1000) kittyandrew  (1000)        0 2023-06-13 15:38:14.611359 cyberfame-tools-2023.6.14/
+-rw-rw-r--   0 kittyandrew  (1000) kittyandrew  (1000)       39 2023-02-11 15:59:23.000000 cyberfame-tools-2023.6.14/MANIFEST.in
+-rw-rw-r--   0 kittyandrew  (1000) kittyandrew  (1000)      652 2023-06-13 15:38:14.611359 cyberfame-tools-2023.6.14/PKG-INFO
+-rw-rw-r--   0 kittyandrew  (1000) kittyandrew  (1000)      123 2023-02-16 16:35:41.000000 cyberfame-tools-2023.6.14/README.md
+drwxrwxr-x   0 kittyandrew  (1000) kittyandrew  (1000)        0 2023-06-13 15:38:14.607359 cyberfame-tools-2023.6.14/cyberfame_tools.egg-info/
+-rw-rw-r--   0 kittyandrew  (1000) kittyandrew  (1000)      652 2023-06-13 15:38:14.000000 cyberfame-tools-2023.6.14/cyberfame_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 kittyandrew  (1000) kittyandrew  (1000)      387 2023-06-13 15:38:14.000000 cyberfame-tools-2023.6.14/cyberfame_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 kittyandrew  (1000) kittyandrew  (1000)        1 2023-06-13 15:38:14.000000 cyberfame-tools-2023.6.14/cyberfame_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 kittyandrew  (1000) kittyandrew  (1000)        8 2023-06-13 15:38:14.000000 cyberfame-tools-2023.6.14/cyberfame_tools.egg-info/requires.txt
+-rw-rw-r--   0 kittyandrew  (1000) kittyandrew  (1000)       15 2023-06-13 15:38:14.000000 cyberfame-tools-2023.6.14/cyberfame_tools.egg-info/top_level.txt
+drwxrwxr-x   0 kittyandrew  (1000) kittyandrew  (1000)        0 2023-06-13 15:38:14.611359 cyberfame-tools-2023.6.14/cyberfametools/
+-rw-rw-r--   0 kittyandrew  (1000) kittyandrew  (1000)      180 2023-06-13 15:23:20.000000 cyberfame-tools-2023.6.14/cyberfametools/__init__.py
+-rw-rw-r--   0 kittyandrew  (1000) kittyandrew  (1000)      729 2023-02-16 16:37:02.000000 cyberfame-tools-2023.6.14/cyberfametools/__main__.py
+-rw-rw-r--   0 kittyandrew  (1000) kittyandrew  (1000)     2057 2023-04-03 14:51:16.000000 cyberfame-tools-2023.6.14/cyberfametools/basic.py
+drwxrwxr-x   0 kittyandrew  (1000) kittyandrew  (1000)        0 2023-06-13 15:38:14.611359 cyberfame-tools-2023.6.14/cyberfametools/data/
+-rw-rw-r--   0 kittyandrew  (1000) kittyandrew  (1000)   341846 2023-02-13 21:39:19.000000 cyberfame-tools-2023.6.14/cyberfametools/data/packed.bin
+-rw-rw-r--   0 kittyandrew  (1000) kittyandrew  (1000)    19090 2023-06-12 19:14:57.000000 cyberfame-tools-2023.6.14/cyberfametools/gh.py
+-rw-rw-r--   0 kittyandrew  (1000) kittyandrew  (1000)     9008 2023-02-13 21:39:37.000000 cyberfame-tools-2023.6.14/cyberfametools/identification.py
+-rw-rw-r--   0 kittyandrew  (1000) kittyandrew  (1000)       38 2023-06-13 15:38:14.611359 cyberfame-tools-2023.6.14/setup.cfg
+-rw-rw-r--   0 kittyandrew  (1000) kittyandrew  (1000)     1092 2023-06-13 15:38:05.000000 cyberfame-tools-2023.6.14/setup.py
```

### Comparing `cyberfame-tools-2023.6.13b0/PKG-INFO` & `cyberfame-tools-2023.6.14/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberfame-tools
-Version: 2023.6.13b0
+Version: 2023.6.14
 Summary: Answering interesting cybersecurity questions with graph theory.
 Author: Cyberfame Team
 Author-email: contact@morphysm.com
 Keywords: cyberfame tools
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cyberfame-tools-2023.6.13b0/cyberfame_tools.egg-info/PKG-INFO` & `cyberfame-tools-2023.6.14/cyberfame_tools.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberfame-tools
-Version: 2023.6.13b0
+Version: 2023.6.14
 Summary: Answering interesting cybersecurity questions with graph theory.
 Author: Cyberfame Team
 Author-email: contact@morphysm.com
 Keywords: cyberfame tools
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cyberfame-tools-2023.6.13b0/cyberfametools/__main__.py` & `cyberfame-tools-2023.6.14/cyberfametools/__main__.py`

 * *Files identical despite different names*

### Comparing `cyberfame-tools-2023.6.13b0/cyberfametools/basic.py` & `cyberfame-tools-2023.6.14/cyberfametools/basic.py`

 * *Files identical despite different names*

### Comparing `cyberfame-tools-2023.6.13b0/cyberfametools/data/packed.bin` & `cyberfame-tools-2023.6.14/cyberfametools/data/packed.bin`

 * *Files identical despite different names*

### Comparing `cyberfame-tools-2023.6.13b0/cyberfametools/gh.py` & `cyberfame-tools-2023.6.14/cyberfametools/gh.py`

 * *Files identical despite different names*

### Comparing `cyberfame-tools-2023.6.13b0/cyberfametools/identification.py` & `cyberfame-tools-2023.6.14/cyberfametools/identification.py`

 * *Files identical despite different names*

### Comparing `cyberfame-tools-2023.6.13b0/setup.py` & `cyberfame-tools-2023.6.14/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # from cyberfametools import __version__
-__version__ = "2023.06.13b"
+__version__ = "2023.06.14"
 import setuptools
 
 
 setuptools.setup(
     name="cyberfame-tools",
     version=__version__,
     description="Answering interesting cybersecurity questions with graph theory.",
```

