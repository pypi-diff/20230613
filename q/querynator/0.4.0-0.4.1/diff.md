# Comparing `tmp/querynator-0.4.0.tar.gz` & `tmp/querynator-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "querynator-0.4.0.tar", last modified: Wed May 31 13:06:10 2023, max compression
+gzip compressed data, was "querynator-0.4.1.tar", last modified: Tue Jun 13 14:19:40 2023, max compression
```

## Comparing `querynator-0.4.0.tar` & `querynator-0.4.1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:06:10.857042 querynator-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-05-31 13:05:13.000000 querynator-0.4.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-05-31 13:05:13.000000 querynator-0.4.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-31 13:05:13.000000 querynator-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-31 13:05:13.000000 querynator-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6082 2023-05-31 13:06:10.857042 querynator-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-05-31 13:05:13.000000 querynator-0.4.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:06:10.857042 querynator-0.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-31 13:05:13.000000 querynator-0.4.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-31 13:05:13.000000 querynator-0.4.0/docs/changelog.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     4881 2023-05-31 13:05:13.000000 querynator-0.4.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-31 13:05:13.000000 querynator-0.4.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-31 13:05:13.000000 querynator-0.4.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-31 13:05:13.000000 querynator-0.4.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-31 13:05:13.000000 querynator-0.4.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-31 13:05:13.000000 querynator-0.4.0/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-31 13:05:13.000000 querynator-0.4.0/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9198 2023-05-31 13:05:13.000000 querynator-0.4.0/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-31 13:05:13.000000 querynator-0.4.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:06:10.857042 querynator-0.4.0/querynator/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-31 13:05:13.000000 querynator-0.4.0/querynator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15304 2023-05-31 13:05:13.000000 querynator-0.4.0/querynator/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:06:10.857042 querynator-0.4.0/querynator/helper_functions/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-31 13:05:13.000000 querynator-0.4.0/querynator/helper_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-05-31 13:05:13.000000 querynator-0.4.0/querynator/helper_functions/helper_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:06:10.857042 querynator-0.4.0/querynator/query_api/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-31 13:05:13.000000 querynator-0.4.0/querynator/query_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7952 2023-05-31 13:05:13.000000 querynator-0.4.0/querynator/query_api/cancertypes.js
--rw-r--r--   0 runner    (1001) docker     (123)     8423 2023-05-31 13:05:13.000000 querynator-0.4.0/querynator/query_api/cgi_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19214 2023-05-31 13:05:13.000000 querynator-0.4.0/querynator/query_api/civic_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:06:10.857042 querynator-0.4.0/querynator/report_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-31 13:05:13.000000 querynator-0.4.0/querynator/report_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11756 2023-05-31 13:05:13.000000 querynator-0.4.0/querynator/report_scripts/combine_cgi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-05-31 13:05:13.000000 querynator-0.4.0/querynator/report_scripts/combine_cgi_civic.py
--rw-r--r--   0 runner    (1001) docker     (123)     9132 2023-05-31 13:05:13.000000 querynator-0.4.0/querynator/report_scripts/combine_civic.py
--rw-r--r--   0 runner    (1001) docker     (123)    24775 2023-05-31 13:05:13.000000 querynator-0.4.0/querynator/report_scripts/create_report.py
--rw-r--r--   0 runner    (1001) docker     (123)    16843 2023-05-31 13:05:13.000000 querynator-0.4.0/querynator/report_scripts/sort_variants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:06:10.857042 querynator-0.4.0/querynator/report_scripts/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-05-31 13:05:13.000000 querynator-0.4.0/querynator/report_scripts/templates/template_individual.html
--rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-05-31 13:05:13.000000 querynator-0.4.0/querynator/report_scripts/templates/template_overall_plotly_pieplots.html
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-05-31 13:05:13.000000 querynator-0.4.0/querynator/report_scripts/templates/template_overall_upsetplots.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:06:10.857042 querynator-0.4.0/querynator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6082 2023-05-31 13:06:10.000000 querynator-0.4.0/querynator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-31 13:06:10.000000 querynator-0.4.0/querynator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 13:06:10.000000 querynator-0.4.0/querynator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-31 13:06:10.000000 querynator-0.4.0/querynator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 13:05:25.000000 querynator-0.4.0/querynator.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-31 13:06:10.000000 querynator-0.4.0/querynator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-31 13:06:10.000000 querynator-0.4.0/querynator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-31 13:05:13.000000 querynator-0.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 13:06:10.857042 querynator-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-05-31 13:05:13.000000 querynator-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:06:10.857042 querynator-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-31 13:05:13.000000 querynator-0.4.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-05-31 13:05:13.000000 querynator-0.4.0/tests/test_querynator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:19:40.286818 querynator-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-06-13 14:18:53.000000 querynator-0.4.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-06-13 14:18:53.000000 querynator-0.4.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-13 14:18:53.000000 querynator-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-13 14:18:53.000000 querynator-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-06-13 14:19:40.286818 querynator-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-06-13 14:18:53.000000 querynator-0.4.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:19:40.278818 querynator-0.4.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-13 14:18:53.000000 querynator-0.4.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-13 14:18:53.000000 querynator-0.4.1/docs/changelog.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4881 2023-06-13 14:18:53.000000 querynator-0.4.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-13 14:18:53.000000 querynator-0.4.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-13 14:18:53.000000 querynator-0.4.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-06-13 14:18:53.000000 querynator-0.4.1/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-13 14:18:53.000000 querynator-0.4.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-06-13 14:18:53.000000 querynator-0.4.1/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-13 14:18:53.000000 querynator-0.4.1/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9198 2023-06-13 14:18:53.000000 querynator-0.4.1/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-13 14:18:53.000000 querynator-0.4.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:19:40.278818 querynator-0.4.1/querynator/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-13 14:18:53.000000 querynator-0.4.1/querynator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15304 2023-06-13 14:18:53.000000 querynator-0.4.1/querynator/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:19:40.282818 querynator-0.4.1/querynator/helper_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-13 14:18:53.000000 querynator-0.4.1/querynator/helper_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-06-13 14:18:53.000000 querynator-0.4.1/querynator/helper_functions/helper_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:19:40.282818 querynator-0.4.1/querynator/query_api/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-13 14:18:53.000000 querynator-0.4.1/querynator/query_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7952 2023-06-13 14:18:53.000000 querynator-0.4.1/querynator/query_api/cancertypes.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8423 2023-06-13 14:18:53.000000 querynator-0.4.1/querynator/query_api/cgi_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23131 2023-06-13 14:18:53.000000 querynator-0.4.1/querynator/query_api/civic_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:19:40.286818 querynator-0.4.1/querynator/report_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-13 14:18:53.000000 querynator-0.4.1/querynator/report_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11756 2023-06-13 14:18:53.000000 querynator-0.4.1/querynator/report_scripts/combine_cgi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-06-13 14:18:53.000000 querynator-0.4.1/querynator/report_scripts/combine_cgi_civic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9132 2023-06-13 14:18:53.000000 querynator-0.4.1/querynator/report_scripts/combine_civic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26968 2023-06-13 14:18:53.000000 querynator-0.4.1/querynator/report_scripts/create_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17134 2023-06-13 14:18:53.000000 querynator-0.4.1/querynator/report_scripts/sort_variants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:19:40.286818 querynator-0.4.1/querynator/report_scripts/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-06-13 14:18:53.000000 querynator-0.4.1/querynator/report_scripts/templates/template_individual.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-06-13 14:18:53.000000 querynator-0.4.1/querynator/report_scripts/templates/template_overall_plotly_pieplots.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-06-13 14:18:53.000000 querynator-0.4.1/querynator/report_scripts/templates/template_overall_upsetplots.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:19:40.282818 querynator-0.4.1/querynator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-06-13 14:19:40.000000 querynator-0.4.1/querynator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-06-13 14:19:40.000000 querynator-0.4.1/querynator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 14:19:40.000000 querynator-0.4.1/querynator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-13 14:19:40.000000 querynator-0.4.1/querynator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 14:18:59.000000 querynator-0.4.1/querynator.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-13 14:19:40.000000 querynator-0.4.1/querynator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-13 14:19:40.000000 querynator-0.4.1/querynator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-13 14:18:53.000000 querynator-0.4.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 14:19:40.286818 querynator-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-13 14:18:53.000000 querynator-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:19:40.286818 querynator-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-13 14:18:53.000000 querynator-0.4.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-06-13 14:18:53.000000 querynator-0.4.1/tests/test_querynator.py
```

### Comparing `querynator-0.4.0/CHANGELOG.rst` & `querynator-0.4.1/CHANGELOG.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,23 @@
 Changelog
 ============
 
