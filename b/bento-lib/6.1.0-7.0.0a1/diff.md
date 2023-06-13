# Comparing `tmp/bento_lib-6.1.0.tar.gz` & `tmp/bento_lib-7.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bento_lib-6.1.0.tar", last modified: Fri Jun  2 20:15:06 2023, max compression
+gzip compressed data, was "bento_lib-7.0.0a1.tar", last modified: Tue Jun 13 12:15:22 2023, max compression
```

## Comparing `bento_lib-6.1.0.tar` & `bento_lib-7.0.0a1.tar`

### file list

```diff
@@ -1,54 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 20:15:06.748854 bento_lib-6.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-06-02 20:14:55.000000 bento_lib-6.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-02 20:14:55.000000 bento_lib-6.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-06-02 20:15:06.748854 bento_lib-6.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-06-02 20:14:55.000000 bento_lib-6.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 20:15:06.744854 bento_lib-6.1.0/bento_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-02 20:14:55.000000 bento_lib-6.1.0/bento_lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 20:15:06.744854 bento_lib-6.1.0/bento_lib/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 20:14:55.000000 bento_lib-6.1.0/bento_lib/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-02 20:14:55.000000 bento_lib-6.1.0/bento_lib/auth/django_remote_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-02 20:14:55.000000 bento_lib-6.1.0/bento_lib/auth/flask_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-02 20:14:55.000000 bento_lib-6.1.0/bento_lib/auth/headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-06-02 20:14:55.000000 bento_lib-6.1.0/bento_lib/auth/quart_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-02 20:14:55.000000 bento_lib-6.1.0/bento_lib/auth/roles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 20:15:06.744854 bento_lib-6.1.0/bento_lib/drs/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-02 20:14:55.000000 bento_lib-6.1.0/bento_lib/drs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-06-02 20:14:55.000000 bento_lib-6.1.0/bento_lib/drs/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 20:15:06.744854 bento_lib-6.1.0/bento_lib/events/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-02 20:14:55.000000 bento_lib-6.1.0/bento_lib/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8687 2023-06-02 20:14:55.000000 bento_lib-6.1.0/bento_lib/events/_event_bus.py
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-02 20:14:55.000000 bento_lib-6.1.0/bento_lib/events/notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-02 20:14:55.000000 bento_lib-6.1.0/bento_lib/events/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-02 20:14:55.000000 bento_lib-6.1.0/bento_lib/package.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 20:15:06.744854 bento_lib-6.1.0/bento_lib/responses/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-02 20:14:55.000000 bento_lib-6.1.0/bento_lib/responses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-06-02 20:14:55.000000 bento_lib-6.1.0/bento_lib/responses/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-02 20:14:55.000000 bento_lib-6.1.0/bento_lib/responses/fastapi_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-06-02 20:14:55.000000 bento_lib-6.1.0/bento_lib/responses/flask_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-06-02 20:14:55.000000 bento_lib-6.1.0/bento_lib/responses/quart_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 20:15:06.748854 bento_lib-6.1.0/bento_lib/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-02 20:14:55.000000 bento_lib-6.1.0/bento_lib/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-02 20:14:55.000000 bento_lib-6.1.0/bento_lib/schemas/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-02 20:14:55.000000 bento_lib-6.1.0/bento_lib/schemas/bento.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-06-02 20:14:55.000000 bento_lib-6.1.0/bento_lib/schemas/bento_data_use.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-02 20:14:55.000000 bento_lib-6.1.0/bento_lib/schemas/bento_ingest.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-02 20:14:55.000000 bento_lib-6.1.0/bento_lib/schemas/ga4gh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-02 20:14:55.000000 bento_lib-6.1.0/bento_lib/schemas/ga4gh_service_info.schema.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 20:15:06.748854 bento_lib-6.1.0/bento_lib/search/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-02 20:14:55.000000 bento_lib-6.1.0/bento_lib/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-02 20:14:55.000000 bento_lib-6.1.0/bento_lib/search/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    26842 2023-06-02 20:14:55.000000 bento_lib-6.1.0/bento_lib/search/data_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-02 20:14:55.000000 bento_lib-6.1.0/bento_lib/search/operations.py
--rw-r--r--   0 runner    (1001) docker     (123)    22589 2023-06-02 20:14:55.000000 bento_lib-6.1.0/bento_lib/search/postgres.py
--rw-r--r--   0 runner    (1001) docker     (123)     9376 2023-06-02 20:14:55.000000 bento_lib-6.1.0/bento_lib/search/queries.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-06-02 20:14:55.000000 bento_lib-6.1.0/bento_lib/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-06-02 20:14:55.000000 bento_lib-6.1.0/bento_lib/workflows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 20:15:06.744854 bento_lib-6.1.0/bento_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-06-02 20:15:06.000000 bento_lib-6.1.0/bento_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-06-02 20:15:06.000000 bento_lib-6.1.0/bento_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 20:15:06.000000 bento_lib-6.1.0/bento_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-02 20:15:06.000000 bento_lib-6.1.0/bento_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-02 20:15:06.000000 bento_lib-6.1.0/bento_lib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 20:15:06.748854 bento_lib-6.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-06-02 20:14:55.000000 bento_lib-6.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:15:22.841275 bento_lib-7.0.0a1/
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-06-13 12:15:13.000000 bento_lib-7.0.0a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-13 12:15:13.000000 bento_lib-7.0.0a1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-06-13 12:15:22.837275 bento_lib-7.0.0a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-06-13 12:15:13.000000 bento_lib-7.0.0a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:15:22.833275 bento_lib-7.0.0a1/bento_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-13 12:15:13.000000 bento_lib-7.0.0a1/bento_lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:15:22.833275 bento_lib-7.0.0a1/bento_lib/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 12:15:13.000000 bento_lib-7.0.0a1/bento_lib/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-13 12:15:13.000000 bento_lib-7.0.0a1/bento_lib/auth/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:15:22.833275 bento_lib-7.0.0a1/bento_lib/auth/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 12:15:13.000000 bento_lib-7.0.0a1/bento_lib/auth/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4930 2023-06-13 12:15:13.000000 bento_lib-7.0.0a1/bento_lib/auth/middleware/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-13 12:15:13.000000 bento_lib-7.0.0a1/bento_lib/auth/middleware/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-06-13 12:15:13.000000 bento_lib-7.0.0a1/bento_lib/auth/middleware/django.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-06-13 12:15:13.000000 bento_lib-7.0.0a1/bento_lib/auth/middleware/fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-06-13 12:15:13.000000 bento_lib-7.0.0a1/bento_lib/auth/middleware/flask.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:15:22.837275 bento_lib-7.0.0a1/bento_lib/drs/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-13 12:15:13.000000 bento_lib-7.0.0a1/bento_lib/drs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-06-13 12:15:13.000000 bento_lib-7.0.0a1/bento_lib/drs/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:15:22.837275 bento_lib-7.0.0a1/bento_lib/events/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-13 12:15:13.000000 bento_lib-7.0.0a1/bento_lib/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8687 2023-06-13 12:15:13.000000 bento_lib-7.0.0a1/bento_lib/events/_event_bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-13 12:15:13.000000 bento_lib-7.0.0a1/bento_lib/events/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-13 12:15:13.000000 bento_lib-7.0.0a1/bento_lib/events/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-13 12:15:13.000000 bento_lib-7.0.0a1/bento_lib/package.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:15:22.837275 bento_lib-7.0.0a1/bento_lib/responses/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-13 12:15:13.000000 bento_lib-7.0.0a1/bento_lib/responses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-06-13 12:15:13.000000 bento_lib-7.0.0a1/bento_lib/responses/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-06-13 12:15:13.000000 bento_lib-7.0.0a1/bento_lib/responses/fastapi_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-06-13 12:15:13.000000 bento_lib-7.0.0a1/bento_lib/responses/flask_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:15:22.837275 bento_lib-7.0.0a1/bento_lib/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-13 12:15:13.000000 bento_lib-7.0.0a1/bento_lib/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-13 12:15:13.000000 bento_lib-7.0.0a1/bento_lib/schemas/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-13 12:15:13.000000 bento_lib-7.0.0a1/bento_lib/schemas/bento.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-06-13 12:15:13.000000 bento_lib-7.0.0a1/bento_lib/schemas/bento_data_use.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-13 12:15:13.000000 bento_lib-7.0.0a1/bento_lib/schemas/bento_ingest.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-13 12:15:13.000000 bento_lib-7.0.0a1/bento_lib/schemas/ga4gh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-13 12:15:13.000000 bento_lib-7.0.0a1/bento_lib/schemas/ga4gh_service_info.schema.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:15:22.837275 bento_lib-7.0.0a1/bento_lib/search/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-13 12:15:13.000000 bento_lib-7.0.0a1/bento_lib/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-13 12:15:13.000000 bento_lib-7.0.0a1/bento_lib/search/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26842 2023-06-13 12:15:13.000000 bento_lib-7.0.0a1/bento_lib/search/data_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-13 12:15:13.000000 bento_lib-7.0.0a1/bento_lib/search/operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22589 2023-06-13 12:15:13.000000 bento_lib-7.0.0a1/bento_lib/search/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9376 2023-06-13 12:15:13.000000 bento_lib-7.0.0a1/bento_lib/search/queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-06-13 12:15:13.000000 bento_lib-7.0.0a1/bento_lib/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-06-13 12:15:13.000000 bento_lib-7.0.0a1/bento_lib/workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:15:22.833275 bento_lib-7.0.0a1/bento_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-06-13 12:15:22.000000 bento_lib-7.0.0a1/bento_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-06-13 12:15:22.000000 bento_lib-7.0.0a1/bento_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 12:15:22.000000 bento_lib-7.0.0a1/bento_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-13 12:15:22.000000 bento_lib-7.0.0a1/bento_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-13 12:15:22.000000 bento_lib-7.0.0a1/bento_lib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 12:15:22.841275 bento_lib-7.0.0a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-06-13 12:15:13.000000 bento_lib-7.0.0a1/setup.py
```

### Comparing `bento_lib-6.1.0/LICENSE` & `bento_lib-7.0.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `bento_lib-6.1.0/PKG-INFO` & `bento_lib-7.0.0a1/bento_lib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
-Name: bento_lib
-Version: 6.1.0
+Name: bento-lib
+Version: 7.0.0a1
 Summary: A set of common utilities and helpers for Bento platform services.
 Home-page: https://github.com/bento-platform/bento_lib
 Author: David Lougheed, Paul Pillot
 Author-email: david.lougheed@mail.mcgill.ca, paul.pillot@computationalgenomics.ca
 License: LGPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8.1
+Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 Provides-Extra: flask
 Provides-Extra: django
 Provides-Extra: fastapi
-Provides-Extra: quart
 License-File: LICENSE
 
 # Bento Library (for Python Bento microservices)
 
 ![Test Status](https://github.com/bento-platform/bento_lib/workflows/Test/badge.svg)
 ![Lint Status](https://github.com/bento-platform/bento_lib/workflows/Lint/badge.svg)
 [![codecov](https://codecov.io/gh/bento-platform/bento_lib/branch/master/graph/badge.svg)](https://codecov.io/gh/bento-platform/bento_lib)
```

