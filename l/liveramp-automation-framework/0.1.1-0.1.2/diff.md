# Comparing `tmp/liveramp_automation_framework-0.1.1.tar.gz` & `tmp/liveramp_automation_framework-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liveramp_automation_framework-0.1.1.tar", last modified: Tue Jun 13 06:32:25 2023, max compression
+gzip compressed data, was "liveramp_automation_framework-0.1.2.tar", last modified: Tue Jun 13 07:07:17 2023, max compression
```

## Comparing `liveramp_automation_framework-0.1.1.tar` & `liveramp_automation_framework-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-06-13 06:32:25.019393 liveramp_automation_framework-0.1.1/
--rw-r--r--   0 jasqia     (502) staff       (20)      818 2023-06-13 06:32:25.018906 liveramp_automation_framework-0.1.1/PKG-INFO
-drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-06-13 06:32:25.013770 liveramp_automation_framework-0.1.1/liveramp_automation/
--rw-r--r--   0 jasqia     (502) staff       (20)      271 2023-06-08 08:16:59.000000 liveramp_automation_framework-0.1.1/liveramp_automation/allure_util.py
--rw-r--r--   0 jasqia     (502) staff       (20)      928 2023-06-08 08:26:48.000000 liveramp_automation_framework-0.1.1/liveramp_automation/logger.py
--rw-r--r--   0 jasqia     (502) staff       (20)     3120 2023-06-12 02:49:19.000000 liveramp_automation_framework-0.1.1/liveramp_automation/login_util.py
--rw-r--r--   0 jasqia     (502) staff       (20)      713 2023-05-03 08:30:53.000000 liveramp_automation_framework-0.1.1/liveramp_automation/parsers.py
--rw-r--r--   0 jasqia     (502) staff       (20)      818 2023-06-12 02:49:19.000000 liveramp_automation_framework-0.1.1/liveramp_automation/playwright_util.py
--rw-r--r--   0 jasqia     (502) staff       (20)     2317 2023-06-12 02:49:19.000000 liveramp_automation_framework-0.1.1/liveramp_automation/read_report.py
--rw-r--r--   0 jasqia     (502) staff       (20)     6985 2023-06-12 02:49:19.000000 liveramp_automation_framework-0.1.1/liveramp_automation/request_util.py
--rw-r--r--   0 jasqia     (502) staff       (20)      836 2023-06-12 02:49:19.000000 liveramp_automation_framework-0.1.1/liveramp_automation/selenium_util.py
--rw-r--r--   0 jasqia     (502) staff       (20)      781 2023-06-08 08:16:59.000000 liveramp_automation_framework-0.1.1/liveramp_automation/time_util.py
--rw-r--r--   0 jasqia     (502) staff       (20)     1736 2023-06-13 06:32:14.000000 liveramp_automation_framework-0.1.1/liveramp_automation/upload_util.py
-drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-06-13 06:32:25.018065 liveramp_automation_framework-0.1.1/liveramp_automation_framework.egg-info/
--rw-r--r--   0 jasqia     (502) staff       (20)      818 2023-06-13 06:32:24.000000 liveramp_automation_framework-0.1.1/liveramp_automation_framework.egg-info/PKG-INFO
--rw-r--r--   0 jasqia     (502) staff       (20)      617 2023-06-13 06:32:24.000000 liveramp_automation_framework-0.1.1/liveramp_automation_framework.egg-info/SOURCES.txt
--rw-r--r--   0 jasqia     (502) staff       (20)        1 2023-06-13 06:32:24.000000 liveramp_automation_framework-0.1.1/liveramp_automation_framework.egg-info/dependency_links.txt
--rw-r--r--   0 jasqia     (502) staff       (20)      381 2023-06-13 06:32:24.000000 liveramp_automation_framework-0.1.1/liveramp_automation_framework.egg-info/requires.txt
--rw-r--r--   0 jasqia     (502) staff       (20)       20 2023-06-13 06:32:24.000000 liveramp_automation_framework-0.1.1/liveramp_automation_framework.egg-info/top_level.txt
--rw-r--r--   0 jasqia     (502) staff       (20)       38 2023-06-13 06:32:25.019607 liveramp_automation_framework-0.1.1/setup.cfg
--rw-r--r--   0 jasqia     (502) staff       (20)     1169 2023-06-13 06:32:22.000000 liveramp_automation_framework-0.1.1/setup.py
+drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-06-13 07:07:17.578268 liveramp_automation_framework-0.1.2/
+-rw-r--r--   0 jasqia     (502) staff       (20)      818 2023-06-13 07:07:17.577787 liveramp_automation_framework-0.1.2/PKG-INFO
+drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-06-13 07:07:17.572404 liveramp_automation_framework-0.1.2/liveramp_automation/
+-rw-r--r--   0 jasqia     (502) staff       (20)      271 2023-06-08 08:16:59.000000 liveramp_automation_framework-0.1.2/liveramp_automation/allure_util.py
+-rw-r--r--   0 jasqia     (502) staff       (20)      928 2023-06-08 08:26:48.000000 liveramp_automation_framework-0.1.2/liveramp_automation/logger.py
+-rw-r--r--   0 jasqia     (502) staff       (20)     3120 2023-06-12 02:49:19.000000 liveramp_automation_framework-0.1.2/liveramp_automation/login_util.py
+-rw-r--r--   0 jasqia     (502) staff       (20)      713 2023-05-03 08:30:53.000000 liveramp_automation_framework-0.1.2/liveramp_automation/parsers.py
+-rw-r--r--   0 jasqia     (502) staff       (20)      842 2023-06-13 07:07:14.000000 liveramp_automation_framework-0.1.2/liveramp_automation/playwright_util.py
+-rw-r--r--   0 jasqia     (502) staff       (20)     2317 2023-06-12 02:49:19.000000 liveramp_automation_framework-0.1.2/liveramp_automation/read_report.py
+-rw-r--r--   0 jasqia     (502) staff       (20)     6985 2023-06-12 02:49:19.000000 liveramp_automation_framework-0.1.2/liveramp_automation/request_util.py
+-rw-r--r--   0 jasqia     (502) staff       (20)      836 2023-06-12 02:49:19.000000 liveramp_automation_framework-0.1.2/liveramp_automation/selenium_util.py
+-rw-r--r--   0 jasqia     (502) staff       (20)      781 2023-06-08 08:16:59.000000 liveramp_automation_framework-0.1.2/liveramp_automation/time_util.py
+-rw-r--r--   0 jasqia     (502) staff       (20)     1736 2023-06-13 06:32:14.000000 liveramp_automation_framework-0.1.2/liveramp_automation/upload_util.py
+drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-06-13 07:07:17.577003 liveramp_automation_framework-0.1.2/liveramp_automation_framework.egg-info/
+-rw-r--r--   0 jasqia     (502) staff       (20)      818 2023-06-13 07:07:17.000000 liveramp_automation_framework-0.1.2/liveramp_automation_framework.egg-info/PKG-INFO
+-rw-r--r--   0 jasqia     (502) staff       (20)      617 2023-06-13 07:07:17.000000 liveramp_automation_framework-0.1.2/liveramp_automation_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 jasqia     (502) staff       (20)        1 2023-06-13 07:07:17.000000 liveramp_automation_framework-0.1.2/liveramp_automation_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 jasqia     (502) staff       (20)      381 2023-06-13 07:07:17.000000 liveramp_automation_framework-0.1.2/liveramp_automation_framework.egg-info/requires.txt
+-rw-r--r--   0 jasqia     (502) staff       (20)       20 2023-06-13 07:07:17.000000 liveramp_automation_framework-0.1.2/liveramp_automation_framework.egg-info/top_level.txt
+-rw-r--r--   0 jasqia     (502) staff       (20)       38 2023-06-13 07:07:17.578505 liveramp_automation_framework-0.1.2/setup.cfg
+-rw-r--r--   0 jasqia     (502) staff       (20)     1169 2023-06-13 07:07:14.000000 liveramp_automation_framework-0.1.2/setup.py
```

### Comparing `liveramp_automation_framework-0.1.1/PKG-INFO` & `liveramp_automation_framework-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liveramp_automation_framework
-Version: 0.1.1
+Version: 0.1.2
 Summary: This is the base liveramp_automation_framework
 Home-page: https://github.com/LiveRamp/qe_api_framework
 Author: Jasmine Qian
 Author-email: jasmine.qian@liveramp.com
 Description-Content-Type: text/markdown
 
 ### 1. Descprition of the repository