+0.4.1 - Stormy Saturn  (2023-06-13)
+---------------------------------------------
+
+**Added**
+
+**Fixed**
+
+* Bug fixes to include all evidence of CIViC
+
+**Dependencies**
+
+**Deprecated**
+
 0.4.0 - Stormy Saturn  (2023-05-31)
 ---------------------------------------------
 
 **Added**
 
 **Fixed**
```

### Comparing `querynator-0.4.0/CONTRIBUTING.rst` & `querynator-0.4.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `querynator-0.4.0/LICENSE` & `querynator-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `querynator-0.4.0/PKG-INFO` & `querynator-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: querynator
-Version: 0.4.0
+Version: 0.4.1
 Summary: Python package to query cancer variant databases
 Home-page: https://github.com/qbic-pipelines/querynator
 Author: Susanne Jodoin, Mark Polster
 Author-email: susanne.jodoin@qbic.uni-tuebingen.de, mark.polster@uni-tuebingen.de
 License: MIT license
 Keywords: querynator
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -76,14 +76,27 @@
 
 
 
 
 Changelog
 ============
 
+0.4.1 - Stormy Saturn  (2023-06-13)
+---------------------------------------------
+
+**Added**
+
+**Fixed**
+
+* Bug fixes to include all evidence of CIViC
+
+**Dependencies**
+
+**Deprecated**
+
 0.4.0 - Stormy Saturn  (2023-05-31)
 ---------------------------------------------
 
 **Added**
 
 **Fixed**
```

### Comparing `querynator-0.4.0/README.rst` & `querynator-0.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `querynator-0.4.0/docs/Makefile` & `querynator-0.4.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `querynator-0.4.0/docs/conf.py` & `querynator-0.4.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `querynator-0.4.0/docs/installation.rst` & `querynator-0.4.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `querynator-0.4.0/docs/make.bat` & `querynator-0.4.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `querynator-0.4.0/docs/modules.rst` & `querynator-0.4.1/docs/modules.rst`

 * *Files identical despite different names*

### Comparing `querynator-0.4.0/docs/usage.rst` & `querynator-0.4.1/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `querynator-0.4.0/querynator/__main__.py` & `querynator-0.4.1/querynator/__main__.py`

 * *Files identical despite different names*

### Comparing `querynator-0.4.0/querynator/helper_functions/helper_functions.py` & `querynator-0.4.1/querynator/helper_functions/helper_functions.py`

 * *Files identical despite different names*

### Comparing `querynator-0.4.0/querynator/query_api/cancertypes.js` & `querynator-0.4.1/querynator/query_api/cancertypes.js`

 * *Files identical despite different names*

