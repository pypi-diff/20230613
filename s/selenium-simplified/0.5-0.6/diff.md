# Comparing `tmp/selenium-simplified-0.5.tar.gz` & `tmp/selenium-simplified-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selenium-simplified-0.5.tar", last modified: Tue Jun 13 13:45:27 2023, max compression
+gzip compressed data, was "selenium-simplified-0.6.tar", last modified: Tue Jun 13 17:19:17 2023, max compression
```

## Comparing `selenium-simplified-0.5.tar` & `selenium-simplified-0.6.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 13:45:27.183825 selenium-simplified-0.5/
--rw-rw-rw-   0        0        0     2804 2023-06-13 13:45:27.183825 selenium-simplified-0.5/PKG-INFO
--rw-rw-rw-   0        0        0     2324 2023-06-13 13:41:42.000000 selenium-simplified-0.5/README.md
--rw-rw-rw-   0        0        0       97 2023-06-12 17:04:36.000000 selenium-simplified-0.5/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-06-13 13:45:27.183825 selenium-simplified-0.5/selenium_simplified.egg-info/
--rw-rw-rw-   0        0        0     2804 2023-06-13 13:45:27.000000 selenium-simplified-0.5/selenium_simplified.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-06-13 13:45:27.000000 selenium-simplified-0.5/selenium_simplified.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 13:45:27.000000 selenium-simplified-0.5/selenium_simplified.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-13 13:45:27.000000 selenium-simplified-0.5/selenium_simplified.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-13 13:45:27.000000 selenium-simplified-0.5/selenium_simplified.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-13 13:45:27.183825 selenium-simplified-0.5/setup.cfg
--rw-rw-rw-   0        0        0      787 2023-06-13 13:44:53.000000 selenium-simplified-0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-13 13:45:27.183825 selenium-simplified-0.5/simplified/
--rw-rw-rw-   0        0        0      990 2023-06-12 05:05:49.000000 selenium-simplified-0.5/simplified/UserActivities.py
--rw-rw-rw-   0        0        0     1411 2023-06-13 05:29:04.000000 selenium-simplified-0.5/simplified/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 17:19:17.604597 selenium-simplified-0.6/
+-rw-rw-rw-   0        0        0     4264 2023-06-13 17:19:17.603629 selenium-simplified-0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3782 2023-06-13 17:18:33.000000 selenium-simplified-0.6/README.md
+-rw-rw-rw-   0        0        0       97 2023-06-12 17:04:36.000000 selenium-simplified-0.6/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-06-13 17:19:17.597672 selenium-simplified-0.6/selenium_simplified.egg-info/
+-rw-rw-rw-   0        0        0     4264 2023-06-13 17:19:17.000000 selenium-simplified-0.6/selenium_simplified.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      325 2023-06-13 17:19:17.000000 selenium-simplified-0.6/selenium_simplified.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 17:19:17.000000 selenium-simplified-0.6/selenium_simplified.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-13 17:19:17.000000 selenium-simplified-0.6/selenium_simplified.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-13 17:19:17.000000 selenium-simplified-0.6/selenium_simplified.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-13 17:19:17.604597 selenium-simplified-0.6/setup.cfg
+-rw-rw-rw-   0        0        0      787 2023-06-13 17:18:53.000000 selenium-simplified-0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 17:19:17.602678 selenium-simplified-0.6/simplified/
+-rw-rw-rw-   0        0        0     1566 2023-06-13 17:01:15.000000 selenium-simplified-0.6/simplified/UserActivities.py
+-rw-rw-rw-   0        0        0     1848 2023-06-13 17:01:30.000000 selenium-simplified-0.6/simplified/__init__.py
+-rw-rw-rw-   0        0        0      950 2023-06-13 17:17:38.000000 selenium-simplified-0.6/simplified/testLibrary.py
```

### Comparing `selenium-simplified-0.5/PKG-INFO` & `selenium-simplified-0.6/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: selenium-simplified
-Version: 0.5
-Summary: A free, open-source web automation library for the Chrome browser using Selenium Python
-Home-page: https://github.com/raajrajnish/SeleniumSimplified.git
-Author: rajnish kumar
-Author-email: raajrajnish@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-
 # SeleniumSimplified 
 <p align="center">
   <img src="https://github.com/raajrajnish/SeleniumSimplified/blob/master/assets/Se.png?raw=true" alt="Logo-SeleniumSimplified" height=300 width=300/>
 </p>
 
 
 ***A free, open-source web automation library for the Chrome browser using Selenium Python.***
