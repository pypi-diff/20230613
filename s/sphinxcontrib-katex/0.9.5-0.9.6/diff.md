# Comparing `tmp/sphinxcontrib-katex-0.9.5.tar.gz` & `tmp/sphinxcontrib-katex-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinxcontrib-katex-0.9.5.tar", last modified: Wed Jun  7 10:14:25 2023, max compression
+gzip compressed data, was "sphinxcontrib-katex-0.9.6.tar", last modified: Tue Jun 13 06:10:48 2023, max compression
```

## Comparing `sphinxcontrib-katex-0.9.5.tar` & `sphinxcontrib-katex-0.9.6.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:14:25.967483 sphinxcontrib-katex-0.9.5/
--rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-06-07 10:14:17.000000 sphinxcontrib-katex-0.9.5/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-06-07 10:14:17.000000 sphinxcontrib-katex-0.9.5/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-07 10:14:17.000000 sphinxcontrib-katex-0.9.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-07 10:14:17.000000 sphinxcontrib-katex-0.9.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11478 2023-06-07 10:14:25.967483 sphinxcontrib-katex-0.9.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-06-07 10:14:17.000000 sphinxcontrib-katex-0.9.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:14:25.967483 sphinxcontrib-katex-0.9.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-07 10:14:17.000000 sphinxcontrib-katex-0.9.5/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-06-07 10:14:17.000000 sphinxcontrib-katex-0.9.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-07 10:14:17.000000 sphinxcontrib-katex-0.9.5/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-07 10:14:17.000000 sphinxcontrib-katex-0.9.5/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-07 10:14:17.000000 sphinxcontrib-katex-0.9.5/docs/definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-06-07 10:14:17.000000 sphinxcontrib-katex-0.9.5/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-07 10:14:17.000000 sphinxcontrib-katex-0.9.5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-07 10:14:17.000000 sphinxcontrib-katex-0.9.5/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-07 10:14:17.000000 sphinxcontrib-katex-0.9.5/docs/macros.rst
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-07 10:14:17.000000 sphinxcontrib-katex-0.9.5/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-07 10:14:17.000000 sphinxcontrib-katex-0.9.5/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-07 10:14:17.000000 sphinxcontrib-katex-0.9.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-06-07 10:14:25.967483 sphinxcontrib-katex-0.9.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-07 10:14:17.000000 sphinxcontrib-katex-0.9.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:14:25.967483 sphinxcontrib-katex-0.9.5/sphinxcontrib/
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-06-07 10:14:17.000000 sphinxcontrib-katex-0.9.5/sphinxcontrib/auto-render.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-07 10:14:17.000000 sphinxcontrib-katex-0.9.5/sphinxcontrib/katex-math.css
--rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-06-07 10:14:17.000000 sphinxcontrib-katex-0.9.5/sphinxcontrib/katex-server.js
--rw-r--r--   0 runner    (1001) docker     (123)   276757 2023-06-07 10:14:17.000000 sphinxcontrib-katex-0.9.5/sphinxcontrib/katex.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    18711 2023-06-07 10:14:17.000000 sphinxcontrib-katex-0.9.5/sphinxcontrib/katex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:14:25.967483 sphinxcontrib-katex-0.9.5/sphinxcontrib_katex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11478 2023-06-07 10:14:25.000000 sphinxcontrib-katex-0.9.5/sphinxcontrib_katex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-06-07 10:14:25.000000 sphinxcontrib-katex-0.9.5/sphinxcontrib_katex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 10:14:25.000000 sphinxcontrib-katex-0.9.5/sphinxcontrib_katex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-07 10:14:25.000000 sphinxcontrib-katex-0.9.5/sphinxcontrib_katex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-07 10:14:25.000000 sphinxcontrib-katex-0.9.5/sphinxcontrib_katex.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:10:48.816928 sphinxcontrib-katex-0.9.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-06-13 06:10:39.000000 sphinxcontrib-katex-0.9.6/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-06-13 06:10:39.000000 sphinxcontrib-katex-0.9.6/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-13 06:10:39.000000 sphinxcontrib-katex-0.9.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-13 06:10:39.000000 sphinxcontrib-katex-0.9.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11623 2023-06-13 06:10:48.816928 sphinxcontrib-katex-0.9.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-06-13 06:10:39.000000 sphinxcontrib-katex-0.9.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:10:48.812928 sphinxcontrib-katex-0.9.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-13 06:10:39.000000 sphinxcontrib-katex-0.9.6/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-06-13 06:10:39.000000 sphinxcontrib-katex-0.9.6/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-13 06:10:39.000000 sphinxcontrib-katex-0.9.6/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-13 06:10:39.000000 sphinxcontrib-katex-0.9.6/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-13 06:10:39.000000 sphinxcontrib-katex-0.9.6/docs/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-06-13 06:10:39.000000 sphinxcontrib-katex-0.9.6/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-13 06:10:39.000000 sphinxcontrib-katex-0.9.6/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-13 06:10:39.000000 sphinxcontrib-katex-0.9.6/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-13 06:10:39.000000 sphinxcontrib-katex-0.9.6/docs/macros.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-13 06:10:39.000000 sphinxcontrib-katex-0.9.6/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-13 06:10:39.000000 sphinxcontrib-katex-0.9.6/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-13 06:10:39.000000 sphinxcontrib-katex-0.9.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-06-13 06:10:48.816928 sphinxcontrib-katex-0.9.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-13 06:10:39.000000 sphinxcontrib-katex-0.9.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:10:48.816928 sphinxcontrib-katex-0.9.6/sphinxcontrib/
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-06-13 06:10:39.000000 sphinxcontrib-katex-0.9.6/sphinxcontrib/auto-render.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-13 06:10:39.000000 sphinxcontrib-katex-0.9.6/sphinxcontrib/katex-math.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-06-13 06:10:39.000000 sphinxcontrib-katex-0.9.6/sphinxcontrib/katex-server.js
+-rw-r--r--   0 runner    (1001) docker     (123)   276757 2023-06-13 06:10:39.000000 sphinxcontrib-katex-0.9.6/sphinxcontrib/katex.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18711 2023-06-13 06:10:39.000000 sphinxcontrib-katex-0.9.6/sphinxcontrib/katex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:10:48.816928 sphinxcontrib-katex-0.9.6/sphinxcontrib_katex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11623 2023-06-13 06:10:48.000000 sphinxcontrib-katex-0.9.6/sphinxcontrib_katex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-06-13 06:10:48.000000 sphinxcontrib-katex-0.9.6/sphinxcontrib_katex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 06:10:48.000000 sphinxcontrib-katex-0.9.6/sphinxcontrib_katex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-13 06:10:48.000000 sphinxcontrib-katex-0.9.6/sphinxcontrib_katex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-13 06:10:48.000000 sphinxcontrib-katex-0.9.6/sphinxcontrib_katex.egg-info/top_level.txt
```

### Comparing `sphinxcontrib-katex-0.9.5/CHANGELOG.rst` & `sphinxcontrib-katex-0.9.6/CHANGELOG.rst`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,22 @@
 
 All notable changes to this project will be documented in this file.
 
 The format is based on `Keep a Changelog`_,
 and this project adheres to `Semantic Versioning`_.
 
 
+Version 0.9.6 (2023-06-13)
+--------------------------
+
+* Changed: use custom sphinx theme
+  based on ``insipid``
+  for HTML documentation pages
+
+
 Version 0.9.5 (2023-06-07)
 --------------------------
 
 * Changed: use KaTeX 0.16.7
 * Fixed: convert ``KaTeXServer.timeout_error()``
   to class method
```