### Comparing `querynator-0.4.0/querynator/query_api/cgi_api.py` & `querynator-0.4.1/querynator/query_api/cgi_api.py`

 * *Files identical despite different names*

### Comparing `querynator-0.4.0/querynator/query_api/civic_api.py` & `querynator-0.4.1/querynator/query_api/civic_api.py`

 * *Files 16% similar despite different names*

```diff
@@ -140,14 +140,61 @@
                         ): querynator_id
                     }
                 )
 
     return coord_dict
 
 
+def append_to_dict(dict1, dict2):
+    """
+    appends values of a dictionary to another dictionary with lists as values
+    :param dict1: dictionary to append to
+    :type dict1: dict
+    :param dict2: dictionary with values to append
+    :type: dict2: dict
+    :return: appended dict
+    :rtype: dict
+    """
+    for key, value in dict2.items():
+        if key in dict1:
+            if type(dict1[key]) == list:
+                dict1[key].append(value)
+            else:
+                if dict1[key] == "":
+                    dict1[key] = dict2[key]
+                else:
+                    dict1[key] = [dict1[key], dict2[key]]
+
+    return dict1
+
+
+def smoothen_dict(dict, s):
+    """
+    makes string out of lists
+
+    :param dict: dict with lists as values
+    :type dict: dict
+    :param s: True if string and special string character needed
+    :type s: bool
+    :return: dict with strings as values
+    :rtype: dict
+    """
+    for key in dict:
+        if type(dict[key]) == list:
+            filtered_list = [i if i is not None else "" for i in dict[key]]
+            if s:
+                if key in ["evidence_source", "evidence_description"]:
+                    dict[key] = "|".join(str(i) for i in filtered_list)
+                else:
+                    dict[key] = ",".join(str(i) for i in filtered_list)
+            else:
+                dict[key] = ",".join(str(i) for i in filtered_list)
+    return dict
+
+
 def access_civic_by_coordinate(coord_dict, logger, build):
     """
     Query CIViC API for individual variants
 
     :param coord_list: List of CoordinateQuery objects
     :type coord_list: list
     :param build: reference genome
@@ -209,24 +256,29 @@
     Get all molecular profile information from a single CIViC variant object
 
     :param variant_obj: single CIViC variant object
     :type variant_ob: CIViC variant object
     :return: Molecular profile information for respective CIViC variant object
     :rtype: dict
     """
-    try:
-        mol_profile = variant_obj.molecular_profiles[0]
-        mol_profile_dict = {
-            "mol_profile_name": mol_profile.name,
-            "mol_profile_definition": mol_profile.description,
-            "mol_profile_score": mol_profile.molecular_profile_score,
-        }
-    except IndexError:
-        mol_profile_dict = {"mol_profile_name": None, "mol_profile_definition": None, "mol_profile_score": None}
-    return mol_profile_dict
+    mol_profile_dict = {"mol_profile_name": "", "mol_profile_definition": "", "mol_profile_score": ""}
+
+    for mol_profile in variant_obj.molecular_profiles:
+        try:
+            # mol_profile = variant_obj.molecular_profiles[0]
+            new_dict = {
+                "mol_profile_name": mol_profile.name,
+                "mol_profile_definition": mol_profile.description,
+                "mol_profile_score": mol_profile.molecular_profile_score,
+            }
+        except IndexError:
+            new_dict = {"mol_profile_name": None, "mol_profile_definition": None, "mol_profile_score": None}
+        mol_profile_dict = append_to_dict(mol_profile_dict, new_dict)
+
+    return smoothen_dict(mol_profile_dict, False)
 
 
 def get_gene_information_from_variant(variant_obj):
     """
     Get all gene information from a single CIViC variant object
 
     :param variant_obj: single CIViC variant object
@@ -249,107 +301,152 @@
     Get all assertion information from a single CIViC variant object
 
     :param variant_obj: single CIViC variant object
     :type variant_ob: CIViC variant object
     :return: Assertion information for respective CIViC variant object
     :rtype: dict
     """
-    try:
-        assertion = variant_obj.molecular_profiles[0].assertions[0]
-        assertion_dict = {
-            "assertion_name": assertion.name,
-            "assertion_acmg_codes": ", ".join([i.code for i in assertion.acmg_codes]),
-            "assertion_acmg_codes_description": ", ".join([i.description for i in assertion.acmg_codes]),
-            "assertion_amp_level": assertion.amp_level,
-            "assertion_direction": assertion.assertion_direction,
-            "assertion_type": assertion.assertion_type,
-            "assertion_description": assertion.description,
-            "assertion_disease_name": ", ".join([i.name for i in assertion.disease]),
-            "assertion_disease_doid": ", ".join([i.doid for i in assertion.disease]),
-            "assertion_disease_url": ", ".join([i.disease_url for i in assertion.disease]),
-            "assertion_disease_aliases": ", ".join([i.aliases for i in assertion.disease]),
-            "assertion_phenotypes": ", ".join([i.name for i in assertion.phenotypes]),
-            "assertion_significance": assertion.significance,
-            "assertion_status": assertion.status,
-            "assertion_summary": assertion.summary,
-            "assertion_therapies_name": ", ".join([i.name for i in assertion.therapies]),
-            "assertion_therapies_ncit_id": ", ".join([i.ncit_id for i in assertion.therapies]),
-            "assertion_therapies_aliases": ", ".join([", ".join(i.aliases) for i in assertion.therapies]),
-            "assertion_therapies_interaction_type": assertion.therapy_interaction_type,
-            "assertion_variant_origin": assertion.variant_origin,
-        }
-    except IndexError:
-        assertion_dict = {
-            "assertion_name": np.nan,
-            "assertion_acmg_codes": np.nan,
-            "assertion_acmg_codes_description": np.nan,
-            "assertion_amp_level": np.nan,
-            "assertion_direction": np.nan,
-            "assertion_type": np.nan,
-            "assertion_description": np.nan,
-            "assertion_disease_name": np.nan,
-            "assertion_disease_doid": np.nan,
-            "assertion_disease_url": np.nan,
-            "assertion_disease_aliases": np.nan,
-            "assertion_phenotypes": np.nan,
-            "assertion_significance": np.nan,
-            "assertion_status": np.nan,
-            "assertion_summary": np.nan,
-            "assertion_therapies_name": np.nan,
-            "assertion_therapies_ncit_id": np.nan,
-            "assertion_therapies_aliases": np.nan,
-            "assertion_therapies_interaction_type": np.nan,
-            "assertion_variant_origin": np.nan,
-        }
-    return assertion_dict
+    assertion_dict = {
+        "assertion_name": "",
+        "assertion_acmg_codes": "",
+        "assertion_acmg_codes_description": "",
+        "assertion_amp_level": "",
+        "assertion_direction": "",
+        "assertion_type": "",
+        "assertion_description": "",
+        "assertion_disease_name": "",
+        "assertion_disease_doid": "",
+        "assertion_disease_url": "",
+        "assertion_disease_aliases": "",
+        "assertion_phenotypes": "",
+        "assertion_significance": "",
+        "assertion_status": "",
+        "assertion_summary": "",
+        "assertion_therapies_name": "",
+        "assertion_therapies_ncit_id": "",
+        "assertion_therapies_aliases": "",
+        "assertion_therapies_interaction_type": "",
+        "assertion_variant_origin": "",
+    }
+    for mol_prof in variant_obj.molecular_profiles:
+        for assertion in mol_prof.assertions:
+            try:
+                new_dict = {
+                    "assertion_name": assertion.name,
+                    "assertion_acmg_codes": ", ".join([i.code for i in assertion.acmg_codes]),
+                    "assertion_acmg_codes_description": ", ".join([i.description for i in assertion.acmg_codes]),
+                    "assertion_amp_level": assertion.amp_level,
+                    "assertion_direction": assertion.assertion_direction,
+                    "assertion_type": assertion.assertion_type,
+                    "assertion_description": assertion.description,
+                    "assertion_disease_name": ", ".join([i.name for i in assertion.disease]),
+                    "assertion_disease_doid": ", ".join([i.doid for i in assertion.disease]),
+                    "assertion_disease_url": ", ".join([i.disease_url for i in assertion.disease]),
+                    "assertion_disease_aliases": ", ".join([i.aliases for i in assertion.disease]),
+                    "assertion_phenotypes": ", ".join([i.name for i in assertion.phenotypes]),
+                    "assertion_significance": assertion.significance,
+                    "assertion_status": assertion.status,
+                    "assertion_summary": assertion.summary,
+                    "assertion_therapies_name": ", ".join([i.name for i in assertion.therapies]),
+                    "assertion_therapies_ncit_id": ", ".join([i.ncit_id for i in assertion.therapies]),
+                    "assertion_therapies_aliases": ", ".join([", ".join(i.aliases) for i in assertion.therapies]),
+                    "assertion_therapies_interaction_type": assertion.therapy_interaction_type,
+                    "assertion_variant_origin": assertion.variant_origin,
+                }
+            except IndexError:
+                new_dict = {
+                    "assertion_name": np.nan,
+                    "assertion_acmg_codes": np.nan,
+                    "assertion_acmg_codes_description": np.nan,
+                    "assertion_amp_level": np.nan,
+                    "assertion_direction": np.nan,
+                    "assertion_type": np.nan,
+                    "assertion_description": np.nan,
+                    "assertion_disease_name": np.nan,
+                    "assertion_disease_doid": np.nan,
+                    "assertion_disease_url": np.nan,
+                    "assertion_disease_aliases": np.nan,
+                    "assertion_phenotypes": np.nan,
+                    "assertion_significance": np.nan,
+                    "assertion_status": np.nan,
+                    "assertion_summary": np.nan,
+                    "assertion_therapies_name": np.nan,
+                    "assertion_therapies_ncit_id": np.nan,
+                    "assertion_therapies_aliases": np.nan,
+                    "assertion_therapies_interaction_type": np.nan,
+                    "assertion_variant_origin": np.nan,
+                }
+            assertion_dict = append_to_dict(assertion_dict, new_dict)
+    return smoothen_dict(assertion_dict, False)
 
 
 def get_evidence_information_from_variant(variant_obj):
     """
     Get all evidence from a single CIViC variant object
 
     :param variant_obj: single CIViC variant object
     :type variant_ob: CIViC variant object
     :return: Evidence information for respective CIViC variant object
     :rtype: dict
     """
-    try:
-        evidence = variant_obj.molecular_profiles[0].assertions[0].evidence[0]
-        evidence_dict = {
-            "evidence_name": evidence.name,
-            "evidence_description": evidence.description,
-            "evidence_disease": evidence.disease,
-            "evidence_level": evidence.evidence_level,
-            "evidence_support": evidence.evidence_direction,
-            "evidence_type": evidence.evidence_type,
-            "evidence_phenotypes": ", ".join([i.name for i in evidence.phenotypes]),
-            "evidence_rating": evidence.rating,
-            "evidence_significance": evidence.significance,
-            "evidence_source": evidence.source,
-            "evidence_status": evidence.status,
-            "evidence_therapies": ", ".join([i.name for i in evidence.therapies]),
-            "evidence_therapy_interaction_type": evidence.therapy_interaction_type,
-        }
-    except IndexError:
-        evidence_dict = {
-            "evidence_name": np.nan,
-            "evidence_description": np.nan,
-            "evidence_disease": np.nan,
-            "evidence_level": np.nan,
-            "evidence_support": np.nan,
-            "evidence_type": np.nan,
-            "evidence_phenotypes": np.nan,
-            "evidence_rating": np.nan,
-            "evidence_significance": np.nan,
-            "evidence_source": np.nan,
-            "evidence_status": np.nan,
-            "evidence_therapies": np.nan,
-            "evidence_therapy_interaction_type": np.nan,
-        }
-    return evidence_dict
+
+    evidence_dict = {
+        "evidence_name": "",
+        "evidence_description": "",
+        "evidence_disease": "",
+        "evidence_level": "",
+        "evidence_support": "",
+        "evidence_type": "",
+        "evidence_phenotypes": "",
+        "evidence_rating": "",
+        "evidence_significance": "",
+        "evidence_source": "",
+        "evidence_status": "",
+        "evidence_therapies": "",
+        "evidence_therapy_interaction_type": "",
+    }
+
+    for mol_prof in variant_obj.molecular_profiles:
+        for evidence in mol_prof.evidence:
+            try:
+                # evidence = variant_obj.molecular_profiles[0].evidence[0]
+                new_dict = {
+                    "evidence_name": evidence.name,
+                    "evidence_description": evidence.description,
+                    "evidence_disease": evidence.disease.name if type(evidence.disease) != dict else np.nan,
+                    "evidence_level": evidence.evidence_level,
+                    "evidence_support": evidence.evidence_direction,
+                    "evidence_type": evidence.evidence_type,
+                    "evidence_phenotypes": ", ".join([i.name for i in evidence.phenotypes]),
+                    "evidence_rating": evidence.rating,
+                    "evidence_significance": evidence.significance,
+                    "evidence_source": evidence.source.name,
+                    "evidence_status": evidence.status,
+                    "evidence_therapies": ", ".join([i.name for i in evidence.therapies]),
+                    "evidence_therapy_interaction_type": evidence.therapy_interaction_type,
+                }
+            except IndexError:
+                new_dict = {
+                    "evidence_name": np.nan,
+                    "evidence_description": np.nan,
+                    "evidence_disease": np.nan,
+                    "evidence_level": np.nan,
+                    "evidence_support": np.nan,
+                    "evidence_type": np.nan,
+                    "evidence_phenotypes": np.nan,
+                    "evidence_rating": np.nan,
+                    "evidence_significance": np.nan,
+                    "evidence_source": np.nan,
+                    "evidence_status": np.nan,
+                    "evidence_therapies": np.nan,
+                    "evidence_therapy_interaction_type": np.nan,
+                }
+            evidence_dict = append_to_dict(evidence_dict, new_dict)
+
+    return smoothen_dict(evidence_dict, True)
 
 
 def get_positional_information_from_coord_obj(coord_obj):
     """
     Get information about the position of the variant in the genome
 
     :param coord_obj: CoordinateQuery Object to respective variant object
```

