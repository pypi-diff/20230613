# Comparing `tmp/liveramp_automation_framework-0.1.6.tar.gz` & `tmp/liveramp_automation_framework-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liveramp_automation_framework-0.1.6.tar", last modified: Tue Jun 13 07:58:50 2023, max compression
+gzip compressed data, was "liveramp_automation_framework-0.1.7.tar", last modified: Tue Jun 13 08:06:17 2023, max compression
```

## Comparing `liveramp_automation_framework-0.1.6.tar` & `liveramp_automation_framework-0.1.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-06-13 07:58:50.302883 liveramp_automation_framework-0.1.6/
--rw-r--r--   0 jasqia     (502) staff       (20)      818 2023-06-13 07:58:50.302115 liveramp_automation_framework-0.1.6/PKG-INFO
-drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-06-13 07:58:50.295733 liveramp_automation_framework-0.1.6/liveramp_automation/
--rw-r--r--   0 jasqia     (502) staff       (20)      370 2023-06-13 07:16:27.000000 liveramp_automation_framework-0.1.6/liveramp_automation/allure_util.py
--rw-r--r--   0 jasqia     (502) staff       (20)      928 2023-06-08 08:26:48.000000 liveramp_automation_framework-0.1.6/liveramp_automation/logger.py
--rw-r--r--   0 jasqia     (502) staff       (20)     3120 2023-06-12 02:49:19.000000 liveramp_automation_framework-0.1.6/liveramp_automation/login_util.py
--rw-r--r--   0 jasqia     (502) staff       (20)      713 2023-05-03 08:30:53.000000 liveramp_automation_framework-0.1.6/liveramp_automation/parsers.py
--rw-r--r--   0 jasqia     (502) staff       (20)      742 2023-06-13 07:55:12.000000 liveramp_automation_framework-0.1.6/liveramp_automation/playwright_util.py
--rw-r--r--   0 jasqia     (502) staff       (20)     2232 2023-06-13 07:16:27.000000 liveramp_automation_framework-0.1.6/liveramp_automation/read_report.py
--rw-r--r--   0 jasqia     (502) staff       (20)     6966 2023-06-13 07:16:27.000000 liveramp_automation_framework-0.1.6/liveramp_automation/request_util.py
--rw-r--r--   0 jasqia     (502) staff       (20)      743 2023-06-13 07:58:47.000000 liveramp_automation_framework-0.1.6/liveramp_automation/selenium_util.py
--rw-r--r--   0 jasqia     (502) staff       (20)      781 2023-06-08 08:16:59.000000 liveramp_automation_framework-0.1.6/liveramp_automation/time_util.py
--rw-r--r--   0 jasqia     (502) staff       (20)      718 2023-06-13 07:16:27.000000 liveramp_automation_framework-0.1.6/liveramp_automation/upload_util.py
-drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-06-13 07:58:50.300987 liveramp_automation_framework-0.1.6/liveramp_automation_framework.egg-info/
--rw-r--r--   0 jasqia     (502) staff       (20)      818 2023-06-13 07:58:50.000000 liveramp_automation_framework-0.1.6/liveramp_automation_framework.egg-info/PKG-INFO
--rw-r--r--   0 jasqia     (502) staff       (20)      617 2023-06-13 07:58:50.000000 liveramp_automation_framework-0.1.6/liveramp_automation_framework.egg-info/SOURCES.txt
--rw-r--r--   0 jasqia     (502) staff       (20)        1 2023-06-13 07:58:50.000000 liveramp_automation_framework-0.1.6/liveramp_automation_framework.egg-info/dependency_links.txt
--rw-r--r--   0 jasqia     (502) staff       (20)      381 2023-06-13 07:58:50.000000 liveramp_automation_framework-0.1.6/liveramp_automation_framework.egg-info/requires.txt
--rw-r--r--   0 jasqia     (502) staff       (20)       20 2023-06-13 07:58:50.000000 liveramp_automation_framework-0.1.6/liveramp_automation_framework.egg-info/top_level.txt
--rw-r--r--   0 jasqia     (502) staff       (20)       38 2023-06-13 07:58:50.303132 liveramp_automation_framework-0.1.6/setup.cfg
--rw-r--r--   0 jasqia     (502) staff       (20)     1169 2023-06-13 07:58:47.000000 liveramp_automation_framework-0.1.6/setup.py
+drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-06-13 08:06:17.625425 liveramp_automation_framework-0.1.7/
+-rw-r--r--   0 jasqia     (502) staff       (20)      818 2023-06-13 08:06:17.624921 liveramp_automation_framework-0.1.7/PKG-INFO
+drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-06-13 08:06:17.618456 liveramp_automation_framework-0.1.7/liveramp_automation/
+-rw-r--r--   0 jasqia     (502) staff       (20)      348 2023-06-13 08:06:15.000000 liveramp_automation_framework-0.1.7/liveramp_automation/allure_util.py
+-rw-r--r--   0 jasqia     (502) staff       (20)      928 2023-06-08 08:26:48.000000 liveramp_automation_framework-0.1.7/liveramp_automation/logger.py
+-rw-r--r--   0 jasqia     (502) staff       (20)     3120 2023-06-12 02:49:19.000000 liveramp_automation_framework-0.1.7/liveramp_automation/login_util.py
+-rw-r--r--   0 jasqia     (502) staff       (20)      713 2023-05-03 08:30:53.000000 liveramp_automation_framework-0.1.7/liveramp_automation/parsers.py
+-rw-r--r--   0 jasqia     (502) staff       (20)      742 2023-06-13 07:55:12.000000 liveramp_automation_framework-0.1.7/liveramp_automation/playwright_util.py
+-rw-r--r--   0 jasqia     (502) staff       (20)     2232 2023-06-13 07:16:27.000000 liveramp_automation_framework-0.1.7/liveramp_automation/read_report.py
+-rw-r--r--   0 jasqia     (502) staff       (20)     6966 2023-06-13 07:16:27.000000 liveramp_automation_framework-0.1.7/liveramp_automation/request_util.py
+-rw-r--r--   0 jasqia     (502) staff       (20)      743 2023-06-13 07:58:47.000000 liveramp_automation_framework-0.1.7/liveramp_automation/selenium_util.py
+-rw-r--r--   0 jasqia     (502) staff       (20)      781 2023-06-08 08:16:59.000000 liveramp_automation_framework-0.1.7/liveramp_automation/time_util.py
+-rw-r--r--   0 jasqia     (502) staff       (20)      718 2023-06-13 07:16:27.000000 liveramp_automation_framework-0.1.7/liveramp_automation/upload_util.py
+drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-06-13 08:06:17.623850 liveramp_automation_framework-0.1.7/liveramp_automation_framework.egg-info/
+-rw-r--r--   0 jasqia     (502) staff       (20)      818 2023-06-13 08:06:17.000000 liveramp_automation_framework-0.1.7/liveramp_automation_framework.egg-info/PKG-INFO
+-rw-r--r--   0 jasqia     (502) staff       (20)      617 2023-06-13 08:06:17.000000 liveramp_automation_framework-0.1.7/liveramp_automation_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 jasqia     (502) staff       (20)        1 2023-06-13 08:06:17.000000 liveramp_automation_framework-0.1.7/liveramp_automation_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 jasqia     (502) staff       (20)      381 2023-06-13 08:06:17.000000 liveramp_automation_framework-0.1.7/liveramp_automation_framework.egg-info/requires.txt
+-rw-r--r--   0 jasqia     (502) staff       (20)       20 2023-06-13 08:06:17.000000 liveramp_automation_framework-0.1.7/liveramp_automation_framework.egg-info/top_level.txt
+-rw-r--r--   0 jasqia     (502) staff       (20)       38 2023-06-13 08:06:17.625598 liveramp_automation_framework-0.1.7/setup.cfg
+-rw-r--r--   0 jasqia     (502) staff       (20)     1169 2023-06-13 08:06:15.000000 liveramp_automation_framework-0.1.7/setup.py
```

### Comparing `liveramp_automation_framework-0.1.6/PKG-INFO` & `liveramp_automation_framework-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liveramp_automation_framework
-Version: 0.1.6
+Version: 0.1.7
 Summary: This is the base liveramp_automation_framework
 Home-page: https://github.com/LiveRamp/qe_api_framework
 Author: Jasmine Qian
 Author-email: jasmine.qian@liveramp.com
 Description-Content-Type: text/markdown
 
 ### 1. Descprition of the repository
