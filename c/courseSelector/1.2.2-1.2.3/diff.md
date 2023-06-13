# Comparing `tmp/courseSelector-1.2.2.tar.gz` & `tmp/courseSelector-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "courseSelector-1.2.2.tar", last modified: Tue Jan 10 15:26:15 2023, max compression
+gzip compressed data, was "courseSelector-1.2.3.tar", last modified: Tue Jun 13 07:54:40 2023, max compression
```

## Comparing `courseSelector-1.2.2.tar` & `courseSelector-1.2.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 jtc        (501) staff       (20)        0 2023-01-10 15:26:15.176614 courseSelector-1.2.2/
--rwxrwxrwx   0 jtc        (501) staff       (20)    18092 2022-05-15 16:29:48.000000 courseSelector-1.2.2/LICENSE
--rw-r--r--   0 jtc        (501) staff       (20)      319 2023-01-10 15:26:15.176500 courseSelector-1.2.2/PKG-INFO
--rwxrwxrwx   0 jtc        (501) staff       (20)     2737 2022-09-04 08:26:24.000000 courseSelector-1.2.2/README.md
-drwxr-xr-x   0 jtc        (501) staff       (20)        0 2023-01-10 15:26:15.175663 courseSelector-1.2.2/courseSelector/
--rw-r--r--   0 jtc        (501) staff       (20)      700 2023-01-10 15:24:49.000000 courseSelector-1.2.2/courseSelector/__init__.py
--rw-r--r--   0 jtc        (501) staff       (20)     9480 2023-01-10 15:25:19.000000 courseSelector-1.2.2/courseSelector/functions.py
--rw-r--r--   0 jtc        (501) staff       (20)     8616 2023-01-10 15:25:35.000000 courseSelector-1.2.2/courseSelector/globalVariable.py
--rw-r--r--   0 jtc        (501) staff       (20)     8548 2022-08-10 12:13:02.000000 courseSelector-1.2.2/courseSelector/login.py
--rw-r--r--   0 jtc        (501) staff       (20)     8149 2023-01-10 15:25:48.000000 courseSelector-1.2.2/courseSelector/main.py
--rw-r--r--   0 jtc        (501) staff       (20)     4772 2022-08-10 12:13:02.000000 courseSelector-1.2.2/courseSelector/myHttp.py
-drwxr-xr-x   0 jtc        (501) staff       (20)        0 2023-01-10 15:26:15.176343 courseSelector-1.2.2/courseSelector.egg-info/
--rwxrwxrwx   0 jtc        (501) staff       (20)      319 2023-01-10 15:26:14.000000 courseSelector-1.2.2/courseSelector.egg-info/PKG-INFO
--rwxrwxrwx   0 jtc        (501) staff       (20)      375 2023-01-10 15:26:15.000000 courseSelector-1.2.2/courseSelector.egg-info/SOURCES.txt
--rwxrwxrwx   0 jtc        (501) staff       (20)        1 2023-01-10 15:26:14.000000 courseSelector-1.2.2/courseSelector.egg-info/dependency_links.txt
--rwxrwxrwx   0 jtc        (501) staff       (20)       76 2023-01-10 15:26:15.000000 courseSelector-1.2.2/courseSelector.egg-info/requires.txt
--rwxrwxrwx   0 jtc        (501) staff       (20)       15 2023-01-10 15:26:15.000000 courseSelector-1.2.2/courseSelector.egg-info/top_level.txt
--rw-r--r--   0 jtc        (501) staff       (20)       38 2023-01-10 15:26:15.176654 courseSelector-1.2.2/setup.cfg
--rwxrwxrwx   0 jtc        (501) staff       (20)      507 2023-01-10 15:24:36.000000 courseSelector-1.2.2/setup.py
+drwxr-xr-x   0 jtc        (501) staff       (20)        0 2023-06-13 07:54:40.978089 courseSelector-1.2.3/
+-rwxrwxrwx   0 jtc        (501) staff       (20)    18092 2022-05-15 16:29:48.000000 courseSelector-1.2.3/LICENSE
+-rw-r--r--   0 jtc        (501) staff       (20)      319 2023-06-13 07:54:40.977977 courseSelector-1.2.3/PKG-INFO
+-rwxrwxrwx   0 jtc        (501) staff       (20)     2737 2022-09-04 08:26:24.000000 courseSelector-1.2.3/README.md
+drwxr-xr-x   0 jtc        (501) staff       (20)        0 2023-06-13 07:54:40.977152 courseSelector-1.2.3/courseSelector/
+-rw-r--r--   0 jtc        (501) staff       (20)      700 2023-06-13 07:52:36.000000 courseSelector-1.2.3/courseSelector/__init__.py
+-rw-r--r--   0 jtc        (501) staff       (20)     9539 2023-06-13 07:53:39.000000 courseSelector-1.2.3/courseSelector/functions.py
+-rw-r--r--   0 jtc        (501) staff       (20)     8616 2023-01-10 15:25:35.000000 courseSelector-1.2.3/courseSelector/globalVariable.py
+-rw-r--r--   0 jtc        (501) staff       (20)     8548 2022-08-10 12:13:02.000000 courseSelector-1.2.3/courseSelector/login.py
+-rw-r--r--   0 jtc        (501) staff       (20)     8149 2023-01-10 15:25:48.000000 courseSelector-1.2.3/courseSelector/main.py
+-rw-r--r--   0 jtc        (501) staff       (20)     4772 2022-08-10 12:13:02.000000 courseSelector-1.2.3/courseSelector/myHttp.py
+drwxr-xr-x   0 jtc        (501) staff       (20)        0 2023-06-13 07:54:40.977808 courseSelector-1.2.3/courseSelector.egg-info/
+-rwxrwxrwx   0 jtc        (501) staff       (20)      319 2023-06-13 07:54:40.000000 courseSelector-1.2.3/courseSelector.egg-info/PKG-INFO
+-rwxrwxrwx   0 jtc        (501) staff       (20)      375 2023-06-13 07:54:40.000000 courseSelector-1.2.3/courseSelector.egg-info/SOURCES.txt
+-rwxrwxrwx   0 jtc        (501) staff       (20)        1 2023-06-13 07:54:40.000000 courseSelector-1.2.3/courseSelector.egg-info/dependency_links.txt
+-rwxrwxrwx   0 jtc        (501) staff       (20)       76 2023-06-13 07:54:40.000000 courseSelector-1.2.3/courseSelector.egg-info/requires.txt
+-rwxrwxrwx   0 jtc        (501) staff       (20)       15 2023-06-13 07:54:40.000000 courseSelector-1.2.3/courseSelector.egg-info/top_level.txt
+-rw-r--r--   0 jtc        (501) staff       (20)       38 2023-06-13 07:54:40.978132 courseSelector-1.2.3/setup.cfg
+-rwxrwxrwx   0 jtc        (501) staff       (20)      507 2023-06-13 07:53:57.000000 courseSelector-1.2.3/setup.py
```

### Comparing `courseSelector-1.2.2/LICENSE` & `courseSelector-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `courseSelector-1.2.2/README.md` & `courseSelector-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `courseSelector-1.2.2/courseSelector/__init__.py` & `courseSelector-1.2.3/courseSelector/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     'printCourseList_byJaccount',
     'waitEmptySpace_byJaccount',
     'fastSelect_byJaccount',
     'luckyDraw_byJaccount'
 ]
 
 
