# Comparing `tmp/lqcv-0.1.0.tar.gz` & `tmp/lqcv-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lqcv-0.1.0.tar", last modified: Wed May 17 05:53:06 2023, max compression
+gzip compressed data, was "lqcv-0.2.0.tar", last modified: Tue Jun 13 09:13:17 2023, max compression
```

## Comparing `lqcv-0.1.0.tar` & `lqcv-0.2.0.tar`

### file list

```diff
@@ -1,61 +1,45 @@
-drwxr-xr-x   0 laughing  (1000) wheel      (998)        0 2023-05-17 05:53:06.293211 lqcv-0.1.0/
--rw-r--r--   0 laughing  (1000) wheel      (998)      770 2023-05-17 05:53:06.293211 lqcv-0.1.0/PKG-INFO
--rw-r--r--   0 laughing  (1000) wheel      (998)      584 2022-07-07 09:32:49.000000 lqcv-0.1.0/README.md
-drwxr-xr-x   0 laughing  (1000) wheel      (998)        0 2023-05-17 05:53:06.289877 lqcv-0.1.0/lqcv/
--rw-r--r--   0 laughing  (1000) wheel      (998)       66 2022-06-25 07:22:08.000000 lqcv-0.1.0/lqcv/__init__.py
-drwxr-xr-x   0 laughing  (1000) wheel      (998)        0 2023-05-17 05:53:06.289877 lqcv-0.1.0/lqcv/bbox/
--rw-r--r--   0 laughing  (1000) wheel      (998)       70 2022-07-14 06:17:43.000000 lqcv-0.1.0/lqcv/bbox/__init__.py
--rw-r--r--   0 laughing  (1000) wheel      (998)     8775 2022-06-24 06:36:13.000000 lqcv-0.1.0/lqcv/bbox/areas.py
--rw-r--r--   0 laughing  (1000) wheel      (998)     3179 2022-06-24 06:36:13.000000 lqcv-0.1.0/lqcv/bbox/bbox_utils.py
--rw-r--r--   0 laughing  (1000) wheel      (998)     3290 2022-07-14 06:17:43.000000 lqcv-0.1.0/lqcv/bbox/convert.py
--rw-r--r--   0 laughing  (1000) wheel      (998)     4525 2022-11-30 09:07:12.000000 lqcv-0.1.0/lqcv/bbox/utils.py
-drwxr-xr-x   0 laughing  (1000) wheel      (998)        0 2023-05-17 05:53:06.289877 lqcv-0.1.0/lqcv/data/
--rw-r--r--   0 laughing  (1000) wheel      (998)       39 2022-06-24 06:36:13.000000 lqcv-0.1.0/lqcv/data/__init__.py
--rw-r--r--   0 laughing  (1000) wheel      (998)    10730 2023-02-01 06:45:50.000000 lqcv-0.1.0/lqcv/data/data_reader.py
-drwxr-xr-x   0 laughing  (1000) wheel      (998)        0 2023-05-17 05:53:06.289877 lqcv-0.1.0/lqcv/fileio/
--rw-r--r--   0 laughing  (1000) wheel      (998)      478 2022-06-25 02:20:53.000000 lqcv-0.1.0/lqcv/fileio/__init__.py
--rw-r--r--   0 laughing  (1000) wheel      (998)    42383 2022-06-25 07:25:19.000000 lqcv-0.1.0/lqcv/fileio/file_client.py
-drwxr-xr-x   0 laughing  (1000) wheel      (998)        0 2023-05-17 05:53:06.289877 lqcv-0.1.0/lqcv/fileio/handlers/
--rw-r--r--   0 laughing  (1000) wheel      (998)      278 2022-06-25 02:20:53.000000 lqcv-0.1.0/lqcv/fileio/handlers/__init__.py
--rw-r--r--   0 laughing  (1000) wheel      (998)     1017 2022-06-25 02:20:53.000000 lqcv-0.1.0/lqcv/fileio/handlers/base.py
--rw-r--r--   0 laughing  (1000) wheel      (998)     1068 2022-06-25 02:20:53.000000 lqcv-0.1.0/lqcv/fileio/handlers/json_handler.py
--rw-r--r--   0 laughing  (1000) wheel      (998)      753 2022-06-25 02:20:53.000000 lqcv-0.1.0/lqcv/fileio/handlers/pickle_handler.py
--rw-r--r--   0 laughing  (1000) wheel      (998)      701 2022-06-25 02:20:53.000000 lqcv-0.1.0/lqcv/fileio/handlers/yaml_handler.py
--rw-r--r--   0 laughing  (1000) wheel      (998)     6035 2022-06-25 07:25:45.000000 lqcv-0.1.0/lqcv/fileio/io.py
--rw-r--r--   0 laughing  (1000) wheel      (998)     3661 2022-06-25 02:20:53.000000 lqcv-0.1.0/lqcv/fileio/parse.py
-drwxr-xr-x   0 laughing  (1000) wheel      (998)        0 2023-05-17 05:53:06.289877 lqcv-0.1.0/lqcv/image/
--rw-r--r--   0 laughing  (1000) wheel      (998)       25 2022-07-08 08:29:09.000000 lqcv-0.1.0/lqcv/image/__init__.py
--rw-r--r--   0 laughing  (1000) wheel      (998)     1436 2022-07-14 07:07:48.000000 lqcv-0.1.0/lqcv/image/geometric.py
--rw-r--r--   0 laughing  (1000) wheel      (998)     1606 2022-06-24 06:36:13.000000 lqcv-0.1.0/lqcv/image/utils.py
-drwxr-xr-x   0 laughing  (1000) wheel      (998)        0 2023-05-17 05:53:06.289877 lqcv-0.1.0/lqcv/segment/
--rw-r--r--   0 laughing  (1000) wheel      (998)        0 2022-06-24 06:36:13.000000 lqcv-0.1.0/lqcv/segment/__init__.py
--rw-r--r--   0 laughing  (1000) wheel      (998)     1538 2022-06-24 06:36:13.000000 lqcv-0.1.0/lqcv/segment/polygon.py
--rw-r--r--   0 laughing  (1000) wheel      (998)     2051 2022-06-24 06:36:13.000000 lqcv-0.1.0/lqcv/segment/utils.py
-drwxr-xr-x   0 laughing  (1000) wheel      (998)        0 2023-05-17 05:53:06.293211 lqcv-0.1.0/lqcv/utils/
--rw-r--r--   0 laughing  (1000) wheel      (998)      157 2022-07-08 09:38:06.000000 lqcv-0.1.0/lqcv/utils/__init__.py
--rw-r--r--   0 laughing  (1000) wheel      (998)     8593 2022-06-24 06:36:13.000000 lqcv-0.1.0/lqcv/utils/checker.py
--rw-r--r--   0 laughing  (1000) wheel      (998)    27981 2022-06-25 07:26:31.000000 lqcv-0.1.0/lqcv/utils/config.py
--rw-r--r--   0 laughing  (1000) wheel      (998)     5270 2022-06-24 06:36:13.000000 lqcv-0.1.0/lqcv/utils/general.py
--rw-r--r--   0 laughing  (1000) wheel      (998)    11439 2022-06-25 07:23:39.000000 lqcv-0.1.0/lqcv/utils/misc.py
--rw-r--r--   0 laughing  (1000) wheel      (998)     1028 2022-06-25 07:24:47.000000 lqcv-0.1.0/lqcv/utils/path.py
--rw-r--r--   0 laughing  (1000) wheel      (998)     3293 2022-06-25 09:58:10.000000 lqcv-0.1.0/lqcv/utils/registry.py
--rw-r--r--   0 laughing  (1000) wheel      (998)     4290 2022-06-24 06:36:13.000000 lqcv-0.1.0/lqcv/utils/timer.py
-drwxr-xr-x   0 laughing  (1000) wheel      (998)        0 2023-05-17 05:53:06.293211 lqcv-0.1.0/lqcv/video/
--rw-r--r--   0 laughing  (1000) wheel      (998)        0 2022-06-24 06:36:13.000000 lqcv-0.1.0/lqcv/video/__init__.py
--rw-r--r--   0 laughing  (1000) wheel      (998)      158 2022-06-24 06:36:13.000000 lqcv-0.1.0/lqcv/video/utils.py
--rw-r--r--   0 laughing  (1000) wheel      (998)     4205 2022-06-24 06:36:13.000000 lqcv-0.1.0/lqcv/video/video2image.py
-drwxr-xr-x   0 laughing  (1000) wheel      (998)        0 2023-05-17 05:53:06.293211 lqcv-0.1.0/lqcv/visualization/
--rw-r--r--   0 laughing  (1000) wheel      (998)        0 2022-06-24 06:36:13.000000 lqcv-0.1.0/lqcv/visualization/__init__.py
--rw-r--r--   0 laughing  (1000) wheel      (998)     1048 2022-06-24 06:36:13.000000 lqcv-0.1.0/lqcv/visualization/color.py
--rw-r--r--   0 laughing  (1000) wheel      (998)     7933 2022-06-24 06:36:13.000000 lqcv-0.1.0/lqcv/visualization/image.py
--rw-r--r--   0 laughing  (1000) wheel      (998)     1213 2022-06-24 06:36:13.000000 lqcv-0.1.0/lqcv/visualization/utils.py
-drwxr-xr-x   0 laughing  (1000) wheel      (998)        0 2023-05-17 05:53:06.289877 lqcv-0.1.0/lqcv.egg-info/
--rw-r--r--   0 laughing  (1000) wheel      (998)      770 2023-05-17 05:53:06.000000 lqcv-0.1.0/lqcv.egg-info/PKG-INFO
--rw-r--r--   0 laughing  (1000) wheel      (998)     1093 2023-05-17 05:53:06.000000 lqcv-0.1.0/lqcv.egg-info/SOURCES.txt
--rw-r--r--   0 laughing  (1000) wheel      (998)        1 2023-05-17 05:53:06.000000 lqcv-0.1.0/lqcv.egg-info/dependency_links.txt
--rw-r--r--   0 laughing  (1000) wheel      (998)        5 2023-05-17 05:53:06.000000 lqcv-0.1.0/lqcv.egg-info/top_level.txt
--rw-r--r--   0 laughing  (1000) wheel      (998)       38 2023-05-17 05:53:06.293211 lqcv-0.1.0/setup.cfg
--rw-r--r--   0 laughing  (1000) wheel      (998)      776 2022-06-24 06:36:13.000000 lqcv-0.1.0/setup.py
-drwxr-xr-x   0 laughing  (1000) wheel      (998)        0 2023-05-17 05:53:06.293211 lqcv-0.1.0/test/
--rw-r--r--   0 laughing  (1000) wheel      (998)     2948 2022-06-24 06:36:13.000000 lqcv-0.1.0/test/test_area.py
--rw-r--r--   0 laughing  (1000) wheel      (998)      567 2022-06-24 06:36:13.000000 lqcv-0.1.0/test/test_reader.py
+drwxr-xr-x   0 laughing  (1000) wheel      (998)        0 2023-06-13 09:13:17.405139 lqcv-0.2.0/
+-rw-r--r--   0 laughing  (1000) wheel      (998)      770 2023-06-13 09:13:17.405139 lqcv-0.2.0/PKG-INFO
+-rw-r--r--   0 laughing  (1000) wheel      (998)      584 2022-07-07 09:32:49.000000 lqcv-0.2.0/README.md
+drwxr-xr-x   0 laughing  (1000) wheel      (998)        0 2023-06-13 09:13:17.401805 lqcv-0.2.0/lqcv/
+-rw-r--r--   0 laughing  (1000) wheel      (998)       64 2023-06-13 09:12:34.000000 lqcv-0.2.0/lqcv/__init__.py
+drwxr-xr-x   0 laughing  (1000) wheel      (998)        0 2023-06-13 09:13:17.401805 lqcv-0.2.0/lqcv/bbox/
+-rw-r--r--   0 laughing  (1000) wheel      (998)       41 2023-06-13 09:11:38.000000 lqcv-0.2.0/lqcv/bbox/__init__.py
+-rw-r--r--   0 laughing  (1000) wheel      (998)    10031 2023-06-13 09:11:38.000000 lqcv-0.2.0/lqcv/bbox/areas.py
+-rw-r--r--   0 laughing  (1000) wheel      (998)     5723 2023-06-13 09:11:38.000000 lqcv-0.2.0/lqcv/bbox/bbox.py
+drwxr-xr-x   0 laughing  (1000) wheel      (998)        0 2023-06-13 09:13:17.401805 lqcv-0.2.0/lqcv/data/
+-rw-r--r--   0 laughing  (1000) wheel      (998)       70 2023-06-13 09:11:38.000000 lqcv-0.2.0/lqcv/data/__init__.py
+drwxr-xr-x   0 laughing  (1000) wheel      (998)        0 2023-06-13 09:13:17.401805 lqcv-0.2.0/lqcv/data/converter/
+-rw-r--r--   0 laughing  (1000) wheel      (998)       94 2023-06-13 09:11:38.000000 lqcv-0.2.0/lqcv/data/converter/__init__.py
+-rw-r--r--   0 laughing  (1000) wheel      (998)    10948 2023-06-13 09:11:38.000000 lqcv-0.2.0/lqcv/data/converter/base.py
+-rw-r--r--   0 laughing  (1000) wheel      (998)     3262 2023-06-13 09:11:38.000000 lqcv-0.2.0/lqcv/data/converter/coco.py
+-rw-r--r--   0 laughing  (1000) wheel      (998)     4421 2023-06-13 09:11:38.000000 lqcv-0.2.0/lqcv/data/converter/xml.py
+-rw-r--r--   0 laughing  (1000) wheel      (998)     4955 2023-06-13 09:11:38.000000 lqcv-0.2.0/lqcv/data/converter/yolo.py
+-rw-r--r--   0 laughing  (1000) wheel      (998)    11718 2023-06-13 09:11:38.000000 lqcv-0.2.0/lqcv/data/reader.py
+-rw-r--r--   0 laughing  (1000) wheel      (998)      407 2023-06-13 09:11:38.000000 lqcv-0.2.0/lqcv/data/utils.py
+drwxr-xr-x   0 laughing  (1000) wheel      (998)        0 2023-06-13 09:13:17.401805 lqcv-0.2.0/lqcv/simi/
+-rw-r--r--   0 laughing  (1000) wheel      (998)        0 2023-06-13 09:11:38.000000 lqcv-0.2.0/lqcv/simi/__init__.py
+-rw-r--r--   0 laughing  (1000) wheel      (998)     1033 2023-06-13 09:11:38.000000 lqcv-0.2.0/lqcv/simi/hash.py
+drwxr-xr-x   0 laughing  (1000) wheel      (998)        0 2023-06-13 09:13:17.405139 lqcv-0.2.0/lqcv/tools/
+-rw-r--r--   0 laughing  (1000) wheel      (998)      132 2023-06-13 09:11:38.000000 lqcv-0.2.0/lqcv/tools/__init__.py
+-rw-r--r--   0 laughing  (1000) wheel      (998)     2683 2023-06-13 09:11:38.000000 lqcv-0.2.0/lqcv/tools/file.py
+-rw-r--r--   0 laughing  (1000) wheel      (998)     4034 2023-06-13 09:11:38.000000 lqcv-0.2.0/lqcv/tools/image.py
+-rw-r--r--   0 laughing  (1000) wheel      (998)     1718 2023-06-13 09:11:38.000000 lqcv-0.2.0/lqcv/tools/video.py
+drwxr-xr-x   0 laughing  (1000) wheel      (998)        0 2023-06-13 09:13:17.405139 lqcv-0.2.0/lqcv/utils/
+-rw-r--r--   0 laughing  (1000) wheel      (998)       32 2023-06-13 09:11:38.000000 lqcv-0.2.0/lqcv/utils/__init__.py
+-rw-r--r--   0 laughing  (1000) wheel      (998)      697 2023-06-13 09:11:38.000000 lqcv-0.2.0/lqcv/utils/log.py
+-rw-r--r--   0 laughing  (1000) wheel      (998)     5183 2023-06-13 09:11:38.000000 lqcv-0.2.0/lqcv/utils/ops.py
+-rw-r--r--   0 laughing  (1000) wheel      (998)     2122 2023-06-13 09:11:38.000000 lqcv-0.2.0/lqcv/utils/plot.py
+-rw-r--r--   0 laughing  (1000) wheel      (998)     3570 2023-06-13 09:11:38.000000 lqcv-0.2.0/lqcv/utils/timer.py
+drwxr-xr-x   0 laughing  (1000) wheel      (998)        0 2023-06-13 09:13:17.401805 lqcv-0.2.0/lqcv.egg-info/
+-rw-r--r--   0 laughing  (1000) wheel      (998)      770 2023-06-13 09:13:17.000000 lqcv-0.2.0/lqcv.egg-info/PKG-INFO
+-rw-r--r--   0 laughing  (1000) wheel      (998)      709 2023-06-13 09:13:17.000000 lqcv-0.2.0/lqcv.egg-info/SOURCES.txt
+-rw-r--r--   0 laughing  (1000) wheel      (998)        1 2023-06-13 09:13:17.000000 lqcv-0.2.0/lqcv.egg-info/dependency_links.txt
+-rw-r--r--   0 laughing  (1000) wheel      (998)        5 2023-06-13 09:13:17.000000 lqcv-0.2.0/lqcv.egg-info/top_level.txt
+-rw-r--r--   0 laughing  (1000) wheel      (998)       38 2023-06-13 09:13:17.405139 lqcv-0.2.0/setup.cfg
+-rw-r--r--   0 laughing  (1000) wheel      (998)      776 2023-05-30 03:03:32.000000 lqcv-0.2.0/setup.py
+drwxr-xr-x   0 laughing  (1000) wheel      (998)        0 2023-06-13 09:13:17.405139 lqcv-0.2.0/test/
+-rw-r--r--   0 laughing  (1000) wheel      (998)     2128 2023-06-13 09:11:38.000000 lqcv-0.2.0/test/test_area.py
+-rw-r--r--   0 laughing  (1000) wheel      (998)     2005 2023-06-13 09:11:38.000000 lqcv-0.2.0/test/test_converter.py
+-rw-r--r--   0 laughing  (1000) wheel      (998)     1737 2023-06-13 09:11:38.000000 lqcv-0.2.0/test/test_reader.py
+-rw-r--r--   0 laughing  (1000) wheel      (998)      178 2023-06-13 09:11:38.000000 lqcv-0.2.0/test/test_tool.py
```

### Comparing `lqcv-0.1.0/PKG-INFO` & `lqcv-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lqcv
-Version: 0.1.0
+Version: 0.2.0
 Author: Laughing-q
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 
 # lqcv
 This is my computer vision lib.
