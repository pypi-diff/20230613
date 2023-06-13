# Comparing `tmp/BLACKFORGE2-0.1.2.tar.gz` & `tmp/BLACKFORGE2-0.1.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BLACKFORGE2-0.1.2.tar", last modified: Tue Jun 13 02:35:00 2023, max compression
+gzip compressed data, was "BLACKFORGE2-0.1.post2.tar", last modified: Tue Jun 13 07:30:29 2023, max compression
```

## Comparing `BLACKFORGE2-0.1.2.tar` & `BLACKFORGE2-0.1.post2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 02:35:00.652837 BLACKFORGE2-0.1.2/
-drwxrwxrwx   0        0        0        0 2023-06-13 02:35:00.628994 BLACKFORGE2-0.1.2/BLACKFORGE2/
--rw-rw-rw-   0        0        0    14204 2023-06-13 02:34:43.000000 BLACKFORGE2-0.1.2/BLACKFORGE2/FORGE.py
--rw-rw-rw-   0        0        0       20 2023-06-13 01:21:24.000000 BLACKFORGE2-0.1.2/BLACKFORGE2/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 02:35:00.650173 BLACKFORGE2-0.1.2/BLACKFORGE2.egg-info/
--rw-rw-rw-   0        0        0      311 2023-06-13 02:35:00.000000 BLACKFORGE2-0.1.2/BLACKFORGE2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2023-06-13 02:35:00.000000 BLACKFORGE2-0.1.2/BLACKFORGE2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 02:35:00.000000 BLACKFORGE2-0.1.2/BLACKFORGE2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-06-13 02:35:00.000000 BLACKFORGE2-0.1.2/BLACKFORGE2.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-13 02:35:00.000000 BLACKFORGE2-0.1.2/BLACKFORGE2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1085 2023-06-13 00:44:16.000000 BLACKFORGE2-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      311 2023-06-13 02:35:00.651556 BLACKFORGE2-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0       70 2023-06-13 00:44:29.000000 BLACKFORGE2-0.1.2/README.rst
--rw-rw-rw-   0        0        0       42 2023-06-13 02:35:00.652837 BLACKFORGE2-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      491 2023-06-13 02:34:48.000000 BLACKFORGE2-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 07:30:29.908442 BLACKFORGE2-0.1.post2/
+drwxrwxrwx   0        0        0        0 2023-06-13 07:30:29.881263 BLACKFORGE2-0.1.post2/BLACKFORGE2/
+-rw-rw-rw-   0        0        0    14204 2023-06-13 02:34:43.000000 BLACKFORGE2-0.1.post2/BLACKFORGE2/FORGE.py
+-rw-rw-rw-   0        0        0       20 2023-06-13 01:21:24.000000 BLACKFORGE2-0.1.post2/BLACKFORGE2/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 07:30:29.905450 BLACKFORGE2-0.1.post2/BLACKFORGE2.egg-info/
+-rw-rw-rw-   0        0        0      315 2023-06-13 07:30:29.000000 BLACKFORGE2-0.1.post2/BLACKFORGE2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2023-06-13 07:30:29.000000 BLACKFORGE2-0.1.post2/BLACKFORGE2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 07:30:29.000000 BLACKFORGE2-0.1.post2/BLACKFORGE2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-06-13 07:30:29.000000 BLACKFORGE2-0.1.post2/BLACKFORGE2.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-13 07:30:29.000000 BLACKFORGE2-0.1.post2/BLACKFORGE2.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1085 2023-06-13 00:44:16.000000 BLACKFORGE2-0.1.post2/LICENSE
+-rw-rw-rw-   0        0        0      315 2023-06-13 07:30:29.907446 BLACKFORGE2-0.1.post2/PKG-INFO
+-rw-rw-rw-   0        0        0     8041 2023-06-13 07:29:39.000000 BLACKFORGE2-0.1.post2/README.rst
+-rw-rw-rw-   0        0        0       42 2023-06-13 07:30:29.908442 BLACKFORGE2-0.1.post2/setup.cfg
+-rw-rw-rw-   0        0        0      495 2023-06-13 07:30:15.000000 BLACKFORGE2-0.1.post2/setup.py
```

### Comparing `BLACKFORGE2-0.1.2/BLACKFORGE2/FORGE.py` & `BLACKFORGE2-0.1.post2/BLACKFORGE2/FORGE.py`

 * *Files identical despite different names*

### Comparing `BLACKFORGE2-0.1.2/LICENSE` & `BLACKFORGE2-0.1.post2/LICENSE`

 * *Files identical despite different names*

