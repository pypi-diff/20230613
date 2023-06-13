# Comparing `tmp/nure-2023.5.8.tar.gz` & `tmp/nure-2023.6.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nure-2023.5.8.tar", last modified: Mon May  8 06:17:02 2023, max compression
+gzip compressed data, was "nure-2023.6.13.tar", last modified: Tue Jun 13 10:23:30 2023, max compression
```

## Comparing `nure-2023.5.8.tar` & `nure-2023.6.13.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        0 2023-05-08 06:17:02.550119 nure-2023.5.8/
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)    35149 2021-05-21 04:50:18.000000 nure-2023.5.8/LICENSE
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      611 2023-05-08 06:17:02.551459 nure-2023.5.8/PKG-INFO
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)       30 2021-05-21 04:25:06.000000 nure-2023.5.8/README.md
-drwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        0 2023-05-08 06:16:06.754092 nure-2023.5.8/nure/
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        0 2021-05-21 05:41:00.000000 nure-2023.5.8/nure/__init__.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     2523 2021-11-20 09:30:50.000000 nure-2023.5.8/nure/archive.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     2379 2023-05-08 05:52:06.000000 nure-2023.5.8/nure/array.py
-drwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        0 2023-05-08 06:16:06.792652 nure-2023.5.8/nure/code/
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)       62 2021-07-13 10:11:18.000000 nure-2023.5.8/nure/code/__init__.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     1353 2021-07-13 16:16:01.000000 nure-2023.5.8/nure/code/label_coder.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     4912 2022-07-29 07:41:08.000000 nure-2023.5.8/nure/dataframe.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     1263 2021-07-21 05:24:39.000000 nure-2023.5.8/nure/datetime.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      106 2021-05-21 06:28:06.000000 nure-2023.5.8/nure/debug.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     1416 2023-05-08 06:16:05.000000 nure-2023.5.8/nure/dict.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      487 2021-11-30 04:03:48.000000 nure-2023.5.8/nure/func.py
-drwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        0 2023-05-08 06:16:06.891279 nure-2023.5.8/nure/image/
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        0 2022-04-14 09:32:11.000000 nure-2023.5.8/nure/image/__init__.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)    10331 2022-04-14 09:44:09.000000 nure-2023.5.8/nure/image/annotate.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     6438 2022-04-14 09:32:48.000000 nure-2023.5.8/nure/image/func.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     6060 2023-04-29 16:36:51.000000 nure-2023.5.8/nure/image/pil.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     1457 2022-03-22 08:57:21.000000 nure-2023.5.8/nure/meta.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      445 2021-05-21 04:25:40.000000 nure-2023.5.8/nure/path.py
-drwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        0 2023-05-08 06:16:07.041371 nure-2023.5.8/nure/sync/
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        0 2021-05-21 05:53:57.000000 nure-2023.5.8/nure/sync/__init__.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      457 2021-05-21 09:16:57.000000 nure-2023.5.8/nure/sync/bigquery.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     1628 2021-11-30 04:09:01.000000 nure-2023.5.8/nure/sync/cache.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     3249 2021-07-23 06:18:01.000000 nure-2023.5.8/nure/sync/googlesheet.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      706 2021-05-21 09:17:03.000000 nure-2023.5.8/nure/sync/postgre.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     3481 2023-04-29 16:38:30.000000 nure-2023.5.8/nure/sync/s3.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     1806 2022-09-18 04:11:30.000000 nure-2023.5.8/nure/sync/sql.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     1450 2021-09-17 11:26:33.000000 nure-2023.5.8/nure/sync/suffix.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     2872 2021-11-05 14:16:28.000000 nure-2023.5.8/nure/volatitle.py
-drwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        0 2023-05-08 06:16:07.111087 nure-2023.5.8/nure.egg-info/
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      611 2023-05-08 06:16:06.000000 nure-2023.5.8/nure.egg-info/PKG-INFO
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      842 2023-05-08 06:16:06.000000 nure-2023.5.8/nure.egg-info/SOURCES.txt
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        1 2023-05-08 06:16:06.000000 nure-2023.5.8/nure.egg-info/dependency_links.txt
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      145 2023-05-08 06:16:06.000000 nure-2023.5.8/nure.egg-info/requires.txt
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        5 2023-05-08 06:16:06.000000 nure-2023.5.8/nure.egg-info/top_level.txt
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      103 2021-05-21 04:28:28.000000 nure-2023.5.8/pyproject.toml
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      849 2023-05-08 06:17:02.556865 nure-2023.5.8/setup.cfg
-drwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        0 2023-05-08 06:17:02.532619 nure-2023.5.8/tests/
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     1011 2021-11-20 09:51:16.000000 nure-2023.5.8/tests/test_archive.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     1225 2021-09-17 11:28:32.000000 nure-2023.5.8/tests/test_bigquery.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     2890 2021-07-13 16:25:33.000000 nure-2023.5.8/tests/test_coder.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      792 2021-07-23 06:18:01.000000 nure-2023.5.8/tests/test_googlesheet.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     3698 2021-11-30 04:05:08.000000 nure-2023.5.8/tests/test_parallel.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      708 2021-09-17 11:49:25.000000 nure-2023.5.8/tests/test_postgre.py
--rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      655 2021-10-08 07:11:48.000000 nure-2023.5.8/tests/test_s3.py
+drwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        0 2023-06-13 10:23:30.533268 nure-2023.6.13/
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)    35149 2021-05-21 04:50:18.000000 nure-2023.6.13/LICENSE
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      612 2023-06-13 10:23:30.533268 nure-2023.6.13/PKG-INFO
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)       30 2021-05-21 04:25:06.000000 nure-2023.6.13/README.md
+drwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        0 2023-06-13 10:23:29.995476 nure-2023.6.13/nure/
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        0 2021-05-21 05:41:00.000000 nure-2023.6.13/nure/__init__.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     2523 2021-11-20 09:30:50.000000 nure-2023.6.13/nure/archive.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     2379 2023-05-08 05:52:06.000000 nure-2023.6.13/nure/array.py
+drwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        0 2023-06-13 10:23:30.046029 nure-2023.6.13/nure/code/
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)       62 2021-07-13 10:11:18.000000 nure-2023.6.13/nure/code/__init__.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     1353 2021-07-13 16:16:01.000000 nure-2023.6.13/nure/code/label_coder.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     4912 2022-07-29 07:41:08.000000 nure-2023.6.13/nure/dataframe.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     1263 2021-07-21 05:24:39.000000 nure-2023.6.13/nure/datetime.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      106 2021-05-21 06:28:06.000000 nure-2023.6.13/nure/debug.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     1416 2023-05-08 06:16:05.000000 nure-2023.6.13/nure/dict.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      487 2021-11-30 04:03:48.000000 nure-2023.6.13/nure/func.py
+drwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        0 2023-06-13 10:23:30.140486 nure-2023.6.13/nure/image/
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        0 2022-04-14 09:32:11.000000 nure-2023.6.13/nure/image/__init__.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)    10331 2022-04-14 09:44:09.000000 nure-2023.6.13/nure/image/annotate.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     6438 2022-04-14 09:32:48.000000 nure-2023.6.13/nure/image/func.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     6667 2023-06-13 09:52:59.000000 nure-2023.6.13/nure/image/pil.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     1457 2022-03-22 08:57:21.000000 nure-2023.6.13/nure/meta.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      445 2021-05-21 04:25:40.000000 nure-2023.6.13/nure/path.py
+drwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        0 2023-06-13 10:23:30.322217 nure-2023.6.13/nure/sync/
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        0 2021-05-21 05:53:57.000000 nure-2023.6.13/nure/sync/__init__.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      457 2021-05-21 09:16:57.000000 nure-2023.6.13/nure/sync/bigquery.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     1628 2021-11-30 04:09:01.000000 nure-2023.6.13/nure/sync/cache.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     3249 2021-07-23 06:18:01.000000 nure-2023.6.13/nure/sync/googlesheet.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      706 2021-05-21 09:17:03.000000 nure-2023.6.13/nure/sync/postgre.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     3481 2023-04-29 16:38:30.000000 nure-2023.6.13/nure/sync/s3.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     1806 2022-09-18 04:11:30.000000 nure-2023.6.13/nure/sync/sql.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     1450 2021-09-17 11:26:33.000000 nure-2023.6.13/nure/sync/suffix.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     2872 2021-11-05 14:16:28.000000 nure-2023.6.13/nure/volatitle.py
+drwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        0 2023-06-13 10:23:30.400192 nure-2023.6.13/nure.egg-info/
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      612 2023-06-13 10:23:29.000000 nure-2023.6.13/nure.egg-info/PKG-INFO
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      842 2023-06-13 10:23:29.000000 nure-2023.6.13/nure.egg-info/SOURCES.txt
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        1 2023-06-13 10:23:29.000000 nure-2023.6.13/nure.egg-info/dependency_links.txt
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      154 2023-06-13 10:23:29.000000 nure-2023.6.13/nure.egg-info/requires.txt
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        5 2023-06-13 10:23:29.000000 nure-2023.6.13/nure.egg-info/top_level.txt
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      103 2021-05-21 04:28:28.000000 nure-2023.6.13/pyproject.toml
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      858 2023-06-13 10:23:30.539520 nure-2023.6.13/setup.cfg
+drwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)        0 2023-06-13 10:23:30.516484 nure-2023.6.13/tests/
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     1011 2021-11-20 09:51:16.000000 nure-2023.6.13/tests/test_archive.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     1225 2021-09-17 11:28:32.000000 nure-2023.6.13/tests/test_bigquery.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     2890 2021-07-13 16:25:33.000000 nure-2023.6.13/tests/test_coder.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      792 2021-07-23 06:18:01.000000 nure-2023.6.13/tests/test_googlesheet.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)     3698 2021-11-30 04:05:08.000000 nure-2023.6.13/tests/test_parallel.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      708 2021-09-17 11:49:25.000000 nure-2023.6.13/tests/test_postgre.py
+-rwxrwxrwx   0 tranduytrung  (1000) tranduytrung  (1000)      655 2021-10-08 07:11:48.000000 nure-2023.6.13/tests/test_s3.py
```

### Comparing `nure-2023.5.8/LICENSE` & `nure-2023.6.13/LICENSE`

 * *Files identical despite different names*

### Comparing `nure-2023.5.8/PKG-INFO` & `nure-2023.6.13/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nure
-Version: 2023.5.8
+Version: 2023.6.13
 Summary: Data Science Utilities
 Home-page: https://github.com/tranduytrung/nure
 Author: Trung Tran
 Author-email: tranduytrung@outlook.com
 Project-URL: Bug Tracker, https://github.com/tranduytrung/nure/issues
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `nure-2023.5.8/nure/archive.py` & `nure-2023.6.13/nure/archive.py`

 * *Files identical despite different names*

