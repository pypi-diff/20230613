# Comparing `tmp/kares-0.1.tar.gz` & `tmp/kares-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kares-0.1.tar", last modified: Tue Jun 13 18:52:56 2023, max compression
+gzip compressed data, was "kares-0.2.tar", last modified: Tue Jun 13 19:00:00 2023, max compression
```

## Comparing `kares-0.1.tar` & `kares-0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 18:52:56.981078 kares-0.1/
--rw-rw-rw-   0        0        0      323 2023-06-13 18:52:56.980316 kares-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-13 18:52:56.954388 kares-0.1/kares/
--rw-rw-rw-   0        0        0      566 2023-06-13 18:24:27.000000 kares-0.1/kares/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 18:52:56.978842 kares-0.1/kares.egg-info/
--rw-rw-rw-   0        0        0      323 2023-06-13 18:52:56.000000 kares-0.1/kares.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      142 2023-06-13 18:52:56.000000 kares-0.1/kares.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 18:52:56.000000 kares-0.1/kares.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-13 18:52:56.000000 kares-0.1/kares.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-13 18:52:56.981078 kares-0.1/setup.cfg
--rw-rw-rw-   0        0        0      424 2023-06-13 18:52:50.000000 kares-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 19:00:00.573192 kares-0.2/
+-rw-rw-rw-   0        0        0      323 2023-06-13 19:00:00.570941 kares-0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-13 19:00:00.554760 kares-0.2/kares/
+-rw-rw-rw-   0        0        0      566 2023-06-13 18:24:27.000000 kares-0.2/kares/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 19:00:00.570196 kares-0.2/kares.egg-info/
+-rw-rw-rw-   0        0        0      323 2023-06-13 19:00:00.000000 kares-0.2/kares.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      142 2023-06-13 19:00:00.000000 kares-0.2/kares.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 19:00:00.000000 kares-0.2/kares.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-13 19:00:00.000000 kares-0.2/kares.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-13 19:00:00.573192 kares-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      424 2023-06-13 18:58:32.000000 kares-0.2/setup.py
```

### Comparing `kares-0.1/kares/__init__.py` & `kares-0.2/kares/__init__.py`

 * *Files identical despite different names*

