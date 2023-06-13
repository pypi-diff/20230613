# Comparing `tmp/selenium-simplified-0.2.tar.gz` & `tmp/selenium-simplified-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selenium-simplified-0.2.tar", last modified: Tue Jun 13 13:33:09 2023, max compression
+gzip compressed data, was "selenium-simplified-0.3.tar", last modified: Tue Jun 13 13:36:43 2023, max compression
```

## Comparing `selenium-simplified-0.2.tar` & `selenium-simplified-0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 13:33:09.573601 selenium-simplified-0.2/
--rw-rw-rw-   0        0        0     2059 2023-06-13 13:33:09.573601 selenium-simplified-0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1590 2023-06-13 12:55:35.000000 selenium-simplified-0.2/README.md
--rw-rw-rw-   0        0        0       97 2023-06-12 17:04:36.000000 selenium-simplified-0.2/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-06-13 13:33:09.557920 selenium-simplified-0.2/selenium_simplified.egg-info/
--rw-rw-rw-   0        0        0     2059 2023-06-13 13:33:09.000000 selenium-simplified-0.2/selenium_simplified.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-06-13 13:33:09.000000 selenium-simplified-0.2/selenium_simplified.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 13:33:09.000000 selenium-simplified-0.2/selenium_simplified.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-13 13:33:09.000000 selenium-simplified-0.2/selenium_simplified.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-13 13:33:09.000000 selenium-simplified-0.2/selenium_simplified.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-13 13:33:09.573601 selenium-simplified-0.2/setup.cfg
--rw-rw-rw-   0        0        0      776 2023-06-13 13:32:27.000000 selenium-simplified-0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-13 13:33:09.573601 selenium-simplified-0.2/simplified/
--rw-rw-rw-   0        0        0      990 2023-06-12 05:05:49.000000 selenium-simplified-0.2/simplified/UserActivities.py
--rw-rw-rw-   0        0        0     1411 2023-06-13 05:29:04.000000 selenium-simplified-0.2/simplified/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 13:36:43.642880 selenium-simplified-0.3/
+-rw-rw-rw-   0        0        0     2794 2023-06-13 13:36:43.642880 selenium-simplified-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2314 2023-06-13 13:35:12.000000 selenium-simplified-0.3/README.md
+-rw-rw-rw-   0        0        0       97 2023-06-12 17:04:36.000000 selenium-simplified-0.3/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-06-13 13:36:43.641858 selenium-simplified-0.3/selenium_simplified.egg-info/
+-rw-rw-rw-   0        0        0     2794 2023-06-13 13:36:43.000000 selenium-simplified-0.3/selenium_simplified.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-06-13 13:36:43.000000 selenium-simplified-0.3/selenium_simplified.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 13:36:43.000000 selenium-simplified-0.3/selenium_simplified.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-13 13:36:43.000000 selenium-simplified-0.3/selenium_simplified.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-13 13:36:43.000000 selenium-simplified-0.3/selenium_simplified.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-13 13:36:43.650106 selenium-simplified-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      787 2023-06-13 13:36:08.000000 selenium-simplified-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 13:36:43.642880 selenium-simplified-0.3/simplified/
+-rw-rw-rw-   0        0        0      990 2023-06-12 05:05:49.000000 selenium-simplified-0.3/simplified/UserActivities.py
+-rw-rw-rw-   0        0        0     1411 2023-06-13 05:29:04.000000 selenium-simplified-0.3/simplified/__init__.py
```

### Comparing `selenium-simplified-0.2/PKG-INFO` & `selenium-simplified-0.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,51 @@
 Metadata-Version: 2.1
 Name: selenium-simplified
-Version: 0.2
-Summary: a better approach to do automation using simplified python on chrome browser
+Version: 0.3
+Summary: A free, open-source web automation library for the Chrome browser using Selenium Python
 Home-page: https://github.com/raajrajnish/SeleniumSimplified.git
 Author: rajnish kumar
 Author-email: raajrajnish@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
-# SeleniumSimplified
-
+# SeleniumSimplified 
+<p align="center">
+  <img src="https://github.com/raajrajnish/SeleniumSimplified/blob/master/assets/Se.png?raw=true" alt="Logo-SeleniumSimplified" height=300 width=300/>
+</p>
 A free, open-source web automation library for the Chrome browser using Selenium Python.
 
 ### Description
-This library is created keeping those developers in mind who wish to automate their website for a task but do not wish to spend an excessive amount of time learning a new library.We made every effort when creating this toolkit to make web automation as simple and efficient as possible. This library's backend is the Python client for Selenium (https://www.selenium.dev/). Selenium is the standard library for web automation and is quite powerful.
+This library is created keeping those developers in mind who wish to automate their website for a task but do not wish to spend an excessive amount of time learning a new library.We made every effort when creating this toolkit to make web automation as simple and efficient as possible. This library's backend is the Python client for [Selenium](https://www.selenium.dev/). Selenium is the standard library for web automation and is quite powerful.
 
 In order to make things simple and easy to understand for anyone with a background in selenium, we have made an effort to keep the function name as close to the original selenium functions as possible.
 
