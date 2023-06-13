# Comparing `tmp/needed-libs-0.7.tar.gz` & `tmp/needed-libs-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "needed-libs-0.7.tar", last modified: Sun Jun 11 13:06:20 2023, max compression
+gzip compressed data, was "needed-libs-0.8.tar", last modified: Tue Jun 13 20:36:35 2023, max compression
```

## Comparing `needed-libs-0.7.tar` & `needed-libs-0.8.tar`

### file list

```diff
@@ -1,12 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 13:06:20.604233 needed-libs-0.7/
--rw-rw-rw-   0        0        0       56 2023-06-11 13:06:20.604233 needed-libs-0.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-11 13:06:20.599237 needed-libs-0.7/needed_libs/
--rw-rw-rw-   0        0        0        0 2023-06-10 18:56:07.000000 needed-libs-0.7/needed_libs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-11 13:06:20.603234 needed-libs-0.7/needed_libs.egg-info/
--rw-rw-rw-   0        0        0       56 2023-06-11 13:06:20.000000 needed-libs-0.7/needed_libs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      216 2023-06-11 13:06:20.000000 needed-libs-0.7/needed_libs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 13:06:20.000000 needed-libs-0.7/needed_libs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      339 2023-06-11 13:06:20.000000 needed-libs-0.7/needed_libs.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-11 13:06:20.000000 needed-libs-0.7/needed_libs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-11 13:06:20.604233 needed-libs-0.7/setup.cfg
--rw-rw-rw-   0        0        0      920 2023-06-11 13:06:14.000000 needed-libs-0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 20:36:35.790924 needed-libs-0.8/
+-rw-rw-rw-   0        0        0       35 2023-06-10 18:54:12.000000 needed-libs-0.8/.gitignore
+-rw-rw-rw-   0        0        0       56 2023-06-13 20:36:35.790924 needed-libs-0.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-13 20:36:35.784928 needed-libs-0.8/needed_libs/
+-rw-rw-rw-   0        0        0     1364 2023-06-12 11:29:22.000000 needed-libs-0.8/needed_libs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 20:36:35.789924 needed-libs-0.8/needed_libs/__pycache__/
+-rw-rw-rw-   0        0        0      838 2023-06-11 14:50:34.000000 needed-libs-0.8/needed_libs/__pycache__/__init__.cpython-39.pyc
+drwxrwxrwx   0        0        0        0 2023-06-13 20:36:35.788925 needed-libs-0.8/needed_libs.egg-info/
+-rw-rw-rw-   0        0        0       56 2023-06-13 20:36:35.000000 needed-libs-0.8/needed_libs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2023-06-13 20:36:35.000000 needed-libs-0.8/needed_libs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 20:36:35.000000 needed-libs-0.8/needed_libs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      338 2023-06-13 20:36:35.000000 needed-libs-0.8/needed_libs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-13 20:36:35.000000 needed-libs-0.8/needed_libs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-13 20:36:35.790924 needed-libs-0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1768 2023-06-13 20:36:28.000000 needed-libs-0.8/setup.py
+-rw-rw-rw-   0        0        0     2363 2023-06-12 11:27:48.000000 needed-libs-0.8/test.py
```

