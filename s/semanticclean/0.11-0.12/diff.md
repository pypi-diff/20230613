# Comparing `tmp/semanticclean-0.11.tar.gz` & `tmp/semanticclean-0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semanticclean-0.11.tar", last modified: Sun Jun 11 16:42:46 2023, max compression
+gzip compressed data, was "semanticclean-0.12.tar", last modified: Tue Jun 13 10:34:40 2023, max compression
```

## Comparing `semanticclean-0.11.tar` & `semanticclean-0.12.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 elshehawy  (1000) elshehawy  (1000)        0 2023-06-11 16:42:46.232499 semanticclean-0.11/
--rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)      234 2023-06-11 16:42:46.232499 semanticclean-0.11/PKG-INFO
-drwxrwxr-x   0 elshehawy  (1000) elshehawy  (1000)        0 2023-06-11 16:42:46.232499 semanticclean-0.11/semanticclean/
--rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)        0 2023-06-11 13:16:36.000000 semanticclean-0.11/semanticclean/__init__.py
--rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)     6768 2023-06-11 16:09:42.000000 semanticclean-0.11/semanticclean/label.py
-drwxrwxr-x   0 elshehawy  (1000) elshehawy  (1000)        0 2023-06-11 16:42:46.232499 semanticclean-0.11/semanticclean.egg-info/
--rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)      234 2023-06-11 16:42:46.000000 semanticclean-0.11/semanticclean.egg-info/PKG-INFO
--rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)      241 2023-06-11 16:42:46.000000 semanticclean-0.11/semanticclean.egg-info/SOURCES.txt
--rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)        1 2023-06-11 16:42:46.000000 semanticclean-0.11/semanticclean.egg-info/dependency_links.txt
--rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)        1 2023-06-11 16:42:46.000000 semanticclean-0.11/semanticclean.egg-info/not-zip-safe
--rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)       14 2023-06-11 16:42:46.000000 semanticclean-0.11/semanticclean.egg-info/top_level.txt
--rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)       38 2023-06-11 16:42:46.232499 semanticclean-0.11/setup.cfg
--rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)      302 2023-06-11 16:42:39.000000 semanticclean-0.11/setup.py
+drwxrwxr-x   0 elshehawy  (1000) elshehawy  (1000)        0 2023-06-13 10:34:40.024365 semanticclean-0.12/
+-rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)      234 2023-06-13 10:34:40.024365 semanticclean-0.12/PKG-INFO
+drwxrwxr-x   0 elshehawy  (1000) elshehawy  (1000)        0 2023-06-13 10:34:40.024365 semanticclean-0.12/semanticclean/
+-rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)        0 2023-06-13 10:31:58.000000 semanticclean-0.12/semanticclean/__init__.py
+-rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)    11397 2023-06-13 10:31:58.000000 semanticclean-0.12/semanticclean/label.py
+drwxrwxr-x   0 elshehawy  (1000) elshehawy  (1000)        0 2023-06-13 10:34:40.024365 semanticclean-0.12/semanticclean.egg-info/
+-rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)      234 2023-06-13 10:34:40.000000 semanticclean-0.12/semanticclean.egg-info/PKG-INFO
+-rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)      241 2023-06-13 10:34:40.000000 semanticclean-0.12/semanticclean.egg-info/SOURCES.txt
+-rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)        1 2023-06-13 10:34:40.000000 semanticclean-0.12/semanticclean.egg-info/dependency_links.txt
+-rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)        1 2023-06-13 10:34:40.000000 semanticclean-0.12/semanticclean.egg-info/not-zip-safe
+-rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)       14 2023-06-13 10:34:40.000000 semanticclean-0.12/semanticclean.egg-info/top_level.txt
+-rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)       38 2023-06-13 10:34:40.024365 semanticclean-0.12/setup.cfg
+-rw-rw-r--   0 elshehawy  (1000) elshehawy  (1000)      302 2023-06-13 10:33:39.000000 semanticclean-0.12/setup.py
```

