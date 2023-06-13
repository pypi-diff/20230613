# Comparing `tmp/tiktok-dlpy-1.1.0.tar.gz` & `tmp/tiktok-dlpy-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiktok-dlpy-1.1.0.tar", last modified: Mon Jun 12 14:01:27 2023, max compression
+gzip compressed data, was "tiktok-dlpy-1.1.1.tar", last modified: Tue Jun 13 06:44:27 2023, max compression
```

## Comparing `tiktok-dlpy-1.1.0.tar` & `tiktok-dlpy-1.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 becky      (501) staff       (20)        0 2023-06-12 14:01:27.518151 tiktok-dlpy-1.1.0/
--rw-r--r--   0 becky      (501) staff       (20)     1082 2023-05-26 11:18:26.000000 tiktok-dlpy-1.1.0/LICENSE
--rw-r--r--   0 becky      (501) staff       (20)     1031 2023-06-12 14:01:27.518198 tiktok-dlpy-1.1.0/PKG-INFO
--rw-r--r--   0 becky      (501) staff       (20)      484 2023-06-12 13:55:00.000000 tiktok-dlpy-1.1.0/README.md
--rw-r--r--   0 becky      (501) staff       (20)       79 2023-06-12 14:01:27.518366 tiktok-dlpy-1.1.0/setup.cfg
--rw-r--r--   0 becky      (501) staff       (20)      873 2023-06-12 14:01:20.000000 tiktok-dlpy-1.1.0/setup.py
-drwxr-xr-x   0 becky      (501) staff       (20)        0 2023-06-12 14:01:27.516919 tiktok-dlpy-1.1.0/tiktok_dlpy.egg-info/
--rw-r--r--   0 becky      (501) staff       (20)     1031 2023-06-12 14:01:27.000000 tiktok-dlpy-1.1.0/tiktok_dlpy.egg-info/PKG-INFO
--rw-r--r--   0 becky      (501) staff       (20)      333 2023-06-12 14:01:27.000000 tiktok-dlpy-1.1.0/tiktok_dlpy.egg-info/SOURCES.txt
--rw-r--r--   0 becky      (501) staff       (20)        1 2023-06-12 14:01:27.000000 tiktok-dlpy-1.1.0/tiktok_dlpy.egg-info/dependency_links.txt
--rw-r--r--   0 becky      (501) staff       (20)       40 2023-06-12 14:01:27.000000 tiktok-dlpy-1.1.0/tiktok_dlpy.egg-info/requires.txt
--rw-r--r--   0 becky      (501) staff       (20)        9 2023-06-12 14:01:27.000000 tiktok-dlpy-1.1.0/tiktok_dlpy.egg-info/top_level.txt
-drwxr-xr-x   0 becky      (501) staff       (20)        0 2023-06-12 14:01:27.517913 tiktok-dlpy-1.1.0/tiktokdl/
--rw-r--r--   0 becky      (501) staff       (20)       22 2023-05-27 18:10:11.000000 tiktok-dlpy-1.1.0/tiktokdl/__init__.py
--rw-r--r--   0 becky      (501) staff       (20)    11880 2023-06-12 11:37:03.000000 tiktok-dlpy-1.1.0/tiktokdl/download_video.py
--rw-r--r--   0 becky      (501) staff       (20)      288 2023-05-26 12:24:58.000000 tiktok-dlpy-1.1.0/tiktokdl/exceptions.py
--rw-r--r--   0 becky      (501) staff       (20)     2141 2023-05-26 12:21:24.000000 tiktok-dlpy-1.1.0/tiktokdl/image_processing.py
--rw-r--r--   0 becky      (501) staff       (20)      443 2023-06-11 17:49:11.000000 tiktok-dlpy-1.1.0/tiktokdl/video_data.py
+drwxr-xr-x   0 becky      (501) staff       (20)        0 2023-06-13 06:44:27.299894 tiktok-dlpy-1.1.1/
+-rw-r--r--   0 becky      (501) staff       (20)     1082 2023-05-26 11:18:26.000000 tiktok-dlpy-1.1.1/LICENSE
+-rw-r--r--   0 becky      (501) staff       (20)      506 2023-06-13 06:44:27.299941 tiktok-dlpy-1.1.1/PKG-INFO
+-rw-r--r--   0 becky      (501) staff       (20)      487 2023-06-12 14:02:52.000000 tiktok-dlpy-1.1.1/README.md
+-rw-r--r--   0 becky      (501) staff       (20)       79 2023-06-13 06:44:27.300107 tiktok-dlpy-1.1.1/setup.cfg
+-rw-r--r--   0 becky      (501) staff       (20)      766 2023-06-13 06:40:41.000000 tiktok-dlpy-1.1.1/setup.py
+drwxr-xr-x   0 becky      (501) staff       (20)        0 2023-06-13 06:44:27.298672 tiktok-dlpy-1.1.1/tiktok_dlpy.egg-info/
+-rw-r--r--   0 becky      (501) staff       (20)      506 2023-06-13 06:44:27.000000 tiktok-dlpy-1.1.1/tiktok_dlpy.egg-info/PKG-INFO
+-rw-r--r--   0 becky      (501) staff       (20)      333 2023-06-13 06:44:27.000000 tiktok-dlpy-1.1.1/tiktok_dlpy.egg-info/SOURCES.txt
+-rw-r--r--   0 becky      (501) staff       (20)        1 2023-06-13 06:44:27.000000 tiktok-dlpy-1.1.1/tiktok_dlpy.egg-info/dependency_links.txt
+-rw-r--r--   0 becky      (501) staff       (20)       40 2023-06-13 06:44:27.000000 tiktok-dlpy-1.1.1/tiktok_dlpy.egg-info/requires.txt
+-rw-r--r--   0 becky      (501) staff       (20)        9 2023-06-13 06:44:27.000000 tiktok-dlpy-1.1.1/tiktok_dlpy.egg-info/top_level.txt
+drwxr-xr-x   0 becky      (501) staff       (20)        0 2023-06-13 06:44:27.299677 tiktok-dlpy-1.1.1/tiktokdl/
+-rw-r--r--   0 becky      (501) staff       (20)       22 2023-05-27 18:10:11.000000 tiktok-dlpy-1.1.1/tiktokdl/__init__.py
+-rw-r--r--   0 becky      (501) staff       (20)    11880 2023-06-12 11:37:03.000000 tiktok-dlpy-1.1.1/tiktokdl/download_video.py
+-rw-r--r--   0 becky      (501) staff       (20)      288 2023-05-26 12:24:58.000000 tiktok-dlpy-1.1.1/tiktokdl/exceptions.py
+-rw-r--r--   0 becky      (501) staff       (20)     2141 2023-05-26 12:21:24.000000 tiktok-dlpy-1.1.1/tiktokdl/image_processing.py
+-rw-r--r--   0 becky      (501) staff       (20)      443 2023-06-11 17:49:11.000000 tiktok-dlpy-1.1.1/tiktokdl/video_data.py
```

### Comparing `tiktok-dlpy-1.1.0/LICENSE` & `tiktok-dlpy-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tiktok-dlpy-1.1.0/tiktokdl/download_video.py` & `tiktok-dlpy-1.1.1/tiktokdl/download_video.py`

 * *Files identical despite different names*

### Comparing `tiktok-dlpy-1.1.0/tiktokdl/image_processing.py` & `tiktok-dlpy-1.1.1/tiktokdl/image_processing.py`

 * *Files identical despite different names*

