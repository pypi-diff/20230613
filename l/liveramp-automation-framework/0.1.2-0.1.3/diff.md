# Comparing `tmp/liveramp_automation_framework-0.1.2.tar.gz` & `tmp/liveramp_automation_framework-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liveramp_automation_framework-0.1.2.tar", last modified: Tue Jun 13 07:07:17 2023, max compression
+gzip compressed data, was "liveramp_automation_framework-0.1.3.tar", last modified: Tue Jun 13 07:16:30 2023, max compression
```

## Comparing `liveramp_automation_framework-0.1.2.tar` & `liveramp_automation_framework-0.1.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-06-13 07:07:17.578268 liveramp_automation_framework-0.1.2/
--rw-r--r--   0 jasqia     (502) staff       (20)      818 2023-06-13 07:07:17.577787 liveramp_automation_framework-0.1.2/PKG-INFO
-drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-06-13 07:07:17.572404 liveramp_automation_framework-0.1.2/liveramp_automation/
--rw-r--r--   0 jasqia     (502) staff       (20)      271 2023-06-08 08:16:59.000000 liveramp_automation_framework-0.1.2/liveramp_automation/allure_util.py
--rw-r--r--   0 jasqia     (502) staff       (20)      928 2023-06-08 08:26:48.000000 liveramp_automation_framework-0.1.2/liveramp_automation/logger.py
--rw-r--r--   0 jasqia     (502) staff       (20)     3120 2023-06-12 02:49:19.000000 liveramp_automation_framework-0.1.2/liveramp_automation/login_util.py
--rw-r--r--   0 jasqia     (502) staff       (20)      713 2023-05-03 08:30:53.000000 liveramp_automation_framework-0.1.2/liveramp_automation/parsers.py
--rw-r--r--   0 jasqia     (502) staff       (20)      842 2023-06-13 07:07:14.000000 liveramp_automation_framework-0.1.2/liveramp_automation/playwright_util.py
--rw-r--r--   0 jasqia     (502) staff       (20)     2317 2023-06-12 02:49:19.000000 liveramp_automation_framework-0.1.2/liveramp_automation/read_report.py
--rw-r--r--   0 jasqia     (502) staff       (20)     6985 2023-06-12 02:49:19.000000 liveramp_automation_framework-0.1.2/liveramp_automation/request_util.py
--rw-r--r--   0 jasqia     (502) staff       (20)      836 2023-06-12 02:49:19.000000 liveramp_automation_framework-0.1.2/liveramp_automation/selenium_util.py
--rw-r--r--   0 jasqia     (502) staff       (20)      781 2023-06-08 08:16:59.000000 liveramp_automation_framework-0.1.2/liveramp_automation/time_util.py
--rw-r--r--   0 jasqia     (502) staff       (20)     1736 2023-06-13 06:32:14.000000 liveramp_automation_framework-0.1.2/liveramp_automation/upload_util.py
-drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-06-13 07:07:17.577003 liveramp_automation_framework-0.1.2/liveramp_automation_framework.egg-info/
--rw-r--r--   0 jasqia     (502) staff       (20)      818 2023-06-13 07:07:17.000000 liveramp_automation_framework-0.1.2/liveramp_automation_framework.egg-info/PKG-INFO
--rw-r--r--   0 jasqia     (502) staff       (20)      617 2023-06-13 07:07:17.000000 liveramp_automation_framework-0.1.2/liveramp_automation_framework.egg-info/SOURCES.txt
--rw-r--r--   0 jasqia     (502) staff       (20)        1 2023-06-13 07:07:17.000000 liveramp_automation_framework-0.1.2/liveramp_automation_framework.egg-info/dependency_links.txt
--rw-r--r--   0 jasqia     (502) staff       (20)      381 2023-06-13 07:07:17.000000 liveramp_automation_framework-0.1.2/liveramp_automation_framework.egg-info/requires.txt
--rw-r--r--   0 jasqia     (502) staff       (20)       20 2023-06-13 07:07:17.000000 liveramp_automation_framework-0.1.2/liveramp_automation_framework.egg-info/top_level.txt
--rw-r--r--   0 jasqia     (502) staff       (20)       38 2023-06-13 07:07:17.578505 liveramp_automation_framework-0.1.2/setup.cfg
--rw-r--r--   0 jasqia     (502) staff       (20)     1169 2023-06-13 07:07:14.000000 liveramp_automation_framework-0.1.2/setup.py
+drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-06-13 07:16:30.710612 liveramp_automation_framework-0.1.3/
+-rw-r--r--   0 jasqia     (502) staff       (20)      818 2023-06-13 07:16:30.710122 liveramp_automation_framework-0.1.3/PKG-INFO
+drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-06-13 07:16:30.704762 liveramp_automation_framework-0.1.3/liveramp_automation/
+-rw-r--r--   0 jasqia     (502) staff       (20)      370 2023-06-13 07:16:27.000000 liveramp_automation_framework-0.1.3/liveramp_automation/allure_util.py
+-rw-r--r--   0 jasqia     (502) staff       (20)      928 2023-06-08 08:26:48.000000 liveramp_automation_framework-0.1.3/liveramp_automation/logger.py
+-rw-r--r--   0 jasqia     (502) staff       (20)     3120 2023-06-12 02:49:19.000000 liveramp_automation_framework-0.1.3/liveramp_automation/login_util.py
+-rw-r--r--   0 jasqia     (502) staff       (20)      713 2023-05-03 08:30:53.000000 liveramp_automation_framework-0.1.3/liveramp_automation/parsers.py
+-rw-r--r--   0 jasqia     (502) staff       (20)      842 2023-06-13 07:07:14.000000 liveramp_automation_framework-0.1.3/liveramp_automation/playwright_util.py
+-rw-r--r--   0 jasqia     (502) staff       (20)     2232 2023-06-13 07:16:27.000000 liveramp_automation_framework-0.1.3/liveramp_automation/read_report.py
+-rw-r--r--   0 jasqia     (502) staff       (20)     6966 2023-06-13 07:16:27.000000 liveramp_automation_framework-0.1.3/liveramp_automation/request_util.py
+-rw-r--r--   0 jasqia     (502) staff       (20)      836 2023-06-12 02:49:19.000000 liveramp_automation_framework-0.1.3/liveramp_automation/selenium_util.py
+-rw-r--r--   0 jasqia     (502) staff       (20)      781 2023-06-08 08:16:59.000000 liveramp_automation_framework-0.1.3/liveramp_automation/time_util.py
+-rw-r--r--   0 jasqia     (502) staff       (20)      718 2023-06-13 07:16:27.000000 liveramp_automation_framework-0.1.3/liveramp_automation/upload_util.py
+drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-06-13 07:16:30.709237 liveramp_automation_framework-0.1.3/liveramp_automation_framework.egg-info/
+-rw-r--r--   0 jasqia     (502) staff       (20)      818 2023-06-13 07:16:30.000000 liveramp_automation_framework-0.1.3/liveramp_automation_framework.egg-info/PKG-INFO
+-rw-r--r--   0 jasqia     (502) staff       (20)      617 2023-06-13 07:16:30.000000 liveramp_automation_framework-0.1.3/liveramp_automation_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 jasqia     (502) staff       (20)        1 2023-06-13 07:16:30.000000 liveramp_automation_framework-0.1.3/liveramp_automation_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 jasqia     (502) staff       (20)      381 2023-06-13 07:16:30.000000 liveramp_automation_framework-0.1.3/liveramp_automation_framework.egg-info/requires.txt
+-rw-r--r--   0 jasqia     (502) staff       (20)       20 2023-06-13 07:16:30.000000 liveramp_automation_framework-0.1.3/liveramp_automation_framework.egg-info/top_level.txt
+-rw-r--r--   0 jasqia     (502) staff       (20)       38 2023-06-13 07:16:30.710810 liveramp_automation_framework-0.1.3/setup.cfg
+-rw-r--r--   0 jasqia     (502) staff       (20)     1169 2023-06-13 07:16:27.000000 liveramp_automation_framework-0.1.3/setup.py
```

### Comparing `liveramp_automation_framework-0.1.2/PKG-INFO` & `liveramp_automation_framework-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liveramp_automation_framework
-Version: 0.1.2
+Version: 0.1.3
 Summary: This is the base liveramp_automation_framework
 Home-page: https://github.com/LiveRamp/qe_api_framework
 Author: Jasmine Qian
 Author-email: jasmine.qian@liveramp.com
 Description-Content-Type: text/markdown
 
 ### 1. Descprition of the repository
