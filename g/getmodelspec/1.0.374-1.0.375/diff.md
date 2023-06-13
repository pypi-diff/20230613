# Comparing `tmp/getmodelspec-1.0.374.tar.gz` & `tmp/getmodelspec-1.0.375.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\getmodelspec-1.0.374.tar", last modified: Tue Jun 13 15:27:31 2023, max compression
+gzip compressed data, was "dist\getmodelspec-1.0.375.tar", last modified: Tue Jun 13 15:34:00 2023, max compression
```

## Comparing `getmodelspec-1.0.374.tar` & `getmodelspec-1.0.375.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 15:27:31.000000 getmodelspec-1.0.374/
--rw-rw-rw-   0        0        0      351 2023-06-13 15:27:31.000000 getmodelspec-1.0.374/PKG-INFO
--rw-rw-rw-   0        0        0     3796 2023-06-12 13:29:40.000000 getmodelspec-1.0.374/README.md
-drwxrwxrwx   0        0        0        0 2023-06-13 15:27:31.000000 getmodelspec-1.0.374/getmodelspec/
--rw-rw-rw-   0        0        0      253 2023-06-12 12:36:25.000000 getmodelspec-1.0.374/getmodelspec/__init__.py
--rw-rw-rw-   0        0        0      531 2023-06-11 16:18:57.000000 getmodelspec-1.0.374/getmodelspec/lineup.py
-drwxrwxrwx   0        0        0        0 2023-06-13 15:27:31.000000 getmodelspec-1.0.374/getmodelspec/src/
--rw-rw-rw-   0        0        0        0 2023-06-05 07:20:11.000000 getmodelspec-1.0.374/getmodelspec/src/__init__.py
--rw-rw-rw-   0        0        0     7507 2023-06-13 15:21:27.000000 getmodelspec-1.0.374/getmodelspec/src/panasonic.py
--rw-rw-rw-   0        0        0    23230 2023-06-13 10:21:02.000000 getmodelspec-1.0.374/getmodelspec/src/sony.py
--rw-rw-rw-   0        0        0      935 2023-06-13 15:13:47.000000 getmodelspec-1.0.374/getmodelspec/src/teast1.py
--rw-rw-rw-   0        0        0     5284 2023-06-13 15:19:37.000000 getmodelspec-1.0.374/getmodelspec/src/test.py
--rw-rw-rw-   0        0        0     1817 2023-06-12 11:30:21.000000 getmodelspec-1.0.374/getmodelspec/src/tv_score.py
--rw-rw-rw-   0        0        0     4277 2023-06-10 11:21:39.000000 getmodelspec-1.0.374/getmodelspec/src/tv_spepcifications.py
-drwxrwxrwx   0        0        0        0 2023-06-13 15:27:31.000000 getmodelspec-1.0.374/getmodelspec/tools/
--rw-rw-rw-   0        0        0        0 2023-06-05 07:20:04.000000 getmodelspec-1.0.374/getmodelspec/tools/__init__.py
--rw-rw-rw-   0        0        0     2512 2023-06-13 15:09:07.000000 getmodelspec-1.0.374/getmodelspec/tools/functions.py
--rw-rw-rw-   0        0        0     5038 2023-06-10 06:31:05.000000 getmodelspec-1.0.374/getmodelspec/tools/webdriver.py
-drwxrwxrwx   0        0        0        0 2023-06-13 15:27:31.000000 getmodelspec-1.0.374/getmodelspec.egg-info/
--rw-rw-rw-   0        0        0      351 2023-06-13 15:27:30.000000 getmodelspec-1.0.374/getmodelspec.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      583 2023-06-13 15:27:31.000000 getmodelspec-1.0.374/getmodelspec.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 15:27:30.000000 getmodelspec-1.0.374/getmodelspec.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-06-13 15:27:30.000000 getmodelspec-1.0.374/getmodelspec.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       26 2023-06-13 15:27:30.000000 getmodelspec-1.0.374/getmodelspec.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-13 15:27:30.000000 getmodelspec-1.0.374/getmodelspec.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-13 15:27:31.000000 getmodelspec-1.0.374/setup.cfg
--rw-rw-rw-   0        0        0      811 2023-06-13 15:27:27.000000 getmodelspec-1.0.374/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 15:34:00.000000 getmodelspec-1.0.375/
+-rw-rw-rw-   0        0        0      351 2023-06-13 15:34:00.000000 getmodelspec-1.0.375/PKG-INFO
+-rw-rw-rw-   0        0        0     3785 2023-06-13 15:33:43.000000 getmodelspec-1.0.375/README.md
+drwxrwxrwx   0        0        0        0 2023-06-13 15:34:00.000000 getmodelspec-1.0.375/getmodelspec/
+-rw-rw-rw-   0        0        0      253 2023-06-12 12:36:25.000000 getmodelspec-1.0.375/getmodelspec/__init__.py
+-rw-rw-rw-   0        0        0      778 2023-06-13 15:30:10.000000 getmodelspec-1.0.375/getmodelspec/lineup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 15:34:00.000000 getmodelspec-1.0.375/getmodelspec/src/
+-rw-rw-rw-   0        0        0        0 2023-06-05 07:20:11.000000 getmodelspec-1.0.375/getmodelspec/src/__init__.py
+-rw-rw-rw-   0        0        0     7328 2023-06-13 15:28:52.000000 getmodelspec-1.0.375/getmodelspec/src/panasonic.py
+-rw-rw-rw-   0        0        0    23230 2023-06-13 10:21:02.000000 getmodelspec-1.0.375/getmodelspec/src/sony.py
+-rw-rw-rw-   0        0        0      935 2023-06-13 15:13:47.000000 getmodelspec-1.0.375/getmodelspec/src/teast1.py
+-rw-rw-rw-   0        0        0     5284 2023-06-13 15:19:37.000000 getmodelspec-1.0.375/getmodelspec/src/test.py
+-rw-rw-rw-   0        0        0     1817 2023-06-12 11:30:21.000000 getmodelspec-1.0.375/getmodelspec/src/tv_score.py
+-rw-rw-rw-   0        0        0     4277 2023-06-10 11:21:39.000000 getmodelspec-1.0.375/getmodelspec/src/tv_spepcifications.py
+drwxrwxrwx   0        0        0        0 2023-06-13 15:34:00.000000 getmodelspec-1.0.375/getmodelspec/tools/
+-rw-rw-rw-   0        0        0        0 2023-06-05 07:20:04.000000 getmodelspec-1.0.375/getmodelspec/tools/__init__.py
+-rw-rw-rw-   0        0        0     2512 2023-06-13 15:09:07.000000 getmodelspec-1.0.375/getmodelspec/tools/functions.py
+-rw-rw-rw-   0        0        0     5038 2023-06-10 06:31:05.000000 getmodelspec-1.0.375/getmodelspec/tools/webdriver.py
+drwxrwxrwx   0        0        0        0 2023-06-13 15:34:00.000000 getmodelspec-1.0.375/getmodelspec.egg-info/
+-rw-rw-rw-   0        0        0      351 2023-06-13 15:34:00.000000 getmodelspec-1.0.375/getmodelspec.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      583 2023-06-13 15:34:00.000000 getmodelspec-1.0.375/getmodelspec.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 15:34:00.000000 getmodelspec-1.0.375/getmodelspec.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-06-13 15:34:00.000000 getmodelspec-1.0.375/getmodelspec.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       26 2023-06-13 15:34:00.000000 getmodelspec-1.0.375/getmodelspec.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-13 15:34:00.000000 getmodelspec-1.0.375/getmodelspec.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-13 15:34:00.000000 getmodelspec-1.0.375/setup.cfg
+-rw-rw-rw-   0        0        0      811 2023-06-13 15:33:31.000000 getmodelspec-1.0.375/setup.py
```

### Comparing `getmodelspec-1.0.374/README.md` & `getmodelspec-1.0.375/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 ## 사용법
 ### 1. 필요한 라이브러리 설치
 ```bash
 pip install selenium pandas openpyxl
 ```
 ### 2. lineup 모듈 임포트
 ```python
-from getmodelspec.src.lineup import LineUp
+from getmodelspec import LineUp
 ```
 ### 3. LineUp 클래스 인스턴스 생성
 ```python
 lineup = LineUp()
 ```
 ### 4-1. 사이트에서 제품 정보 가져오기
 ```python
```

