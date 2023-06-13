# Comparing `tmp/mykit-2.0.0rc1.tar.gz` & `tmp/mykit-2.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mykit-2.0.0rc1.tar", last modified: Tue Jun 13 15:27:17 2023, max compression
+gzip compressed data, was "mykit-2.0.0rc2.tar", last modified: Tue Jun 13 16:07:55 2023, max compression
```

## Comparing `mykit-2.0.0rc1.tar` & `mykit-2.0.0rc2.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 15:27:17.279163 mykit-2.0.0rc1/
--rw-rw-rw-   0        0        0     1097 2023-04-10 22:01:23.000000 mykit-2.0.0rc1/LICENSE
--rw-rw-rw-   0        0        0     3554 2023-06-13 15:27:17.280161 mykit-2.0.0rc1/PKG-INFO
--rw-rw-rw-   0        0        0     2440 2023-06-13 14:48:45.000000 mykit-2.0.0rc1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-13 15:27:16.670361 mykit-2.0.0rc1/mykit/
--rw-rw-rw-   0        0        0      223 2023-06-12 18:01:09.000000 mykit-2.0.0rc1/mykit/__init__.py
--rw-rw-rw-   0        0        0      346 2023-06-12 18:02:00.000000 mykit-2.0.0rc1/mykit/__main__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 15:27:16.856565 mykit-2.0.0rc1/mykit/app/
--rw-rw-rw-   0        0        0     3645 2023-06-13 13:53:56.000000 mykit-2.0.0rc1/mykit/app/__init__.py
--rw-rw-rw-   0        0        0      128 2023-06-13 12:39:40.000000 mykit-2.0.0rc1/mykit/app/_runtime.py
--rw-rw-rw-   0        0        0     4157 2023-06-13 13:01:03.000000 mykit-2.0.0rc1/mykit/app/arrow.py
--rw-rw-rw-   0        0        0    12724 2023-06-13 12:41:28.000000 mykit-2.0.0rc1/mykit/app/button.py
-drwxrwxrwx   0        0        0        0 2023-06-13 15:27:16.867557 mykit-2.0.0rc1/mykit/app/complex/
--rw-rw-rw-   0        0        0    20467 2023-06-13 14:43:30.000000 mykit-2.0.0rc1/mykit/app/complex/biplot.py
--rw-rw-rw-   0        0        0    16360 2023-06-13 13:49:53.000000 mykit-2.0.0rc1/mykit/app/complex/plot.py
--rw-rw-rw-   0        0        0     9010 2023-06-13 13:12:29.000000 mykit-2.0.0rc1/mykit/app/label.py
--rw-rw-rw-   0        0        0    27866 2023-06-13 13:13:12.000000 mykit-2.0.0rc1/mykit/app/slider.py
-drwxrwxrwx   0        0        0        0 2023-06-13 15:27:16.982837 mykit-2.0.0rc1/mykit/kit/
--rw-rw-rw-   0        0        0     2965 2023-06-12 13:39:03.000000 mykit-2.0.0rc1/mykit/kit/color.py
-drwxrwxrwx   0        0        0        0 2023-06-13 15:27:16.398362 mykit-2.0.0rc1/mykit/kit/fast_visualizations/
-drwxrwxrwx   0        0        0        0 2023-06-13 15:27:17.076595 mykit-2.0.0rc1/mykit/kit/fast_visualizations/static/
--rw-rw-rw-   0        0        0      500 2023-06-13 14:50:18.000000 mykit-2.0.0rc1/mykit/kit/fast_visualizations/static/plot.py
--rw-rw-rw-   0        0        0     5809 2023-06-12 11:57:08.000000 mykit-2.0.0rc1/mykit/kit/ffmpeg.py
-drwxrwxrwx   0        0        0        0 2023-06-13 15:27:17.076595 mykit-2.0.0rc1/mykit/kit/keycrate/
--rw-rw-rw-   0        0        0     6473 2023-06-12 14:01:25.000000 mykit-2.0.0rc1/mykit/kit/keycrate/__init__.py
--rw-rw-rw-   0        0        0     2741 2023-06-12 12:12:05.000000 mykit-2.0.0rc1/mykit/kit/math.py
-drwxrwxrwx   0        0        0        0 2023-06-13 15:27:17.155874 mykit-2.0.0rc1/mykit/kit/neuralnet/
--rw-rw-rw-   0        0        0     7320 2023-06-12 14:05:32.000000 mykit-2.0.0rc1/mykit/kit/neuralnet/dense.py
--rw-rw-rw-   0        0        0    15109 2023-06-12 14:05:43.000000 mykit-2.0.0rc1/mykit/kit/neuralnet/genetic.py
--rw-rw-rw-   0        0        0     3039 2023-05-06 18:30:49.000000 mykit-2.0.0rc1/mykit/kit/noise.py
--rw-rw-rw-   0        0        0     4253 2023-05-18 13:55:09.000000 mykit-2.0.0rc1/mykit/kit/path.py
--rw-rw-rw-   0        0        0      403 2023-06-11 18:43:02.000000 mykit-2.0.0rc1/mykit/kit/text.py
--rw-rw-rw-   0        0        0     2453 2023-06-12 11:34:47.000000 mykit-2.0.0rc1/mykit/kit/time.py
--rw-rw-rw-   0        0        0     3156 2023-05-18 13:20:09.000000 mykit-2.0.0rc1/mykit/kit/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-13 15:27:16.815898 mykit-2.0.0rc1/mykit.egg-info/
--rw-rw-rw-   0        0        0     3554 2023-06-13 15:27:16.000000 mykit-2.0.0rc1/mykit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      826 2023-06-13 15:27:16.000000 mykit-2.0.0rc1/mykit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 15:27:16.000000 mykit-2.0.0rc1/mykit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-06-13 15:27:16.000000 mykit-2.0.0rc1/mykit.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       28 2023-06-13 15:27:16.000000 mykit-2.0.0rc1/mykit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-06-13 15:27:16.000000 mykit-2.0.0rc1/mykit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1253 2023-06-13 15:26:00.000000 mykit-2.0.0rc1/pyproject.toml
--rw-rw-rw-   0        0        0      161 2023-06-13 15:27:17.285262 mykit-2.0.0rc1/setup.cfg
--rw-rw-rw-   0        0        0       37 2023-06-12 16:59:26.000000 mykit-2.0.0rc1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-13 15:27:17.224893 mykit-2.0.0rc1/tests/
--rw-rw-rw-   0        0        0        0 2023-06-12 14:37:00.000000 mykit-2.0.0rc1/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 15:27:17.277161 mykit-2.0.0rc1/tests/test_kit/
--rw-rw-rw-   0        0        0        0 2023-06-12 14:37:00.000000 mykit-2.0.0rc1/tests/test_kit/__init__.py
--rw-rw-rw-   0        0        0     4212 2023-06-12 14:37:42.000000 mykit-2.0.0rc1/tests/test_kit/test_color.py
--rw-rw-rw-   0        0        0     3546 2023-06-12 12:14:14.000000 mykit-2.0.0rc1/tests/test_kit/test_math.py
+drwxrwxrwx   0        0        0        0 2023-06-13 16:07:55.376056 mykit-2.0.0rc2/
+-rw-rw-rw-   0        0        0     1097 2023-04-10 22:01:23.000000 mykit-2.0.0rc2/LICENSE
+-rw-rw-rw-   0        0        0     3751 2023-06-13 16:07:55.391682 mykit-2.0.0rc2/PKG-INFO
+-rw-rw-rw-   0        0        0     2637 2023-06-13 16:04:50.000000 mykit-2.0.0rc2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-13 16:07:55.085529 mykit-2.0.0rc2/mykit/
+-rw-rw-rw-   0        0        0      223 2023-06-12 18:01:09.000000 mykit-2.0.0rc2/mykit/__init__.py
+-rw-rw-rw-   0        0        0      346 2023-06-12 18:02:00.000000 mykit-2.0.0rc2/mykit/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 16:07:55.282299 mykit-2.0.0rc2/mykit/app/
+-rw-rw-rw-   0        0        0     3762 2023-06-13 15:59:31.000000 mykit-2.0.0rc2/mykit/app/__init__.py
+-rw-rw-rw-   0        0        0      128 2023-06-13 12:39:40.000000 mykit-2.0.0rc2/mykit/app/_runtime.py
+-rw-rw-rw-   0        0        0     4157 2023-06-13 13:01:03.000000 mykit-2.0.0rc2/mykit/app/arrow.py
+-rw-rw-rw-   0        0        0    12724 2023-06-13 12:41:28.000000 mykit-2.0.0rc2/mykit/app/button.py
+drwxrwxrwx   0        0        0        0 2023-06-13 16:07:55.297927 mykit-2.0.0rc2/mykit/app/complex/
+-rw-rw-rw-   0        0        0    20467 2023-06-13 14:43:30.000000 mykit-2.0.0rc2/mykit/app/complex/biplot.py
+-rw-rw-rw-   0        0        0    16360 2023-06-13 13:49:53.000000 mykit-2.0.0rc2/mykit/app/complex/plot.py
+-rw-rw-rw-   0        0        0     9010 2023-06-13 13:12:29.000000 mykit-2.0.0rc2/mykit/app/label.py
+-rw-rw-rw-   0        0        0    27866 2023-06-13 13:13:12.000000 mykit-2.0.0rc2/mykit/app/slider.py
+drwxrwxrwx   0        0        0        0 2023-06-13 16:07:55.329197 mykit-2.0.0rc2/mykit/kit/
+-rw-rw-rw-   0        0        0     2965 2023-06-12 13:39:03.000000 mykit-2.0.0rc2/mykit/kit/color.py
+drwxrwxrwx   0        0        0        0 2023-06-13 16:07:54.978651 mykit-2.0.0rc2/mykit/kit/fast_visualizations/
+drwxrwxrwx   0        0        0        0 2023-06-13 16:07:55.344803 mykit-2.0.0rc2/mykit/kit/fast_visualizations/static/
+-rw-rw-rw-   0        0        0      500 2023-06-13 14:50:18.000000 mykit-2.0.0rc2/mykit/kit/fast_visualizations/static/plot.py
+-rw-rw-rw-   0        0        0     5809 2023-06-12 11:57:08.000000 mykit-2.0.0rc2/mykit/kit/ffmpeg.py
+drwxrwxrwx   0        0        0        0 2023-06-13 16:07:55.344803 mykit-2.0.0rc2/mykit/kit/keycrate/
+-rw-rw-rw-   0        0        0     6473 2023-06-12 14:01:25.000000 mykit-2.0.0rc2/mykit/kit/keycrate/__init__.py
+-rw-rw-rw-   0        0        0     2741 2023-06-12 12:12:05.000000 mykit-2.0.0rc2/mykit/kit/math.py
+drwxrwxrwx   0        0        0        0 2023-06-13 16:07:55.360434 mykit-2.0.0rc2/mykit/kit/neuralnet/
+-rw-rw-rw-   0        0        0     7320 2023-06-12 14:05:32.000000 mykit-2.0.0rc2/mykit/kit/neuralnet/dense.py
+-rw-rw-rw-   0        0        0    15109 2023-06-12 14:05:43.000000 mykit-2.0.0rc2/mykit/kit/neuralnet/genetic.py
+-rw-rw-rw-   0        0        0     3039 2023-05-06 18:30:49.000000 mykit-2.0.0rc2/mykit/kit/noise.py
+-rw-rw-rw-   0        0        0     4253 2023-05-18 13:55:09.000000 mykit-2.0.0rc2/mykit/kit/path.py
+-rw-rw-rw-   0        0        0      403 2023-06-11 18:43:02.000000 mykit-2.0.0rc2/mykit/kit/text.py
+-rw-rw-rw-   0        0        0     2453 2023-06-12 11:34:47.000000 mykit-2.0.0rc2/mykit/kit/time.py
+-rw-rw-rw-   0        0        0     3156 2023-05-18 13:20:09.000000 mykit-2.0.0rc2/mykit/kit/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-13 16:07:55.251051 mykit-2.0.0rc2/mykit.egg-info/
+-rw-rw-rw-   0        0        0     3751 2023-06-13 16:07:54.000000 mykit-2.0.0rc2/mykit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      826 2023-06-13 16:07:54.000000 mykit-2.0.0rc2/mykit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 16:07:54.000000 mykit-2.0.0rc2/mykit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-06-13 16:07:54.000000 mykit-2.0.0rc2/mykit.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       28 2023-06-13 16:07:54.000000 mykit-2.0.0rc2/mykit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-13 16:07:54.000000 mykit-2.0.0rc2/mykit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1276 2023-06-13 15:43:48.000000 mykit-2.0.0rc2/pyproject.toml
+-rw-rw-rw-   0        0        0      161 2023-06-13 16:07:55.391682 mykit-2.0.0rc2/setup.cfg
+-rw-rw-rw-   0        0        0       37 2023-06-12 16:59:26.000000 mykit-2.0.0rc2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 16:07:55.360434 mykit-2.0.0rc2/tests/
+-rw-rw-rw-   0        0        0        0 2023-06-12 14:37:00.000000 mykit-2.0.0rc2/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 16:07:55.376056 mykit-2.0.0rc2/tests/test_kit/
+-rw-rw-rw-   0        0        0        0 2023-06-12 14:37:00.000000 mykit-2.0.0rc2/tests/test_kit/__init__.py
+-rw-rw-rw-   0        0        0     4212 2023-06-12 14:37:42.000000 mykit-2.0.0rc2/tests/test_kit/test_color.py
+-rw-rw-rw-   0        0        0     3546 2023-06-12 12:14:14.000000 mykit-2.0.0rc2/tests/test_kit/test_math.py
```

### Comparing `mykit-2.0.0rc1/LICENSE` & `mykit-2.0.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `mykit-2.0.0rc1/PKG-INFO` & `mykit-2.0.0rc2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mykit
-Version: 2.0.0rc1
+Version: 2.0.0rc2
 Summary: Python utility library
 Home-page: https://nvfp.github.io/mykit
 Author: Nicholas Valentinus
 Author-email: nvfastplease@gmail.com
 License: MIT
 Project-URL: documentation, https://nvfp.github.io/mykit/docs
 Project-URL: report bugs, https://github.com/nvfp/mykit/issues
@@ -26,15 +26,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # myKit
 
 Python utility toolkit.
 
-![mykit's banner](assets/20230613-mykit-banner-fhd.png)
+![mykit's banner](https://raw.githubusercontent.com/nvfp/mykit/master/assets/20230613-mykit-banner-fhd.png)
 
 [![pypi version](https://img.shields.io/pypi/v/mykit?logo=pypi)](https://pypi.org/project/mykit/)
 [![MIT License](https://img.shields.io/badge/license-MIT-blue.svg?style=flat)](http://choosealicense.com/licenses/mit/)
 
 
 ## Installation
 
@@ -61,44 +61,46 @@
 - 
 
 
 ## Changelog
 
 - 2.0.0 (June 13, 2023):
     - Breaking changes:
-        - New mechanism for app: `app/__init__.py`
-        - Moved: `kit/graph/graph2d.py` -> `app/complex/plot.py`
-        - transform: `kit/quick_visual/plot2d.py` -> `kit/fast_visualizations/static/plot.py`
-    - New: `app/complex/biplot.py`
+        - New mechanism for app: `/app/__init__.py`
+        - Moved: `/kit/graph/graph2d.py` -> `/app/complex/plot.py`
+        - transform: `/kit/quick_visual/plot2d.py` -> `/kit/fast_visualizations/static/plot.py`
+    - Bugfixed:
+        - folder `mykit/tests/` should also be excluded during build (rc version)
+    - New: `/app/complex/biplot.py`
 - 1.0.0 (June 12, 2023):
-    - changed arg name: `kit/quick_visual/plot2d.py`: `graph2d_cfg` -> `cfg`
+    - changed arg name: `/kit/quick_visual/plot2d.py`: `graph2d_cfg` -> `cfg`
 - 0.1.3 (June 12, 2023):
-    - removed `get_gray` from `kit/color.py`
-    - transform `kit/gui/button/` -> `app/button.py`
-    - transform `kit/gui/label/` -> `app/label.py`
-    - transform `kit/gui/slider/` -> `app/slider.py`
-    - transform `kit/gui/shape/` -> `app/arrow.py`
-    - transform `kit/neuralnet/dense/` -> `kit/neuralnet/dense.py`
-    - transform `kit/neuralnet/genetic/` -> `kit/neuralnet/genetic.py`
+    - removed `get_gray` from `/kit/color.py`
+    - transform `/kit/gui/button/` -> `/app/button.py`
+    - transform `/kit/gui/label/` -> `/app/label.py`
+    - transform `/kit/gui/slider/` -> `/app/slider.py`
+    - transform `/kit/gui/shape/` -> `/app/arrow.py`
+    - transform `/kit/neuralnet/dense/` -> `/kit/neuralnet/dense.py`
+    - transform `/kit/neuralnet/genetic/` -> `/kit/neuralnet/genetic.py`
 - 0.1.0 (June 12, 2023):
-    - migrated all modules from [carbon](https://github.com/nvfp/carbon) into `kit/`
-    - deleted `kit/math/`
-    - added `rec/` and `app/`
-    - transform `kit/color/` -> `kit/color.py`
-    - moved `kit/color/test_color.py` to `mykit/tests/test_kit/test_color.py`
-    - transform `kit/ffmpeg/` -> `kit/ffmpeg.py`
-    - deleted `kit/graph/graph2d/`
-    - transform `kit/graph/graph2d/v2.py` -> `kit/graph/graph2d.py`
-    - transform `kit/maths/` -> `kit/math.py`
-    - moved `kit/maths/test_maths.py` -> `mykit/tests/test_math.py`
-    - transform `kit/noise/` -> `kit/noise.py`
-    - transform `kit/path/` -> `kit/path.py`
-    - transform `kit/text/` -> `kit/text.py`
-    - transform `kit/time/` -> `kit/time.py`
-    - transform `kit/utils/` -> `kit/utils.py`
+    - migrated all modules from [carbon](https://github.com/nvfp/carbon) into `/kit/`
+    - deleted `/kit/math/`
+    - added `/rec/` and `/app/`
+    - transform `/kit/color/` -> `/kit/color.py`
+    - moved `/kit/color/test_color.py` to `mykit/tests/test_kit/test_color.py`
+    - transform `/kit/ffmpeg/` -> `/kit/ffmpeg.py`
+    - deleted `/kit/graph/graph2d/`
+    - transform `/kit/graph/graph2d/v2.py` -> `/kit/graph/graph2d.py`
+    - transform `/kit/maths/` -> `/kit/math.py`
+    - moved `/kit/maths/test_maths.py` -> `mykit/tests/test_math.py`
+    - transform `/kit/noise/` -> `/kit/noise.py`
+    - transform `/kit/path/` -> `/kit/path.py`
+    - transform `/kit/text/` -> `/kit/text.py`
+    - transform `/kit/time/` -> `/kit/time.py`
+    - transform `/kit/utils/` -> `/kit/utils.py`
 
 
 ## Troubleshoot
 
 - To report bugs, please open an issue/pull request, or you can reach me [here](https://nvfp.github.io/contact).
```

