# Comparing `tmp/OpenFintech-0.0.4.tar.gz` & `tmp/OpenFintech-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OpenFintech-0.0.4.tar", last modified: Mon Jun 12 04:24:11 2023, max compression
+gzip compressed data, was "OpenFintech-0.0.5.tar", last modified: Tue Jun 13 17:25:45 2023, max compression
```

## Comparing `OpenFintech-0.0.4.tar` & `OpenFintech-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,19 @@
-drwxr-xr-x   0 harri      (501) staff       (20)        0 2023-06-12 04:24:11.009088 OpenFintech-0.0.4/
--rw-r--r--   0 harri      (501) staff       (20)    11357 2023-06-05 19:27:30.000000 OpenFintech-0.0.4/LICENSE
-drwxr-xr-x   0 harri      (501) staff       (20)        0 2023-06-12 04:24:11.007758 OpenFintech-0.0.4/OpenFintech/
--rw-r--r--   0 harri      (501) staff       (20)     6459 2023-06-12 04:23:26.000000 OpenFintech-0.0.4/OpenFintech/FinMongo.py
--rw-r--r--   0 harri      (501) staff       (20)     1284 2023-06-12 04:23:25.000000 OpenFintech-0.0.4/OpenFintech/User.py
--rw-r--r--   0 harri      (501) staff       (20)       53 2023-06-08 20:01:22.000000 OpenFintech-0.0.4/OpenFintech/__init__.py
-drwxr-xr-x   0 harri      (501) staff       (20)        0 2023-06-12 04:24:11.008671 OpenFintech-0.0.4/OpenFintech.egg-info/
--rw-r--r--   0 harri      (501) staff       (20)       77 2023-06-12 04:24:10.000000 OpenFintech-0.0.4/OpenFintech.egg-info/PKG-INFO
--rw-r--r--   0 harri      (501) staff       (20)      234 2023-06-12 04:24:10.000000 OpenFintech-0.0.4/OpenFintech.egg-info/SOURCES.txt
--rw-r--r--   0 harri      (501) staff       (20)        1 2023-06-12 04:24:10.000000 OpenFintech-0.0.4/OpenFintech.egg-info/dependency_links.txt
--rw-r--r--   0 harri      (501) staff       (20)       12 2023-06-12 04:24:10.000000 OpenFintech-0.0.4/OpenFintech.egg-info/top_level.txt
--rw-r--r--   0 harri      (501) staff       (20)       77 2023-06-12 04:24:11.008910 OpenFintech-0.0.4/PKG-INFO
--rw-r--r--   0 harri      (501) staff       (20)       14 2023-06-05 19:27:30.000000 OpenFintech-0.0.4/README.md
--rw-r--r--   0 harri      (501) staff       (20)       38 2023-06-12 04:24:11.009142 OpenFintech-0.0.4/setup.cfg
--rw-r--r--   0 harri      (501) staff       (20)      128 2023-06-12 04:21:45.000000 OpenFintech-0.0.4/setup.py
+drwxr-xr-x   0 harri      (501) staff       (20)        0 2023-06-13 17:25:45.058304 OpenFintech-0.0.5/
+-rw-r--r--   0 harri      (501) staff       (20)    11357 2023-06-05 19:27:30.000000 OpenFintech-0.0.5/LICENSE
+drwxr-xr-x   0 harri      (501) staff       (20)        0 2023-06-13 17:25:45.056888 OpenFintech-0.0.5/OpenFintech/
+-rw-r--r--   0 harri      (501) staff       (20)      662 2023-06-13 17:15:54.000000 OpenFintech-0.0.5/OpenFintech/FinData.py
+-rw-r--r--   0 harri      (501) staff       (20)     3704 2023-06-13 17:15:54.000000 OpenFintech-0.0.5/OpenFintech/FinMongo.py
+-rw-r--r--   0 harri      (501) staff       (20)     2459 2023-06-13 17:15:54.000000 OpenFintech-0.0.5/OpenFintech/Market.py
+-rw-r--r--   0 harri      (501) staff       (20)     5492 2023-06-13 17:15:54.000000 OpenFintech-0.0.5/OpenFintech/Model.py
+-rw-r--r--   0 harri      (501) staff       (20)     6865 2023-06-13 17:15:54.000000 OpenFintech-0.0.5/OpenFintech/User.py
+-rw-r--r--   0 harri      (501) staff       (20)      130 2023-06-13 03:54:03.000000 OpenFintech-0.0.5/OpenFintech/__init__.py
+-rw-r--r--   0 harri      (501) staff       (20)      856 2023-06-13 17:04:24.000000 OpenFintech-0.0.5/OpenFintech/utilities.py
+drwxr-xr-x   0 harri      (501) staff       (20)        0 2023-06-13 17:25:45.057840 OpenFintech-0.0.5/OpenFintech.egg-info/
+-rw-r--r--   0 harri      (501) staff       (20)       77 2023-06-13 17:25:45.000000 OpenFintech-0.0.5/OpenFintech.egg-info/PKG-INFO
+-rw-r--r--   0 harri      (501) staff       (20)      325 2023-06-13 17:25:45.000000 OpenFintech-0.0.5/OpenFintech.egg-info/SOURCES.txt
+-rw-r--r--   0 harri      (501) staff       (20)        1 2023-06-13 17:25:45.000000 OpenFintech-0.0.5/OpenFintech.egg-info/dependency_links.txt
+-rw-r--r--   0 harri      (501) staff       (20)       12 2023-06-13 17:25:45.000000 OpenFintech-0.0.5/OpenFintech.egg-info/top_level.txt
+-rw-r--r--   0 harri      (501) staff       (20)       77 2023-06-13 17:25:45.058120 OpenFintech-0.0.5/PKG-INFO
+-rw-r--r--   0 harri      (501) staff       (20)    11338 2023-06-13 17:15:54.000000 OpenFintech-0.0.5/README.md
+-rw-r--r--   0 harri      (501) staff       (20)       38 2023-06-13 17:25:45.058354 OpenFintech-0.0.5/setup.cfg
+-rw-r--r--   0 harri      (501) staff       (20)      128 2023-06-13 17:24:44.000000 OpenFintech-0.0.5/setup.py
```

### Comparing `OpenFintech-0.0.4/LICENSE` & `OpenFintech-0.0.5/LICENSE`

 * *Files identical despite different names*

