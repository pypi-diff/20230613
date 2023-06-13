# Comparing `tmp/nonebot-plugin-b23-0.0.6.tar.gz` & `tmp/nonebot-plugin-b23-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-b23-0.0.6.tar", last modified: Wed Feb  1 12:01:40 2023, max compression
+gzip compressed data, was "nonebot-plugin-b23-0.0.7.tar", last modified: Tue Jun 13 13:49:37 2023, max compression
```

## Comparing `nonebot-plugin-b23-0.0.6.tar` & `nonebot-plugin-b23-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 12:01:40.701378 nonebot-plugin-b23-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-02-01 12:01:29.000000 nonebot-plugin-b23-0.0.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-02-01 12:01:40.705378 nonebot-plugin-b23-0.0.6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 12:01:40.701378 nonebot-plugin-b23-0.0.6/nonebot_plugin_b23/
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-02-01 12:01:29.000000 nonebot-plugin-b23-0.0.6/nonebot_plugin_b23/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-02-01 12:01:29.000000 nonebot-plugin-b23-0.0.6/nonebot_plugin_b23/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 12:01:40.701378 nonebot-plugin-b23-0.0.6/nonebot_plugin_b23.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-02-01 12:01:40.000000 nonebot-plugin-b23-0.0.6/nonebot_plugin_b23.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-02-01 12:01:40.000000 nonebot-plugin-b23-0.0.6/nonebot_plugin_b23.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-01 12:01:40.000000 nonebot-plugin-b23-0.0.6/nonebot_plugin_b23.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-02-01 12:01:40.000000 nonebot-plugin-b23-0.0.6/nonebot_plugin_b23.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-02-01 12:01:40.000000 nonebot-plugin-b23-0.0.6/nonebot_plugin_b23.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-02-01 12:01:40.705378 nonebot-plugin-b23-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-02-01 12:01:29.000000 nonebot-plugin-b23-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:49:37.239415 nonebot-plugin-b23-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-13 13:49:24.000000 nonebot-plugin-b23-0.0.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-13 13:49:37.239415 nonebot-plugin-b23-0.0.7/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:49:37.239415 nonebot-plugin-b23-0.0.7/nonebot_plugin_b23/
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-06-13 13:49:24.000000 nonebot-plugin-b23-0.0.7/nonebot_plugin_b23/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-13 13:49:24.000000 nonebot-plugin-b23-0.0.7/nonebot_plugin_b23/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:49:37.239415 nonebot-plugin-b23-0.0.7/nonebot_plugin_b23.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-13 13:49:37.000000 nonebot-plugin-b23-0.0.7/nonebot_plugin_b23.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-13 13:49:37.000000 nonebot-plugin-b23-0.0.7/nonebot_plugin_b23.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 13:49:37.000000 nonebot-plugin-b23-0.0.7/nonebot_plugin_b23.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-13 13:49:37.000000 nonebot-plugin-b23-0.0.7/nonebot_plugin_b23.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-13 13:49:37.000000 nonebot-plugin-b23-0.0.7/nonebot_plugin_b23.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-13 13:49:37.239415 nonebot-plugin-b23-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-13 13:49:24.000000 nonebot-plugin-b23-0.0.7/setup.py
```

### Comparing `nonebot-plugin-b23-0.0.6/LICENSE.txt` & `nonebot-plugin-b23-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-b23-0.0.6/setup.py` & `nonebot-plugin-b23-0.0.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import setuptools
 
 setuptools.setup(
     name="nonebot-plugin-b23",
-    version="0.0.6",
+    version="0.0.7",
     author="eya46",
     install_requires=[
         'httpx~=0.23.0',
-        'nonebot2>=2.0.0-beta.1',
+        'nonebot2~=2.0.0',
         'pydantic~=1.10.4'
     ],
     author_email="eya46@qq.com",
     description="nonebot2 plugin B站热搜",  # 包的简述
     long_description_content_type="text/markdown",
     url="https://github.com/eya46/nonebot_plugin_b23",
     packages=setuptools.find_packages(),
```