@@ -44,10 +32,52 @@
 driver.type_in_element(xpath="//*[@name='q']",text='selenium')
 driver.click_on_element(xpath="//*[@name='btnK']")
 ```
 
 ### Functions Supported
   1. ***open_url*** - Used for open a url in the chrome browser, takes one param1- as url 
   2. ***type_in_element*** - Used for typing in input box, takes to parameter param1- xpath as locator and param2- as text
-  3. ***click_on_element*** - Used for clicking on webelement, takes one param1- as xpath
+  3. ***click_on_element*** - Used for clicking on web-element, takes one param1- as xpath
+  4. ***take_screenshot*** - Use when you have to take screenshot, take one param1 as dir (directory name)
+  5. ***get_tab_title*** - Use to get the current tab title in the browser, do not take any params
+  6. ***close_current_tab*** - Use to close the current tab in focus in the browser,do not take any params
+  7. ***close_browser*** - Use for closing the current browser instance including all tabs, do not take any params
 
 adding more functions...
+
+### Example Usage - Basic user actions
+```commandline
+# Step 1 : install the library
+# pip install selenium-simplified
+
+# Step 2: import the library
+from simplified import SeleniumSimplified
+
+# Step 3 - Open the chrome browser
+driver = SeleniumSimplified()
+
+'''
+Examples - Showing how to use SeleniumSimplified functions
+Please Note - SeleniumSimplified uses XPATH only as its locator strategy
+'''
+
+# How to open a specific url
+driver.open_url(url='https://www.google.com')
+
+# How to find an element and type some text in it
+driver.type_in_element(xpath="//*[@name='q']",text='selenium')
+
+# How to find an element and click on it
+driver.click_on_element(xpath="//*[@name='btnK']")
+
+# How to take screenshot and save it inside the screenshot directory
+driver.take_screenshot(dir='../screenshot/')
+
+# how to get the current browser tab title
+print(driver.get_tab_title())
+
+# How to close the current browser tab
+driver.close_current_tab()
+
+# How to close browser
+driver.close_browser()
+```
```

### Comparing `selenium-simplified-0.5/selenium_simplified.egg-info/PKG-INFO` & `selenium-simplified-0.6/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selenium-simplified
-Version: 0.5
+Version: 0.6
 Summary: A free, open-source web automation library for the Chrome browser using Selenium Python
 Home-page: https://github.com/raajrajnish/SeleniumSimplified.git
 Author: rajnish kumar
 Author-email: raajrajnish@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -44,10 +44,52 @@
 driver.type_in_element(xpath="//*[@name='q']",text='selenium')
 driver.click_on_element(xpath="//*[@name='btnK']")
 ```
 
 ### Functions Supported
   1. ***open_url*** - Used for open a url in the chrome browser, takes one param1- as url 
   2. ***type_in_element*** - Used for typing in input box, takes to parameter param1- xpath as locator and param2- as text
-  3. ***click_on_element*** - Used for clicking on webelement, takes one param1- as xpath
+  3. ***click_on_element*** - Used for clicking on web-element, takes one param1- as xpath
+  4. ***take_screenshot*** - Use when you have to take screenshot, take one param1 as dir (directory name)
+  5. ***get_tab_title*** - Use to get the current tab title in the browser, do not take any params
+  6. ***close_current_tab*** - Use to close the current tab in focus in the browser,do not take any params
+  7. ***close_browser*** - Use for closing the current browser instance including all tabs, do not take any params
 
 adding more functions...
+
+### Example Usage - Basic user actions
+```commandline
+# Step 1 : install the library
+# pip install selenium-simplified
+
+# Step 2: import the library
+from simplified import SeleniumSimplified
+
+# Step 3 - Open the chrome browser
+driver = SeleniumSimplified()
+
+'''
+Examples - Showing how to use SeleniumSimplified functions
+Please Note - SeleniumSimplified uses XPATH only as its locator strategy
+'''
+
+# How to open a specific url
+driver.open_url(url='https://www.google.com')
+
+# How to find an element and type some text in it
+driver.type_in_element(xpath="//*[@name='q']",text='selenium')
+
+# How to find an element and click on it
+driver.click_on_element(xpath="//*[@name='btnK']")
+
+# How to take screenshot and save it inside the screenshot directory
+driver.take_screenshot(dir='../screenshot/')
+
+# how to get the current browser tab title
+print(driver.get_tab_title())
+
+# How to close the current browser tab
+driver.close_current_tab()
+
+# How to close browser
+driver.close_browser()
+```
```