```

### Comparing `liveramp_automation_framework-0.1.6/liveramp_automation/logger.py` & `liveramp_automation_framework-0.1.7/liveramp_automation/logger.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation_framework-0.1.6/liveramp_automation/login_util.py` & `liveramp_automation_framework-0.1.7/liveramp_automation/login_util.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation_framework-0.1.6/liveramp_automation/parsers.py` & `liveramp_automation_framework-0.1.7/liveramp_automation/parsers.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation_framework-0.1.6/liveramp_automation/playwright_util.py` & `liveramp_automation_framework-0.1.7/liveramp_automation/playwright_util.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation_framework-0.1.6/liveramp_automation/read_report.py` & `liveramp_automation_framework-0.1.7/liveramp_automation/read_report.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation_framework-0.1.6/liveramp_automation/request_util.py` & `liveramp_automation_framework-0.1.7/liveramp_automation/request_util.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation_framework-0.1.6/liveramp_automation/selenium_util.py` & `liveramp_automation_framework-0.1.7/liveramp_automation/selenium_util.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation_framework-0.1.6/liveramp_automation/time_util.py` & `liveramp_automation_framework-0.1.7/liveramp_automation/time_util.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation_framework-0.1.6/liveramp_automation/upload_util.py` & `liveramp_automation_framework-0.1.7/liveramp_automation/upload_util.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation_framework-0.1.6/liveramp_automation_framework.egg-info/PKG-INFO` & `liveramp_automation_framework-0.1.7/liveramp_automation_framework.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liveramp-automation-framework
-Version: 0.1.6
+Version: 0.1.7
 Summary: This is the base liveramp_automation_framework
 Home-page: https://github.com/LiveRamp/qe_api_framework
 Author: Jasmine Qian
 Author-email: jasmine.qian@liveramp.com
 Description-Content-Type: text/markdown
 
 ### 1. Descprition of the repository
```

### Comparing `liveramp_automation_framework-0.1.6/liveramp_automation_framework.egg-info/SOURCES.txt` & `liveramp_automation_framework-0.1.7/liveramp_automation_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `liveramp_automation_framework-0.1.6/setup.py` & `liveramp_automation_framework-0.1.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("readme.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='liveramp_automation_framework',
-    version='0.1.6',
+    version='0.1.7',
     author='Jasmine Qian',
     author_email='jasmine.qian@liveramp.com',
     description="This is the base liveramp_automation_framework",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/LiveRamp/qe_api_framework",
     packages=['liveramp_automation'],
```

