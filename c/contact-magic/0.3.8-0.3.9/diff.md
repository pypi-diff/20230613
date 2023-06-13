# Comparing `tmp/contact_magic-0.3.8.tar.gz` & `tmp/contact_magic-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contact_magic-0.3.8.tar", max compression
+gzip compressed data, was "contact_magic-0.3.9.tar", max compression
```

## Comparing `contact_magic-0.3.8.tar` & `contact_magic-0.3.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     4514 2023-06-09 23:55:24.983205 contact_magic-0.3.8/README.md
--rw-r--r--   0        0        0      280 2023-06-11 21:59:22.389422 contact_magic-0.3.8/contact_magic/__init__.py
--rw-r--r--   0        0        0      977 2023-06-11 23:20:08.446401 contact_magic-0.3.8/contact_magic/asyncio.py
--rw-r--r--   0        0        0       51 2023-06-10 00:10:37.013402 contact_magic-0.3.8/contact_magic/conf/__init__.py
--rw-r--r--   0        0        0     5209 2023-06-11 23:14:52.369840 contact_magic-0.3.8/contact_magic/conf/settings.py
--rw-r--r--   0        0        0     3359 2023-06-11 22:03:43.467264 contact_magic-0.3.8/contact_magic/helpers.py
--rw-r--r--   0        0        0      121 2023-06-07 09:00:51.259272 contact_magic-0.3.8/contact_magic/integrations/__init__.py
--rw-r--r--   0        0        0     2177 2023-06-11 12:02:22.673968 contact_magic-0.3.8/contact_magic/integrations/copyfactory.py
--rw-r--r--   0        0        0     1498 2023-06-11 12:02:22.663490 contact_magic-0.3.8/contact_magic/integrations/sales_scrapers.py
--rw-r--r--   0        0        0     1447 2023-06-09 23:24:56.319390 contact_magic-0.3.8/contact_magic/integrations/sheets.py
--rw-r--r--   0        0        0       65 2023-06-08 09:44:27.736870 contact_magic-0.3.8/contact_magic/logger.py
--rw-r--r--   0        0        0    12297 2023-06-11 23:14:52.374634 contact_magic-0.3.8/contact_magic/models.py
--rw-r--r--   0        0        0     3080 2023-06-11 22:22:02.791793 contact_magic-0.3.8/contact_magic/preprocessors.py
--rw-r--r--   0        0        0        0 2023-06-09 17:35:50.408715 contact_magic-0.3.8/contact_magic/scripts/__init__.py
--rw-r--r--   0        0        0     1601 2023-06-10 00:10:37.396531 contact_magic-0.3.8/contact_magic/scripts/agency.py
--rw-r--r--   0        0        0       61 2023-06-08 09:10:28.353224 contact_magic-0.3.8/contact_magic/scripts/logger.py
--rw-r--r--   0        0        0     4083 2023-06-11 10:34:51.812723 contact_magic-0.3.8/contact_magic/scripts/run_workflows.py
--rw-r--r--   0        0        0     2073 2023-06-10 00:10:37.400242 contact_magic-0.3.8/contact_magic/scripts/update_workflow_approval_metrics.py
--rw-r--r--   0        0        0     3441 2023-06-10 22:11:15.781991 contact_magic-0.3.8/contact_magic/utils.py
--rw-r--r--   0        0        0     1710 2023-06-11 23:19:54.178623 contact_magic-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     6201 1970-01-01 00:00:00.000000 contact_magic-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0     4514 2023-06-09 23:55:24.983205 contact_magic-0.3.9/README.md
+-rw-r--r--   0        0        0      280 2023-06-11 21:59:22.389422 contact_magic-0.3.9/contact_magic/__init__.py
+-rw-r--r--   0        0        0     1159 2023-06-13 07:02:38.019401 contact_magic-0.3.9/contact_magic/asyncio.py
+-rw-r--r--   0        0        0       51 2023-06-10 00:10:37.013402 contact_magic-0.3.9/contact_magic/conf/__init__.py
+-rw-r--r--   0        0        0     5209 2023-06-11 23:14:52.369840 contact_magic-0.3.9/contact_magic/conf/settings.py
+-rw-r--r--   0        0        0     3359 2023-06-11 22:03:43.467264 contact_magic-0.3.9/contact_magic/helpers.py
+-rw-r--r--   0        0        0      121 2023-06-07 09:00:51.259272 contact_magic-0.3.9/contact_magic/integrations/__init__.py
+-rw-r--r--   0        0        0     2177 2023-06-13 06:14:51.344787 contact_magic-0.3.9/contact_magic/integrations/copyfactory.py
+-rw-r--r--   0        0        0     1498 2023-06-11 12:02:22.663490 contact_magic-0.3.9/contact_magic/integrations/sales_scrapers.py
+-rw-r--r--   0        0        0     1447 2023-06-09 23:24:56.319390 contact_magic-0.3.9/contact_magic/integrations/sheets.py
+-rw-r--r--   0        0        0       65 2023-06-08 09:44:27.736870 contact_magic-0.3.9/contact_magic/logger.py
+-rw-r--r--   0        0        0    12297 2023-06-11 23:14:52.374634 contact_magic-0.3.9/contact_magic/models.py
+-rw-r--r--   0        0        0     3080 2023-06-11 22:22:02.791793 contact_magic-0.3.9/contact_magic/preprocessors.py
+-rw-r--r--   0        0        0        0 2023-06-09 17:35:50.408715 contact_magic-0.3.9/contact_magic/scripts/__init__.py
+-rw-r--r--   0        0        0     1601 2023-06-10 00:10:37.396531 contact_magic-0.3.9/contact_magic/scripts/agency.py
+-rw-r--r--   0        0        0       61 2023-06-08 09:10:28.353224 contact_magic-0.3.9/contact_magic/scripts/logger.py
+-rw-r--r--   0        0        0     4083 2023-06-11 10:34:51.812723 contact_magic-0.3.9/contact_magic/scripts/run_workflows.py
+-rw-r--r--   0        0        0     2073 2023-06-10 00:10:37.400242 contact_magic-0.3.9/contact_magic/scripts/update_workflow_approval_metrics.py
+-rw-r--r--   0        0        0     3441 2023-06-10 22:11:15.781991 contact_magic-0.3.9/contact_magic/utils.py
+-rw-r--r--   0        0        0     1710 2023-06-13 07:02:20.259410 contact_magic-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0     6201 1970-01-01 00:00:00.000000 contact_magic-0.3.9/PKG-INFO
```

### Comparing `contact_magic-0.3.8/README.md` & `contact_magic-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `contact_magic-0.3.8/contact_magic/asyncio.py` & `contact_magic-0.3.9/contact_magic/asyncio.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import asyncio
 from asyncio import QueueEmpty
 
 from contact_magic.conf.settings import SETTINGS
+from contact_magic.logger import logger
 
 
 async def do_bulk(ops: list, max_workers: int = SETTINGS.MAX_WORKERS):
     """
     Bulk operation
     This function can be used to run bulk operations
     using a limited number of concurrent requests.
@@ -31,10 +32,15 @@
         except QueueEmpty:
             break
 
         try:
             response = await op[0](**op[1])
             results[index] = response
         except Exception as e:
-            # log warning
-            results[index] = {"data": {}, "index": 0}
+            logger.error(
+                "processing_row",
+                row_number=op[1]["row"].index,
+                status="ERROR",
+                message=e,
+            )
+            results[index] = op[1]["row"]
         queue.task_done()
```

