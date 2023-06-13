# Comparing `tmp/mkdocs_exporter-3.0.3.tar.gz` & `tmp/mkdocs_exporter-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_exporter-3.0.3.tar", max compression
+gzip compressed data, was "mkdocs_exporter-3.1.0.tar", max compression
```

## Comparing `mkdocs_exporter-3.0.3.tar` & `mkdocs_exporter-3.1.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1071 2023-05-08 13:15:16.904792 mkdocs_exporter-3.0.3/LICENSE
--rw-r--r--   0        0        0     4007 2023-05-29 18:27:56.949905 mkdocs_exporter-3.0.3/README.md
--rw-r--r--   0        0        0        0 2023-05-08 15:45:32.453553 mkdocs_exporter-3.0.3/mkdocs_exporter/__init__.py
--rw-r--r--   0        0        0     1973 2023-06-02 10:45:00.862475 mkdocs_exporter-3.0.3/mkdocs_exporter/browser.py
--rw-r--r--   0        0        0      264 2023-05-30 17:10:15.899396 mkdocs_exporter-3.0.3/mkdocs_exporter/config.py
--rw-r--r--   0        0        0       96 2023-05-08 19:25:05.801769 mkdocs_exporter-3.0.3/mkdocs_exporter/logging.py
--rw-r--r--   0        0        0      543 2023-05-27 16:58:36.537218 mkdocs_exporter-3.0.3/mkdocs_exporter/page.py
--rw-r--r--   0        0        0     1935 2023-05-30 17:10:15.899396 mkdocs_exporter-3.0.3/mkdocs_exporter/plugin.py
--rw-r--r--   0        0        0        0 2023-05-06 21:44:34.488343 mkdocs_exporter-3.0.3/mkdocs_exporter/plugins/__init__.py
--rw-r--r--   0        0        0        0 2023-05-07 17:00:48.574613 mkdocs_exporter-3.0.3/mkdocs_exporter/plugins/extras/__init__.py
--rw-r--r--   0        0        0      867 2023-05-30 17:10:15.899396 mkdocs_exporter-3.0.3/mkdocs_exporter/plugins/extras/config.py
--rw-r--r--   0        0        0     1121 2023-05-30 17:10:15.899396 mkdocs_exporter-3.0.3/mkdocs_exporter/plugins/extras/plugin.py
--rw-r--r--   0        0        0        0 2023-05-07 17:48:51.834620 mkdocs_exporter-3.0.3/mkdocs_exporter/plugins/pdf/__init__.py
--rw-r--r--   0        0        0      526 2023-05-27 12:57:36.091210 mkdocs_exporter-3.0.3/mkdocs_exporter/plugins/pdf/button.py
--rw-r--r--   0        0        0     1040 2023-05-27 16:58:36.537218 mkdocs_exporter-3.0.3/mkdocs_exporter/plugins/pdf/config.py
--rw-r--r--   0        0        0     4869 2023-05-30 20:15:51.466325 mkdocs_exporter-3.0.3/mkdocs_exporter/plugins/pdf/plugin.py
--rw-r--r--   0        0        0     2181 2023-06-02 10:50:17.882385 mkdocs_exporter-3.0.3/mkdocs_exporter/plugins/pdf/renderer.py
--rw-r--r--   0        0        0     3860 2023-06-02 10:45:22.632469 mkdocs_exporter-3.0.3/mkdocs_exporter/preprocessor.py
--rw-r--r--   0        0        0      241 2023-05-07 12:23:00.605366 mkdocs_exporter-3.0.3/mkdocs_exporter/renderer.py
--rw-r--r--   0        0        0        0 2023-05-08 14:16:51.163540 mkdocs_exporter-3.0.3/mkdocs_exporter/resources/__init__.py
--rw-r--r--   0        0        0        0 2023-05-27 16:58:36.537218 mkdocs_exporter-3.0.3/mkdocs_exporter/resources/css/__init__.py
--rw-r--r--   0        0        0       93 2023-05-27 16:58:36.537218 mkdocs_exporter-3.0.3/mkdocs_exporter/resources/css/readthedocs.css
--rw-r--r--   0        0        0        0 2023-05-08 14:16:39.063540 mkdocs_exporter-3.0.3/mkdocs_exporter/resources/js/__init__.py
--rw-r--r--   0        0        0   504034 2023-05-27 16:58:36.537218 mkdocs_exporter-3.0.3/mkdocs_exporter/resources/js/pagedjs.min.js
--rw-r--r--   0        0        0      599 2023-05-27 16:58:36.537218 mkdocs_exporter-3.0.3/mkdocs_exporter/theme.py
--rw-r--r--   0        0        0        0 2023-05-27 16:58:36.537218 mkdocs_exporter-3.0.3/mkdocs_exporter/themes/__init__.py
--rw-r--r--   0        0        0      650 2023-05-27 16:58:36.537218 mkdocs_exporter-3.0.3/mkdocs_exporter/themes/factory.py
--rw-r--r--   0        0        0        0 2023-05-27 16:58:36.537218 mkdocs_exporter-3.0.3/mkdocs_exporter/themes/material/__init__.py
--rw-r--r--   0        0        0      681 2023-05-27 16:58:36.537218 mkdocs_exporter-3.0.3/mkdocs_exporter/themes/material/icons.py
--rw-r--r--   0        0        0     1317 2023-05-27 16:58:36.537218 mkdocs_exporter-3.0.3/mkdocs_exporter/themes/material/theme.py
--rw-r--r--   0        0        0        0 2023-05-27 16:58:36.537218 mkdocs_exporter-3.0.3/mkdocs_exporter/themes/readthedocs/__init__.py
--rw-r--r--   0        0        0     1221 2023-05-27 16:58:36.537218 mkdocs_exporter-3.0.3/mkdocs_exporter/themes/readthedocs/theme.py
--rw-r--r--   0        0        0     1618 2023-06-02 11:12:57.682011 mkdocs_exporter-3.0.3/pyproject.toml
--rw-r--r--   0        0        0     5357 1970-01-01 00:00:00.000000 mkdocs_exporter-3.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-08 13:15:16.904792 mkdocs_exporter-3.1.0/LICENSE
+-rw-r--r--   0        0        0     4007 2023-05-29 18:27:56.949905 mkdocs_exporter-3.1.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-08 15:45:32.453553 mkdocs_exporter-3.1.0/mkdocs_exporter/__init__.py
+-rw-r--r--   0        0        0      264 2023-05-30 17:10:15.899396 mkdocs_exporter-3.1.0/mkdocs_exporter/config.py
+-rw-r--r--   0        0        0       96 2023-05-08 19:25:05.801769 mkdocs_exporter-3.1.0/mkdocs_exporter/logging.py
+-rw-r--r--   0        0        0      543 2023-05-27 16:58:36.537218 mkdocs_exporter-3.1.0/mkdocs_exporter/page.py
+-rw-r--r--   0        0        0     1935 2023-05-30 17:10:15.899396 mkdocs_exporter-3.1.0/mkdocs_exporter/plugin.py
+-rw-r--r--   0        0        0        0 2023-05-06 21:44:34.488343 mkdocs_exporter-3.1.0/mkdocs_exporter/plugins/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-07 17:00:48.574613 mkdocs_exporter-3.1.0/mkdocs_exporter/plugins/extras/__init__.py
+-rw-r--r--   0        0        0      867 2023-05-30 17:10:15.899396 mkdocs_exporter-3.1.0/mkdocs_exporter/plugins/extras/config.py
+-rw-r--r--   0        0        0     1121 2023-05-30 17:10:15.899396 mkdocs_exporter-3.1.0/mkdocs_exporter/plugins/extras/plugin.py
+-rw-r--r--   0        0        0        0 2023-05-07 17:48:51.834620 mkdocs_exporter-3.1.0/mkdocs_exporter/plugins/pdf/__init__.py
+-rw-r--r--   0        0        0     2268 2023-06-13 18:22:11.411936 mkdocs_exporter-3.1.0/mkdocs_exporter/plugins/pdf/browser.py
+-rw-r--r--   0        0        0      526 2023-05-27 12:57:36.091210 mkdocs_exporter-3.1.0/mkdocs_exporter/plugins/pdf/button.py
+-rw-r--r--   0        0        0     1291 2023-06-13 18:20:29.951946 mkdocs_exporter-3.1.0/mkdocs_exporter/plugins/pdf/config.py
+-rw-r--r--   0        0        0     4912 2023-06-13 18:23:23.621929 mkdocs_exporter-3.1.0/mkdocs_exporter/plugins/pdf/plugin.py
+-rw-r--r--   0        0        0     2238 2023-06-13 18:12:31.191994 mkdocs_exporter-3.1.0/mkdocs_exporter/plugins/pdf/renderer.py
+-rw-r--r--   0        0        0     3845 2023-06-02 11:44:31.861490 mkdocs_exporter-3.1.0/mkdocs_exporter/preprocessor.py
+-rw-r--r--   0        0        0      241 2023-05-07 12:23:00.605366 mkdocs_exporter-3.1.0/mkdocs_exporter/renderer.py
+-rw-r--r--   0        0        0        0 2023-05-08 14:16:51.163540 mkdocs_exporter-3.1.0/mkdocs_exporter/resources/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-27 16:58:36.537218 mkdocs_exporter-3.1.0/mkdocs_exporter/resources/css/__init__.py
+-rw-r--r--   0        0        0       93 2023-05-27 16:58:36.537218 mkdocs_exporter-3.1.0/mkdocs_exporter/resources/css/readthedocs.css
+-rw-r--r--   0        0        0        0 2023-05-08 14:16:39.063540 mkdocs_exporter-3.1.0/mkdocs_exporter/resources/js/__init__.py
+-rw-r--r--   0        0        0   504034 2023-05-27 16:58:36.537218 mkdocs_exporter-3.1.0/mkdocs_exporter/resources/js/pagedjs.min.js
+-rw-r--r--   0        0        0      599 2023-05-27 16:58:36.537218 mkdocs_exporter-3.1.0/mkdocs_exporter/theme.py
+-rw-r--r--   0        0        0        0 2023-05-27 16:58:36.537218 mkdocs_exporter-3.1.0/mkdocs_exporter/themes/__init__.py
+-rw-r--r--   0        0        0      650 2023-05-27 16:58:36.537218 mkdocs_exporter-3.1.0/mkdocs_exporter/themes/factory.py
+-rw-r--r--   0        0        0        0 2023-05-27 16:58:36.537218 mkdocs_exporter-3.1.0/mkdocs_exporter/themes/material/__init__.py
+-rw-r--r--   0        0        0      681 2023-05-27 16:58:36.537218 mkdocs_exporter-3.1.0/mkdocs_exporter/themes/material/icons.py
+-rw-r--r--   0        0        0     1317 2023-05-27 16:58:36.537218 mkdocs_exporter-3.1.0/mkdocs_exporter/themes/material/theme.py
+-rw-r--r--   0        0        0        0 2023-05-27 16:58:36.537218 mkdocs_exporter-3.1.0/mkdocs_exporter/themes/readthedocs/__init__.py
+-rw-r--r--   0        0        0     1221 2023-05-27 16:58:36.537218 mkdocs_exporter-3.1.0/mkdocs_exporter/themes/readthedocs/theme.py
+-rw-r--r--   0        0        0     1618 2023-06-13 18:26:55.291907 mkdocs_exporter-3.1.0/pyproject.toml
+-rw-r--r--   0        0        0     5357 1970-01-01 00:00:00.000000 mkdocs_exporter-3.1.0/PKG-INFO
```

### Comparing `mkdocs_exporter-3.0.3/LICENSE` & `mkdocs_exporter-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-3.0.3/README.md` & `mkdocs_exporter-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-3.0.3/mkdocs_exporter/browser.py` & `mkdocs_exporter-3.1.0/mkdocs_exporter/plugins/pdf/browser.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,22 +20,23 @@
   @property
   def launched(self):
     """Has the browser been launched?"""
 
     return self._launched
 
 
