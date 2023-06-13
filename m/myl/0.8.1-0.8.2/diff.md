# Comparing `tmp/myl-0.8.1.tar.gz` & `tmp/myl-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myl-0.8.1.tar", last modified: Tue Jun 13 19:29:31 2023, max compression
+gzip compressed data, was "myl-0.8.2.tar", last modified: Tue Jun 13 20:35:30 2023, max compression
```

## Comparing `myl-0.8.1.tar` & `myl-0.8.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:29:31.050301 myl-0.8.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:29:31.050301 myl-0.8.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-13 19:29:19.000000 myl-0.8.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:29:31.050301 myl-0.8.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-13 19:29:19.000000 myl-0.8.1/.github/workflows/lint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-13 19:29:19.000000 myl-0.8.1/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-13 19:29:19.000000 myl-0.8.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-13 19:29:19.000000 myl-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    40931 2023-06-13 19:29:31.050301 myl-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-13 19:29:19.000000 myl-0.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:29:31.050301 myl-0.8.1/myl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    40931 2023-06-13 19:29:31.000000 myl-0.8.1/myl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-13 19:29:31.000000 myl-0.8.1/myl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 19:29:31.000000 myl-0.8.1/myl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-13 19:29:31.000000 myl-0.8.1/myl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-13 19:29:31.000000 myl-0.8.1/myl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-13 19:29:31.000000 myl-0.8.1/myl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8368 2023-06-13 19:29:19.000000 myl-0.8.1/myl.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-13 19:29:19.000000 myl-0.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 19:29:31.050301 myl-0.8.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:35:30.921270 myl-0.8.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:35:30.917270 myl-0.8.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-13 20:35:19.000000 myl-0.8.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:35:30.921270 myl-0.8.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-13 20:35:19.000000 myl-0.8.2/.github/workflows/lint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-13 20:35:19.000000 myl-0.8.2/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-13 20:35:19.000000 myl-0.8.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-13 20:35:19.000000 myl-0.8.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    40931 2023-06-13 20:35:30.921270 myl-0.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-13 20:35:19.000000 myl-0.8.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:35:30.921270 myl-0.8.2/myl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    40931 2023-06-13 20:35:30.000000 myl-0.8.2/myl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-13 20:35:30.000000 myl-0.8.2/myl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 20:35:30.000000 myl-0.8.2/myl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-13 20:35:30.000000 myl-0.8.2/myl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-13 20:35:30.000000 myl-0.8.2/myl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-13 20:35:30.000000 myl-0.8.2/myl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-06-13 20:35:19.000000 myl-0.8.2/myl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-13 20:35:19.000000 myl-0.8.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 20:35:30.921270 myl-0.8.2/setup.cfg
```

### Comparing `myl-0.8.1/.github/workflows/release.yaml` & `myl-0.8.2/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `myl-0.8.1/LICENSE` & `myl-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `myl-0.8.1/PKG-INFO` & `myl-0.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myl
-Version: 0.8.1
+Version: 0.8.2
 Summary: Dead simple IMAP CLI client
 Author-email: Philipp Schmitt <philipp@schmitt.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `myl-0.8.1/myl.egg-info/PKG-INFO` & `myl-0.8.2/myl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myl
-Version: 0.8.1
+Version: 0.8.2
 Summary: Dead simple IMAP CLI client
 Author-email: Philipp Schmitt <philipp@schmitt.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `myl-0.8.1/pyproject.toml` & `myl-0.8.2/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -12,20 +12,18 @@
 requires-python = ">=3.8"
 keywords = ["imap", "email"]
 license = {file = "LICENSE"}
 classifiers = [
   "Programming Language :: Python :: 3",
 ]
 dependencies = [
-  "dnspython",
   "imap_tools",
-  "requests",
+  "myl-discovery",
   "rich",
-  "xmltodict"
 ]
-version = "0.8.1"
+version = "0.8.2"
 
 [tool.black]
 line-length = 79
 
 [project.scripts]
 myl = "myl:main"
```