```

### Comparing `lqcv-0.1.0/README.md` & `lqcv-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `lqcv-0.1.0/lqcv/data/data_reader.py` & `lqcv-0.2.0/lqcv/data/reader.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,74 +1,53 @@
 import glob
 import os.path as osp
 import cv2
 import time
 from pathlib import Path
 from threading import Thread
-from ..image.utils import IMG_FORMATS
-from ..video.utils import VID_FORMATS
-from ..utils.checker import check_requirements
-from ..utils.general import clean_str
-
-"""
-NOTE:
-    `ReadVideosAndImages` and `ReadStreams` are pure data readers without preprocessing.
-"""
+from .utils import IMG_FORMATS, VID_FORMATS
 
 
 class ReadStreams:
     """Read Streams, modified from yolov5, support multi streams reading, but support one streams saving for now."""
 
     def __init__(self, sources="streams.txt"):
         self.mode = "stream"
 
         if osp.isfile(sources):
             with open(sources, "r") as f:
-                sources = [
-                    x.strip() for x in f.read().strip().splitlines() if len(x.strip())
-                ]
+                sources = [x.strip() for x in f.read().strip().splitlines() if len(x.strip())]
         else:
             sources = [sources]
 
         n = len(sources)
         self.vid_path, self.vid_writer = [None] * n, [None] * n
         self.imgs, self.fps, self.frames, self.threads = (
             [None] * n,
             [0] * n,
             [0] * n,
             [None] * n,
         )
-        self.sources = [clean_str(x) for x in sources]  # clean source names for later
+        self.sources = sources  # clean source names for later
         for i, s in enumerate(sources):  # index, source
             # Start thread to read frames from video stream
             print(f"{i + 1}/{n}: {s}... ", end="")
-            if "youtube.com/" in s or "youtu.be/" in s:  # if source is YouTube video
-                check_requirements(("pafy", "youtube_dl"))
-                import pafy
-
-                s = pafy.new(s).getbest(preftype="mp4").url  # YouTube URL
             s = eval(s) if s.isnumeric() else s  # i.e. s = '0' local webcam
             cap = cv2.VideoCapture(s)
             assert cap.isOpened(), f"Failed to open {s}"
             w = int(cap.get(cv2.CAP_PROP_FRAME_WIDTH))
             h = int(cap.get(cv2.CAP_PROP_FRAME_HEIGHT))
-            self.fps[i] = (
-                max(cap.get(cv2.CAP_PROP_FPS) % 100, 0) or 30.0
-            )  # 30 FPS fallback
+            self.fps[i] = max(cap.get(cv2.CAP_PROP_FPS) % 100, 0) or 30.0  # 30 FPS fallback
             self.frames[i] = max(int(cap.get(cv2.CAP_PROP_FRAME_COUNT)), 0) or float(
                 "inf"
             )  # infinite stream fallback
 
             _, self.imgs[i] = cap.read()  # guarantee first frame
-            self.threads[i] = Thread(
-                target=self.update, args=([i, cap, s]), daemon=True
-            )
-            print(
-                f" success ({self.frames[i]} frames {w}x{h} at {self.fps[i]:.2f} FPS)"
-            )
+            self.threads[i] = Thread(target=self.update, args=([i, cap, s]), daemon=True)
+            print(f" success ({self.frames[i]} frames {w}x{h} at {self.fps[i]:.2f} FPS)")
             self.threads[i].start()
         print("")  # newline
 
     def update(self, i, cap, stream):
         # Read stream `i` frames in daemon thread
         n, f, read = (
             0,
@@ -80,30 +59,26 @@
             # _, self.imgs[index] = cap.read()
             cap.grab()
             if n % read == 0:
                 success, im = cap.retrieve()
                 if success:
                     self.imgs[i] = im
                 else:
-                    print(
-                        "WARNING: Video stream unresponsive, please check your IP camera connection."
-                    )
+                    print("WARNING: Video stream unresponsive, please check your IP camera connection.")
                     self.imgs[i] *= 0
                     cap.open(stream)  # re-open stream if signal was lost
             time.sleep(1 / self.fps[i])  # wait time
 
     def __iter__(self):
         self.count = -1
         return self
 
     def __next__(self):
         self.count += 1
-        if not all(x.is_alive() for x in self.threads) or cv2.waitKey(1) == ord(
-            "q"
-        ):  # q to quit
+        if not all(x.is_alive() for x in self.threads) or cv2.waitKey(1) == ord("q"):  # q to quit
             cv2.destroyAllWindows()
             raise StopIteration
 
         img0 = self.imgs.copy()
 
         # list
         return img0, self.sources, " "
@@ -122,79 +97,100 @@
             )
         self.vid_writer[i].write(image)
 
 
 class ReadOneStream:
     """Read one Stream, modified from yolov5, support one streams reading and saving."""
 
-    def __init__(self, source):
+    def __init__(self, source, vid_stride=1, imgsz=None, im_only=False):
+        """ReadOneStream
+
+        Args:
+            source (str): Source, could be a folder or a direct file.
+            vid_stride (int | optional): Video stride.
+            imgsz (tuple | optional): Image size, (height, width)
+            im_only (bool | optional): Whether to return image only, or it'll return
+                image, path and description.
+        """
         self.mode = "stream"
 
         self.vid_path, self.vid_writer = None, None
         self.fps, self.frames = 0, 0
-        self.source = clean_str(source)  # clean source names for later
+        self.source = source  # clean source names for later
+        self.vid_stride = vid_stride
+        self.imgsz = imgsz
+        self.im_only = im_only
 
         # Start thread to read frames from video stream
         print(f"{1}/{1}: {source}... ", end="")
-        if (
-            "youtube.com/" in source or "youtu.be/" in source
-        ):  # if source is YouTube video
-            check_requirements(("pafy", "youtube_dl"))
-            import pafy
-
-            source = pafy.new(source).getbest(preftype="mp4").url  # YouTube URL
-        source = (
-            eval(source) if source.isnumeric() else source
-        )  # i.e. s = '0' local webcam
+        source = eval(source) if source.isnumeric() else source  # i.e. s = '0' local webcam
         self.cap = cv2.VideoCapture(source)
         assert self.cap.isOpened(), f"Failed to open {source}"
         w = int(self.cap.get(cv2.CAP_PROP_FRAME_WIDTH))
         h = int(self.cap.get(cv2.CAP_PROP_FRAME_HEIGHT))
-        self.fps = (
-            max(self.cap.get(cv2.CAP_PROP_FPS) % 100, 0) or 30.0
-        )  # 30 FPS fallback
+        self.fps = max(self.cap.get(cv2.CAP_PROP_FPS) % 100, 0) or 30.0  # 30 FPS fallback
         self.frames = max(int(self.cap.get(cv2.CAP_PROP_FRAME_COUNT)), 0) or float(
             "inf"
         )  # infinite stream fallback
 
         print(f" success ({self.frames} frames {w}x{h} at {self.fps:.2f} FPS)")
         print("")  # newline
 
     def __iter__(self):
         self.count = -1
         return self
 
     def __next__(self):
-        self.count += 1
-        ret_val, img0 = self.cap.read()
-        if not ret_val or cv2.waitKey(1) == ord("q"):  # q to quit
+        for _ in range(self.vid_stride):
+            self.cap.grab()
+        success, img0 = self.cap.retrieve()
+        if not success or cv2.waitKey(1) == ord("q"):  # q to quit
             self.count += 1
             self.cap.release()
             cv2.destroyAllWindows()
             raise StopIteration
 
-        return img0, self.source, " "
+        if self.imgsz:
+            h, w = self.imgsz
+            img0 = cv2.resize(img0, (w, h))
+        return img0 if self.im_only else (img0, self.source, " ")
 
     def __len__(self):
         return 1
 
     def save(self, save_path, image):
+        """save video.
+
+        Args:
+            save_path (str): Save path, with suffix(`.avi`, `.mp4`) or not.
+            image (nd.ndarray): The image/frame.
+        """
+        save_path = f"{save_path}.mp4" if Path(save_path).suffix[1:] not in VID_FORMATS else save_path
         if self.vid_path != save_path:  # new video
             self.vid_path = save_path
-            fps, w, h = 30, image.shape[1], image.shape[0]
+            w, h = image.shape[1], image.shape[0]
             self.vid_writer = cv2.VideoWriter(
                 save_path, cv2.VideoWriter_fourcc(*"mp4v"), int(self.fps), (w, h)
             )
         self.vid_writer.write(image)
 
 
 class ReadVideosAndImages:
     """Read Videos and Images, modified from yolov5"""
 
-    def __init__(self, source: str):
+    def __init__(self, source: str, vid_stride=1, imgsz=None, im_only=False):
+        """ReadVideosAndImages
+
+        Args:
+            source (str): Source, could be a folder or a direct file.
+            vid_stride (int | optional): Video stride.
+            imgsz (tuple | optional): Image size, (height, width)
+            im_only (bool | optional): Whether to return image only, or it'll return
+                image, path and description.
+        """
         p = str(Path(source).resolve())  # os-agnostic absolute path
         if "*" in p:
             files = sorted(glob.glob(p, recursive=True))  # glob
         elif osp.isdir(p):
             files = sorted(glob.glob(osp.join(p, "*.*")))  # dir
         elif osp.isfile(p):
             files = [p]  # files
@@ -206,15 +202,18 @@
         videos = [x for x in files if x.split(".")[-1].lower() in VID_FORMATS]
         ni, nv = len(images), len(videos)
 
         self.vid_path, self.vid_writer = None, None
         self.files = images + videos
         self.nf = ni + nv  # number of files
         self.video_flag = [False] * ni + [True] * nv
+        self.vid_stride = vid_stride
         self.mode = "image"
+        self.imgsz = imgsz
+        self.im_only = im_only
         if any(videos):
             self.new_video(videos[0])  # new video
         else:
             self.cap = None
         assert self.nf > 0, (
             f"No images or videos found in {p}. "
             f"Supported formats are:\nimages: {IMG_FORMATS}\nvideos: {VID_FORMATS}"
@@ -228,55 +227,71 @@
         if self.count == self.nf:
             raise StopIteration
         path = self.files[self.count]
 
         if self.video_flag[self.count]:
             # Read video
             self.mode = "video"
-            ret_val, img0 = self.cap.read()
-            if not ret_val:
+            for _ in range(self.vid_stride):
+                self.cap.grab()
+            success, img0 = self.cap.retrieve()
+            if self.frame >= self.frames:
+            # if not success:
                 self.count += 1
                 self.cap.release()
                 if self.count == self.nf:  # last video
                     raise StopIteration
                 else:
                     path = self.files[self.count]
                     self.new_video(path)
-                    ret_val, img0 = self.cap.read()
+                    success, img0 = self.cap.read()
 
-            self.frame += 1
-            s = f"video {self.count + 1}/{self.nf} "
+            self.frame += self.vid_stride
+            s = f"video {self.count + 1}/{self.nf} {self.frame}/{self.frames}"
         else:
             # Read image
             self.count += 1
             img0 = cv2.imread(path)  # BGR
             assert img0 is not None, "Image Not Found " + path
             s = f"image {self.count}/{self.nf} "
 
-        return img0, path, s
+        if self.imgsz:
+            h, w = self.imgsz
+            img0 = cv2.resize(img0, (w, h))
+        return img0 if self.im_only else (img0, path, s)
 
     def new_video(self, path):
         self.frame = 0
         self.cap = cv2.VideoCapture(path)
         self.frames = int(self.cap.get(cv2.CAP_PROP_FRAME_COUNT))
+        try:
+            self.fps = int(self.cap.get(cv2.CAP_PROP_FPS))
+        except:
+            print("Warning: get inf fps, hand-coded it to 25.")
+            self.fps = 25
 
     def save(self, save_path, image):
+        """save image or video.
+
+        Args:
+            save_path (str): Save path, with suffix(`.jpg`, `.mp4`) or not.
+            image (nd.ndarray): The image/frame.
+        """
         if self.mode == "image":
+            save_path = f"{save_path}.jpg" if Path(save_path).suffix[1:] not in IMG_FORMATS else save_path
             cv2.imwrite(save_path, image)
         else:  # 'video' or 'stream'
+            save_path = f"{save_path}.mp4" if Path(save_path).suffix[1:] not in VID_FORMATS else save_path
             if self.vid_path != save_path:  # new video
                 self.vid_path = save_path
                 if isinstance(self.vid_writer, cv2.VideoWriter):
                     self.vid_writer.release()  # release previous video writer
-                fps = self.cap.get(cv2.CAP_PROP_FPS)
                 w = int(self.cap.get(cv2.CAP_PROP_FRAME_WIDTH))
                 h = int(self.cap.get(cv2.CAP_PROP_FRAME_HEIGHT))
-                self.vid_writer = cv2.VideoWriter(
-                    save_path, cv2.VideoWriter_fourcc(*"mp4v"), fps, (w, h)
-                )
+                self.vid_writer = cv2.VideoWriter(save_path, cv2.VideoWriter_fourcc(*"mp4v"), self.fps, (w, h))
             self.vid_writer.write(image)
 
     def __len__(self):
         return self.nf  # number of files
 
 
 def create_reader(source: str):
@@ -287,16 +302,7 @@
         reader(ReadVideosAndImages | ReadStreams): data reader.
         webcam(bool): the source is webcam or not.
     """
     is_file = Path(source).suffix[1:] in (IMG_FORMATS + VID_FORMATS)
     is_url = source.lower().startswith(("rtsp://", "rtmp://", "http://", "https://"))
     webcam = source.isnumeric() or source.endswith(".txt") or (is_url and not is_file)
     return ReadOneStream(source) if webcam else ReadVideosAndImages(source), webcam
-
-
-if __name__ == "__main__":
-    test = create_reader(source="/d/九江/playphone/20211223/imgs")
-    for img, p, s in test:
-        print(s, p)
-        cv2.imshow("p", img)
-        if cv2.waitKey(1) == ord("q"):
-            break
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `lqcv-0.1.0/lqcv/utils/timer.py` & `lqcv-0.2.0/lqcv/utils/timer.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,63 +1,59 @@
-# from mmcv
-from time import time
-from time import sleep
+# from time import time
+import time
 import torch
 import functools
 
 
 def time_sync():
     # pytorch-accurate time
     if torch.cuda.is_available():
         torch.cuda.synchronize()
