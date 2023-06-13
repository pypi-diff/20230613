# Comparing `tmp/bludwig-0.0.0.tar.gz` & `tmp/bludwig-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bludwig-0.0.0.tar", last modified: Sat Jun 10 10:19:37 2023, max compression
+gzip compressed data, was "bludwig-0.0.2.tar", last modified: Tue Jun 13 06:28:30 2023, max compression
```

## Comparing `bludwig-0.0.0.tar` & `bludwig-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-10 10:19:37.612524 bludwig-0.0.0/
--rw-r--r--   0 me        (1000) me        (1000)     1063 2022-09-06 17:06:11.000000 bludwig-0.0.0/LICENSE
--rw-rw-r--   0 me        (1000) me        (1000)      485 2023-06-10 10:19:37.612524 bludwig-0.0.0/PKG-INFO
--rw-r--r--   0 me        (1000) me        (1000)       58 2023-06-10 10:12:53.000000 bludwig-0.0.0/README.md
--rw-r--r--   0 me        (1000) me        (1000)     1114 2023-06-10 10:08:02.000000 bludwig-0.0.0/pyproject.toml
--rw-rw-r--   0 me        (1000) me        (1000)       38 2023-06-10 10:19:37.612524 bludwig-0.0.0/setup.cfg
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-10 10:19:37.612524 bludwig-0.0.0/src/
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-10 10:19:37.612524 bludwig-0.0.0/src/bludwig/
--rw-r--r--   0 me        (1000) me        (1000)       65 2023-06-10 09:57:05.000000 bludwig-0.0.0/src/bludwig/__init__.py
--rw-r--r--   0 me        (1000) me        (1000)      197 2023-06-10 09:59:04.000000 bludwig-0.0.0/src/bludwig/__main__.py
--rw-r--r--   0 me        (1000) me        (1000)      338 2023-06-10 09:58:21.000000 bludwig-0.0.0/src/bludwig/helper.py
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-10 10:19:37.612524 bludwig-0.0.0/src/bludwig.egg-info/
--rw-rw-r--   0 me        (1000) me        (1000)      485 2023-06-10 10:19:37.000000 bludwig-0.0.0/src/bludwig.egg-info/PKG-INFO
--rw-rw-r--   0 me        (1000) me        (1000)      314 2023-06-10 10:19:37.000000 bludwig-0.0.0/src/bludwig.egg-info/SOURCES.txt
--rw-rw-r--   0 me        (1000) me        (1000)        1 2023-06-10 10:19:37.000000 bludwig-0.0.0/src/bludwig.egg-info/dependency_links.txt
--rw-rw-r--   0 me        (1000) me        (1000)       50 2023-06-10 10:19:37.000000 bludwig-0.0.0/src/bludwig.egg-info/entry_points.txt
--rw-rw-r--   0 me        (1000) me        (1000)       11 2023-06-10 10:19:37.000000 bludwig-0.0.0/src/bludwig.egg-info/requires.txt
--rw-rw-r--   0 me        (1000) me        (1000)        8 2023-06-10 10:19:37.000000 bludwig-0.0.0/src/bludwig.egg-info/top_level.txt
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-13 06:28:30.092600 bludwig-0.0.2/
+-rw-r--r--   0 me        (1000) me        (1000)     1063 2022-09-06 17:06:11.000000 bludwig-0.0.2/LICENSE
+-rw-rw-r--   0 me        (1000) me        (1000)      485 2023-06-13 06:28:30.092600 bludwig-0.0.2/PKG-INFO
+-rw-r--r--   0 me        (1000) me        (1000)       58 2023-06-13 06:27:25.000000 bludwig-0.0.2/README.md
+-rw-r--r--   0 me        (1000) me        (1000)     1114 2023-06-13 06:26:55.000000 bludwig-0.0.2/pyproject.toml
+-rw-rw-r--   0 me        (1000) me        (1000)       38 2023-06-13 06:28:30.092600 bludwig-0.0.2/setup.cfg
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-13 06:28:30.084600 bludwig-0.0.2/src/
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-13 06:28:30.088600 bludwig-0.0.2/src/bludwig/
+-rw-rw-r--   0 me        (1000) me        (1000)    13992 2023-06-12 20:12:05.000000 bludwig-0.0.2/src/bludwig/LudwigJob.py
+-rw-r--r--   0 me        (1000) me        (1000)       82 2023-06-11 18:48:52.000000 bludwig-0.0.2/src/bludwig/__init__.py
+-rw-r--r--   0 me        (1000) me        (1000)      197 2023-06-10 09:59:04.000000 bludwig-0.0.2/src/bludwig/__main__.py
+-rw-r--r--   0 me        (1000) me        (1000)     3798 2023-06-11 20:20:52.000000 bludwig-0.0.2/src/bludwig/helper.py
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-13 06:28:30.092600 bludwig-0.0.2/src/bludwig.egg-info/
+-rw-rw-r--   0 me        (1000) me        (1000)      485 2023-06-13 06:28:30.000000 bludwig-0.0.2/src/bludwig.egg-info/PKG-INFO
+-rw-rw-r--   0 me        (1000) me        (1000)      339 2023-06-13 06:28:30.000000 bludwig-0.0.2/src/bludwig.egg-info/SOURCES.txt
+-rw-rw-r--   0 me        (1000) me        (1000)        1 2023-06-13 06:28:30.000000 bludwig-0.0.2/src/bludwig.egg-info/dependency_links.txt
+-rw-rw-r--   0 me        (1000) me        (1000)       50 2023-06-13 06:28:30.000000 bludwig-0.0.2/src/bludwig.egg-info/entry_points.txt
+-rw-rw-r--   0 me        (1000) me        (1000)       11 2023-06-13 06:28:30.000000 bludwig-0.0.2/src/bludwig.egg-info/requires.txt
+-rw-rw-r--   0 me        (1000) me        (1000)        8 2023-06-13 06:28:30.000000 bludwig-0.0.2/src/bludwig.egg-info/top_level.txt
```

### Comparing `bludwig-0.0.0/LICENSE` & `bludwig-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bludwig-0.0.0/pyproject.toml` & `bludwig-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # pyproject.toml
 
 
 [project]
 name            = "bludwig"
-version         = "0.0.0"        
+version         = "0.0.2"        
 
 requires-python = ">=3.9"
 dependencies    = ['pandasklar',]
 
 authors        = [{ name = "djekra", email = "hopsalla@gmail.com" }]
 description     = "Some helper for Ludwig"
 readme          = "README.md"
```

