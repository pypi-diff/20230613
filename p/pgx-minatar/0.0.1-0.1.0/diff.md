# Comparing `tmp/pgx-minatar-0.0.1.tar.gz` & `tmp/pgx-minatar-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgx-minatar-0.0.1.tar", last modified: Tue Jun 13 08:21:56 2023, max compression
+gzip compressed data, was "pgx-minatar-0.1.0.tar", last modified: Tue Jun 13 08:28:12 2023, max compression
```

## Comparing `pgx-minatar-0.0.1.tar` & `pgx-minatar-0.1.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 koyamada   (502) staff       (20)        0 2023-06-13 08:21:56.552536 pgx-minatar-0.0.1/
--rw-r--r--   0 koyamada   (502) staff       (20)    35149 2023-06-13 07:52:56.000000 pgx-minatar-0.0.1/LICENSE
--rw-r--r--   0 koyamada   (502) staff       (20)      482 2023-06-13 08:21:56.552348 pgx-minatar-0.0.1/PKG-INFO
--rw-r--r--   0 koyamada   (502) staff       (20)       28 2023-06-13 07:52:56.000000 pgx-minatar-0.0.1/README.md
-drwxr-xr-x   0 koyamada   (502) staff       (20)        0 2023-06-13 08:21:56.548128 pgx-minatar-0.0.1/pgx_minatar/
--rw-r--r--   0 koyamada   (502) staff       (20)        0 2023-06-13 07:47:51.000000 pgx-minatar-0.0.1/pgx_minatar/__init__.py
--rw-r--r--   0 koyamada   (502) staff       (20)    12926 2023-06-13 07:47:51.000000 pgx-minatar-0.0.1/pgx_minatar/asterix.py
--rw-r--r--   0 koyamada   (502) staff       (20)     9090 2023-06-13 07:47:51.000000 pgx-minatar-0.0.1/pgx_minatar/breakout.py
--rw-r--r--   0 koyamada   (502) staff       (20)     8762 2023-06-13 07:47:51.000000 pgx-minatar-0.0.1/pgx_minatar/freeway.py
--rw-r--r--   0 koyamada   (502) staff       (20)    25316 2023-06-13 07:47:51.000000 pgx-minatar-0.0.1/pgx_minatar/seaquest.py
--rw-r--r--   0 koyamada   (502) staff       (20)    10042 2023-06-13 07:47:51.000000 pgx-minatar-0.0.1/pgx_minatar/space_invaders.py
--rw-r--r--   0 koyamada   (502) staff       (20)     2382 2023-06-13 07:47:51.000000 pgx-minatar-0.0.1/pgx_minatar/utils.py
-drwxr-xr-x   0 koyamada   (502) staff       (20)        0 2023-06-13 08:21:56.549806 pgx-minatar-0.0.1/pgx_minatar.egg-info/
--rw-r--r--   0 koyamada   (502) staff       (20)      482 2023-06-13 08:21:56.000000 pgx-minatar-0.0.1/pgx_minatar.egg-info/PKG-INFO
--rw-r--r--   0 koyamada   (502) staff       (20)      488 2023-06-13 08:21:56.000000 pgx-minatar-0.0.1/pgx_minatar.egg-info/SOURCES.txt
--rw-r--r--   0 koyamada   (502) staff       (20)        1 2023-06-13 08:21:56.000000 pgx-minatar-0.0.1/pgx_minatar.egg-info/dependency_links.txt
--rw-r--r--   0 koyamada   (502) staff       (20)       34 2023-06-13 08:21:56.000000 pgx-minatar-0.0.1/pgx_minatar.egg-info/requires.txt
--rw-r--r--   0 koyamada   (502) staff       (20)       12 2023-06-13 08:21:56.000000 pgx-minatar-0.0.1/pgx_minatar.egg-info/top_level.txt
--rw-r--r--   0 koyamada   (502) staff       (20)       38 2023-06-13 08:21:56.552585 pgx-minatar-0.0.1/setup.cfg
--rw-r--r--   0 koyamada   (502) staff       (20)      885 2023-06-13 08:19:03.000000 pgx-minatar-0.0.1/setup.py
-drwxr-xr-x   0 koyamada   (502) staff       (20)        0 2023-06-13 08:21:56.551808 pgx-minatar-0.0.1/tests/
--rw-r--r--   0 koyamada   (502) staff       (20)     2818 2023-06-13 07:56:46.000000 pgx-minatar-0.0.1/tests/test_asterix.py
--rw-r--r--   0 koyamada   (502) staff       (20)     2576 2023-06-13 07:57:17.000000 pgx-minatar-0.0.1/tests/test_breakout.py
--rw-r--r--   0 koyamada   (502) staff       (20)     2843 2023-06-13 07:57:24.000000 pgx-minatar-0.0.1/tests/test_freeway.py
--rw-r--r--   0 koyamada   (502) staff       (20)     5374 2023-06-13 07:57:31.000000 pgx-minatar-0.0.1/tests/test_seaquest.py
--rw-r--r--   0 koyamada   (502) staff       (20)     3012 2023-06-13 07:57:38.000000 pgx-minatar-0.0.1/tests/test_space_invaders.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 08:28:12.257532 pgx-minatar-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-13 08:28:01.000000 pgx-minatar-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-13 08:28:12.257532 pgx-minatar-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-13 08:28:01.000000 pgx-minatar-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 08:28:12.253532 pgx-minatar-0.1.0/pgx_minatar/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 08:28:01.000000 pgx-minatar-0.1.0/pgx_minatar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12926 2023-06-13 08:28:01.000000 pgx-minatar-0.1.0/pgx_minatar/asterix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9090 2023-06-13 08:28:01.000000 pgx-minatar-0.1.0/pgx_minatar/breakout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8762 2023-06-13 08:28:01.000000 pgx-minatar-0.1.0/pgx_minatar/freeway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25316 2023-06-13 08:28:01.000000 pgx-minatar-0.1.0/pgx_minatar/seaquest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10042 2023-06-13 08:28:01.000000 pgx-minatar-0.1.0/pgx_minatar/space_invaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-06-13 08:28:01.000000 pgx-minatar-0.1.0/pgx_minatar/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 08:28:12.257532 pgx-minatar-0.1.0/pgx_minatar.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-13 08:28:12.000000 pgx-minatar-0.1.0/pgx_minatar.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-13 08:28:12.000000 pgx-minatar-0.1.0/pgx_minatar.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 08:28:12.000000 pgx-minatar-0.1.0/pgx_minatar.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-13 08:28:12.000000 pgx-minatar-0.1.0/pgx_minatar.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-13 08:28:12.000000 pgx-minatar-0.1.0/pgx_minatar.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 08:28:12.257532 pgx-minatar-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-13 08:28:01.000000 pgx-minatar-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 08:28:12.257532 pgx-minatar-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-06-13 08:28:01.000000 pgx-minatar-0.1.0/tests/test_asterix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-06-13 08:28:01.000000 pgx-minatar-0.1.0/tests/test_breakout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-06-13 08:28:01.000000 pgx-minatar-0.1.0/tests/test_freeway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-06-13 08:28:01.000000 pgx-minatar-0.1.0/tests/test_seaquest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-06-13 08:28:01.000000 pgx-minatar-0.1.0/tests/test_space_invaders.py
```

### Comparing `pgx-minatar-0.0.1/LICENSE` & `pgx-minatar-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pgx-minatar-0.0.1/pgx_minatar/asterix.py` & `pgx-minatar-0.1.0/pgx_minatar/asterix.py`

 * *Files identical despite different names*

### Comparing `pgx-minatar-0.0.1/pgx_minatar/breakout.py` & `pgx-minatar-0.1.0/pgx_minatar/breakout.py`

 * *Files identical despite different names*

### Comparing `pgx-minatar-0.0.1/pgx_minatar/freeway.py` & `pgx-minatar-0.1.0/pgx_minatar/freeway.py`

 * *Files identical despite different names*

### Comparing `pgx-minatar-0.0.1/pgx_minatar/seaquest.py` & `pgx-minatar-0.1.0/pgx_minatar/seaquest.py`

 * *Files identical despite different names*

### Comparing `pgx-minatar-0.0.1/pgx_minatar/space_invaders.py` & `pgx-minatar-0.1.0/pgx_minatar/space_invaders.py`

 * *Files identical despite different names*

### Comparing `pgx-minatar-0.0.1/pgx_minatar/utils.py` & `pgx-minatar-0.1.0/pgx_minatar/utils.py`

 * *Files identical despite different names*

### Comparing `pgx-minatar-0.0.1/setup.py` & `pgx-minatar-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 from pathlib import Path
 
 long_description = (Path(__file__).parent / "README.md").read_text()
 
 setup(
     name="pgx-minatar",
-    version="0.0.1",
+    version="0.1.0",
     description="MinAtar extension of Pgx",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/sotetsuk/pgx-minatar",
     author="Sotetsu KOYAMADA",
     author_email="sotetsu.koyamada@gmail.com",
     keywords="",
```

### Comparing `pgx-minatar-0.0.1/tests/test_asterix.py` & `pgx-minatar-0.1.0/tests/test_asterix.py`

 * *Files identical despite different names*

### Comparing `pgx-minatar-0.0.1/tests/test_breakout.py` & `pgx-minatar-0.1.0/tests/test_breakout.py`

 * *Files identical despite different names*

### Comparing `pgx-minatar-0.0.1/tests/test_freeway.py` & `pgx-minatar-0.1.0/tests/test_freeway.py`

 * *Files identical despite different names*

### Comparing `pgx-minatar-0.0.1/tests/test_seaquest.py` & `pgx-minatar-0.1.0/tests/test_seaquest.py`

 * *Files identical despite different names*

### Comparing `pgx-minatar-0.0.1/tests/test_space_invaders.py` & `pgx-minatar-0.1.0/tests/test_space_invaders.py`

 * *Files identical despite different names*