### Comparing `nure-2023.5.8/nure/array.py` & `nure-2023.6.13/nure/array.py`

 * *Files identical despite different names*

### Comparing `nure-2023.5.8/nure/code/label_coder.py` & `nure-2023.6.13/nure/code/label_coder.py`

 * *Files identical despite different names*

### Comparing `nure-2023.5.8/nure/dataframe.py` & `nure-2023.6.13/nure/dataframe.py`

 * *Files identical despite different names*

### Comparing `nure-2023.5.8/nure/datetime.py` & `nure-2023.6.13/nure/datetime.py`

 * *Files identical despite different names*

### Comparing `nure-2023.5.8/nure/dict.py` & `nure-2023.6.13/nure/dict.py`

 * *Files identical despite different names*

### Comparing `nure-2023.5.8/nure/image/annotate.py` & `nure-2023.6.13/nure/image/annotate.py`

 * *Files identical despite different names*

### Comparing `nure-2023.5.8/nure/image/func.py` & `nure-2023.6.13/nure/image/func.py`

 * *Files identical despite different names*

### Comparing `nure-2023.5.8/nure/image/pil.py` & `nure-2023.6.13/nure/image/pil.py`

 * *Files 3% similar despite different names*

```diff
@@ -196,7 +196,30 @@
     new_image = PIL.Image.new(image.mode, (image_width, image_height), color=background_color)
     new_image.paste(image, (image_x, image_y))
     # draw text
     draw = PIL.ImageDraw.Draw(new_image)
     draw.text((text_x, text_y), wrapped_text, fill=text_color, font=font)
 
     return new_image
+
+
+def concat_images(l_pImage: List[Image], axis=0):
+    l_width = [pImage.size[0] for pImage in l_pImage]
+    l_height = [pImage.size[1] for pImage in l_pImage]
+    if axis == 0:
+        width = max(l_width)
+        height = sum(l_height)
+    else:
+        width = sum(l_width)
+        height = max(l_height)
+
+    concated_pImage = PIL.Image.new('RGB', (width, height), color='white')
+    x = 0
+    y = 0
+    for pImage in l_pImage:
+        concated_pImage.paste(pImage, (x, y))
+        if axis == 0:
+            y += pImage.size[1]
+        else:
+            x += pImage.size[0]
+
+    return concated_pImage
```