```

### Comparing `liveramp_automation_framework-0.1.2/liveramp_automation/logger.py` & `liveramp_automation_framework-0.1.3/liveramp_automation/logger.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation_framework-0.1.2/liveramp_automation/login_util.py` & `liveramp_automation_framework-0.1.3/liveramp_automation/login_util.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation_framework-0.1.2/liveramp_automation/parsers.py` & `liveramp_automation_framework-0.1.3/liveramp_automation/parsers.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation_framework-0.1.2/liveramp_automation/playwright_util.py` & `liveramp_automation_framework-0.1.3/liveramp_automation/playwright_util.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation_framework-0.1.2/liveramp_automation/read_report.py` & `liveramp_automation_framework-0.1.3/liveramp_automation/read_report.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,11 +59,7 @@
             print('Exit code 1')
             print(1)
             Logger.info("Some test cases run failed")
         elif errors != 0:
             print('Exit code 3')
             print(3)
             Logger.info("Some scripts have issues and please check")
-
-
-if __name__ == '__main__':
-    Report.read_junit_xml_report("./reports/junit.xml")
```

### Comparing `liveramp_automation_framework-0.1.2/liveramp_automation/request_util.py` & `liveramp_automation_framework-0.1.3/liveramp_automation/request_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import requests
-from liveramp_automation.allure_util import allure_attach_text
+from liveramp_automation.allure_util import *
 from liveramp_automation.logger import Logger
 
 
 def request_post(url, headers, data=None, json=None):
     Logger.info("The url infomation is {}".format(url))
     Logger.info("The request method is POST")
     allure_attach_text("The url infomation is {}".format(url), "URL")
     allure_attach_text("The request method is POST", "Method")
     if data:
         Logger.info("The request data infomation is {}".format(data))
         allure_attach_text(data, "The request data infomation is as the following." )
     if json:
         Logger.info("The json in request body is {}".format(json))