```

### Comparing `liveramp_automation_framework-0.1.1/liveramp_automation/logger.py` & `liveramp_automation_framework-0.1.2/liveramp_automation/logger.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation_framework-0.1.1/liveramp_automation/login_util.py` & `liveramp_automation_framework-0.1.2/liveramp_automation/login_util.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation_framework-0.1.1/liveramp_automation/parsers.py` & `liveramp_automation_framework-0.1.2/liveramp_automation/parsers.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation_framework-0.1.1/liveramp_automation/playwright_util.py` & `liveramp_automation_framework-0.1.2/liveramp_automation/playwright_util.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 class PlaywrightUtils:
 
     def __init__(self, page):
         self.page = page
 
     def navigate_url(self, scheme=None, host_name=None, path=None, query=None):
         parsed_uri = urlparse(self.page.url)
-        self.page.goto(urlunsplit((parsed_uri.scheme if scheme is None else scheme,
-                                   parsed_uri.hostname if host_name is None else host_name,
-                                   parsed_uri.path if path is None else path,
-                                   parsed_uri.query if query is None else query,
-                                   '')))
+        self.page.url.goto(urlunsplit((parsed_uri.scheme if scheme is None else scheme,
+                                       parsed_uri.hostname if host_name is None else host_name,
+                                       parsed_uri.path if path is None else path,
+                                       parsed_uri.query if query is None else query,
+                                       '')))
 
     def savescreenshot(self, name):
         name = "reports/{}_{}.png".format(MACROS["now"], name)
