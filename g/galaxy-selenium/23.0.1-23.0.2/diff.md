# Comparing `tmp/galaxy-selenium-23.0.1.tar.gz` & `tmp/galaxy-selenium-23.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/galaxy/galaxy/packages/selenium/dist/.tmp-qu3m6_t1/galaxy-selenium-23.0.1.tar", last modified: Thu Jun  8 17:41:57 2023, max compression
+gzip compressed data, was "/home/runner/work/galaxy/galaxy/packages/selenium/dist/.tmp-le8wyi7_/galaxy-selenium-23.0.2.tar", last modified: Tue Jun 13 17:09:42 2023, max compression
```

## Comparing `galaxy-selenium-23.0.1.tar` & `galaxy-selenium-23.0.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:41:57.000000 galaxy-selenium-23.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-08 17:37:04.000000 galaxy-selenium-23.0.1/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12875 2023-06-08 17:37:03.000000 galaxy-selenium-23.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-08 17:37:04.000000 galaxy-selenium-23.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-06-08 17:41:57.000000 galaxy-selenium-23.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-08 17:37:04.000000 galaxy-selenium-23.0.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-08 17:37:04.000000 galaxy-selenium-23.0.1/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:41:56.000000 galaxy-selenium-23.0.1/galaxy/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-08 17:37:04.000000 galaxy-selenium-23.0.1/galaxy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 17:37:04.000000 galaxy-selenium-23.0.1/galaxy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:41:57.000000 galaxy-selenium-23.0.1/galaxy/selenium/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-08 17:37:04.000000 galaxy-selenium-23.0.1/galaxy/selenium/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-06-08 17:37:04.000000 galaxy-selenium-23.0.1/galaxy/selenium/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-06-08 17:37:04.000000 galaxy-selenium-23.0.1/galaxy/selenium/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-06-08 17:37:04.000000 galaxy-selenium-23.0.1/galaxy/selenium/driver_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    11208 2023-06-08 17:37:04.000000 galaxy-selenium-23.0.1/galaxy/selenium/has_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-08 17:37:04.000000 galaxy-selenium-23.0.1/galaxy/selenium/jupyter_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    88548 2023-06-08 17:37:04.000000 galaxy-selenium-23.0.1/galaxy/selenium/navigates_galaxy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:41:57.000000 galaxy-selenium-23.0.1/galaxy/selenium/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 17:37:04.000000 galaxy-selenium-23.0.1/galaxy/selenium/scripts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1435 2023-06-08 17:37:04.000000 galaxy-selenium-23.0.1/galaxy/selenium/scripts/dump_tour.py
--rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-06-08 17:37:04.000000 galaxy-selenium-23.0.1/galaxy/selenium/sizzle.py
--rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-06-08 17:37:04.000000 galaxy-selenium-23.0.1/galaxy/selenium/smart_components.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:41:57.000000 galaxy-selenium-23.0.1/galaxy/selenium/toolbox/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 17:37:04.000000 galaxy-selenium-23.0.1/galaxy/selenium/toolbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-08 17:37:04.000000 galaxy-selenium-23.0.1/galaxy/selenium/toolbox/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:41:57.000000 galaxy-selenium-23.0.1/galaxy_selenium.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-06-08 17:41:56.000000 galaxy-selenium-23.0.1/galaxy_selenium.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-08 17:41:56.000000 galaxy-selenium-23.0.1/galaxy_selenium.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 17:41:56.000000 galaxy-selenium-23.0.1/galaxy_selenium.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-08 17:41:56.000000 galaxy-selenium-23.0.1/galaxy_selenium.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-08 17:41:56.000000 galaxy-selenium-23.0.1/galaxy_selenium.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-08 17:41:56.000000 galaxy-selenium-23.0.1/galaxy_selenium.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-08 17:37:04.000000 galaxy-selenium-23.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-08 17:41:57.000000 galaxy-selenium-23.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-08 17:37:04.000000 galaxy-selenium-23.0.1/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:09:42.000000 galaxy-selenium-23.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-06-13 17:04:37.000000 galaxy-selenium-23.0.2/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12875 2023-06-13 17:04:36.000000 galaxy-selenium-23.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-13 17:04:37.000000 galaxy-selenium-23.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-06-13 17:09:42.000000 galaxy-selenium-23.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-13 17:04:37.000000 galaxy-selenium-23.0.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-13 17:04:37.000000 galaxy-selenium-23.0.2/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:09:42.000000 galaxy-selenium-23.0.2/galaxy/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-13 17:04:37.000000 galaxy-selenium-23.0.2/galaxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 17:04:37.000000 galaxy-selenium-23.0.2/galaxy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:09:42.000000 galaxy-selenium-23.0.2/galaxy/selenium/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-13 17:04:37.000000 galaxy-selenium-23.0.2/galaxy/selenium/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-06-13 17:04:37.000000 galaxy-selenium-23.0.2/galaxy/selenium/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-06-13 17:04:37.000000 galaxy-selenium-23.0.2/galaxy/selenium/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-06-13 17:04:37.000000 galaxy-selenium-23.0.2/galaxy/selenium/driver_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11208 2023-06-13 17:04:37.000000 galaxy-selenium-23.0.2/galaxy/selenium/has_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-13 17:04:37.000000 galaxy-selenium-23.0.2/galaxy/selenium/jupyter_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88548 2023-06-13 17:04:37.000000 galaxy-selenium-23.0.2/galaxy/selenium/navigates_galaxy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:09:42.000000 galaxy-selenium-23.0.2/galaxy/selenium/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 17:04:37.000000 galaxy-selenium-23.0.2/galaxy/selenium/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1435 2023-06-13 17:04:37.000000 galaxy-selenium-23.0.2/galaxy/selenium/scripts/dump_tour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-06-13 17:04:37.000000 galaxy-selenium-23.0.2/galaxy/selenium/sizzle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-06-13 17:04:37.000000 galaxy-selenium-23.0.2/galaxy/selenium/smart_components.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:09:42.000000 galaxy-selenium-23.0.2/galaxy/selenium/toolbox/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 17:04:37.000000 galaxy-selenium-23.0.2/galaxy/selenium/toolbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-13 17:04:37.000000 galaxy-selenium-23.0.2/galaxy/selenium/toolbox/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:09:42.000000 galaxy-selenium-23.0.2/galaxy_selenium.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-06-13 17:09:42.000000 galaxy-selenium-23.0.2/galaxy_selenium.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-13 17:09:42.000000 galaxy-selenium-23.0.2/galaxy_selenium.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 17:09:42.000000 galaxy-selenium-23.0.2/galaxy_selenium.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-13 17:09:42.000000 galaxy-selenium-23.0.2/galaxy_selenium.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-13 17:09:42.000000 galaxy-selenium-23.0.2/galaxy_selenium.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-13 17:09:42.000000 galaxy-selenium-23.0.2/galaxy_selenium.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-13 17:04:37.000000 galaxy-selenium-23.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-13 17:09:42.000000 galaxy-selenium-23.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-13 17:04:37.000000 galaxy-selenium-23.0.2/test-requirements.txt
```

### Comparing `galaxy-selenium-23.0.1/HISTORY.rst` & `galaxy-selenium-23.0.2/HISTORY.rst`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,24 @@
 History
 -------
 
 .. to_doc
 
 -------------------
+23.0.2 (2023-06-13)
+-------------------
+
+
+============
+Enhancements
+============
+
+* Port selenium setup to non-deprecated selenium options by `@mvdbeek <https://github.com/mvdbeek>`_ in `#16215 <https://github.com/galaxyproject/galaxy/pull/16215>`_
+
+-------------------
 23.0.1 (2023-06-08)
 -------------------
 
 
 ============
 Enhancements
 ============