### Comparing `bento_lib-6.1.0/README.md` & `bento_lib-7.0.0a1/README.md`

 * *Files identical despite different names*

### Comparing `bento_lib-6.1.0/bento_lib/drs/utils.py` & `bento_lib-7.0.0a1/bento_lib/drs/utils.py`

 * *Files identical despite different names*

### Comparing `bento_lib-6.1.0/bento_lib/events/_event_bus.py` & `bento_lib-7.0.0a1/bento_lib/events/_event_bus.py`

 * *Files identical despite different names*

### Comparing `bento_lib-6.1.0/bento_lib/events/notifications.py` & `bento_lib-7.0.0a1/bento_lib/events/notifications.py`

 * *Files identical despite different names*

### Comparing `bento_lib-6.1.0/bento_lib/events/types.py` & `bento_lib-7.0.0a1/bento_lib/events/types.py`

 * *Files identical despite different names*

### Comparing `bento_lib-6.1.0/bento_lib/responses/errors.py` & `bento_lib-7.0.0a1/bento_lib/responses/errors.py`

 * *Files identical despite different names*

### Comparing `bento_lib-6.1.0/bento_lib/responses/fastapi_errors.py` & `bento_lib-7.0.0a1/bento_lib/responses/fastapi_errors.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,34 +4,47 @@
 from fastapi import status
 from fastapi.exceptions import HTTPException, RequestValidationError
 from fastapi.requests import Request
 from fastapi.responses import JSONResponse
 from starlette.responses import Response
 from typing import Callable
 
