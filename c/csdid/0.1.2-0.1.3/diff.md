# Comparing `tmp/csdid-0.1.2.tar.gz` & `tmp/csdid-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csdid-0.1.2.tar", last modified: Tue Jun 13 21:47:55 2023, max compression
+gzip compressed data, was "csdid-0.1.3.tar", last modified: Tue Jun 13 21:53:53 2023, max compression
```

## Comparing `csdid-0.1.2.tar` & `csdid-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 21:47:55.428304 csdid-0.1.2/
--rw-rw-rw-   0        0        0     1126 2023-06-13 21:34:25.000000 csdid-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      533 2023-06-13 21:47:55.427304 csdid-0.1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-13 21:47:55.418301 csdid-0.1.2/csdid/
--rw-rw-rw-   0        0        0        0 2023-06-13 15:53:11.000000 csdid-0.1.2/csdid/__init__.py
--rw-rw-rw-   0        0        0     3842 2023-06-13 21:46:48.000000 csdid-0.1.2/csdid/att_gt.py
-drwxrwxrwx   0        0        0        0 2023-06-13 21:47:55.427304 csdid-0.1.2/csdid.egg-info/
--rw-rw-rw-   0        0        0      533 2023-06-13 21:47:55.000000 csdid-0.1.2/csdid.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      166 2023-06-13 21:47:55.000000 csdid-0.1.2/csdid.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 21:47:55.000000 csdid-0.1.2/csdid.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-13 21:47:55.000000 csdid-0.1.2/csdid.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-13 21:47:55.428304 csdid-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      607 2023-06-13 21:47:47.000000 csdid-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 21:53:53.680320 csdid-0.1.3/
+-rw-rw-rw-   0        0        0     1126 2023-06-13 21:34:25.000000 csdid-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0      533 2023-06-13 21:53:53.680320 csdid-0.1.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-13 21:53:53.672319 csdid-0.1.3/csdid/
+-rw-rw-rw-   0        0        0        0 2023-06-13 15:53:11.000000 csdid-0.1.3/csdid/__init__.py
+-rw-rw-rw-   0        0        0     3842 2023-06-13 21:46:48.000000 csdid-0.1.3/csdid/att_gt.py
+drwxrwxrwx   0        0        0        0 2023-06-13 21:53:53.679320 csdid-0.1.3/csdid.egg-info/
+-rw-rw-rw-   0        0        0      533 2023-06-13 21:53:53.000000 csdid-0.1.3/csdid.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      166 2023-06-13 21:53:53.000000 csdid-0.1.3/csdid.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 21:53:53.000000 csdid-0.1.3/csdid.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-13 21:53:53.000000 csdid-0.1.3/csdid.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-13 21:53:53.680320 csdid-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      607 2023-06-13 21:53:43.000000 csdid-0.1.3/setup.py
```

### Comparing `csdid-0.1.2/LICENSE` & `csdid-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `csdid-0.1.2/PKG-INFO` & `csdid-0.1.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csdid
-Version: 0.1.2
+Version: 0.1.3
 Summary: Difference in Difference in Python
 Home-page: https://github.com/d2cml-ai/csdid
 Author: D2CML Team, Alexander Quispe, Carlos Guevara, Jhon Flroes
 License: MIT
 Keywords: Causal inference,Research
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `csdid-0.1.2/csdid/att_gt.py` & `csdid-0.1.3/csdid/att_gt.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.2/csdid.egg-info/PKG-INFO` & `csdid-0.1.3/csdid.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csdid
-Version: 0.1.2
+Version: 0.1.3
 Summary: Difference in Difference in Python
 Home-page: https://github.com/d2cml-ai/csdid
 Author: D2CML Team, Alexander Quispe, Carlos Guevara, Jhon Flroes
 License: MIT
 Keywords: Causal inference,Research
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `csdid-0.1.2/setup.py` & `csdid-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
   name = 'csdid',
-  version='0.1.2',
+  version='0.1.3',
   url='https://github.com/d2cml-ai/csdid',
   author='D2CML Team, Alexander Quispe, Carlos Guevara, Jhon Flroes',
   keywords=['Causal inference', 'Research'],
   license="MIT",
   description='Difference in Difference in Python',
   classifiers=[
         "Intended Audience :: Developers",
```

