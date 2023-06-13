# Comparing `tmp/YTRequests-1.0.2-1.tar.gz` & `tmp/YTRequests-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/YTRequests-1.0.2.tar", last modified: Thu May 26 00:27:06 2022, max compression
+gzip compressed data, was "YTRequests-1.0.3.tar", last modified: Tue Jun 13 07:07:41 2023, max compression
```

## Comparing `YTRequests-1.0.2-1.tar` & `YTRequests-1.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 tsubasaami   (501) staff       (20)        0 2022-05-26 00:27:06.000000 YTRequests-1.0.2/
--rw-r--r--   0 tsubasaami   (501) staff       (20)     1067 2022-05-26 00:26:19.000000 YTRequests-1.0.2/LICENSE
--rw-r--r--   0 tsubasaami   (501) staff       (20)      338 2022-05-26 00:27:06.000000 YTRequests-1.0.2/PKG-INFO
-drwxr-xr-x   0 tsubasaami   (501) staff       (20)        0 2022-05-26 00:27:06.000000 YTRequests-1.0.2/YTRequests/
--rw-r--r--   0 tsubasaami   (501) staff       (20)       44 2022-05-12 16:38:04.000000 YTRequests-1.0.2/YTRequests/__init__.py
--rw-r--r--   0 tsubasaami   (501) staff       (20)     5681 2022-05-26 00:07:23.000000 YTRequests-1.0.2/YTRequests/ytrequests.py
-drwxr-xr-x   0 tsubasaami   (501) staff       (20)        0 2022-05-26 00:27:06.000000 YTRequests-1.0.2/YTRequests.egg-info/
--rw-r--r--   0 tsubasaami   (501) staff       (20)      338 2022-05-26 00:27:06.000000 YTRequests-1.0.2/YTRequests.egg-info/PKG-INFO
--rw-r--r--   0 tsubasaami   (501) staff       (20)      233 2022-05-26 00:27:06.000000 YTRequests-1.0.2/YTRequests.egg-info/SOURCES.txt
--rw-r--r--   0 tsubasaami   (501) staff       (20)        1 2022-05-26 00:27:06.000000 YTRequests-1.0.2/YTRequests.egg-info/dependency_links.txt
--rw-r--r--   0 tsubasaami   (501) staff       (20)        9 2022-05-26 00:27:06.000000 YTRequests-1.0.2/YTRequests.egg-info/requires.txt
--rw-r--r--   0 tsubasaami   (501) staff       (20)       11 2022-05-26 00:27:06.000000 YTRequests-1.0.2/YTRequests.egg-info/top_level.txt
--rw-r--r--   0 tsubasaami   (501) staff       (20)       38 2022-05-26 00:27:06.000000 YTRequests-1.0.2/setup.cfg
--rw-r--r--   0 tsubasaami   (501) staff       (20)      523 2022-05-26 00:12:40.000000 YTRequests-1.0.2/setup.py
+drwxr-xr-x   0 tsubasaami   (501) staff       (20)        0 2023-06-13 07:07:41.431581 YTRequests-1.0.3/
+-rw-r--r--   0 tsubasaami   (501) staff       (20)     1067 2023-06-13 06:48:33.000000 YTRequests-1.0.3/LICENSE
+-rw-r--r--   0 tsubasaami   (501) staff       (20)      338 2023-06-13 07:07:41.431449 YTRequests-1.0.3/PKG-INFO
+drwxr-xr-x   0 tsubasaami   (501) staff       (20)        0 2023-06-13 07:07:41.430679 YTRequests-1.0.3/YTRequests/
+-rw-r--r--   0 tsubasaami   (501) staff       (20)       44 2023-06-13 06:48:33.000000 YTRequests-1.0.3/YTRequests/__init__.py
+-rw-r--r--   0 tsubasaami   (501) staff       (20)     5681 2023-06-13 06:48:33.000000 YTRequests-1.0.3/YTRequests/ytrequests.py
+drwxr-xr-x   0 tsubasaami   (501) staff       (20)        0 2023-06-13 07:07:41.431276 YTRequests-1.0.3/YTRequests.egg-info/
+-rw-r--r--   0 tsubasaami   (501) staff       (20)      338 2023-06-13 07:07:41.000000 YTRequests-1.0.3/YTRequests.egg-info/PKG-INFO
+-rw-r--r--   0 tsubasaami   (501) staff       (20)      233 2023-06-13 07:07:41.000000 YTRequests-1.0.3/YTRequests.egg-info/SOURCES.txt
+-rw-r--r--   0 tsubasaami   (501) staff       (20)        1 2023-06-13 07:07:41.000000 YTRequests-1.0.3/YTRequests.egg-info/dependency_links.txt
+-rw-r--r--   0 tsubasaami   (501) staff       (20)        9 2023-06-13 07:07:41.000000 YTRequests-1.0.3/YTRequests.egg-info/requires.txt
+-rw-r--r--   0 tsubasaami   (501) staff       (20)       11 2023-06-13 07:07:41.000000 YTRequests-1.0.3/YTRequests.egg-info/top_level.txt
+-rw-r--r--   0 tsubasaami   (501) staff       (20)       38 2023-06-13 07:07:41.431634 YTRequests-1.0.3/setup.cfg
+-rw-r--r--   0 tsubasaami   (501) staff       (20)      498 2023-06-13 07:07:38.000000 YTRequests-1.0.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `YTRequests-1.0.2/LICENSE` & `YTRequests-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `YTRequests-1.0.2/YTRequests/ytrequests.py` & `YTRequests-1.0.3/YTRequests/ytrequests.py`

 * *Files identical despite different names*

