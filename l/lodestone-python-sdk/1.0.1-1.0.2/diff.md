# Comparing `tmp/lodestone-python-sdk-1.0.1.tar.gz` & `tmp/lodestone-python-sdk-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lodestone-python-sdk-1.0.1.tar", last modified: Tue Jun 13 07:37:06 2023, max compression
+gzip compressed data, was "lodestone-python-sdk-1.0.2.tar", last modified: Tue Jun 13 07:43:16 2023, max compression
```

## Comparing `lodestone-python-sdk-1.0.1.tar` & `lodestone-python-sdk-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 bocai      (501) staff       (20)        0 2023-06-13 07:37:06.224117 lodestone-python-sdk-1.0.1/
--rw-r--r--   0 bocai      (501) staff       (20)      237 2023-06-13 07:37:06.223987 lodestone-python-sdk-1.0.1/PKG-INFO
--rw-r--r--   0 bocai      (501) staff       (20)       33 2023-06-13 07:02:54.000000 lodestone-python-sdk-1.0.1/README.md
-drwxr-xr-x   0 bocai      (501) staff       (20)        0 2023-06-13 07:37:06.223086 lodestone-python-sdk-1.0.1/lodestone_python_sdk/
--rw-r--r--   0 bocai      (501) staff       (20)        0 2023-06-13 06:22:56.000000 lodestone-python-sdk-1.0.1/lodestone_python_sdk/__init__.py
--rw-r--r--   0 bocai      (501) staff       (20)      954 2023-06-13 06:41:28.000000 lodestone-python-sdk-1.0.1/lodestone_python_sdk/client.py
--rw-r--r--   0 bocai      (501) staff       (20)       42 2023-06-13 03:03:25.000000 lodestone-python-sdk-1.0.1/lodestone_python_sdk/exceptions.py
-drwxr-xr-x   0 bocai      (501) staff       (20)        0 2023-06-13 07:37:06.223810 lodestone-python-sdk-1.0.1/lodestone_python_sdk.egg-info/
--rw-r--r--   0 bocai      (501) staff       (20)      237 2023-06-13 07:37:06.000000 lodestone-python-sdk-1.0.1/lodestone_python_sdk.egg-info/PKG-INFO
--rw-r--r--   0 bocai      (501) staff       (20)      293 2023-06-13 07:37:06.000000 lodestone-python-sdk-1.0.1/lodestone_python_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 bocai      (501) staff       (20)        1 2023-06-13 07:37:06.000000 lodestone-python-sdk-1.0.1/lodestone_python_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 bocai      (501) staff       (20)       21 2023-06-13 07:37:06.000000 lodestone-python-sdk-1.0.1/lodestone_python_sdk.egg-info/top_level.txt
--rw-r--r--   0 bocai      (501) staff       (20)       38 2023-06-13 07:37:06.224168 lodestone-python-sdk-1.0.1/setup.cfg
--rw-r--r--   0 bocai      (501) staff       (20)      397 2023-06-13 07:36:22.000000 lodestone-python-sdk-1.0.1/setup.py
+drwxr-xr-x   0 bocai      (501) staff       (20)        0 2023-06-13 07:43:16.595610 lodestone-python-sdk-1.0.2/
+-rw-r--r--   0 bocai      (501) staff       (20)      303 2023-06-13 07:43:16.595498 lodestone-python-sdk-1.0.2/PKG-INFO
+-rw-r--r--   0 bocai      (501) staff       (20)       33 2023-06-13 07:02:54.000000 lodestone-python-sdk-1.0.2/README.md
+drwxr-xr-x   0 bocai      (501) staff       (20)        0 2023-06-13 07:43:16.594910 lodestone-python-sdk-1.0.2/lodestone_python_sdk/
+-rw-r--r--   0 bocai      (501) staff       (20)        0 2023-06-13 06:22:56.000000 lodestone-python-sdk-1.0.2/lodestone_python_sdk/__init__.py
+-rw-r--r--   0 bocai      (501) staff       (20)      954 2023-06-13 06:41:28.000000 lodestone-python-sdk-1.0.2/lodestone_python_sdk/client.py
+-rw-r--r--   0 bocai      (501) staff       (20)       42 2023-06-13 03:03:25.000000 lodestone-python-sdk-1.0.2/lodestone_python_sdk/exceptions.py
+drwxr-xr-x   0 bocai      (501) staff       (20)        0 2023-06-13 07:43:16.595340 lodestone-python-sdk-1.0.2/lodestone_python_sdk.egg-info/
+-rw-r--r--   0 bocai      (501) staff       (20)      303 2023-06-13 07:43:16.000000 lodestone-python-sdk-1.0.2/lodestone_python_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 bocai      (501) staff       (20)      293 2023-06-13 07:43:16.000000 lodestone-python-sdk-1.0.2/lodestone_python_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 bocai      (501) staff       (20)        1 2023-06-13 07:43:16.000000 lodestone-python-sdk-1.0.2/lodestone_python_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 bocai      (501) staff       (20)       21 2023-06-13 07:43:16.000000 lodestone-python-sdk-1.0.2/lodestone_python_sdk.egg-info/top_level.txt
+-rw-r--r--   0 bocai      (501) staff       (20)       38 2023-06-13 07:43:16.595654 lodestone-python-sdk-1.0.2/setup.cfg
+-rw-r--r--   0 bocai      (501) staff       (20)      477 2023-06-13 07:43:08.000000 lodestone-python-sdk-1.0.2/setup.py
```

### Comparing `lodestone-python-sdk-1.0.1/lodestone_python_sdk/client.py` & `lodestone-python-sdk-1.0.2/lodestone_python_sdk/client.py`

 * *Files identical despite different names*

