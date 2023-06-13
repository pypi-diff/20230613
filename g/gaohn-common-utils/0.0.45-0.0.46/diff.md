# Comparing `tmp/gaohn-common-utils-0.0.45.tar.gz` & `tmp/gaohn-common-utils-0.0.46.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gaohn-common-utils-0.0.45.tar", last modified: Tue Jun 13 07:39:55 2023, max compression
+gzip compressed data, was "gaohn-common-utils-0.0.46.tar", last modified: Tue Jun 13 09:42:45 2023, max compression
```

## Comparing `gaohn-common-utils-0.0.45.tar` & `gaohn-common-utils-0.0.46.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:39:55.945152 gaohn-common-utils-0.0.45/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-13 07:39:27.000000 gaohn-common-utils-0.0.45/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-06-13 07:39:55.945152 gaohn-common-utils-0.0.45/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-06-13 07:39:27.000000 gaohn-common-utils-0.0.45/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:39:55.941152 gaohn-common-utils-0.0.45/common_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 07:39:27.000000 gaohn-common-utils-0.0.45/common_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:39:55.941152 gaohn-common-utils-0.0.45/common_utils/cloud/
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-13 07:39:27.000000 gaohn-common-utils-0.0.45/common_utils/cloud/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:39:55.941152 gaohn-common-utils-0.0.45/common_utils/cloud/gcp/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:39:55.941152 gaohn-common-utils-0.0.45/common_utils/cloud/gcp/database/
--rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-06-13 07:39:27.000000 gaohn-common-utils-0.0.45/common_utils/cloud/gcp/database/bigquery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:39:55.941152 gaohn-common-utils-0.0.45/common_utils/cloud/gcp/storage/
--rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-06-13 07:39:27.000000 gaohn-common-utils-0.0.45/common_utils/cloud/gcp/storage/gcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:39:55.945152 gaohn-common-utils-0.0.45/common_utils/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 07:39:27.000000 gaohn-common-utils-0.0.45/common_utils/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-13 07:39:27.000000 gaohn-common-utils-0.0.45/common_utils/core/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-06-13 07:39:27.000000 gaohn-common-utils-0.0.45/common_utils/core/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-06-13 07:39:27.000000 gaohn-common-utils-0.0.45/common_utils/core/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-06-13 07:39:27.000000 gaohn-common-utils-0.0.45/common_utils/core/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-06-13 07:39:27.000000 gaohn-common-utils-0.0.45/common_utils/core/file_system_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-06-13 07:39:27.000000 gaohn-common-utils-0.0.45/common_utils/core/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:39:55.945152 gaohn-common-utils-0.0.45/common_utils/orchestrator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 07:39:27.000000 gaohn-common-utils-0.0.45/common_utils/orchestrator/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:39:55.941152 gaohn-common-utils-0.0.45/common_utils/versioning/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:39:55.945152 gaohn-common-utils-0.0.45/common_utils/versioning/dvc/
--rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-06-13 07:39:27.000000 gaohn-common-utils-0.0.45/common_utils/versioning/dvc/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:39:55.945152 gaohn-common-utils-0.0.45/gaohn_common_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-06-13 07:39:55.000000 gaohn-common-utils-0.0.45/gaohn_common_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-13 07:39:55.000000 gaohn-common-utils-0.0.45/gaohn_common_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 07:39:55.000000 gaohn-common-utils-0.0.45/gaohn_common_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-13 07:39:55.000000 gaohn-common-utils-0.0.45/gaohn_common_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-13 07:39:55.000000 gaohn-common-utils-0.0.45/gaohn_common_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-06-13 07:39:27.000000 gaohn-common-utils-0.0.45/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 07:39:55.945152 gaohn-common-utils-0.0.45/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:42:45.412915 gaohn-common-utils-0.0.46/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-13 09:42:22.000000 gaohn-common-utils-0.0.46/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-06-13 09:42:45.408915 gaohn-common-utils-0.0.46/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-06-13 09:42:22.000000 gaohn-common-utils-0.0.46/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:42:45.404915 gaohn-common-utils-0.0.46/common_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:42:22.000000 gaohn-common-utils-0.0.46/common_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:42:45.404915 gaohn-common-utils-0.0.46/common_utils/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-13 09:42:22.000000 gaohn-common-utils-0.0.46/common_utils/cloud/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:42:45.404915 gaohn-common-utils-0.0.46/common_utils/cloud/gcp/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:42:45.404915 gaohn-common-utils-0.0.46/common_utils/cloud/gcp/database/
+-rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-06-13 09:42:22.000000 gaohn-common-utils-0.0.46/common_utils/cloud/gcp/database/bigquery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:42:45.408915 gaohn-common-utils-0.0.46/common_utils/cloud/gcp/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-06-13 09:42:22.000000 gaohn-common-utils-0.0.46/common_utils/cloud/gcp/storage/gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:42:45.408915 gaohn-common-utils-0.0.46/common_utils/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:42:22.000000 gaohn-common-utils-0.0.46/common_utils/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-13 09:42:22.000000 gaohn-common-utils-0.0.46/common_utils/core/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-06-13 09:42:22.000000 gaohn-common-utils-0.0.46/common_utils/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-06-13 09:42:22.000000 gaohn-common-utils-0.0.46/common_utils/core/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-06-13 09:42:22.000000 gaohn-common-utils-0.0.46/common_utils/core/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-06-13 09:42:22.000000 gaohn-common-utils-0.0.46/common_utils/core/file_system_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-06-13 09:42:22.000000 gaohn-common-utils-0.0.46/common_utils/core/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:42:45.408915 gaohn-common-utils-0.0.46/common_utils/orchestrator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:42:22.000000 gaohn-common-utils-0.0.46/common_utils/orchestrator/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:42:45.404915 gaohn-common-utils-0.0.46/common_utils/versioning/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:42:45.408915 gaohn-common-utils-0.0.46/common_utils/versioning/dvc/
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-06-13 09:42:22.000000 gaohn-common-utils-0.0.46/common_utils/versioning/dvc/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:42:45.408915 gaohn-common-utils-0.0.46/gaohn_common_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-06-13 09:42:45.000000 gaohn-common-utils-0.0.46/gaohn_common_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-13 09:42:45.000000 gaohn-common-utils-0.0.46/gaohn_common_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 09:42:45.000000 gaohn-common-utils-0.0.46/gaohn_common_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-13 09:42:45.000000 gaohn-common-utils-0.0.46/gaohn_common_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-13 09:42:45.000000 gaohn-common-utils-0.0.46/gaohn_common_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-06-13 09:42:22.000000 gaohn-common-utils-0.0.46/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 09:42:45.412915 gaohn-common-utils-0.0.46/setup.cfg
```

### Comparing `gaohn-common-utils-0.0.45/LICENSE` & `gaohn-common-utils-0.0.46/LICENSE`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.45/PKG-INFO` & `gaohn-common-utils-0.0.46/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaohn-common-utils
-Version: 0.0.45
+Version: 0.0.46
 Summary: A small utility package
 Author-email: Gao Hongnan <hongnangao@gmail.com>
 Project-URL: Homepage, https://github.com/gao-hongnan/common-utils
 Project-URL: Bug Tracker, https://github.com/gao-hongnan/common-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gaohn-common-utils-0.0.45/README.md` & `gaohn-common-utils-0.0.46/README.md`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.45/common_utils/cloud/base.py` & `gaohn-common-utils-0.0.46/common_utils/cloud/base.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.45/common_utils/cloud/gcp/database/bigquery.py` & `gaohn-common-utils-0.0.46/common_utils/cloud/gcp/database/bigquery.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.45/common_utils/cloud/gcp/storage/gcs.py` & `gaohn-common-utils-0.0.46/common_utils/cloud/gcp/storage/gcs.py`

 * *Files 5% similar despite different names*

```diff
@@ -150,7 +150,35 @@
         """
         for file_path in Path(source_dir).glob("**/*"):
             if file_path.is_file():
                 destination_blob_name = (
                     destination_dir + "/" + str(file_path.relative_to(source_dir))
                 )
                 self.upload_blob(str(file_path), destination_blob_name, **kwargs)
+
+    def download_blob(
+        self,
+        source_blob_name: str,
+        destination_file_name: str,
+        **kwargs: Dict[str, Any],
+    ) -> None:
+        """
+        Downloads a blob from the bucket.
+        https://cloud.google.com/storage/docs/downloading-objects
+
+        # The ID of your GCS bucket
+        # bucket_name = "your-bucket-name"
+
+        # The ID of your GCS object
+        # source_blob_name = "storage-object-name"
+
+        # The path to which the file should be downloaded
+        # destination_file_name = "local/path/to/file"
+        """
+
+        # Construct a client side representation of a blob.
+        # Note `Bucket.blob` differs from `Bucket.get_blob` as it doesn't retrieve
+        # any content from Google Cloud Storage. As we don't need additional data,
+        # using `Bucket.blob` is preferred here.
+        blob = self.create_blob(source_blob_name)
+
+        blob.download_to_filename(destination_file_name, **kwargs)
```

### Comparing `gaohn-common-utils-0.0.45/common_utils/core/artifacts.py` & `gaohn-common-utils-0.0.46/common_utils/core/artifacts.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.45/common_utils/core/base.py` & `gaohn-common-utils-0.0.46/common_utils/core/base.py`

 * *Files 11% similar despite different names*

```diff
@@ -57,13 +57,13 @@
         """Save multiple files to a specific location."""
 
     @abstractmethod
     def upload_directory(self) -> None:
         """Save a directory to a specific location."""
 
     @abstractmethod
-    def load_blob(self) -> None:
+    def download_blob(self) -> None:
         """Load a file from a specific location."""
 
     @abstractmethod
-    def load_blobs(self) -> None:
+    def download_blobs(self) -> None:
         """Load multiple files from a specific location."""
```

### Comparing `gaohn-common-utils-0.0.45/common_utils/core/common.py` & `gaohn-common-utils-0.0.46/common_utils/core/common.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.45/common_utils/core/decorators.py` & `gaohn-common-utils-0.0.46/common_utils/core/decorators.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.45/common_utils/core/file_system_utils.py` & `gaohn-common-utils-0.0.46/common_utils/core/file_system_utils.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.45/common_utils/core/logger.py` & `gaohn-common-utils-0.0.46/common_utils/core/logger.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.45/common_utils/versioning/dvc/base.py` & `gaohn-common-utils-0.0.46/common_utils/versioning/dvc/base.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.45/gaohn_common_utils.egg-info/PKG-INFO` & `gaohn-common-utils-0.0.46/gaohn_common_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaohn-common-utils
-Version: 0.0.45
+Version: 0.0.46
 Summary: A small utility package
 Author-email: Gao Hongnan <hongnangao@gmail.com>
 Project-URL: Homepage, https://github.com/gao-hongnan/common-utils
 Project-URL: Bug Tracker, https://github.com/gao-hongnan/common-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gaohn-common-utils-0.0.45/gaohn_common_utils.egg-info/SOURCES.txt` & `gaohn-common-utils-0.0.46/gaohn_common_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.45/pyproject.toml` & `gaohn-common-utils-0.0.46/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gaohn-common-utils"
-version = "0.0.45"
+version = "0.0.46"
 authors = [
   { name="Gao Hongnan", email="hongnangao@gmail.com" },
 ]
 description = "A small utility package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