-### Advantage
-This library has below advantages when compared with others
-  1. Saves a tonne of time by preventing us from writing repetitive code because it is simple to setup and use.
-  2. There is no need to configure anything because it supports the Chrome browser out of the box; internally, everything is taken care of.
-  3. Prior to taking any action, it by default highlights the weblement (the target web element on which you wish to conduct some operations).
-  4. It makes things simpler for the user by using XPATH by default for the locator strategy.
-  5. Finally, although it is a plug-and-play library built on top of Selenium, you still get the power of Selenium when using it.
-
-
+### Advantages
+This library has below advantages
+  1. It is a plug-and-play library built on top of Selenium, you still get the power of Selenium when using it.
+  2. It supports the Chrome browser out of the box; internally, everything is taken care of.
+  3. It by default highlights the weblement (the target web element on which you wish to conduct some operations) before doing anything.
+  4. It use XPATH as a default for the locator strategy.
+  5. Saves a tonne of time by preventing us from writing repetitive code because it is simple to setup and use.
+
+### How to install
+```pip install selenium-simplified```
+
+### Example
+Below code will open chrome browser and navigate to Google home page and do a search for SeleniumSimplified
+``` 
+from simplified import *
+
+driver = SeleniumSimplified()
+driver.open_url(url='https://www.google.com')
+driver.type_in_element(xpath="//*[@name='q']",text='selenium')
+driver.click_on_element(xpath="//*[@name='btnK']")
+```
+
+### Functions Supported
+  1. ***open_url*** - Used for open a url in the chrome browser, takes one param1- as url 
+  2. ***type_in_element*** - Used for typing in input box, takes to parameter param1- xpath as locator and param2- as text
+  3. ***click_on_element*** - Used for clicking on webelement, takes one param1- as xpath
 
-https://www.freecodecamp.org/news/how-to-create-and-upload-your-first-python-package-to-pypi/
+adding more functions...
```

### Comparing `selenium-simplified-0.2/README.md` & `selenium-simplified-0.3/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,39 @@
-# SeleniumSimplified
-
+# SeleniumSimplified 
+<p align="center">
+  <img src="https://github.com/raajrajnish/SeleniumSimplified/blob/master/assets/Se.png?raw=true" alt="Logo-SeleniumSimplified" height=300 width=300/>
+</p>
 A free, open-source web automation library for the Chrome browser using Selenium Python.
 
 ### Description
-This library is created keeping those developers in mind who wish to automate their website for a task but do not wish to spend an excessive amount of time learning a new library.We made every effort when creating this toolkit to make web automation as simple and efficient as possible. This library's backend is the Python client for Selenium (https://www.selenium.dev/). Selenium is the standard library for web automation and is quite powerful.
+This library is created keeping those developers in mind who wish to automate their website for a task but do not wish to spend an excessive amount of time learning a new library.We made every effort when creating this toolkit to make web automation as simple and efficient as possible. This library's backend is the Python client for [Selenium](https://www.selenium.dev/). Selenium is the standard library for web automation and is quite powerful.
 
 In order to make things simple and easy to understand for anyone with a background in selenium, we have made an effort to keep the function name as close to the original selenium functions as possible.
 
-### Advantage
-This library has below advantages when compared with others
-  1. Saves a tonne of time by preventing us from writing repetitive code because it is simple to setup and use.
-  2. There is no need to configure anything because it supports the Chrome browser out of the box; internally, everything is taken care of.
-  3. Prior to taking any action, it by default highlights the weblement (the target web element on which you wish to conduct some operations).
-  4. It makes things simpler for the user by using XPATH by default for the locator strategy.
-  5. Finally, although it is a plug-and-play library built on top of Selenium, you still get the power of Selenium when using it.
-
-
+### Advantages
+This library has below advantages
+  1. It is a plug-and-play library built on top of Selenium, you still get the power of Selenium when using it.
+  2. It supports the Chrome browser out of the box; internally, everything is taken care of.
+  3. It by default highlights the weblement (the target web element on which you wish to conduct some operations) before doing anything.
+  4. It use XPATH as a default for the locator strategy.
+  5. Saves a tonne of time by preventing us from writing repetitive code because it is simple to setup and use.
+
+### How to install
+```pip install selenium-simplified```
+
+### Example
+Below code will open chrome browser and navigate to Google home page and do a search for SeleniumSimplified
+``` 
+from simplified import *
+
+driver = SeleniumSimplified()
+driver.open_url(url='https://www.google.com')
+driver.type_in_element(xpath="//*[@name='q']",text='selenium')
+driver.click_on_element(xpath="//*[@name='btnK']")
+```
+
+### Functions Supported
+  1. ***open_url*** - Used for open a url in the chrome browser, takes one param1- as url 
+  2. ***type_in_element*** - Used for typing in input box, takes to parameter param1- xpath as locator and param2- as text
+  3. ***click_on_element*** - Used for clicking on webelement, takes one param1- as xpath
 