-  def __init__(self):
+  def __init__(self, options: dict = {}):
     """The constructor."""
 
     self.browser = None
     self.context = None
     self._launched = False
     self.playwright = None
     self.lock = asyncio.Lock()
+    self.debug = options.get('debug', False)
 
 
   async def launch(self) -> Browser:
     """Launches the browser."""
 
     if self.launched:
       return self
@@ -46,14 +47,21 @@
 
       logger.info('Launching browser...')
 
       self.playwright = await async_playwright().start()
       self.browser = await self.playwright.chromium.launch(headless=True, args=self.args)
       self.context = await self.browser.new_context()
 
+      if self.debug:
+        async def log(msg):
+          for arg in msg.args:
+            logger.info(f"[pdf.browser] ({msg.type}) {await msg.page.title()}\n\t{await arg.json_value()}")
+
+        self.context.on('console', log)
+
       self._launched = True
 
     return self
 
 
   async def close(self) -> Browser:
     """Closes the browser."""
```

### Comparing `mkdocs_exporter-3.0.3/mkdocs_exporter/page.py` & `mkdocs_exporter-3.1.0/mkdocs_exporter/page.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-3.0.3/mkdocs_exporter/plugin.py` & `mkdocs_exporter-3.1.0/mkdocs_exporter/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-3.0.3/mkdocs_exporter/plugins/extras/config.py` & `mkdocs_exporter-3.1.0/mkdocs_exporter/plugins/extras/config.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-3.0.3/mkdocs_exporter/plugins/extras/plugin.py` & `mkdocs_exporter-3.1.0/mkdocs_exporter/plugins/extras/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-3.0.3/mkdocs_exporter/plugins/pdf/button.py` & `mkdocs_exporter-3.1.0/mkdocs_exporter/plugins/pdf/button.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-3.0.3/mkdocs_exporter/plugins/pdf/config.py` & `mkdocs_exporter-3.1.0/mkdocs_exporter/plugins/pdf/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 from mkdocs.config import config_options as c
 from mkdocs.config.base import Config as BaseConfig
 
 