### Comparing `querynator-0.4.0/querynator/report_scripts/combine_cgi.py` & `querynator-0.4.1/querynator/report_scripts/combine_cgi.py`

 * *Files identical despite different names*

### Comparing `querynator-0.4.0/querynator/report_scripts/combine_cgi_civic.py` & `querynator-0.4.1/querynator/report_scripts/combine_cgi_civic.py`

 * *Files identical despite different names*

### Comparing `querynator-0.4.0/querynator/report_scripts/combine_civic.py` & `querynator-0.4.1/querynator/report_scripts/combine_civic.py`

 * *Files identical despite different names*

### Comparing `querynator-0.4.0/querynator/report_scripts/create_report.py` & `querynator-0.4.1/querynator/report_scripts/create_report.py`

 * *Files 6% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     """
     cgi_str = "-"
     civic_str = "-"
     if not pd.isnull(row["evidence_CGI"]):
         cgi_str = row["evidence_CGI"]
 
     if not pd.isnull(row["evidence_level_CIVIC"]):
-        civic_str = row["evidence_level_CIVIC"]
+        civic_str = min(row["evidence_level_CIVIC"].split(","))
 
     return f"{cgi_str}(cgi), {civic_str}(civic)"
 
 
 def get_disease_names_CIViC(row):
     """
     Get CIViC's disease names for the variant
