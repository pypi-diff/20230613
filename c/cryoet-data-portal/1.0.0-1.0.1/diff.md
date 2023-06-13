# Comparing `tmp/cryoet_data_portal-1.0.0.tar.gz` & `tmp/cryoet_data_portal-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cryoet_data_portal-1.0.0.tar", last modified: Thu Jun  8 06:41:40 2023, max compression
+gzip compressed data, was "cryoet_data_portal-1.0.1.tar", last modified: Tue Jun 13 16:08:19 2023, max compression
```

## Comparing `cryoet_data_portal-1.0.0.tar` & `cryoet_data_portal-1.0.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:41:40.410415 cryoet_data_portal-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-08 06:41:25.000000 cryoet_data_portal-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-08 06:41:40.410415 cryoet_data_portal-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-08 06:41:25.000000 cryoet_data_portal-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-06-08 06:41:25.000000 cryoet_data_portal-1.0.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:41:40.406415 cryoet_data_portal-1.0.0/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-08 06:41:25.000000 cryoet_data_portal-1.0.0/scripts/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 06:41:40.410415 cryoet_data_portal-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:41:40.406415 cryoet_data_portal-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:41:40.406415 cryoet_data_portal-1.0.0/src/cryoet_data_portal/
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-08 06:41:25.000000 cryoet_data_portal-1.0.0/src/cryoet_data_portal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-06-08 06:41:25.000000 cryoet_data_portal-1.0.0/src/cryoet_data_portal/_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-06-08 06:41:25.000000 cryoet_data_portal-1.0.0/src/cryoet_data_portal/_file_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     8072 2023-06-08 06:41:25.000000 cryoet_data_portal-1.0.0/src/cryoet_data_portal/_gql_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    28822 2023-06-08 06:41:25.000000 cryoet_data_portal-1.0.0/src/cryoet_data_portal/_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:41:40.410415 cryoet_data_portal-1.0.0/src/cryoet_data_portal/data/
--rw-r--r--   0 runner    (1001) docker     (123)   171477 2023-06-08 06:41:25.000000 cryoet_data_portal-1.0.0/src/cryoet_data_portal/data/schema.graphql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:41:40.410415 cryoet_data_portal-1.0.0/src/cryoet_data_portal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-08 06:41:40.000000 cryoet_data_portal-1.0.0/src/cryoet_data_portal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-08 06:41:40.000000 cryoet_data_portal-1.0.0/src/cryoet_data_portal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 06:41:40.000000 cryoet_data_portal-1.0.0/src/cryoet_data_portal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-08 06:41:40.000000 cryoet_data_portal-1.0.0/src/cryoet_data_portal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-08 06:41:40.000000 cryoet_data_portal-1.0.0/src/cryoet_data_portal.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:41:40.410415 cryoet_data_portal-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-08 06:41:25.000000 cryoet_data_portal-1.0.0/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-08 06:41:25.000000 cryoet_data_portal-1.0.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-08 06:41:25.000000 cryoet_data_portal-1.0.0/tests/test_get_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:08:19.144934 cryoet_data_portal-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-13 16:08:05.000000 cryoet_data_portal-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-13 16:08:19.140934 cryoet_data_portal-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-13 16:08:05.000000 cryoet_data_portal-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-06-13 16:08:05.000000 cryoet_data_portal-1.0.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:08:19.140934 cryoet_data_portal-1.0.1/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-13 16:08:05.000000 cryoet_data_portal-1.0.1/scripts/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 16:08:19.144934 cryoet_data_portal-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:08:19.140934 cryoet_data_portal-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:08:19.140934 cryoet_data_portal-1.0.1/src/cryoet_data_portal/
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-13 16:08:05.000000 cryoet_data_portal-1.0.1/src/cryoet_data_portal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-06-13 16:08:05.000000 cryoet_data_portal-1.0.1/src/cryoet_data_portal/_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-06-13 16:08:05.000000 cryoet_data_portal-1.0.1/src/cryoet_data_portal/_file_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8128 2023-06-13 16:08:05.000000 cryoet_data_portal-1.0.1/src/cryoet_data_portal/_gql_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28822 2023-06-13 16:08:05.000000 cryoet_data_portal-1.0.1/src/cryoet_data_portal/_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:08:19.140934 cryoet_data_portal-1.0.1/src/cryoet_data_portal/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   171477 2023-06-13 16:08:05.000000 cryoet_data_portal-1.0.1/src/cryoet_data_portal/data/schema.graphql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:08:19.140934 cryoet_data_portal-1.0.1/src/cryoet_data_portal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-13 16:08:19.000000 cryoet_data_portal-1.0.1/src/cryoet_data_portal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-13 16:08:19.000000 cryoet_data_portal-1.0.1/src/cryoet_data_portal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 16:08:19.000000 cryoet_data_portal-1.0.1/src/cryoet_data_portal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-13 16:08:19.000000 cryoet_data_portal-1.0.1/src/cryoet_data_portal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-13 16:08:19.000000 cryoet_data_portal-1.0.1/src/cryoet_data_portal.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:08:19.140934 cryoet_data_portal-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-13 16:08:05.000000 cryoet_data_portal-1.0.1/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-13 16:08:05.000000 cryoet_data_portal-1.0.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-13 16:08:05.000000 cryoet_data_portal-1.0.1/tests/test_get_client.py
```

### Comparing `cryoet_data_portal-1.0.0/LICENSE` & `cryoet_data_portal-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cryoet_data_portal-1.0.0/PKG-INFO` & `cryoet_data_portal-1.0.1/src/cryoet_data_portal.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cryoet_data_portal
-Version: 1.0.0
+Name: cryoet-data-portal
+Version: 1.0.1
 Summary: API Client to facilitate the use of the CryoET Portal. For more information about the API and the project visit https://github.com/chanzuckerberg/cryoet-data-portal/
 Author-email: Chan Zuckerberg Initiative <cryoetdataportal@chanzuckerberg.com>
 License: MIT
 Project-URL: homepage, https://github.com/chanzuckerberg/cryoet-data-portal
 Project-URL: repository, https://github.com/chanzuckerberg/cryoet-data-portal
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `cryoet_data_portal-1.0.0/README.md` & `cryoet_data_portal-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `cryoet_data_portal-1.0.0/pyproject.toml` & `cryoet_data_portal-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cryoet_data_portal-1.0.0/src/cryoet_data_portal/__init__.py` & `cryoet_data_portal-1.0.1/src/cryoet_data_portal/__init__.py`

 * *Files identical despite different names*

### Comparing `cryoet_data_portal-1.0.0/src/cryoet_data_portal/_client.py` & `cryoet_data_portal-1.0.1/src/cryoet_data_portal/_client.py`

 * *Files identical despite different names*

### Comparing `cryoet_data_portal-1.0.0/src/cryoet_data_portal/_file_tools.py` & `cryoet_data_portal-1.0.1/src/cryoet_data_portal/_file_tools.py`

 * *Files identical despite different names*

### Comparing `cryoet_data_portal-1.0.0/src/cryoet_data_portal/_gql_base.py` & `cryoet_data_portal-1.0.1/src/cryoet_data_portal/_gql_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -252,15 +252,17 @@
 
         Examples:
             Get a Run by ID:
 
             >>> run = Runs.get_by_id(client), 1
                 print(run.name)
         """
-        return client.find_one(cls, [cls.id == id])
+        results = cls.find(client, [cls.id == id])
+        for result in results:
+            return result
 
     @classmethod
     def setup(cls):
         for field in cls._get_scalar_fields():
             getattr(cls, field).configure(cls, field)
         for field in cls._get_relationship_fields():
             getattr(cls, field).configure(cls, field)
```

### Comparing `cryoet_data_portal-1.0.0/src/cryoet_data_portal/_models.py` & `cryoet_data_portal-1.0.1/src/cryoet_data_portal/_models.py`

 * *Files identical despite different names*

### Comparing `cryoet_data_portal-1.0.0/src/cryoet_data_portal/data/schema.graphql` & `cryoet_data_portal-1.0.1/src/cryoet_data_portal/data/schema.graphql`

 * *Files identical despite different names*

### Comparing `cryoet_data_portal-1.0.0/src/cryoet_data_portal.egg-info/PKG-INFO` & `cryoet_data_portal-1.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cryoet-data-portal
-Version: 1.0.0
+Name: cryoet_data_portal
+Version: 1.0.1
 Summary: API Client to facilitate the use of the CryoET Portal. For more information about the API and the project visit https://github.com/chanzuckerberg/cryoet-data-portal/
 Author-email: Chan Zuckerberg Initiative <cryoetdataportal@chanzuckerberg.com>
 License: MIT
 Project-URL: homepage, https://github.com/chanzuckerberg/cryoet-data-portal
 Project-URL: repository, https://github.com/chanzuckerberg/cryoet-data-portal
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `cryoet_data_portal-1.0.0/src/cryoet_data_portal.egg-info/SOURCES.txt` & `cryoet_data_portal-1.0.1/src/cryoet_data_portal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cryoet_data_portal-1.0.0/tests/README.md` & `cryoet_data_portal-1.0.1/tests/README.md`

 * *Files identical despite different names*

