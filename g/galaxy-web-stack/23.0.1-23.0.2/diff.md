# Comparing `tmp/galaxy-web-stack-23.0.1.tar.gz` & `tmp/galaxy-web-stack-23.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/galaxy/galaxy/packages/web_stack/dist/.tmp-szsfagqx/galaxy-web-stack-23.0.1.tar", last modified: Thu Jun  8 17:44:05 2023, max compression
+gzip compressed data, was "/home/runner/work/galaxy/galaxy/packages/web_stack/dist/.tmp-o6jakg4s/galaxy-web-stack-23.0.2.tar", last modified: Tue Jun 13 17:11:53 2023, max compression
```

## Comparing `galaxy-web-stack-23.0.1.tar` & `galaxy-web-stack-23.0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:44:05.000000 galaxy-web-stack-23.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-08 17:37:04.000000 galaxy-web-stack-23.0.1/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12875 2023-06-08 17:37:03.000000 galaxy-web-stack-23.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-08 17:37:04.000000 galaxy-web-stack-23.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-08 17:44:05.000000 galaxy-web-stack-23.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-08 17:37:04.000000 galaxy-web-stack-23.0.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-08 17:37:04.000000 galaxy-web-stack-23.0.1/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:44:05.000000 galaxy-web-stack-23.0.1/galaxy/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-08 17:37:04.000000 galaxy-web-stack-23.0.1/galaxy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 17:37:04.000000 galaxy-web-stack-23.0.1/galaxy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:44:05.000000 galaxy-web-stack-23.0.1/galaxy/web_stack/
--rw-r--r--   0 runner    (1001) docker     (123)    12414 2023-06-08 17:37:04.000000 galaxy-web-stack-23.0.1/galaxy/web_stack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-06-08 17:37:04.000000 galaxy-web-stack-23.0.1/galaxy/web_stack/gunicorn_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    21744 2023-06-08 17:37:04.000000 galaxy-web-stack-23.0.1/galaxy/web_stack/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-06-08 17:37:04.000000 galaxy-web-stack-23.0.1/galaxy/web_stack/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-06-08 17:37:04.000000 galaxy-web-stack-23.0.1/galaxy/web_stack/transport.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:44:05.000000 galaxy-web-stack-23.0.1/galaxy_web_stack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-08 17:44:05.000000 galaxy-web-stack-23.0.1/galaxy_web_stack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-08 17:44:05.000000 galaxy-web-stack-23.0.1/galaxy_web_stack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 17:44:05.000000 galaxy-web-stack-23.0.1/galaxy_web_stack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-08 17:44:05.000000 galaxy-web-stack-23.0.1/galaxy_web_stack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-08 17:44:05.000000 galaxy-web-stack-23.0.1/galaxy_web_stack.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-08 17:37:04.000000 galaxy-web-stack-23.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-06-08 17:44:05.000000 galaxy-web-stack-23.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-08 17:37:04.000000 galaxy-web-stack-23.0.1/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:11:53.000000 galaxy-web-stack-23.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-13 17:04:37.000000 galaxy-web-stack-23.0.2/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12875 2023-06-13 17:04:36.000000 galaxy-web-stack-23.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-13 17:04:37.000000 galaxy-web-stack-23.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-06-13 17:11:53.000000 galaxy-web-stack-23.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-13 17:04:37.000000 galaxy-web-stack-23.0.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-13 17:04:37.000000 galaxy-web-stack-23.0.2/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:11:53.000000 galaxy-web-stack-23.0.2/galaxy/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-13 17:04:37.000000 galaxy-web-stack-23.0.2/galaxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 17:04:37.000000 galaxy-web-stack-23.0.2/galaxy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:11:53.000000 galaxy-web-stack-23.0.2/galaxy/web_stack/
+-rw-r--r--   0 runner    (1001) docker     (123)    12414 2023-06-13 17:04:37.000000 galaxy-web-stack-23.0.2/galaxy/web_stack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-06-13 17:04:37.000000 galaxy-web-stack-23.0.2/galaxy/web_stack/gunicorn_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21744 2023-06-13 17:04:37.000000 galaxy-web-stack-23.0.2/galaxy/web_stack/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-06-13 17:04:37.000000 galaxy-web-stack-23.0.2/galaxy/web_stack/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-06-13 17:04:37.000000 galaxy-web-stack-23.0.2/galaxy/web_stack/transport.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:11:53.000000 galaxy-web-stack-23.0.2/galaxy_web_stack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-06-13 17:11:53.000000 galaxy-web-stack-23.0.2/galaxy_web_stack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-13 17:11:53.000000 galaxy-web-stack-23.0.2/galaxy_web_stack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 17:11:53.000000 galaxy-web-stack-23.0.2/galaxy_web_stack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-13 17:11:53.000000 galaxy-web-stack-23.0.2/galaxy_web_stack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-13 17:11:53.000000 galaxy-web-stack-23.0.2/galaxy_web_stack.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-13 17:04:37.000000 galaxy-web-stack-23.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-06-13 17:11:53.000000 galaxy-web-stack-23.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-13 17:04:37.000000 galaxy-web-stack-23.0.2/test-requirements.txt
```

### Comparing `galaxy-web-stack-23.0.1/LICENSE` & `galaxy-web-stack-23.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `galaxy-web-stack-23.0.1/PKG-INFO` & `galaxy-web-stack-23.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-web-stack
-Version: 23.0.1
+Version: 23.0.2
 Summary: Galaxy web stack abstraction
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -42,14 +42,20 @@
 
 History
 -------
 
 .. to_doc
 
 -------------------
+23.0.2 (2023-06-13)
+-------------------
+
+No recorded changes since last release
+
+-------------------
 23.0.1 (2023-06-08)
 -------------------
 
 No recorded changes since last release
 
 -------------------
 20.5.0 (2020-07-04)
```

