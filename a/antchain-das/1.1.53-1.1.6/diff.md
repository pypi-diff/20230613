# Comparing `tmp/antchain_das-1.1.53.tar.gz` & `tmp/antchain_das-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_das-1.1.53.tar", last modified: Tue Jun 13 04:24:58 2023, max compression
+gzip compressed data, was "dist/antchain_das-1.1.6.tar", last modified: Tue Sep 14 03:46:09 2021, max compression
```

## Comparing `antchain_das-1.1.53.tar` & `antchain_das-1.1.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 04:24:58.000000 antchain_das-1.1.53/
--rw-r--r--   0 root         (0) root         (0)      600 2023-06-13 04:24:57.000000 antchain_das-1.1.53/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-06-13 04:24:57.000000 antchain_das-1.1.53/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2163 2023-06-13 04:24:58.000000 antchain_das-1.1.53/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      804 2023-06-13 04:24:57.000000 antchain_das-1.1.53/README-CN.md
--rw-r--r--   0 root         (0) root         (0)      990 2023-06-13 04:24:57.000000 antchain_das-1.1.53/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 04:24:58.000000 antchain_das-1.1.53/antchain_das.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2163 2023-06-13 04:24:57.000000 antchain_das-1.1.53/antchain_das.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      323 2023-06-13 04:24:57.000000 antchain_das-1.1.53/antchain_das.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 04:24:57.000000 antchain_das-1.1.53/antchain_das.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-06-13 04:24:57.000000 antchain_das-1.1.53/antchain_das.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-06-13 04:24:57.000000 antchain_das-1.1.53/antchain_das.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 04:24:58.000000 antchain_das-1.1.53/antchain_sdk_das/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-13 04:24:57.000000 antchain_das-1.1.53/antchain_sdk_das/__init__.py
--rw-r--r--   0 root         (0) root         (0)    96944 2023-06-13 04:24:57.000000 antchain_das-1.1.53/antchain_sdk_das/client.py
--rw-r--r--   0 root         (0) root         (0)   233041 2023-06-13 04:24:57.000000 antchain_das-1.1.53/antchain_sdk_das/models.py
--rw-r--r--   0 root         (0) root         (0)       73 2023-06-13 04:24:58.000000 antchain_das-1.1.53/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2488 2023-06-13 04:24:57.000000 antchain_das-1.1.53/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-14 03:46:09.000000 antchain_das-1.1.6/
+-rw-r--r--   0 root         (0) root         (0)      600 2021-09-14 03:46:09.000000 antchain_das-1.1.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2021-09-14 03:46:09.000000 antchain_das-1.1.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2170 2021-09-14 03:46:09.000000 antchain_das-1.1.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      812 2021-09-14 03:46:09.000000 antchain_das-1.1.6/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)      998 2021-09-14 03:46:09.000000 antchain_das-1.1.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-14 03:46:09.000000 antchain_das-1.1.6/antchain_das.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2170 2021-09-14 03:46:09.000000 antchain_das-1.1.6/antchain_das.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      323 2021-09-14 03:46:09.000000 antchain_das-1.1.6/antchain_das.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-09-14 03:46:09.000000 antchain_das-1.1.6/antchain_das.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2021-09-14 03:46:09.000000 antchain_das-1.1.6/antchain_das.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2021-09-14 03:46:09.000000 antchain_das-1.1.6/antchain_das.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-14 03:46:09.000000 antchain_das-1.1.6/antchain_sdk_das/
+-rw-r--r--   0 root         (0) root         (0)       21 2021-09-14 03:46:09.000000 antchain_das-1.1.6/antchain_sdk_das/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    38842 2021-09-14 03:46:09.000000 antchain_das-1.1.6/antchain_sdk_das/client.py
+-rw-r--r--   0 root         (0) root         (0)    75009 2021-09-14 03:46:09.000000 antchain_das-1.1.6/antchain_sdk_das/models.py
+-rw-r--r--   0 root         (0) root         (0)       73 2021-09-14 03:46:09.000000 antchain_das-1.1.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2488 2021-09-14 03:46:09.000000 antchain_das-1.1.6/setup.py
```

### Comparing `antchain_das-1.1.53/LICENSE` & `antchain_das-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_das-1.1.53/PKG-INFO` & `antchain_das-1.1.6/antchain_das.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: antchain_das
-Version: 1.1.53
+Name: antchain-das
+Version: 1.1.6
 Summary: Ant Chain DAS SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         
