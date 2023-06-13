# Comparing `tmp/myl-0.6.tar.gz` & `tmp/myl-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myl-0.6.tar", last modified: Mon May 29 10:35:51 2023, max compression
+gzip compressed data, was "myl-0.7.0.tar", last modified: Tue Jun 13 16:49:57 2023, max compression
```

## Comparing `myl-0.6.tar` & `myl-0.7.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:35:50.999130 myl-0.6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:35:50.995130 myl-0.6/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-29 10:35:36.000000 myl-0.6/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:35:50.995130 myl-0.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-29 10:35:36.000000 myl-0.6/.github/workflows/lint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-29 10:35:36.000000 myl-0.6/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-29 10:35:36.000000 myl-0.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-29 10:35:36.000000 myl-0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    40929 2023-05-29 10:35:50.999130 myl-0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-29 10:35:36.000000 myl-0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:35:50.995130 myl-0.6/myl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    40929 2023-05-29 10:35:50.000000 myl-0.6/myl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-29 10:35:50.000000 myl-0.6/myl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 10:35:50.000000 myl-0.6/myl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-29 10:35:50.000000 myl-0.6/myl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-29 10:35:50.000000 myl-0.6/myl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-29 10:35:50.000000 myl-0.6/myl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-05-29 10:35:36.000000 myl-0.6/myl.py
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-29 10:35:36.000000 myl-0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 10:35:50.999130 myl-0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:49:57.137238 myl-0.7.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:49:57.133238 myl-0.7.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-13 16:49:46.000000 myl-0.7.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:49:57.133238 myl-0.7.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-13 16:49:46.000000 myl-0.7.0/.github/workflows/lint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-13 16:49:46.000000 myl-0.7.0/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-13 16:49:46.000000 myl-0.7.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-13 16:49:46.000000 myl-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    40931 2023-06-13 16:49:57.133238 myl-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-13 16:49:46.000000 myl-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:49:57.133238 myl-0.7.0/myl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    40931 2023-06-13 16:49:57.000000 myl-0.7.0/myl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-13 16:49:57.000000 myl-0.7.0/myl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 16:49:57.000000 myl-0.7.0/myl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-13 16:49:57.000000 myl-0.7.0/myl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-13 16:49:57.000000 myl-0.7.0/myl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-13 16:49:57.000000 myl-0.7.0/myl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-06-13 16:49:46.000000 myl-0.7.0/myl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-13 16:49:46.000000 myl-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 16:49:57.137238 myl-0.7.0/setup.cfg
```

### Comparing `myl-0.6/.github/workflows/release.yaml` & `myl-0.7.0/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `myl-0.6/LICENSE` & `myl-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `myl-0.6/PKG-INFO` & `myl-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myl
-Version: 0.6
+Version: 0.7.0
 Summary: Dead simple IMAP CLI client
 Author-email: Philipp Schmitt <philipp@schmitt.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `myl-0.6/myl.egg-info/PKG-INFO` & `myl-0.7.0/myl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myl
-Version: 0.6
+Version: 0.7.0
 Summary: Dead simple IMAP CLI client
 Author-email: Philipp Schmitt <philipp@schmitt.co>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `myl-0.6/pyproject.toml` & `myl-0.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,14 @@
 classifiers = [
   "Programming Language :: Python :: 3",
 ]
 dependencies = [
   "imap_tools",
   "rich"
 ]
-version = "0.6"
+version = "0.7.0"
 
 [tool.black]
 line-length = 79
 
 [project.scripts]
 myl = "myl:main"
```

