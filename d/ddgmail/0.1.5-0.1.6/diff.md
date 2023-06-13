# Comparing `tmp/ddgmail-0.1.5.tar.gz` & `tmp/ddgmail-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ddgmail-0.1.5.tar", last modified: Mon Jun 12 20:15:52 2023, max compression
+gzip compressed data, was "ddgmail-0.1.6.tar", last modified: Tue Jun 13 08:12:42 2023, max compression
```

## Comparing `ddgmail-0.1.5.tar` & `ddgmail-0.1.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-12 20:15:52.197408 ddgmail-0.1.5/
--rw-rw-r--   0 user      (1000) user      (1000)     3078 2023-06-12 15:21:01.000000 ddgmail-0.1.5/.gitignore
--rw-rw-r--   0 user      (1000) user      (1000)    20623 2023-06-12 17:51:04.000000 ddgmail-0.1.5/.pylintrc
--rw-------   0 user      (1000) user      (1000)    35149 2023-06-12 11:39:18.000000 ddgmail-0.1.5/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)      220 2023-06-12 12:07:16.000000 ddgmail-0.1.5/Makefile
--rw-rw-r--   0 user      (1000) user      (1000)      454 2023-06-12 20:15:52.197408 ddgmail-0.1.5/PKG-INFO
--rwx------   0 user      (1000) user      (1000)      136 2023-06-12 15:37:51.000000 ddgmail-0.1.5/build_and_publish.sh
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-12 20:15:52.197408 ddgmail-0.1.5/ddgmail.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)      454 2023-06-12 20:15:52.000000 ddgmail-0.1.5/ddgmail.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      266 2023-06-12 20:15:52.000000 ddgmail-0.1.5/ddgmail.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-06-12 20:15:52.000000 ddgmail-0.1.5/ddgmail.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)       41 2023-06-12 20:15:52.000000 ddgmail-0.1.5/ddgmail.egg-info/entry_points.txt
--rw-rw-r--   0 user      (1000) user      (1000)       25 2023-06-12 20:15:52.000000 ddgmail-0.1.5/ddgmail.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        8 2023-06-12 20:15:52.000000 ddgmail-0.1.5/ddgmail.egg-info/top_level.txt
--rwxrwxr-x   0 user      (1000) user      (1000)     5552 2023-06-12 20:15:20.000000 ddgmail-0.1.5/ddgmail.py
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-06-12 20:15:52.197408 ddgmail-0.1.5/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     1126 2023-06-12 20:15:42.000000 ddgmail-0.1.5/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-13 08:12:42.771241 ddgmail-0.1.6/
+-rw-rw-r--   0 user      (1000) user      (1000)     3078 2023-06-12 15:21:01.000000 ddgmail-0.1.6/.gitignore
+-rw-rw-r--   0 user      (1000) user      (1000)    20623 2023-06-12 17:51:04.000000 ddgmail-0.1.6/.pylintrc
+-rw-------   0 user      (1000) user      (1000)    35149 2023-06-12 11:39:18.000000 ddgmail-0.1.6/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)      220 2023-06-12 12:07:16.000000 ddgmail-0.1.6/Makefile
+-rw-rw-r--   0 user      (1000) user      (1000)      454 2023-06-13 08:12:42.771241 ddgmail-0.1.6/PKG-INFO
+-rwx------   0 user      (1000) user      (1000)      136 2023-06-12 15:37:51.000000 ddgmail-0.1.6/build_and_publish.sh
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-13 08:12:42.771241 ddgmail-0.1.6/ddgmail.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)      454 2023-06-13 08:12:42.000000 ddgmail-0.1.6/ddgmail.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      266 2023-06-13 08:12:42.000000 ddgmail-0.1.6/ddgmail.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-06-13 08:12:42.000000 ddgmail-0.1.6/ddgmail.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       41 2023-06-13 08:12:42.000000 ddgmail-0.1.6/ddgmail.egg-info/entry_points.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       34 2023-06-13 08:12:42.000000 ddgmail-0.1.6/ddgmail.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        8 2023-06-13 08:12:42.000000 ddgmail-0.1.6/ddgmail.egg-info/top_level.txt
+-rwxrwxr-x   0 user      (1000) user      (1000)     5552 2023-06-12 20:15:20.000000 ddgmail-0.1.6/ddgmail.py
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-06-13 08:12:42.771241 ddgmail-0.1.6/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     1146 2023-06-13 08:12:30.000000 ddgmail-0.1.6/setup.py
```

### Comparing `ddgmail-0.1.5/.gitignore` & `ddgmail-0.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `ddgmail-0.1.5/.pylintrc` & `ddgmail-0.1.6/.pylintrc`

 * *Files identical despite different names*

### Comparing `ddgmail-0.1.5/LICENSE` & `ddgmail-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ddgmail-0.1.5/ddgmail.py` & `ddgmail-0.1.6/ddgmail.py`

 * *Files identical despite different names*

### Comparing `ddgmail-0.1.5/setup.py` & `ddgmail-0.1.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,22 +6,23 @@
 # This conditional isn't necessary, but it provides better error messages to
 # people who try to install this package with older versions of setuptools.
 if parse_version(setuptools_version) < parse_version(min_setuptools_version):
     raise RuntimeError(f"setuptools {min_setuptools_version}+ is required")
 
 setup(
     name="ddgmail",
-    version="0.1.5",
+    version="0.1.6",
     py_modules=["ddgmail"],
     author="rany",
     author_email="ranygh@riseup.net",
     url="https://github.com/rany2/ddgmail",
     description="A command line tool to use DuckDuckGo's E-mail forwarding service",
     install_requires=[
         "Click",
+        "requests",
         f"setuptools>={min_setuptools_version}",
     ],
     entry_points={
         "console_scripts": [
             "ddgmail = ddgmail:cli",
         ],
     },
```

