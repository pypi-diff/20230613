# Comparing `tmp/manylabels-0.0.3.tar.gz` & `tmp/manylabels-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manylabels-0.0.3.tar", last modified: Tue Jun 13 13:57:14 2023, max compression
+gzip compressed data, was "manylabels-0.0.4.tar", last modified: Tue Jun 13 14:07:05 2023, max compression
```

## Comparing `manylabels-0.0.3.tar` & `manylabels-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:57:14.287547 manylabels-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-13 13:56:50.000000 manylabels-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-13 13:56:50.000000 manylabels-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-13 13:57:14.287547 manylabels-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-13 13:56:50.000000 manylabels-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-13 13:56:50.000000 manylabels-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-06-13 13:57:14.287547 manylabels-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 13:56:50.000000 manylabels-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:57:14.283547 manylabels-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:57:14.283547 manylabels-0.0.3/src/manylabels/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-13 13:56:50.000000 manylabels-0.0.3/src/manylabels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5556 2023-06-13 13:56:50.000000 manylabels-0.0.3/src/manylabels/_manylabels.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:56:50.000000 manylabels-0.0.3/src/manylabels/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:57:14.283547 manylabels-0.0.3/src/manylabels.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-13 13:57:14.000000 manylabels-0.0.3/src/manylabels.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-13 13:57:14.000000 manylabels-0.0.3/src/manylabels.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 13:57:14.000000 manylabels-0.0.3/src/manylabels.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-13 13:57:14.000000 manylabels-0.0.3/src/manylabels.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:57:14.283547 manylabels-0.0.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-13 13:56:50.000000 manylabels-0.0.3/test/test_manylabels.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:07:05.119136 manylabels-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-13 14:06:37.000000 manylabels-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-13 14:06:37.000000 manylabels-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-06-13 14:07:05.119136 manylabels-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-13 14:06:37.000000 manylabels-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-13 14:06:37.000000 manylabels-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-13 14:07:05.119136 manylabels-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 14:06:37.000000 manylabels-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:07:05.115136 manylabels-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:07:05.119136 manylabels-0.0.4/src/manylabels/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-13 14:06:37.000000 manylabels-0.0.4/src/manylabels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5556 2023-06-13 14:06:37.000000 manylabels-0.0.4/src/manylabels/_manylabels.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 14:06:37.000000 manylabels-0.0.4/src/manylabels/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:07:05.119136 manylabels-0.0.4/src/manylabels.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-06-13 14:07:05.000000 manylabels-0.0.4/src/manylabels.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-13 14:07:05.000000 manylabels-0.0.4/src/manylabels.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 14:07:05.000000 manylabels-0.0.4/src/manylabels.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-13 14:07:05.000000 manylabels-0.0.4/src/manylabels.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:07:05.119136 manylabels-0.0.4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-13 14:06:37.000000 manylabels-0.0.4/test/test_manylabels.py
```

### Comparing `manylabels-0.0.3/PKG-INFO` & `manylabels-0.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: manylabels
-Version: 0.0.3
+Version: 0.0.4
 Summary: Automatically add multiple x-axis labels to your matplotlib subplots.
-Home-page: https://github.com/daneah/publishing-python-packages
+Home-page: https://github.com/mshumko/manylabels
 Author: Mykhaylo Shumko
 Author-email: "Mykhaylo Shumko" <msshumko@gmail.com>
 License: GNU General Public License v3 (GPLv3)
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-![manylabels collage](./docs/_static/manylabels_collage.png)
+![manylabels collage](https://github.com/mshumko/manylabels/blob/main/docs/_static/manylabels_collage.png?raw=true)
 
 # manylabels
 
 Many plots in the heliophysics science community are of satellites showing various physical 
 observations. To place these observations in context, scientists often include multiple
 x-axis labels showing, for example, the satellite location. This is surprisingly hard to implement using matplotlib. Nevertheless, `manylabels.ManyLabels()` class provides this functionality.
```

### Comparing `manylabels-0.0.3/README.md` & `manylabels-0.0.4/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-![manylabels collage](./docs/_static/manylabels_collage.png)
+![manylabels collage](https://github.com/mshumko/manylabels/blob/main/docs/_static/manylabels_collage.png?raw=true)
 
 # manylabels
 
 Many plots in the heliophysics science community are of satellites showing various physical 
 observations. To place these observations in context, scientists often include multiple
 x-axis labels showing, for example, the satellite location. This is surprisingly hard to implement using matplotlib. Nevertheless, `manylabels.ManyLabels()` class provides this functionality.
```

### Comparing `manylabels-0.0.3/setup.cfg` & `manylabels-0.0.4/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [metadata]
 name = manylabels
-version = 0.0.3
+version = 0.0.4
 description = Automatically add multiple x-axis labels to your matplotlib subplots.
 long_description = file: README.md
 long_description_content_type = text/markdown
-url = https://github.com/daneah/publishing-python-packages
+url = https://github.com/mshumko/manylabels
 author = Mykhaylo Shumko
 author_email = "Mykhaylo Shumko" <msshumko@gmail.com>
 license = GNU General Public License v3 (GPLv3)
 license_files = LICENSE
 classifiers = 
 	License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `manylabels-0.0.3/src/manylabels/_manylabels.py` & `manylabels-0.0.4/src/manylabels/_manylabels.py`

 * *Files identical despite different names*

### Comparing `manylabels-0.0.3/src/manylabels.egg-info/PKG-INFO` & `manylabels-0.0.4/src/manylabels.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: manylabels
-Version: 0.0.3
+Version: 0.0.4
 Summary: Automatically add multiple x-axis labels to your matplotlib subplots.
-Home-page: https://github.com/daneah/publishing-python-packages
+Home-page: https://github.com/mshumko/manylabels
 Author: Mykhaylo Shumko
 Author-email: "Mykhaylo Shumko" <msshumko@gmail.com>
 License: GNU General Public License v3 (GPLv3)
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-![manylabels collage](./docs/_static/manylabels_collage.png)
+![manylabels collage](https://github.com/mshumko/manylabels/blob/main/docs/_static/manylabels_collage.png?raw=true)
 
 # manylabels
 
 Many plots in the heliophysics science community are of satellites showing various physical 
 observations. To place these observations in context, scientists often include multiple
 x-axis labels showing, for example, the satellite location. This is surprisingly hard to implement using matplotlib. Nevertheless, `manylabels.ManyLabels()` class provides this functionality.
```

### Comparing `manylabels-0.0.3/test/test_manylabels.py` & `manylabels-0.0.4/test/test_manylabels.py`

 * *Files identical despite different names*