+from ..auth.exceptions import BentoAuthException
 from .errors import http_error
 
 __all__ = [
     "http_exception_handler_factory",
+    "bento_auth_exception_handler_factory",
     "validation_exception_handler",
 ]
 
 
+def _log_if_500(logger: logging.Logger, code: int, exc: Exception) -> None:
+    if code == status.HTTP_500_INTERNAL_SERVER_ERROR:
+        logger.error(f"Encountered error:\n{traceback.format_exception(type(exc), exc, exc.__traceback__)}")
+
+
 def http_exception_handler_factory(logger: logging.Logger) -> Callable[[Request, HTTPException], Response]:
     def http_exception_handler(_request: Request, exc: HTTPException) -> JSONResponse:
         code = exc.status_code
-
-        if code == status.HTTP_500_INTERNAL_SERVER_ERROR:
-            logger.error(f"Encountered error:\n{traceback.format_exception(type(exc), exc, exc.__traceback__)}")
-
+        _log_if_500(logger, code, exc)
         return JSONResponse(http_error(code, exc.detail), status_code=code)
 
     return http_exception_handler
 
 
+def bento_auth_exception_handler_factory(logger: logging.Logger) -> Callable[[Request, BentoAuthException], Response]:
+    def bento_auth_exception_handler(_request: Request, exc: BentoAuthException) -> JSONResponse:
+        code = exc.status_code
+        _log_if_500(logger, code, exc)
+        return JSONResponse(http_error(code, exc.message), status_code=code)
+
+    return bento_auth_exception_handler
+
+
 def validation_exception_handler(_request: Request, exc: RequestValidationError) -> JSONResponse:
     code = status.HTTP_400_BAD_REQUEST
     return JSONResponse(
         http_error(
             code,
             *((".".join(map(str, e["loc"])) + ": " + e["msg"]) if e.get("loc") else e["msg"] for e in exc.errors())),
         status_code=code)