+class BrowserConfig(BaseConfig):
+  """The browser's configuration."""
+
+  debug = c.Type(bool, default=False)
+  """Should console messages sent to the browser be logged?"""
+
+
 class CoversConfig(BaseConfig):
   """The cover's configuration."""
 
   front = c.Optional(c.File(exists=True))
   """The front cover template location."""
 
   back = c.Optional(c.File(exists=True))
@@ -28,7 +35,10 @@
   """A list of custom stylesheets to apply before rendering documents."""
 
   scripts = c.ListOfItems(c.File(exists=True), default=[])
   """A list of custom scripts to inject before rendering documents."""
 
   covers = c.SubConfig(CoversConfig)
   """The document's cover pages."""
+
+  browser = c.SubConfig(BrowserConfig)
+  """The browser's configuration."""
```

### Comparing `mkdocs_exporter-3.0.3/mkdocs_exporter/plugins/pdf/plugin.py` & `mkdocs_exporter-3.1.0/mkdocs_exporter/plugins/pdf/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,15 +78,15 @@
     """Invoked before the build process starts."""
 
     self.tasks.clear()
 
     if not self._enabled():
       return
 
-    self.renderer = Renderer()
+    self.renderer = Renderer(browser_options=self.config.browser)
 
     for stylesheet in self.config.stylesheets:
       self.renderer.add_stylesheet(stylesheet)
     for script in self.config.scripts:
       self.renderer.add_script(script)
 
 
