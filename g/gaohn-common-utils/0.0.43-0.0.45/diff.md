# Comparing `tmp/gaohn-common-utils-0.0.43.tar.gz` & `tmp/gaohn-common-utils-0.0.45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gaohn-common-utils-0.0.43.tar", last modified: Tue Jun 13 07:23:39 2023, max compression
+gzip compressed data, was "gaohn-common-utils-0.0.45.tar", last modified: Tue Jun 13 07:39:55 2023, max compression
```

## Comparing `gaohn-common-utils-0.0.43.tar` & `gaohn-common-utils-0.0.45.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:23:39.120857 gaohn-common-utils-0.0.43/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-13 07:23:18.000000 gaohn-common-utils-0.0.43/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-06-13 07:23:39.120857 gaohn-common-utils-0.0.43/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-06-13 07:23:18.000000 gaohn-common-utils-0.0.43/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:23:39.116857 gaohn-common-utils-0.0.43/common_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 07:23:18.000000 gaohn-common-utils-0.0.43/common_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:23:39.116857 gaohn-common-utils-0.0.43/common_utils/cloud/
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-13 07:23:18.000000 gaohn-common-utils-0.0.43/common_utils/cloud/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:23:39.112857 gaohn-common-utils-0.0.43/common_utils/cloud/gcp/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:23:39.116857 gaohn-common-utils-0.0.43/common_utils/cloud/gcp/database/
--rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-06-13 07:23:18.000000 gaohn-common-utils-0.0.43/common_utils/cloud/gcp/database/bigquery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:23:39.116857 gaohn-common-utils-0.0.43/common_utils/cloud/gcp/storage/
--rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-06-13 07:23:18.000000 gaohn-common-utils-0.0.43/common_utils/cloud/gcp/storage/gcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:23:39.116857 gaohn-common-utils-0.0.43/common_utils/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 07:23:18.000000 gaohn-common-utils-0.0.43/common_utils/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-13 07:23:18.000000 gaohn-common-utils-0.0.43/common_utils/core/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-06-13 07:23:18.000000 gaohn-common-utils-0.0.43/common_utils/core/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-06-13 07:23:18.000000 gaohn-common-utils-0.0.43/common_utils/core/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-06-13 07:23:18.000000 gaohn-common-utils-0.0.43/common_utils/core/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-06-13 07:23:18.000000 gaohn-common-utils-0.0.43/common_utils/core/file_system_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-06-13 07:23:18.000000 gaohn-common-utils-0.0.43/common_utils/core/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:23:39.120857 gaohn-common-utils-0.0.43/common_utils/orchestrator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 07:23:18.000000 gaohn-common-utils-0.0.43/common_utils/orchestrator/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:23:39.112857 gaohn-common-utils-0.0.43/common_utils/versioning/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:23:39.120857 gaohn-common-utils-0.0.43/common_utils/versioning/dvc/
--rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-06-13 07:23:18.000000 gaohn-common-utils-0.0.43/common_utils/versioning/dvc/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:23:39.120857 gaohn-common-utils-0.0.43/gaohn_common_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-06-13 07:23:39.000000 gaohn-common-utils-0.0.43/gaohn_common_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-13 07:23:39.000000 gaohn-common-utils-0.0.43/gaohn_common_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 07:23:39.000000 gaohn-common-utils-0.0.43/gaohn_common_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-13 07:23:39.000000 gaohn-common-utils-0.0.43/gaohn_common_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-13 07:23:39.000000 gaohn-common-utils-0.0.43/gaohn_common_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-06-13 07:23:18.000000 gaohn-common-utils-0.0.43/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 07:23:39.120857 gaohn-common-utils-0.0.43/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:39:55.945152 gaohn-common-utils-0.0.45/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-13 07:39:27.000000 gaohn-common-utils-0.0.45/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-06-13 07:39:55.945152 gaohn-common-utils-0.0.45/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-06-13 07:39:27.000000 gaohn-common-utils-0.0.45/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:39:55.941152 gaohn-common-utils-0.0.45/common_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 07:39:27.000000 gaohn-common-utils-0.0.45/common_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:39:55.941152 gaohn-common-utils-0.0.45/common_utils/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-13 07:39:27.000000 gaohn-common-utils-0.0.45/common_utils/cloud/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:39:55.941152 gaohn-common-utils-0.0.45/common_utils/cloud/gcp/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:39:55.941152 gaohn-common-utils-0.0.45/common_utils/cloud/gcp/database/
+-rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-06-13 07:39:27.000000 gaohn-common-utils-0.0.45/common_utils/cloud/gcp/database/bigquery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:39:55.941152 gaohn-common-utils-0.0.45/common_utils/cloud/gcp/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-06-13 07:39:27.000000 gaohn-common-utils-0.0.45/common_utils/cloud/gcp/storage/gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:39:55.945152 gaohn-common-utils-0.0.45/common_utils/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 07:39:27.000000 gaohn-common-utils-0.0.45/common_utils/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-13 07:39:27.000000 gaohn-common-utils-0.0.45/common_utils/core/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-06-13 07:39:27.000000 gaohn-common-utils-0.0.45/common_utils/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-06-13 07:39:27.000000 gaohn-common-utils-0.0.45/common_utils/core/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-06-13 07:39:27.000000 gaohn-common-utils-0.0.45/common_utils/core/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-06-13 07:39:27.000000 gaohn-common-utils-0.0.45/common_utils/core/file_system_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-06-13 07:39:27.000000 gaohn-common-utils-0.0.45/common_utils/core/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:39:55.945152 gaohn-common-utils-0.0.45/common_utils/orchestrator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 07:39:27.000000 gaohn-common-utils-0.0.45/common_utils/orchestrator/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:39:55.941152 gaohn-common-utils-0.0.45/common_utils/versioning/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:39:55.945152 gaohn-common-utils-0.0.45/common_utils/versioning/dvc/
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-06-13 07:39:27.000000 gaohn-common-utils-0.0.45/common_utils/versioning/dvc/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:39:55.945152 gaohn-common-utils-0.0.45/gaohn_common_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-06-13 07:39:55.000000 gaohn-common-utils-0.0.45/gaohn_common_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-13 07:39:55.000000 gaohn-common-utils-0.0.45/gaohn_common_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 07:39:55.000000 gaohn-common-utils-0.0.45/gaohn_common_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-13 07:39:55.000000 gaohn-common-utils-0.0.45/gaohn_common_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-13 07:39:55.000000 gaohn-common-utils-0.0.45/gaohn_common_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-06-13 07:39:27.000000 gaohn-common-utils-0.0.45/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 07:39:55.945152 gaohn-common-utils-0.0.45/setup.cfg
```

### Comparing `gaohn-common-utils-0.0.43/LICENSE` & `gaohn-common-utils-0.0.45/LICENSE`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.43/PKG-INFO` & `gaohn-common-utils-0.0.45/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaohn-common-utils
-Version: 0.0.43
+Version: 0.0.45
 Summary: A small utility package
 Author-email: Gao Hongnan <hongnangao@gmail.com>
 Project-URL: Homepage, https://github.com/gao-hongnan/common-utils
 Project-URL: Bug Tracker, https://github.com/gao-hongnan/common-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gaohn-common-utils-0.0.43/README.md` & `gaohn-common-utils-0.0.45/README.md`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.43/common_utils/cloud/base.py` & `gaohn-common-utils-0.0.45/common_utils/cloud/base.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.43/common_utils/cloud/gcp/database/bigquery.py` & `gaohn-common-utils-0.0.45/common_utils/cloud/gcp/database/bigquery.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.43/common_utils/cloud/gcp/storage/gcs.py` & `gaohn-common-utils-0.0.45/common_utils/cloud/gcp/storage/gcs.py`

 * *Files 3% similar despite different names*

```diff
@@ -94,15 +94,15 @@
         """Creates a new blob in the bucket. See upload_blob for example."""
         blob = self.bucket.blob(destination_blob_name)
         return blob
 
     def upload_blob(
         self,
         source_file_name: str,
-        blob: storage.Blob,
+        destination_blob_name: str,
         **kwargs: Dict[str, Any],
     ) -> None:
         """
         Uploads a file to a GCS bucket.
         https://cloud.google.com/storage/docs/uploading-objects#storage-upload-object-client-libraries
 
         # The ID of your GCS bucket
@@ -129,14 +129,16 @@
         # and data corruptions. The request to upload is aborted if the object's
         # generation number does not match your precondition. For a destination
         # object that does not yet exist, set the if_generation_match precondition to 0.
         # If the destination object already exists in your bucket, set instead a
         # generation-match precondition using its generation number.
         generation_match_precondition = 0
 
+        blob = self.create_blob(destination_blob_name)
+
         blob.upload_from_filename(
             source_file_name,
             if_generation_match=generation_match_precondition,
             **kwargs,
         )
 
     def upload_directory(
```

### Comparing `gaohn-common-utils-0.0.43/common_utils/core/artifacts.py` & `gaohn-common-utils-0.0.45/common_utils/core/artifacts.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.43/common_utils/core/base.py` & `gaohn-common-utils-0.0.45/common_utils/core/base.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.43/common_utils/core/common.py` & `gaohn-common-utils-0.0.45/common_utils/core/common.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.43/common_utils/core/decorators.py` & `gaohn-common-utils-0.0.45/common_utils/core/decorators.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.43/common_utils/core/file_system_utils.py` & `gaohn-common-utils-0.0.45/common_utils/core/file_system_utils.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.43/common_utils/core/logger.py` & `gaohn-common-utils-0.0.45/common_utils/core/logger.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.43/common_utils/versioning/dvc/base.py` & `gaohn-common-utils-0.0.45/common_utils/versioning/dvc/base.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.43/gaohn_common_utils.egg-info/PKG-INFO` & `gaohn-common-utils-0.0.45/gaohn_common_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaohn-common-utils
-Version: 0.0.43
+Version: 0.0.45
 Summary: A small utility package
 Author-email: Gao Hongnan <hongnangao@gmail.com>
 Project-URL: Homepage, https://github.com/gao-hongnan/common-utils
 Project-URL: Bug Tracker, https://github.com/gao-hongnan/common-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gaohn-common-utils-0.0.43/gaohn_common_utils.egg-info/SOURCES.txt` & `gaohn-common-utils-0.0.45/gaohn_common_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.43/pyproject.toml` & `gaohn-common-utils-0.0.45/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gaohn-common-utils"
-version = "0.0.43"
+version = "0.0.45"
 authors = [
   { name="Gao Hongnan", email="hongnangao@gmail.com" },
 ]
 description = "A small utility package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