### Comparing `sphinxcontrib-katex-0.9.5/CONTRIBUTING.rst` & `sphinxcontrib-katex-0.9.6/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-katex-0.9.5/LICENSE` & `sphinxcontrib-katex-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-katex-0.9.5/PKG-INFO` & `sphinxcontrib-katex-0.9.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinxcontrib-katex
-Version: 0.9.5
+Version: 0.9.6
 Summary: A Sphinx extension for rendering math in HTML pages
 Home-page: https://github.com/hagenw/sphinxcontrib-katex
 Author: Hagen Wierstorf
 Author-email: hagenw@posteo.de
 License: MIT
 Keywords: sphinx,latex,katex,math,documentation
 Platform: any
@@ -82,15 +82,15 @@
 
 In ``conf.py`` of your Sphinx project, add the extension with:
 
 .. code-block:: python
 
     extensions = ['sphinxcontrib.katex']
 
-For enable server side pre-rendering
+To enable server side pre-rendering
 add in addition
 (nodejs_ installation needed):
 
 .. code-block:: python
 
     katex_prerender = True
 
@@ -201,14 +201,22 @@
 
 All notable changes to this project will be documented in this file.
 
 The format is based on `Keep a Changelog`_,
 and this project adheres to `Semantic Versioning`_.
 
 
+Version 0.9.6 (2023-06-13)
+--------------------------
+
+* Changed: use custom sphinx theme
+  based on ``insipid``
+  for HTML documentation pages
+
+
 Version 0.9.5 (2023-06-07)
 --------------------------
 
 * Changed: use KaTeX 0.16.7
 * Fixed: convert ``KaTeXServer.timeout_error()``
   to class method
```

### Comparing `sphinxcontrib-katex-0.9.5/README.rst` & `sphinxcontrib-katex-0.9.6/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 
 In ``conf.py`` of your Sphinx project, add the extension with:
 
 .. code-block:: python
 
     extensions = ['sphinxcontrib.katex']
 
-For enable server side pre-rendering
+To enable server side pre-rendering
 add in addition
 (nodejs_ installation needed):
 
 .. code-block:: python
 
     katex_prerender = True
```

### Comparing `sphinxcontrib-katex-0.9.5/docs/conf.py` & `sphinxcontrib-katex-0.9.6/docs/conf.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,15 +31,14 @@
     release = release.decode().strip()
 except Exception:
     release = '<unknown>'
 
 # Code syntax highlighting style
 pygments_style = 'tango'
 