### Comparing `contact_magic-0.3.8/contact_magic/conf/settings.py` & `contact_magic-0.3.9/contact_magic/conf/settings.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.3.8/contact_magic/helpers.py` & `contact_magic-0.3.9/contact_magic/helpers.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.3.8/contact_magic/integrations/copyfactory.py` & `contact_magic-0.3.9/contact_magic/integrations/copyfactory.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.3.8/contact_magic/integrations/sales_scrapers.py` & `contact_magic-0.3.9/contact_magic/integrations/sales_scrapers.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.3.8/contact_magic/integrations/sheets.py` & `contact_magic-0.3.9/contact_magic/integrations/sheets.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.3.8/contact_magic/models.py` & `contact_magic-0.3.9/contact_magic/models.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.3.8/contact_magic/preprocessors.py` & `contact_magic-0.3.9/contact_magic/preprocessors.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.3.8/contact_magic/scripts/agency.py` & `contact_magic-0.3.9/contact_magic/scripts/agency.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.3.8/contact_magic/scripts/run_workflows.py` & `contact_magic-0.3.9/contact_magic/scripts/run_workflows.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.3.8/contact_magic/scripts/update_workflow_approval_metrics.py` & `contact_magic-0.3.9/contact_magic/scripts/update_workflow_approval_metrics.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.3.8/contact_magic/utils.py` & `contact_magic-0.3.9/contact_magic/utils.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.3.8/pyproject.toml` & `contact_magic-0.3.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "contact-magic"
-version = "0.3.8"
+version = "0.3.9"
 description = "Quickly set up workflows for retrieving hard-to-find contact information and composing personalized messages based on any data point."
 authors = ["Copyfactory <dev@copyfactory.io>"]
 readme = "README.md"
 packages = [
     { include = "contact_magic"}
 ]
 license = "MIT"
```

### Comparing `contact_magic-0.3.8/PKG-INFO` & `contact_magic-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contact-magic
-Version: 0.3.8
+Version: 0.3.9
 Summary: Quickly set up workflows for retrieving hard-to-find contact information and composing personalized messages based on any data point.
 License: MIT
 Author: Copyfactory
 Author-email: dev@copyfactory.io
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

