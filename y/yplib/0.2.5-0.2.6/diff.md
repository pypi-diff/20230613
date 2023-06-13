# Comparing `tmp/yplib-0.2.5.tar.gz` & `tmp/yplib-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-0.2.5.tar", last modified: Mon Jun 12 09:00:51 2023, max compression
+gzip compressed data, was "dist\yplib-0.2.6.tar", last modified: Tue Jun 13 00:30:38 2023, max compression
```

## Comparing `yplib-0.2.5.tar` & `yplib-0.2.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 09:00:51.408081 yplib-0.2.5/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-0.2.5/LICENSE
--rw-rw-rw-   0        0        0      567 2023-06-12 09:00:51.407904 yplib-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0      178 2023-06-08 01:05:32.000000 yplib-0.2.5/README.md
--rw-rw-rw-   0        0        0       42 2023-06-12 09:00:51.408689 yplib-0.2.5/setup.cfg
--rw-rw-rw-   0        0        0      561 2023-06-12 09:00:39.000000 yplib-0.2.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-12 09:00:51.404835 yplib-0.2.5/yplib/
--rw-rw-rw-   0        0        0    15370 2023-06-12 07:49:32.000000 yplib-0.2.5/yplib/__init__.py
--rw-rw-rw-   0        0        0     2609 2023-06-09 02:24:26.000000 yplib-0.2.5/yplib/line_stack_temp.py
-drwxrwxrwx   0        0        0        0 2023-06-12 09:00:51.407140 yplib-0.2.5/yplib.egg-info/
--rw-rw-rw-   0        0        0      567 2023-06-12 09:00:51.000000 yplib-0.2.5/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      185 2023-06-12 09:00:51.000000 yplib-0.2.5/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 09:00:51.000000 yplib-0.2.5/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-12 09:00:51.000000 yplib-0.2.5/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-13 00:30:38.957977 yplib-0.2.6/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-0.2.6/LICENSE
+-rw-rw-rw-   0        0        0      567 2023-06-13 00:30:38.957977 yplib-0.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0      178 2023-06-08 01:05:32.000000 yplib-0.2.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-13 00:30:38.957977 yplib-0.2.6/setup.cfg
+-rw-rw-rw-   0        0        0      561 2023-06-13 00:30:19.000000 yplib-0.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 00:30:38.954763 yplib-0.2.6/yplib/
+-rw-rw-rw-   0        0        0    15573 2023-06-13 00:29:50.000000 yplib-0.2.6/yplib/__init__.py
+-rw-rw-rw-   0        0        0     2609 2023-06-09 02:24:26.000000 yplib-0.2.6/yplib/line_stack_temp.py
+drwxrwxrwx   0        0        0        0 2023-06-13 00:30:38.957343 yplib-0.2.6/yplib.egg-info/
+-rw-rw-rw-   0        0        0      567 2023-06-13 00:30:38.000000 yplib-0.2.6/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      185 2023-06-13 00:30:38.000000 yplib-0.2.6/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 00:30:38.000000 yplib-0.2.6/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-13 00:30:38.000000 yplib-0.2.6/yplib.egg-info/top_level.txt
```

### Comparing `yplib-0.2.5/LICENSE` & `yplib-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-0.2.5/PKG-INFO` & `yplib-0.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yplib
-Version: 0.2.5
+Version: 0.2.6
 Summary: util
 Home-page: https://github.com/pypa/sampleproject
 Author: yangpu
 Author-email: wantwaterfish@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `yplib-0.2.5/setup.py` & `yplib-0.2.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="0.2.5",
+  version="0.2.6",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/pypa/sampleproject",
   packages=setuptools.find_packages(),
```

### Comparing `yplib-0.2.5/yplib/__init__.py` & `yplib-0.2.6/yplib/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # name = "yplib"
 
 import json
 import os
 import uuid
 from datetime import datetime
+from datetime import timedelta
 
 import xlrd
 import xlwt
 import time
 import re
 # import random
 import hashlib
@@ -163,41 +164,48 @@
 
 
 def to_datetime(s=None, return_str=False):
     if s is None or s == '':
         return datetime.today()
     s = str(s)
     r = datetime.today()
