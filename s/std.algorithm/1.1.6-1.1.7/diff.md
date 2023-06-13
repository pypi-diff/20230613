# Comparing `tmp/std.algorithm-1.1.6.tar.gz` & `tmp/std.algorithm-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "std.algorithm-1.1.6.tar", last modified: Tue Jun 13 03:21:12 2023, max compression
+gzip compressed data, was "std.algorithm-1.1.7.tar", last modified: Tue Jun 13 06:01:09 2023, max compression
```

## Comparing `std.algorithm-1.1.6.tar` & `std.algorithm-1.1.7.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 03:21:12.698940 std.algorithm-1.1.6/
--rw-rw-rw-   0        0        0      324 2023-06-13 03:21:12.698940 std.algorithm-1.1.6/PKG-INFO
--rw-rw-rw-   0        0        0       47 2022-10-13 00:41:19.000000 std.algorithm-1.1.6/README.md
--rw-rw-rw-   0        0        0      312 2023-06-13 03:21:12.699943 std.algorithm-1.1.6/setup.cfg
--rw-rw-rw-   0        0        0      478 2023-03-01 06:13:36.000000 std.algorithm-1.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-13 03:21:12.681594 std.algorithm-1.1.6/std/
--rw-rw-rw-   0        0        0    14485 2023-06-05 00:56:34.000000 std.algorithm-1.1.6/std/MySQL.py
--rw-rw-rw-   0        0        0    20878 2023-06-09 00:47:00.000000 std.algorithm-1.1.6/std/__init__.py
--rw-rw-rw-   0        0        0     2276 2023-04-19 00:57:44.000000 std.algorithm-1.1.6/std/combinatorics.py
--rw-rw-rw-   0        0        0     2819 2023-05-15 01:39:31.000000 std.algorithm-1.1.6/std/data.py
--rw-rw-rw-   0        0        0      202 2022-10-13 00:41:19.000000 std.algorithm-1.1.6/std/error.py
--rw-rw-rw-   0        0        0     8575 2023-06-06 01:16:49.000000 std.algorithm-1.1.6/std/file.py
--rw-rw-rw-   0        0        0     1754 2023-03-01 06:13:03.000000 std.algorithm-1.1.6/std/http.py
--rw-rw-rw-   0        0        0    39618 2023-05-24 03:29:48.000000 std.algorithm-1.1.6/std/keras.py
-drwxrwxrwx   0        0        0        0 2023-06-13 03:21:12.691589 std.algorithm-1.1.6/std/lib/
--rw-rw-rw-   0        0        0  2220528 2022-10-21 02:36:11.000000 std.algorithm-1.1.6/std/lib/eigen.dll
--rw-rw-rw-   0        0        0    13812 2023-06-13 03:09:24.000000 std.algorithm-1.1.6/std/nlp.py
--rw-rw-rw-   0        0        0       89 2023-03-07 01:03:31.000000 std.algorithm-1.1.6/std/regexp.py
--rw-rw-rw-   0        0        0      740 2022-10-13 00:41:19.000000 std.algorithm-1.1.6/std/search.py
--rw-rw-rw-   0        0        0    19454 2023-03-08 09:05:45.000000 std.algorithm-1.1.6/std/sets.py
--rw-rw-rw-   0        0        0     1162 2022-10-13 00:41:19.000000 std.algorithm-1.1.6/std/tree.py
--rw-rw-rw-   0        0        0      443 2023-03-16 02:15:53.000000 std.algorithm-1.1.6/std/unicode.py
--rw-rw-rw-   0        0        0    35286 2023-02-02 07:42:54.000000 std.algorithm-1.1.6/std/xml.py
-drwxrwxrwx   0        0        0        0 2023-06-13 03:21:12.690590 std.algorithm-1.1.6/std.algorithm.egg-info/
--rw-rw-rw-   0        0        0      324 2023-06-13 03:21:11.000000 std.algorithm-1.1.6/std.algorithm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      431 2023-06-13 03:21:11.000000 std.algorithm-1.1.6/std.algorithm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 03:21:11.000000 std.algorithm-1.1.6/std.algorithm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-13 03:21:11.000000 std.algorithm-1.1.6/std.algorithm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-06-13 03:21:11.000000 std.algorithm-1.1.6/std.algorithm.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-13 06:01:09.891359 std.algorithm-1.1.7/
+-rw-rw-rw-   0        0        0      324 2023-06-13 06:01:09.891359 std.algorithm-1.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0       47 2022-10-13 00:41:19.000000 std.algorithm-1.1.7/README.md
+-rw-rw-rw-   0        0        0      312 2023-06-13 06:01:09.892359 std.algorithm-1.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      478 2023-03-01 06:13:36.000000 std.algorithm-1.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 06:01:09.881366 std.algorithm-1.1.7/std/
+-rw-rw-rw-   0        0        0    14485 2023-06-05 00:56:34.000000 std.algorithm-1.1.7/std/MySQL.py
+-rw-rw-rw-   0        0        0    20878 2023-06-09 00:47:00.000000 std.algorithm-1.1.7/std/__init__.py
+-rw-rw-rw-   0        0        0     2276 2023-04-19 00:57:44.000000 std.algorithm-1.1.7/std/combinatorics.py
+-rw-rw-rw-   0        0        0     2819 2023-05-15 01:39:31.000000 std.algorithm-1.1.7/std/data.py
+-rw-rw-rw-   0        0        0      202 2022-10-13 00:41:19.000000 std.algorithm-1.1.7/std/error.py
+-rw-rw-rw-   0        0        0     8575 2023-06-13 06:00:00.000000 std.algorithm-1.1.7/std/file.py
+-rw-rw-rw-   0        0        0     1754 2023-03-01 06:13:03.000000 std.algorithm-1.1.7/std/http.py
+-rw-rw-rw-   0        0        0    39618 2023-05-24 03:29:48.000000 std.algorithm-1.1.7/std/keras.py
+drwxrwxrwx   0        0        0        0 2023-06-13 06:01:09.887362 std.algorithm-1.1.7/std/lib/
+-rw-rw-rw-   0        0        0  2220528 2022-10-21 02:36:11.000000 std.algorithm-1.1.7/std/lib/eigen.dll
+-rw-rw-rw-   0        0        0    13812 2023-06-13 03:09:24.000000 std.algorithm-1.1.7/std/nlp.py
+-rw-rw-rw-   0        0        0       89 2023-03-07 01:03:31.000000 std.algorithm-1.1.7/std/regexp.py
+-rw-rw-rw-   0        0        0      740 2022-10-13 00:41:19.000000 std.algorithm-1.1.7/std/search.py
+-rw-rw-rw-   0        0        0    19454 2023-03-08 09:05:45.000000 std.algorithm-1.1.7/std/sets.py
+-rw-rw-rw-   0        0        0     1162 2022-10-13 00:41:19.000000 std.algorithm-1.1.7/std/tree.py
+-rw-rw-rw-   0        0        0      443 2023-03-16 02:15:53.000000 std.algorithm-1.1.7/std/unicode.py
+-rw-rw-rw-   0        0        0    35286 2023-02-02 07:42:54.000000 std.algorithm-1.1.7/std/xml.py
+drwxrwxrwx   0        0        0        0 2023-06-13 06:01:09.886362 std.algorithm-1.1.7/std.algorithm.egg-info/
+-rw-rw-rw-   0        0        0      324 2023-06-13 06:01:09.000000 std.algorithm-1.1.7/std.algorithm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      431 2023-06-13 06:01:09.000000 std.algorithm-1.1.7/std.algorithm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 06:01:09.000000 std.algorithm-1.1.7/std.algorithm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-13 06:01:09.000000 std.algorithm-1.1.7/std.algorithm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-06-13 06:01:09.000000 std.algorithm-1.1.7/std.algorithm.egg-info/top_level.txt
```

### Comparing `std.algorithm-1.1.6/std/MySQL.py` & `std.algorithm-1.1.7/std/MySQL.py`

 * *Files identical despite different names*

### Comparing `std.algorithm-1.1.6/std/__init__.py` & `std.algorithm-1.1.7/std/__init__.py`

 * *Files identical despite different names*

### Comparing `std.algorithm-1.1.6/std/combinatorics.py` & `std.algorithm-1.1.7/std/combinatorics.py`

 * *Files identical despite different names*

### Comparing `std.algorithm-1.1.6/std/data.py` & `std.algorithm-1.1.7/std/data.py`

 * *Files identical despite different names*

### Comparing `std.algorithm-1.1.6/std/file.py` & `std.algorithm-1.1.7/std/file.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
     def __init__(self, path, encoding="utf-8", **kwargs):
         mode = kwargs.get('mode') or "r+" if os.path.isfile(path) else "w+"
         try:
             self.file = open(path, mode=mode, encoding=encoding)
         except PermissionError as e:
             print("error message printed in std.file:", e)