### Comparing `galaxy-web-stack-23.0.1/galaxy/web_stack/__init__.py` & `galaxy-web-stack-23.0.2/galaxy/web_stack/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-stack-23.0.1/galaxy/web_stack/gunicorn_config.py` & `galaxy-web-stack-23.0.2/galaxy/web_stack/gunicorn_config.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-stack-23.0.1/galaxy/web_stack/handlers.py` & `galaxy-web-stack-23.0.2/galaxy/web_stack/handlers.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-stack-23.0.1/galaxy/web_stack/message.py` & `galaxy-web-stack-23.0.2/galaxy/web_stack/message.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-stack-23.0.1/galaxy/web_stack/transport.py` & `galaxy-web-stack-23.0.2/galaxy/web_stack/transport.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-stack-23.0.1/galaxy_web_stack.egg-info/PKG-INFO` & `galaxy-web-stack-23.0.2/galaxy_web_stack.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-web-stack
-Version: 23.0.1
+Version: 23.0.2
 Summary: Galaxy web stack abstraction
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -42,14 +42,20 @@
 
 History
 -------
 
 .. to_doc
 
 -------------------
+23.0.2 (2023-06-13)
+-------------------
+
+No recorded changes since last release
+
+-------------------
 23.0.1 (2023-06-08)
 -------------------
 
 No recorded changes since last release
 
 -------------------
 20.5.0 (2020-07-04)
```

### Comparing `galaxy-web-stack-23.0.1/setup.cfg` & `galaxy-web-stack-23.0.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 license = AFL
 license_files = 
 	LICENSE
 long_description = file: README.rst, HISTORY.rst
 long_description_content_type = text/x-rst
 name = galaxy-web-stack
 url = https://github.com/galaxyproject/galaxy
-version = 23.0.1
+version = 23.0.2
 
 [options]
 include_package_data = True
 install_requires = 
 	galaxy-util
 	SQLAlchemy>=1.4.25,<2
 packages = find:
```

