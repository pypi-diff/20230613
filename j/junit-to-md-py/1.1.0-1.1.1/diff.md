# Comparing `tmp/junit-to-md-py-1.1.0.tar.gz` & `tmp/junit-to-md-py-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "junit-to-md-py-1.1.0.tar", last modified: Fri Jun  9 11:45:33 2023, max compression
+gzip compressed data, was "junit-to-md-py-1.1.1.tar", last modified: Tue Jun 13 12:43:16 2023, max compression
```

## Comparing `junit-to-md-py-1.1.0.tar` & `junit-to-md-py-1.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 11:45:33.535014 junit-to-md-py-1.1.0/
--rw-rw-rw-   0        0        0      617 2023-06-09 11:45:33.534014 junit-to-md-py-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      301 2023-06-07 18:12:45.000000 junit-to-md-py-1.1.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-09 11:45:33.527013 junit-to-md-py-1.1.0/junit_to_md_py.egg-info/
--rw-rw-rw-   0        0        0      617 2023-06-09 11:45:33.000000 junit-to-md-py-1.1.0/junit_to_md_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      290 2023-06-09 11:45:33.000000 junit-to-md-py-1.1.0/junit_to_md_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 11:45:33.000000 junit-to-md-py-1.1.0/junit_to_md_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-06-09 11:45:33.000000 junit-to-md-py-1.1.0/junit_to_md_py.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        5 2023-06-09 11:45:33.000000 junit-to-md-py-1.1.0/junit_to_md_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-09 11:45:33.000000 junit-to-md-py-1.1.0/junit_to_md_py.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-09 11:45:33.531014 junit-to-md-py-1.1.0/script/
--rw-rw-rw-   0        0        0        0 2023-06-09 11:39:01.000000 junit-to-md-py-1.1.0/script/__init__.py
--rw-rw-rw-   0        0        0     1267 2023-06-09 11:45:28.000000 junit-to-md-py-1.1.0/script/junit_to_md.py
--rw-rw-rw-   0        0        0       42 2023-06-09 11:45:33.535014 junit-to-md-py-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      616 2023-06-09 11:42:54.000000 junit-to-md-py-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 12:43:16.726388 junit-to-md-py-1.1.1/
+-rw-rw-rw-   0        0        0      554 2023-06-13 12:43:16.725388 junit-to-md-py-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2023-06-09 11:48:23.000000 junit-to-md-py-1.1.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-13 12:43:16.716406 junit-to-md-py-1.1.1/junit_to_md_py.egg-info/
+-rw-rw-rw-   0        0        0      554 2023-06-13 12:43:16.000000 junit-to-md-py-1.1.1/junit_to_md_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      290 2023-06-13 12:43:16.000000 junit-to-md-py-1.1.1/junit_to_md_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 12:43:16.000000 junit-to-md-py-1.1.1/junit_to_md_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-06-13 12:43:16.000000 junit-to-md-py-1.1.1/junit_to_md_py.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        5 2023-06-13 12:43:16.000000 junit-to-md-py-1.1.1/junit_to_md_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-13 12:43:16.000000 junit-to-md-py-1.1.1/junit_to_md_py.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-13 12:43:16.722389 junit-to-md-py-1.1.1/script/
+-rw-rw-rw-   0        0        0        0 2023-06-09 11:39:01.000000 junit-to-md-py-1.1.1/script/__init__.py
+-rw-rw-rw-   0        0        0     1267 2023-06-09 11:45:28.000000 junit-to-md-py-1.1.1/script/junit_to_md.py
+-rw-rw-rw-   0        0        0       42 2023-06-13 12:43:16.726388 junit-to-md-py-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      642 2023-06-13 12:42:48.000000 junit-to-md-py-1.1.1/setup.py
```

### Comparing `junit-to-md-py-1.1.0/PKG-INFO` & `junit-to-md-py-1.1.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: junit-to-md-py
-Version: 1.1.0
+Version: 1.1.1
 Summary: Python script which converts junit xml file/text into the markdown representation
 Home-page: https://github.com/catalogicsoftware/dpx-utils-junit-to-md
 Author: srydz_catalogicsoftware
 Author-email: srydz@catalogicsoftware.com
 License: MIT
 
 Python script which converts junit xml file/text into the markdown representation
 =================================================================================
 
+
 Example usage
 ~~~~~~~~~~~~~
 
 ::
 
-   from junit_to_md import junit_to_md
-
-   junit_to_md(open("sample_junitOutput.xml", "r"))
+   junit-to-md-py report.xml
```

### Comparing `junit-to-md-py-1.1.0/junit_to_md_py.egg-info/PKG-INFO` & `junit-to-md-py-1.1.1/junit_to_md_py.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: junit-to-md-py
-Version: 1.1.0
+Version: 1.1.1
 Summary: Python script which converts junit xml file/text into the markdown representation
 Home-page: https://github.com/catalogicsoftware/dpx-utils-junit-to-md
 Author: srydz_catalogicsoftware
 Author-email: srydz@catalogicsoftware.com
 License: MIT
 
 Python script which converts junit xml file/text into the markdown representation
 =================================================================================
 
+
 Example usage
 ~~~~~~~~~~~~~
 
 ::
 
-   from junit_to_md import junit_to_md
-
-   junit_to_md(open("sample_junitOutput.xml", "r"))
+   junit-to-md-py report.xml
```

### Comparing `junit-to-md-py-1.1.0/script/junit_to_md.py` & `junit-to-md-py-1.1.1/script/junit_to_md.py`

 * *Files identical despite different names*

### Comparing `junit-to-md-py-1.1.0/setup.py` & `junit-to-md-py-1.1.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from setuptools import setup
 
 setup(
     name="junit-to-md-py",
-    version="1.1.0",
+    version="1.1.1",
     author="srydz_catalogicsoftware",
     author_email="srydz@catalogicsoftware.com",
     description="Python script which converts junit xml file/text into the markdown representation",
     long_description=open("README.rst", encoding="utf-8").read(),
     url="https://github.com/catalogicsoftware/dpx-utils-junit-to-md",
     license="MIT",
+    packages=["script"],
     install_requires=[
         "lxml",
     ],
     entry_points={
         "console_scripts": [
             "junit-to-md-py = script.junit_to_md:main",
         ]
```

