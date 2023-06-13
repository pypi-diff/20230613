# Comparing `tmp/nonebot_plugin_bili_push-0.1.0.tar.gz` & `tmp/nonebot_plugin_bili_push-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bili_push-0.1.0.tar", last modified: Mon Jun 12 19:05:09 2023, max compression
+gzip compressed data, was "nonebot_plugin_bili_push-0.1.1.tar", last modified: Tue Jun 13 04:47:52 2023, max compression
```

## Comparing `nonebot_plugin_bili_push-0.1.0.tar` & `nonebot_plugin_bili_push-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 19:05:09.121185 nonebot_plugin_bili_push-0.1.0/
--rw-rw-rw-   0        0        0     1078 2023-06-13 02:14:36.000000 nonebot_plugin_bili_push-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      268 2023-06-12 19:05:09.120185 nonebot_plugin_bili_push-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1046 2023-06-12 19:01:08.000000 nonebot_plugin_bili_push-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 19:05:09.110183 nonebot_plugin_bili_push-0.1.0/nonebot_plugin_bili_push/
--rw-rw-rw-   0        0        0   102893 2023-06-12 15:39:34.000000 nonebot_plugin_bili_push-0.1.0/nonebot_plugin_bili_push/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 19:05:09.119184 nonebot_plugin_bili_push-0.1.0/nonebot_plugin_bili_push.egg-info/
--rw-rw-rw-   0        0        0      268 2023-06-12 19:05:09.000000 nonebot_plugin_bili_push-0.1.0/nonebot_plugin_bili_push.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      302 2023-06-12 19:05:09.000000 nonebot_plugin_bili_push-0.1.0/nonebot_plugin_bili_push.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 19:05:09.000000 nonebot_plugin_bili_push-0.1.0/nonebot_plugin_bili_push.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2023-06-12 19:05:09.000000 nonebot_plugin_bili_push-0.1.0/nonebot_plugin_bili_push.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-06-12 19:05:09.000000 nonebot_plugin_bili_push-0.1.0/nonebot_plugin_bili_push.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-12 19:05:09.121185 nonebot_plugin_bili_push-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      675 2023-06-12 18:16:14.000000 nonebot_plugin_bili_push-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 04:47:52.341422 nonebot_plugin_bili_push-0.1.1/
+-rw-rw-rw-   0        0        0     1078 2023-06-13 02:14:36.000000 nonebot_plugin_bili_push-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      268 2023-06-13 04:47:52.341422 nonebot_plugin_bili_push-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1046 2023-06-12 19:01:08.000000 nonebot_plugin_bili_push-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-13 04:47:52.332423 nonebot_plugin_bili_push-0.1.1/nonebot_plugin_bili_push/
+-rw-rw-rw-   0        0        0   102893 2023-06-12 15:39:34.000000 nonebot_plugin_bili_push-0.1.1/nonebot_plugin_bili_push/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 04:47:52.340423 nonebot_plugin_bili_push-0.1.1/nonebot_plugin_bili_push.egg-info/
+-rw-rw-rw-   0        0        0      268 2023-06-13 04:47:52.000000 nonebot_plugin_bili_push-0.1.1/nonebot_plugin_bili_push.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      302 2023-06-13 04:47:52.000000 nonebot_plugin_bili_push-0.1.1/nonebot_plugin_bili_push.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 04:47:52.000000 nonebot_plugin_bili_push-0.1.1/nonebot_plugin_bili_push.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       84 2023-06-13 04:47:52.000000 nonebot_plugin_bili_push-0.1.1/nonebot_plugin_bili_push.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-06-13 04:47:52.000000 nonebot_plugin_bili_push-0.1.1/nonebot_plugin_bili_push.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-13 04:47:52.342421 nonebot_plugin_bili_push-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      752 2023-06-13 04:47:22.000000 nonebot_plugin_bili_push-0.1.1/setup.py
```

### Comparing `nonebot_plugin_bili_push-0.1.0/LICENSE` & `nonebot_plugin_bili_push-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bili_push-0.1.0/README.md` & `nonebot_plugin_bili_push-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bili_push-0.1.0/nonebot_plugin_bili_push/__init__.py` & `nonebot_plugin_bili_push-0.1.1/nonebot_plugin_bili_push/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bili_push-0.1.0/setup.py` & `nonebot_plugin_bili_push-0.1.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,21 +2,23 @@
 # -*- coding:utf-8 -*-
 from setuptools import setup, find_packages
 
 
 def get_install_requires():
     reqs = [
         'pillow>=9.5.0',
-        'requests>=2.30.0'
+        'requests>=2.30.0',
+        'nonebot2>=2.0.0rc3',
+        'nonebot_plugin_apscheduler>=0.2.0'
     ]
     return reqs
 
 
 setup(name='nonebot_plugin_bili_push',
-      version='0.1.0',
+      version='0.1.1',
       description='Nonebot2 plugin',
       author='SuperGuGuGu',
       author_email='13680478000@163.com',
       url='https://github.com/SuperGuGuGu/nonebot_plugin_bili_push',
       packages=find_packages(),
       python_requires=">=3.8",
       install_requires=get_install_requires(),
```

