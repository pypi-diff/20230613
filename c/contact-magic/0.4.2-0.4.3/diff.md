# Comparing `tmp/contact_magic-0.4.2.tar.gz` & `tmp/contact_magic-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contact_magic-0.4.2.tar", max compression
+gzip compressed data, was "contact_magic-0.4.3.tar", max compression
```

## Comparing `contact_magic-0.4.2.tar` & `contact_magic-0.4.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     4514 2023-06-09 23:55:24.983205 contact_magic-0.4.2/README.md
--rw-r--r--   0        0        0      280 2023-06-11 21:59:22.389422 contact_magic-0.4.2/contact_magic/__init__.py
--rw-r--r--   0        0        0     1159 2023-06-13 07:02:38.019401 contact_magic-0.4.2/contact_magic/asyncio.py
--rw-r--r--   0        0        0       51 2023-06-10 00:10:37.013402 contact_magic-0.4.2/contact_magic/conf/__init__.py
--rw-r--r--   0        0        0     5209 2023-06-11 23:14:52.369840 contact_magic-0.4.2/contact_magic/conf/settings.py
--rw-r--r--   0        0        0     3359 2023-06-11 22:03:43.467264 contact_magic-0.4.2/contact_magic/helpers.py
--rw-r--r--   0        0        0      121 2023-06-07 09:00:51.259272 contact_magic-0.4.2/contact_magic/integrations/__init__.py
--rw-r--r--   0        0        0     2177 2023-06-13 06:14:51.344787 contact_magic-0.4.2/contact_magic/integrations/copyfactory.py
--rw-r--r--   0        0        0     1498 2023-06-11 12:02:22.663490 contact_magic-0.4.2/contact_magic/integrations/sales_scrapers.py
--rw-r--r--   0        0        0     1638 2023-06-13 07:39:32.822031 contact_magic-0.4.2/contact_magic/integrations/sheets.py
--rw-r--r--   0        0        0       65 2023-06-08 09:44:27.736870 contact_magic-0.4.2/contact_magic/logger.py
--rw-r--r--   0        0        0    12297 2023-06-11 23:14:52.374634 contact_magic-0.4.2/contact_magic/models.py
--rw-r--r--   0        0        0     3080 2023-06-11 22:22:02.791793 contact_magic-0.4.2/contact_magic/preprocessors.py
--rw-r--r--   0        0        0        0 2023-06-09 17:35:50.408715 contact_magic-0.4.2/contact_magic/scripts/__init__.py
--rw-r--r--   0        0        0     1601 2023-06-10 00:10:37.396531 contact_magic-0.4.2/contact_magic/scripts/agency.py
--rw-r--r--   0        0        0       61 2023-06-08 09:10:28.353224 contact_magic-0.4.2/contact_magic/scripts/logger.py
--rw-r--r--   0        0        0     4266 2023-06-13 07:39:32.815975 contact_magic-0.4.2/contact_magic/scripts/run_workflows.py
--rw-r--r--   0        0        0     2073 2023-06-10 00:10:37.400242 contact_magic-0.4.2/contact_magic/scripts/update_workflow_approval_metrics.py
--rw-r--r--   0        0        0     3441 2023-06-10 22:11:15.781991 contact_magic-0.4.2/contact_magic/utils.py
--rw-r--r--   0        0        0     1960 2023-06-13 07:58:17.804446 contact_magic-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     6308 1970-01-01 00:00:00.000000 contact_magic-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     4514 2023-06-09 23:55:24.983205 contact_magic-0.4.3/README.md
+-rw-r--r--   0        0        0      280 2023-06-11 21:59:22.389422 contact_magic-0.4.3/contact_magic/__init__.py
+-rw-r--r--   0        0        0     1159 2023-06-13 07:02:38.019401 contact_magic-0.4.3/contact_magic/asyncio.py
+-rw-r--r--   0        0        0       51 2023-06-10 00:10:37.013402 contact_magic-0.4.3/contact_magic/conf/__init__.py
+-rw-r--r--   0        0        0     5209 2023-06-11 23:14:52.369840 contact_magic-0.4.3/contact_magic/conf/settings.py
+-rw-r--r--   0        0        0     3359 2023-06-11 22:03:43.467264 contact_magic-0.4.3/contact_magic/helpers.py
+-rw-r--r--   0        0        0      121 2023-06-07 09:00:51.259272 contact_magic-0.4.3/contact_magic/integrations/__init__.py
+-rw-r--r--   0        0        0     2177 2023-06-13 06:14:51.344787 contact_magic-0.4.3/contact_magic/integrations/copyfactory.py
+-rw-r--r--   0        0        0     1498 2023-06-11 12:02:22.663490 contact_magic-0.4.3/contact_magic/integrations/sales_scrapers.py
+-rw-r--r--   0        0        0     1638 2023-06-13 07:39:32.822031 contact_magic-0.4.3/contact_magic/integrations/sheets.py
+-rw-r--r--   0        0        0       65 2023-06-08 09:44:27.736870 contact_magic-0.4.3/contact_magic/logger.py
+-rw-r--r--   0        0        0    12297 2023-06-11 23:14:52.374634 contact_magic-0.4.3/contact_magic/models.py
+-rw-r--r--   0        0        0     3080 2023-06-11 22:22:02.791793 contact_magic-0.4.3/contact_magic/preprocessors.py
+-rw-r--r--   0        0        0        0 2023-06-09 17:35:50.408715 contact_magic-0.4.3/contact_magic/scripts/__init__.py
+-rw-r--r--   0        0        0     1601 2023-06-10 00:10:37.396531 contact_magic-0.4.3/contact_magic/scripts/agency.py
+-rw-r--r--   0        0        0       61 2023-06-08 09:10:28.353224 contact_magic-0.4.3/contact_magic/scripts/logger.py
+-rw-r--r--   0        0        0     4266 2023-06-13 07:39:32.815975 contact_magic-0.4.3/contact_magic/scripts/run_workflows.py
+-rw-r--r--   0        0        0     2073 2023-06-10 00:10:37.400242 contact_magic-0.4.3/contact_magic/scripts/update_workflow_approval_metrics.py
+-rw-r--r--   0        0        0     3441 2023-06-10 22:11:15.781991 contact_magic-0.4.3/contact_magic/utils.py
+-rw-r--r--   0        0        0     1903 2023-06-13 08:14:13.348239 contact_magic-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     6284 1970-01-01 00:00:00.000000 contact_magic-0.4.3/PKG-INFO
```

### Comparing `contact_magic-0.4.2/README.md` & `contact_magic-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `contact_magic-0.4.2/contact_magic/asyncio.py` & `contact_magic-0.4.3/contact_magic/asyncio.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.4.2/contact_magic/conf/settings.py` & `contact_magic-0.4.3/contact_magic/conf/settings.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.4.2/contact_magic/helpers.py` & `contact_magic-0.4.3/contact_magic/helpers.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.4.2/contact_magic/integrations/copyfactory.py` & `contact_magic-0.4.3/contact_magic/integrations/copyfactory.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.4.2/contact_magic/integrations/sales_scrapers.py` & `contact_magic-0.4.3/contact_magic/integrations/sales_scrapers.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.4.2/contact_magic/integrations/sheets.py` & `contact_magic-0.4.3/contact_magic/integrations/sheets.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.4.2/contact_magic/models.py` & `contact_magic-0.4.3/contact_magic/models.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.4.2/contact_magic/preprocessors.py` & `contact_magic-0.4.3/contact_magic/preprocessors.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.4.2/contact_magic/scripts/agency.py` & `contact_magic-0.4.3/contact_magic/scripts/agency.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.4.2/contact_magic/scripts/run_workflows.py` & `contact_magic-0.4.3/contact_magic/scripts/run_workflows.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.4.2/contact_magic/scripts/update_workflow_approval_metrics.py` & `contact_magic-0.4.3/contact_magic/scripts/update_workflow_approval_metrics.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.4.2/contact_magic/utils.py` & `contact_magic-0.4.3/contact_magic/utils.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.4.2/pyproject.toml` & `contact_magic-0.4.3/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "contact-magic"
-version = "0.4.2"
+version = "0.4.3"
 description = "Quickly set up workflows for retrieving hard-to-find contact information and composing personalized messages based on any data point."
 authors = ["Copyfactory <dev@copyfactory.io>"]
 readme = "README.md"
 packages = [
     { include = "contact_magic"}
 ]
 license = "MIT"
@@ -35,17 +35,17 @@
 typer = {extras = ["all"], version = "^0.9.0"}
 httpx = "^0.24.1"
 pandas = "^2.0.2"
 python-dotenv = "^1.0.0"
 pydantic = "1.10.8"
 structlog = "23.1.0"
 rich = "^13.4.1"
-gspread = {version="4.0.1", extras=["sheets"], optional = true}
-oauth2client = {version="4.1.3", extras=["sheets"], optional = true}
-oauthlib = {version="3.1.1", extras=["sheets"], optional = true}
+gspread = {version="4.0.1", optional = true}
+oauth2client = {version="4.1.3", optional = true}
+oauthlib = {version="3.1.1", optional = true}
 
 [tool.poetry.extras]
 sheets = ["gspread", "oauth2client", "oauthlib"]
 
 [tool.poetry.scripts]
 contact-magic = "contact_magic.scripts.agency:app"
```

### Comparing `contact_magic-0.4.2/PKG-INFO` & `contact_magic-0.4.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contact-magic
-Version: 0.4.2
+Version: 0.4.3
 Summary: Quickly set up workflows for retrieving hard-to-find contact information and composing personalized messages based on any data point.
 License: MIT
 Author: Copyfactory
 Author-email: dev@copyfactory.io
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
@@ -23,18 +23,18 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Provides-Extra: sheets
-Requires-Dist: gspread[sheets] (==4.0.1) ; extra == "sheets"
+Requires-Dist: gspread (==4.0.1) ; extra == "sheets"
 Requires-Dist: httpx (>=0.24.1,<0.25.0)
-Requires-Dist: oauth2client[sheets] (==4.1.3) ; extra == "sheets"
-Requires-Dist: oauthlib[sheets] (==3.1.1) ; extra == "sheets"
+Requires-Dist: oauth2client (==4.1.3) ; extra == "sheets"
+Requires-Dist: oauthlib (==3.1.1) ; extra == "sheets"
 Requires-Dist: pandas (>=2.0.2,<3.0.0)
 Requires-Dist: pydantic (==1.10.8)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: rich (>=13.4.1,<14.0.0)
 Requires-Dist: structlog (==23.1.0)
 Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
```