@@ -113,25 +113,25 @@
       del page.formats['pdf']
     if 'pdf' not in page.formats:
       return html
 
     page.html = html
 
     async def render(page: Page) -> None:
-      logger.info('Rendering PDF for %s...', page.file.src_path)
+      logger.info("[pdf] Rendering '%s'...", page.file.src_path)
 
       pdf = await self.renderer.render(page)
       fullpath = os.path.join(config['site_dir'], page.formats['pdf'])
 
       page.html = None
 
       with open(fullpath, 'wb+') as file:
         file.write(pdf)
 
-      logger.info('File written to %s!', fullpath)
+      logger.info("[pdf] File written to '%s'!", fullpath)
 
     self.tasks.append(render(page))
 
     return page.html
 
 
   def on_post_build(self, **kwargs) -> None:
```

### Comparing `mkdocs_exporter-3.0.3/mkdocs_exporter/plugins/pdf/renderer.py` & `mkdocs_exporter-3.1.0/mkdocs_exporter/plugins/pdf/renderer.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 
 import os
 import importlib_resources
 
 from urllib.parse import unquote
 from mkdocs_exporter.page import Page
 from mkdocs_exporter.resources import js
-from mkdocs_exporter.browser import Browser
 from mkdocs_exporter.preprocessor import Preprocessor
