# Comparing `tmp/pginter-0.2.5.tar.gz` & `tmp/pginter-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pginter-0.2.5.tar", last modified: Tue Jun 13 14:29:47 2023, max compression
+gzip compressed data, was "pginter-0.2.6.tar", last modified: Tue Jun 13 15:28:01 2023, max compression
```

## Comparing `pginter-0.2.5.tar` & `pginter-0.2.6.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-13 14:29:47.682923 pginter-0.2.5/
--rwxrwxrwx   0 nilusink  (1000) nilusink  (1000)     1065 2023-02-04 21:58:18.000000 pginter-0.2.5/LICENSE
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      115 2023-05-31 20:31:36.000000 pginter-0.2.5/MANIFEST.in
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      493 2023-06-13 14:29:47.682923 pginter-0.2.5/PKG-INFO
--rwxrwxrwx   0 nilusink  (1000) nilusink  (1000)       54 2023-02-04 21:58:18.000000 pginter-0.2.5/README.md
--rwxr-xr-x   0 nilusink  (1000) nilusink  (1000)      116 2023-05-24 18:38:46.000000 pginter-0.2.5/pyproject.toml
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)       38 2023-06-13 14:29:47.682923 pginter-0.2.5/setup.cfg
--rwxr-xr-x   0 nilusink  (1000) nilusink  (1000)     1021 2023-06-01 19:06:50.000000 pginter-0.2.5/setup.py
-drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-13 14:29:47.676256 pginter-0.2.5/src/
-drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-13 14:29:47.676256 pginter-0.2.5/src/pginter/
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      124 2023-02-10 14:14:25.000000 pginter-0.2.5/src/pginter/__init__.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)     8707 2023-06-01 19:29:58.000000 pginter-0.2.5/src/pginter/_pg_root.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)    20019 2023-02-10 14:14:25.000000 pginter-0.2.5/src/pginter/icon.png
-drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-13 14:29:47.679589 pginter-0.2.5/src/pginter/theme/
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)       35 2023-02-10 14:14:25.000000 pginter-0.2.5/src/pginter/theme/__init__.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)     3997 2023-05-25 23:31:05.000000 pginter-0.2.5/src/pginter/theme/_manager.py
-drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-13 14:29:47.679589 pginter-0.2.5/src/pginter/theme/themes/
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      673 2023-06-01 19:26:32.000000 pginter-0.2.5/src/pginter/theme/themes/default.json
-drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-13 14:29:47.679589 pginter-0.2.5/src/pginter/types/
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      335 2023-05-25 22:58:36.000000 pginter-0.2.5/src/pginter/types/__init__.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      368 2023-02-10 14:14:25.000000 pginter-0.2.5/src/pginter/types/_better_dict.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      455 2023-05-25 19:05:55.000000 pginter-0.2.5/src/pginter/types/_binds.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)     4227 2023-05-25 23:31:05.000000 pginter-0.2.5/src/pginter/types/_color.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      456 2023-05-25 23:31:05.000000 pginter-0.2.5/src/pginter/types/_constants.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      273 2023-05-14 20:36:55.000000 pginter-0.2.5/src/pginter/types/_geo_types.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      161 2023-05-25 15:16:09.000000 pginter-0.2.5/src/pginter/types/_notifications.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)     5384 2023-05-30 12:53:46.000000 pginter-0.2.5/src/pginter/types/_scheme.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)     6528 2023-05-15 19:07:58.000000 pginter-0.2.5/src/pginter/types/_style.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)     4301 2023-05-25 23:22:37.000000 pginter-0.2.5/src/pginter/types/_tk_vars.py
-drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-13 14:29:47.679589 pginter-0.2.5/src/pginter/utils/
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)       49 2023-05-14 20:09:36.000000 pginter-0.2.5/src/pginter/utils/__init__.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      872 2023-05-25 23:31:06.000000 pginter-0.2.5/src/pginter/utils/_funcs.py
-drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-13 14:29:47.682923 pginter-0.2.5/src/pginter/widgets/
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      197 2023-05-25 22:58:36.000000 pginter-0.2.5/src/pginter/widgets/__init__.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)     4982 2023-05-25 10:36:44.000000 pginter-0.2.5/src/pginter/widgets/_button.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)    14178 2023-05-30 19:45:06.000000 pginter-0.2.5/src/pginter/widgets/_entry.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)    28167 2023-06-13 14:28:55.000000 pginter-0.2.5/src/pginter/widgets/_frame.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)    26315 2023-06-01 18:54:30.000000 pginter-0.2.5/src/pginter/widgets/_geo_manager.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)     5961 2023-05-30 19:49:43.000000 pginter-0.2.5/src/pginter/widgets/_label.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      412 2023-02-10 14:14:25.000000 pginter-0.2.5/src/pginter/widgets/_supports_children.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)     1022 2023-05-24 20:39:09.000000 pginter-0.2.5/src/pginter/widgets/_surface_frame.py
-drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-13 14:29:47.679589 pginter-0.2.5/src/pginter.egg-info/
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      493 2023-06-13 14:29:47.000000 pginter-0.2.5/src/pginter.egg-info/PKG-INFO
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)     1028 2023-06-13 14:29:47.000000 pginter-0.2.5/src/pginter.egg-info/SOURCES.txt
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)        1 2023-06-13 14:29:47.000000 pginter-0.2.5/src/pginter.egg-info/dependency_links.txt
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)       33 2023-06-13 14:29:47.000000 pginter-0.2.5/src/pginter.egg-info/requires.txt
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)        8 2023-06-13 14:29:47.000000 pginter-0.2.5/src/pginter.egg-info/top_level.txt
+drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-13 15:28:01.828294 pginter-0.2.6/
+-rwxrwxrwx   0 nilusink  (1000) nilusink  (1000)     1065 2023-02-04 21:58:18.000000 pginter-0.2.6/LICENSE
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      115 2023-05-31 20:31:36.000000 pginter-0.2.6/MANIFEST.in
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      493 2023-06-13 15:28:01.824960 pginter-0.2.6/PKG-INFO
+-rwxrwxrwx   0 nilusink  (1000) nilusink  (1000)       54 2023-02-04 21:58:18.000000 pginter-0.2.6/README.md
+-rwxr-xr-x   0 nilusink  (1000) nilusink  (1000)      116 2023-05-24 18:38:46.000000 pginter-0.2.6/pyproject.toml
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)       38 2023-06-13 15:28:01.828294 pginter-0.2.6/setup.cfg
+-rwxr-xr-x   0 nilusink  (1000) nilusink  (1000)     1021 2023-06-13 14:30:14.000000 pginter-0.2.6/setup.py
+drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-13 15:28:01.818293 pginter-0.2.6/src/
+drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-13 15:28:01.821627 pginter-0.2.6/src/pginter/
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      124 2023-02-10 14:14:25.000000 pginter-0.2.6/src/pginter/__init__.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)     8707 2023-06-01 19:29:58.000000 pginter-0.2.6/src/pginter/_pg_root.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)    20019 2023-02-10 14:14:25.000000 pginter-0.2.6/src/pginter/icon.png
+drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-13 15:28:01.821627 pginter-0.2.6/src/pginter/theme/
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)       35 2023-02-10 14:14:25.000000 pginter-0.2.6/src/pginter/theme/__init__.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)     3997 2023-05-25 23:31:05.000000 pginter-0.2.6/src/pginter/theme/_manager.py
+drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-13 15:28:01.821627 pginter-0.2.6/src/pginter/theme/themes/
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      673 2023-06-01 19:26:32.000000 pginter-0.2.6/src/pginter/theme/themes/default.json
+drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-13 15:28:01.824960 pginter-0.2.6/src/pginter/types/
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      335 2023-05-25 22:58:36.000000 pginter-0.2.6/src/pginter/types/__init__.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      368 2023-02-10 14:14:25.000000 pginter-0.2.6/src/pginter/types/_better_dict.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      455 2023-05-25 19:05:55.000000 pginter-0.2.6/src/pginter/types/_binds.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)     4227 2023-05-25 23:31:05.000000 pginter-0.2.6/src/pginter/types/_color.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      456 2023-05-25 23:31:05.000000 pginter-0.2.6/src/pginter/types/_constants.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      273 2023-05-14 20:36:55.000000 pginter-0.2.6/src/pginter/types/_geo_types.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      161 2023-05-25 15:16:09.000000 pginter-0.2.6/src/pginter/types/_notifications.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)     5384 2023-05-30 12:53:46.000000 pginter-0.2.6/src/pginter/types/_scheme.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)     6528 2023-05-15 19:07:58.000000 pginter-0.2.6/src/pginter/types/_style.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)     4301 2023-05-25 23:22:37.000000 pginter-0.2.6/src/pginter/types/_tk_vars.py
+drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-13 15:28:01.824960 pginter-0.2.6/src/pginter/utils/
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)       63 2023-06-13 15:26:29.000000 pginter-0.2.6/src/pginter/utils/__init__.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)     1486 2023-06-13 15:27:29.000000 pginter-0.2.6/src/pginter/utils/_funcs.py
+drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-13 15:28:01.824960 pginter-0.2.6/src/pginter/widgets/
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      197 2023-05-25 22:58:36.000000 pginter-0.2.6/src/pginter/widgets/__init__.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)     4982 2023-05-25 10:36:44.000000 pginter-0.2.6/src/pginter/widgets/_button.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)    14178 2023-05-30 19:45:06.000000 pginter-0.2.6/src/pginter/widgets/_entry.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)    28606 2023-06-13 15:27:29.000000 pginter-0.2.6/src/pginter/widgets/_frame.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)    26315 2023-06-01 18:54:30.000000 pginter-0.2.6/src/pginter/widgets/_geo_manager.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)     5961 2023-05-30 19:49:43.000000 pginter-0.2.6/src/pginter/widgets/_label.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      412 2023-02-10 14:14:25.000000 pginter-0.2.6/src/pginter/widgets/_supports_children.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)     1022 2023-05-24 20:39:09.000000 pginter-0.2.6/src/pginter/widgets/_surface_frame.py
+drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-13 15:28:01.821627 pginter-0.2.6/src/pginter.egg-info/
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      493 2023-06-13 15:28:01.000000 pginter-0.2.6/src/pginter.egg-info/PKG-INFO
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)     1028 2023-06-13 15:28:01.000000 pginter-0.2.6/src/pginter.egg-info/SOURCES.txt
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)        1 2023-06-13 15:28:01.000000 pginter-0.2.6/src/pginter.egg-info/dependency_links.txt
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)       33 2023-06-13 15:28:01.000000 pginter-0.2.6/src/pginter.egg-info/requires.txt
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)        8 2023-06-13 15:28:01.000000 pginter-0.2.6/src/pginter.egg-info/top_level.txt
```

### Comparing `pginter-0.2.5/LICENSE` & `pginter-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pginter-0.2.5/setup.py` & `pginter-0.2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pginter",
-    version="0.2.5",
+    version="0.2.6",
     author="Nilusink",
     author_email="nilusink@protonmail.com",
     description="A python GUI interface, based on pygame",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Nilusink/PgInter",
     # project_urls={
