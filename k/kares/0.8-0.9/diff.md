# Comparing `tmp/kares-0.8.tar.gz` & `tmp/kares-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kares-0.8.tar", last modified: Tue Jun 13 19:47:01 2023, max compression
+gzip compressed data, was "kares-0.9.tar", last modified: Tue Jun 13 19:56:49 2023, max compression
```

## Comparing `kares-0.8.tar` & `kares-0.9.tar`

### file list

```diff
@@ -1,22 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 19:47:01.654098 kares-0.8/
--rw-rw-rw-   0        0        0      331 2023-06-13 19:46:35.000000 kares-0.8/MANIFEST.in
--rw-rw-rw-   0        0        0      323 2023-06-13 19:47:01.652628 kares-0.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-13 19:47:01.590424 kares-0.8/kares/
--rw-rw-rw-   0        0        0     1046 2023-06-13 19:38:10.000000 kares-0.8/kares/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 19:47:01.651331 kares-0.8/kares/pracs/
--rw-rw-rw-   0        0        0     2328 2023-06-13 18:07:06.000000 kares-0.8/kares/pracs/Practical_1.txt
--rw-rw-rw-   0        0        0     2244 2023-06-13 18:08:38.000000 kares-0.8/kares/pracs/Practical_2.txt
--rw-rw-rw-   0        0        0     2051 2023-06-13 18:12:03.000000 kares-0.8/kares/pracs/Practical_3.txt
--rw-rw-rw-   0        0        0     2179 2023-06-13 18:12:15.000000 kares-0.8/kares/pracs/Practical_4.txt
--rw-rw-rw-   0        0        0     1673 2023-06-13 18:12:26.000000 kares-0.8/kares/pracs/Practical_5.txt
--rw-rw-rw-   0        0        0     2161 2023-06-13 18:12:44.000000 kares-0.8/kares/pracs/Practical_6.txt
--rw-rw-rw-   0        0        0     9929 2023-06-13 18:45:06.000000 kares-0.8/kares/pracs/Practical_7.txt
--rw-rw-rw-   0        0        0     4267 2023-06-13 18:46:08.000000 kares-0.8/kares/pracs/Practical_8.txt
--rw-rw-rw-   0        0        0     1897 2023-06-13 18:46:26.000000 kares-0.8/kares/pracs/Practical_9.txt
-drwxrwxrwx   0        0        0        0 2023-06-13 19:47:01.618334 kares-0.8/kares.egg-info/
--rw-rw-rw-   0        0        0      323 2023-06-13 19:47:01.000000 kares-0.8/kares.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      406 2023-06-13 19:47:01.000000 kares-0.8/kares.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 19:47:01.000000 kares-0.8/kares.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-13 19:47:01.000000 kares-0.8/kares.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-13 19:47:01.654849 kares-0.8/setup.cfg
--rw-rw-rw-   0        0        0      424 2023-06-13 19:46:55.000000 kares-0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 19:56:49.532279 kares-0.9/
+-rw-rw-rw-   0        0        0      323 2023-06-13 19:56:49.531011 kares-0.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-13 19:56:49.467594 kares-0.9/kares/
+-rw-rw-rw-   0        0        0     1046 2023-06-13 19:38:10.000000 kares-0.9/kares/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 19:56:49.529512 kares-0.9/kares/pracs/
+-rw-rw-rw-   0        0        0     2328 2023-06-13 18:07:06.000000 kares-0.9/kares/pracs/Practical_1.txt
+-rw-rw-rw-   0        0        0     2244 2023-06-13 18:08:38.000000 kares-0.9/kares/pracs/Practical_2.txt
+-rw-rw-rw-   0        0        0     2051 2023-06-13 18:12:03.000000 kares-0.9/kares/pracs/Practical_3.txt
+-rw-rw-rw-   0        0        0     2179 2023-06-13 18:12:15.000000 kares-0.9/kares/pracs/Practical_4.txt
+-rw-rw-rw-   0        0        0     1673 2023-06-13 18:12:26.000000 kares-0.9/kares/pracs/Practical_5.txt
+-rw-rw-rw-   0        0        0     2161 2023-06-13 18:12:44.000000 kares-0.9/kares/pracs/Practical_6.txt
+-rw-rw-rw-   0        0        0     9929 2023-06-13 18:45:06.000000 kares-0.9/kares/pracs/Practical_7.txt
+-rw-rw-rw-   0        0        0     4267 2023-06-13 18:46:08.000000 kares-0.9/kares/pracs/Practical_8.txt
+-rw-rw-rw-   0        0        0     1897 2023-06-13 18:46:26.000000 kares-0.9/kares/pracs/Practical_9.txt
+drwxrwxrwx   0        0        0        0 2023-06-13 19:56:49.495084 kares-0.9/kares.egg-info/
+-rw-rw-rw-   0        0        0      323 2023-06-13 19:56:49.000000 kares-0.9/kares.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      394 2023-06-13 19:56:49.000000 kares-0.9/kares.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 19:56:49.000000 kares-0.9/kares.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-13 19:56:49.000000 kares-0.9/kares.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-13 19:56:49.533031 kares-0.9/setup.cfg
+-rw-rw-rw-   0        0        0      471 2023-06-13 19:56:47.000000 kares-0.9/setup.py
```

### Comparing `kares-0.8/kares/__init__.py` & `kares-0.9/kares/__init__.py`

 * *Files identical despite different names*

### Comparing `kares-0.8/kares/pracs/Practical_1.txt` & `kares-0.9/kares/pracs/Practical_1.txt`

 * *Files identical despite different names*

### Comparing `kares-0.8/kares/pracs/Practical_2.txt` & `kares-0.9/kares/pracs/Practical_2.txt`

 * *Files identical despite different names*

### Comparing `kares-0.8/kares/pracs/Practical_3.txt` & `kares-0.9/kares/pracs/Practical_3.txt`

 * *Files identical despite different names*

### Comparing `kares-0.8/kares/pracs/Practical_4.txt` & `kares-0.9/kares/pracs/Practical_4.txt`

 * *Files identical despite different names*

### Comparing `kares-0.8/kares/pracs/Practical_5.txt` & `kares-0.9/kares/pracs/Practical_5.txt`

 * *Files identical despite different names*

### Comparing `kares-0.8/kares/pracs/Practical_6.txt` & `kares-0.9/kares/pracs/Practical_6.txt`

 * *Files identical despite different names*

### Comparing `kares-0.8/kares/pracs/Practical_7.txt` & `kares-0.9/kares/pracs/Practical_7.txt`

 * *Files identical despite different names*

### Comparing `kares-0.8/kares/pracs/Practical_8.txt` & `kares-0.9/kares/pracs/Practical_8.txt`

 * *Files identical despite different names*

### Comparing `kares-0.8/kares/pracs/Practical_9.txt` & `kares-0.9/kares/pracs/Practical_9.txt`

 * *Files identical despite different names*

