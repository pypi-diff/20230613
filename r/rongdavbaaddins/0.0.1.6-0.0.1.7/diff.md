# Comparing `tmp/rongdavbaaddins-0.0.1.6.tar.gz` & `tmp/rongdavbaaddins-0.0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rongdavbaaddins-0.0.1.6.tar", last modified: Mon Jun 12 08:02:02 2023, max compression
+gzip compressed data, was "rongdavbaaddins-0.0.1.7.tar", last modified: Mon Jun 12 08:04:09 2023, max compression
```

## Comparing `rongdavbaaddins-0.0.1.6.tar` & `rongdavbaaddins-0.0.1.7.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 08:02:02.001472 rongdavbaaddins-0.0.1.6/
--rw-rw-rw-   0        0        0     1090 2022-12-21 02:47:10.000000 rongdavbaaddins-0.0.1.6/LICENSE.txt
--rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 rongdavbaaddins-0.0.1.6/MANIFEST.in
--rw-rw-rw-   0        0        0      409 2023-06-12 08:02:02.001472 rongdavbaaddins-0.0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0       33 2023-02-21 06:55:26.000000 rongdavbaaddins-0.0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 08:02:01.990472 rongdavbaaddins-0.0.1.6/rongdaVbaAddins/
--rw-rw-rw-   0        0        0    15227 2023-06-02 06:14:22.000000 rongdavbaaddins-0.0.1.6/rongdaVbaAddins/Excel.officeUI
-drwxrwxrwx   0        0        0        0 2023-06-12 08:02:01.994470 rongdavbaaddins-0.0.1.6/rongdaVbaAddins/Function/
--rw-rw-rw-   0        0        0        0 2023-06-08 02:38:12.000000 rongdavbaaddins-0.0.1.6/rongdaVbaAddins/Function/__init__.py
--rw-rw-rw-   0        0        0    41472 2023-06-01 02:58:27.000000 rongdavbaaddins-0.0.1.6/rongdaVbaAddins/Function/minusFunction.pyd
--rw-rw-rw-   0        0        0      204 2023-06-01 03:01:41.000000 rongdavbaaddins-0.0.1.6/rongdaVbaAddins/Function/minusFunctionpy.py
--rw-rw-rw-   0        0        0   110002 2023-06-12 07:30:57.000000 rongdavbaaddins-0.0.1.6/rongdaVbaAddins/RDaddins.xlam
-drwxrwxrwx   0        0        0        0 2023-06-12 08:02:01.996472 rongdavbaaddins-0.0.1.6/rongdaVbaAddins/Ui/
--rw-rw-rw-   0        0        0        0 2023-06-08 02:38:04.000000 rongdavbaaddins-0.0.1.6/rongdaVbaAddins/Ui/__init__.py
--rw-rw-rw-   0        0        0     3281 2023-06-07 05:42:04.000000 rongdavbaaddins-0.0.1.6/rongdaVbaAddins/Ui/rongdaVbaAddinsUi.py
--rw-rw-rw-   0        0        0    54784 2023-05-31 09:26:30.000000 rongdavbaaddins-0.0.1.6/rongdaVbaAddins/Vbalog.pyd
--rw-rw-rw-   0        0        0     1000 2023-06-08 09:19:01.000000 rongdavbaaddins-0.0.1.6/rongdaVbaAddins/Vbalogpy.py
--rw-rw-rw-   0        0        0        0 2023-06-01 01:46:56.000000 rongdavbaaddins-0.0.1.6/rongdaVbaAddins/__init__.py
--rw-rw-rw-   0        0        0    48640 2023-06-08 01:57:00.000000 rongdavbaaddins-0.0.1.6/rongdaVbaAddins/getNumber.pyd
--rw-rw-rw-   0        0        0      448 2023-06-09 06:42:10.000000 rongdavbaaddins-0.0.1.6/rongdaVbaAddins/getNumberpy.py
--rw-rw-rw-   0        0        0    41984 2023-06-08 01:39:24.000000 rongdavbaaddins-0.0.1.6/rongdaVbaAddins/minusFunction.pyd
--rw-rw-rw-   0        0        0   141312 2023-06-12 08:01:31.000000 rongdavbaaddins-0.0.1.6/rongdaVbaAddins/rongdavbaaddins.pyd
--rw-rw-rw-   0        0        0    66560 2023-06-09 03:08:54.000000 rongdavbaaddins-0.0.1.6/rongdaVbaAddins/vbaLogin.pyd
--rw-rw-rw-   0        0        0      289 2023-06-08 07:23:23.000000 rongdavbaaddins-0.0.1.6/rongdaVbaAddins/vbaloginpy.py
--rw-rw-rw-   0        0        0    27954 2023-06-12 07:30:57.000000 rongdavbaaddins-0.0.1.6/rongdaVbaAddins/文件处理类模板.xlsx
-drwxrwxrwx   0        0        0        0 2023-06-12 08:02:02.000471 rongdavbaaddins-0.0.1.6/rongdavbaaddins.egg-info/
--rw-rw-rw-   0        0        0      409 2023-06-12 08:02:01.000000 rongdavbaaddins-0.0.1.6/rongdavbaaddins.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      780 2023-06-12 08:02:01.000000 rongdavbaaddins-0.0.1.6/rongdavbaaddins.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 08:02:01.000000 rongdavbaaddins-0.0.1.6/rongdavbaaddins.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-06-12 08:02:01.000000 rongdavbaaddins-0.0.1.6/rongdavbaaddins.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      136 2023-06-12 08:02:02.003473 rongdavbaaddins-0.0.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1024 2023-06-12 07:59:41.000000 rongdavbaaddins-0.0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 08:04:09.884605 rongdavbaaddins-0.0.1.7/
+-rw-rw-rw-   0        0        0     1090 2022-12-21 02:47:10.000000 rongdavbaaddins-0.0.1.7/LICENSE.txt
+-rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 rongdavbaaddins-0.0.1.7/MANIFEST.in
+-rw-rw-rw-   0        0        0      409 2023-06-12 08:04:09.884605 rongdavbaaddins-0.0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0       33 2023-02-21 06:55:26.000000 rongdavbaaddins-0.0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 08:04:09.870612 rongdavbaaddins-0.0.1.7/rongdaVbaAddins/
+-rw-rw-rw-   0        0        0    15227 2023-06-02 06:14:22.000000 rongdavbaaddins-0.0.1.7/rongdaVbaAddins/Excel.officeUI
+drwxrwxrwx   0        0        0        0 2023-06-12 08:04:09.874621 rongdavbaaddins-0.0.1.7/rongdaVbaAddins/Function/
+-rw-rw-rw-   0        0        0        0 2023-06-08 02:38:12.000000 rongdavbaaddins-0.0.1.7/rongdaVbaAddins/Function/__init__.py
+-rw-rw-rw-   0        0        0    41472 2023-06-01 02:58:27.000000 rongdavbaaddins-0.0.1.7/rongdaVbaAddins/Function/minusFunction.pyd
+-rw-rw-rw-   0        0        0      204 2023-06-01 03:01:41.000000 rongdavbaaddins-0.0.1.7/rongdaVbaAddins/Function/minusFunctionpy.py
+-rw-rw-rw-   0        0        0   110436 2023-06-12 07:59:28.000000 rongdavbaaddins-0.0.1.7/rongdaVbaAddins/RDaddins.xlam
+drwxrwxrwx   0        0        0        0 2023-06-12 08:04:09.877616 rongdavbaaddins-0.0.1.7/rongdaVbaAddins/Ui/
+-rw-rw-rw-   0        0        0        0 2023-06-08 02:38:04.000000 rongdavbaaddins-0.0.1.7/rongdaVbaAddins/Ui/__init__.py
+-rw-rw-rw-   0        0        0     3281 2023-06-07 05:42:04.000000 rongdavbaaddins-0.0.1.7/rongdaVbaAddins/Ui/rongdaVbaAddinsUi.py
+-rw-rw-rw-   0        0        0    54784 2023-05-31 09:26:30.000000 rongdavbaaddins-0.0.1.7/rongdaVbaAddins/Vbalog.pyd
+-rw-rw-rw-   0        0        0     1000 2023-06-08 09:19:01.000000 rongdavbaaddins-0.0.1.7/rongdaVbaAddins/Vbalogpy.py
+-rw-rw-rw-   0        0        0        0 2023-06-01 01:46:56.000000 rongdavbaaddins-0.0.1.7/rongdaVbaAddins/__init__.py
+-rw-rw-rw-   0        0        0    48640 2023-06-08 01:57:00.000000 rongdavbaaddins-0.0.1.7/rongdaVbaAddins/getNumber.pyd
+-rw-rw-rw-   0        0        0      448 2023-06-09 06:42:10.000000 rongdavbaaddins-0.0.1.7/rongdaVbaAddins/getNumberpy.py
+-rw-rw-rw-   0        0        0    41984 2023-06-08 01:39:24.000000 rongdavbaaddins-0.0.1.7/rongdaVbaAddins/minusFunction.pyd
+-rw-rw-rw-   0        0        0   141312 2023-06-12 08:03:33.000000 rongdavbaaddins-0.0.1.7/rongdaVbaAddins/rongdavbaaddins.pyd
+-rw-rw-rw-   0        0        0    66560 2023-06-09 03:08:54.000000 rongdavbaaddins-0.0.1.7/rongdaVbaAddins/vbaLogin.pyd
+-rw-rw-rw-   0        0        0      289 2023-06-08 07:23:23.000000 rongdavbaaddins-0.0.1.7/rongdaVbaAddins/vbaloginpy.py
+-rw-rw-rw-   0        0        0    27954 2023-06-12 07:59:27.000000 rongdavbaaddins-0.0.1.7/rongdaVbaAddins/文件处理类模板.xlsx
+drwxrwxrwx   0        0        0        0 2023-06-12 08:04:09.882638 rongdavbaaddins-0.0.1.7/rongdavbaaddins.egg-info/
+-rw-rw-rw-   0        0        0      409 2023-06-12 08:04:09.000000 rongdavbaaddins-0.0.1.7/rongdavbaaddins.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      780 2023-06-12 08:04:09.000000 rongdavbaaddins-0.0.1.7/rongdavbaaddins.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 08:04:09.000000 rongdavbaaddins-0.0.1.7/rongdavbaaddins.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-06-12 08:04:09.000000 rongdavbaaddins-0.0.1.7/rongdavbaaddins.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      136 2023-06-12 08:04:09.885671 rongdavbaaddins-0.0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1024 2023-06-12 08:03:11.000000 rongdavbaaddins-0.0.1.7/setup.py
```

### Comparing `rongdavbaaddins-0.0.1.6/LICENSE.txt` & `rongdavbaaddins-0.0.1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.1.6/rongdaVbaAddins/Excel.officeUI` & `rongdavbaaddins-0.0.1.7/rongdaVbaAddins/Excel.officeUI`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.1.6/rongdaVbaAddins/Ui/rongdaVbaAddinsUi.py` & `rongdavbaaddins-0.0.1.7/rongdaVbaAddins/Ui/rongdaVbaAddinsUi.py`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.1.6/rongdaVbaAddins/Vbalogpy.py` & `rongdavbaaddins-0.0.1.7/rongdaVbaAddins/Vbalogpy.py`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.1.6/rongdaVbaAddins/文件处理类模板.xlsx` & `rongdavbaaddins-0.0.1.7/rongdaVbaAddins/文件处理类模板.xlsx`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.1.6/rongdavbaaddins.egg-info/SOURCES.txt` & `rongdavbaaddins-0.0.1.7/rongdavbaaddins.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.1.6/setup.py` & `rongdavbaaddins-0.0.1.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #-*- coding:utf-8 -*-
 import os 
 from setuptools import setup, find_packages
 
 MAJOR = 0
 MINOR = 0
 PATCH = 1
-VERSION = f"{MAJOR}.{MINOR}.{PATCH}.6"
+VERSION = f"{MAJOR}.{MINOR}.{PATCH}.7"
 
 def get_install_requires():
     reqs = []
     return reqs
 setup(
 	name = "rongdavbaaddins",
     version=VERSION,
```