-        self.page.screenshot(path=name)
+        self.page.savescreenshot(path=name)
```

### Comparing `liveramp_automation_framework-0.1.1/liveramp_automation/read_report.py` & `liveramp_automation_framework-0.1.2/liveramp_automation/read_report.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation_framework-0.1.1/liveramp_automation/request_util.py` & `liveramp_automation_framework-0.1.2/liveramp_automation/request_util.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation_framework-0.1.1/liveramp_automation/selenium_util.py` & `liveramp_automation_framework-0.1.2/liveramp_automation/selenium_util.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation_framework-0.1.1/liveramp_automation/time_util.py` & `liveramp_automation_framework-0.1.2/liveramp_automation/time_util.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation_framework-0.1.1/liveramp_automation/upload_util.py` & `liveramp_automation_framework-0.1.2/liveramp_automation/upload_util.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation_framework-0.1.1/liveramp_automation_framework.egg-info/PKG-INFO` & `liveramp_automation_framework-0.1.2/liveramp_automation_framework.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liveramp-automation-framework
-Version: 0.1.1
+Version: 0.1.2
 Summary: This is the base liveramp_automation_framework
 Home-page: https://github.com/LiveRamp/qe_api_framework
 Author: Jasmine Qian
 Author-email: jasmine.qian@liveramp.com
 Description-Content-Type: text/markdown
 
 ### 1. Descprition of the repository
```

### Comparing `liveramp_automation_framework-0.1.1/liveramp_automation_framework.egg-info/SOURCES.txt` & `liveramp_automation_framework-0.1.2/liveramp_automation_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `liveramp_automation_framework-0.1.1/setup.py` & `liveramp_automation_framework-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("readme.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='liveramp_automation_framework',
-    version='0.1.1',
+    version='0.1.2',
     author='Jasmine Qian',
     author_email='jasmine.qian@liveramp.com',
     description="This is the base liveramp_automation_framework",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/LiveRamp/qe_api_framework",
     packages=['liveramp_automation'],
```