```

### Comparing `galaxy-selenium-23.0.1/LICENSE` & `galaxy-selenium-23.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `galaxy-selenium-23.0.1/PKG-INFO` & `galaxy-selenium-23.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-selenium
-Version: 23.0.1
+Version: 23.0.2
 Summary: Galaxy Selenium interaction framework
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -43,14 +43,25 @@
 
 History
 -------
 
 .. to_doc
 
 -------------------
+23.0.2 (2023-06-13)
+-------------------
+
+
+============
+Enhancements
+============
+
+* Port selenium setup to non-deprecated selenium options by `@mvdbeek <https://github.com/mvdbeek>`_ in `#16215 <https://github.com/galaxyproject/galaxy/pull/16215>`_
+
+-------------------
 23.0.1 (2023-06-08)
 -------------------
 
 
 ============
 Enhancements
 ============
```

### Comparing `galaxy-selenium-23.0.1/galaxy/selenium/cli.py` & `galaxy-selenium-23.0.2/galaxy/selenium/cli.py`

 * *Files identical despite different names*

### Comparing `galaxy-selenium-23.0.1/galaxy/selenium/context.py` & `galaxy-selenium-23.0.2/galaxy/selenium/context.py`

 * *Files identical despite different names*

### Comparing `galaxy-selenium-23.0.1/galaxy/selenium/driver_factory.py` & `galaxy-selenium-23.0.2/galaxy/selenium/driver_factory.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import logging
 import os
