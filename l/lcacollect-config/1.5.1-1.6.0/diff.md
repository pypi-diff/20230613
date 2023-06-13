# Comparing `tmp/lcacollect_config-1.5.1.tar.gz` & `tmp/lcacollect_config-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lcacollect_config-1.5.1.tar", max compression
+gzip compressed data, was "lcacollect_config-1.6.0.tar", max compression
```

## Comparing `lcacollect_config-1.5.1.tar` & `lcacollect_config-1.6.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0     1030 2023-05-23 09:33:34.682656 lcacollect_config-1.5.1/README.md
--rw-r--r--   0        0        0     2527 2023-05-23 09:33:34.682656 lcacollect_config-1.5.1/pyproject.toml
--rw-r--r--   0        0        0       22 2023-05-23 09:33:34.682656 lcacollect_config-1.5.1/src/lcacollect_config/__init__.py
--rw-r--r--   0        0        0     2831 2023-05-23 09:33:34.682656 lcacollect_config-1.5.1/src/lcacollect_config/config.py
--rw-r--r--   0        0        0     1507 2023-05-23 09:33:34.686656 lcacollect_config-1.5.1/src/lcacollect_config/connection.py
--rw-r--r--   0        0        0      372 2023-05-23 09:33:34.686656 lcacollect_config-1.5.1/src/lcacollect_config/context.py
--rw-r--r--   0        0        0     2835 2023-05-23 09:33:34.686656 lcacollect_config-1.5.1/src/lcacollect_config/email.py
--rw-r--r--   0        0        0      263 2023-05-23 09:33:34.686656 lcacollect_config-1.5.1/src/lcacollect_config/exceptions.py
--rw-r--r--   0        0        0      637 2023-05-23 09:33:34.686656 lcacollect_config-1.5.1/src/lcacollect_config/fastapi.py
--rw-r--r--   0        0        0      597 2023-05-23 09:33:34.686656 lcacollect_config-1.5.1/src/lcacollect_config/formatting.py
--rw-r--r--   0        0        0        0 2023-05-23 09:33:34.686656 lcacollect_config-1.5.1/src/lcacollect_config/graphql/__init__.py
--rw-r--r--   0        0        0     2772 2023-05-23 09:33:34.686656 lcacollect_config-1.5.1/src/lcacollect_config/graphql/input_filters.py
--rw-r--r--   0        0        0     1270 2023-05-23 09:33:34.686656 lcacollect_config-1.5.1/src/lcacollect_config/graphql/pagination.py
--rw-r--r--   0        0        0      400 2023-05-23 09:33:34.686656 lcacollect_config-1.5.1/src/lcacollect_config/permissions.py
--rw-r--r--   0        0        0     1043 2023-05-23 09:33:34.686656 lcacollect_config-1.5.1/src/lcacollect_config/router.py
--rw-r--r--   0        0        0      535 2023-05-23 09:33:34.686656 lcacollect_config-1.5.1/src/lcacollect_config/security.py
--rw-r--r--   0        0        0     5079 2023-05-23 09:33:34.686656 lcacollect_config-1.5.1/src/lcacollect_config/user.py
--rw-r--r--   0        0        0     2634 2023-05-23 09:33:34.686656 lcacollect_config-1.5.1/src/lcacollect_config/validate.py
--rw-r--r--   0        0        0     2144 1970-01-01 00:00:00.000000 lcacollect_config-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0    10173 2023-06-13 11:00:45.514885 lcacollect_config-1.6.0/LICENSE
+-rw-r--r--   0        0        0     1462 2023-06-13 11:00:45.514885 lcacollect_config-1.6.0/README.md
+-rw-r--r--   0        0        0     2520 2023-06-13 11:00:45.514885 lcacollect_config-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-06-13 11:00:45.514885 lcacollect_config-1.6.0/src/lcacollect_config/__init__.py
+-rw-r--r--   0        0        0     2831 2023-06-13 11:00:45.514885 lcacollect_config-1.6.0/src/lcacollect_config/config.py
+-rw-r--r--   0        0        0     1507 2023-06-13 11:00:45.514885 lcacollect_config-1.6.0/src/lcacollect_config/connection.py
+-rw-r--r--   0        0        0      372 2023-06-13 11:00:45.514885 lcacollect_config-1.6.0/src/lcacollect_config/context.py
+-rw-r--r--   0        0        0     2835 2023-06-13 11:00:45.514885 lcacollect_config-1.6.0/src/lcacollect_config/email.py
+-rw-r--r--   0        0        0      263 2023-06-13 11:00:45.514885 lcacollect_config-1.6.0/src/lcacollect_config/exceptions.py
+-rw-r--r--   0        0        0      637 2023-06-13 11:00:45.514885 lcacollect_config-1.6.0/src/lcacollect_config/fastapi.py
+-rw-r--r--   0        0        0      597 2023-06-13 11:00:45.514885 lcacollect_config-1.6.0/src/lcacollect_config/formatting.py
+-rw-r--r--   0        0        0        0 2023-06-13 11:00:45.514885 lcacollect_config-1.6.0/src/lcacollect_config/graphql/__init__.py
+-rw-r--r--   0        0        0     2772 2023-06-13 11:00:45.514885 lcacollect_config-1.6.0/src/lcacollect_config/graphql/input_filters.py
+-rw-r--r--   0        0        0     1270 2023-06-13 11:00:45.514885 lcacollect_config-1.6.0/src/lcacollect_config/graphql/pagination.py
+-rw-r--r--   0        0        0      400 2023-06-13 11:00:45.514885 lcacollect_config-1.6.0/src/lcacollect_config/permissions.py
+-rw-r--r--   0        0        0     1043 2023-06-13 11:00:45.514885 lcacollect_config-1.6.0/src/lcacollect_config/router.py
+-rw-r--r--   0        0        0      535 2023-06-13 11:00:45.514885 lcacollect_config-1.6.0/src/lcacollect_config/security.py
+-rw-r--r--   0        0        0     5079 2023-06-13 11:00:45.514885 lcacollect_config-1.6.0/src/lcacollect_config/user.py
+-rw-r--r--   0        0        0     2634 2023-06-13 11:00:45.514885 lcacollect_config-1.6.0/src/lcacollect_config/validate.py
+-rw-r--r--   0        0        0     2537 1970-01-01 00:00:00.000000 lcacollect_config-1.6.0/PKG-INFO
```

### Comparing `lcacollect_config-1.5.1/README.md` & `lcacollect_config-1.6.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -30,7 +30,16 @@
 manage [versioning of this package](https://dev.azure.com/arkitema/lca-platform/_artifacts/feed/backend-packages/PyPI/lcaconfig/versions)
 . When a new version is ready to be published, remember to update the version by running the following command:
 ```shell
 poetry version minor
 ```
 otherwise the pipeline will fail to publish the package.
 Publishing happens automatically on merges to `main` in an Azure Pipeline.
+
+
+
+# License
+
+Unless otherwise described, the code in this repository is licensed under the Apache-2.0 License. Please note that some
+modules, extensions or code herein might be otherwise licensed. This is indicated either in the root of the containing
+folder under a different license file, or in the respective file's header. If you have any questions, don't hesitate to
+get in touch with us via [email](mailto:chrk@arkitema.com).
```

### Comparing `lcacollect_config-1.5.1/pyproject.toml` & `lcacollect_config-1.6.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 name = "lcacollect-config"
-version = "1.5.1"
+version = "1.6.0"
 description = "This package contains shared config and utils to be used across LCAcollect backends."
 authors = ["Christian Kongsgaard <chrk@arkitema.com>"]
 repository = "https://github.com/lcacollect/shared-config-backend"
-license = "LGPL-3.0-or-later"
+license = "Apache-2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 pydantic = "*"
 strawberry-graphql = {extras = ["fastapi"], version = ">=0.164.0"}
 fastapi-azure-auth = ">=4.0.0"
```

### Comparing `lcacollect_config-1.5.1/src/lcacollect_config/config.py` & `lcacollect_config-1.6.0/src/lcacollect_config/config.py`

 * *Files identical despite different names*

### Comparing `lcacollect_config-1.5.1/src/lcacollect_config/connection.py` & `lcacollect_config-1.6.0/src/lcacollect_config/connection.py`

 * *Files identical despite different names*

### Comparing `lcacollect_config-1.5.1/src/lcacollect_config/email.py` & `lcacollect_config-1.6.0/src/lcacollect_config/email.py`

 * *Files identical despite different names*

### Comparing `lcacollect_config-1.5.1/src/lcacollect_config/fastapi.py` & `lcacollect_config-1.6.0/src/lcacollect_config/fastapi.py`

 * *Files identical despite different names*

### Comparing `lcacollect_config-1.5.1/src/lcacollect_config/formatting.py` & `lcacollect_config-1.6.0/src/lcacollect_config/formatting.py`

 * *Files identical despite different names*

### Comparing `lcacollect_config-1.5.1/src/lcacollect_config/graphql/input_filters.py` & `lcacollect_config-1.6.0/src/lcacollect_config/graphql/input_filters.py`

 * *Files identical despite different names*

### Comparing `lcacollect_config-1.5.1/src/lcacollect_config/graphql/pagination.py` & `lcacollect_config-1.6.0/src/lcacollect_config/graphql/pagination.py`

 * *Files identical despite different names*

### Comparing `lcacollect_config-1.5.1/src/lcacollect_config/router.py` & `lcacollect_config-1.6.0/src/lcacollect_config/router.py`

 * *Files identical despite different names*

### Comparing `lcacollect_config-1.5.1/src/lcacollect_config/security.py` & `lcacollect_config-1.6.0/src/lcacollect_config/security.py`

 * *Files identical despite different names*

### Comparing `lcacollect_config-1.5.1/src/lcacollect_config/user.py` & `lcacollect_config-1.6.0/src/lcacollect_config/user.py`

 * *Files identical despite different names*

### Comparing `lcacollect_config-1.5.1/src/lcacollect_config/validate.py` & `lcacollect_config-1.6.0/src/lcacollect_config/validate.py`

 * *Files identical despite different names*

### Comparing `lcacollect_config-1.5.1/PKG-INFO` & `lcacollect_config-1.6.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: lcacollect-config
-Version: 1.5.1
+Version: 1.6.0
 Summary: This package contains shared config and utils to be used across LCAcollect backends.
 Home-page: https://github.com/lcacollect/shared-config-backend
-License: LGPL-3.0-or-later
+License: Apache-2.0
 Author: Christian Kongsgaard
 Author-email: chrk@arkitema.com
 Requires-Python: >=3.11,<4.0
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: database
 Requires-Dist: SQLAlchemy[asyncio] (>=1.4.35) ; extra == "database"
 Requires-Dist: aiocache
 Requires-Dist: asyncpg (>=0.26.0,<0.27.0) ; extra == "database"
 Requires-Dist: azure-identity
@@ -58,7 +58,15 @@
 . When a new version is ready to be published, remember to update the version by running the following command:
 ```shell
 poetry version minor
 ```
 otherwise the pipeline will fail to publish the package.
 Publishing happens automatically on merges to `main` in an Azure Pipeline.
 
+
+
+# License
+
+Unless otherwise described, the code in this repository is licensed under the Apache-2.0 License. Please note that some
+modules, extensions or code herein might be otherwise licensed. This is indicated either in the root of the containing
+folder under a different license file, or in the respective file's header. If you have any questions, don't hesitate to
+get in touch with us via [email](mailto:chrk@arkitema.com).
```