-__version__='1.2.2'
+__version__='1.2.3'
 __license__='GPL-2.0 License'
 __author__='Tiancheng Jiao'
 __url__='https://github.com/jtc1246/courseSelector'
 __author_email__='jtc1246@outlook.com'
 __description__='An automatic course selection program for SJTU-JI'
```

### Comparing `courseSelector-1.2.2/courseSelector/functions.py` & `courseSelector-1.2.3/courseSelector/functions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from .globalVariable import *
 import time,json
 from copy import deepcopy
 from .myHttp import *
 import os
 from time import sleep
+from random import randint
 
 # 格式:
 # {"electTurnId":"158C59EB-C733-4C3A-8E78-C314DCEC70BF","autoElect":true,"lessonTasks":["A57528CC-AECA-4266-874E-039386315A2A"]}
 def getJsonString(electTurnId,electTurnLessonTaskId):
     return '{"electTurnId":"'+electTurnId+'","autoElect":true,"lessonTasks":["'+electTurnLessonTaskId+'"]}'
 
 
@@ -234,14 +235,15 @@
         t=getAllInformation()
         if(t==-1):
             addGlobalVariable('failTimes')
             continue
         setGlobalValue('allInfo',t)
         setGlobalValue('newMsg',True)
         setGlobalValue('failTimes',0)
+        sleep(randint(5,8)/100)
 
 
 
 
 def mainControl():
     while True:
         if(not getGlobalValue('newMsg')):
```

### Comparing `courseSelector-1.2.2/courseSelector/globalVariable.py` & `courseSelector-1.2.3/courseSelector/globalVariable.py`

 * *Files identical despite different names*

### Comparing `courseSelector-1.2.2/courseSelector/login.py` & `courseSelector-1.2.3/courseSelector/login.py`

 * *Files identical despite different names*

### Comparing `courseSelector-1.2.2/courseSelector/main.py` & `courseSelector-1.2.3/courseSelector/main.py`

 * *Files identical despite different names*

### Comparing `courseSelector-1.2.2/courseSelector/myHttp.py` & `courseSelector-1.2.3/courseSelector/myHttp.py`

 * *Files identical despite different names*