@@ -82,18 +82,19 @@
 
     disease_rows = [
         row["evidence_phenotypes_CIVIC"],
         row["assertion_phenotypes_CIVIC"],
         row["evidence_disease_CIVIC"],
         row["assertion_disease_name_CIVIC"],
     ]
+
     disease_list = [i for i in disease_rows if not pd.isnull(i)]
 
     if disease_list != []:
-        return ", ".join([i for i in disease_list])
+        return ", ".join([i for i in disease_list]).replace("nan", "")
     else:
         return ""
 
 
 def get_therapy_names(row, civic_only):
     """
     Get the therapy names for the variant
@@ -101,21 +102,22 @@
     :param row: Row of the variant dataframe
     :type row: pandas DataFrame row
     """
     therapy_str = ""
     therapy_rows = [row["assertion_therapies_name_CIVIC"], row["evidence_therapies_CIVIC"]]
     therapy_list = [i.split(",") for i in therapy_rows if not pd.isnull(i)]
     if therapy_list != []:
-        therapy_list = [i.strip() for i in flatten(therapy_list)]
-        therapy_str = ", ".join([i for i in set(therapy_list)])
-    if not pd.isnull(row["evidence_CGI"]) and not civic_only:
-        if therapy_list != []:
-            therapy_str = therapy_str + ", CGI (see Details)"
-        else:
-            therapy_str = "CGI (see Details)"
+        therapy_list = set([i.strip() for i in flatten(therapy_list)])
+        therapy_str = ", ".join([i for i in set(therapy_list) if not i == ""])
+    if not pd.isnull(row["evidence_CGI"]):
+        if not civic_only:
+            if therapy_list != []:
+                therapy_str = therapy_str + ", CGI (see Details)"
+            else:
+                therapy_str = "CGI (see Details)"
     else:
         return ""
 
     return therapy_str
 
 
 def add_variant_name_report(df):