### Comparing `nure-2023.5.8/nure/meta.py` & `nure-2023.6.13/nure/meta.py`

 * *Files identical despite different names*

### Comparing `nure-2023.5.8/nure/sync/cache.py` & `nure-2023.6.13/nure/sync/cache.py`

 * *Files identical despite different names*

### Comparing `nure-2023.5.8/nure/sync/googlesheet.py` & `nure-2023.6.13/nure/sync/googlesheet.py`

 * *Files identical despite different names*

### Comparing `nure-2023.5.8/nure/sync/postgre.py` & `nure-2023.6.13/nure/sync/postgre.py`

 * *Files identical despite different names*

### Comparing `nure-2023.5.8/nure/sync/s3.py` & `nure-2023.6.13/nure/sync/s3.py`

 * *Files identical despite different names*

### Comparing `nure-2023.5.8/nure/sync/sql.py` & `nure-2023.6.13/nure/sync/sql.py`

 * *Files identical despite different names*

### Comparing `nure-2023.5.8/nure/sync/suffix.py` & `nure-2023.6.13/nure/sync/suffix.py`

 * *Files identical despite different names*

### Comparing `nure-2023.5.8/nure/volatitle.py` & `nure-2023.6.13/nure/volatitle.py`

 * *Files identical despite different names*

