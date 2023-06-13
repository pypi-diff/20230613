# Comparing `tmp/selenium-simplified-0.3.tar.gz` & `tmp/selenium-simplified-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selenium-simplified-0.3.tar", last modified: Tue Jun 13 13:36:43 2023, max compression
+gzip compressed data, was "selenium-simplified-0.4.tar", last modified: Tue Jun 13 13:39:15 2023, max compression
```

## Comparing `selenium-simplified-0.3.tar` & `selenium-simplified-0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 13:36:43.642880 selenium-simplified-0.3/
--rw-rw-rw-   0        0        0     2794 2023-06-13 13:36:43.642880 selenium-simplified-0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2314 2023-06-13 13:35:12.000000 selenium-simplified-0.3/README.md
--rw-rw-rw-   0        0        0       97 2023-06-12 17:04:36.000000 selenium-simplified-0.3/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-06-13 13:36:43.641858 selenium-simplified-0.3/selenium_simplified.egg-info/
--rw-rw-rw-   0        0        0     2794 2023-06-13 13:36:43.000000 selenium-simplified-0.3/selenium_simplified.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-06-13 13:36:43.000000 selenium-simplified-0.3/selenium_simplified.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 13:36:43.000000 selenium-simplified-0.3/selenium_simplified.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-13 13:36:43.000000 selenium-simplified-0.3/selenium_simplified.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-13 13:36:43.000000 selenium-simplified-0.3/selenium_simplified.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-13 13:36:43.650106 selenium-simplified-0.3/setup.cfg
--rw-rw-rw-   0        0        0      787 2023-06-13 13:36:08.000000 selenium-simplified-0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-13 13:36:43.642880 selenium-simplified-0.3/simplified/
--rw-rw-rw-   0        0        0      990 2023-06-12 05:05:49.000000 selenium-simplified-0.3/simplified/UserActivities.py
--rw-rw-rw-   0        0        0     1411 2023-06-13 05:29:04.000000 selenium-simplified-0.3/simplified/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 13:39:15.497128 selenium-simplified-0.4/
+-rw-rw-rw-   0        0        0     2796 2023-06-13 13:39:15.497128 selenium-simplified-0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2316 2023-06-13 13:38:17.000000 selenium-simplified-0.4/README.md
+-rw-rw-rw-   0        0        0       97 2023-06-12 17:04:36.000000 selenium-simplified-0.4/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-06-13 13:39:15.490115 selenium-simplified-0.4/selenium_simplified.egg-info/
+-rw-rw-rw-   0        0        0     2796 2023-06-13 13:39:15.000000 selenium-simplified-0.4/selenium_simplified.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-06-13 13:39:15.000000 selenium-simplified-0.4/selenium_simplified.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 13:39:15.000000 selenium-simplified-0.4/selenium_simplified.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-13 13:39:15.000000 selenium-simplified-0.4/selenium_simplified.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-13 13:39:15.000000 selenium-simplified-0.4/selenium_simplified.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-13 13:39:15.497128 selenium-simplified-0.4/setup.cfg
+-rw-rw-rw-   0        0        0      787 2023-06-13 13:38:35.000000 selenium-simplified-0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 13:39:15.497128 selenium-simplified-0.4/simplified/
+-rw-rw-rw-   0        0        0      990 2023-06-12 05:05:49.000000 selenium-simplified-0.4/simplified/UserActivities.py
+-rw-rw-rw-   0        0        0     1411 2023-06-13 05:29:04.000000 selenium-simplified-0.4/simplified/__init__.py
```

### Comparing `selenium-simplified-0.3/PKG-INFO` & `selenium-simplified-0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: selenium-simplified
-Version: 0.3
+Version: 0.4
 Summary: A free, open-source web automation library for the Chrome browser using Selenium Python
 Home-page: https://github.com/raajrajnish/SeleniumSimplified.git
 Author: rajnish kumar
 Author-email: raajrajnish@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 # SeleniumSimplified 
 <p align="center">
   <img src="https://github.com/raajrajnish/SeleniumSimplified/blob/master/assets/Se.png?raw=true" alt="Logo-SeleniumSimplified" height=300 width=300/>
 </p>
+
 A free, open-source web automation library for the Chrome browser using Selenium Python.
 
 ### Description
 This library is created keeping those developers in mind who wish to automate their website for a task but do not wish to spend an excessive amount of time learning a new library.We made every effort when creating this toolkit to make web automation as simple and efficient as possible. This library's backend is the Python client for [Selenium](https://www.selenium.dev/). Selenium is the standard library for web automation and is quite powerful.
 
 In order to make things simple and easy to understand for anyone with a background in selenium, we have made an effort to keep the function name as close to the original selenium functions as possible.
```

### Comparing `selenium-simplified-0.3/README.md` & `selenium-simplified-0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # SeleniumSimplified 
 <p align="center">
   <img src="https://github.com/raajrajnish/SeleniumSimplified/blob/master/assets/Se.png?raw=true" alt="Logo-SeleniumSimplified" height=300 width=300/>
 </p>
+
 A free, open-source web automation library for the Chrome browser using Selenium Python.
 
 ### Description
 This library is created keeping those developers in mind who wish to automate their website for a task but do not wish to spend an excessive amount of time learning a new library.We made every effort when creating this toolkit to make web automation as simple and efficient as possible. This library's backend is the Python client for [Selenium](https://www.selenium.dev/). Selenium is the standard library for web automation and is quite powerful.
 
 In order to make things simple and easy to understand for anyone with a background in selenium, we have made an effort to keep the function name as close to the original selenium functions as possible.
```

### Comparing `selenium-simplified-0.3/selenium_simplified.egg-info/PKG-INFO` & `selenium-simplified-0.4/selenium_simplified.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: selenium-simplified
-Version: 0.3
+Version: 0.4
 Summary: A free, open-source web automation library for the Chrome browser using Selenium Python
 Home-page: https://github.com/raajrajnish/SeleniumSimplified.git
 Author: rajnish kumar
 Author-email: raajrajnish@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 # SeleniumSimplified 
 <p align="center">
   <img src="https://github.com/raajrajnish/SeleniumSimplified/blob/master/assets/Se.png?raw=true" alt="Logo-SeleniumSimplified" height=300 width=300/>
 </p>
+
 A free, open-source web automation library for the Chrome browser using Selenium Python.
 
 ### Description
 This library is created keeping those developers in mind who wish to automate their website for a task but do not wish to spend an excessive amount of time learning a new library.We made every effort when creating this toolkit to make web automation as simple and efficient as possible. This library's backend is the Python client for [Selenium](https://www.selenium.dev/). Selenium is the standard library for web automation and is quite powerful.
 
 In order to make things simple and easy to understand for anyone with a background in selenium, we have made an effort to keep the function name as close to the original selenium functions as possible.
```

### Comparing `selenium-simplified-0.3/setup.py` & `selenium-simplified-0.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="selenium-simplified",
-    version="0.3",
+    version="0.4",
     author="rajnish kumar",
     author_email="raajrajnish@gmail.com",
     description="A free, open-source web automation library for the Chrome browser using Selenium Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/raajrajnish/SeleniumSimplified.git",
     packages=setuptools.find_packages(),
```

### Comparing `selenium-simplified-0.3/simplified/UserActivities.py` & `selenium-simplified-0.4/simplified/UserActivities.py`

 * *Files identical despite different names*

### Comparing `selenium-simplified-0.3/simplified/__init__.py` & `selenium-simplified-0.4/simplified/__init__.py`

 * *Files identical despite different names*