@@ -259,14 +261,26 @@
     tmpfile = BytesIO()
     fig.savefig(tmpfile, format="png")
     encoded = base64.b64encode(tmpfile.getvalue()).decode("utf-8")
 
     return "<img src='data:image/png;base64,{}'>".format(encoded)
 
 
+def remove_dups(row):
+    """
+    Removes duplicates from string
+
+    :param row: row of pd DataFrame
+    :type row: pd Series
+    :return: row without duplicates
+    :rtype: pd Series
+    """
+    return ", ".join(list(set(row.split(","))))
+
+
 def create_tier_table(df, tier, report_path):
     """
     Creates a table for the report for the given tier
 
     :param df: df containing all variants
     :type df: pandas DataFrame
     :param tier: tier to create the table for
@@ -305,19 +319,24 @@
             "Oncogenic Summary_CGI": "Oncogenicity",
             "disease_names_report": "Disease Name",
             "therapy_names_report": "Therapies",
             "evidence_levels_comb": "Evidence Level",
             "report_link": "Details",
         }
     )
+
+    # remove duplicates from therapies & diseases
+    tier_report_subset["Therapies"] = tier_report_subset["Therapies"].apply(lambda x: remove_dups(x))
+    tier_report_subset["Disease Name"] = tier_report_subset["Disease Name"].apply(lambda x: remove_dups(x))
+
     html_table = build_table(
         tier_report_subset,
         color="blue_light",
         escape=False,
-        width_dict=["100px", "300px", "200px", "200px", "200px", "100px", "auto"],
+        width_dict=["50px", "200px", "100px", "500px", "500px", "100px", "auto"],
         text_align="center",
     )
 
     return html_table
 
 
 def write_overall_report(template_html, report_html, fig_kb, fig_tiers, tier_table_list):
@@ -436,44 +455,86 @@
                 width_dict=width_dict,
             )
 
     else:
         return ""
 
 
-def create_evidence_table(row):
+def split_cols(col, col_name):
+    """
+    splits specific string cols differently
+
+    :param col: The column of the dataframe.
+    :type row: pandas.Series
+    :param col_name: the name of the column
+    :type: col_name: str
+    :return: Split column
+    :rtype: pandas.Series
+    """
+    if col_name not in ["evidence_description_CIVIC", "evidence_source_CIVIC"]:
+        return col.astype(str).str.split(",")
+    else:
+        return col.astype(str).str.split(".,")
+
+
+def create_evidence_table(row, width_dict):
     """
     Creates a table containing CIViC evidence information for a specific variant.
     :param row: The row of the dataframe.
     :type row: pandas.Series
+    :param width_dict: A list containing the width of each column.
+    :type width_dict: list
     """
     evidence_subset = (
         row.loc[
             [
                 "evidence_name_CIVIC",
                 "evidence_type_CIVIC",
                 "evidence_level_CIVIC",
-                "evidence_rating_CIVIC",
                 "evidence_significance_CIVIC",
                 "evidence_support_CIVIC",
+                "evidence_disease_CIVIC",
+                "evidence_description_CIVIC",
+                "evidence_source_CIVIC",
             ]
         ]
         .to_frame()
         .T
     )
-    evidence_subset.columns = ["Name", "Level", "Rating", "Type", "Significance", "Direction"]
-    if len(evidence_subset) > 0:
-        return build_table(evidence_subset, color="blue_light", escape=False)
+    evidence_subset.columns = ["Name", "Type", "Level", "Significance", "Direction", "Disease", "Description", "Source"]
+    # drop completly nan rows
+    evidence_subset = evidence_subset.dropna(how="all")
+    if not evidence_subset.empty:
+        evidence_cols = evidence_subset.columns
+        exploded_data = []
+        for _, row in evidence_subset.iterrows():
+            # replace nan values with empty string
+            row = row.fillna("")
+            # explode row --> split the individual evidence annotations and create a single col for each
+            exploded_row = pd.DataFrame(
+                data=[
+                    pd.Series(row[col].split(","))
+                    if col not in ["Description", "Source"]
+                    else pd.Series(row[col].split("|"))
+                    for col in evidence_cols
+                ],
+                index=evidence_cols,
+            ).T
+            exploded_data.append(exploded_row)
+
+        evidence_subset = pd.concat(exploded_data, ignore_index=True).sort_values("Level", ascending=True)
+        return build_table(evidence_subset, color="blue_light", escape=False, width_dict=width_dict)
     else:
         return ""
 
 
 def create_therapy_table(row, response, width_dict, biomarkers_df):
     """
     Creates a HTML table containing all Therapy & Drug related information provided by CGI for a specific Protein Change.
+
     :param row: The row of the dataframe.
     :type row: pandas.Series
     :param response: The response to a specific drug.
     :type response: str
     :param width_dict: A list containing the width of each column.
     :type width_dict: list
     :param biomarkers_df: The biomarkers dataframe from CGI.
@@ -500,14 +561,26 @@
     with open(metadata_path, "r") as f:
         for line in f:
             if line.startswith("Reference genome"):
                 return line.split(":")[1].strip()
         return ""
 
 
