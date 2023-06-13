# Comparing `tmp/SpotiStats-0.1.4.tar.gz` & `tmp/SpotiStats-0.1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SpotiStats-0.1.4.tar", last modified: Tue Jun 13 02:47:39 2023, max compression
+gzip compressed data, was "SpotiStats-0.1.4.1.tar", last modified: Tue Jun 13 02:55:10 2023, max compression
```

## Comparing `SpotiStats-0.1.4.tar` & `SpotiStats-0.1.4.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 jaydenpyles   (501) staff       (20)        0 2023-06-13 02:47:39.548394 SpotiStats-0.1.4/
--rw-r--r--   0 jaydenpyles   (501) staff       (20)      512 2023-06-13 02:47:39.547971 SpotiStats-0.1.4/PKG-INFO
--rw-r--r--   0 jaydenpyles   (501) staff       (20)      331 2023-06-12 15:17:38.000000 SpotiStats-0.1.4/README.md
-drwxr-xr-x   0 jaydenpyles   (501) staff       (20)        0 2023-06-13 02:47:39.546033 SpotiStats-0.1.4/SpotiStats/
--rw-r--r--   0 jaydenpyles   (501) staff       (20)       69 2023-06-10 23:30:35.000000 SpotiStats-0.1.4/SpotiStats/__init__.py
--rw-r--r--   0 jaydenpyles   (501) staff       (20)     1057 2023-06-13 02:33:36.000000 SpotiStats-0.1.4/SpotiStats/__main__.py
--rw-r--r--   0 jaydenpyles   (501) staff       (20)       81 2023-06-10 23:30:35.000000 SpotiStats-0.1.4/SpotiStats/exceptions.py
--rw-r--r--   0 jaydenpyles   (501) staff       (20)     6228 2023-06-10 23:30:35.000000 SpotiStats-0.1.4/SpotiStats/spotify.py
--rw-r--r--   0 jaydenpyles   (501) staff       (20)      298 2023-06-10 23:30:35.000000 SpotiStats-0.1.4/SpotiStats/test.py
-drwxr-xr-x   0 jaydenpyles   (501) staff       (20)        0 2023-06-13 02:47:39.547442 SpotiStats-0.1.4/SpotiStats.egg-info/
--rw-r--r--   0 jaydenpyles   (501) staff       (20)      512 2023-06-13 02:47:39.000000 SpotiStats-0.1.4/SpotiStats.egg-info/PKG-INFO
--rw-r--r--   0 jaydenpyles   (501) staff       (20)      272 2023-06-13 02:47:39.000000 SpotiStats-0.1.4/SpotiStats.egg-info/SOURCES.txt
--rw-r--r--   0 jaydenpyles   (501) staff       (20)        1 2023-06-13 02:47:39.000000 SpotiStats-0.1.4/SpotiStats.egg-info/dependency_links.txt
--rw-r--r--   0 jaydenpyles   (501) staff       (20)       11 2023-06-13 02:47:39.000000 SpotiStats-0.1.4/SpotiStats.egg-info/top_level.txt
--rw-r--r--   0 jaydenpyles   (501) staff       (20)      577 2023-06-13 02:47:29.000000 SpotiStats-0.1.4/pyproject.toml
--rw-r--r--   0 jaydenpyles   (501) staff       (20)       38 2023-06-13 02:47:39.548519 SpotiStats-0.1.4/setup.cfg
+drwxr-xr-x   0 jaydenpyles   (501) staff       (20)        0 2023-06-13 02:55:10.510759 SpotiStats-0.1.4.1/
+-rw-r--r--   0 jaydenpyles   (501) staff       (20)      514 2023-06-13 02:55:10.510326 SpotiStats-0.1.4.1/PKG-INFO
+-rw-r--r--   0 jaydenpyles   (501) staff       (20)      331 2023-06-12 15:17:38.000000 SpotiStats-0.1.4.1/README.md
+drwxr-xr-x   0 jaydenpyles   (501) staff       (20)        0 2023-06-13 02:55:10.508233 SpotiStats-0.1.4.1/SpotiStats/
+-rw-r--r--   0 jaydenpyles   (501) staff       (20)       69 2023-06-10 23:30:35.000000 SpotiStats-0.1.4.1/SpotiStats/__init__.py
+-rw-r--r--   0 jaydenpyles   (501) staff       (20)     1057 2023-06-13 02:33:36.000000 SpotiStats-0.1.4.1/SpotiStats/__main__.py
+-rw-r--r--   0 jaydenpyles   (501) staff       (20)       81 2023-06-10 23:30:35.000000 SpotiStats-0.1.4.1/SpotiStats/exceptions.py
+-rw-r--r--   0 jaydenpyles   (501) staff       (20)     6228 2023-06-10 23:30:35.000000 SpotiStats-0.1.4.1/SpotiStats/spotify.py
+-rw-r--r--   0 jaydenpyles   (501) staff       (20)      298 2023-06-10 23:30:35.000000 SpotiStats-0.1.4.1/SpotiStats/test.py
+drwxr-xr-x   0 jaydenpyles   (501) staff       (20)        0 2023-06-13 02:55:10.509900 SpotiStats-0.1.4.1/SpotiStats.egg-info/
+-rw-r--r--   0 jaydenpyles   (501) staff       (20)      514 2023-06-13 02:55:10.000000 SpotiStats-0.1.4.1/SpotiStats.egg-info/PKG-INFO
+-rw-r--r--   0 jaydenpyles   (501) staff       (20)      272 2023-06-13 02:55:10.000000 SpotiStats-0.1.4.1/SpotiStats.egg-info/SOURCES.txt
+-rw-r--r--   0 jaydenpyles   (501) staff       (20)        1 2023-06-13 02:55:10.000000 SpotiStats-0.1.4.1/SpotiStats.egg-info/dependency_links.txt
+-rw-r--r--   0 jaydenpyles   (501) staff       (20)       11 2023-06-13 02:55:10.000000 SpotiStats-0.1.4.1/SpotiStats.egg-info/top_level.txt
+-rw-r--r--   0 jaydenpyles   (501) staff       (20)      579 2023-06-13 02:54:56.000000 SpotiStats-0.1.4.1/pyproject.toml
+-rw-r--r--   0 jaydenpyles   (501) staff       (20)       38 2023-06-13 02:55:10.510860 SpotiStats-0.1.4.1/setup.cfg
```

### Comparing `SpotiStats-0.1.4/PKG-INFO` & `SpotiStats-0.1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SpotiStats
-Version: 0.1.4
+Version: 0.1.4.1
 Author-email: jaypyles <jpylesbusiness@gmail.com>
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # SpotiStats
```

### Comparing `SpotiStats-0.1.4/SpotiStats/__main__.py` & `SpotiStats-0.1.4.1/SpotiStats/__main__.py`

 * *Files identical despite different names*

### Comparing `SpotiStats-0.1.4/SpotiStats/spotify.py` & `SpotiStats-0.1.4.1/SpotiStats/spotify.py`

 * *Files identical despite different names*

### Comparing `SpotiStats-0.1.4/SpotiStats.egg-info/PKG-INFO` & `SpotiStats-0.1.4.1/SpotiStats.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SpotiStats
-Version: 0.1.4
+Version: 0.1.4.1
 Author-email: jaypyles <jpylesbusiness@gmail.com>
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # SpotiStats
```

### Comparing `SpotiStats-0.1.4/pyproject.toml` & `SpotiStats-0.1.4.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "SpotiStats"
-version = "0.1.4"
+version = "0.1.4.1"
 description = ""
 authors = [
     { name = "jaypyles", email = "jpylesbusiness@gmail.com" },
 ]
 requires-python = ">=3.9"
 readme = "README.md"
 license = { text = "MIT" }
```