-    return time()
+    return time.time()
 
 
 class TimerError(Exception):
     def __init__(self, message):
         self.message = message
         super(TimerError, self).__init__(message)
 
 
 class Timer:
     """A flexible Timer class.
 
     :Example:
 
     >>> import time
-    >>> import mmcv
-    >>> with mmcv.Timer():
+    >>> with Timer():
     >>>     # simulate a code block that will run for 1s
     >>>     time.sleep(1)
     1.000
-    >>> with mmcv.Timer(print_tmpl='it takes {:.1f} seconds'):
+    >>> with Timer(print_tmpl='it takes {:.1f} seconds'):
     >>>     # simulate a code block that will run for 1s
     >>>     time.sleep(1)
     it takes 1.0 seconds
-    >>> timer = mmcv.Timer()
+    >>> timer = Timer()
     >>> time.sleep(0.5)
     >>> print(timer.since_start())
     0.500
     >>> time.sleep(0.5)
     >>> print(timer.since_last_check())
     0.500
     >>> print(timer.since_start())
     1.000
     """
 
-    def __init__(
-        self, start=True, print_tmpl=None, cuda_sync=False, round=None, unit="s"
-    ):
-        assert unit in ['s', 'ms']
+    def __init__(self, start=True, print_tmpl=None, cuda_sync=False, round=None, unit="s"):
+        assert unit in ["s", "ms"]
         assert round is None or isinstance(round, int)
         self._is_running = False
         self.round = round
         self.unit = unit
         self.print_tmpl = print_tmpl if print_tmpl else "{:.3f}"