+from typing import Union
 
 try:
     from pyvirtualdisplay import Display
 except ImportError:
     Display = None
 
 from selenium import webdriver
 from selenium.webdriver.chrome.options import Options as ChromeOptions
-from selenium.webdriver.common.desired_capabilities import DesiredCapabilities
 from selenium.webdriver.remote.webdriver import WebDriver
+from selenium.webdriver.safari.options import Options as SafariOptions
 
 logger = logging.getLogger("selenium.webdriver.remote.remote_connection")
 logger.setLevel(logging.WARNING)
 
 DEFAULT_BROWSER = "auto"
 DEFAULT_DOWNLOAD_PATH = "/tmp/"
 LOGGING_PREFS = {
@@ -86,44 +87,49 @@
         raise AssertionError(f"{browser} not in VALID_LOCAL_BROWSERS ({VALID_LOCAL_BROWSERS})")
     driver_to_class = {
         "CHROME": webdriver.Chrome,
         "FIREFOX": webdriver.Firefox,
     }
     driver_class = driver_to_class[browser]
     if browser == "CHROME":
-        options = ChromeOptions()
+        chrome_options = ChromeOptions()
         if headless:
-            options.add_argument("--headless")
+            chrome_options.add_argument("--headless")
         prefs = {"download.default_directory": DEFAULT_DOWNLOAD_PATH}
-        options.add_experimental_option("prefs", prefs)
-        return driver_class(desired_capabilities={"loggingPrefs": LOGGING_PREFS}, chrome_options=options)
-    elif browser == "FIREFOX":
-        fp = webdriver.FirefoxProfile()
-        fp.set_preference("network.proxy.type", 2)
-        fp.set_preference("network.proxy.autoconfig_url", "http://127.0.0.1:9675")
-        fp.set_preference("browser.download.folderList", 2)
-        fp.set_preference("browser.download.dir", DEFAULT_DOWNLOAD_PATH)
-        fp.set_preference("browser.helperApps.neverAsk.saveToDisk", "application/octet-stream")
-        return driver_class(firefox_profile=fp)
-
+        chrome_options.add_experimental_option("prefs", prefs)
+        chrome_options.set_capability("goog:loggingPrefs", LOGGING_PREFS)
+        return driver_class(options=chrome_options)
     else:
-        return driver_class(desired_capabilities={"loggingPrefs": LOGGING_PREFS})
+        firefox_options = webdriver.FirefoxOptions()
+        firefox_options.set_preference("network.proxy.type", 2)
+        firefox_options.set_preference("network.proxy.autoconfig_url", "http://127.0.0.1:9675")
+        firefox_options.set_preference("browser.download.folderList", 2)
+        firefox_options.set_preference("browser.download.dir", DEFAULT_DOWNLOAD_PATH)
+        firefox_options.set_preference("browser.helperApps.neverAsk.saveToDisk", "application/octet-stream")
+        return driver_class(options=firefox_options)
 
 
 def get_remote_driver(host, port, browser=DEFAULT_BROWSER) -> WebDriver:
     # docker run -d -p 4444:4444 -v /dev/shm:/dev/shm selenium/standalone-chrome:3.0.1-aluminum
-    if browser == "auto":
-        browser = "CHROME"
-    assert browser in ["CHROME", "EDGE", "ANDROID", "FIREFOX", "INTERNETEXPLORER", "IPAD", "IPHONE", "SAFARI"]
-    desired_capabilities = getattr(DesiredCapabilities, browser)
-    desired_capabilities["loggingPrefs"] = LOGGING_PREFS
+    options: Union[webdriver.ChromeOptions, webdriver.FirefoxOptions, webdriver.EdgeOptions, SafariOptions]
+    if browser == "auto" or browser == "CHROME":
+        options = webdriver.ChromeOptions()
+        options.set_capability("goog:loggingPrefs", LOGGING_PREFS)
+    elif browser == "FIREFOX":
+        options = webdriver.FirefoxOptions()
+    elif browser == "EDGE":
+        options = webdriver.EdgeOptions()
+    elif browser == "SAFARI":
+        options = SafariOptions()
+    else:
+        raise Exception(f"Browser '{browser}' not supported.")
     executor = f"http://{host}:{port}/wd/hub"
     driver = webdriver.Remote(
         command_executor=executor,
-        desired_capabilities=desired_capabilities,
+        options=options,
     )
     return driver
 
 
 def is_virtual_display_available():
     return Display is not None
```

### Comparing `galaxy-selenium-23.0.1/galaxy/selenium/has_driver.py` & `galaxy-selenium-23.0.2/galaxy/selenium/has_driver.py`

 * *Files identical despite different names*

### Comparing `galaxy-selenium-23.0.1/galaxy/selenium/navigates_galaxy.py` & `galaxy-selenium-23.0.2/galaxy/selenium/navigates_galaxy.py`

 * *Files identical despite different names*

### Comparing `galaxy-selenium-23.0.1/galaxy/selenium/scripts/dump_tour.py` & `galaxy-selenium-23.0.2/galaxy/selenium/scripts/dump_tour.py`

 * *Files identical despite different names*

### Comparing `galaxy-selenium-23.0.1/galaxy/selenium/sizzle.py` & `galaxy-selenium-23.0.2/galaxy/selenium/sizzle.py`

 * *Files identical despite different names*

### Comparing `galaxy-selenium-23.0.1/galaxy/selenium/smart_components.py` & `galaxy-selenium-23.0.2/galaxy/selenium/smart_components.py`

 * *Files identical despite different names*

### Comparing `galaxy-selenium-23.0.1/galaxy_selenium.egg-info/PKG-INFO` & `galaxy-selenium-23.0.2/galaxy_selenium.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-selenium
-Version: 23.0.1
+Version: 23.0.2
 Summary: Galaxy Selenium interaction framework
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -43,14 +43,25 @@
 
 History
 -------
 
 .. to_doc
 
 -------------------
+23.0.2 (2023-06-13)
+-------------------
+
+
+============
+Enhancements
+============
+
+* Port selenium setup to non-deprecated selenium options by `@mvdbeek <https://github.com/mvdbeek>`_ in `#16215 <https://github.com/galaxyproject/galaxy/pull/16215>`_
+
+-------------------
 23.0.1 (2023-06-08)
 -------------------
 
 
 ============
 Enhancements
 ============
```

### Comparing `galaxy-selenium-23.0.1/galaxy_selenium.egg-info/SOURCES.txt` & `galaxy-selenium-23.0.2/galaxy_selenium.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `galaxy-selenium-23.0.1/setup.cfg` & `galaxy-selenium-23.0.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 license = AFL
 license_files = 
 	LICENSE
 long_description = file: README.rst, HISTORY.rst
 long_description_content_type = text/x-rst
 name = galaxy-selenium
 url = https://github.com/galaxyproject/galaxy
-version = 23.0.1
+version = 23.0.2
 
 [options]
 include_package_data = True
 install_requires = 
 	galaxy-navigation
 	galaxy-util
 	PyYAML
```