+def get_evidence_description(row):
+    """
+    takes in string of evidence descriptions and returns them as a HTML list
+
+    :param row: row of the dataframe
+    :type row: pandas.core.series.Series
+    :return: string of evidence descriptions
+    :rtype: str
+    """
+    pass
+
+
 def retrieve_info_from_row(row, biomarkers_df, metadata_path):
     """
     This function retrieves the information from a row of the merged dataframe
     and returns a dictionary with the information for the report of a specific variant.
 
     :param row: row of the dataframe
     :type row: pandas.core.series.Series
@@ -551,32 +624,31 @@
     info_dict["PROT_CHANGE"] = check_if_nan(row["Protein Change_CGI"])
     info_dict["CIVIC_CGI_PRESENT"] = check_if_nan(row["sources"])
     info_dict["EXT_ANNOS"] = check_if_nan(row["External oncogenic annotation_CGI"])
     info_dict["LINKED_DISEASES"] = get_disease_names_CIViC(row) if get_disease_names_CIViC(row) != "" else "None"
     info_dict["LINKED_THERAPIES_CIVIC"] = (
         get_therapy_names(row, civic_only=True) if get_therapy_names(row, civic_only=True) != "" else "None"
     )
-    info_dict["EVIDENCE_LIST"] = create_evidence_table(row) if create_evidence_table(row) != "" else "None"
-    info_dict["CIVIC_SUMMARY"] = check_if_nan(row["assertion_summary_CIVIC"])
-    info_dict["ASSERTION_DESCRIPTION"] = check_if_nan(row["assertion_description_CIVIC"])
-    info_dict["EVIDENCE_DESCRIPTION"] = check_if_nan(row["evidence_description_CIVIC"])
+    info_dict["EVIDENCE_LIST"] = (
+        create_evidence_table(row, ["5%", "5%", "5%", "5%", "5%", "5%", "65%", "5"])
+        if create_evidence_table(row, ["40%", "20%", "20%", "20%", "20%", "20%", "20%"]) != ""
+        else "None"
+    )
     info_dict["LINKED_DRUGS_RESPONSIVE"] = (
         get_therapy_information_CGI(row, biomarkers_df, "Responsive", ["40%", "20%", "20%", "20%", "20%", "20%"])
         if get_therapy_information_CGI(row, biomarkers_df, "Responsive", ["40%", "20%", "20%", "20%", "20%", "20%"])
         != ""
         else "None"
     )
     info_dict["LINKED_DRUGS_RESISTANT"] = (
         get_therapy_information_CGI(row, biomarkers_df, "Resistant", ["40%", "20%", "20%", "20%", "20%", "20%"])
         if get_therapy_information_CGI(row, biomarkers_df, "Resistant", ["40%", "20%", "20%", "20%", "20%", "20%"])
         != ""
         else "None"
     )
-    info_dict["EVIDENCE_DESCRIPTION"] = check_if_nan(row["evidence_description_CIVIC"])
-    info_dict["LITERATURE_CIVIC"] = check_if_nan(row["evidence_source_CIVIC"])
 
     return info_dict
 
 
 def write_individual_report(row, template_html, report_path, biomarkers_df, metadata_path):
     """
     This function creates a report for a specific variant.
```

### Comparing `querynator-0.4.0/querynator/report_scripts/sort_variants.py` & `querynator-0.4.1/querynator/report_scripts/sort_variants.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,41 +33,57 @@
     elif bool_nan == False:
         if get_largest_af(af) < 0.01 and get_largest_af(gnomad) < 0.01:
             return True
         else:
             return False
 
 
+def get_min(e):
+    """
+    returns minimum of an input
+
+    :param e: string or np.nan
+    :type e: str
+    :return: min of string or np.nan
+    :rtype: str
+    """
+    if pd.isnull(e):
+        return np.nan
+    else:
+        return min(e.split(","))
+
+
 def subset_variants_into_tiers(row):
     """
     decides tier (1-4) for specific variant
 
     :param row: row of a pandas DataFrame
     :type row: pandas Series
     :return: variant's tier
     :rtype: str
     """
     # check whether civic already provides AMP-based Tiers
+
     if not pd.isnull(row["assertion_amp_level_CIVIC"]):
         if "TIER_I_" in row["assertion_amp_level_CIVIC"]:
             return "tier_1"
         elif "TIER_II_" in row["assertion_amp_level_CIVIC"]:
             return "tier_2"
         elif "TIER_III_" in row["assertion_amp_level_CIVIC"]:
             return "tier_3"
         elif "TIER_IV_" in row["assertion_amp_level_CIVIC"]:
             return "tier_4"
     else:
-        if row["evidence_CGI"] in ["A", "B"] or row["evidence_level_CIVIC"] in ["A", "B"]:
+        if row["evidence_CGI"] in ["A", "B"] or get_min(row["evidence_level_CIVIC"]) in ["A", "B"]:
             return "tier_1"
-        elif row["evidence_CGI"] in ["C", "D"] or row["evidence_level_CIVIC"] in ["C", "D"]:
+        elif row["evidence_CGI"] in ["C", "D"] or get_min(row["evidence_level_CIVIC"]) in ["C", "D"]:
             return "tier_2"
         else:  # no evidence given (tier 3 or 4)
             # Tier 3 if oncogenic & MAF fits
-            if row["evidence_level_CIVIC"] == "E":
+            if get_min(row["evidence_level_CIVIC"]) == "E":
                 return "tier_3"
             elif (
                 row["Oncogenic Summary_CGI"] not in ["non-oncogenic", "non-protein affecting"]
                 and pd.isnull(row["Oncogenic Summary_CGI"]) == False
             ):
                 if get_allele_freq_tiering(row):
                     return "tier_3"
