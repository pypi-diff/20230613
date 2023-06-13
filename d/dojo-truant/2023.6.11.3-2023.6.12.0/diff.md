# Comparing `tmp/dojo_truant-2023.6.11.3.tar.gz` & `tmp/dojo_truant-2023.6.12.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dojo_truant-2023.6.11.3.tar", last modified: Mon Jun 12 04:22:30 2023, max compression
+gzip compressed data, was "dojo_truant-2023.6.12.0.tar", last modified: Tue Jun 13 04:54:22 2023, max compression
```

## Comparing `dojo_truant-2023.6.11.3.tar` & `dojo_truant-2023.6.12.0.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:22:30.150029 dojo_truant-2023.6.11.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-06-12 04:22:11.000000 dojo_truant-2023.6.11.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-12 04:22:30.150029 dojo_truant-2023.6.11.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-12 04:22:11.000000 dojo_truant-2023.6.11.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:22:30.146029 dojo_truant-2023.6.11.3/dojo/
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-12 04:22:11.000000 dojo_truant-2023.6.11.3/dojo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12014 2023-06-12 04:22:11.000000 dojo_truant-2023.6.11.3/dojo/api.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 04:22:11.000000 dojo_truant-2023.6.11.3/dojo/api_multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-06-12 04:22:11.000000 dojo_truant-2023.6.11.3/dojo/development_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-06-12 04:22:11.000000 dojo_truant-2023.6.11.3/dojo/dojo_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-06-12 04:22:11.000000 dojo_truant-2023.6.11.3/dojo/engagement.py
--rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-06-12 04:22:11.000000 dojo_truant-2023.6.11.3/dojo/finding.py
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-06-12 04:22:11.000000 dojo_truant-2023.6.11.3/dojo/product.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-12 04:22:11.000000 dojo_truant-2023.6.11.3/dojo/product_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-12 04:22:11.000000 dojo_truant-2023.6.11.3/dojo/stub_finding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-06-12 04:22:11.000000 dojo_truant-2023.6.11.3/dojo/test.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-12 04:22:11.000000 dojo_truant-2023.6.11.3/dojo/test_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-06-12 04:22:11.000000 dojo_truant-2023.6.11.3/dojo/write_chain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 04:22:30.150029 dojo_truant-2023.6.11.3/dojo_truant.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-12 04:22:30.000000 dojo_truant-2023.6.11.3/dojo_truant.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-12 04:22:30.000000 dojo_truant-2023.6.11.3/dojo_truant.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 04:22:30.000000 dojo_truant-2023.6.11.3/dojo_truant.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-12 04:22:30.000000 dojo_truant-2023.6.11.3/dojo_truant.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-12 04:22:30.000000 dojo_truant-2023.6.11.3/dojo_truant.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-12 04:22:11.000000 dojo_truant-2023.6.11.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 04:22:30.150029 dojo_truant-2023.6.11.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 04:54:22.153690 dojo_truant-2023.6.12.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-06-13 04:54:04.000000 dojo_truant-2023.6.12.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-13 04:54:22.153690 dojo_truant-2023.6.12.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-13 04:54:04.000000 dojo_truant-2023.6.12.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 04:54:22.149690 dojo_truant-2023.6.12.0/dojo/
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-13 04:54:04.000000 dojo_truant-2023.6.12.0/dojo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12014 2023-06-13 04:54:04.000000 dojo_truant-2023.6.12.0/dojo/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 04:54:04.000000 dojo_truant-2023.6.12.0/dojo/api_multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-06-13 04:54:04.000000 dojo_truant-2023.6.12.0/dojo/development_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-13 04:54:04.000000 dojo_truant-2023.6.12.0/dojo/dojo_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-06-13 04:54:04.000000 dojo_truant-2023.6.12.0/dojo/engagement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-06-13 04:54:04.000000 dojo_truant-2023.6.12.0/dojo/finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-06-13 04:54:04.000000 dojo_truant-2023.6.12.0/dojo/jira_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-06-13 04:54:04.000000 dojo_truant-2023.6.12.0/dojo/jira_product_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-06-13 04:54:04.000000 dojo_truant-2023.6.12.0/dojo/product.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-13 04:54:04.000000 dojo_truant-2023.6.12.0/dojo/product_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-13 04:54:04.000000 dojo_truant-2023.6.12.0/dojo/stub_finding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-06-13 04:54:04.000000 dojo_truant-2023.6.12.0/dojo/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-13 04:54:04.000000 dojo_truant-2023.6.12.0/dojo/test_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-06-13 04:54:04.000000 dojo_truant-2023.6.12.0/dojo/write_chain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 04:54:22.153690 dojo_truant-2023.6.12.0/dojo_truant.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-13 04:54:22.000000 dojo_truant-2023.6.12.0/dojo_truant.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-13 04:54:22.000000 dojo_truant-2023.6.12.0/dojo_truant.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 04:54:22.000000 dojo_truant-2023.6.12.0/dojo_truant.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-13 04:54:22.000000 dojo_truant-2023.6.12.0/dojo_truant.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-13 04:54:22.000000 dojo_truant-2023.6.12.0/dojo_truant.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-13 04:54:04.000000 dojo_truant-2023.6.12.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 04:54:22.153690 dojo_truant-2023.6.12.0/setup.cfg
```

### Comparing `dojo_truant-2023.6.11.3/LICENSE.txt` & `dojo_truant-2023.6.12.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.6.11.3/PKG-INFO` & `dojo_truant-2023.6.12.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dojo_truant
-Version: 2023.6.11.3
+Version: 2023.6.12.0
 Summary: A minimal client for deject dojo to be used by me in my projects. Some functionality may be absent.
 Author-email: Chris Halbersma <chalbersma@auditboard.com>
 License: BSD-3-Clause
 Keywords: defectDojo
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
```

### Comparing `dojo_truant-2023.6.11.3/dojo/__init__.py` & `dojo_truant-2023.6.12.0/dojo/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -9,15 +9,20 @@
 from .test_type import Test_Type
 from .development_environment import Development_Environment
 from .test import Test
 
 from .finding import Finding
 from .stub_finding import Stub_Finding
 