```

### Comparing `bento_lib-6.1.0/bento_lib/responses/flask_errors.py` & `bento_lib-7.0.0a1/bento_lib/responses/flask_errors.py`

 * *Files identical despite different names*

### Comparing `bento_lib-6.1.0/bento_lib/schemas/bento_data_use.schema.json` & `bento_lib-7.0.0a1/bento_lib/schemas/bento_data_use.schema.json`

 * *Files identical despite different names*

### Comparing `bento_lib-6.1.0/bento_lib/schemas/bento_ingest.schema.json` & `bento_lib-7.0.0a1/bento_lib/schemas/bento_ingest.schema.json`

 * *Files identical despite different names*

### Comparing `bento_lib-6.1.0/bento_lib/schemas/ga4gh_service_info.schema.json` & `bento_lib-7.0.0a1/bento_lib/schemas/ga4gh_service_info.schema.json`

 * *Files identical despite different names*

### Comparing `bento_lib-6.1.0/bento_lib/search/data_structure.py` & `bento_lib-7.0.0a1/bento_lib/search/data_structure.py`

 * *Files identical despite different names*

### Comparing `bento_lib-6.1.0/bento_lib/search/operations.py` & `bento_lib-7.0.0a1/bento_lib/search/operations.py`

 * *Files identical despite different names*

### Comparing `bento_lib-6.1.0/bento_lib/search/postgres.py` & `bento_lib-7.0.0a1/bento_lib/search/postgres.py`

 * *Files identical despite different names*

### Comparing `bento_lib-6.1.0/bento_lib/search/queries.py` & `bento_lib-7.0.0a1/bento_lib/search/queries.py`

 * *Files identical despite different names*

### Comparing `bento_lib-6.1.0/bento_lib/types.py` & `bento_lib-7.0.0a1/bento_lib/types.py`

 * *Files identical despite different names*

### Comparing `bento_lib-6.1.0/bento_lib/workflows.py` & `bento_lib-7.0.0a1/bento_lib/workflows.py`

 * *Files identical despite different names*

### Comparing `bento_lib-6.1.0/bento_lib.egg-info/PKG-INFO` & `bento_lib-7.0.0a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
-Name: bento-lib
-Version: 6.1.0
+Name: bento_lib
+Version: 7.0.0a1
 Summary: A set of common utilities and helpers for Bento platform services.
 Home-page: https://github.com/bento-platform/bento_lib
 Author: David Lougheed, Paul Pillot
 Author-email: david.lougheed@mail.mcgill.ca, paul.pillot@computationalgenomics.ca
 License: LGPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8.1
+Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 Provides-Extra: flask
 Provides-Extra: django
 Provides-Extra: fastapi
-Provides-Extra: quart
 License-File: LICENSE
 
 # Bento Library (for Python Bento microservices)
 
 ![Test Status](https://github.com/bento-platform/bento_lib/workflows/Test/badge.svg)
 ![Lint Status](https://github.com/bento-platform/bento_lib/workflows/Lint/badge.svg)
 [![codecov](https://codecov.io/gh/bento-platform/bento_lib/branch/master/graph/badge.svg)](https://codecov.io/gh/bento-platform/bento_lib)
```

### Comparing `bento_lib-6.1.0/bento_lib.egg-info/SOURCES.txt` & `bento_lib-7.0.0a1/bento_lib.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -8,30 +8,31 @@
 bento_lib/workflows.py
 bento_lib.egg-info/PKG-INFO
 bento_lib.egg-info/SOURCES.txt
 bento_lib.egg-info/dependency_links.txt
 bento_lib.egg-info/requires.txt
 bento_lib.egg-info/top_level.txt
 bento_lib/auth/__init__.py
-bento_lib/auth/django_remote_user.py
-bento_lib/auth/flask_decorators.py
-bento_lib/auth/headers.py
-bento_lib/auth/quart_decorators.py
-bento_lib/auth/roles.py
+bento_lib/auth/exceptions.py
+bento_lib/auth/middleware/__init__.py
+bento_lib/auth/middleware/base.py
+bento_lib/auth/middleware/constants.py
+bento_lib/auth/middleware/django.py
+bento_lib/auth/middleware/fastapi.py
+bento_lib/auth/middleware/flask.py
 bento_lib/drs/__init__.py
 bento_lib/drs/utils.py
 bento_lib/events/__init__.py
 bento_lib/events/_event_bus.py
 bento_lib/events/notifications.py
 bento_lib/events/types.py
 bento_lib/responses/__init__.py
 bento_lib/responses/errors.py
 bento_lib/responses/fastapi_errors.py
 bento_lib/responses/flask_errors.py
-bento_lib/responses/quart_errors.py
 bento_lib/schemas/__init__.py
 bento_lib/schemas/_utils.py
 bento_lib/schemas/bento.py
 bento_lib/schemas/bento_data_use.schema.json
 bento_lib/schemas/bento_ingest.schema.json
 bento_lib/schemas/ga4gh.py
 bento_lib/schemas/ga4gh_service_info.schema.json
```

### Comparing `bento_lib-6.1.0/setup.py` & `bento_lib-7.0.0a1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,28 +10,27 @@
 config = configparser.ConfigParser()
 config.read(os.path.join(os.path.dirname(os.path.realpath(__file__)), "bento_lib", "package.cfg"))
 
 setuptools.setup(
     name=config["package"]["name"],
     version=config["package"]["version"],
 
-    python_requires=">=3.8.1",
+    python_requires=">=3.10.0",
     install_requires=[
         "aiohttp>=3.8.4,<4",
         "jsonschema>=4.17.3,<5",
         "psycopg2-binary>=2.9.5,<3.0",
-        "redis>=4.5.1,<5.0",
+        "redis>=4.5.4,<5.0",
         "requests>=2.28.1,<3",
         "Werkzeug>=2.2.3,<3",
     ],
     extras_require={
         "flask": ["Flask>=2.2.5,<3"],
         "django": ["Django>=4.1.9,<5", "djangorestframework>=3.14.0,<3.15"],
         "fastapi": ["fastapi>=0.95.2,<0.96"],
-        "quart": ["quart>=0.18.4,<0.19"],
     },
 
     author=config["package"]["authors"],
     author_email=config["package"]["author_emails"],
 
     description="A set of common utilities and helpers for Bento platform services.",
     long_description=long_description,
```