### Comparing `nure-2023.5.8/nure.egg-info/PKG-INFO` & `nure-2023.6.13/nure.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nure
-Version: 2023.5.8
+Version: 2023.6.13
 Summary: Data Science Utilities
 Home-page: https://github.com/tranduytrung/nure
 Author: Trung Tran
 Author-email: tranduytrung@outlook.com
 Project-URL: Bug Tracker, https://github.com/tranduytrung/nure/issues
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `nure-2023.5.8/nure.egg-info/SOURCES.txt` & `nure-2023.6.13/nure.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nure-2023.5.8/setup.cfg` & `nure-2023.6.13/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nure
-version = 2023.05.08
+version = 2023.06.13
 author = Trung Tran
 author_email = tranduytrung@outlook.com
 description = Data Science Utilities
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/tranduytrung/nure
 project_urls = 
@@ -24,15 +24,15 @@
 	numpy
 	pandas
 	pyarrow
 
 [options.extras_require]
 image = 
 	pillow
-	opencv-python
+	opencv-python-headless
 sql = 
 	mysql-connector-python
 	sqlalchemy-bigquery
 	psycopg2-binary
 aws = 
 	boto3
```

### Comparing `nure-2023.5.8/tests/test_archive.py` & `nure-2023.6.13/tests/test_archive.py`

 * *Files identical despite different names*

### Comparing `nure-2023.5.8/tests/test_bigquery.py` & `nure-2023.6.13/tests/test_bigquery.py`

 * *Files identical despite different names*

### Comparing `nure-2023.5.8/tests/test_coder.py` & `nure-2023.6.13/tests/test_coder.py`

 * *Files identical despite different names*

### Comparing `nure-2023.5.8/tests/test_googlesheet.py` & `nure-2023.6.13/tests/test_googlesheet.py`

 * *Files identical despite different names*

### Comparing `nure-2023.5.8/tests/test_parallel.py` & `nure-2023.6.13/tests/test_parallel.py`

 * *Files identical despite different names*

### Comparing `nure-2023.5.8/tests/test_postgre.py` & `nure-2023.6.13/tests/test_postgre.py`

 * *Files identical despite different names*

### Comparing `nure-2023.5.8/tests/test_s3.py` & `nure-2023.6.13/tests/test_s3.py`

 * *Files identical despite different names*