### Comparing `selenium-simplified-0.5/setup.py` & `selenium-simplified-0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="selenium-simplified",
-    version="0.5",
+    version="0.6",
     author="rajnish kumar",
     author_email="raajrajnish@gmail.com",
     description="A free, open-source web automation library for the Chrome browser using Selenium Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/raajrajnish/SeleniumSimplified.git",
     packages=setuptools.find_packages(),
```

### Comparing `selenium-simplified-0.5/simplified/UserActivities.py` & `selenium-simplified-0.6/simplified/UserActivities.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,52 @@
 from selenium.webdriver.common.by import By
 import time
+from datetime import datetime
 
 
 def highlight(element):
     """Highlights (blinks) a Selenium Webdriver element"""
     driver = element._parent
 
     def apply_style(s):
         driver.execute_script("arguments[0].setAttribute('style', arguments[1]);", element, s)
     original_style = element.get_attribute('style')
     apply_style("background: blue; border: 2px solid orange;")
     time.sleep(.3)
     apply_style(original_style)
 
 
-class CommonActivities():
+class CommonActivities:
     def __init__(self,driver):
         self.driver = driver
 
     def open_url(self, url):
         self.driver.get(url)
 
+    def get_title(self):
+        return self.driver.title
+
     def find_element(self, xpath):
-        element = self.driver.find_element(By.XPATH, xpath)
-        return element
+        return self.driver.find_element(By.XPATH, xpath)
 
     def type_in_element(self,web_element,text):
         highlight(element=web_element)
         web_element.send_keys(text)
 
     def click_on_element(self,web_element):
         highlight(element=web_element)
-        web_element.click()
+        web_element.click()
+
+    def close_current_tab(self):
+        self.driver.close()
+
+    def close_browser(self):
+        self.driver.quit()
+
+    def click_screenshot(self, dir):
+        now = datetime.now()
+        dt_string = now.strftime("%d/%m/%Y %H:%M:%S")
+        current_date = dt_string.split(" ")[0].replace('/','_')
+        current_time = dt_string.split(" ")[1].replace(':', '_')
+        file_name = current_date+'_'+current_time.replace(':','_')+".png"
+        self.driver.save_screenshot(dir+file_name)
+
```

### Comparing `selenium-simplified-0.5/simplified/__init__.py` & `selenium-simplified-0.6/simplified/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -26,12 +26,27 @@
         driver = open_chrome()
         base_functions = CommonActivities(driver)
         self.base_functions = base_functions
 
     def open_url(self, url):
         self.base_functions.open_url(url=url)
 
+    def get_tab_title(self):
+        return self.base_functions.get_title()
+
     def type_in_element(self, xpath, text):
         self.base_functions.type_in_element(web_element=self.base_functions.find_element(xpath=xpath), text=text)
 
     def click_on_element(self, xpath):
-        self.base_functions.click_on_element(web_element=self.base_functions.find_element(xpath=xpath))
+        self.base_functions.click_on_element(web_element=self.base_functions.find_element(xpath=xpath))
+
+    def web_element(self, xpath):
+        return self.base_functions.find_element(xpath=xpath)
+
+    def close_current_tab(self):
+        self.base_functions.close_current_tab()
+
+    def close_browser(self):
+        self.base_functions.close_browser()
+
+    def take_screenshot(self, dir):
+        self.base_functions.click_screenshot(dir=dir)
```