-            exit(0)
+            raise e
         except FileNotFoundError:
             createNewFile(path)
             self.file = open(path, "w+", encoding=encoding)
 
         self.rewind()
         
         if kwargs.get('strip'):
```

### Comparing `std.algorithm-1.1.6/std/http.py` & `std.algorithm-1.1.7/std/http.py`

 * *Files identical despite different names*

### Comparing `std.algorithm-1.1.6/std/keras.py` & `std.algorithm-1.1.7/std/keras.py`

 * *Files identical despite different names*

### Comparing `std.algorithm-1.1.6/std/lib/eigen.dll` & `std.algorithm-1.1.7/std/lib/eigen.dll`

 * *Files identical despite different names*

### Comparing `std.algorithm-1.1.6/std/nlp.py` & `std.algorithm-1.1.7/std/nlp.py`

 * *Files identical despite different names*

### Comparing `std.algorithm-1.1.6/std/search.py` & `std.algorithm-1.1.7/std/search.py`

 * *Files identical despite different names*

### Comparing `std.algorithm-1.1.6/std/sets.py` & `std.algorithm-1.1.7/std/sets.py`

 * *Files identical despite different names*

### Comparing `std.algorithm-1.1.6/std/tree.py` & `std.algorithm-1.1.7/std/tree.py`

 * *Files identical despite different names*

### Comparing `std.algorithm-1.1.6/std/xml.py` & `std.algorithm-1.1.7/std/xml.py`

 * *Files identical despite different names*