-    if re.match("^\\d{4}$", s):
-        r = datetime.strptime(s, "%Y")
-    if re.match("^\\d{4}-\\d{1,2}$", s):
-        r = datetime.strptime(s, "%Y-%m")
-    if re.match("^\\d{4}-\\d{1,2}-\\d{1,2}$", s):
-        r = datetime.strptime(s, "%Y-%m-%d")
-    if re.match("^\\d{4}-\\d{1,2}-\\d{1,2} {1}\\d{1,2}$", s):
-        r = datetime.strptime(s, "%Y-%m-%d %H")
-    if re.match("^\\d{4}-\\d{1,2}-\\d{1,2} {1}\\d{1,2}:\\d{1,2}$", s):
-        r = datetime.strptime(s, "%Y-%m-%d %H:%M")
-    if re.match("^\\d{4}-\\d{1,2}-\\d{1,2} {1}\\d{1,2}:\\d{1,2}:\\d{1,2}$", s):
-        r = datetime.strptime(s, "%Y-%m-%d %H:%M:%S")
-    if re.match("^\\d{4}-\\d{1,2}-\\d{1,2} {1}\\d{1,2}:\\d{1,2}:\\d{1,2}.\\d{1,9}$", s):
-        r = datetime.strptime(s.split('.')[0], "%Y-%m-%d %H:%M:%S")
+    m_s = {
+        "^\\d{4}$": "%Y",
+        "^\\d{4}-\\d{1,2}$": "%Y-%m",
+        "^\\d{4}-\\d{1,2}-\\d{1,2}$": "%Y-%m-%d",
+        "^\\d{4}-\\d{1,2}-\\d{1,2} {1}\\d{1,2}$": "%Y-%m-%d %H",
+        "^\\d{4}-\\d{1,2}-\\d{1,2} {1}\\d{1,2}:\\d{1,2}$": "%Y-%m-%d %H:%M",
+        "^\\d{4}-\\d{1,2}-\\d{1,2} {1}\\d{1,2}:\\d{1,2}:\\d{1,2}$": "%Y-%m-%d %H:%M:%S",
+        "^\\d{4}-\\d{1,2}-\\d{1,2} {1}\\d{1,2}:\\d{1,2}:\\d{1,2}.\\d{1,9}$": "%Y-%m-%d %H:%M:%S",
+    }
+    for m in m_s:
+        if re.match(m, s):
+            r = datetime.strptime(s.split('.')[0], m_s[m])
     if re.match("^\\d{1,13}$", s):
         s_int = int(s)
         if len(s) > 10:
             s_int = int(s_int / 1000)
         time_arr = time.localtime(s_int)
         time_str = time.strftime("%Y-%m-%d %H:%M:%S", time_arr)
         r = datetime.strptime(time_str, "%Y-%m-%d %H:%M:%S")
-
     if return_str:
         return str(r)
     return r
 
 
+# 时间加几天
+def datetime_add(s=None, days=0, seconds=0, microseconds=0, milliseconds=0, minutes=0, hours=0, weeks=0):
+    return to_datetime(s) + timedelta(days=days, seconds=seconds, microseconds=microseconds, milliseconds=milliseconds, minutes=minutes, hours=hours,
+                                      weeks=weeks)
+
+
+def to_date(s=None):
+    return to_datetime(s, True)[0:10]
+
+
 # 将 list 中的数据以 json 或者基本类型的形式写入到文件中
 # list_data : 数组数据, 也可以不是数组
 # file_name : 文件名
 # fixed_name : 是否固定文件名
 # file_path : 文件路径
 def to_txt(list_data, file_name='txt', file_path='txt', fixed_name=False, suffix='.txt'):
     file_name = str(file_name)
@@ -453,18 +461,18 @@
 # print(to_int(2.2))
 
 # print(to_float('a'))
 # print(to_float(2))
 # print(to_float(2.2))
 # print(to_float(2.24))
 
-# print(to_datetime('2019-09'))
-# print(to_datetime('2019-09-08'))
-# print(to_datetime('2019-09-08 12'))
-# print(to_datetime('2019-09-08 12:13'))
+# print(to_date('2019-09'))
+# print(to_date('2019-09-08'))
+# print(to_date('2019-09-08 12'))
+# print(to_date('2019-09-08 12:13'))
 # print(to_datetime('2019-09-08 12:13:14'))
 # print(to_datetime('2019-09-08 12:13:14.789'))
 # print(to_datetime(1686537485))
 # print(to_datetime(1686537484467))
 # print(to_datetime(datetime.today()))
 #
 # print(do_md5())
```

### Comparing `yplib-0.2.5/yplib/line_stack_temp.py` & `yplib-0.2.6/yplib/line_stack_temp.py`

 * *Files identical despite different names*

### Comparing `yplib-0.2.5/yplib.egg-info/PKG-INFO` & `yplib-0.2.6/yplib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yplib
-Version: 0.2.5
+Version: 0.2.6
 Summary: util
 Home-page: https://github.com/pypa/sampleproject
 Author: yangpu
 Author-email: wantwaterfish@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