@@ -438,15 +454,15 @@
         not pd.isnull(row["evidence_therapies_CIVIC"])
         or not pd.isnull(row["assertion_therapies_name_CIVIC"])
         or not pd.isnull(row["evidence_CGI"])
     ):
         score += 2
 
     # Evidence associated CIViC
-    score += generate_evidence_score(row["evidence_level_CIVIC"])
+    score += generate_evidence_score(get_min(row["evidence_level_CIVIC"]))
 
     # Evidence associated CGI
     score += generate_evidence_score(row["evidence_CGI"])
 
     # consequence
     score += generate_consequence_score(row["Consequence_CGI"], row["variant_type_CIVIC"])
```

### Comparing `querynator-0.4.0/querynator/report_scripts/templates/template_individual.html` & `querynator-0.4.1/querynator/report_scripts/templates/template_individual.html`

 * *Files 9% similar despite different names*

```diff
@@ -104,43 +104,31 @@
 
     <strong> Seen In: </strong> CIVIC_CGI_PRESENT (External Annotations CGI:
     EXT_ANNOS)
     <br />
     <br />
 
     <h3><em>CIViC</em></h3>
-    <strong> Linked Diseases: </strong> LINKED_DISEASES
-    <br />
-    <br />
+    
     <strong> Linked Therapies: </strong> LINKED_THERAPIES_CIVIC
     <br />
     <br />
+    
     <details class="left">
       <summary><strong> Evidence: </strong></summary>
       Learn more about CIViC Evidence Items
       <a href="https://civic.readthedocs.io/en/latest/model/evidence.html"
         >here</a
       >
     </details>
     <br />
     EVIDENCE_LIST
     <br />
     <br />
-    <details class="left">
-      <summary><strong> Description: </strong> CIVIC_SUMMARY</summary>
-      <ul>
-        <li>ASSERTION_DESCRIPTION</li>
-        <br />
-        <li>EVIDENCE_DESCRIPTION</li>
-      </ul>
-    </details>
-    <br />
-    <br />
-    <strong> Literature: </strong> LITERATURE_CIVIC
-
+    
     <h3><em>CGI</em></h3>
 
     <details class="left">
       <summary><h4>Linked Therapies</h4></summary>
       Here we show those drugs that are linked to the Protein Change of this
       variant in the CGI Knowledgebase.
     </details>
```

#### html2text {}

```diff
@@ -24,28 +24,19 @@
 
 Protein Change: PROT_CHANGE
 ===============================================================================
 ***** Knowledgebase Annotations *****
 Seen In: CIVIC_CGI_PRESENT (External Annotations CGI: EXT_ANNOS)
 
 **** CIViC ****
-Linked Diseases: LINKED_DISEASES
-
 Linked Therapies: LINKED_THERAPIES_CIVIC
 
  Evidence: Learn more about CIViC Evidence Items here
 EVIDENCE_LIST
 
- Description: CIVIC_SUMMARY
-    * ASSERTION_DESCRIPTION
-    *
-    * EVIDENCE_DESCRIPTION
-
-
-Literature: LITERATURE_CIVIC
 **** CGI ****
 *** Linked Therapies ***
 Here we show those drugs that are linked to the Protein Change of this variant
 in the CGI Knowledgebase.
 Linked Therapies responsive: LINKED_DRUGS_RESPONSIVE
 
 Linked Therapies resistant: LINKED_DRUGS_RESISTANT
```

### Comparing `querynator-0.4.0/querynator/report_scripts/templates/template_overall_plotly_pieplots.html` & `querynator-0.4.1/querynator/report_scripts/templates/template_overall_plotly_pieplots.html`

 * *Files identical despite different names*

### Comparing `querynator-0.4.0/querynator/report_scripts/templates/template_overall_upsetplots.html` & `querynator-0.4.1/querynator/report_scripts/templates/template_overall_upsetplots.html`

 * *Files identical despite different names*

### Comparing `querynator-0.4.0/querynator.egg-info/PKG-INFO` & `querynator-0.4.1/querynator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: querynator
-Version: 0.4.0
+Version: 0.4.1
 Summary: Python package to query cancer variant databases
 Home-page: https://github.com/qbic-pipelines/querynator
 Author: Susanne Jodoin, Mark Polster
 Author-email: susanne.jodoin@qbic.uni-tuebingen.de, mark.polster@uni-tuebingen.de
 License: MIT license
 Keywords: querynator
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -76,14 +76,27 @@
 
 
 
 
 Changelog
 ============
 
+0.4.1 - Stormy Saturn  (2023-06-13)
+---------------------------------------------
+
+**Added**
+
+**Fixed**
+
+* Bug fixes to include all evidence of CIViC
+
+**Dependencies**
+
+**Deprecated**
+
 0.4.0 - Stormy Saturn  (2023-05-31)
 ---------------------------------------------
 
 **Added**
 
 **Fixed**
```

### Comparing `querynator-0.4.0/querynator.egg-info/SOURCES.txt` & `querynator-0.4.1/querynator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `querynator-0.4.0/setup.py` & `querynator-0.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,10 +42,10 @@
     keywords="querynator",
     name="querynator",
     packages=find_packages(exclude=("docs")),
     package_data={"": ["report_scripts/templates/*.html"]},
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/qbic-pipelines/querynator",
-    version="0.4.0",
+    version="0.4.1",
     zip_safe=False,
 )
```

### Comparing `querynator-0.4.0/tests/test_querynator.py` & `querynator-0.4.1/tests/test_querynator.py`

 * *Files identical despite different names*

