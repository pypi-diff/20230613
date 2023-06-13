# Comparing `tmp/robocorp_browser-1.0.0.tar.gz` & `tmp/robocorp_browser-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robocorp_browser-1.0.0.tar", max compression
+gzip compressed data, was "robocorp_browser-1.0.1.tar", max compression
```

## Comparing `robocorp_browser-1.0.0.tar` & `robocorp_browser-1.0.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       94 2023-06-09 12:05:54.414735 robocorp_browser-1.0.0/README.md
--rw-r--r--   0        0        0      638 2023-06-09 12:05:54.414735 robocorp_browser-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     6289 2023-06-09 12:05:54.418735 robocorp_browser-1.0.0/src/robocorp/browser/__init__.py
--rw-r--r--   0        0        0       81 2023-06-09 12:05:54.418735 robocorp_browser-1.0.0/src/robocorp/browser/__main__.py
--rw-r--r--   0        0        0     6725 2023-06-09 12:05:54.418735 robocorp_browser-1.0.0/src/robocorp/browser/_browser_context.py
--rw-r--r--   0        0        0     1890 2023-06-09 12:05:54.418735 robocorp_browser-1.0.0/src/robocorp/browser/_browser_engines.py
--rw-r--r--   0        0        0      825 2023-06-09 12:05:54.418735 robocorp_browser-1.0.0/src/robocorp/browser/cli.py
--rw-r--r--   0        0        0        0 2023-06-09 12:05:54.418735 robocorp_browser-1.0.0/src/robocorp/browser/py.typed
--rw-r--r--   0        0        0      606 1970-01-01 00:00:00.000000 robocorp_browser-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1583 2023-06-13 15:07:28.840150 robocorp_browser-1.0.1/README.md
+-rw-r--r--   0        0        0      636 2023-06-13 15:07:28.844150 robocorp_browser-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     6289 2023-06-13 15:07:28.844150 robocorp_browser-1.0.1/src/robocorp/browser/__init__.py
+-rw-r--r--   0        0        0       81 2023-06-13 15:07:28.844150 robocorp_browser-1.0.1/src/robocorp/browser/__main__.py
+-rw-r--r--   0        0        0     6725 2023-06-13 15:07:28.844150 robocorp_browser-1.0.1/src/robocorp/browser/_browser_context.py
+-rw-r--r--   0        0        0     1890 2023-06-13 15:07:28.844150 robocorp_browser-1.0.1/src/robocorp/browser/_browser_engines.py
+-rw-r--r--   0        0        0      825 2023-06-13 15:07:28.844150 robocorp_browser-1.0.1/src/robocorp/browser/cli.py
+-rw-r--r--   0        0        0        0 2023-06-13 15:07:28.844150 robocorp_browser-1.0.1/src/robocorp/browser/py.typed
+-rw-r--r--   0        0        0     2091 1970-01-01 00:00:00.000000 robocorp_browser-1.0.1/PKG-INFO
```

### Comparing `robocorp_browser-1.0.0/pyproject.toml` & `robocorp_browser-1.0.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "robocorp-browser"
-version = "1.0.0"
+version = "1.0.1"
 description = "Robocorp browser automation library"
 authors = [
 	"Fabio Z. <fabio@robocorp.com>",
 	"Kerkko P. <kerkko@robocorp.com>",
 	"Ossi R. <ossi@robocorp.com>",
 ]
 readme = "README.md"
 packages = [{include = "robocorp", from="src"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 playwright = "^1.32.1"
-robocorp-tasks = "^0.4"
+robocorp-tasks = "^1"
 
 [tool.poetry.group.dev.dependencies]
 robocorp-devutils = {path = "../devutils/", develop = true}
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `robocorp_browser-1.0.0/src/robocorp/browser/__init__.py` & `robocorp_browser-1.0.1/src/robocorp/browser/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     Locator,
     Page,
     Playwright,
 )
 
 from ._browser_engines import BrowserEngine
 
-__version__ = "1.0.0"
+__version__ = "1.0.1"
 version_info = [int(x) for x in __version__.split(".")]
 
 
 def configure(**kwargs) -> None:
     """
     May be called before any other method to configure the browser settings.
```

### Comparing `robocorp_browser-1.0.0/src/robocorp/browser/_browser_context.py` & `robocorp_browser-1.0.1/src/robocorp/browser/_browser_context.py`

 * *Files identical despite different names*

### Comparing `robocorp_browser-1.0.0/src/robocorp/browser/_browser_engines.py` & `robocorp_browser-1.0.1/src/robocorp/browser/_browser_engines.py`

 * *Files identical despite different names*

### Comparing `robocorp_browser-1.0.0/src/robocorp/browser/cli.py` & `robocorp_browser-1.0.1/src/robocorp/browser/cli.py`

 * *Files identical despite different names*