### Comparing `getmodelspec-1.0.374/getmodelspec/lineup.py` & `getmodelspec-1.0.375/getmodelspec/lineup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from getmodelspec.src.sony import GetSONY,  GetSONYjp
-
+from getmodelspec.src.panasonic import GetPanajp
 class LineUp:
 
     def __init__(self):
 
         pass
     def getSony(self, src="jp", fastMode: bool = True,  toExcel: bool = True) -> None:
         """
@@ -12,13 +12,22 @@
         """
 
         if src == "global":
             sony = GetSONY(fastMode=fastMode, toExcel=toExcel)
         elif "jp":
             sony = GetSONYjp(toExcel=toExcel)
 
-        dfModels = sony.getModels()
-        return dfModels
+        dictModels = sony.getModels()
+        return dictModels
+
+    def getPana(self, toExcel: bool = True) -> None:
+        """
+
+        """
+        pana = GetPanajp(toExcel=toExcel)
+
+        dictModels = pana.getModels()
+        return dictModels
```

### Comparing `getmodelspec-1.0.374/getmodelspec/src/panasonic.py` & `getmodelspec-1.0.375/getmodelspec/src/panasonic.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,14 @@
 
 from bs4 import BeautifulSoup
 from datetime import date
-import requests
 from tqdm import tqdm
 import traceback
 from collections import OrderedDict
 
