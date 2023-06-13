# Comparing `tmp/kares-0.4.tar.gz` & `tmp/kares-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kares-0.4.tar", last modified: Tue Jun 13 19:12:02 2023, max compression
+gzip compressed data, was "kares-0.5.tar", last modified: Tue Jun 13 19:16:42 2023, max compression
```

## Comparing `kares-0.4.tar` & `kares-0.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 19:12:02.693249 kares-0.4/
--rw-rw-rw-   0        0        0      323 2023-06-13 19:12:02.691974 kares-0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-13 19:12:02.670502 kares-0.4/kares/
--rw-rw-rw-   0        0        0      613 2023-06-13 19:11:32.000000 kares-0.4/kares/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 19:12:02.691223 kares-0.4/kares.egg-info/
--rw-rw-rw-   0        0        0      323 2023-06-13 19:12:02.000000 kares-0.4/kares.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      142 2023-06-13 19:12:02.000000 kares-0.4/kares.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 19:12:02.000000 kares-0.4/kares.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-13 19:12:02.000000 kares-0.4/kares.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-13 19:12:02.693249 kares-0.4/setup.cfg
--rw-rw-rw-   0        0        0      424 2023-06-13 19:11:57.000000 kares-0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 19:16:42.564066 kares-0.5/
+-rw-rw-rw-   0        0        0      323 2023-06-13 19:16:42.563319 kares-0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-13 19:16:42.532884 kares-0.5/kares/
+-rw-rw-rw-   0        0        0      626 2023-06-13 19:14:47.000000 kares-0.5/kares/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 19:16:42.561296 kares-0.5/kares.egg-info/
+-rw-rw-rw-   0        0        0      323 2023-06-13 19:16:42.000000 kares-0.5/kares.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      142 2023-06-13 19:16:42.000000 kares-0.5/kares.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 19:16:42.000000 kares-0.5/kares.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-13 19:16:42.000000 kares-0.5/kares.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-13 19:16:42.564066 kares-0.5/setup.cfg
+-rw-rw-rw-   0        0        0      424 2023-06-13 19:15:36.000000 kares-0.5/setup.py
```

### Comparing `kares-0.4/kares/__init__.py` & `kares-0.5/kares/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import os
+
 def keras(val):
     pracs = {
         1:"Practical_1.txt",
         2:"Practical_2.txt",
         3:"Practical_3.txt",
         4:"Practical_4.txt",
         5:"Practical_5.txt",
```