```

### Comparing `pginter-0.2.5/src/pginter/_pg_root.py` & `pginter-0.2.6/src/pginter/_pg_root.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.5/src/pginter/icon.png` & `pginter-0.2.6/src/pginter/icon.png`

 * *Files identical despite different names*

### Comparing `pginter-0.2.5/src/pginter/theme/_manager.py` & `pginter-0.2.6/src/pginter/theme/_manager.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.5/src/pginter/theme/themes/default.json` & `pginter-0.2.6/src/pginter/theme/themes/default.json`

 * *Files identical despite different names*

### Comparing `pginter-0.2.5/src/pginter/types/_color.py` & `pginter-0.2.6/src/pginter/types/_color.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.5/src/pginter/types/_scheme.py` & `pginter-0.2.6/src/pginter/types/_scheme.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.5/src/pginter/types/_style.py` & `pginter-0.2.6/src/pginter/types/_style.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.5/src/pginter/types/_tk_vars.py` & `pginter-0.2.6/src/pginter/types/_tk_vars.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.5/src/pginter/widgets/_button.py` & `pginter-0.2.6/src/pginter/widgets/_button.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.5/src/pginter/widgets/_entry.py` & `pginter-0.2.6/src/pginter/widgets/_entry.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.5/src/pginter/widgets/_frame.py` & `pginter-0.2.6/src/pginter/widgets/_frame.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 Author:
 Nilusink
 """
 from ._geo_manager import GeometryManager
 from concurrent.futures import Future
 from ..theme import ThemeManager
+from ..utils import merge_alphas
 from ..types import *
 import typing as tp
 import pygame as pg
 
 # try importing pil. The user shouldn't be forced to install pil, but
 # will get an error if they try to use the image widget without having it
 # installed
@@ -37,14 +38,24 @@
 def add_corners(
         im: Image,
         ulr: int,
         urr: int,
         llr: int,
         lrr: int
 ) -> Image:
+    """
+    adds corners to an image
+
+    :param im: input image
+    :param ulr: upper left radius
+    :param urr: upper right radius
+    :param llr: lower left radius
+    :param lrr: lower right radius
+    :returns: the converted image
+    """
     alpha = Image.new('L', im.size, 255)
     w, h = im.size
 
     # upper left corner
     ulc = Image.new("L", (ulr * 2, ulr * 2), 0)
     draw = ImageDraw.Draw(ulc)
     draw.ellipse((0, 0, ulr * 2 - 1, ulr * 2 - 1), fill=255)
@@ -68,15 +79,17 @@
     # lower right radius
     lrc = Image.new("L", (lrr * 2, lrr * 2), 0)
     draw = ImageDraw.Draw(lrc)
     draw.ellipse((0, 0, lrr * 2 - 1, lrr * 2 - 1), fill=255)
     lrc = lrc.crop((lrr, lrr, lrr * 2, lrr * 2))
     alpha.paste(lrc, (w - lrr, h - lrr))
 
-    im.putalpha(alpha)
+    # apply the corner radius, keeping the image's alpha (if already present)
+    *_, ia = im.split()  # extract alpha channel from image
+    im.putalpha(merge_alphas(alpha, ia, min))
     return im
 
 
 def display_configurify(key: str) -> str:
     """
     convert a Frame init key to it's corresponding DisplayConfig key
     """
```

### Comparing `pginter-0.2.5/src/pginter/widgets/_geo_manager.py` & `pginter-0.2.6/src/pginter/widgets/_geo_manager.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.5/src/pginter/widgets/_label.py` & `pginter-0.2.6/src/pginter/widgets/_label.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.5/src/pginter/widgets/_surface_frame.py` & `pginter-0.2.6/src/pginter/widgets/_surface_frame.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.5/src/pginter.egg-info/SOURCES.txt` & `pginter-0.2.6/src/pginter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

