# Comparing `tmp/pywellcad-0.2.1.tar.gz` & `tmp/pywellcad-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywellcad-0.2.1.tar", last modified: Thu Jun  8 12:31:41 2023, max compression
+gzip compressed data, was "pywellcad-0.2.2.tar", last modified: Tue Jun 13 09:46:14 2023, max compression
```

## Comparing `pywellcad-0.2.1.tar` & `pywellcad-0.2.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 12:31:41.009512 pywellcad-0.2.1/
--rw-rw-rw-   0        0        0      229 2023-06-07 06:40:01.000000 pywellcad-0.2.1/.gitignore
--rw-rw-rw-   0        0        0     1565 2022-10-11 07:39:08.000000 pywellcad-0.2.1/LICENSE.txt
--rw-rw-rw-   0        0        0       49 2022-10-11 07:39:08.000000 pywellcad-0.2.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2751 2023-06-08 12:31:41.010492 pywellcad-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     2313 2023-04-28 08:03:58.000000 pywellcad-0.2.1/README.md
--rw-rw-rw-   0        0        0      149 2022-10-11 07:39:08.000000 pywellcad-0.2.1/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-06-08 12:31:40.809337 pywellcad-0.2.1/pywellcad.egg-info/
--rw-rw-rw-   0        0        0     2751 2023-06-08 12:31:38.000000 pywellcad-0.2.1/pywellcad.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      974 2023-06-08 12:31:40.000000 pywellcad-0.2.1/pywellcad.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 12:31:38.000000 pywellcad-0.2.1/pywellcad.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-10-11 07:43:31.000000 pywellcad-0.2.1/pywellcad.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       46 2023-06-08 12:31:38.000000 pywellcad-0.2.1/pywellcad.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-08 12:31:38.000000 pywellcad-0.2.1/pywellcad.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      579 2023-06-08 12:31:41.016348 pywellcad-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0       39 2022-10-11 07:39:08.000000 pywellcad-0.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-08 12:31:40.815196 pywellcad-0.2.1/wellcad/
--rw-rw-rw-   0        0        0       17 2022-10-11 07:39:09.000000 pywellcad-0.2.1/wellcad/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-08 12:31:41.005605 pywellcad-0.2.1/wellcad/com/
--rw-rw-rw-   0        0        0      839 2022-10-11 07:39:09.000000 pywellcad-0.2.1/wellcad/com/__init__.py
--rw-rw-rw-   0        0        0     9137 2022-10-11 07:39:09.000000 pywellcad-0.2.1/wellcad/com/_application.py
--rw-rw-rw-   0        0        0   174458 2023-06-07 06:40:01.000000 pywellcad-0.2.1/wellcad/com/_borehole.py
--rw-rw-rw-   0        0        0      647 2022-10-11 07:39:09.000000 pywellcad-0.2.1/wellcad/com/_comment_box.py
--rw-rw-rw-   0        0        0      902 2022-10-11 07:39:09.000000 pywellcad-0.2.1/wellcad/com/_cross_section_box.py
--rw-rw-rw-   0        0        0     4534 2022-10-11 07:39:09.000000 pywellcad-0.2.1/wellcad/com/_depth.py
--rw-rw-rw-   0        0        0     3086 2023-06-07 09:03:05.000000 pywellcad-0.2.1/wellcad/com/_dispatch_wrapper.py
--rw-rw-rw-   0        0        0     1740 2022-10-11 07:39:09.000000 pywellcad-0.2.1/wellcad/com/_drill_item.py
--rw-rw-rw-   0        0        0     5267 2022-10-11 07:39:09.000000 pywellcad-0.2.1/wellcad/com/_equipment_item.py
--rw-rw-rw-   0        0        0     2935 2022-10-11 07:39:09.000000 pywellcad-0.2.1/wellcad/com/_font.py
--rw-rw-rw-   0        0        0     1765 2022-10-11 07:39:09.000000 pywellcad-0.2.1/wellcad/com/_fossil_item.py
--rw-rw-rw-   0        0        0     3799 2022-10-11 07:39:09.000000 pywellcad-0.2.1/wellcad/com/_header.py
--rw-rw-rw-   0        0        0     1097 2022-10-11 07:39:09.000000 pywellcad-0.2.1/wellcad/com/_interval_item.py
--rw-rw-rw-   0        0        0     1972 2022-10-11 07:39:09.000000 pywellcad-0.2.1/wellcad/com/_litho_bed.py
--rw-rw-rw-   0        0        0     1672 2022-10-11 07:39:09.000000 pywellcad-0.2.1/wellcad/com/_litho_dictionary.py
--rw-rw-rw-   0        0        0     1344 2022-10-11 07:39:09.000000 pywellcad-0.2.1/wellcad/com/_litho_pattern.py
--rw-rw-rw-   0        0        0    79368 2023-04-25 10:02:45.000000 pywellcad-0.2.1/wellcad/com/_log.py
--rw-rw-rw-   0        0        0     1282 2022-10-11 07:39:09.000000 pywellcad-0.2.1/wellcad/com/_marker_item.py
--rw-rw-rw-   0        0        0      920 2022-10-11 07:39:09.000000 pywellcad-0.2.1/wellcad/com/_odbc.py
--rw-rw-rw-   0        0        0     5459 2022-10-11 07:39:09.000000 pywellcad-0.2.1/wellcad/com/_page.py
--rw-rw-rw-   0        0        0     1273 2022-10-11 07:39:09.000000 pywellcad-0.2.1/wellcad/com/_polar_and_rose_box.py
--rw-rw-rw-   0        0        0     1675 2022-10-11 07:39:09.000000 pywellcad-0.2.1/wellcad/com/_stacking_pattern_item.py
--rw-rw-rw-   0        0        0    11879 2022-10-11 07:39:09.000000 pywellcad-0.2.1/wellcad/com/_structure.py
--rw-rw-rw-   0        0        0    13812 2022-10-11 07:39:09.000000 pywellcad-0.2.1/wellcad/com/_title.py
--rw-rw-rw-   0        0        0    12737 2023-06-07 06:40:01.000000 pywellcad-0.2.1/wellcad/com/_workspace.py
+drwxrwxrwx   0        0        0        0 2023-06-13 09:46:14.590878 pywellcad-0.2.2/
+-rw-rw-rw-   0        0        0      229 2023-06-07 06:40:01.000000 pywellcad-0.2.2/.gitignore
+-rw-rw-rw-   0        0        0     1565 2022-10-11 07:39:08.000000 pywellcad-0.2.2/LICENSE.txt
+-rw-rw-rw-   0        0        0       49 2022-10-11 07:39:08.000000 pywellcad-0.2.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2751 2023-06-13 09:46:14.591854 pywellcad-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2313 2023-04-28 08:03:58.000000 pywellcad-0.2.2/README.md
+-rw-rw-rw-   0        0        0      149 2022-10-11 07:39:08.000000 pywellcad-0.2.2/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-06-13 09:46:14.397531 pywellcad-0.2.2/pywellcad.egg-info/
+-rw-rw-rw-   0        0        0     2751 2023-06-13 09:46:12.000000 pywellcad-0.2.2/pywellcad.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      974 2023-06-13 09:46:14.000000 pywellcad-0.2.2/pywellcad.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 09:46:12.000000 pywellcad-0.2.2/pywellcad.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-10-11 07:43:31.000000 pywellcad-0.2.2/pywellcad.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       46 2023-06-13 09:46:12.000000 pywellcad-0.2.2/pywellcad.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-13 09:46:12.000000 pywellcad-0.2.2/pywellcad.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      579 2023-06-13 09:46:14.598689 pywellcad-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0       39 2022-10-11 07:39:08.000000 pywellcad-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 09:46:14.402412 pywellcad-0.2.2/wellcad/
+-rw-rw-rw-   0        0        0       17 2022-10-11 07:39:09.000000 pywellcad-0.2.2/wellcad/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 09:46:14.588926 pywellcad-0.2.2/wellcad/com/
+-rw-rw-rw-   0        0        0      839 2022-10-11 07:39:09.000000 pywellcad-0.2.2/wellcad/com/__init__.py
+-rw-rw-rw-   0        0        0     9137 2022-10-11 07:39:09.000000 pywellcad-0.2.2/wellcad/com/_application.py
+-rw-rw-rw-   0        0        0   174458 2023-06-07 06:40:01.000000 pywellcad-0.2.2/wellcad/com/_borehole.py
+-rw-rw-rw-   0        0        0      647 2022-10-11 07:39:09.000000 pywellcad-0.2.2/wellcad/com/_comment_box.py
+-rw-rw-rw-   0        0        0      902 2022-10-11 07:39:09.000000 pywellcad-0.2.2/wellcad/com/_cross_section_box.py
+-rw-rw-rw-   0        0        0     4534 2022-10-11 07:39:09.000000 pywellcad-0.2.2/wellcad/com/_depth.py
+-rw-rw-rw-   0        0        0     3086 2023-06-07 09:03:05.000000 pywellcad-0.2.2/wellcad/com/_dispatch_wrapper.py
+-rw-rw-rw-   0        0        0     1740 2022-10-11 07:39:09.000000 pywellcad-0.2.2/wellcad/com/_drill_item.py
+-rw-rw-rw-   0        0        0     5267 2022-10-11 07:39:09.000000 pywellcad-0.2.2/wellcad/com/_equipment_item.py
+-rw-rw-rw-   0        0        0     2935 2022-10-11 07:39:09.000000 pywellcad-0.2.2/wellcad/com/_font.py
+-rw-rw-rw-   0        0        0     1765 2022-10-11 07:39:09.000000 pywellcad-0.2.2/wellcad/com/_fossil_item.py
+-rw-rw-rw-   0        0        0     3799 2022-10-11 07:39:09.000000 pywellcad-0.2.2/wellcad/com/_header.py
+-rw-rw-rw-   0        0        0     1097 2022-10-11 07:39:09.000000 pywellcad-0.2.2/wellcad/com/_interval_item.py
+-rw-rw-rw-   0        0        0     1972 2022-10-11 07:39:09.000000 pywellcad-0.2.2/wellcad/com/_litho_bed.py
+-rw-rw-rw-   0        0        0     1672 2022-10-11 07:39:09.000000 pywellcad-0.2.2/wellcad/com/_litho_dictionary.py
+-rw-rw-rw-   0        0        0     1344 2022-10-11 07:39:09.000000 pywellcad-0.2.2/wellcad/com/_litho_pattern.py
+-rw-rw-rw-   0        0        0    79368 2023-04-25 10:02:45.000000 pywellcad-0.2.2/wellcad/com/_log.py
+-rw-rw-rw-   0        0        0     1282 2022-10-11 07:39:09.000000 pywellcad-0.2.2/wellcad/com/_marker_item.py
+-rw-rw-rw-   0        0        0      920 2022-10-11 07:39:09.000000 pywellcad-0.2.2/wellcad/com/_odbc.py
+-rw-rw-rw-   0        0        0     5459 2022-10-11 07:39:09.000000 pywellcad-0.2.2/wellcad/com/_page.py
+-rw-rw-rw-   0        0        0     1273 2022-10-11 07:39:09.000000 pywellcad-0.2.2/wellcad/com/_polar_and_rose_box.py
+-rw-rw-rw-   0        0        0     1675 2022-10-11 07:39:09.000000 pywellcad-0.2.2/wellcad/com/_stacking_pattern_item.py
+-rw-rw-rw-   0        0        0    11879 2022-10-11 07:39:09.000000 pywellcad-0.2.2/wellcad/com/_structure.py
+-rw-rw-rw-   0        0        0    13812 2022-10-11 07:39:09.000000 pywellcad-0.2.2/wellcad/com/_title.py
+-rw-rw-rw-   0        0        0    12737 2023-06-07 06:40:01.000000 pywellcad-0.2.2/wellcad/com/_workspace.py
```

### Comparing `pywellcad-0.2.1/LICENSE.txt` & `pywellcad-0.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pywellcad-0.2.1/PKG-INFO` & `pywellcad-0.2.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywellcad
-Version: 0.2.1
+Version: 0.2.2
 Summary: a Python client for the WellCAD Automation API
 Home-page: https://www.alt.lu/
 Author: Advanced Logic Technology
 Author-email: support@alt.lu
 License: BSD 3-Clause License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `pywellcad-0.2.1/README.md` & `pywellcad-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `pywellcad-0.2.1/pywellcad.egg-info/PKG-INFO` & `pywellcad-0.2.2/pywellcad.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywellcad
-Version: 0.2.1
+Version: 0.2.2
 Summary: a Python client for the WellCAD Automation API
 Home-page: https://www.alt.lu/
 Author: Advanced Logic Technology
 Author-email: support@alt.lu
 License: BSD 3-Clause License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `pywellcad-0.2.1/pywellcad.egg-info/SOURCES.txt` & `pywellcad-0.2.2/pywellcad.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pywellcad-0.2.1/setup.cfg` & `pywellcad-0.2.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `pywellcad-0.2.1/wellcad/com/__init__.py` & `pywellcad-0.2.2/wellcad/com/__init__.py`

 * *Files identical despite different names*

### Comparing `pywellcad-0.2.1/wellcad/com/_application.py` & `pywellcad-0.2.2/wellcad/com/_application.py`

 * *Files identical despite different names*

### Comparing `pywellcad-0.2.1/wellcad/com/_borehole.py` & `pywellcad-0.2.2/wellcad/com/_borehole.py`

 * *Files identical despite different names*

### Comparing `pywellcad-0.2.1/wellcad/com/_comment_box.py` & `pywellcad-0.2.2/wellcad/com/_comment_box.py`

 * *Files identical despite different names*

### Comparing `pywellcad-0.2.1/wellcad/com/_cross_section_box.py` & `pywellcad-0.2.2/wellcad/com/_cross_section_box.py`

 * *Files identical despite different names*

### Comparing `pywellcad-0.2.1/wellcad/com/_depth.py` & `pywellcad-0.2.2/wellcad/com/_depth.py`

 * *Files identical despite different names*

### Comparing `pywellcad-0.2.1/wellcad/com/_dispatch_wrapper.py` & `pywellcad-0.2.2/wellcad/com/_dispatch_wrapper.py`

 * *Files identical despite different names*

### Comparing `pywellcad-0.2.1/wellcad/com/_drill_item.py` & `pywellcad-0.2.2/wellcad/com/_drill_item.py`

 * *Files identical despite different names*

### Comparing `pywellcad-0.2.1/wellcad/com/_equipment_item.py` & `pywellcad-0.2.2/wellcad/com/_equipment_item.py`

 * *Files identical despite different names*

### Comparing `pywellcad-0.2.1/wellcad/com/_font.py` & `pywellcad-0.2.2/wellcad/com/_font.py`

 * *Files identical despite different names*

### Comparing `pywellcad-0.2.1/wellcad/com/_fossil_item.py` & `pywellcad-0.2.2/wellcad/com/_fossil_item.py`

 * *Files identical despite different names*

### Comparing `pywellcad-0.2.1/wellcad/com/_header.py` & `pywellcad-0.2.2/wellcad/com/_header.py`

 * *Files identical despite different names*

### Comparing `pywellcad-0.2.1/wellcad/com/_interval_item.py` & `pywellcad-0.2.2/wellcad/com/_interval_item.py`

 * *Files identical despite different names*

### Comparing `pywellcad-0.2.1/wellcad/com/_litho_bed.py` & `pywellcad-0.2.2/wellcad/com/_litho_bed.py`

 * *Files identical despite different names*

### Comparing `pywellcad-0.2.1/wellcad/com/_litho_dictionary.py` & `pywellcad-0.2.2/wellcad/com/_litho_dictionary.py`

 * *Files identical despite different names*

### Comparing `pywellcad-0.2.1/wellcad/com/_litho_pattern.py` & `pywellcad-0.2.2/wellcad/com/_litho_pattern.py`

 * *Files identical despite different names*

### Comparing `pywellcad-0.2.1/wellcad/com/_log.py` & `pywellcad-0.2.2/wellcad/com/_log.py`

 * *Files identical despite different names*

### Comparing `pywellcad-0.2.1/wellcad/com/_marker_item.py` & `pywellcad-0.2.2/wellcad/com/_marker_item.py`

 * *Files identical despite different names*

### Comparing `pywellcad-0.2.1/wellcad/com/_odbc.py` & `pywellcad-0.2.2/wellcad/com/_odbc.py`

 * *Files identical despite different names*

### Comparing `pywellcad-0.2.1/wellcad/com/_page.py` & `pywellcad-0.2.2/wellcad/com/_page.py`

 * *Files identical despite different names*

### Comparing `pywellcad-0.2.1/wellcad/com/_polar_and_rose_box.py` & `pywellcad-0.2.2/wellcad/com/_polar_and_rose_box.py`

 * *Files identical despite different names*

### Comparing `pywellcad-0.2.1/wellcad/com/_stacking_pattern_item.py` & `pywellcad-0.2.2/wellcad/com/_stacking_pattern_item.py`

 * *Files identical despite different names*

### Comparing `pywellcad-0.2.1/wellcad/com/_structure.py` & `pywellcad-0.2.2/wellcad/com/_structure.py`

 * *Files identical despite different names*

### Comparing `pywellcad-0.2.1/wellcad/com/_title.py` & `pywellcad-0.2.2/wellcad/com/_title.py`

 * *Files identical despite different names*

### Comparing `pywellcad-0.2.1/wellcad/com/_workspace.py` & `pywellcad-0.2.2/wellcad/com/_workspace.py`

 * *Files identical despite different names*