@@ -17,16 +17,16 @@
         ## Installation
         
         - **Install with pip**
         
         Python SDK uses a common package management tool named `pip`. If pip is not installed, see the [pip user guide](https://pip.pypa.io/en/stable/installing/ "pip User Guide") to install pip.
         
         ```bash
-        # Install the antchain-das
-        pip install antchain-das
+        # Install the antchain_sdk_das
+        pip install antchain_sdk_das
         ```
         
         ## Issues
         
         [Opening an Issue](https://github.com/alipay/antchain-openapi-prod-sdk/issues/new), Issues not conforming to the guidelines may be closed immediately.
         
         ## Usage
```

### Comparing `antchain_das-1.1.53/README-CN.md` & `antchain_das-1.1.6/README-CN.md`

 * *Files 15% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 ## 安装
 
 - **使用 pip 安装(推荐)**
 
 如未安装 `pip`, 请先至pip官网 [pip user guide](https://pip.pypa.io/en/stable/installing/ "pip User Guide") 安装pip .
 
 ```bash
-# 安装 antchain-das
-pip install antchain-das
+# 安装 antchain_sdk_das
+pip install antchain_sdk_das
 ```
 
 ## 问题
 
 [提交 Issue](https://github.com/alipay/antchain-openapi-prod-sdk/issues/new)，不符合指南的问题可能会立即关闭。
 
 ## 使用说明
```

### Comparing `antchain_das-1.1.53/README.md` & `antchain_das-1.1.6/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 ## Installation
 
 - **Install with pip**
 
 Python SDK uses a common package management tool named `pip`. If pip is not installed, see the [pip user guide](https://pip.pypa.io/en/stable/installing/ "pip User Guide") to install pip.
 
 ```bash
-# Install the antchain-das
-pip install antchain-das
+# Install the antchain_sdk_das
+pip install antchain_sdk_das
 ```
 
 ## Issues
 
 [Opening an Issue](https://github.com/alipay/antchain-openapi-prod-sdk/issues/new), Issues not conforming to the guidelines may be closed immediately.
 
 ## Usage
```

### Comparing `antchain_das-1.1.53/antchain_das.egg-info/PKG-INFO` & `antchain_das-1.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: antchain-das
-Version: 1.1.53
+Name: antchain_das
+Version: 1.1.6
 Summary: Ant Chain DAS SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         
@@ -17,16 +17,16 @@
         ## Installation
         
         - **Install with pip**
         
         Python SDK uses a common package management tool named `pip`. If pip is not installed, see the [pip user guide](https://pip.pypa.io/en/stable/installing/ "pip User Guide") to install pip.
         
         ```bash
-        # Install the antchain-das
-        pip install antchain-das
+        # Install the antchain_sdk_das
+        pip install antchain_sdk_das
         ```
         
         ## Issues
         
         [Opening an Issue](https://github.com/alipay/antchain-openapi-prod-sdk/issues/new), Issues not conforming to the guidelines may be closed immediately.
         
         ## Usage
```

### Comparing `antchain_das-1.1.53/setup.py` & `antchain_das-1.1.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,29 +20,29 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for antchain_das.
 
-Created on 13/06/2023
+Created on 14/09/2021
 
 @author: Ant Chain SDK
 """
 
 PACKAGE = "antchain_sdk_das"
 NAME = "antchain_das" or "alibabacloud-package"
 DESCRIPTION = "Ant Chain DAS SDK Library for Python"
 AUTHOR = "Ant Chain SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/alipay/antchain-openapi-prod-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
     "antchain_alipay_util>=1.0.1, <2.0.0",
-    "alibabacloud_tea_util>=0.3.8, <1.0.0",
+    "alibabacloud_tea_util>=0.3.5, <1.0.0",
     "alibabacloud_rpc_util>=0.0.4, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
```

