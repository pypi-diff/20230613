# Comparing `tmp/Carter-Offline-1.0.0.tar.gz` & `tmp/Carter-Offline-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Carter-Offline-1.0.0.tar", last modified: Mon Jun 12 19:53:54 2023, max compression
+gzip compressed data, was "Carter-Offline-1.0.2.tar", last modified: Tue Jun 13 08:14:53 2023, max compression
```

## Comparing `Carter-Offline-1.0.0.tar` & `Carter-Offline-1.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 jackfranklin   (501) staff       (20)        0 2023-06-12 19:53:54.702261 Carter-Offline-1.0.0/
-drwxr-xr-x   0 jackfranklin   (501) staff       (20)        0 2023-06-12 19:53:54.701979 Carter-Offline-1.0.0/Carter_Offline.egg-info/
--rw-r--r--   0 jackfranklin   (501) staff       (20)      249 2023-06-12 19:53:54.000000 Carter-Offline-1.0.0/Carter_Offline.egg-info/PKG-INFO
--rw-r--r--   0 jackfranklin   (501) staff       (20)      197 2023-06-12 19:53:54.000000 Carter-Offline-1.0.0/Carter_Offline.egg-info/SOURCES.txt
--rw-r--r--   0 jackfranklin   (501) staff       (20)        1 2023-06-12 19:53:54.000000 Carter-Offline-1.0.0/Carter_Offline.egg-info/dependency_links.txt
--rw-r--r--   0 jackfranklin   (501) staff       (20)       27 2023-06-12 19:53:54.000000 Carter-Offline-1.0.0/Carter_Offline.egg-info/requires.txt
--rw-r--r--   0 jackfranklin   (501) staff       (20)        1 2023-06-12 19:53:54.000000 Carter-Offline-1.0.0/Carter_Offline.egg-info/top_level.txt
--rw-r--r--   0 jackfranklin   (501) staff       (20)      249 2023-06-12 19:53:54.702149 Carter-Offline-1.0.0/PKG-INFO
--rw-r--r--   0 jackfranklin   (501) staff       (20)       38 2023-06-12 19:53:54.702299 Carter-Offline-1.0.0/setup.cfg
--rw-r--r--   0 jackfranklin   (501) staff       (20)      488 2023-06-12 19:52:28.000000 Carter-Offline-1.0.0/setup.py
+drwxr-xr-x   0 jackfranklin   (501) staff       (20)        0 2023-06-13 08:14:53.790417 Carter-Offline-1.0.2/
+drwxr-xr-x   0 jackfranklin   (501) staff       (20)        0 2023-06-13 08:14:53.790114 Carter-Offline-1.0.2/Carter_Offline.egg-info/
+-rw-r--r--   0 jackfranklin   (501) staff       (20)      249 2023-06-13 08:14:53.000000 Carter-Offline-1.0.2/Carter_Offline.egg-info/PKG-INFO
+-rw-r--r--   0 jackfranklin   (501) staff       (20)      197 2023-06-13 08:14:53.000000 Carter-Offline-1.0.2/Carter_Offline.egg-info/SOURCES.txt
+-rw-r--r--   0 jackfranklin   (501) staff       (20)        1 2023-06-13 08:14:53.000000 Carter-Offline-1.0.2/Carter_Offline.egg-info/dependency_links.txt
+-rw-r--r--   0 jackfranklin   (501) staff       (20)       43 2023-06-13 08:14:53.000000 Carter-Offline-1.0.2/Carter_Offline.egg-info/requires.txt
+-rw-r--r--   0 jackfranklin   (501) staff       (20)        1 2023-06-13 08:14:53.000000 Carter-Offline-1.0.2/Carter_Offline.egg-info/top_level.txt
+-rw-r--r--   0 jackfranklin   (501) staff       (20)      249 2023-06-13 08:14:53.790296 Carter-Offline-1.0.2/PKG-INFO
+-rw-r--r--   0 jackfranklin   (501) staff       (20)       38 2023-06-13 08:14:53.790455 Carter-Offline-1.0.2/setup.cfg
+-rw-r--r--   0 jackfranklin   (501) staff       (20)      526 2023-06-13 08:14:29.000000 Carter-Offline-1.0.2/setup.py
```

