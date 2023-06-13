# Comparing `tmp/visokio_omniprint-1.0.2.tar.gz` & `tmp/visokio_omniprint-1.1.1.tar.gz`

## Comparing `visokio_omniprint-1.0.2.tar` & `visokio_omniprint-1.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rwxr-xr-x   0        0        0       22 2020-02-02 00:00:00.000000 visokio_omniprint-1.0.2/scripts/build.sh
--rwxr-xr-x   0        0        0       46 2020-02-02 00:00:00.000000 visokio_omniprint-1.0.2/scripts/install.sh
--rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 visokio_omniprint-1.0.2/scripts/test_install.sh
--rwxr-xr-x   0        0        0       42 2020-02-02 00:00:00.000000 visokio_omniprint-1.0.2/scripts/test_upload.sh
--rwxr-xr-x   0        0        0       20 2020-02-02 00:00:00.000000 visokio_omniprint-1.0.2/scripts/upload.sh
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 visokio_omniprint-1.0.2/tests/__init__.py
--rw-r--r--   0        0        0     4969 2020-02-02 00:00:00.000000 visokio_omniprint-1.0.2/visokio_omniprint/DriverBase.py
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 visokio_omniprint-1.0.2/visokio_omniprint/Image.py
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 visokio_omniprint-1.0.2/visokio_omniprint/ImagesPdf.py
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 visokio_omniprint-1.0.2/visokio_omniprint/Pdf.py
--rw-r--r--   0        0        0     3174 2020-02-02 00:00:00.000000 visokio_omniprint-1.0.2/visokio_omniprint/Tools.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 visokio_omniprint-1.0.2/visokio_omniprint/__about__.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 visokio_omniprint-1.0.2/visokio_omniprint/__init__.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 visokio_omniprint-1.0.2/.gitignore
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 visokio_omniprint-1.0.2/LICENSE
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 visokio_omniprint-1.0.2/README.md
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 visokio_omniprint-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 visokio_omniprint-1.0.2/PKG-INFO
+-rwxr-xr-x   0        0        0       22 2020-02-02 00:00:00.000000 visokio_omniprint-1.1.1/scripts/build.sh
+-rwxr-xr-x   0        0        0       46 2020-02-02 00:00:00.000000 visokio_omniprint-1.1.1/scripts/install.sh
+-rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 visokio_omniprint-1.1.1/scripts/test_install.sh
+-rwxr-xr-x   0        0        0       42 2020-02-02 00:00:00.000000 visokio_omniprint-1.1.1/scripts/test_upload.sh
+-rwxr-xr-x   0        0        0       20 2020-02-02 00:00:00.000000 visokio_omniprint-1.1.1/scripts/upload.sh
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 visokio_omniprint-1.1.1/tests/__init__.py
+-rw-r--r--   0        0        0     5107 2020-02-02 00:00:00.000000 visokio_omniprint-1.1.1/visokio_omniprint/DriverBase.py
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 visokio_omniprint-1.1.1/visokio_omniprint/Image.py
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 visokio_omniprint-1.1.1/visokio_omniprint/ImagesPdf.py
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 visokio_omniprint-1.1.1/visokio_omniprint/Pdf.py
+-rw-r--r--   0        0        0     3174 2020-02-02 00:00:00.000000 visokio_omniprint-1.1.1/visokio_omniprint/Tools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 visokio_omniprint-1.1.1/visokio_omniprint/__about__.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 visokio_omniprint-1.1.1/visokio_omniprint/__init__.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 visokio_omniprint-1.1.1/.gitignore
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 visokio_omniprint-1.1.1/LICENSE
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 visokio_omniprint-1.1.1/README.md
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 visokio_omniprint-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 visokio_omniprint-1.1.1/PKG-INFO
```

### Comparing `visokio_omniprint-1.0.2/visokio_omniprint/DriverBase.py` & `visokio_omniprint-1.1.1/visokio_omniprint/DriverBase.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,22 +46,23 @@
 
 
     def get_driver_docker(self, options):
         """
         This function creates a ChromeDriver instance to be used in a Docker container.
         """
         chrome_service = Service("/chromedriver")
-        return webdriver.Chrome(service=chrome_service, options=options)
+        return webdriver.Chrome(options=options, service=chrome_service)
 
     def get_driver_host(self, options):
         """
         This function creates a ChromeDriver instance to be used on the host machine.
         """
         version = self.get_compatible_chromedriver()
-        return webdriver.Chrome(ChromeDriverManager(version=version).install(), options=options)
+        chrome_service = Service(ChromeDriverManager(version=version).install())
+        return webdriver.Chrome(options=options, service=chrome_service)
 
 
     def get_driver(self, is_docker):
         """
         This function creates and returns a ChromeDriver instance based on the provided configuration.
         """
         options = self.create_options()
@@ -100,16 +101,16 @@
             )
         except TimeoutException:
             driver.quit()
             raise Exception("App remained busy for too long")
 
         # Also wait for a further n seconds (configurable). 1 second is recommended if the app
         # supports aria-busy. Longer otherwise.
+        # TODO: reduce the default in the PDF block manifests from 3 to 1 once 2023.2.x aria-busy support becomes widely available
         try:
-            # Wait until the page is fully loaded
             WebDriverWait(driver, timeout).until(
                 staleness_of(driver.find_element(by=By.TAG_NAME, value="html"))
             )
         except TimeoutException:
             return driver
 
         driver.quit()
```

### Comparing `visokio_omniprint-1.0.2/visokio_omniprint/Image.py` & `visokio_omniprint-1.1.1/visokio_omniprint/Image.py`

 * *Files identical despite different names*

### Comparing `visokio_omniprint-1.0.2/visokio_omniprint/ImagesPdf.py` & `visokio_omniprint-1.1.1/visokio_omniprint/ImagesPdf.py`

 * *Files identical despite different names*

### Comparing `visokio_omniprint-1.0.2/visokio_omniprint/Pdf.py` & `visokio_omniprint-1.1.1/visokio_omniprint/Pdf.py`

 * *Files identical despite different names*

### Comparing `visokio_omniprint-1.0.2/visokio_omniprint/Tools.py` & `visokio_omniprint-1.1.1/visokio_omniprint/Tools.py`

 * *Files identical despite different names*

### Comparing `visokio_omniprint-1.0.2/pyproject.toml` & `visokio_omniprint-1.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "visokio-omniprint"
-version = "1.0.2"
+version = "1.1.1"
 description = "Visokio Omniscope PDF printing library"
 readme = "README.md"
 requires-python = ">=3.7"
 license = "MIT"
 keywords = []
 authors = [
   { name = "Visokio" },
```

### Comparing `visokio_omniprint-1.0.2/PKG-INFO` & `visokio_omniprint-1.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visokio-omniprint
-Version: 1.0.2
+Version: 1.1.1
 Summary: Visokio Omniscope PDF printing library
 Project-URL: Documentation, https://github.com/visokio/omniscope-custom-blocks/tree/master/visokio-omniprint#readme
 Project-URL: Issues, https://github.com/visokio/omniscope-custom-blocks/tree/master/visokio-omniprint/issues
 Project-URL: Source, https://github.com/visokio/omniscope-custom-blocks/tree/master/visokio-omniprint
 Author: Visokio
 License-Expression: MIT
 License-File: LICENSE
```