+from .jira_instance import Jira_Instance
+from .jira_product_configuration import Jira_Product_Configuration
+
 from .write_chain import write_chain
 
 
 ID_LOOKUPS = {"prod_type": Product_Type,
               "group": Dojo_Group,
               "engagement": Engagement,
               "test_type": Test_Type,
-              "environment": Development_Environment}
+              "environment": Development_Environment,
+              "jira_instance": Jira_Instance,
+              "product": Product}
```

### Comparing `dojo_truant-2023.6.11.3/dojo/api.py` & `dojo_truant-2023.6.12.0/dojo/api.py`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.6.11.3/dojo/development_environment.py` & `dojo_truant-2023.6.12.0/dojo/development_environment.py`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.6.11.3/dojo/dojo_group.py` & `dojo_truant-2023.6.12.0/dojo/dojo_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,8 +26,8 @@
     _obj_iterate = ".results[]"
 
     _type = "dojo_group"
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
 
-        self.logger = logging.getLogger("DAPI.Product_Type")
+        self.logger = logging.getLogger("DAPI.Dojo_Group")
```

### Comparing `dojo_truant-2023.6.11.3/dojo/engagement.py` & `dojo_truant-2023.6.12.0/dojo/engagement.py`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.6.11.3/dojo/finding.py` & `dojo_truant-2023.6.12.0/dojo/finding.py`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.6.11.3/dojo/product.py` & `dojo_truant-2023.6.12.0/dojo/product.py`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.6.11.3/dojo/product_type.py` & `dojo_truant-2023.6.12.0/dojo/product_type.py`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.6.11.3/dojo/stub_finding.py` & `dojo_truant-2023.6.12.0/dojo/stub_finding.py`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.6.11.3/dojo/test.py` & `dojo_truant-2023.6.12.0/dojo/test.py`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.6.11.3/dojo/test_type.py` & `dojo_truant-2023.6.12.0/dojo/test_type.py`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.6.11.3/dojo/write_chain.py` & `dojo_truant-2023.6.12.0/dojo/write_chain.py`

 * *Files identical despite different names*

### Comparing `dojo_truant-2023.6.11.3/dojo_truant.egg-info/PKG-INFO` & `dojo_truant-2023.6.12.0/dojo_truant.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dojo-truant
-Version: 2023.6.11.3
+Version: 2023.6.12.0
 Summary: A minimal client for deject dojo to be used by me in my projects. Some functionality may be absent.
 Author-email: Chris Halbersma <chalbersma@auditboard.com>
 License: BSD-3-Clause
 Keywords: defectDojo
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
```

### Comparing `dojo_truant-2023.6.11.3/pyproject.toml` & `dojo_truant-2023.6.12.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
   "twine",
   "setuptools"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dojo_truant"
-version = "2023.6.11.3"
+version = "2023.6.12.0"
 authors = [
     {name = "Chris Halbersma", email = "chalbersma@auditboard.com"},
 ]
 description = "A minimal client for deject dojo to be used by me in my projects. Some functionality may be absent."
 readme = "README.md"
 requires-python = ">=3.11"
 keywords = ["defectDojo"]
```

