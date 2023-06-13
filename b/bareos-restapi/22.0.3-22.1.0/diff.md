# Comparing `tmp/bareos-restapi-22.0.3.tar.gz` & `tmp/bareos-restapi-22.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bareos-restapi-22.0.3.tar", last modified: Fri Mar 24 13:07:28 2023, max compression
+gzip compressed data, was "dist/bareos-restapi-22.1.0.tar", last modified: Tue Jun 13 10:17:09 2023, max compression
```

## Comparing `bareos-restapi-22.0.3.tar` & `bareos-restapi-22.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-24 13:07:28.000000 bareos-restapi-22.0.3/
--rw-r--r--   0 runner    (1001) docker     (122)     3658 2023-03-24 13:07:28.000000 bareos-restapi-22.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2497 2023-03-24 13:07:23.000000 bareos-restapi-22.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-24 13:07:28.000000 bareos-restapi-22.0.3/bareos_restapi/
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-03-24 13:07:26.000000 bareos-restapi-22.0.3/bareos_restapi/VERSION.txt
--rw-r--r--   0 runner    (1001) docker     (122)    61638 2023-03-24 13:07:23.000000 bareos-restapi-22.0.3/bareos_restapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      369 2023-03-24 13:07:23.000000 bareos-restapi-22.0.3/bareos_restapi/api.ini.example
--rw-r--r--   0 runner    (1001) docker     (122)     2827 2023-03-24 13:07:23.000000 bareos-restapi-22.0.3/bareos_restapi/metatags.yaml
--rw-r--r--   0 runner    (1001) docker     (122)    25039 2023-03-24 13:07:23.000000 bareos-restapi-22.0.3/bareos_restapi/models.py
--rw-r--r--   0 runner    (1001) docker     (122)   149657 2023-03-24 13:07:23.000000 bareos-restapi-22.0.3/bareos_restapi/openapi.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-24 13:07:28.000000 bareos-restapi-22.0.3/bareos_restapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3658 2023-03-24 13:07:27.000000 bareos-restapi-22.0.3/bareos_restapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      374 2023-03-24 13:07:28.000000 bareos-restapi-22.0.3/bareos_restapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-24 13:07:27.000000 bareos-restapi-22.0.3/bareos_restapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       93 2023-03-24 13:07:27.000000 bareos-restapi-22.0.3/bareos_restapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-03-24 13:07:27.000000 bareos-restapi-22.0.3/bareos_restapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-03-24 13:07:28.000000 bareos-restapi-22.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2857 2023-03-24 13:07:23.000000 bareos-restapi-22.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 10:17:09.000000 bareos-restapi-22.1.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     3658 2023-06-13 10:17:09.000000 bareos-restapi-22.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2497 2023-06-13 10:17:03.000000 bareos-restapi-22.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 10:17:09.000000 bareos-restapi-22.1.0/bareos_restapi/
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-06-13 10:17:08.000000 bareos-restapi-22.1.0/bareos_restapi/VERSION.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    61638 2023-06-13 10:17:03.000000 bareos-restapi-22.1.0/bareos_restapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      369 2023-06-13 10:17:03.000000 bareos-restapi-22.1.0/bareos_restapi/api.ini.example
+-rw-r--r--   0 runner    (1001) docker     (122)     2827 2023-06-13 10:17:03.000000 bareos-restapi-22.1.0/bareos_restapi/metatags.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)    25039 2023-06-13 10:17:03.000000 bareos-restapi-22.1.0/bareos_restapi/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)   149657 2023-06-13 10:17:03.000000 bareos-restapi-22.1.0/bareos_restapi/openapi.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 10:17:09.000000 bareos-restapi-22.1.0/bareos_restapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3658 2023-06-13 10:17:09.000000 bareos-restapi-22.1.0/bareos_restapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      374 2023-06-13 10:17:09.000000 bareos-restapi-22.1.0/bareos_restapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-13 10:17:09.000000 bareos-restapi-22.1.0/bareos_restapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       93 2023-06-13 10:17:09.000000 bareos-restapi-22.1.0/bareos_restapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-06-13 10:17:09.000000 bareos-restapi-22.1.0/bareos_restapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-13 10:17:09.000000 bareos-restapi-22.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2857 2023-06-13 10:17:03.000000 bareos-restapi-22.1.0/setup.py
```

### Comparing `bareos-restapi-22.0.3/PKG-INFO` & `bareos-restapi-22.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bareos-restapi
-Version: 22.0.3
+Version: 22.1.0
 Summary: REST API for Bareos console access.
 Home-page: https://github.com/bareos/bareos/
 Author: Bareos Team
 Author-email: packager@bareos.com
 License: AGPLv3
 Description: # Bareos REST API using fastAPI and python-bareos
```

### Comparing `bareos-restapi-22.0.3/README.md` & `bareos-restapi-22.1.0/README.md`

 * *Files identical despite different names*

### Comparing `bareos-restapi-22.0.3/bareos_restapi/__init__.py` & `bareos-restapi-22.1.0/bareos_restapi/__init__.py`

 * *Files identical despite different names*

### Comparing `bareos-restapi-22.0.3/bareos_restapi/metatags.yaml` & `bareos-restapi-22.1.0/bareos_restapi/metatags.yaml`

 * *Files identical despite different names*

### Comparing `bareos-restapi-22.0.3/bareos_restapi/models.py` & `bareos-restapi-22.1.0/bareos_restapi/models.py`

 * *Files identical despite different names*

### Comparing `bareos-restapi-22.0.3/bareos_restapi/openapi.json` & `bareos-restapi-22.1.0/bareos_restapi/openapi.json`

 * *Files identical despite different names*

### Comparing `bareos-restapi-22.0.3/bareos_restapi.egg-info/PKG-INFO` & `bareos-restapi-22.1.0/bareos_restapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bareos-restapi
-Version: 22.0.3
+Version: 22.1.0
 Summary: REST API for Bareos console access.
 Home-page: https://github.com/bareos/bareos/
 Author: Bareos Team
 Author-email: packager@bareos.com
 License: AGPLv3
 Description: # Bareos REST API using fastAPI and python-bareos
```

### Comparing `bareos-restapi-22.0.3/setup.py` & `bareos-restapi-22.1.0/setup.py`

 * *Files identical despite different names*