+from mkdocs_exporter.plugins.pdf.browser import Browser
 from mkdocs_exporter.renderer import Renderer as BaseRenderer
 
 
 class Renderer(BaseRenderer):
   """The renderer."""
 
-  def __init__(self, browser: Browser = None):
+  def __init__(self, browser: Browser = None, browser_options: dict = None):
     """The constructor."""
 
     self.scripts: list[str] = []
     self.stylesheets: list[str] = []
-    self.browser = browser or Browser()
+    self.browser = browser or Browser(browser_options)
 
 
   def add_stylesheet(self, path: str) -> Renderer:
     """Adds a stylesheet to the renderer."""
 
     self.stylesheets.append(path)
```

### Comparing `mkdocs_exporter-3.0.3/mkdocs_exporter/preprocessor.py` & `mkdocs_exporter-3.1.0/mkdocs_exporter/preprocessor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import os
 import sass
 
+from typing import Union
 from urllib.parse import urlparse
 from bs4 import BeautifulSoup, Tag
-from typing import Any, Callable, Union
 from mkdocs_exporter.theme import Theme
 from mkdocs_exporter.logging import logger
 
 
 class Preprocessor():
   """The HTML preprocessor."""
```

### Comparing `mkdocs_exporter-3.0.3/mkdocs_exporter/resources/js/pagedjs.min.js` & `mkdocs_exporter-3.1.0/mkdocs_exporter/resources/js/pagedjs.min.js`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-3.0.3/mkdocs_exporter/theme.py` & `mkdocs_exporter-3.1.0/mkdocs_exporter/theme.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-3.0.3/mkdocs_exporter/themes/factory.py` & `mkdocs_exporter-3.1.0/mkdocs_exporter/themes/factory.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-3.0.3/mkdocs_exporter/themes/material/icons.py` & `mkdocs_exporter-3.1.0/mkdocs_exporter/themes/material/icons.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-3.0.3/mkdocs_exporter/themes/material/theme.py` & `mkdocs_exporter-3.1.0/mkdocs_exporter/themes/material/theme.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-3.0.3/mkdocs_exporter/themes/readthedocs/theme.py` & `mkdocs_exporter-3.1.0/mkdocs_exporter/themes/readthedocs/theme.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-3.0.3/pyproject.toml` & `mkdocs_exporter-3.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "mkdocs-exporter"
-version = "3.0.3"
+version = "3.1.0"
 repository = "https://github.com/adrienbrignon/mkdocs-exporter"
 keywords = ["mkdocs", "pdf", "exporter"]
 description = "A highly-configurable plugin for MkDocs that exports your pages to PDF files."
 authors = ["Adrien Brignon <adrien@brignon.dev>"]
 readme = "README.md"
 classifiers = [
   "License :: OSI Approved :: MIT License",
```

### Comparing `mkdocs_exporter-3.0.3/PKG-INFO` & `mkdocs_exporter-3.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-exporter
-Version: 3.0.3
+Version: 3.1.0
 Summary: A highly-configurable plugin for MkDocs that exports your pages to PDF files.
 Home-page: https://github.com/adrienbrignon/mkdocs-exporter
 Keywords: mkdocs,pdf,exporter
 Author: Adrien Brignon
 Author-email: adrien@brignon.dev
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mkdocs-exporter Version: 3.0.3 Summary: A highly-
+Metadata-Version: 2.1 Name: mkdocs-exporter Version: 3.1.0 Summary: A highly-
 configurable plugin for MkDocs that exports your pages to PDF files. Home-page:
 https://github.com/adrienbrignon/mkdocs-exporter Keywords: mkdocs,pdf,exporter
 Author: Adrien Brignon Author-email: adrien@brignon.dev Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