-        allure_attach_text("The json in request body is:", json)
+        allure_attach_json("The json in request body is:", json)
     try:
         response = requests.post(url=url, data=data, json=json, headers=headers)
         Logger.info("The response infomation is {}".format(response.text))
         allure_attach_text(response.text,"The response infomation is as the following.")
     except requests.exceptions.HTTPError as error:
         Logger.info("HTTP error occurred {}".format(error))
     except requests.exceptions.Timeout as error:
@@ -31,15 +31,15 @@
     Logger.info("The url infomation is {}".format(url))
     Logger.info("The request method is GET")
     allure_attach_text("The url infomation is {}".format(url), "URL")
     allure_attach_text("The request method is GET", "Method")
     if data:
         Logger.info("The request data infomation is {}".format(data))
     if json:
-        Logger.info("The json in request body is {}".format(json))
+        allure_attach_json("The json in request body is:", json)
     try:
         response = requests.get(url=url, data=data, json=json, headers=headers)
         Logger.info("The response infomation is {}".format(response.text))
     except requests.exceptions.HTTPError as error:
         Logger.info("HTTP error occurred {}".format(error))
     except requests.exceptions.Timeout as error:
         Logger.info("Request timed out {}".format(error))
```

### Comparing `liveramp_automation_framework-0.1.2/liveramp_automation/selenium_util.py` & `liveramp_automation_framework-0.1.3/liveramp_automation/selenium_util.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation_framework-0.1.2/liveramp_automation/time_util.py` & `liveramp_automation_framework-0.1.3/liveramp_automation/time_util.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation_framework-0.1.2/liveramp_automation_framework.egg-info/PKG-INFO` & `liveramp_automation_framework-0.1.3/liveramp_automation_framework.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liveramp-automation-framework
-Version: 0.1.2
+Version: 0.1.3
 Summary: This is the base liveramp_automation_framework
 Home-page: https://github.com/LiveRamp/qe_api_framework
 Author: Jasmine Qian
 Author-email: jasmine.qian@liveramp.com
 Description-Content-Type: text/markdown
 
 ### 1. Descprition of the repository
```

### Comparing `liveramp_automation_framework-0.1.2/liveramp_automation_framework.egg-info/SOURCES.txt` & `liveramp_automation_framework-0.1.3/liveramp_automation_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `liveramp_automation_framework-0.1.2/setup.py` & `liveramp_automation_framework-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("readme.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='liveramp_automation_framework',
-    version='0.1.2',
+    version='0.1.3',
     author='Jasmine Qian',
     author_email='jasmine.qian@liveramp.com',
     description="This is the base liveramp_automation_framework",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/LiveRamp/qe_api_framework",
     packages=['liveramp_automation'],
```