-https://www.freecodecamp.org/news/how-to-create-and-upload-your-first-python-package-to-pypi/
+adding more functions...
```

### Comparing `selenium-simplified-0.2/selenium_simplified.egg-info/PKG-INFO` & `selenium-simplified-0.3/selenium_simplified.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,51 @@
 Metadata-Version: 2.1
 Name: selenium-simplified
-Version: 0.2
-Summary: a better approach to do automation using simplified python on chrome browser
+Version: 0.3
+Summary: A free, open-source web automation library for the Chrome browser using Selenium Python
 Home-page: https://github.com/raajrajnish/SeleniumSimplified.git
 Author: rajnish kumar
 Author-email: raajrajnish@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
-# SeleniumSimplified
-
+# SeleniumSimplified 
+<p align="center">
+  <img src="https://github.com/raajrajnish/SeleniumSimplified/blob/master/assets/Se.png?raw=true" alt="Logo-SeleniumSimplified" height=300 width=300/>
+</p>
 A free, open-source web automation library for the Chrome browser using Selenium Python.
 
 ### Description
-This library is created keeping those developers in mind who wish to automate their website for a task but do not wish to spend an excessive amount of time learning a new library.We made every effort when creating this toolkit to make web automation as simple and efficient as possible. This library's backend is the Python client for Selenium (https://www.selenium.dev/). Selenium is the standard library for web automation and is quite powerful.
+This library is created keeping those developers in mind who wish to automate their website for a task but do not wish to spend an excessive amount of time learning a new library.We made every effort when creating this toolkit to make web automation as simple and efficient as possible. This library's backend is the Python client for [Selenium](https://www.selenium.dev/). Selenium is the standard library for web automation and is quite powerful.
 
 In order to make things simple and easy to understand for anyone with a background in selenium, we have made an effort to keep the function name as close to the original selenium functions as possible.
 
-### Advantage
-This library has below advantages when compared with others
-  1. Saves a tonne of time by preventing us from writing repetitive code because it is simple to setup and use.
-  2. There is no need to configure anything because it supports the Chrome browser out of the box; internally, everything is taken care of.
-  3. Prior to taking any action, it by default highlights the weblement (the target web element on which you wish to conduct some operations).
-  4. It makes things simpler for the user by using XPATH by default for the locator strategy.
-  5. Finally, although it is a plug-and-play library built on top of Selenium, you still get the power of Selenium when using it.
-
-
+### Advantages
+This library has below advantages
+  1. It is a plug-and-play library built on top of Selenium, you still get the power of Selenium when using it.
+  2. It supports the Chrome browser out of the box; internally, everything is taken care of.
+  3. It by default highlights the weblement (the target web element on which you wish to conduct some operations) before doing anything.
+  4. It use XPATH as a default for the locator strategy.
+  5. Saves a tonne of time by preventing us from writing repetitive code because it is simple to setup and use.
+
+### How to install
+```pip install selenium-simplified```
+
+### Example
+Below code will open chrome browser and navigate to Google home page and do a search for SeleniumSimplified
+``` 
+from simplified import *
+
+driver = SeleniumSimplified()
+driver.open_url(url='https://www.google.com')
+driver.type_in_element(xpath="//*[@name='q']",text='selenium')
+driver.click_on_element(xpath="//*[@name='btnK']")
+```
+
+### Functions Supported
+  1. ***open_url*** - Used for open a url in the chrome browser, takes one param1- as url 
+  2. ***type_in_element*** - Used for typing in input box, takes to parameter param1- xpath as locator and param2- as text
+  3. ***click_on_element*** - Used for clicking on webelement, takes one param1- as xpath
 
-https://www.freecodecamp.org/news/how-to-create-and-upload-your-first-python-package-to-pypi/
+adding more functions...
```

### Comparing `selenium-simplified-0.2/setup.py` & `selenium-simplified-0.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="selenium-simplified",
-    version="0.2",
+    version="0.3",
     author="rajnish kumar",
     author_email="raajrajnish@gmail.com",
-    description="a better approach to do automation using simplified python on chrome browser",
+    description="A free, open-source web automation library for the Chrome browser using Selenium Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/raajrajnish/SeleniumSimplified.git",
     packages=setuptools.find_packages(),
     # packages=['simplified'],
     install_requires=['selenium'],
     classifiers=[
```

### Comparing `selenium-simplified-0.2/simplified/UserActivities.py` & `selenium-simplified-0.3/simplified/UserActivities.py`

 * *Files identical despite different names*

### Comparing `selenium-simplified-0.2/simplified/__init__.py` & `selenium-simplified-0.3/simplified/__init__.py`

 * *Files identical despite different names*

