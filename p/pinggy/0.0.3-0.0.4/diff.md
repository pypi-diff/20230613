# Comparing `tmp/pinggy-0.0.3.tar.gz` & `tmp/pinggy-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pinggy-0.0.3.tar", last modified: Mon Jun 12 02:53:36 2023, max compression
+gzip compressed data, was "pinggy-0.0.4.tar", last modified: Tue Jun 13 02:46:31 2023, max compression
```

## Comparing `pinggy-0.0.3.tar` & `pinggy-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 abhijit   (1000) abhijit   (1000)        0 2023-06-12 02:53:36.024803 pinggy-0.0.3/
--rw-r--r--   0 abhijit   (1000) abhijit   (1000)     1070 2023-06-11 13:32:33.000000 pinggy-0.0.3/LICENSE.md
--rw-r--r--   0 abhijit   (1000) abhijit   (1000)     1798 2023-06-12 02:53:36.021470 pinggy-0.0.3/PKG-INFO
--rw-r--r--   0 abhijit   (1000) abhijit   (1000)      111 2023-06-11 13:13:00.000000 pinggy-0.0.3/README.md
--rw-r--r--   0 abhijit   (1000) abhijit   (1000)     1064 2023-06-12 02:52:04.000000 pinggy-0.0.3/pyproject.toml
--rw-r--r--   0 abhijit   (1000) abhijit   (1000)       38 2023-06-12 02:53:36.024803 pinggy-0.0.3/setup.cfg
-drwxr-xr-x   0 abhijit   (1000) abhijit   (1000)        0 2023-06-12 02:53:36.018137 pinggy-0.0.3/src/
-drwxr-xr-x   0 abhijit   (1000) abhijit   (1000)        0 2023-06-12 02:53:36.021470 pinggy-0.0.3/src/pinggy/
--rw-r--r--   0 abhijit   (1000) abhijit   (1000)       48 2023-06-08 06:06:51.000000 pinggy-0.0.3/src/pinggy/__init__.py
--rw-r--r--   0 abhijit   (1000) abhijit   (1000)      675 2023-06-08 06:23:03.000000 pinggy-0.0.3/src/pinggy/fileno.py
--rw-r--r--   0 abhijit   (1000) abhijit   (1000)      856 2023-06-11 12:12:05.000000 pinggy-0.0.3/src/pinggy/http.py
--rw-r--r--   0 abhijit   (1000) abhijit   (1000)     6222 2023-06-11 11:28:41.000000 pinggy-0.0.3/src/pinggy/pinggyConnection.py
-drwxr-xr-x   0 abhijit   (1000) abhijit   (1000)        0 2023-06-12 02:53:36.021470 pinggy-0.0.3/src/pinggy.egg-info/
--rw-r--r--   0 abhijit   (1000) abhijit   (1000)     1798 2023-06-12 02:53:36.000000 pinggy-0.0.3/src/pinggy.egg-info/PKG-INFO
--rw-r--r--   0 abhijit   (1000) abhijit   (1000)      335 2023-06-12 02:53:36.000000 pinggy-0.0.3/src/pinggy.egg-info/SOURCES.txt
--rw-r--r--   0 abhijit   (1000) abhijit   (1000)        1 2023-06-12 02:53:36.000000 pinggy-0.0.3/src/pinggy.egg-info/dependency_links.txt
--rw-r--r--   0 abhijit   (1000) abhijit   (1000)       48 2023-06-12 02:53:36.000000 pinggy-0.0.3/src/pinggy.egg-info/entry_points.txt
--rw-r--r--   0 abhijit   (1000) abhijit   (1000)       24 2023-06-12 02:53:36.000000 pinggy-0.0.3/src/pinggy.egg-info/requires.txt
--rw-r--r--   0 abhijit   (1000) abhijit   (1000)        7 2023-06-12 02:53:36.000000 pinggy-0.0.3/src/pinggy.egg-info/top_level.txt
+drwxr-xr-x   0 abhijit   (1000) abhijit   (1000)        0 2023-06-13 02:46:31.208629 pinggy-0.0.4/
+-rw-r--r--   0 abhijit   (1000) abhijit   (1000)     1070 2023-06-11 13:32:33.000000 pinggy-0.0.4/LICENSE.md
+-rw-r--r--   0 abhijit   (1000) abhijit   (1000)     1798 2023-06-13 02:46:31.208629 pinggy-0.0.4/PKG-INFO
+-rw-r--r--   0 abhijit   (1000) abhijit   (1000)      111 2023-06-11 13:13:00.000000 pinggy-0.0.4/README.md
+-rw-r--r--   0 abhijit   (1000) abhijit   (1000)     1064 2023-06-13 02:40:46.000000 pinggy-0.0.4/pyproject.toml
+-rw-r--r--   0 abhijit   (1000) abhijit   (1000)       38 2023-06-13 02:46:31.208629 pinggy-0.0.4/setup.cfg
+drwxr-xr-x   0 abhijit   (1000) abhijit   (1000)        0 2023-06-13 02:46:31.205296 pinggy-0.0.4/src/
+drwxr-xr-x   0 abhijit   (1000) abhijit   (1000)        0 2023-06-13 02:46:31.208629 pinggy-0.0.4/src/pinggy/
+-rw-r--r--   0 abhijit   (1000) abhijit   (1000)       48 2023-06-08 06:06:51.000000 pinggy-0.0.4/src/pinggy/__init__.py
+-rw-r--r--   0 abhijit   (1000) abhijit   (1000)      675 2023-06-08 06:23:03.000000 pinggy-0.0.4/src/pinggy/fileno.py
+-rw-r--r--   0 abhijit   (1000) abhijit   (1000)     6222 2023-06-11 11:28:41.000000 pinggy-0.0.4/src/pinggy/pinggyConnection.py
+-rw-r--r--   0 abhijit   (1000) abhijit   (1000)     1204 2023-06-12 16:27:39.000000 pinggy-0.0.4/src/pinggy/serve.py
+drwxr-xr-x   0 abhijit   (1000) abhijit   (1000)        0 2023-06-13 02:46:31.208629 pinggy-0.0.4/src/pinggy.egg-info/
+-rw-r--r--   0 abhijit   (1000) abhijit   (1000)     1798 2023-06-13 02:46:31.000000 pinggy-0.0.4/src/pinggy.egg-info/PKG-INFO
+-rw-r--r--   0 abhijit   (1000) abhijit   (1000)      336 2023-06-13 02:46:31.000000 pinggy-0.0.4/src/pinggy.egg-info/SOURCES.txt
+-rw-r--r--   0 abhijit   (1000) abhijit   (1000)        1 2023-06-13 02:46:31.000000 pinggy-0.0.4/src/pinggy.egg-info/dependency_links.txt
+-rw-r--r--   0 abhijit   (1000) abhijit   (1000)       48 2023-06-13 02:46:31.000000 pinggy-0.0.4/src/pinggy.egg-info/entry_points.txt
+-rw-r--r--   0 abhijit   (1000) abhijit   (1000)       24 2023-06-13 02:46:31.000000 pinggy-0.0.4/src/pinggy.egg-info/requires.txt
+-rw-r--r--   0 abhijit   (1000) abhijit   (1000)        7 2023-06-13 02:46:31.000000 pinggy-0.0.4/src/pinggy.egg-info/top_level.txt
```

### Comparing `pinggy-0.0.3/LICENSE.md` & `pinggy-0.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pinggy-0.0.3/PKG-INFO` & `pinggy-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pinggy
-Version: 0.0.3
+Version: 0.0.4
 Summary: Very initial version of pinggy python sdk
 Author-email: Pinggy <contact@pinggy.io>
 License: MIT License
         
         Copyright (c) 2023 Abhijit Mondal
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pinggy-0.0.3/pyproject.toml` & `pinggy-0.0.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pinggy"
-version = "0.0.3"
+version = "0.0.4"
 description = "Very initial version of pinggy python sdk"
 readme = "README.md"
 authors = [{ name = "Pinggy", email = "contact@pinggy.io" }]
 license = { file = "LICENSE.md" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
@@ -28,15 +28,15 @@
 Homepage = "https://github.com/abhimp/pinggypython"
 
 [project.scripts]
 realpython = "pinggy.http:main"
 
 
 [tool.bumpver]
-current_version = "0.0.3"
+current_version = "0.0.4"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = false
 tag = false
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `pinggy-0.0.3/src/pinggy/fileno.py` & `pinggy-0.0.4/src/pinggy/fileno.py`

 * *Files identical despite different names*

### Comparing `pinggy-0.0.3/src/pinggy/pinggyConnection.py` & `pinggy-0.0.4/src/pinggy/pinggyConnection.py`

 * *Files identical despite different names*

### Comparing `pinggy-0.0.3/src/pinggy.egg-info/PKG-INFO` & `pinggy-0.0.4/src/pinggy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pinggy
-Version: 0.0.3
+Version: 0.0.4
 Summary: Very initial version of pinggy python sdk
 Author-email: Pinggy <contact@pinggy.io>
 License: MIT License
         
         Copyright (c) 2023 Abhijit Mondal
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