-from selenium.webdriver.common.keys import Keys
-from selenium.webdriver.common.by import By
-from selenium.webdriver.common.action_chains import ActionChains
-
 from getmodelspec.src.tv_spepcifications import Specifications
 from getmodelspec.src.tv_score import Score
 from getmodelspec.tools.functions import *
 from getmodelspec.tools.webdriver import WebDriver
 
 class GetPanajp:
     def __init__(self,  toExcel=True):
```

### Comparing `getmodelspec-1.0.374/getmodelspec/src/sony.py` & `getmodelspec-1.0.375/getmodelspec/src/sony.py`

 * *Files identical despite different names*

### Comparing `getmodelspec-1.0.374/getmodelspec/src/teast1.py` & `getmodelspec-1.0.375/getmodelspec/src/teast1.py`

 * *Files identical despite different names*

### Comparing `getmodelspec-1.0.374/getmodelspec/src/test.py` & `getmodelspec-1.0.375/getmodelspec/src/test.py`

 * *Files identical despite different names*

### Comparing `getmodelspec-1.0.374/getmodelspec/src/tv_score.py` & `getmodelspec-1.0.375/getmodelspec/src/tv_score.py`

 * *Files identical despite different names*

### Comparing `getmodelspec-1.0.374/getmodelspec/src/tv_spepcifications.py` & `getmodelspec-1.0.375/getmodelspec/src/tv_spepcifications.py`

 * *Files identical despite different names*

### Comparing `getmodelspec-1.0.374/getmodelspec/tools/functions.py` & `getmodelspec-1.0.375/getmodelspec/tools/functions.py`

 * *Files identical despite different names*

### Comparing `getmodelspec-1.0.374/getmodelspec/tools/webdriver.py` & `getmodelspec-1.0.375/getmodelspec/tools/webdriver.py`

 * *Files identical despite different names*

### Comparing `getmodelspec-1.0.374/getmodelspec.egg-info/SOURCES.txt` & `getmodelspec-1.0.375/getmodelspec.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `getmodelspec-1.0.374/setup.py` & `getmodelspec-1.0.375/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='getmodelspec',
-    version='1.0.374',
+    version='1.0.375',
     author='xikest',
     description='get model spec,',
     packages=find_packages(),
     python_requires='>=3.7',
     install_requires=[
         'numpy',
         'pandas',
```

