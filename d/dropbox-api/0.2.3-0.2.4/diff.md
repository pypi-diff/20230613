# Comparing `tmp/dropbox-api-0.2.3.tar.gz` & `tmp/dropbox-api-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dropbox-api-0.2.3.tar", last modified: Tue Jun 13 16:11:33 2023, max compression
+gzip compressed data, was "dist/dropbox-api-0.2.4.tar", last modified: Tue Jun 13 17:31:15 2023, max compression
```

## Comparing `dropbox-api-0.2.3.tar` & `dropbox-api-0.2.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 16:11:33.000000 dropbox-api-0.2.3/
--rw-r--r--   0 root         (0) root         (0)       67 2023-06-13 16:11:33.000000 dropbox-api-0.2.3/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 16:11:33.000000 dropbox-api-0.2.3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 16:11:33.000000 dropbox-api-0.2.3/src/dropbox/
--rw-r--r--   0 root         (0) root         (0)     1655 2023-06-13 16:11:27.000000 dropbox-api-0.2.3/src/dropbox/user.py
--rw-r--r--   0 root         (0) root         (0)     1406 2023-06-13 16:11:27.000000 dropbox-api-0.2.3/src/dropbox/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1829 2023-06-13 16:11:27.000000 dropbox-api-0.2.3/src/dropbox/shared_link.py
--rw-r--r--   0 root         (0) root         (0)     6715 2023-06-13 16:11:27.000000 dropbox-api-0.2.3/src/dropbox/base.py
--rw-r--r--   0 root         (0) root         (0)     6218 2023-06-13 16:11:27.000000 dropbox-api-0.2.3/src/dropbox/file.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 16:11:33.000000 dropbox-api-0.2.3/src/dropbox_api.egg-info/
--rw-r--r--   0 root         (0) root         (0)        7 2023-06-13 16:11:33.000000 dropbox-api-0.2.3/src/dropbox_api.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 16:11:33.000000 dropbox-api-0.2.3/src/dropbox_api.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      371 2023-06-13 16:11:33.000000 dropbox-api-0.2.3/src/dropbox_api.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     2460 2023-06-13 16:11:33.000000 dropbox-api-0.2.3/src/dropbox_api.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-13 16:11:33.000000 dropbox-api-0.2.3/src/dropbox_api.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 16:11:29.000000 dropbox-api-0.2.3/src/dropbox_api.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)     2460 2023-06-13 16:11:33.000000 dropbox-api-0.2.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2732 2023-06-13 16:11:27.000000 dropbox-api-0.2.3/setup.py
--rw-r--r--   0 root         (0) root         (0)     1250 2023-06-13 16:11:27.000000 dropbox-api-0.2.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 17:31:15.000000 dropbox-api-0.2.4/
+-rw-r--r--   0 root         (0) root         (0)       67 2023-06-13 17:31:15.000000 dropbox-api-0.2.4/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 17:31:15.000000 dropbox-api-0.2.4/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 17:31:15.000000 dropbox-api-0.2.4/src/dropbox/
+-rw-r--r--   0 root         (0) root         (0)     1655 2023-06-13 17:31:09.000000 dropbox-api-0.2.4/src/dropbox/user.py
+-rw-r--r--   0 root         (0) root         (0)     1406 2023-06-13 17:31:09.000000 dropbox-api-0.2.4/src/dropbox/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1829 2023-06-13 17:31:09.000000 dropbox-api-0.2.4/src/dropbox/shared_link.py
+-rw-r--r--   0 root         (0) root         (0)     6668 2023-06-13 17:31:09.000000 dropbox-api-0.2.4/src/dropbox/base.py
+-rw-r--r--   0 root         (0) root         (0)     6218 2023-06-13 17:31:09.000000 dropbox-api-0.2.4/src/dropbox/file.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 17:31:15.000000 dropbox-api-0.2.4/src/dropbox_api.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        7 2023-06-13 17:31:15.000000 dropbox-api-0.2.4/src/dropbox_api.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 17:31:15.000000 dropbox-api-0.2.4/src/dropbox_api.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      371 2023-06-13 17:31:15.000000 dropbox-api-0.2.4/src/dropbox_api.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     2460 2023-06-13 17:31:15.000000 dropbox-api-0.2.4/src/dropbox_api.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-13 17:31:15.000000 dropbox-api-0.2.4/src/dropbox_api.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 17:31:11.000000 dropbox-api-0.2.4/src/dropbox_api.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)     2460 2023-06-13 17:31:15.000000 dropbox-api-0.2.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2732 2023-06-13 17:31:09.000000 dropbox-api-0.2.4/setup.py
+-rw-r--r--   0 root         (0) root         (0)     1250 2023-06-13 17:31:09.000000 dropbox-api-0.2.4/README.md
```

### Comparing `dropbox-api-0.2.3/src/dropbox/user.py` & `dropbox-api-0.2.4/src/dropbox/user.py`

 * *Files identical despite different names*

### Comparing `dropbox-api-0.2.3/src/dropbox/__init__.py` & `dropbox-api-0.2.4/src/dropbox/__init__.py`

 * *Files identical despite different names*

### Comparing `dropbox-api-0.2.3/src/dropbox/shared_link.py` & `dropbox-api-0.2.4/src/dropbox/shared_link.py`

 * *Files identical despite different names*

### Comparing `dropbox-api-0.2.3/src/dropbox/base.py` & `dropbox-api-0.2.4/src/dropbox/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,13 +179,12 @@
         contents = self.post(
             url,
             callback = False,
             token = False,
             client_id = self.client_id,
             client_secret = self.client_secret,
             grant_type = "refresh_token",
-            redirect_uri = self.redirect_url,
             refresh_token = self.refresh_token
         )
         self.access_token = contents["access_token"]
         self.trigger("access_token", self.access_token)
         return self.access_token
```

### Comparing `dropbox-api-0.2.3/src/dropbox/file.py` & `dropbox-api-0.2.4/src/dropbox/file.py`

 * *Files identical despite different names*

### Comparing `dropbox-api-0.2.3/src/dropbox_api.egg-info/PKG-INFO` & `dropbox-api-0.2.4/src/dropbox_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dropbox-api
-Version: 0.2.3
+Version: 0.2.4
 Summary: Dropbox API Client
 Home-page: http://dropbox-api.hive.pt
 Author: Hive Solutions Lda.
 Author-email: development@hive.pt
 License: Apache License, Version 2.0
 Description: # [Dropbox API](http://dropbox-api.hive.pt)
```

### Comparing `dropbox-api-0.2.3/PKG-INFO` & `dropbox-api-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dropbox-api
-Version: 0.2.3
+Version: 0.2.4
 Summary: Dropbox API Client
 Home-page: http://dropbox-api.hive.pt
 Author: Hive Solutions Lda.
 Author-email: development@hive.pt
 License: Apache License, Version 2.0
 Description: # [Dropbox API](http://dropbox-api.hive.pt)
```

### Comparing `dropbox-api-0.2.3/setup.py` & `dropbox-api-0.2.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 """ The license for the module """
 
 import os
 import setuptools
 
 setuptools.setup(
     name = "dropbox-api",
-    version = "0.2.3",
+    version = "0.2.4",
     author = "Hive Solutions Lda.",
     author_email = "development@hive.pt",
     description = "Dropbox API Client",
     license = "Apache License, Version 2.0",
     keywords = "dropbox api",
     url = "http://dropbox-api.hive.pt",
     zip_safe = False,
```

### Comparing `dropbox-api-0.2.3/README.md` & `dropbox-api-0.2.4/README.md`

 * *Files identical despite different names*

