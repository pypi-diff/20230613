# Comparing `tmp/SpotiStats-0.1.2.tar.gz` & `tmp/SpotiStats-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SpotiStats-0.1.2.tar", last modified: Mon Apr  3 23:23:15 2023, max compression
+gzip compressed data, was "SpotiStats-0.1.3.tar", last modified: Tue Jun 13 02:34:57 2023, max compression
```

## Comparing `SpotiStats-0.1.2.tar` & `SpotiStats-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 jaydenpyles   (501) staff       (20)        0 2023-04-03 23:23:15.983439 SpotiStats-0.1.2/
--rw-r--r--   0 jaydenpyles   (501) staff       (20)      196 2023-04-03 23:23:15.982914 SpotiStats-0.1.2/PKG-INFO
--rw-r--r--   0 jaydenpyles   (501) staff       (20)       15 2023-04-03 23:15:32.000000 SpotiStats-0.1.2/README.md
-drwxr-xr-x   0 jaydenpyles   (501) staff       (20)        0 2023-04-03 23:23:15.980487 SpotiStats-0.1.2/SpotiStats/
--rw-r--r--   0 jaydenpyles   (501) staff       (20)       69 2023-04-03 20:08:26.000000 SpotiStats-0.1.2/SpotiStats/__init__.py
--rw-r--r--   0 jaydenpyles   (501) staff       (20)     1084 2023-04-03 22:19:33.000000 SpotiStats-0.1.2/SpotiStats/__main__.py
--rw-r--r--   0 jaydenpyles   (501) staff       (20)       81 2023-04-03 20:05:58.000000 SpotiStats-0.1.2/SpotiStats/exceptions.py
--rw-r--r--   0 jaydenpyles   (501) staff       (20)     6228 2023-04-03 22:21:44.000000 SpotiStats-0.1.2/SpotiStats/spotify.py
--rw-r--r--   0 jaydenpyles   (501) staff       (20)      298 2023-04-03 21:23:14.000000 SpotiStats-0.1.2/SpotiStats/test.py
-drwxr-xr-x   0 jaydenpyles   (501) staff       (20)        0 2023-04-03 23:23:15.982409 SpotiStats-0.1.2/SpotiStats.egg-info/
--rw-r--r--   0 jaydenpyles   (501) staff       (20)      196 2023-04-03 23:23:15.000000 SpotiStats-0.1.2/SpotiStats.egg-info/PKG-INFO
--rw-r--r--   0 jaydenpyles   (501) staff       (20)      305 2023-04-03 23:23:15.000000 SpotiStats-0.1.2/SpotiStats.egg-info/SOURCES.txt
--rw-r--r--   0 jaydenpyles   (501) staff       (20)        1 2023-04-03 23:23:15.000000 SpotiStats-0.1.2/SpotiStats.egg-info/dependency_links.txt
--rw-r--r--   0 jaydenpyles   (501) staff       (20)       41 2023-04-03 23:23:15.000000 SpotiStats-0.1.2/SpotiStats.egg-info/requires.txt
--rw-r--r--   0 jaydenpyles   (501) staff       (20)       11 2023-04-03 23:23:15.000000 SpotiStats-0.1.2/SpotiStats.egg-info/top_level.txt
--rw-r--r--   0 jaydenpyles   (501) staff       (20)      452 2023-04-03 23:22:26.000000 SpotiStats-0.1.2/pyproject.toml
--rw-r--r--   0 jaydenpyles   (501) staff       (20)       38 2023-04-03 23:23:15.983588 SpotiStats-0.1.2/setup.cfg
+drwxr-xr-x   0 jaydenpyles   (501) staff       (20)        0 2023-06-13 02:34:57.348127 SpotiStats-0.1.3/
+-rw-r--r--   0 jaydenpyles   (501) staff       (20)      512 2023-06-13 02:34:57.347631 SpotiStats-0.1.3/PKG-INFO
+-rw-r--r--   0 jaydenpyles   (501) staff       (20)      331 2023-06-12 15:17:38.000000 SpotiStats-0.1.3/README.md
+drwxr-xr-x   0 jaydenpyles   (501) staff       (20)        0 2023-06-13 02:34:57.344994 SpotiStats-0.1.3/SpotiStats/
+-rw-r--r--   0 jaydenpyles   (501) staff       (20)       69 2023-06-10 23:30:35.000000 SpotiStats-0.1.3/SpotiStats/__init__.py
+-rw-r--r--   0 jaydenpyles   (501) staff       (20)     1057 2023-06-13 02:33:36.000000 SpotiStats-0.1.3/SpotiStats/__main__.py
+-rw-r--r--   0 jaydenpyles   (501) staff       (20)       81 2023-06-10 23:30:35.000000 SpotiStats-0.1.3/SpotiStats/exceptions.py
+-rw-r--r--   0 jaydenpyles   (501) staff       (20)     6228 2023-06-10 23:30:35.000000 SpotiStats-0.1.3/SpotiStats/spotify.py
+-rw-r--r--   0 jaydenpyles   (501) staff       (20)      298 2023-06-10 23:30:35.000000 SpotiStats-0.1.3/SpotiStats/test.py
+drwxr-xr-x   0 jaydenpyles   (501) staff       (20)        0 2023-06-13 02:34:57.347029 SpotiStats-0.1.3/SpotiStats.egg-info/
+-rw-r--r--   0 jaydenpyles   (501) staff       (20)      512 2023-06-13 02:34:57.000000 SpotiStats-0.1.3/SpotiStats.egg-info/PKG-INFO
+-rw-r--r--   0 jaydenpyles   (501) staff       (20)      305 2023-06-13 02:34:57.000000 SpotiStats-0.1.3/SpotiStats.egg-info/SOURCES.txt
+-rw-r--r--   0 jaydenpyles   (501) staff       (20)        1 2023-06-13 02:34:57.000000 SpotiStats-0.1.3/SpotiStats.egg-info/dependency_links.txt
+-rw-r--r--   0 jaydenpyles   (501) staff       (20)       41 2023-06-13 02:34:57.000000 SpotiStats-0.1.3/SpotiStats.egg-info/requires.txt
+-rw-r--r--   0 jaydenpyles   (501) staff       (20)       11 2023-06-13 02:34:57.000000 SpotiStats-0.1.3/SpotiStats.egg-info/top_level.txt
+-rw-r--r--   0 jaydenpyles   (501) staff       (20)      452 2023-06-13 02:34:49.000000 SpotiStats-0.1.3/pyproject.toml
+-rw-r--r--   0 jaydenpyles   (501) staff       (20)       38 2023-06-13 02:34:57.348288 SpotiStats-0.1.3/setup.cfg
```

### Comparing `SpotiStats-0.1.2/SpotiStats/__main__.py` & `SpotiStats-0.1.3/SpotiStats/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
+import os
 import webbrowser
+
 import click
 from dotenv import load_dotenv
-import os
-from webbrowser import open
 
 from SpotiStats.spotify import Authenticator, Spotify
 
 load_dotenv()
 CLIENT_ID = os.environ["CLIENT_ID"]
 CLIENT_SECRET = os.environ["CLIENT_SECRET"]
 auth = Authenticator(CLIENT_ID, CLIENT_SECRET)
```

### Comparing `SpotiStats-0.1.2/SpotiStats/spotify.py` & `SpotiStats-0.1.3/SpotiStats/spotify.py`

 * *Files identical despite different names*

