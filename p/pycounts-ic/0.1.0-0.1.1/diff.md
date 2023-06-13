# Comparing `tmp/pycounts_ic-0.1.0.tar.gz` & `tmp/pycounts_ic-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycounts_ic-0.1.0.tar", max compression
+gzip compressed data, was "pycounts_ic-0.1.1.tar", max compression
```

## Comparing `pycounts_ic-0.1.0.tar` & `pycounts_ic-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rwxr-xr-x   0        0        0     1070 2023-06-10 13:23:17.893441 pycounts_ic-0.1.0/LICENSE
--rw-r--r--   0        0        0      971 2023-06-10 19:27:15.116818 pycounts_ic-0.1.0/README.md
--rw-r--r--   0        0        0      563 2023-06-10 19:58:19.348236 pycounts_ic-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      113 2023-06-10 13:23:17.988842 pycounts_ic-0.1.0/src/pycounts_ic/__init__.py
--rw-r--r--   0        0        0      789 2023-06-10 19:35:46.982581 pycounts_ic-0.1.0/src/pycounts_ic/plotting.py
--rw-r--r--   0        0        0     1350 2023-06-10 19:37:12.060312 pycounts_ic-0.1.0/src/pycounts_ic/pycounts_ic.py
--rw-r--r--   0        0        0     1416 1970-01-01 00:00:00.000000 pycounts_ic-0.1.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1070 2023-06-10 13:23:17.893441 pycounts_ic-0.1.1/LICENSE
+-rw-r--r--   0        0        0      971 2023-06-10 19:27:15.116818 pycounts_ic-0.1.1/README.md
+-rw-r--r--   0        0        0     1238 2023-06-13 10:06:28.949320 pycounts_ic-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      113 2023-06-10 13:23:17.988842 pycounts_ic-0.1.1/src/pycounts_ic/__init__.py
+-rw-r--r--   0        0        0      789 2023-06-10 19:35:46.982581 pycounts_ic-0.1.1/src/pycounts_ic/plotting.py
+-rw-r--r--   0        0        0     1350 2023-06-10 19:37:12.060312 pycounts_ic-0.1.1/src/pycounts_ic/pycounts_ic.py
+-rw-r--r--   0        0        0     1416 1970-01-01 00:00:00.000000 pycounts_ic-0.1.1/PKG-INFO
```

### Comparing `pycounts_ic-0.1.0/LICENSE` & `pycounts_ic-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pycounts_ic-0.1.0/README.md` & `pycounts_ic-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pycounts_ic-0.1.0/src/pycounts_ic/plotting.py` & `pycounts_ic-0.1.1/src/pycounts_ic/plotting.py`

 * *Files identical despite different names*

### Comparing `pycounts_ic-0.1.0/src/pycounts_ic/pycounts_ic.py` & `pycounts_ic-0.1.1/src/pycounts_ic/pycounts_ic.py`

 * *Files identical despite different names*

### Comparing `pycounts_ic-0.1.0/PKG-INFO` & `pycounts_ic-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycounts-ic
-Version: 0.1.0
+Version: 0.1.1
 Summary: Calculate word counts in a text file.
 License: MIT
 Author: Ivo Camargo
 Requires-Python: >=3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

