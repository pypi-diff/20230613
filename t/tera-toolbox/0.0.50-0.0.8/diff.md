# Comparing `tmp/tera-toolbox-0.0.50.tar.gz` & `tmp/tera-toolbox-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tera-toolbox-0.0.50.tar", last modified: Tue Jun 13 17:35:56 2023, max compression
+gzip compressed data, was "tera-toolbox-0.0.8.tar", last modified: Fri May 19 17:16:46 2023, max compression
```

## Comparing `tera-toolbox-0.0.50.tar` & `tera-toolbox-0.0.8.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 17:35:56.361802 tera-toolbox-0.0.50/
--rw-r--r--   0 runner    (1001) docker     (122)      527 2023-06-13 17:35:56.361802 tera-toolbox-0.0.50/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-13 17:35:48.000000 tera-toolbox-0.0.50/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-13 17:35:56.361802 tera-toolbox-0.0.50/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1429 2023-06-13 17:35:48.000000 tera-toolbox-0.0.50/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 17:35:56.361802 tera-toolbox-0.0.50/tera_toolbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      527 2023-06-13 17:35:56.000000 tera-toolbox-0.0.50/tera_toolbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      325 2023-06-13 17:35:56.000000 tera-toolbox-0.0.50/tera_toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-13 17:35:56.000000 tera-toolbox-0.0.50/tera_toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       40 2023-06-13 17:35:56.000000 tera-toolbox-0.0.50/tera_toolbox.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       42 2023-06-13 17:35:56.000000 tera-toolbox-0.0.50/tera_toolbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        8 2023-06-13 17:35:56.000000 tera-toolbox-0.0.50/tera_toolbox.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 17:35:56.361802 tera-toolbox-0.0.50/toolbox/
--rw-r--r--   0 runner    (1001) docker     (122)      179 2023-06-13 17:35:48.000000 tera-toolbox-0.0.50/toolbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      762 2023-06-13 17:35:48.000000 tera-toolbox-0.0.50/toolbox/data.py
--rw-r--r--   0 runner    (1001) docker     (122)    30355 2023-06-13 17:35:48.000000 tera-toolbox-0.0.50/toolbox/stats.py
--rw-r--r--   0 runner    (1001) docker     (122)    23162 2023-06-13 17:35:48.000000 tera-toolbox-0.0.50/toolbox/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)       20 2023-06-13 17:35:48.000000 tera-toolbox-0.0.50/toolbox/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 17:16:46.782336 tera-toolbox-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (122)      526 2023-05-19 17:16:46.782336 tera-toolbox-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-05-19 17:16:39.000000 tera-toolbox-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-19 17:16:46.782336 tera-toolbox-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1433 2023-05-19 17:16:39.000000 tera-toolbox-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 17:16:46.782336 tera-toolbox-0.0.8/tera_toolbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      526 2023-05-19 17:16:46.000000 tera-toolbox-0.0.8/tera_toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      290 2023-05-19 17:16:46.000000 tera-toolbox-0.0.8/tera_toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-19 17:16:46.000000 tera-toolbox-0.0.8/tera_toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       40 2023-05-19 17:16:46.000000 tera-toolbox-0.0.8/tera_toolbox.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        8 2023-05-19 17:16:46.000000 tera-toolbox-0.0.8/tera_toolbox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 17:16:46.782336 tera-toolbox-0.0.8/toolbox/
+-rw-r--r--   0 runner    (1001) docker     (122)      178 2023-05-19 17:16:39.000000 tera-toolbox-0.0.8/toolbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      506 2023-05-19 17:16:39.000000 tera-toolbox-0.0.8/toolbox/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-05-19 17:16:39.000000 tera-toolbox-0.0.8/toolbox/stats.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3848 2023-05-19 17:16:39.000000 tera-toolbox-0.0.8/toolbox/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-05-19 17:16:39.000000 tera-toolbox-0.0.8/toolbox/version.py
```

### Comparing `tera-toolbox-0.0.50/PKG-INFO` & `tera-toolbox-0.0.8/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: tera-toolbox
-Version: 0.0.50
+Version: 0.0.8
 Summary: financial analysis toolbox
 Home-page: https://github.com/tera-capital/tera-toolbox
 Author: Tera Capital
 Author-email: jose.governo@teracapital.com.br
 License: Apache Software License
 Description: # Financial Tools
```

### Comparing `tera-toolbox-0.0.50/setup.py` & `tera-toolbox-0.0.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,11 +36,11 @@
     keywords="""quant finance analysis portfolio""",
     entry_points={
         "console_scripts": [
             "sample=sample:main",
         ],
     },
     packages=find_packages(exclude=["contrib", "docs", "tests", "examples"]),
-    install_requires=requirements,
+    install_requirements=requirements,
     python_requires=">=3.6",
     include_package_data=True,
 )
```

### Comparing `tera-toolbox-0.0.50/tera_toolbox.egg-info/PKG-INFO` & `tera-toolbox-0.0.8/tera_toolbox.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: tera-toolbox
-Version: 0.0.50
+Version: 0.0.8
 Summary: financial analysis toolbox
 Home-page: https://github.com/tera-capital/tera-toolbox
 Author: Tera Capital
 Author-email: jose.governo@teracapital.com.br
 License: Apache Software License
 Description: # Financial Tools
```