-        self.time = time_sync if cuda_sync else time
+        self.time = time_sync if cuda_sync else time.time
         if start:
             self.start()
 
     @property
     def is_running(self):
         """bool: indicate whether the timer is running"""
         return self._is_running
@@ -83,15 +79,15 @@
 
         Returns (float): Time in seconds.
         """
         if not self._is_running:
             raise TimerError("timer is not running")
         self._t_last = self.time()
         dur = self._t_last - self._t_start
-        if self.unit == 'ms':
+        if self.unit == "ms":
             dur = dur * 1000
         if self.round is not None:
             dur = round(dur, self.round)
         return dur
 
     def since_last_check(self):
         """Time since the last checking.
@@ -100,54 +96,22 @@
         operation.
 
         Returns (float): Time in seconds.
         """
         if not self._is_running:
             raise TimerError("timer is not running")
         dur = self.time() - self._t_last
-        if self.unit == 'ms':
+        if self.unit == "ms":
             dur = dur * 1000
         if self.round is not None:
             dur = round(dur, self.round)
         self._t_last = self.time()
         return dur
 
 
-_g_timers = {}  # global timers
-
-
-def check_time(timer_id):
-    """Add check points in a single line.
-
-    This method is suitable for running a task on a list of items. A timer will
-    be registered when the method is called for the first time.
-
-    :Example:
-
-    >>> import time
-    >>> import mmcv
-    >>> for i in range(1, 6):
-    >>>     # simulate a code block
-    >>>     time.sleep(i)
-    >>>     mmcv.check_time('task1')
-    2.000
-    3.000
-    4.000
-    5.000
-
-    Args:
-        timer_id (str): Timer identifier.
-    """
-    if timer_id not in _g_timers:
-        _g_timers[timer_id] = Timer()
-        return 0
-    else:
-        return _g_timers[timer_id].since_last_check()
-
-
 def timer(cuda_sync=False):
     def out_func(old_func):
         time = Timer(start=False, cuda_sync=cuda_sync)
 
         @functools.wraps(old_func)
         def new_func(*args, **kwargs):
             time.start()
@@ -157,13 +121,13 @@
 
         return new_func
 
     return out_func
 
 
 if __name__ == "__main__":
-    timer = Timer()
-    sleep(0.5)
+    timer = Timer(unit="ms", round=2)
+    time.sleep(0.5)
     print(timer.since_start())
-    sleep(0.5)
+    time.sleep(0.5)
     print(timer.since_last_check())
     print(timer.since_start())
```

### Comparing `lqcv-0.1.0/lqcv.egg-info/PKG-INFO` & `lqcv-0.2.0/lqcv.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lqcv
-Version: 0.1.0
+Version: 0.2.0
 Author: Laughing-q
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 
 # lqcv
 This is my computer vision lib.
```

### Comparing `lqcv-0.1.0/setup.py` & `lqcv-0.2.0/setup.py`

 * *Files identical despite different names*

