# Comparing `tmp/kares-0.6.tar.gz` & `tmp/kares-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kares-0.6.tar", last modified: Tue Jun 13 19:25:30 2023, max compression
+gzip compressed data, was "kares-0.7.tar", last modified: Tue Jun 13 19:38:47 2023, max compression
```

## Comparing `kares-0.6.tar` & `kares-0.7.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 19:25:30.662165 kares-0.6/
--rw-rw-rw-   0        0        0      323 2023-06-13 19:25:30.660671 kares-0.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-13 19:25:30.630866 kares-0.6/kares/
--rw-rw-rw-   0        0        0      645 2023-06-13 19:21:40.000000 kares-0.6/kares/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 19:25:30.660148 kares-0.6/kares.egg-info/
--rw-rw-rw-   0        0        0      323 2023-06-13 19:25:30.000000 kares-0.6/kares.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      142 2023-06-13 19:25:30.000000 kares-0.6/kares.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 19:25:30.000000 kares-0.6/kares.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-13 19:25:30.000000 kares-0.6/kares.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-13 19:25:30.662165 kares-0.6/setup.cfg
--rw-rw-rw-   0        0        0      424 2023-06-13 19:21:46.000000 kares-0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 19:38:47.040091 kares-0.7/
+-rw-rw-rw-   0        0        0      323 2023-06-13 19:38:47.037775 kares-0.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-13 19:38:47.011235 kares-0.7/kares/
+-rw-rw-rw-   0        0        0     1046 2023-06-13 19:38:10.000000 kares-0.7/kares/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 19:38:47.037025 kares-0.7/kares.egg-info/
+-rw-rw-rw-   0        0        0      323 2023-06-13 19:38:46.000000 kares-0.7/kares.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      142 2023-06-13 19:38:46.000000 kares-0.7/kares.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 19:38:46.000000 kares-0.7/kares.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-13 19:38:46.000000 kares-0.7/kares.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-13 19:38:47.040091 kares-0.7/setup.cfg
+-rw-rw-rw-   0        0        0      424 2023-06-13 19:38:41.000000 kares-0.7/setup.py
```

