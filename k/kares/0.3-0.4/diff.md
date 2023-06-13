# Comparing `tmp/kares-0.3.tar.gz` & `tmp/kares-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kares-0.3.tar", last modified: Tue Jun 13 19:06:03 2023, max compression
+gzip compressed data, was "kares-0.4.tar", last modified: Tue Jun 13 19:12:02 2023, max compression
```

## Comparing `kares-0.3.tar` & `kares-0.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 19:06:03.080275 kares-0.3/
--rw-rw-rw-   0        0        0      323 2023-06-13 19:06:03.077178 kares-0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-13 19:06:03.056017 kares-0.3/kares/
--rw-rw-rw-   0        0        0      506 2023-06-13 19:05:58.000000 kares-0.3/kares/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 19:06:03.075913 kares-0.3/kares.egg-info/
--rw-rw-rw-   0        0        0      323 2023-06-13 19:06:02.000000 kares-0.3/kares.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      142 2023-06-13 19:06:02.000000 kares-0.3/kares.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 19:06:02.000000 kares-0.3/kares.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-13 19:06:02.000000 kares-0.3/kares.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-13 19:06:03.080275 kares-0.3/setup.cfg
--rw-rw-rw-   0        0        0      424 2023-06-13 19:03:53.000000 kares-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 19:12:02.693249 kares-0.4/
+-rw-rw-rw-   0        0        0      323 2023-06-13 19:12:02.691974 kares-0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-13 19:12:02.670502 kares-0.4/kares/
+-rw-rw-rw-   0        0        0      613 2023-06-13 19:11:32.000000 kares-0.4/kares/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 19:12:02.691223 kares-0.4/kares.egg-info/
+-rw-rw-rw-   0        0        0      323 2023-06-13 19:12:02.000000 kares-0.4/kares.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      142 2023-06-13 19:12:02.000000 kares-0.4/kares.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 19:12:02.000000 kares-0.4/kares.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-13 19:12:02.000000 kares-0.4/kares.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-13 19:12:02.693249 kares-0.4/setup.cfg
+-rw-rw-rw-   0        0        0      424 2023-06-13 19:11:57.000000 kares-0.4/setup.py
```

