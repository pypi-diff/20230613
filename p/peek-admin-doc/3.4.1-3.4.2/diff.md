# Comparing `tmp/peek-admin-doc-3.4.1.tar.gz` & `tmp/peek-admin-doc-3.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peek-admin-doc-3.4.1.tar", last modified: Wed May 17 03:30:31 2023, max compression
+gzip compressed data, was "peek-admin-doc-3.4.2.tar", last modified: Tue Jun 13 11:58:39 2023, max compression
```

## Comparing `peek-admin-doc-3.4.1.tar` & `peek-admin-doc-3.4.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:30:31.965306 peek-admin-doc-3.4.1/
--rw-r--r--   0 root         (0) root         (0)      358 2023-05-17 03:30:31.965306 peek-admin-doc-3.4.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      678 2023-05-17 03:29:54.000000 peek-admin-doc-3.4.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:30:31.964306 peek-admin-doc-3.4.1/peek_admin_doc/
--rw-r--r--   0 root         (0) root         (0)      460 2023-05-17 03:29:54.000000 peek-admin-doc-3.4.1/peek_admin_doc/PlatformDependencyTest.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 03:30:31.000000 peek-admin-doc-3.4.1/peek_admin_doc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:30:31.965306 peek-admin-doc-3.4.1/peek_admin_doc/_static/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 03:29:54.000000 peek-admin-doc-3.4.1/peek_admin_doc/_static/.gitkeep
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:30:31.965306 peek-admin-doc-3.4.1/peek_admin_doc/_static/fonts/
--rw-r--r--   0 root         (0) root         (0)    77160 2023-05-17 03:29:54.000000 peek-admin-doc-3.4.1/peek_admin_doc/_static/fonts/fontawesome-webfont.woff2
--rw-r--r--   0 root         (0) root         (0)      556 2023-05-17 03:29:54.000000 peek-admin-doc-3.4.1/peek_admin_doc/build_html_docs.sh
--rw-r--r--   0 root         (0) root         (0)      545 2023-05-17 03:29:54.000000 peek-admin-doc-3.4.1/peek_admin_doc/build_latex_docs.sh
--rw-r--r--   0 root         (0) root         (0)    11240 2023-05-17 03:30:31.000000 peek-admin-doc-3.4.1/peek_admin_doc/conf.py
--rw-r--r--   0 root         (0) root         (0)      294 2023-05-17 03:29:54.000000 peek-admin-doc-3.4.1/peek_admin_doc/index.rst
--rw-r--r--   0 root         (0) root         (0)     1091 2023-05-17 03:29:54.000000 peek-admin-doc-3.4.1/peek_admin_doc/watch_docs.sh
--rw-r--r--   0 root         (0) root         (0)      456 2023-05-17 03:29:54.000000 peek-admin-doc-3.4.1/peek_admin_doc/welcome.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:30:31.964306 peek-admin-doc-3.4.1/peek_admin_doc.egg-info/
--rw-r--r--   0 root         (0) root         (0)      358 2023-05-17 03:30:31.000000 peek-admin-doc-3.4.1/peek_admin_doc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      573 2023-05-17 03:30:31.000000 peek-admin-doc-3.4.1/peek_admin_doc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 03:30:31.000000 peek-admin-doc-3.4.1/peek_admin_doc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 03:30:31.000000 peek-admin-doc-3.4.1/peek_admin_doc.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-17 03:30:31.000000 peek-admin-doc-3.4.1/peek_admin_doc.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-05-17 03:30:31.000000 peek-admin-doc-3.4.1/peek_admin_doc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-17 03:30:31.965306 peek-admin-doc-3.4.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3077 2023-05-17 03:30:31.000000 peek-admin-doc-3.4.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 11:58:39.899906 peek-admin-doc-3.4.2/
+-rw-r--r--   0 root         (0) root         (0)      358 2023-06-13 11:58:39.898906 peek-admin-doc-3.4.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      678 2023-06-13 11:58:03.000000 peek-admin-doc-3.4.2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 11:58:39.898906 peek-admin-doc-3.4.2/peek_admin_doc/
+-rw-r--r--   0 root         (0) root         (0)      460 2023-06-13 11:58:03.000000 peek-admin-doc-3.4.2/peek_admin_doc/PlatformDependencyTest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 11:58:39.000000 peek-admin-doc-3.4.2/peek_admin_doc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 11:58:39.898906 peek-admin-doc-3.4.2/peek_admin_doc/_static/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 11:58:03.000000 peek-admin-doc-3.4.2/peek_admin_doc/_static/.gitkeep
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 11:58:39.898906 peek-admin-doc-3.4.2/peek_admin_doc/_static/fonts/
+-rw-r--r--   0 root         (0) root         (0)    77160 2023-06-13 11:58:03.000000 peek-admin-doc-3.4.2/peek_admin_doc/_static/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0 root         (0) root         (0)      556 2023-06-13 11:58:03.000000 peek-admin-doc-3.4.2/peek_admin_doc/build_html_docs.sh
+-rw-r--r--   0 root         (0) root         (0)      545 2023-06-13 11:58:03.000000 peek-admin-doc-3.4.2/peek_admin_doc/build_latex_docs.sh
+-rw-r--r--   0 root         (0) root         (0)    11240 2023-06-13 11:58:39.000000 peek-admin-doc-3.4.2/peek_admin_doc/conf.py
+-rw-r--r--   0 root         (0) root         (0)      294 2023-06-13 11:58:03.000000 peek-admin-doc-3.4.2/peek_admin_doc/index.rst
+-rw-r--r--   0 root         (0) root         (0)     1091 2023-06-13 11:58:03.000000 peek-admin-doc-3.4.2/peek_admin_doc/watch_docs.sh
+-rw-r--r--   0 root         (0) root         (0)      456 2023-06-13 11:58:03.000000 peek-admin-doc-3.4.2/peek_admin_doc/welcome.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 11:58:39.898906 peek-admin-doc-3.4.2/peek_admin_doc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      358 2023-06-13 11:58:39.000000 peek-admin-doc-3.4.2/peek_admin_doc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      573 2023-06-13 11:58:39.000000 peek-admin-doc-3.4.2/peek_admin_doc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 11:58:39.000000 peek-admin-doc-3.4.2/peek_admin_doc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 11:58:39.000000 peek-admin-doc-3.4.2/peek_admin_doc.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-13 11:58:39.000000 peek-admin-doc-3.4.2/peek_admin_doc.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-06-13 11:58:39.000000 peek-admin-doc-3.4.2/peek_admin_doc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-13 11:58:39.899906 peek-admin-doc-3.4.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3077 2023-06-13 11:58:39.000000 peek-admin-doc-3.4.2/setup.py
```

### Comparing `peek-admin-doc-3.4.1/README.rst` & `peek-admin-doc-3.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `peek-admin-doc-3.4.1/peek_admin_doc/_static/fonts/fontawesome-webfont.woff2` & `peek-admin-doc-3.4.2/peek_admin_doc/_static/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `peek-admin-doc-3.4.1/peek_admin_doc/build_html_docs.sh` & `peek-admin-doc-3.4.2/peek_admin_doc/build_html_docs.sh`

 * *Files identical despite different names*

### Comparing `peek-admin-doc-3.4.1/peek_admin_doc/build_latex_docs.sh` & `peek-admin-doc-3.4.2/peek_admin_doc/build_latex_docs.sh`

 * *Files identical despite different names*

### Comparing `peek-admin-doc-3.4.1/peek_admin_doc/conf.py` & `peek-admin-doc-3.4.2/peek_admin_doc/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # sys.path.insert(0, os.path.abspath('.'))
 from sphinx.ext.apidoc import create_modules_toc_file, recurse_tree
 
 title = "Synerty Peek - Administration Documentation"
 __project__ = "SynertyPeek-AdminDocs"
 __copyright__ = "2021, Synerty"
 __author__ = "Synerty"
-__version__ = '3.4.1'
+__version__ = '3.4.2'
 
 import sphinx_rtd_theme
 
 # -- General configuration ------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
```

### Comparing `peek-admin-doc-3.4.1/peek_admin_doc/watch_docs.sh` & `peek-admin-doc-3.4.2/peek_admin_doc/watch_docs.sh`

 * *Files identical despite different names*

### Comparing `peek-admin-doc-3.4.1/peek_admin_doc.egg-info/SOURCES.txt` & `peek-admin-doc-3.4.2/peek_admin_doc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `peek-admin-doc-3.4.1/setup.py` & `peek-admin-doc-3.4.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Modify these values to fork a new plugin
 #
 
 author = "Synerty"
 author_email = "contact@synerty.com"
 py_package_name = "peek_admin_doc"
 pip_package_name = py_package_name.replace("_", "-")
-package_version = "3.4.1"
+package_version = "3.4.2"
 description = "Peek Admin Docs."
 
 download_url = "https://bitbucket.org/synerty/%s/get/%s.zip"
 download_url %= pip_package_name, package_version
 url = "https://bitbucket.org/synerty/%s" % pip_package_name
 
 ###############################################################################
```

