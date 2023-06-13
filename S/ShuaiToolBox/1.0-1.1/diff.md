# Comparing `tmp/ShuaiToolBox-1.0.tar.gz` & `tmp/ShuaiToolBox-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ShuaiToolBox-1.0.tar", last modified: Tue Jun 13 06:27:34 2023, max compression
+gzip compressed data, was "dist\ShuaiToolBox-1.1.tar", last modified: Tue Jun 13 07:08:09 2023, max compression
```

## Comparing `ShuaiToolBox-1.0.tar` & `ShuaiToolBox-1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 06:27:34.000000 ShuaiToolBox-1.0/
--rw-rw-rw-   0        0        0      197 2023-06-13 06:27:34.000000 ShuaiToolBox-1.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-06-13 06:20:27.000000 ShuaiToolBox-1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-13 06:27:34.000000 ShuaiToolBox-1.0/ShuaiToolBox/
--rw-rw-rw-   0        0        0     2617 2021-09-13 13:48:20.000000 ShuaiToolBox-1.0/ShuaiToolBox/FindContours.py
--rw-rw-rw-   0        0        0    13831 2022-07-07 04:05:08.000000 ShuaiToolBox-1.0/ShuaiToolBox/VideoPro.py
--rw-rw-rw-   0        0        0     8060 2023-06-13 06:04:27.000000 ShuaiToolBox-1.0/ShuaiToolBox/VideoProList.py
--rw-rw-rw-   0        0        0       41 2023-06-13 06:20:12.000000 ShuaiToolBox-1.0/ShuaiToolBox/__init__.py
--rw-rw-rw-   0        0        0     1028 2022-12-21 14:44:22.000000 ShuaiToolBox-1.0/ShuaiToolBox/cv_plugin.py
--rw-rw-rw-   0        0        0     2136 2021-08-31 08:12:37.000000 ShuaiToolBox-1.0/ShuaiToolBox/cv_vdopro.py
--rw-rw-rw-   0        0        0     7798 2023-06-13 03:55:53.000000 ShuaiToolBox-1.0/ShuaiToolBox/opencv Functions.py
--rw-rw-rw-   0        0        0     1635 2023-06-13 05:48:13.000000 ShuaiToolBox-1.0/ShuaiToolBox/py_plugin.py
-drwxrwxrwx   0        0        0        0 2023-06-13 06:27:34.000000 ShuaiToolBox-1.0/ShuaiToolBox.egg-info/
--rw-rw-rw-   0        0        0      197 2023-06-13 06:27:34.000000 ShuaiToolBox-1.0/ShuaiToolBox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      381 2023-06-13 06:27:34.000000 ShuaiToolBox-1.0/ShuaiToolBox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 06:27:34.000000 ShuaiToolBox-1.0/ShuaiToolBox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-06-13 06:27:34.000000 ShuaiToolBox-1.0/ShuaiToolBox.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-13 06:27:34.000000 ShuaiToolBox-1.0/setup.cfg
--rw-rw-rw-   0        0        0      238 2023-06-13 06:24:27.000000 ShuaiToolBox-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 07:08:09.000000 ShuaiToolBox-1.1/
+-rw-rw-rw-   0        0        0      197 2023-06-13 07:08:09.000000 ShuaiToolBox-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-06-13 06:20:27.000000 ShuaiToolBox-1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-13 07:08:09.000000 ShuaiToolBox-1.1/ShuaiToolBox/
+-rw-rw-rw-   0        0        0     2617 2021-09-13 13:48:20.000000 ShuaiToolBox-1.1/ShuaiToolBox/FindContours.py
+-rw-rw-rw-   0        0        0    13825 2023-06-13 07:05:00.000000 ShuaiToolBox-1.1/ShuaiToolBox/VideoPro.py
+-rw-rw-rw-   0        0        0     8052 2023-06-13 07:04:46.000000 ShuaiToolBox-1.1/ShuaiToolBox/VideoProList.py
+-rw-rw-rw-   0        0        0      156 2023-06-13 07:05:22.000000 ShuaiToolBox-1.1/ShuaiToolBox/__init__.py
+-rw-rw-rw-   0        0        0     1028 2022-12-21 14:44:22.000000 ShuaiToolBox-1.1/ShuaiToolBox/cv_plugin.py
+-rw-rw-rw-   0        0        0     2136 2021-08-31 08:12:37.000000 ShuaiToolBox-1.1/ShuaiToolBox/cv_vdopro.py
+-rw-rw-rw-   0        0        0     7798 2023-06-13 03:55:53.000000 ShuaiToolBox-1.1/ShuaiToolBox/opencv_Functions.py
+-rw-rw-rw-   0        0        0     1635 2023-06-13 05:48:13.000000 ShuaiToolBox-1.1/ShuaiToolBox/py_plugin.py
+drwxrwxrwx   0        0        0        0 2023-06-13 07:08:09.000000 ShuaiToolBox-1.1/ShuaiToolBox.egg-info/
+-rw-rw-rw-   0        0        0      197 2023-06-13 07:08:09.000000 ShuaiToolBox-1.1/ShuaiToolBox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      381 2023-06-13 07:08:09.000000 ShuaiToolBox-1.1/ShuaiToolBox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 07:08:09.000000 ShuaiToolBox-1.1/ShuaiToolBox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-06-13 07:08:09.000000 ShuaiToolBox-1.1/ShuaiToolBox.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-13 07:08:09.000000 ShuaiToolBox-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      238 2023-06-13 07:05:29.000000 ShuaiToolBox-1.1/setup.py
```

### Comparing `ShuaiToolBox-1.0/ShuaiToolBox/FindContours.py` & `ShuaiToolBox-1.1/ShuaiToolBox/FindContours.py`

 * *Files identical despite different names*

### Comparing `ShuaiToolBox-1.0/ShuaiToolBox/VideoPro.py` & `ShuaiToolBox-1.1/ShuaiToolBox/VideoPro.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import multiprocessing as mp
 
 from cv_plugin import *
 from cv_vdopro import *
 from FindContours import *
 import numpy as np
