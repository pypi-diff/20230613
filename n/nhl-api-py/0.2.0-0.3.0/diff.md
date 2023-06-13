# Comparing `tmp/nhl_api_py-0.2.0.tar.gz` & `tmp/nhl_api_py-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nhl_api_py-0.2.0.tar", max compression
+gzip compressed data, was "nhl_api_py-0.3.0.tar", max compression
```

## Comparing `nhl_api_py-0.2.0.tar` & `nhl_api_py-0.3.0.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0     3702 2023-06-08 18:12:39.049268 nhl_api_py-0.2.0/README.md
--rw-r--r--   0        0        0       34 2023-06-03 14:07:42.805624 nhl_api_py-0.2.0/nhlpy/__init__.py
--rw-r--r--   0        0        0      311 2023-06-03 14:07:42.805624 nhl_api_py-0.2.0/nhlpy/api/__init__.py
--rw-r--r--   0        0        0      743 2023-06-03 14:07:42.805624 nhl_api_py-0.2.0/nhlpy/api/core.py
--rw-r--r--   0        0        0     4171 2023-06-08 18:58:55.919296 nhl_api_py-0.2.0/nhlpy/api/games.py
--rw-r--r--   0        0        0     2016 2023-06-08 18:14:40.069269 nhl_api_py-0.2.0/nhlpy/api/players.py
--rw-r--r--   0        0        0      561 2023-06-03 14:07:42.805624 nhl_api_py-0.2.0/nhlpy/api/schedule.py
--rw-r--r--   0        0        0     1829 2023-06-03 14:07:42.805624 nhl_api_py-0.2.0/nhlpy/api/standings.py
--rw-r--r--   0        0        0     1999 2023-06-03 14:07:42.805624 nhl_api_py-0.2.0/nhlpy/api/teams.py
--rw-r--r--   0        0        0      591 2023-06-08 18:20:08.259272 nhl_api_py-0.2.0/nhlpy/nhl_client.py
--rw-r--r--   0        0        0     1257 2023-06-08 18:59:37.349297 nhl_api_py-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4734 1970-01-01 00:00:00.000000 nhl_api_py-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     3819 2023-06-13 00:29:30.470493 nhl_api_py-0.3.0/README.md
+-rw-r--r--   0        0        0       34 2023-06-03 14:07:42.805624 nhl_api_py-0.3.0/nhlpy/__init__.py
+-rw-r--r--   0        0        0      315 2023-06-09 15:14:25.320047 nhl_api_py-0.3.0/nhlpy/api/__init__.py
+-rw-r--r--   0        0        0      743 2023-06-03 14:07:42.805624 nhl_api_py-0.3.0/nhlpy/api/core.py
+-rw-r--r--   0        0        0     4171 2023-06-08 18:58:55.919296 nhl_api_py-0.3.0/nhlpy/api/games.py
+-rw-r--r--   0        0        0     2856 2023-06-13 00:29:30.470493 nhl_api_py-0.3.0/nhlpy/api/helpers.py
+-rw-r--r--   0        0        0     2016 2023-06-08 18:14:40.069269 nhl_api_py-0.3.0/nhlpy/api/players.py
+-rw-r--r--   0        0        0      561 2023-06-03 14:07:42.805624 nhl_api_py-0.3.0/nhlpy/api/schedule.py
+-rw-r--r--   0        0        0     1829 2023-06-03 14:07:42.805624 nhl_api_py-0.3.0/nhlpy/api/standings.py
+-rw-r--r--   0        0        0     1999 2023-06-03 14:07:42.805624 nhl_api_py-0.3.0/nhlpy/api/teams.py
+-rw-r--r--   0        0        0      641 2023-06-13 00:29:30.470493 nhl_api_py-0.3.0/nhlpy/nhl_client.py
+-rw-r--r--   0        0        0     1277 2023-06-13 00:29:30.470493 nhl_api_py-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4871 1970-01-01 00:00:00.000000 nhl_api_py-0.3.0/PKG-INFO
```

### Comparing `nhl_api_py-0.2.0/README.md` & `nhl_api_py-0.3.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 [![PyPI version](https://badge.fury.io/py/nhl-api-py.svg)](https://badge.fury.io/py/nhl-api-py)
+![nhl-api-py workflow](https://github.com/coreyjs/nhl-api-py/actions/workflows/python-app.yml/badge.svg?branch=main)
 
 # NHL-API-PY
 
 NHL-api-py is a Python package that provides a simple wrapper around the 
 NHL API, allowing you to easily access and retrieve NHL data in your Python 
 applications.
```

### Comparing `nhl_api_py-0.2.0/nhlpy/api/core.py` & `nhl_api_py-0.3.0/nhlpy/api/core.py`

 * *Files identical despite different names*

### Comparing `nhl_api_py-0.2.0/nhlpy/api/games.py` & `nhl_api_py-0.3.0/nhlpy/api/games.py`

 * *Files identical despite different names*

### Comparing `nhl_api_py-0.2.0/nhlpy/api/players.py` & `nhl_api_py-0.3.0/nhlpy/api/players.py`

 * *Files identical despite different names*

### Comparing `nhl_api_py-0.2.0/nhlpy/api/schedule.py` & `nhl_api_py-0.3.0/nhlpy/api/schedule.py`

 * *Files identical despite different names*

### Comparing `nhl_api_py-0.2.0/nhlpy/api/standings.py` & `nhl_api_py-0.3.0/nhlpy/api/standings.py`

 * *Files identical despite different names*

### Comparing `nhl_api_py-0.2.0/nhlpy/api/teams.py` & `nhl_api_py-0.3.0/nhlpy/api/teams.py`

 * *Files identical despite different names*

### Comparing `nhl_api_py-0.2.0/pyproject.toml` & `nhl_api_py-0.3.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "nhl-api-py"
-version = "0.2.0"
-description = "NHL API Wrapper.  For standings, team stats and outcomes."
+version = "0.3.0"
+description = "NHL API Wrapper.  For standings, team stats, outcomes and player information."
 authors = ["Corey Schaf <cschaf@gmail.com>"]
 readme = "README.md"
 packages = [{include = "nhlpy"}]
 license = "GPL-3.0-or-later"
 homepage = "https://github.com/coreyjs/nhl-api-py"
 repository = "https://github.com/coreyjs/nhl-api-py"
 keywords = ["nhl", "api", "wrapper", "hockey", "sports"]
```

### Comparing `nhl_api_py-0.2.0/PKG-INFO` & `nhl_api_py-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: nhl-api-py
-Version: 0.2.0
-Summary: NHL API Wrapper.  For standings, team stats and outcomes.
+Version: 0.3.0
+Summary: NHL API Wrapper.  For standings, team stats, outcomes and player information.
 Home-page: https://github.com/coreyjs/nhl-api-py
 License: GPL-3.0-or-later
 Keywords: nhl,api,wrapper,hockey,sports
 Author: Corey Schaf
 Author-email: cschaf@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -19,14 +19,15 @@
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: httpx
 Project-URL: Repository, https://github.com/coreyjs/nhl-api-py
 Description-Content-Type: text/markdown
 
 [![PyPI version](https://badge.fury.io/py/nhl-api-py.svg)](https://badge.fury.io/py/nhl-api-py)
+![nhl-api-py workflow](https://github.com/coreyjs/nhl-api-py/actions/workflows/python-app.yml/badge.svg?branch=main)
 
 # NHL-API-PY
 
 NHL-api-py is a Python package that provides a simple wrapper around the 
 NHL API, allowing you to easily access and retrieve NHL data in your Python 
 applications.
```