-
 # -- ACRONYMS AND MATH ---------------------------------------------------
 latex_macros = r"""
     \def \x                {\mathbf{x}}
     \def \w                {\omega}
     \def \d                {\operatorname{d}\!}
 """
 katex_macros = katex.latex_defs_to_katex_macros(latex_macros)
@@ -48,17 +47,39 @@
 
 
 # -- HTML ----------------------------------------------------------------
 
 html_title = project
 html_short_title = ""
 htmlhelp_basename = project
+
+# Theme settings,
+# see https://insipid-sphinx-theme.readthedocs.io/configuration.html
+html_theme = 'insipid'
+html_permalinks_icon = '#'
+html_copy_source = False
+html_show_sourcelink = False
+html_use_index = False
 html_theme_options = {
-    'code_font_size': '0.8em',
+    'right_buttons': [
+        'fullscreen-button.html',
+        'pdf-button.html',
+        'repo-button.html',
+    ],
 }
+html_context = {
+    'display_github': True,
+    'github_user': 'hagenw',
+    'github_repo': 'sphinxcontrib-katex',
+}
+
+# Extending theme
+templates_path = ['_templates']
+html_static_path = ['_static']
+html_css_files = ['custom.css']
 
 
 # -- LATEX ---------------------------------------------------------------
 
 # Add arydshln package for dashed lines in array
 latex_macros += r'\usepackage{arydshln}'
```

### Comparing `sphinxcontrib-katex-0.9.5/docs/definitions.py` & `sphinxcontrib-katex-0.9.6/docs/definitions.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-katex-0.9.5/docs/examples.rst` & `sphinxcontrib-katex-0.9.6/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-katex-0.9.5/setup.cfg` & `sphinxcontrib-katex-0.9.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-katex-0.9.5/sphinxcontrib/auto-render.min.js` & `sphinxcontrib-katex-0.9.6/sphinxcontrib/auto-render.min.js`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-katex-0.9.5/sphinxcontrib/katex-math.css` & `sphinxcontrib-katex-0.9.6/sphinxcontrib/katex-math.css`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-katex-0.9.5/sphinxcontrib/katex-server.js` & `sphinxcontrib-katex-0.9.6/sphinxcontrib/katex-server.js`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-katex-0.9.5/sphinxcontrib/katex.min.js` & `sphinxcontrib-katex-0.9.6/sphinxcontrib/katex.min.js`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-katex-0.9.5/sphinxcontrib/katex.py` & `sphinxcontrib-katex-0.9.6/sphinxcontrib/katex.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 from subprocess import PIPE, Popen, TimeoutExpired
 
 from sphinx.locale import _
 from sphinx.errors import ExtensionError
 from sphinx.util.osutil import copyfile
 
 
-__version__ = '0.9.5'
+__version__ = '0.9.6'
 katex_version = '0.16.7'
 filename_css = 'katex-math.css'
 filename_autorenderer = 'katex_autorenderer.js'
 SRC_DIR = Path(__file__).parent
 SCRIPT_PATH = str(SRC_DIR / "katex-server.js")
 
 ONE_MILLISECOND = 0.001
```

### Comparing `sphinxcontrib-katex-0.9.5/sphinxcontrib_katex.egg-info/PKG-INFO` & `sphinxcontrib-katex-0.9.6/sphinxcontrib_katex.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinxcontrib-katex
-Version: 0.9.5
+Version: 0.9.6
 Summary: A Sphinx extension for rendering math in HTML pages
 Home-page: https://github.com/hagenw/sphinxcontrib-katex
 Author: Hagen Wierstorf
 Author-email: hagenw@posteo.de
 License: MIT
 Keywords: sphinx,latex,katex,math,documentation
 Platform: any
@@ -82,15 +82,15 @@
 
 In ``conf.py`` of your Sphinx project, add the extension with:
 
 .. code-block:: python
 
     extensions = ['sphinxcontrib.katex']
 
-For enable server side pre-rendering
+To enable server side pre-rendering
 add in addition
 (nodejs_ installation needed):
 
 .. code-block:: python
 
     katex_prerender = True
 
@@ -201,14 +201,22 @@
 
 All notable changes to this project will be documented in this file.
 
 The format is based on `Keep a Changelog`_,
 and this project adheres to `Semantic Versioning`_.
 
 
+Version 0.9.6 (2023-06-13)
+--------------------------
+
+* Changed: use custom sphinx theme
+  based on ``insipid``
+  for HTML documentation pages
+
+
 Version 0.9.5 (2023-06-07)
 --------------------------
 
 * Changed: use KaTeX 0.16.7
 * Fixed: convert ``KaTeXServer.timeout_error()``
   to class method
```

### Comparing `sphinxcontrib-katex-0.9.5/sphinxcontrib_katex.egg-info/SOURCES.txt` & `sphinxcontrib-katex-0.9.6/sphinxcontrib_katex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