-cvFun = __import__("opencv Functions")
+import opencv_Functions as cvFun
 
 # 根据颜色上下限对图像进行二值化处理
 def color_seperate(image, lower_hsv, upper_hsv):
     hsv = cv2.cvtColor(image, cv2.COLOR_BGR2HSV)  # 对目标图像进行色彩空间转换
     # 依据设定的上下限对目标图像进行二值化转换,在区间内的为1，不在区间内的为0
     mask = cv2.inRange(hsv, lowerb=lower_hsv, upperb=upper_hsv)
     # dst = cv.bitwise_and(image, image, mask=mask)    #将二值化图像与原图进行“与”操作；实际是提取前两个frame 的“与”结果，然后输出mask 为1的部分
```

### Comparing `ShuaiToolBox-1.0/ShuaiToolBox/VideoProList.py` & `ShuaiToolBox-1.1/ShuaiToolBox/VideoProList.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import sys,os
 sys.path.append(r"D:\OneDrive - pku.edu.cn\000 Doing\DataFlux")
 
 import cv2
 import paddlehub as hub
 from VideoPro import *
 import imageio
-
-cvFun = __import__("opencv Functions")
+import opencv_Functions as cvFun
 
 class process():
     def __init__(self,_path,_videos,_Times,_Cliplist):
         self.path=_path
         self.videos=_videos
         self.Times=_Times
         self.Cliplist=_Cliplist
```

### Comparing `ShuaiToolBox-1.0/ShuaiToolBox/cv_plugin.py` & `ShuaiToolBox-1.1/ShuaiToolBox/cv_plugin.py`

 * *Files identical despite different names*

### Comparing `ShuaiToolBox-1.0/ShuaiToolBox/cv_vdopro.py` & `ShuaiToolBox-1.1/ShuaiToolBox/cv_vdopro.py`

 * *Files identical despite different names*

### Comparing `ShuaiToolBox-1.0/ShuaiToolBox/opencv Functions.py` & `ShuaiToolBox-1.1/ShuaiToolBox/opencv_Functions.py`

 * *Files identical despite different names*

### Comparing `ShuaiToolBox-1.0/ShuaiToolBox/py_plugin.py` & `ShuaiToolBox-1.1/ShuaiToolBox/py_plugin.py`

 * *Files identical despite different names*