### Comparing `mykit-2.0.0rc1/README.md` & `mykit-2.0.0rc2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # myKit
 
 Python utility toolkit.
 
-![mykit's banner](assets/20230613-mykit-banner-fhd.png)
+![mykit's banner](https://raw.githubusercontent.com/nvfp/mykit/master/assets/20230613-mykit-banner-fhd.png)
 
 [![pypi version](https://img.shields.io/pypi/v/mykit?logo=pypi)](https://pypi.org/project/mykit/)
 [![MIT License](https://img.shields.io/badge/license-MIT-blue.svg?style=flat)](http://choosealicense.com/licenses/mit/)
 
 
 ## Installation
 
@@ -33,44 +33,46 @@
 - 
 
 
 ## Changelog
 
 - 2.0.0 (June 13, 2023):
     - Breaking changes:
-        - New mechanism for app: `app/__init__.py`
-        - Moved: `kit/graph/graph2d.py` -> `app/complex/plot.py`
-        - transform: `kit/quick_visual/plot2d.py` -> `kit/fast_visualizations/static/plot.py`
-    - New: `app/complex/biplot.py`
+        - New mechanism for app: `/app/__init__.py`
+        - Moved: `/kit/graph/graph2d.py` -> `/app/complex/plot.py`
+        - transform: `/kit/quick_visual/plot2d.py` -> `/kit/fast_visualizations/static/plot.py`
+    - Bugfixed:
+        - folder `mykit/tests/` should also be excluded during build (rc version)
+    - New: `/app/complex/biplot.py`
 - 1.0.0 (June 12, 2023):
-    - changed arg name: `kit/quick_visual/plot2d.py`: `graph2d_cfg` -> `cfg`
+    - changed arg name: `/kit/quick_visual/plot2d.py`: `graph2d_cfg` -> `cfg`
 - 0.1.3 (June 12, 2023):
-    - removed `get_gray` from `kit/color.py`
-    - transform `kit/gui/button/` -> `app/button.py`
-    - transform `kit/gui/label/` -> `app/label.py`
-    - transform `kit/gui/slider/` -> `app/slider.py`
-    - transform `kit/gui/shape/` -> `app/arrow.py`
-    - transform `kit/neuralnet/dense/` -> `kit/neuralnet/dense.py`
-    - transform `kit/neuralnet/genetic/` -> `kit/neuralnet/genetic.py`
+    - removed `get_gray` from `/kit/color.py`
+    - transform `/kit/gui/button/` -> `/app/button.py`
+    - transform `/kit/gui/label/` -> `/app/label.py`
+    - transform `/kit/gui/slider/` -> `/app/slider.py`
+    - transform `/kit/gui/shape/` -> `/app/arrow.py`
+    - transform `/kit/neuralnet/dense/` -> `/kit/neuralnet/dense.py`
+    - transform `/kit/neuralnet/genetic/` -> `/kit/neuralnet/genetic.py`
 - 0.1.0 (June 12, 2023):
-    - migrated all modules from [carbon](https://github.com/nvfp/carbon) into `kit/`
-    - deleted `kit/math/`
-    - added `rec/` and `app/`
-    - transform `kit/color/` -> `kit/color.py`
-    - moved `kit/color/test_color.py` to `mykit/tests/test_kit/test_color.py`
-    - transform `kit/ffmpeg/` -> `kit/ffmpeg.py`
-    - deleted `kit/graph/graph2d/`
-    - transform `kit/graph/graph2d/v2.py` -> `kit/graph/graph2d.py`
-    - transform `kit/maths/` -> `kit/math.py`
-    - moved `kit/maths/test_maths.py` -> `mykit/tests/test_math.py`
-    - transform `kit/noise/` -> `kit/noise.py`
-    - transform `kit/path/` -> `kit/path.py`
-    - transform `kit/text/` -> `kit/text.py`
-    - transform `kit/time/` -> `kit/time.py`
-    - transform `kit/utils/` -> `kit/utils.py`
+    - migrated all modules from [carbon](https://github.com/nvfp/carbon) into `/kit/`
+    - deleted `/kit/math/`
+    - added `/rec/` and `/app/`
+    - transform `/kit/color/` -> `/kit/color.py`
+    - moved `/kit/color/test_color.py` to `mykit/tests/test_kit/test_color.py`
+    - transform `/kit/ffmpeg/` -> `/kit/ffmpeg.py`
+    - deleted `/kit/graph/graph2d/`
+    - transform `/kit/graph/graph2d/v2.py` -> `/kit/graph/graph2d.py`
+    - transform `/kit/maths/` -> `/kit/math.py`
+    - moved `/kit/maths/test_maths.py` -> `mykit/tests/test_math.py`
+    - transform `/kit/noise/` -> `/kit/noise.py`
+    - transform `/kit/path/` -> `/kit/path.py`
+    - transform `/kit/text/` -> `/kit/text.py`
+    - transform `/kit/time/` -> `/kit/time.py`
+    - transform `/kit/utils/` -> `/kit/utils.py`
 
 
 ## Troubleshoot
 
 - To report bugs, please open an issue/pull request, or you can reach me [here](https://nvfp.github.io/contact).
```

### Comparing `mykit-2.0.0rc1/mykit/app/__init__.py` & `mykit-2.0.0rc2/mykit/app/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -45,20 +45,25 @@
         self._left_mouse_hold = []
         self._left_mouse_release = []
 
         self._setup = None
         self._teardown = None
         ## </runtime>
 
-    def listen(self, to: str, do: _typing.Callable[[_tk.Event[_tk.Misc]], None]):
+    def listen(self, to: str, do: _typing.Callable[[_tk.Event], None]):
         """
         Add event listener.
 
         ---
+
+        ## Params
         - `to`: `Literal["left-mouse-press", "left-mouse-hold", "left-mouse-release"]`
+
+        ## Docs
+        - `do` function takes 1 positional parameter, which is a tkinter event object
         """
         
         if to == 'left-mouse-press':
             self._left_mouse_press.append(do)
         elif to == 'left-mouse-hold':
             self._left_mouse_hold.append(do)
         elif to == 'left-mouse-release':
```

### Comparing `mykit-2.0.0rc1/mykit/app/arrow.py` & `mykit-2.0.0rc2/mykit/app/arrow.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.0rc1/mykit/app/button.py` & `mykit-2.0.0rc2/mykit/app/button.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.0rc1/mykit/app/complex/biplot.py` & `mykit-2.0.0rc2/mykit/app/complex/biplot.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.0rc1/mykit/app/complex/plot.py` & `mykit-2.0.0rc2/mykit/app/complex/plot.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.0rc1/mykit/app/label.py` & `mykit-2.0.0rc2/mykit/app/label.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.0rc1/mykit/app/slider.py` & `mykit-2.0.0rc2/mykit/app/slider.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.0rc1/mykit/kit/color.py` & `mykit-2.0.0rc2/mykit/kit/color.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.0rc1/mykit/kit/ffmpeg.py` & `mykit-2.0.0rc2/mykit/kit/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.0rc1/mykit/kit/keycrate/__init__.py` & `mykit-2.0.0rc2/mykit/kit/keycrate/__init__.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.0rc1/mykit/kit/math.py` & `mykit-2.0.0rc2/mykit/kit/math.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.0rc1/mykit/kit/neuralnet/dense.py` & `mykit-2.0.0rc2/mykit/kit/neuralnet/dense.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.0rc1/mykit/kit/neuralnet/genetic.py` & `mykit-2.0.0rc2/mykit/kit/neuralnet/genetic.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.0rc1/mykit/kit/noise.py` & `mykit-2.0.0rc2/mykit/kit/noise.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.0rc1/mykit/kit/path.py` & `mykit-2.0.0rc2/mykit/kit/path.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.0rc1/mykit/kit/time.py` & `mykit-2.0.0rc2/mykit/kit/time.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.0rc1/mykit/kit/utils.py` & `mykit-2.0.0rc2/mykit/kit/utils.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.0rc1/mykit.egg-info/PKG-INFO` & `mykit-2.0.0rc2/mykit.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mykit
-Version: 2.0.0rc1
+Version: 2.0.0rc2
 Summary: Python utility library
 Home-page: https://nvfp.github.io/mykit
 Author: Nicholas Valentinus
 Author-email: nvfastplease@gmail.com
 License: MIT
 Project-URL: documentation, https://nvfp.github.io/mykit/docs
 Project-URL: report bugs, https://github.com/nvfp/mykit/issues
@@ -26,15 +26,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # myKit
 
 Python utility toolkit.
 
-![mykit's banner](assets/20230613-mykit-banner-fhd.png)
+![mykit's banner](https://raw.githubusercontent.com/nvfp/mykit/master/assets/20230613-mykit-banner-fhd.png)
 
 [![pypi version](https://img.shields.io/pypi/v/mykit?logo=pypi)](https://pypi.org/project/mykit/)
 [![MIT License](https://img.shields.io/badge/license-MIT-blue.svg?style=flat)](http://choosealicense.com/licenses/mit/)
 
 
 ## Installation
 
@@ -61,44 +61,46 @@
 - 
 
 
 ## Changelog
 
 - 2.0.0 (June 13, 2023):
     - Breaking changes:
-        - New mechanism for app: `app/__init__.py`
-        - Moved: `kit/graph/graph2d.py` -> `app/complex/plot.py`
-        - transform: `kit/quick_visual/plot2d.py` -> `kit/fast_visualizations/static/plot.py`
-    - New: `app/complex/biplot.py`
+        - New mechanism for app: `/app/__init__.py`
+        - Moved: `/kit/graph/graph2d.py` -> `/app/complex/plot.py`
+        - transform: `/kit/quick_visual/plot2d.py` -> `/kit/fast_visualizations/static/plot.py`
+    - Bugfixed:
+        - folder `mykit/tests/` should also be excluded during build (rc version)
+    - New: `/app/complex/biplot.py`
 - 1.0.0 (June 12, 2023):
-    - changed arg name: `kit/quick_visual/plot2d.py`: `graph2d_cfg` -> `cfg`
+    - changed arg name: `/kit/quick_visual/plot2d.py`: `graph2d_cfg` -> `cfg`
 - 0.1.3 (June 12, 2023):
-    - removed `get_gray` from `kit/color.py`
-    - transform `kit/gui/button/` -> `app/button.py`
-    - transform `kit/gui/label/` -> `app/label.py`
-    - transform `kit/gui/slider/` -> `app/slider.py`
-    - transform `kit/gui/shape/` -> `app/arrow.py`
-    - transform `kit/neuralnet/dense/` -> `kit/neuralnet/dense.py`
-    - transform `kit/neuralnet/genetic/` -> `kit/neuralnet/genetic.py`
+    - removed `get_gray` from `/kit/color.py`
+    - transform `/kit/gui/button/` -> `/app/button.py`
+    - transform `/kit/gui/label/` -> `/app/label.py`
+    - transform `/kit/gui/slider/` -> `/app/slider.py`
+    - transform `/kit/gui/shape/` -> `/app/arrow.py`
+    - transform `/kit/neuralnet/dense/` -> `/kit/neuralnet/dense.py`
+    - transform `/kit/neuralnet/genetic/` -> `/kit/neuralnet/genetic.py`
 - 0.1.0 (June 12, 2023):
-    - migrated all modules from [carbon](https://github.com/nvfp/carbon) into `kit/`
-    - deleted `kit/math/`
-    - added `rec/` and `app/`
-    - transform `kit/color/` -> `kit/color.py`
-    - moved `kit/color/test_color.py` to `mykit/tests/test_kit/test_color.py`
-    - transform `kit/ffmpeg/` -> `kit/ffmpeg.py`
-    - deleted `kit/graph/graph2d/`
-    - transform `kit/graph/graph2d/v2.py` -> `kit/graph/graph2d.py`
-    - transform `kit/maths/` -> `kit/math.py`
-    - moved `kit/maths/test_maths.py` -> `mykit/tests/test_math.py`
-    - transform `kit/noise/` -> `kit/noise.py`
-    - transform `kit/path/` -> `kit/path.py`
-    - transform `kit/text/` -> `kit/text.py`
-    - transform `kit/time/` -> `kit/time.py`
-    - transform `kit/utils/` -> `kit/utils.py`
+    - migrated all modules from [carbon](https://github.com/nvfp/carbon) into `/kit/`
+    - deleted `/kit/math/`
+    - added `/rec/` and `/app/`
+    - transform `/kit/color/` -> `/kit/color.py`
+    - moved `/kit/color/test_color.py` to `mykit/tests/test_kit/test_color.py`
+    - transform `/kit/ffmpeg/` -> `/kit/ffmpeg.py`
+    - deleted `/kit/graph/graph2d/`
+    - transform `/kit/graph/graph2d/v2.py` -> `/kit/graph/graph2d.py`
+    - transform `/kit/maths/` -> `/kit/math.py`
+    - moved `/kit/maths/test_maths.py` -> `mykit/tests/test_math.py`
+    - transform `/kit/noise/` -> `/kit/noise.py`
+    - transform `/kit/path/` -> `/kit/path.py`
+    - transform `/kit/text/` -> `/kit/text.py`
+    - transform `/kit/time/` -> `/kit/time.py`
+    - transform `/kit/utils/` -> `/kit/utils.py`
 
 
 ## Troubleshoot
 
 - To report bugs, please open an issue/pull request, or you can reach me [here](https://nvfp.github.io/contact).
```

### Comparing `mykit-2.0.0rc1/mykit.egg-info/SOURCES.txt` & `mykit-2.0.0rc2/mykit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mykit-2.0.0rc1/pyproject.toml` & `mykit-2.0.0rc2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "mykit"
-version = "2.0.0-rc-1"
+version = "2.0.0-rc-2"
 description = "Python utility library"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {text = "MIT"}
 authors = [
   	{email = "nvfastplease@gmail.com"},
 ]
@@ -30,15 +30,18 @@
 dependencies = [
 	"numba>=0.55.2",
 	"numpy>=1.22.4"
 ]
 
 
 [tool.setuptools.packages.find]
-exclude = ["assets*"]
+exclude = [
+    "assets*",
+    "tests*"
+]
 
 
 [project.urls]
 documentation = "https://nvfp.github.io/mykit/docs"
 "report bugs" = "https://github.com/nvfp/mykit/issues"
 repo = "https://github.com/nvfp/mykit"
 changelog = "https://nvfp.github.io/mykit/changelog"
```

### Comparing `mykit-2.0.0rc1/tests/test_kit/test_color.py` & `mykit-2.0.0rc2/tests/test_kit/test_color.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.0rc1/tests/test_kit/test_math.py` & `mykit-2.0.0rc2/tests/test_kit/test_math.py`

 * *Files identical despite different names*

