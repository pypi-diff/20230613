# Comparing `tmp/azure-batch-8.0.0.zip` & `tmp/azure-batch-9.0.0.zip`

## zipinfo {}

```diff
@@ -1,45 +1,48 @@
-Zip file size: 241961 bytes, number of entries: 43
-drwxr-xr-x  2.0 unx        0 b- stor 19-Aug-12 18:45 azure-batch-8.0.0/
-drwxr-xr-x  2.0 unx        0 b- stor 19-Aug-12 18:45 azure-batch-8.0.0/azure_batch.egg-info/
-drwxr-xr-x  2.0 unx        0 b- stor 19-Aug-12 18:45 azure-batch-8.0.0/azure/
--rw-r--r--  2.0 unx       67 b- defN 19-Aug-12 18:45 azure-batch-8.0.0/setup.cfg
--rw-r--r--  2.0 unx    17350 b- defN 19-Aug-12 18:45 azure-batch-8.0.0/PKG-INFO
--rw-r--r--  2.0 unx       41 b- defN 19-Aug-12 18:45 azure-batch-8.0.0/MANIFEST.in
--rw-r--r--  2.0 unx     1227 b- defN 19-Aug-12 18:45 azure-batch-8.0.0/README.rst
--rw-r--r--  2.0 unx    13296 b- defN 19-Aug-12 18:45 azure-batch-8.0.0/HISTORY.rst
--rw-r--r--  2.0 unx     2844 b- defN 19-Aug-12 18:45 azure-batch-8.0.0/setup.py
--rw-r--r--  2.0 unx       96 b- defN 19-Aug-12 18:45 azure-batch-8.0.0/azure_batch.egg-info/requires.txt
--rw-r--r--  2.0 unx        6 b- defN 19-Aug-12 18:45 azure-batch-8.0.0/azure_batch.egg-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 19-Aug-12 18:45 azure-batch-8.0.0/azure_batch.egg-info/not-zip-safe
--rw-r--r--  2.0 unx        1 b- defN 19-Aug-12 18:45 azure-batch-8.0.0/azure_batch.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx    17350 b- defN 19-Aug-12 18:45 azure-batch-8.0.0/azure_batch.egg-info/PKG-INFO
--rw-r--r--  2.0 unx     1149 b- defN 19-Aug-12 18:45 azure-batch-8.0.0/azure_batch.egg-info/SOURCES.txt
-drwxr-xr-x  2.0 unx        0 b- stor 19-Aug-12 18:45 azure-batch-8.0.0/azure/batch/
--rw-r--r--  2.0 unx       65 b- defN 19-Aug-12 18:45 azure-batch-8.0.0/azure/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 19-Aug-12 18:45 azure-batch-8.0.0/azure/batch/models/
-drwxr-xr-x  2.0 unx        0 b- stor 19-Aug-12 18:45 azure-batch-8.0.0/azure/batch/custom/
-drwxr-xr-x  2.0 unx        0 b- stor 19-Aug-12 18:45 azure-batch-8.0.0/azure/batch/operations/
--rw-r--r--  2.0 unx      710 b- defN 19-Aug-12 18:45 azure-batch-8.0.0/azure/batch/__init__.py
--rw-r--r--  2.0 unx     1720 b- defN 19-Aug-12 18:45 azure-batch-8.0.0/azure/batch/_configuration.py
--rw-r--r--  2.0 unx     3688 b- defN 19-Aug-12 18:45 azure-batch-8.0.0/azure/batch/batch_auth.py
--rw-r--r--  2.0 unx     4037 b- defN 19-Aug-12 18:45 azure-batch-8.0.0/azure/batch/_batch_service_client.py
--rw-r--r--  2.0 unx      493 b- defN 19-Aug-12 18:45 azure-batch-8.0.0/azure/batch/version.py
--rw-r--r--  2.0 unx   534905 b- defN 19-Aug-12 18:45 azure-batch-8.0.0/azure/batch/models/_models.py
--rw-r--r--  2.0 unx    29575 b- defN 19-Aug-12 18:45 azure-batch-8.0.0/azure/batch/models/__init__.py
--rw-r--r--  2.0 unx     5926 b- defN 19-Aug-12 18:45 azure-batch-8.0.0/azure/batch/models/_paged_models.py
--rw-r--r--  2.0 unx   539918 b- defN 19-Aug-12 18:45 azure-batch-8.0.0/azure/batch/models/_models_py3.py
--rw-r--r--  2.0 unx    21049 b- defN 19-Aug-12 18:45 azure-batch-8.0.0/azure/batch/models/_batch_service_client_enums.py
--rw-r--r--  2.0 unx        0 b- defN 19-Aug-12 18:45 azure-batch-8.0.0/azure/batch/custom/__init__.py
--rw-r--r--  2.0 unx    14752 b- defN 19-Aug-12 18:45 azure-batch-8.0.0/azure/batch/custom/patch.py
--rw-r--r--  2.0 unx     2215 b- defN 19-Aug-12 18:45 azure-batch-8.0.0/azure/batch/custom/custom_errors.py
--rw-r--r--  2.0 unx     1184 b- defN 19-Aug-12 18:45 azure-batch-8.0.0/azure/batch/operations/__init__.py
--rw-r--r--  2.0 unx    55787 b- defN 19-Aug-12 18:45 azure-batch-8.0.0/azure/batch/operations/_job_schedule_operations.py
--rw-r--r--  2.0 unx    51139 b- defN 19-Aug-12 18:45 azure-batch-8.0.0/azure/batch/operations/_task_operations.py
--rw-r--r--  2.0 unx    62199 b- defN 19-Aug-12 18:45 azure-batch-8.0.0/azure/batch/operations/_compute_node_operations.py
--rw-r--r--  2.0 unx    45246 b- defN 19-Aug-12 18:45 azure-batch-8.0.0/azure/batch/operations/_file_operations.py
--rw-r--r--  2.0 unx    72816 b- defN 19-Aug-12 18:45 azure-batch-8.0.0/azure/batch/operations/_job_operations.py
--rw-r--r--  2.0 unx    83342 b- defN 19-Aug-12 18:45 azure-batch-8.0.0/azure/batch/operations/_pool_operations.py
--rw-r--r--  2.0 unx    10850 b- defN 19-Aug-12 18:45 azure-batch-8.0.0/azure/batch/operations/_application_operations.py
--rw-r--r--  2.0 unx    25429 b- defN 19-Aug-12 18:45 azure-batch-8.0.0/azure/batch/operations/_certificate_operations.py
--rw-r--r--  2.0 unx    11428 b- defN 19-Aug-12 18:45 azure-batch-8.0.0/azure/batch/operations/_account_operations.py
-43 files, 1631901 bytes uncompressed, 234677 bytes compressed:  85.6%
+Zip file size: 256873 bytes, number of entries: 46
+drwxr-xr-x  2.0 unx        0 b- stor 20-Mar-26 17:45 azure-batch-9.0.0/
+drwxr-xr-x  2.0 unx        0 b- stor 20-Mar-26 17:45 azure-batch-9.0.0/azure/
+drwxr-xr-x  2.0 unx        0 b- stor 20-Mar-26 17:45 azure-batch-9.0.0/azure_batch.egg-info/
+drwxr-xr-x  2.0 unx        0 b- stor 20-Mar-26 17:45 azure-batch-9.0.0/tests/
+-rw-r--r--  2.0 unx       68 b- defN 20-Mar-26 17:44 azure-batch-9.0.0/MANIFEST.in
+-rw-r--r--  2.0 unx       67 b- defN 20-Mar-26 17:45 azure-batch-9.0.0/setup.cfg
+-rw-r--r--  2.0 unx    17584 b- defN 20-Mar-26 17:45 azure-batch-9.0.0/PKG-INFO
+-rw-r--r--  2.0 unx     2852 b- defN 20-Mar-26 17:44 azure-batch-9.0.0/setup.py
+-rw-r--r--  2.0 unx     1143 b- defN 20-Mar-26 17:45 azure-batch-9.0.0/README.md
+-rw-r--r--  2.0 unx    13747 b- defN 20-Mar-26 17:44 azure-batch-9.0.0/CHANGELOG.md
+drwxr-xr-x  2.0 unx        0 b- stor 20-Mar-26 17:45 azure-batch-9.0.0/azure/batch/
+-rw-r--r--  2.0 unx       65 b- defN 20-Mar-26 17:44 azure-batch-9.0.0/azure/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 20-Mar-26 17:45 azure-batch-9.0.0/azure/batch/operations/
+drwxr-xr-x  2.0 unx        0 b- stor 20-Mar-26 17:45 azure-batch-9.0.0/azure/batch/models/
+drwxr-xr-x  2.0 unx        0 b- stor 20-Mar-26 17:45 azure-batch-9.0.0/azure/batch/custom/
+-rw-r--r--  2.0 unx      493 b- defN 20-Mar-26 17:44 azure-batch-9.0.0/azure/batch/_version.py
+-rw-r--r--  2.0 unx     1721 b- defN 20-Mar-26 17:44 azure-batch-9.0.0/azure/batch/_configuration.py
+-rw-r--r--  2.0 unx      711 b- defN 20-Mar-26 17:44 azure-batch-9.0.0/azure/batch/__init__.py
+-rw-r--r--  2.0 unx     3688 b- defN 20-Mar-26 17:44 azure-batch-9.0.0/azure/batch/batch_auth.py
+-rw-r--r--  2.0 unx     4036 b- defN 20-Mar-26 17:44 azure-batch-9.0.0/azure/batch/_batch_service_client.py
+-rw-r--r--  2.0 unx    25429 b- defN 20-Mar-26 17:44 azure-batch-9.0.0/azure/batch/operations/_certificate_operations.py
+-rw-r--r--  2.0 unx    55787 b- defN 20-Mar-26 17:44 azure-batch-9.0.0/azure/batch/operations/_job_schedule_operations.py
+-rw-r--r--  2.0 unx    45246 b- defN 20-Mar-26 17:44 azure-batch-9.0.0/azure/batch/operations/_file_operations.py
+-rw-r--r--  2.0 unx    83342 b- defN 20-Mar-26 17:44 azure-batch-9.0.0/azure/batch/operations/_pool_operations.py
+-rw-r--r--  2.0 unx    11428 b- defN 20-Mar-26 17:44 azure-batch-9.0.0/azure/batch/operations/_account_operations.py
+-rw-r--r--  2.0 unx    72816 b- defN 20-Mar-26 17:44 azure-batch-9.0.0/azure/batch/operations/_job_operations.py
+-rw-r--r--  2.0 unx    10850 b- defN 20-Mar-26 17:44 azure-batch-9.0.0/azure/batch/operations/_application_operations.py
+-rw-r--r--  2.0 unx    62199 b- defN 20-Mar-26 17:44 azure-batch-9.0.0/azure/batch/operations/_compute_node_operations.py
+-rw-r--r--  2.0 unx     1184 b- defN 20-Mar-26 17:44 azure-batch-9.0.0/azure/batch/operations/__init__.py
+-rw-r--r--  2.0 unx    51139 b- defN 20-Mar-26 17:44 azure-batch-9.0.0/azure/batch/operations/_task_operations.py
+-rw-r--r--  2.0 unx    21805 b- defN 20-Mar-26 17:44 azure-batch-9.0.0/azure/batch/models/_batch_service_client_enums.py
+-rw-r--r--  2.0 unx   537286 b- defN 20-Mar-26 17:44 azure-batch-9.0.0/azure/batch/models/_models.py
+-rw-r--r--  2.0 unx   542349 b- defN 20-Mar-26 17:44 azure-batch-9.0.0/azure/batch/models/_models_py3.py
+-rw-r--r--  2.0 unx    29986 b- defN 20-Mar-26 17:44 azure-batch-9.0.0/azure/batch/models/__init__.py
+-rw-r--r--  2.0 unx     5903 b- defN 20-Mar-26 17:44 azure-batch-9.0.0/azure/batch/models/_paged_models.py
+-rw-r--r--  2.0 unx     2175 b- defN 20-Mar-26 17:44 azure-batch-9.0.0/azure/batch/custom/custom_errors.py
+-rw-r--r--  2.0 unx        0 b- defN 20-Mar-26 17:44 azure-batch-9.0.0/azure/batch/custom/__init__.py
+-rw-r--r--  2.0 unx    14752 b- defN 20-Mar-26 17:44 azure-batch-9.0.0/azure/batch/custom/patch.py
+-rw-r--r--  2.0 unx       96 b- defN 20-Mar-26 17:45 azure-batch-9.0.0/azure_batch.egg-info/requires.txt
+-rw-r--r--  2.0 unx    17584 b- defN 20-Mar-26 17:45 azure-batch-9.0.0/azure_batch.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx        6 b- defN 20-Mar-26 17:45 azure-batch-9.0.0/azure_batch.egg-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 20-Mar-26 17:45 azure-batch-9.0.0/azure_batch.egg-info/dependency_links.txt
+-rw-r--r--  2.0 unx        1 b- defN 20-Mar-26 17:45 azure-batch-9.0.0/azure_batch.egg-info/not-zip-safe
+-rw-r--r--  2.0 unx     1195 b- defN 20-Mar-26 17:45 azure-batch-9.0.0/azure_batch.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx    13216 b- defN 20-Mar-26 17:44 azure-batch-9.0.0/tests/batch_preparers.py
+-rw-r--r--  2.0 unx    49713 b- defN 20-Mar-26 17:44 azure-batch-9.0.0/tests/test_batch.py
+46 files, 1701663 bytes uncompressed, 249153 bytes compressed:  85.4%
```

## zipnote {}

```diff
@@ -1,130 +1,139 @@
-Filename: azure-batch-8.0.0/
+Filename: azure-batch-9.0.0/
 Comment: 
 
-Filename: azure-batch-8.0.0/azure_batch.egg-info/
+Filename: azure-batch-9.0.0/azure/
 Comment: 
 
-Filename: azure-batch-8.0.0/azure/
+Filename: azure-batch-9.0.0/azure_batch.egg-info/
 Comment: 
 
-Filename: azure-batch-8.0.0/setup.cfg
+Filename: azure-batch-9.0.0/tests/
 Comment: 
 
-Filename: azure-batch-8.0.0/PKG-INFO
+Filename: azure-batch-9.0.0/MANIFEST.in
 Comment: 
 
-Filename: azure-batch-8.0.0/MANIFEST.in
+Filename: azure-batch-9.0.0/setup.cfg
 Comment: 
 
-Filename: azure-batch-8.0.0/README.rst
+Filename: azure-batch-9.0.0/PKG-INFO
 Comment: 
 
-Filename: azure-batch-8.0.0/HISTORY.rst
+Filename: azure-batch-9.0.0/setup.py
 Comment: 
 
-Filename: azure-batch-8.0.0/setup.py
+Filename: azure-batch-9.0.0/README.md
 Comment: 
 
-Filename: azure-batch-8.0.0/azure_batch.egg-info/requires.txt
+Filename: azure-batch-9.0.0/CHANGELOG.md
 Comment: 
 
-Filename: azure-batch-8.0.0/azure_batch.egg-info/top_level.txt
+Filename: azure-batch-9.0.0/azure/batch/
 Comment: 
 
-Filename: azure-batch-8.0.0/azure_batch.egg-info/not-zip-safe
+Filename: azure-batch-9.0.0/azure/__init__.py
 Comment: 
 
-Filename: azure-batch-8.0.0/azure_batch.egg-info/dependency_links.txt
+Filename: azure-batch-9.0.0/azure/batch/operations/
 Comment: 
 
-Filename: azure-batch-8.0.0/azure_batch.egg-info/PKG-INFO
+Filename: azure-batch-9.0.0/azure/batch/models/
 Comment: 
 
-Filename: azure-batch-8.0.0/azure_batch.egg-info/SOURCES.txt
+Filename: azure-batch-9.0.0/azure/batch/custom/
 Comment: 
 
-Filename: azure-batch-8.0.0/azure/batch/
+Filename: azure-batch-9.0.0/azure/batch/_version.py
 Comment: 
 
-Filename: azure-batch-8.0.0/azure/__init__.py
+Filename: azure-batch-9.0.0/azure/batch/_configuration.py
 Comment: 
 
-Filename: azure-batch-8.0.0/azure/batch/models/
+Filename: azure-batch-9.0.0/azure/batch/__init__.py
 Comment: 
 
-Filename: azure-batch-8.0.0/azure/batch/custom/
+Filename: azure-batch-9.0.0/azure/batch/batch_auth.py
 Comment: 
 
-Filename: azure-batch-8.0.0/azure/batch/operations/
+Filename: azure-batch-9.0.0/azure/batch/_batch_service_client.py
 Comment: 
 
-Filename: azure-batch-8.0.0/azure/batch/__init__.py
+Filename: azure-batch-9.0.0/azure/batch/operations/_certificate_operations.py
 Comment: 
 
-Filename: azure-batch-8.0.0/azure/batch/_configuration.py
+Filename: azure-batch-9.0.0/azure/batch/operations/_job_schedule_operations.py
 Comment: 
 
-Filename: azure-batch-8.0.0/azure/batch/batch_auth.py
+Filename: azure-batch-9.0.0/azure/batch/operations/_file_operations.py
 Comment: 
 
-Filename: azure-batch-8.0.0/azure/batch/_batch_service_client.py
+Filename: azure-batch-9.0.0/azure/batch/operations/_pool_operations.py
 Comment: 
 
-Filename: azure-batch-8.0.0/azure/batch/version.py
+Filename: azure-batch-9.0.0/azure/batch/operations/_account_operations.py
 Comment: 
 
-Filename: azure-batch-8.0.0/azure/batch/models/_models.py
+Filename: azure-batch-9.0.0/azure/batch/operations/_job_operations.py
 Comment: 
 
-Filename: azure-batch-8.0.0/azure/batch/models/__init__.py
+Filename: azure-batch-9.0.0/azure/batch/operations/_application_operations.py
 Comment: 
 
-Filename: azure-batch-8.0.0/azure/batch/models/_paged_models.py
+Filename: azure-batch-9.0.0/azure/batch/operations/_compute_node_operations.py
 Comment: 
 
-Filename: azure-batch-8.0.0/azure/batch/models/_models_py3.py
+Filename: azure-batch-9.0.0/azure/batch/operations/__init__.py
 Comment: 
 
-Filename: azure-batch-8.0.0/azure/batch/models/_batch_service_client_enums.py
+Filename: azure-batch-9.0.0/azure/batch/operations/_task_operations.py
 Comment: 
 
-Filename: azure-batch-8.0.0/azure/batch/custom/__init__.py
+Filename: azure-batch-9.0.0/azure/batch/models/_batch_service_client_enums.py
 Comment: 
 
-Filename: azure-batch-8.0.0/azure/batch/custom/patch.py
+Filename: azure-batch-9.0.0/azure/batch/models/_models.py
 Comment: 
 
-Filename: azure-batch-8.0.0/azure/batch/custom/custom_errors.py
+Filename: azure-batch-9.0.0/azure/batch/models/_models_py3.py
 Comment: 
 
-Filename: azure-batch-8.0.0/azure/batch/operations/__init__.py
+Filename: azure-batch-9.0.0/azure/batch/models/__init__.py
 Comment: 
 
-Filename: azure-batch-8.0.0/azure/batch/operations/_job_schedule_operations.py
+Filename: azure-batch-9.0.0/azure/batch/models/_paged_models.py
 Comment: 
 
-Filename: azure-batch-8.0.0/azure/batch/operations/_task_operations.py
+Filename: azure-batch-9.0.0/azure/batch/custom/custom_errors.py
 Comment: 
 
-Filename: azure-batch-8.0.0/azure/batch/operations/_compute_node_operations.py
+Filename: azure-batch-9.0.0/azure/batch/custom/__init__.py
 Comment: 
 
-Filename: azure-batch-8.0.0/azure/batch/operations/_file_operations.py
+Filename: azure-batch-9.0.0/azure/batch/custom/patch.py
 Comment: 
 
-Filename: azure-batch-8.0.0/azure/batch/operations/_job_operations.py
+Filename: azure-batch-9.0.0/azure_batch.egg-info/requires.txt
 Comment: 
 
-Filename: azure-batch-8.0.0/azure/batch/operations/_pool_operations.py
+Filename: azure-batch-9.0.0/azure_batch.egg-info/PKG-INFO
 Comment: 
 
-Filename: azure-batch-8.0.0/azure/batch/operations/_application_operations.py
+Filename: azure-batch-9.0.0/azure_batch.egg-info/top_level.txt
 Comment: 
 
-Filename: azure-batch-8.0.0/azure/batch/operations/_certificate_operations.py
+Filename: azure-batch-9.0.0/azure_batch.egg-info/dependency_links.txt
 Comment: 
 
-Filename: azure-batch-8.0.0/azure/batch/operations/_account_operations.py
+Filename: azure-batch-9.0.0/azure_batch.egg-info/not-zip-safe
+Comment: 
+
+Filename: azure-batch-9.0.0/azure_batch.egg-info/SOURCES.txt
+Comment: 
+
+Filename: azure-batch-9.0.0/tests/batch_preparers.py
+Comment: 
+
+Filename: azure-batch-9.0.0/tests/test_batch.py
 Comment: 
 
 Zip file comment:
```

## Comparing `azure-batch-8.0.0/PKG-INFO` & `azure-batch-9.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,95 +1,93 @@
 Metadata-Version: 2.1
 Name: azure-batch
-Version: 8.0.0
+Version: 9.0.0
 Summary: Microsoft Azure Batch Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
-Description: Microsoft Azure SDK for Python
-        ==============================
+Description: # Microsoft Azure SDK for Python
         
         This is the Microsoft Azure Batch Client Library.
         
         This package has been tested with Python 2.7, 3.4, 3.5, 3.6 and 3.7.
         
-        For a more complete set of Azure libraries, see the `azure <https://pypi.python.org/pypi/azure>`__ bundle package.
+        For a more complete set of Azure libraries, see the [azure](https://pypi.python.org/pypi/azure) bundle package.
         
         
-        Compatibility
-        =============
+        # Compatibility
         
         **IMPORTANT**: If you have an earlier version of the azure package
         (version < 1.0), you should uninstall it before installing this package.
         
         You can check the version using pip:
         
-        .. code:: shell
-        
-            pip freeze
+        ```shell
+        pip freeze
+        ```
         
         If you see azure==0.11.0 (or any version below 1.0), uninstall it first:
         
-        .. code:: shell
-        
-            pip uninstall azure
+        ```shell
+        pip uninstall azure
+        ```
         
         
-        Usage
-        =====
+        # Usage
         
-        For code examples, see `the Batch samples repo
-        <https://github.com/Azure/azure-batch-samples/tree/master/Python>`__
-        on GitHub or see `Batch
-        <https://docs.microsoft.com/python/api/overview/azure/batch>`__
+        For code examples, see [the Batch samples repo](https://github.com/Azure/azure-batch-samples/tree/master/Python)
+        on GitHub or see [Batch](https://docs.microsoft.com/python/api/overview/azure/batch)
         on docs.microsoft.com.
         
         
-        Provide Feedback
-        ================
+        # Provide Feedback
         
         If you encounter any bugs or have suggestions, please file an issue in the
-        `Issues <https://github.com/Azure/azure-sdk-for-python/issues>`__
+        [Issues](https://github.com/Azure/azure-sdk-for-python/issues)
         section of the project.
         
         
-        .. image::  https://azure-sdk-impressions.azurewebsites.net/api/impressions/azure-sdk-for-python%2Fazure-batch%2FREADME.png
+        ![Impressions](https://azure-sdk-impressions.azurewebsites.net/api/impressions/azure-sdk-for-python%2Fazure-batch%2FREADME.png)
+        
+        
+        # Release History
         
+        ## 9.0.0 (2020-03-24)
         
-        .. :changelog:
+        ### Features
+        - Added ability to encrypt `ComputeNode` disk drives using the new `disk_encryption_configuration` property of `VirtualMachineConfiguration`.
+        - **[Breaking]** The `virtual_machine_id` property of `ImageReference` can now only refer to a Shared Image Gallery image.
+        - **[Breaking]** Pools can now be provisioned without a public IP using the new `public_ip_address_configuration` property of `NetworkConfiguration`.
+          - The `public_ips` property of `NetworkConfiguration` has moved in to `public_ip_address_configuration` as well. This property can only be specified if `ip_provisioning_type` is `UserManaged`.
         
-        Release History
-        ===============
+        ### REST API version
+        This version of the Batch .NET client library targets version 2020-03-01.11.0 of the Azure Batch REST API.
         
-        8.0.0 (2019-8-5)
-        ++++++++++++++++++
+        ## 8.0.0 (2019-8-5)
         
         - Using REST API version 2019-08-01.10.0.
             * Added ability to specify a collection of public IPs on `NetworkConfiguration` via the new `public_ips` property. This guarantees nodes in the Pool will have an IP from the list user provided IPs.
             * Added ability to mount remote file-systems on each node of a pool via the `mount_configuration` property on `CloudPool`.
             * Shared Image Gallery images can now be specified on the `virtual_machine_image_id` property of `ImageReference` by referencing the image via its ARM ID.
             * **Breaking** When not specified, the default value for `wait_for_success` on `StartTask` is now `True` (was `False`).
             * **Breaking** When not specified, the default value for `scope` on `AutoUserSpecification` is now always `Pool` (was `Task` on Windows nodes, `Pool` on Linux nodes).
         
-        7.0.0 (2019-6-11)
-        ++++++++++++++++++
+        ## 7.0.0 (2019-6-11)
         
         - Using REST API version 2019-06-01.9.0.
             * **Breaking** Replaced `AccountOperations.list_node_agent_skus` with `AccountOperations.list_supported_images`. `list_supported_images` contains all of the same information originally available in `list_node_agent_skus` but in a clearer format. New non-verified images are also now returned. Additional information about `capabilities` and `batch_support_end_of_life` is accessible on the `ImageInformation` object returned by `list_supported_images`.
             * Now support network security rules blocking network access to a `CloudPool` based on the source port of the traffic. This is done via the `source_port_ranges` property on `network_security_group_rules`.
             * When running a container, Batch now supports executing the task in the container working directory or in the Batch task working directory. This is controlled by the `working_directory` property on `TaskContainerSettings`.
         
-        6.0.1 (2019-2-26)
-        ++++++++++++++++++
+        ## 6.0.1 (2019-2-26)
         
         - Fix bug in TaskOperations.add_collection methods exception handling
         
-        6.0.0 (2018-12-14)
-        ++++++++++++++++++
+        ## 6.0.0 (2018-12-14)
         
         - Using REST API version 2018-12-01.8.0.
             * **Breaking** Removed support for the `upgrade_os` API on `CloudServiceConfiguration` pools.
                 - Removed `PoolOperations.upgrade_os` API.
                 - Renamed `target_os_version` to `os_version` and removed `current_os_version` on `CloudServiceConfiguration`.
                 - Removed `upgrading` state from `PoolState` enum.
             * **Breaking** Removed `data_egress_gi_b` and `data_ingress_gi_b` from `PoolUsageMetrics`. These properties are no longer supported.
@@ -104,36 +102,33 @@
             * Pools which set the `dynamic_vnet_assignment_scope` on `NetworkConfiguration` to be `DynamicVNetAssignmentScope.job` can now dynamically assign a Virtual Network to each node the job's tasks run on. The specific Virtual Network to join the nodes to is specified in the new `network_configuration` property on `CloudJob` and `JobSpecification`.
                 - Note: This feature is in public preview. It is disabled for all Batch accounts except for those which have contacted us and requested to be in the pilot.
             * The maximum lifetime of a task is now 180 days (previously it was 7).
             * Added support on Windows pools for creating users with a specific login mode (either `batch` or `interactive`) via `WindowsUserConfiguration.login_mode`.
             * The default task retention time for all tasks is now 7 days, previously it was infinite.
         - **Breaking** Renamed the `base_url` parameter to `batch_url` on `BatchServiceClient` class, and it is required now.
         
-        5.1.1 (2018-10-16)
-        ++++++++++++++++++
+        ## 5.1.1 (2018-10-16)
         
         **Bugfixes**
         
         - Fix authentication class to allow HTTP session to be re-used
         
         **Note**
         
         - azure-nspkg is not installed anymore on Python 3 (PEP420-based namespace package)
         
-        5.1.0 (2018-08-28)
-        ++++++++++++++++++
+        ## 5.1.0 (2018-08-28)
         
         - Update operation TaskOperations.add_collection with the following added functionality:
             + Retry server side errors.
             + Automatically chunk lists of more than 100 tasks to multiple requests.
             + If tasks are too large to be submitted in chunks of 100, reduces number of tasks per request.
             + Add a parameter to specify number of threads to use when submitting tasks.
         
-        5.0.0 (2018-08-24)
-        ++++++++++++++++++
+        ## 5.0.0 (2018-08-24)
         
         - Using REST API version 2018-08-01.7.0.
             + Added `node_agent_info` in ComputeNode to return the node agent information
             + **Breaking** Removed the `validation_status` property from `TaskCounts`.
             + **Breaking** The default caching type for `DataDisk` and `OSDisk` is now `read_write` instead of `none`.
         - `BatchServiceClient` can be used as a context manager to keep the underlying HTTP session open for performance.
         - **Breaking** Model signatures are now using only keywords-arguments syntax. Each positional argument must be rewritten as a keyword argument.
@@ -142,63 +137,56 @@
            + Operation TaskOperations.update
            + Operation ComputeNodeOperations.reimage
            + Operation ComputeNodeOperations.disable_scheduling
            + Operation ComputeNodeOperations.reboot
            + Operation JobOperations.terminate
         - Enum types now use the "str" mixin (class AzureEnum(str, Enum)) to improve the behavior when unrecognized enum values are encountered.
         
-        4.1.3 (2018-04-24)
-        ++++++++++++++++++
+        ## 4.1.3 (2018-04-24)
         
         - Update some APIs' comments
         - New property `leaving_pool` in `node_counts` type.
         
-        4.1.2 (2018-04-23)
-        ++++++++++++++++++
+        ## 4.1.2 (2018-04-23)
         
         **Bugfixes**
         
         - Compatibility of the sdist with wheel 0.31.0
         - Compatibility with msrestazure 0.4.28
         
-        4.1.1 (2018-03-26)
-        ++++++++++++++++++
+        ## 4.1.1 (2018-03-26)
         
         - Fix regression on method `enable_auto_scale`.
         
-        4.1.0 (2018-03-07)
-        ++++++++++++++++++
+        ## 4.1.0 (2018-03-07)
         
         - Using REST API version 2018-03-01.6.1.
         - Added the ability to query pool node counts by state, via the new `list_pool_node_counts` method.
         - Added the ability to upload Azure Batch node agent logs from a particular node, via the `upload_batch_service_logs` method.
            + This is intended for use in debugging by Microsoft support when there are problems on a node.
         
-        4.0.0 (2017-09-25)
-        ++++++++++++++++++
+        ## 4.0.0 (2017-09-25)
         
         - Using REST API version 2017-09-01.6.0.
         - Added the ability to get a discount on Windows VM pricing if you have on-premises licenses for the OS SKUs you are deploying, via `license_type` on `VirtualMachineConfiguration`.
         - Added support for attaching empty data drives to `VirtualMachineConfiguration` based pools, via the new `data_disks` attribute on `VirtualMachineConfiguration`.
         - **Breaking** Custom images must now be deployed using a reference to an ARM Image, instead of pointing to .vhd files in blobs directly.
             + The new `virtual_machine_image_id` property on `ImageReference` contains the reference to the ARM Image, and `OSDisk.image_uris` no longer exists.
             + Because of this, `image_reference` is now a required attribute of `VirtualMachineConfiguration`.
         - **Breaking** Multi-instance tasks (created using `MultiInstanceSettings`) must now specify a `coordination_commandLine`, and `number_of_instances` is now optional and defaults to 1.
         - Added support for tasks run using Docker containers. To run a task using a Docker container you must specify a `container_configuration` on the `VirtualMachineConfiguration` for a pool, and then add `container_settings` on the Task.
         
-        3.1.0 (2017-07-24)
-        ++++++++++++++++++
+        ## 3.1.0 (2017-07-24)
         
         - Added a new operation `job.get_task_counts` to retrieve the number of tasks in each state.
         - Added suuport for inbound endpoint configuration on a pool - there is a new `pool_endpoint_configuration` attribute on `NetworkConfiguration`.
           This property is only supported on pools that use `virtual_machine_configuration`.
         - A `ComputeNode` now also has an `endpoint_configuration` attribute with the details of the applied endpoint configuration for that node.
         
-        3.0.0 (2017-05-10)
-        ++++++++++++++++++
+        ## 3.0.0 (2017-05-10)
         
         - Added support for the new low-priority node type; `AddPoolParameter` and `PoolSpecification` now have an additional property `target_low_priority_nodes`.
         - `target_dedicated` and `current_dedicated` on `CloudPool`, `AddPoolParameter` and `PoolSpecification` have been renamed to `target_dedicated_nodes` and `current_dedicated_nodes`.
         - `resize_error` on `CloudPool` is now a collection called `resize_errors`.
         - Added a new `is_dedicated` property on `ComputeNode`, which is `false` for low-priority nodes.
         - Added a new `allow_low_priority_node` property to `JobManagerTask`, which if `true` allows the `JobManagerTask` to run on a low-priority compute node.
         - `PoolResizeParameter` now takes two optional parameters, `target_dedicated_nodes` and `target_low_priority_nodes`, instead of one required parameter `target_dedicated`.
@@ -213,21 +201,19 @@
         - Added support for provisioning application licenses to your pool, via a new `application_licenses` property on `PoolAddParameter`, `CloudPool` and `PoolSpecification`.
           Please note that this feature is in gated public preview, and you must request access to it via a support ticket.
         - The `ssh_private_key` attribute of a `UserAccount` object has been replaced with an expanded `LinuxUserConfiguration` object with additional settings for a user ID and group ID of the
           user account.
         - Removed `unmapped` enum state from `AddTaskStatus`, `CertificateFormat`, `CertificateVisibility`, `CertStoreLocation`, `ComputeNodeFillType`, `OSType`, and `PoolLifetimeOption` as they were not ever used.
         - Improved and clarified documentation.
         
-        2.0.1 (2017-04-19)
-        ++++++++++++++++++
+        ## 2.0.1 (2017-04-19)
         
         - This wheel package is now built with the azure wheel extension
         
-        2.0.0 (2017-02-23)
-        ++++++++++++++++++
+        ## 2.0.0 (2017-02-23)
         
         - AAD token authentication now supported.
         - Some operation names have changed (along with their associated parameter model classes):
             * pool.list_pool_usage_metrics -> pool.list_usage_metrics
             * pool.get_all_pools_lifetime_statistics -> pool.get_all_lifetime_statistics
             * job.get_all_jobs_lifetime_statistics -> job.get_all_lifetime_statistics
             * file.get_node_file_properties_from_task -> file.get_properties_from_task
@@ -235,37 +221,34 @@
         - The attribute 'file_name' in relation to file operations has been renamed to 'file_path'.
         - Change in naming convention for enum values to use underscores: e.g. StartTaskState.waitingforstarttask -> StartTaskState.waiting_for_start_task.
         - Support for running tasks under a predefined or automatic user account. This includes tasks, job manager tasks, job preparation and release tasks and pool start tasks. This feature replaces the previous 'run_elevated' option on a task.
         - Tasks now have an optional scoped authentication token (only applies to tasks and job manager tasks).
         - Support for creating pools with a list of user accounts.
         - Support for creating pools using a custom VM image (only supported on accounts created with a "User Subscription" pool allocation mode).
         
-        1.1.0 (2016-09-15)
-        ++++++++++++++++++
+        ## 1.1.0 (2016-09-15)
         
         - Added support for task reactivation
         
-        1.0.0 (2016-08-09)
-        ++++++++++++++++++
+        ## 1.0.0 (2016-08-09)
         
         - Added support for joining a CloudPool to a virtual network on using the network_configuration property.
         - Added support for application package references on CloudTask and JobManagerTask.
         - Added support for automatically terminating jobs when all tasks complete or when a task fails, via the on_all_tasks_complete property and
           the CloudTask exit_conditions property.
         
-        0.30.0rc5
-        +++++++++
+        ## 0.30.0rc5
         
         - Initial Release
         
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
-Description-Content-Type: text/x-rst
+Description-Content-Type: text/markdown
```

## Comparing `azure-batch-8.0.0/README.rst` & `azure-batch-9.0.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,42 @@
-Microsoft Azure SDK for Python
-==============================
+# Microsoft Azure SDK for Python
 
 This is the Microsoft Azure Batch Client Library.
 
 This package has been tested with Python 2.7, 3.4, 3.5, 3.6 and 3.7.
 
-For a more complete set of Azure libraries, see the `azure <https://pypi.python.org/pypi/azure>`__ bundle package.
+For a more complete set of Azure libraries, see the [azure](https://pypi.python.org/pypi/azure) bundle package.
 
 
-Compatibility
-=============
+# Compatibility
 
 **IMPORTANT**: If you have an earlier version of the azure package
 (version < 1.0), you should uninstall it before installing this package.
 
 You can check the version using pip:
 
-.. code:: shell
-
-    pip freeze
+```shell
+pip freeze
+```
 
 If you see azure==0.11.0 (or any version below 1.0), uninstall it first:
 
-.. code:: shell
-
-    pip uninstall azure
+```shell
+pip uninstall azure
+```
 
 
-Usage
-=====
+# Usage
 
-For code examples, see `the Batch samples repo
-<https://github.com/Azure/azure-batch-samples/tree/master/Python>`__
-on GitHub or see `Batch
-<https://docs.microsoft.com/python/api/overview/azure/batch>`__
+For code examples, see [the Batch samples repo](https://github.com/Azure/azure-batch-samples/tree/master/Python)
+on GitHub or see [Batch](https://docs.microsoft.com/python/api/overview/azure/batch)
 on docs.microsoft.com.
 
 
-Provide Feedback
-================
+# Provide Feedback
 
 If you encounter any bugs or have suggestions, please file an issue in the
-`Issues <https://github.com/Azure/azure-sdk-for-python/issues>`__
+[Issues](https://github.com/Azure/azure-sdk-for-python/issues)
 section of the project.
 
 
-.. image::  https://azure-sdk-impressions.azurewebsites.net/api/impressions/azure-sdk-for-python%2Fazure-batch%2FREADME.png
+![Impressions](https://azure-sdk-impressions.azurewebsites.net/api/impressions/azure-sdk-for-python%2Fazure-batch%2FREADME.png)
```

## Comparing `azure-batch-8.0.0/HISTORY.rst` & `azure-batch-9.0.0/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,41 @@
-.. :changelog:
+# Release History
 
-Release History
-===============
+## 9.0.0 (2020-03-24)
 
-8.0.0 (2019-8-5)
-++++++++++++++++++
+### Features
+- Added ability to encrypt `ComputeNode` disk drives using the new `disk_encryption_configuration` property of `VirtualMachineConfiguration`.
+- **[Breaking]** The `virtual_machine_id` property of `ImageReference` can now only refer to a Shared Image Gallery image.
+- **[Breaking]** Pools can now be provisioned without a public IP using the new `public_ip_address_configuration` property of `NetworkConfiguration`.
+  - The `public_ips` property of `NetworkConfiguration` has moved in to `public_ip_address_configuration` as well. This property can only be specified if `ip_provisioning_type` is `UserManaged`.
+
+### REST API version
+This version of the Batch .NET client library targets version 2020-03-01.11.0 of the Azure Batch REST API.
+
+## 8.0.0 (2019-8-5)
 
 - Using REST API version 2019-08-01.10.0.
     * Added ability to specify a collection of public IPs on `NetworkConfiguration` via the new `public_ips` property. This guarantees nodes in the Pool will have an IP from the list user provided IPs.
     * Added ability to mount remote file-systems on each node of a pool via the `mount_configuration` property on `CloudPool`.
     * Shared Image Gallery images can now be specified on the `virtual_machine_image_id` property of `ImageReference` by referencing the image via its ARM ID.
     * **Breaking** When not specified, the default value for `wait_for_success` on `StartTask` is now `True` (was `False`).
     * **Breaking** When not specified, the default value for `scope` on `AutoUserSpecification` is now always `Pool` (was `Task` on Windows nodes, `Pool` on Linux nodes).
 
-7.0.0 (2019-6-11)
-++++++++++++++++++
+## 7.0.0 (2019-6-11)
 
 - Using REST API version 2019-06-01.9.0.
     * **Breaking** Replaced `AccountOperations.list_node_agent_skus` with `AccountOperations.list_supported_images`. `list_supported_images` contains all of the same information originally available in `list_node_agent_skus` but in a clearer format. New non-verified images are also now returned. Additional information about `capabilities` and `batch_support_end_of_life` is accessible on the `ImageInformation` object returned by `list_supported_images`.
     * Now support network security rules blocking network access to a `CloudPool` based on the source port of the traffic. This is done via the `source_port_ranges` property on `network_security_group_rules`.
     * When running a container, Batch now supports executing the task in the container working directory or in the Batch task working directory. This is controlled by the `working_directory` property on `TaskContainerSettings`.
 
-6.0.1 (2019-2-26)
-++++++++++++++++++
+## 6.0.1 (2019-2-26)
 
 - Fix bug in TaskOperations.add_collection methods exception handling
 
-6.0.0 (2018-12-14)
-++++++++++++++++++
+## 6.0.0 (2018-12-14)
 
 - Using REST API version 2018-12-01.8.0.
     * **Breaking** Removed support for the `upgrade_os` API on `CloudServiceConfiguration` pools.
         - Removed `PoolOperations.upgrade_os` API.
         - Renamed `target_os_version` to `os_version` and removed `current_os_version` on `CloudServiceConfiguration`.
         - Removed `upgrading` state from `PoolState` enum.
     * **Breaking** Removed `data_egress_gi_b` and `data_ingress_gi_b` from `PoolUsageMetrics`. These properties are no longer supported.
@@ -46,36 +50,33 @@
     * Pools which set the `dynamic_vnet_assignment_scope` on `NetworkConfiguration` to be `DynamicVNetAssignmentScope.job` can now dynamically assign a Virtual Network to each node the job's tasks run on. The specific Virtual Network to join the nodes to is specified in the new `network_configuration` property on `CloudJob` and `JobSpecification`.
         - Note: This feature is in public preview. It is disabled for all Batch accounts except for those which have contacted us and requested to be in the pilot.
     * The maximum lifetime of a task is now 180 days (previously it was 7).
     * Added support on Windows pools for creating users with a specific login mode (either `batch` or `interactive`) via `WindowsUserConfiguration.login_mode`.
     * The default task retention time for all tasks is now 7 days, previously it was infinite.
 - **Breaking** Renamed the `base_url` parameter to `batch_url` on `BatchServiceClient` class, and it is required now.
 
-5.1.1 (2018-10-16)
-++++++++++++++++++
+## 5.1.1 (2018-10-16)
 
 **Bugfixes**
 
 - Fix authentication class to allow HTTP session to be re-used
 
 **Note**
 
 - azure-nspkg is not installed anymore on Python 3 (PEP420-based namespace package)
 
-5.1.0 (2018-08-28)
-++++++++++++++++++
+## 5.1.0 (2018-08-28)
 
 - Update operation TaskOperations.add_collection with the following added functionality:
     + Retry server side errors.
     + Automatically chunk lists of more than 100 tasks to multiple requests.
     + If tasks are too large to be submitted in chunks of 100, reduces number of tasks per request.
     + Add a parameter to specify number of threads to use when submitting tasks.
 
-5.0.0 (2018-08-24)
-++++++++++++++++++
+## 5.0.0 (2018-08-24)
 
 - Using REST API version 2018-08-01.7.0.
     + Added `node_agent_info` in ComputeNode to return the node agent information
     + **Breaking** Removed the `validation_status` property from `TaskCounts`.
     + **Breaking** The default caching type for `DataDisk` and `OSDisk` is now `read_write` instead of `none`.
 - `BatchServiceClient` can be used as a context manager to keep the underlying HTTP session open for performance.
 - **Breaking** Model signatures are now using only keywords-arguments syntax. Each positional argument must be rewritten as a keyword argument.
@@ -84,63 +85,56 @@
    + Operation TaskOperations.update
    + Operation ComputeNodeOperations.reimage
    + Operation ComputeNodeOperations.disable_scheduling
    + Operation ComputeNodeOperations.reboot
    + Operation JobOperations.terminate
 - Enum types now use the "str" mixin (class AzureEnum(str, Enum)) to improve the behavior when unrecognized enum values are encountered.
 
-4.1.3 (2018-04-24)
-++++++++++++++++++
+## 4.1.3 (2018-04-24)
 
 - Update some APIs' comments
 - New property `leaving_pool` in `node_counts` type.
 
-4.1.2 (2018-04-23)
-++++++++++++++++++
+## 4.1.2 (2018-04-23)
 
 **Bugfixes**
 
 - Compatibility of the sdist with wheel 0.31.0
 - Compatibility with msrestazure 0.4.28
 
-4.1.1 (2018-03-26)
-++++++++++++++++++
+## 4.1.1 (2018-03-26)
 
 - Fix regression on method `enable_auto_scale`.
 
-4.1.0 (2018-03-07)
-++++++++++++++++++
+## 4.1.0 (2018-03-07)
 
 - Using REST API version 2018-03-01.6.1.
 - Added the ability to query pool node counts by state, via the new `list_pool_node_counts` method.
 - Added the ability to upload Azure Batch node agent logs from a particular node, via the `upload_batch_service_logs` method.
    + This is intended for use in debugging by Microsoft support when there are problems on a node.
 
-4.0.0 (2017-09-25)
-++++++++++++++++++
+## 4.0.0 (2017-09-25)
 
 - Using REST API version 2017-09-01.6.0.
 - Added the ability to get a discount on Windows VM pricing if you have on-premises licenses for the OS SKUs you are deploying, via `license_type` on `VirtualMachineConfiguration`.
 - Added support for attaching empty data drives to `VirtualMachineConfiguration` based pools, via the new `data_disks` attribute on `VirtualMachineConfiguration`.
 - **Breaking** Custom images must now be deployed using a reference to an ARM Image, instead of pointing to .vhd files in blobs directly.
     + The new `virtual_machine_image_id` property on `ImageReference` contains the reference to the ARM Image, and `OSDisk.image_uris` no longer exists.
     + Because of this, `image_reference` is now a required attribute of `VirtualMachineConfiguration`.
 - **Breaking** Multi-instance tasks (created using `MultiInstanceSettings`) must now specify a `coordination_commandLine`, and `number_of_instances` is now optional and defaults to 1.
 - Added support for tasks run using Docker containers. To run a task using a Docker container you must specify a `container_configuration` on the `VirtualMachineConfiguration` for a pool, and then add `container_settings` on the Task.
 
-3.1.0 (2017-07-24)
-++++++++++++++++++
+## 3.1.0 (2017-07-24)
 
 - Added a new operation `job.get_task_counts` to retrieve the number of tasks in each state.
 - Added suuport for inbound endpoint configuration on a pool - there is a new `pool_endpoint_configuration` attribute on `NetworkConfiguration`.
   This property is only supported on pools that use `virtual_machine_configuration`.
 - A `ComputeNode` now also has an `endpoint_configuration` attribute with the details of the applied endpoint configuration for that node.
 
-3.0.0 (2017-05-10)
-++++++++++++++++++
+## 3.0.0 (2017-05-10)
 
 - Added support for the new low-priority node type; `AddPoolParameter` and `PoolSpecification` now have an additional property `target_low_priority_nodes`.
 - `target_dedicated` and `current_dedicated` on `CloudPool`, `AddPoolParameter` and `PoolSpecification` have been renamed to `target_dedicated_nodes` and `current_dedicated_nodes`.
 - `resize_error` on `CloudPool` is now a collection called `resize_errors`.
 - Added a new `is_dedicated` property on `ComputeNode`, which is `false` for low-priority nodes.
 - Added a new `allow_low_priority_node` property to `JobManagerTask`, which if `true` allows the `JobManagerTask` to run on a low-priority compute node.
 - `PoolResizeParameter` now takes two optional parameters, `target_dedicated_nodes` and `target_low_priority_nodes`, instead of one required parameter `target_dedicated`.
@@ -155,21 +149,19 @@
 - Added support for provisioning application licenses to your pool, via a new `application_licenses` property on `PoolAddParameter`, `CloudPool` and `PoolSpecification`.
   Please note that this feature is in gated public preview, and you must request access to it via a support ticket.
 - The `ssh_private_key` attribute of a `UserAccount` object has been replaced with an expanded `LinuxUserConfiguration` object with additional settings for a user ID and group ID of the
   user account.
 - Removed `unmapped` enum state from `AddTaskStatus`, `CertificateFormat`, `CertificateVisibility`, `CertStoreLocation`, `ComputeNodeFillType`, `OSType`, and `PoolLifetimeOption` as they were not ever used.
 - Improved and clarified documentation.
 
-2.0.1 (2017-04-19)
-++++++++++++++++++
+## 2.0.1 (2017-04-19)
 
 - This wheel package is now built with the azure wheel extension
 
-2.0.0 (2017-02-23)
-++++++++++++++++++
+## 2.0.0 (2017-02-23)
 
 - AAD token authentication now supported.
 - Some operation names have changed (along with their associated parameter model classes):
     * pool.list_pool_usage_metrics -> pool.list_usage_metrics
     * pool.get_all_pools_lifetime_statistics -> pool.get_all_lifetime_statistics
     * job.get_all_jobs_lifetime_statistics -> job.get_all_lifetime_statistics
     * file.get_node_file_properties_from_task -> file.get_properties_from_task
@@ -177,24 +169,21 @@
 - The attribute 'file_name' in relation to file operations has been renamed to 'file_path'.
 - Change in naming convention for enum values to use underscores: e.g. StartTaskState.waitingforstarttask -> StartTaskState.waiting_for_start_task.
 - Support for running tasks under a predefined or automatic user account. This includes tasks, job manager tasks, job preparation and release tasks and pool start tasks. This feature replaces the previous 'run_elevated' option on a task.
 - Tasks now have an optional scoped authentication token (only applies to tasks and job manager tasks).
 - Support for creating pools with a list of user accounts.
 - Support for creating pools using a custom VM image (only supported on accounts created with a "User Subscription" pool allocation mode).
 
-1.1.0 (2016-09-15)
-++++++++++++++++++
+## 1.1.0 (2016-09-15)
 
 - Added support for task reactivation
 
-1.0.0 (2016-08-09)
-++++++++++++++++++
+## 1.0.0 (2016-08-09)
 
 - Added support for joining a CloudPool to a virtual network on using the network_configuration property.
 - Added support for application package references on CloudTask and JobManagerTask.
 - Added support for automatically terminating jobs when all tasks complete or when a task fails, via the on_all_tasks_complete property and
   the CloudTask exit_conditions property.
 
-0.30.0rc5
-+++++++++
+## 0.30.0rc5
 
 - Initial Release
```

## Comparing `azure-batch-8.0.0/setup.py` & `azure-batch-9.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,32 +32,32 @@
         )
     except AttributeError:
         pass
 except ImportError:
     pass
 
 # Version extraction inspired from 'requests'
-with open(os.path.join(package_folder_path, 'version.py'), 'r') as fd:
+with open(os.path.join(package_folder_path, '_version.py'), 'r') as fd:
     version = re.search(r'^VERSION\s*=\s*[\'"]([^\'"]*)[\'"]',
                         fd.read(), re.MULTILINE).group(1)
 
 if not version:
     raise RuntimeError('Cannot find version information')
 
-with open('README.rst', encoding='utf-8') as f:
+with open('README.md', encoding='utf-8') as f:
     readme = f.read()
-with open('HISTORY.rst', encoding='utf-8') as f:
-    history = f.read()
+with open('CHANGELOG.md', encoding='utf-8') as f:
+    changelog = f.read()
 
 setup(
     name=PACKAGE_NAME,
     version=version,
     description='Microsoft Azure {} Client Library for Python'.format(PACKAGE_PPRINT_NAME),
-    long_description=readme + '\n\n' + history,
-    long_description_content_type='text/x-rst',
+    long_description=readme + '\n\n' + changelog,
+    long_description_content_type='text/markdown',
     license='MIT License',
     author='Microsoft Corporation',
     author_email='azpysdkhelp@microsoft.com',
     url='https://github.com/Azure/azure-sdk-for-python',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Programming Language :: Python',
```

## Comparing `azure-batch-8.0.0/azure_batch.egg-info/PKG-INFO` & `azure-batch-9.0.0/azure_batch.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,95 +1,93 @@
 Metadata-Version: 2.1
 Name: azure-batch
-Version: 8.0.0
+Version: 9.0.0
 Summary: Microsoft Azure Batch Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
-Description: Microsoft Azure SDK for Python
-        ==============================
+Description: # Microsoft Azure SDK for Python
         
         This is the Microsoft Azure Batch Client Library.
         
         This package has been tested with Python 2.7, 3.4, 3.5, 3.6 and 3.7.
         
-        For a more complete set of Azure libraries, see the `azure <https://pypi.python.org/pypi/azure>`__ bundle package.
+        For a more complete set of Azure libraries, see the [azure](https://pypi.python.org/pypi/azure) bundle package.
         
         
-        Compatibility
-        =============
+        # Compatibility
         
         **IMPORTANT**: If you have an earlier version of the azure package
         (version < 1.0), you should uninstall it before installing this package.
         
         You can check the version using pip:
         
-        .. code:: shell
-        
-            pip freeze
+        ```shell
+        pip freeze
+        ```
         
         If you see azure==0.11.0 (or any version below 1.0), uninstall it first:
         
-        .. code:: shell
-        
-            pip uninstall azure
+        ```shell
+        pip uninstall azure
+        ```
         
         
-        Usage
-        =====
+        # Usage
         
-        For code examples, see `the Batch samples repo
-        <https://github.com/Azure/azure-batch-samples/tree/master/Python>`__
-        on GitHub or see `Batch
-        <https://docs.microsoft.com/python/api/overview/azure/batch>`__
+        For code examples, see [the Batch samples repo](https://github.com/Azure/azure-batch-samples/tree/master/Python)
+        on GitHub or see [Batch](https://docs.microsoft.com/python/api/overview/azure/batch)
         on docs.microsoft.com.
         
         
-        Provide Feedback
-        ================
+        # Provide Feedback
         
         If you encounter any bugs or have suggestions, please file an issue in the
-        `Issues <https://github.com/Azure/azure-sdk-for-python/issues>`__
+        [Issues](https://github.com/Azure/azure-sdk-for-python/issues)
         section of the project.
         
         
-        .. image::  https://azure-sdk-impressions.azurewebsites.net/api/impressions/azure-sdk-for-python%2Fazure-batch%2FREADME.png
+        ![Impressions](https://azure-sdk-impressions.azurewebsites.net/api/impressions/azure-sdk-for-python%2Fazure-batch%2FREADME.png)
+        
+        
+        # Release History
         
+        ## 9.0.0 (2020-03-24)
         
-        .. :changelog:
+        ### Features
+        - Added ability to encrypt `ComputeNode` disk drives using the new `disk_encryption_configuration` property of `VirtualMachineConfiguration`.
+        - **[Breaking]** The `virtual_machine_id` property of `ImageReference` can now only refer to a Shared Image Gallery image.
+        - **[Breaking]** Pools can now be provisioned without a public IP using the new `public_ip_address_configuration` property of `NetworkConfiguration`.
+          - The `public_ips` property of `NetworkConfiguration` has moved in to `public_ip_address_configuration` as well. This property can only be specified if `ip_provisioning_type` is `UserManaged`.
         
-        Release History
-        ===============
+        ### REST API version
+        This version of the Batch .NET client library targets version 2020-03-01.11.0 of the Azure Batch REST API.
         
-        8.0.0 (2019-8-5)
-        ++++++++++++++++++
+        ## 8.0.0 (2019-8-5)
         
         - Using REST API version 2019-08-01.10.0.
             * Added ability to specify a collection of public IPs on `NetworkConfiguration` via the new `public_ips` property. This guarantees nodes in the Pool will have an IP from the list user provided IPs.
             * Added ability to mount remote file-systems on each node of a pool via the `mount_configuration` property on `CloudPool`.
             * Shared Image Gallery images can now be specified on the `virtual_machine_image_id` property of `ImageReference` by referencing the image via its ARM ID.
             * **Breaking** When not specified, the default value for `wait_for_success` on `StartTask` is now `True` (was `False`).
             * **Breaking** When not specified, the default value for `scope` on `AutoUserSpecification` is now always `Pool` (was `Task` on Windows nodes, `Pool` on Linux nodes).
         
-        7.0.0 (2019-6-11)
-        ++++++++++++++++++
+        ## 7.0.0 (2019-6-11)
         
         - Using REST API version 2019-06-01.9.0.
             * **Breaking** Replaced `AccountOperations.list_node_agent_skus` with `AccountOperations.list_supported_images`. `list_supported_images` contains all of the same information originally available in `list_node_agent_skus` but in a clearer format. New non-verified images are also now returned. Additional information about `capabilities` and `batch_support_end_of_life` is accessible on the `ImageInformation` object returned by `list_supported_images`.
             * Now support network security rules blocking network access to a `CloudPool` based on the source port of the traffic. This is done via the `source_port_ranges` property on `network_security_group_rules`.
             * When running a container, Batch now supports executing the task in the container working directory or in the Batch task working directory. This is controlled by the `working_directory` property on `TaskContainerSettings`.
         
-        6.0.1 (2019-2-26)
-        ++++++++++++++++++
+        ## 6.0.1 (2019-2-26)
         
         - Fix bug in TaskOperations.add_collection methods exception handling
         
-        6.0.0 (2018-12-14)
-        ++++++++++++++++++
+        ## 6.0.0 (2018-12-14)
         
         - Using REST API version 2018-12-01.8.0.
             * **Breaking** Removed support for the `upgrade_os` API on `CloudServiceConfiguration` pools.
                 - Removed `PoolOperations.upgrade_os` API.
                 - Renamed `target_os_version` to `os_version` and removed `current_os_version` on `CloudServiceConfiguration`.
                 - Removed `upgrading` state from `PoolState` enum.
             * **Breaking** Removed `data_egress_gi_b` and `data_ingress_gi_b` from `PoolUsageMetrics`. These properties are no longer supported.
@@ -104,36 +102,33 @@
             * Pools which set the `dynamic_vnet_assignment_scope` on `NetworkConfiguration` to be `DynamicVNetAssignmentScope.job` can now dynamically assign a Virtual Network to each node the job's tasks run on. The specific Virtual Network to join the nodes to is specified in the new `network_configuration` property on `CloudJob` and `JobSpecification`.
                 - Note: This feature is in public preview. It is disabled for all Batch accounts except for those which have contacted us and requested to be in the pilot.
             * The maximum lifetime of a task is now 180 days (previously it was 7).
             * Added support on Windows pools for creating users with a specific login mode (either `batch` or `interactive`) via `WindowsUserConfiguration.login_mode`.
             * The default task retention time for all tasks is now 7 days, previously it was infinite.
         - **Breaking** Renamed the `base_url` parameter to `batch_url` on `BatchServiceClient` class, and it is required now.
         
-        5.1.1 (2018-10-16)
-        ++++++++++++++++++
+        ## 5.1.1 (2018-10-16)
         
         **Bugfixes**
         
         - Fix authentication class to allow HTTP session to be re-used
         
         **Note**
         
         - azure-nspkg is not installed anymore on Python 3 (PEP420-based namespace package)
         
-        5.1.0 (2018-08-28)
-        ++++++++++++++++++
+        ## 5.1.0 (2018-08-28)
         
         - Update operation TaskOperations.add_collection with the following added functionality:
             + Retry server side errors.
             + Automatically chunk lists of more than 100 tasks to multiple requests.
             + If tasks are too large to be submitted in chunks of 100, reduces number of tasks per request.
             + Add a parameter to specify number of threads to use when submitting tasks.
         
-        5.0.0 (2018-08-24)
-        ++++++++++++++++++
+        ## 5.0.0 (2018-08-24)
         
         - Using REST API version 2018-08-01.7.0.
             + Added `node_agent_info` in ComputeNode to return the node agent information
             + **Breaking** Removed the `validation_status` property from `TaskCounts`.
             + **Breaking** The default caching type for `DataDisk` and `OSDisk` is now `read_write` instead of `none`.
         - `BatchServiceClient` can be used as a context manager to keep the underlying HTTP session open for performance.
         - **Breaking** Model signatures are now using only keywords-arguments syntax. Each positional argument must be rewritten as a keyword argument.
@@ -142,63 +137,56 @@
            + Operation TaskOperations.update
            + Operation ComputeNodeOperations.reimage
            + Operation ComputeNodeOperations.disable_scheduling
            + Operation ComputeNodeOperations.reboot
            + Operation JobOperations.terminate
         - Enum types now use the "str" mixin (class AzureEnum(str, Enum)) to improve the behavior when unrecognized enum values are encountered.
         
-        4.1.3 (2018-04-24)
-        ++++++++++++++++++
+        ## 4.1.3 (2018-04-24)
         
         - Update some APIs' comments
         - New property `leaving_pool` in `node_counts` type.
         
-        4.1.2 (2018-04-23)
-        ++++++++++++++++++
+        ## 4.1.2 (2018-04-23)
         
         **Bugfixes**
         
         - Compatibility of the sdist with wheel 0.31.0
         - Compatibility with msrestazure 0.4.28
         
-        4.1.1 (2018-03-26)
-        ++++++++++++++++++
+        ## 4.1.1 (2018-03-26)
         
         - Fix regression on method `enable_auto_scale`.
         
-        4.1.0 (2018-03-07)
-        ++++++++++++++++++
+        ## 4.1.0 (2018-03-07)
         
         - Using REST API version 2018-03-01.6.1.
         - Added the ability to query pool node counts by state, via the new `list_pool_node_counts` method.
         - Added the ability to upload Azure Batch node agent logs from a particular node, via the `upload_batch_service_logs` method.
            + This is intended for use in debugging by Microsoft support when there are problems on a node.
         
-        4.0.0 (2017-09-25)
-        ++++++++++++++++++
+        ## 4.0.0 (2017-09-25)
         
         - Using REST API version 2017-09-01.6.0.
         - Added the ability to get a discount on Windows VM pricing if you have on-premises licenses for the OS SKUs you are deploying, via `license_type` on `VirtualMachineConfiguration`.
         - Added support for attaching empty data drives to `VirtualMachineConfiguration` based pools, via the new `data_disks` attribute on `VirtualMachineConfiguration`.
         - **Breaking** Custom images must now be deployed using a reference to an ARM Image, instead of pointing to .vhd files in blobs directly.
             + The new `virtual_machine_image_id` property on `ImageReference` contains the reference to the ARM Image, and `OSDisk.image_uris` no longer exists.
             + Because of this, `image_reference` is now a required attribute of `VirtualMachineConfiguration`.
         - **Breaking** Multi-instance tasks (created using `MultiInstanceSettings`) must now specify a `coordination_commandLine`, and `number_of_instances` is now optional and defaults to 1.
         - Added support for tasks run using Docker containers. To run a task using a Docker container you must specify a `container_configuration` on the `VirtualMachineConfiguration` for a pool, and then add `container_settings` on the Task.
         
-        3.1.0 (2017-07-24)
-        ++++++++++++++++++
+        ## 3.1.0 (2017-07-24)
         
         - Added a new operation `job.get_task_counts` to retrieve the number of tasks in each state.
         - Added suuport for inbound endpoint configuration on a pool - there is a new `pool_endpoint_configuration` attribute on `NetworkConfiguration`.
           This property is only supported on pools that use `virtual_machine_configuration`.
         - A `ComputeNode` now also has an `endpoint_configuration` attribute with the details of the applied endpoint configuration for that node.
         
-        3.0.0 (2017-05-10)
-        ++++++++++++++++++
+        ## 3.0.0 (2017-05-10)
         
         - Added support for the new low-priority node type; `AddPoolParameter` and `PoolSpecification` now have an additional property `target_low_priority_nodes`.
         - `target_dedicated` and `current_dedicated` on `CloudPool`, `AddPoolParameter` and `PoolSpecification` have been renamed to `target_dedicated_nodes` and `current_dedicated_nodes`.
         - `resize_error` on `CloudPool` is now a collection called `resize_errors`.
         - Added a new `is_dedicated` property on `ComputeNode`, which is `false` for low-priority nodes.
         - Added a new `allow_low_priority_node` property to `JobManagerTask`, which if `true` allows the `JobManagerTask` to run on a low-priority compute node.
         - `PoolResizeParameter` now takes two optional parameters, `target_dedicated_nodes` and `target_low_priority_nodes`, instead of one required parameter `target_dedicated`.
@@ -213,21 +201,19 @@
         - Added support for provisioning application licenses to your pool, via a new `application_licenses` property on `PoolAddParameter`, `CloudPool` and `PoolSpecification`.
           Please note that this feature is in gated public preview, and you must request access to it via a support ticket.
         - The `ssh_private_key` attribute of a `UserAccount` object has been replaced with an expanded `LinuxUserConfiguration` object with additional settings for a user ID and group ID of the
           user account.
         - Removed `unmapped` enum state from `AddTaskStatus`, `CertificateFormat`, `CertificateVisibility`, `CertStoreLocation`, `ComputeNodeFillType`, `OSType`, and `PoolLifetimeOption` as they were not ever used.
         - Improved and clarified documentation.
         
-        2.0.1 (2017-04-19)
-        ++++++++++++++++++
+        ## 2.0.1 (2017-04-19)
         
         - This wheel package is now built with the azure wheel extension
         
-        2.0.0 (2017-02-23)
-        ++++++++++++++++++
+        ## 2.0.0 (2017-02-23)
         
         - AAD token authentication now supported.
         - Some operation names have changed (along with their associated parameter model classes):
             * pool.list_pool_usage_metrics -> pool.list_usage_metrics
             * pool.get_all_pools_lifetime_statistics -> pool.get_all_lifetime_statistics
             * job.get_all_jobs_lifetime_statistics -> job.get_all_lifetime_statistics
             * file.get_node_file_properties_from_task -> file.get_properties_from_task
@@ -235,37 +221,34 @@
         - The attribute 'file_name' in relation to file operations has been renamed to 'file_path'.
         - Change in naming convention for enum values to use underscores: e.g. StartTaskState.waitingforstarttask -> StartTaskState.waiting_for_start_task.
         - Support for running tasks under a predefined or automatic user account. This includes tasks, job manager tasks, job preparation and release tasks and pool start tasks. This feature replaces the previous 'run_elevated' option on a task.
         - Tasks now have an optional scoped authentication token (only applies to tasks and job manager tasks).
         - Support for creating pools with a list of user accounts.
         - Support for creating pools using a custom VM image (only supported on accounts created with a "User Subscription" pool allocation mode).
         
-        1.1.0 (2016-09-15)
-        ++++++++++++++++++
+        ## 1.1.0 (2016-09-15)
         
         - Added support for task reactivation
         
-        1.0.0 (2016-08-09)
-        ++++++++++++++++++
+        ## 1.0.0 (2016-08-09)
         
         - Added support for joining a CloudPool to a virtual network on using the network_configuration property.
         - Added support for application package references on CloudTask and JobManagerTask.
         - Added support for automatically terminating jobs when all tasks complete or when a task fails, via the on_all_tasks_complete property and
           the CloudTask exit_conditions property.
         
-        0.30.0rc5
-        +++++++++
+        ## 0.30.0rc5
         
         - Initial Release
         
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
-Description-Content-Type: text/x-rst
+Description-Content-Type: text/markdown
```

## Comparing `azure-batch-8.0.0/azure_batch.egg-info/SOURCES.txt` & `azure-batch-9.0.0/azure_batch.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-HISTORY.rst
+CHANGELOG.md
 MANIFEST.in
-README.rst
+README.md
 setup.cfg
 setup.py
 azure/__init__.py
 azure/batch/__init__.py
 azure/batch/_batch_service_client.py
 azure/batch/_configuration.py
+azure/batch/_version.py
 azure/batch/batch_auth.py
-azure/batch/version.py
 azure/batch/custom/__init__.py
 azure/batch/custom/custom_errors.py
 azure/batch/custom/patch.py
 azure/batch/models/__init__.py
 azure/batch/models/_batch_service_client_enums.py
 azure/batch/models/_models.py
 azure/batch/models/_models_py3.py
@@ -28,8 +28,10 @@
 azure/batch/operations/_pool_operations.py
 azure/batch/operations/_task_operations.py
 azure_batch.egg-info/PKG-INFO
 azure_batch.egg-info/SOURCES.txt
 azure_batch.egg-info/dependency_links.txt
 azure_batch.egg-info/not-zip-safe
 azure_batch.egg-info/requires.txt
-azure_batch.egg-info/top_level.txt
+azure_batch.egg-info/top_level.txt
+tests/batch_preparers.py
+tests/test_batch.py
```

## Comparing `azure-batch-8.0.0/azure/batch/__init__.py` & `azure-batch-9.0.0/azure/batch/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,11 +9,11 @@
 # regenerated.
 # --------------------------------------------------------------------------
 
 from ._configuration import BatchServiceClientConfiguration
 from ._batch_service_client import BatchServiceClient
 __all__ = ['BatchServiceClient', 'BatchServiceClientConfiguration']
 
-from .version import VERSION
+from ._version import VERSION
 
 __version__ = VERSION
```

## Comparing `azure-batch-8.0.0/azure/batch/_configuration.py` & `azure-batch-9.0.0/azure/batch/_configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is
 # regenerated.
 # --------------------------------------------------------------------------
 from msrestazure import AzureConfiguration
 
-from .version import VERSION
+from ._version import VERSION
 
 
 class BatchServiceClientConfiguration(AzureConfiguration):
     """Configuration for BatchServiceClient
     Note that all parameters used to create this instance are saved as instance
     attributes.
```

## Comparing `azure-batch-8.0.0/azure/batch/batch_auth.py` & `azure-batch-9.0.0/azure/batch/batch_auth.py`

 * *Files identical despite different names*

## Comparing `azure-batch-8.0.0/azure/batch/_batch_service_client.py` & `azure-batch-9.0.0/azure/batch/_batch_service_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 from .operations import FileOperations
 from .operations import JobScheduleOperations
 from .operations import TaskOperations
 from .operations import ComputeNodeOperations
 from . import models
 from .custom.patch import patch_client
 
-
 class BatchServiceClient(SDKClient):
     """A client for issuing REST requests to the Azure Batch service.
 
     :ivar config: Configuration for client.
     :vartype config: BatchServiceClientConfiguration
 
     :ivar application: Application operations
@@ -61,15 +60,15 @@
     def __init__(
             self, credentials, batch_url):
 
         self.config = BatchServiceClientConfiguration(credentials, batch_url)
         super(BatchServiceClient, self).__init__(self.config.credentials, self.config)
 
         client_models = {k: v for k, v in models.__dict__.items() if isinstance(v, type)}
-        self.api_version = '2019-08-01.10.0'
+        self.api_version = '2020-03-01.11.0'
         self._serialize = Serializer(client_models)
         self._deserialize = Deserializer(client_models)
 
         self.application = ApplicationOperations(
             self._client, self.config, self._serialize, self._deserialize)
         self.pool = PoolOperations(
             self._client, self.config, self._serialize, self._deserialize)
```

## Comparing `azure-batch-8.0.0/azure/batch/models/_models.py` & `azure-batch-9.0.0/azure/batch/models/_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -693,16 +693,15 @@
     :param data: Required. The base64-encoded contents of the Certificate. The
      maximum size is 10KB.
     :type data: str
     :param certificate_format: The format of the Certificate data. Possible
      values include: 'pfx', 'cer'
     :type certificate_format: str or ~azure.batch.models.CertificateFormat
     :param password: The password to access the Certificate's private key.
-     This is required if the Certificate format is pfx. It should be omitted if
-     the Certificate format is cer.
+     This must be omitted if the Certificate format is cer.
     :type password: str
     """
 
     _validation = {
         'thumbprint': {'required': True},
         'thumbprint_algorithm': {'required': True},
         'data': {'required': True},
@@ -2620,14 +2619,35 @@
     def __init__(self, **kwargs):
         super(DeleteCertificateError, self).__init__(**kwargs)
         self.code = kwargs.get('code', None)
         self.message = kwargs.get('message', None)
         self.values = kwargs.get('values', None)
 
 
+class DiskEncryptionConfiguration(Model):
+    """The disk encryption configuration applied on compute nodes in the pool.
+    Disk encryption configuration is not supported on Linux pool created with
+    Shared Image Gallery Image.
+
+    :param targets: The list of disk targets Batch Service will encrypt on the
+     compute node. If omitted, no disks on the compute nodes in the pool will
+     be encrypted. On Linux pool, only "TemporaryDisk" is supported; on Windows
+     pool, "OsDisk" and "TemporaryDisk" must be specified.
+    :type targets: list[str or ~azure.batch.models.DiskEncryptionTarget]
+    """
+
+    _attribute_map = {
+        'targets': {'key': 'targets', 'type': '[DiskEncryptionTarget]'},
+    }
+
+    def __init__(self, **kwargs):
+        super(DiskEncryptionConfiguration, self).__init__(**kwargs)
+        self.targets = kwargs.get('targets', None)
+
+
 class EnvironmentSetting(Model):
     """An environment variable to be set on a Task process.
 
     All required parameters must be populated in order to send to Azure.
 
     :param name: Required. The name of the environment variable.
     :type name: str
@@ -3278,27 +3298,24 @@
     :param sku: The SKU of the Azure Virtual Machines Marketplace Image. For
      example, 18.04-LTS or 2019-Datacenter.
     :type sku: str
     :param version: The version of the Azure Virtual Machines Marketplace
      Image. A value of 'latest' can be specified to select the latest version
      of an Image. If omitted, the default is 'latest'.
     :type version: str
-    :param virtual_machine_image_id: The ARM resource identifier of the
-     Virtual Machine Image or Shared Image Gallery Image. Computes Compute
-     Nodes of the Pool will be created using this Image Id. This is of either
-     the form
-     /subscriptions/{subscriptionId}/resourceGroups/{resourceGroup}/providers/Microsoft.Compute/images/{imageName}
-     for Virtual Machine Image or
-     /subscriptions/{subscriptionId}/resourceGroups/{resourceGroup}/providers/Microsoft.Compute/galleries/{galleryName}/images/{imageDefinitionName}/versions/{versionId}
-     for SIG image. This property is mutually exclusive with other
-     ImageReference properties. For Virtual Machine Image it must be in the
-     same region and subscription as the Azure Batch account. For SIG image it
-     must have replicas in the same region as the Azure Batch account. For
-     information about the firewall settings for the Batch Compute Node agent
-     to communicate with the Batch service see
+    :param virtual_machine_image_id: The ARM resource identifier of the Shared
+     Image Gallery Image. Compute Nodes in the Pool will be created using this
+     Image Id. This is of the
+     form/subscriptions/{subscriptionId}/resourceGroups/{resourceGroup}/providers/Microsoft.Compute/galleries/{galleryName}/images/{imageDefinitionName}/versions/{versionId}.
+     This property is mutually exclusive with other ImageReference properties.
+     For Virtual Machine Image it must be in the same region and subscription
+     as the Azure Batch account. The Shared Image Gallery Image must have
+     replicas in the same region as the Azure Batch account. For information
+     about the firewall settings for the Batch Compute Node agent to
+     communicate with the Batch service see
      https://docs.microsoft.com/en-us/azure/batch/batch-api-basics#virtual-network-vnet-and-firewall-configuration.
     :type virtual_machine_image_id: str
     """
 
     _attribute_map = {
         'publisher': {'key': 'publisher', 'type': 'str'},
         'offer': {'key': 'offer', 'type': 'str'},
@@ -6475,15 +6492,15 @@
     :param subnet_id: The ARM resource identifier of the virtual network
      subnet which the Compute Nodes of the Pool will join. This is of the form
      /subscriptions/{subscription}/resourceGroups/{group}/providers/{provider}/virtualNetworks/{network}/subnets/{subnet}.
      The virtual network must be in the same region and subscription as the
      Azure Batch Account. The specified subnet should have enough free IP
      addresses to accommodate the number of Compute Nodes in the Pool. If the
      subnet doesn't have enough free IP addresses, the Pool will partially
-     allocate Nodes, and a resize error will occur. The 'MicrosoftAzureBatch'
+     allocate Nodes and a resize error will occur. The 'MicrosoftAzureBatch'
      service principal must have the 'Classic Virtual Machine Contributor'
      Role-Based Access Control (RBAC) role for the specified VNet. The
      specified subnet must allow communication from the Azure Batch service to
      be able to schedule Tasks on the Nodes. This can be verified by checking
      if the specified VNet has any associated Network Security Groups (NSG). If
      communication to the Nodes in the specified subnet is denied by an NSG,
      then the Batch service will set the state of the Compute Nodes to
@@ -6504,50 +6521,47 @@
     :type dynamic_vnet_assignment_scope: str or
      ~azure.batch.models.DynamicVNetAssignmentScope
     :param endpoint_configuration: The configuration for endpoints on Compute
      Nodes in the Batch Pool. Pool endpoint configuration is only supported on
      Pools with the virtualMachineConfiguration property.
     :type endpoint_configuration:
      ~azure.batch.models.PoolEndpointConfiguration
-    :param public_ips: The list of public IPs which the Batch service will use
-     when provisioning Compute Nodes. The number of IPs specified here limits
-     the maximum size of the Pool - 50 dedicated nodes or 20 low-priority nodes
-     can be allocated for each public IP. For example, a pool needing 150
-     dedicated VMs would need at least 3 public IPs specified. Each element of
-     this collection is of the form:
-     /subscriptions/{subscription}/resourceGroups/{group}/providers/Microsoft.Network/publicIPAddresses/{ip}.
-    :type public_ips: list[str]
+    :param public_ip_address_configuration: The Public IPAddress configuration
+     for Compute Nodes in the Batch Pool. Public IP configuration property is
+     only supported on Pools with the virtualMachineConfiguration property.
+    :type public_ip_address_configuration:
+     ~azure.batch.models.PublicIPAddressConfiguration
     """
 
     _attribute_map = {
         'subnet_id': {'key': 'subnetId', 'type': 'str'},
         'dynamic_vnet_assignment_scope': {'key': 'dynamicVNetAssignmentScope', 'type': 'DynamicVNetAssignmentScope'},
         'endpoint_configuration': {'key': 'endpointConfiguration', 'type': 'PoolEndpointConfiguration'},
-        'public_ips': {'key': 'publicIPs', 'type': '[str]'},
+        'public_ip_address_configuration': {'key': 'publicIPAddressConfiguration', 'type': 'PublicIPAddressConfiguration'},
     }
 
     def __init__(self, **kwargs):
         super(NetworkConfiguration, self).__init__(**kwargs)
         self.subnet_id = kwargs.get('subnet_id', None)
         self.dynamic_vnet_assignment_scope = kwargs.get('dynamic_vnet_assignment_scope', None)
         self.endpoint_configuration = kwargs.get('endpoint_configuration', None)
-        self.public_ips = kwargs.get('public_ips', None)
+        self.public_ip_address_configuration = kwargs.get('public_ip_address_configuration', None)
 
 
 class NetworkSecurityGroupRule(Model):
     """A network security group rule to apply to an inbound endpoint.
 
     All required parameters must be populated in order to send to Azure.
 
     :param priority: Required. The priority for this rule. Priorities within a
      Pool must be unique and are evaluated in order of priority. The lower the
      number the higher the priority. For example, rules could be specified with
      order numbers of 150, 250, and 350. The rule with the order number of 150
      takes precedence over the rule that has an order of 250. Allowed
-     priorities are 150 to 3500. If any reserved or duplicate values are
+     priorities are 150 to 4096. If any reserved or duplicate values are
      provided the request fails with HTTP status code 400.
     :type priority: int
     :param access: Required. The action that should be taken for a specified
      IP address, subnet range or tag. Possible values include: 'allow', 'deny'
     :type access: str or ~azure.batch.models.NetworkSecurityGroupRuleAccess
     :param source_address_prefix: Required. The source address prefix or tag
      to match for the rule. Valid values are a single IP address (i.e.
@@ -8605,14 +8619,43 @@
         self.pool_id = kwargs.get('pool_id', None)
         self.start_time = kwargs.get('start_time', None)
         self.end_time = kwargs.get('end_time', None)
         self.vm_size = kwargs.get('vm_size', None)
         self.total_core_hours = kwargs.get('total_core_hours', None)
 
 
+class PublicIPAddressConfiguration(Model):
+    """The public IP Address configuration of the networking configuration of a
+    Pool.
+
+    :param provision: The provisioning type for Public IP Addresses for the
+     Pool. The default value is BatchManaged. Possible values include:
+     'batchManaged', 'userManaged', 'noPublicIPAddresses'
+    :type provision: str or ~azure.batch.models.IPAddressProvisioningType
+    :param ip_address_ids: The list of public IPs which the Batch service will
+     use when provisioning Compute Nodes. The number of IPs specified here
+     limits the maximum size of the Pool - 50 dedicated nodes or 20
+     low-priority nodes can be allocated for each public IP. For example, a
+     pool needing 150 dedicated VMs would need at least 3 public IPs specified.
+     Each element of this collection is of the form:
+     /subscriptions/{subscription}/resourceGroups/{group}/providers/Microsoft.Network/publicIPAddresses/{ip}.
+    :type ip_address_ids: list[str]
+    """
+
+    _attribute_map = {
+        'provision': {'key': 'provision', 'type': 'IPAddressProvisioningType'},
+        'ip_address_ids': {'key': 'ipAddressIds', 'type': '[str]'},
+    }
+
+    def __init__(self, **kwargs):
+        super(PublicIPAddressConfiguration, self).__init__(**kwargs)
+        self.provision = kwargs.get('provision', None)
+        self.ip_address_ids = kwargs.get('ip_address_ids', None)
+
+
 class RecentJob(Model):
     """Information about the most recent Job to run under the Job Schedule.
 
     :param id: The ID of the Job.
     :type id: str
     :param url: The URL of the Job.
     :type url: str
@@ -10644,38 +10687,45 @@
     :type license_type: str
     :param container_configuration: The container configuration for the Pool.
      If specified, setup is performed on each Compute Node in the Pool to allow
      Tasks to run in containers. All regular Tasks and Job manager Tasks run on
      this Pool must specify the containerSettings property, and all other Tasks
      may specify it.
     :type container_configuration: ~azure.batch.models.ContainerConfiguration
+    :param disk_encryption_configuration: The disk encryption configuration
+     for the pool. If specified, encryption is performed on each node in the
+     pool during node provisioning.
+    :type disk_encryption_configuration:
+     ~azure.batch.models.DiskEncryptionConfiguration
     """
 
     _validation = {
         'image_reference': {'required': True},
         'node_agent_sku_id': {'required': True},
     }
 
     _attribute_map = {
         'image_reference': {'key': 'imageReference', 'type': 'ImageReference'},
         'node_agent_sku_id': {'key': 'nodeAgentSKUId', 'type': 'str'},
         'windows_configuration': {'key': 'windowsConfiguration', 'type': 'WindowsConfiguration'},
         'data_disks': {'key': 'dataDisks', 'type': '[DataDisk]'},
         'license_type': {'key': 'licenseType', 'type': 'str'},
         'container_configuration': {'key': 'containerConfiguration', 'type': 'ContainerConfiguration'},
+        'disk_encryption_configuration': {'key': 'diskEncryptionConfiguration', 'type': 'DiskEncryptionConfiguration'},
     }
 
     def __init__(self, **kwargs):
         super(VirtualMachineConfiguration, self).__init__(**kwargs)
         self.image_reference = kwargs.get('image_reference', None)
         self.node_agent_sku_id = kwargs.get('node_agent_sku_id', None)
         self.windows_configuration = kwargs.get('windows_configuration', None)
         self.data_disks = kwargs.get('data_disks', None)
         self.license_type = kwargs.get('license_type', None)
         self.container_configuration = kwargs.get('container_configuration', None)
+        self.disk_encryption_configuration = kwargs.get('disk_encryption_configuration', None)
 
 
 class WindowsConfiguration(Model):
     """Windows operating system settings to apply to the virtual machine.
 
     :param enable_automatic_updates: Whether automatic updates are enabled on
      the virtual machine. If omitted, the default value is true.
```

## Comparing `azure-batch-8.0.0/azure/batch/models/__init__.py` & `azure-batch-9.0.0/azure/batch/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,14 +59,15 @@
     from ._models_py3 import ComputeNodeUpdateUserOptions
     from ._models_py3 import ComputeNodeUploadBatchServiceLogsOptions
     from ._models_py3 import ComputeNodeUser
     from ._models_py3 import ContainerConfiguration
     from ._models_py3 import ContainerRegistry
     from ._models_py3 import DataDisk
     from ._models_py3 import DeleteCertificateError
+    from ._models_py3 import DiskEncryptionConfiguration
     from ._models_py3 import EnvironmentSetting
     from ._models_py3 import ErrorMessage
     from ._models_py3 import ExitCodeMapping
     from ._models_py3 import ExitCodeRangeMapping
     from ._models_py3 import ExitConditions
     from ._models_py3 import ExitOptions
     from ._models_py3 import FileDeleteFromComputeNodeOptions
@@ -170,14 +171,15 @@
     from ._models_py3 import PoolResizeParameter
     from ._models_py3 import PoolSpecification
     from ._models_py3 import PoolStatistics
     from ._models_py3 import PoolStopResizeOptions
     from ._models_py3 import PoolUpdatePropertiesOptions
     from ._models_py3 import PoolUpdatePropertiesParameter
     from ._models_py3 import PoolUsageMetrics
+    from ._models_py3 import PublicIPAddressConfiguration
     from ._models_py3 import RecentJob
     from ._models_py3 import ResizeError
     from ._models_py3 import ResourceFile
     from ._models_py3 import ResourceStatistics
     from ._models_py3 import Schedule
     from ._models_py3 import StartTask
     from ._models_py3 import StartTaskInformation
@@ -265,14 +267,15 @@
     from ._models import ComputeNodeUpdateUserOptions
     from ._models import ComputeNodeUploadBatchServiceLogsOptions
     from ._models import ComputeNodeUser
     from ._models import ContainerConfiguration
     from ._models import ContainerRegistry
     from ._models import DataDisk
     from ._models import DeleteCertificateError
+    from ._models import DiskEncryptionConfiguration
     from ._models import EnvironmentSetting
     from ._models import ErrorMessage
     from ._models import ExitCodeMapping
     from ._models import ExitCodeRangeMapping
     from ._models import ExitConditions
     from ._models import ExitOptions
     from ._models import FileDeleteFromComputeNodeOptions
@@ -376,14 +379,15 @@
     from ._models import PoolResizeParameter
     from ._models import PoolSpecification
     from ._models import PoolStatistics
     from ._models import PoolStopResizeOptions
     from ._models import PoolUpdatePropertiesOptions
     from ._models import PoolUpdatePropertiesParameter
     from ._models import PoolUsageMetrics
+    from ._models import PublicIPAddressConfiguration
     from ._models import RecentJob
     from ._models import ResizeError
     from ._models import ResourceFile
     from ._models import ResourceStatistics
     from ._models import Schedule
     from ._models import StartTask
     from ._models import StartTaskInformation
@@ -447,17 +451,19 @@
     LoginMode,
     OutputFileUploadCondition,
     ComputeNodeFillType,
     CertificateStoreLocation,
     CertificateVisibility,
     CachingType,
     StorageAccountType,
+    DiskEncryptionTarget,
     DynamicVNetAssignmentScope,
     InboundEndpointProtocol,
     NetworkSecurityGroupRuleAccess,
+    IPAddressProvisioningType,
     PoolLifetimeOption,
     OnAllTasksComplete,
     OnTaskFailure,
     JobScheduleState,
     ErrorCategory,
     JobState,
     JobPreparationTaskState,
@@ -528,14 +534,15 @@
     'ComputeNodeUpdateUserOptions',
     'ComputeNodeUploadBatchServiceLogsOptions',
     'ComputeNodeUser',
     'ContainerConfiguration',
     'ContainerRegistry',
     'DataDisk',
     'DeleteCertificateError',
+    'DiskEncryptionConfiguration',
     'EnvironmentSetting',
     'ErrorMessage',
     'ExitCodeMapping',
     'ExitCodeRangeMapping',
     'ExitConditions',
     'ExitOptions',
     'FileDeleteFromComputeNodeOptions',
@@ -639,14 +646,15 @@
     'PoolResizeParameter',
     'PoolSpecification',
     'PoolStatistics',
     'PoolStopResizeOptions',
     'PoolUpdatePropertiesOptions',
     'PoolUpdatePropertiesParameter',
     'PoolUsageMetrics',
+    'PublicIPAddressConfiguration',
     'RecentJob',
     'ResizeError',
     'ResourceFile',
     'ResourceStatistics',
     'Schedule',
     'StartTask',
     'StartTaskInformation',
@@ -709,17 +717,19 @@
     'LoginMode',
     'OutputFileUploadCondition',
     'ComputeNodeFillType',
     'CertificateStoreLocation',
     'CertificateVisibility',
     'CachingType',
     'StorageAccountType',
+    'DiskEncryptionTarget',
     'DynamicVNetAssignmentScope',
     'InboundEndpointProtocol',
     'NetworkSecurityGroupRuleAccess',
+    'IPAddressProvisioningType',
     'PoolLifetimeOption',
     'OnAllTasksComplete',
     'OnTaskFailure',
     'JobScheduleState',
     'ErrorCategory',
     'JobState',
     'JobPreparationTaskState',
```

## Comparing `azure-batch-8.0.0/azure/batch/models/_paged_models.py` & `azure-batch-9.0.0/azure/batch/models/_paged_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,174 +19,151 @@
 
     _attribute_map = {
         'next_link': {'key': 'odata\\.nextLink', 'type': 'str'},
         'current_page': {'key': 'value', 'type': '[ApplicationSummary]'}
     }
 
     def __init__(self, *args, **kwargs):
-
         super(ApplicationSummaryPaged, self).__init__(*args, **kwargs)
 
-
 class PoolUsageMetricsPaged(Paged):
     """
     A paging container for iterating over a list of :class:`PoolUsageMetrics <azure.batch.models.PoolUsageMetrics>` object
     """
 
     _attribute_map = {
         'next_link': {'key': 'odata\\.nextLink', 'type': 'str'},
         'current_page': {'key': 'value', 'type': '[PoolUsageMetrics]'}
     }
 
     def __init__(self, *args, **kwargs):
-
         super(PoolUsageMetricsPaged, self).__init__(*args, **kwargs)
 
-
 class CloudPoolPaged(Paged):
     """
     A paging container for iterating over a list of :class:`CloudPool <azure.batch.models.CloudPool>` object
     """
 
     _attribute_map = {
         'next_link': {'key': 'odata\\.nextLink', 'type': 'str'},
         'current_page': {'key': 'value', 'type': '[CloudPool]'}
     }
 
     def __init__(self, *args, **kwargs):
-
         super(CloudPoolPaged, self).__init__(*args, **kwargs)
 
-
 class ImageInformationPaged(Paged):
     """
     A paging container for iterating over a list of :class:`ImageInformation <azure.batch.models.ImageInformation>` object
     """
 
     _attribute_map = {
         'next_link': {'key': 'odata\\.nextLink', 'type': 'str'},
         'current_page': {'key': 'value', 'type': '[ImageInformation]'}
     }
 
     def __init__(self, *args, **kwargs):
-
         super(ImageInformationPaged, self).__init__(*args, **kwargs)
 
-
 class PoolNodeCountsPaged(Paged):
     """
     A paging container for iterating over a list of :class:`PoolNodeCounts <azure.batch.models.PoolNodeCounts>` object
     """
 
     _attribute_map = {
         'next_link': {'key': 'odata\\.nextLink', 'type': 'str'},
         'current_page': {'key': 'value', 'type': '[PoolNodeCounts]'}
     }
 
     def __init__(self, *args, **kwargs):
-
         super(PoolNodeCountsPaged, self).__init__(*args, **kwargs)
 
-
 class CloudJobPaged(Paged):
     """
     A paging container for iterating over a list of :class:`CloudJob <azure.batch.models.CloudJob>` object
     """
 
     _attribute_map = {
         'next_link': {'key': 'odata\\.nextLink', 'type': 'str'},
         'current_page': {'key': 'value', 'type': '[CloudJob]'}
     }
 
     def __init__(self, *args, **kwargs):
-
         super(CloudJobPaged, self).__init__(*args, **kwargs)
 
-
 class JobPreparationAndReleaseTaskExecutionInformationPaged(Paged):
     """
     A paging container for iterating over a list of :class:`JobPreparationAndReleaseTaskExecutionInformation <azure.batch.models.JobPreparationAndReleaseTaskExecutionInformation>` object
     """
 
     _attribute_map = {
         'next_link': {'key': 'odata\\.nextLink', 'type': 'str'},
         'current_page': {'key': 'value', 'type': '[JobPreparationAndReleaseTaskExecutionInformation]'}
     }
 
     def __init__(self, *args, **kwargs):
-
         super(JobPreparationAndReleaseTaskExecutionInformationPaged, self).__init__(*args, **kwargs)
 
-
 class CertificatePaged(Paged):
     """
     A paging container for iterating over a list of :class:`Certificate <azure.batch.models.Certificate>` object
     """
 
     _attribute_map = {
         'next_link': {'key': 'odata\\.nextLink', 'type': 'str'},
         'current_page': {'key': 'value', 'type': '[Certificate]'}
     }
 
     def __init__(self, *args, **kwargs):
-
         super(CertificatePaged, self).__init__(*args, **kwargs)
 
-
 class NodeFilePaged(Paged):
     """
     A paging container for iterating over a list of :class:`NodeFile <azure.batch.models.NodeFile>` object
     """
 
     _attribute_map = {
         'next_link': {'key': 'odata\\.nextLink', 'type': 'str'},
         'current_page': {'key': 'value', 'type': '[NodeFile]'}
     }
 
     def __init__(self, *args, **kwargs):
-
         super(NodeFilePaged, self).__init__(*args, **kwargs)
 
-
 class CloudJobSchedulePaged(Paged):
     """
     A paging container for iterating over a list of :class:`CloudJobSchedule <azure.batch.models.CloudJobSchedule>` object
     """
 
     _attribute_map = {
         'next_link': {'key': 'odata\\.nextLink', 'type': 'str'},
         'current_page': {'key': 'value', 'type': '[CloudJobSchedule]'}
     }
 
     def __init__(self, *args, **kwargs):
-
         super(CloudJobSchedulePaged, self).__init__(*args, **kwargs)
 
-
 class CloudTaskPaged(Paged):
     """
     A paging container for iterating over a list of :class:`CloudTask <azure.batch.models.CloudTask>` object
     """
 
     _attribute_map = {
         'next_link': {'key': 'odata\\.nextLink', 'type': 'str'},
         'current_page': {'key': 'value', 'type': '[CloudTask]'}
     }
 
     def __init__(self, *args, **kwargs):
-
         super(CloudTaskPaged, self).__init__(*args, **kwargs)
 
-
 class ComputeNodePaged(Paged):
     """
     A paging container for iterating over a list of :class:`ComputeNode <azure.batch.models.ComputeNode>` object
     """
 
     _attribute_map = {
         'next_link': {'key': 'odata\\.nextLink', 'type': 'str'},
         'current_page': {'key': 'value', 'type': '[ComputeNode]'}
     }
 
     def __init__(self, *args, **kwargs):
-
         super(ComputeNodePaged, self).__init__(*args, **kwargs)
```

## Comparing `azure-batch-8.0.0/azure/batch/models/_models_py3.py` & `azure-batch-9.0.0/azure/batch/models/_models_py3.py`

 * *Files 1% similar despite different names*

```diff
@@ -693,16 +693,15 @@
     :param data: Required. The base64-encoded contents of the Certificate. The
      maximum size is 10KB.
     :type data: str
     :param certificate_format: The format of the Certificate data. Possible
      values include: 'pfx', 'cer'
     :type certificate_format: str or ~azure.batch.models.CertificateFormat
     :param password: The password to access the Certificate's private key.
-     This is required if the Certificate format is pfx. It should be omitted if
-     the Certificate format is cer.
+     This must be omitted if the Certificate format is cer.
     :type password: str
     """
 
     _validation = {
         'thumbprint': {'required': True},
         'thumbprint_algorithm': {'required': True},
         'data': {'required': True},
@@ -2620,14 +2619,35 @@
     def __init__(self, *, code: str=None, message: str=None, values=None, **kwargs) -> None:
         super(DeleteCertificateError, self).__init__(**kwargs)
         self.code = code
         self.message = message
         self.values = values
 
 
+class DiskEncryptionConfiguration(Model):
+    """The disk encryption configuration applied on compute nodes in the pool.
+    Disk encryption configuration is not supported on Linux pool created with
+    Shared Image Gallery Image.
+
+    :param targets: The list of disk targets Batch Service will encrypt on the
+     compute node. If omitted, no disks on the compute nodes in the pool will
+     be encrypted. On Linux pool, only "TemporaryDisk" is supported; on Windows
+     pool, "OsDisk" and "TemporaryDisk" must be specified.
+    :type targets: list[str or ~azure.batch.models.DiskEncryptionTarget]
+    """
+
+    _attribute_map = {
+        'targets': {'key': 'targets', 'type': '[DiskEncryptionTarget]'},
+    }
+
+    def __init__(self, *, targets=None, **kwargs) -> None:
+        super(DiskEncryptionConfiguration, self).__init__(**kwargs)
+        self.targets = targets
+
+
 class EnvironmentSetting(Model):
     """An environment variable to be set on a Task process.
 
     All required parameters must be populated in order to send to Azure.
 
     :param name: Required. The name of the environment variable.
     :type name: str
@@ -3278,27 +3298,24 @@
     :param sku: The SKU of the Azure Virtual Machines Marketplace Image. For
      example, 18.04-LTS or 2019-Datacenter.
     :type sku: str
     :param version: The version of the Azure Virtual Machines Marketplace
      Image. A value of 'latest' can be specified to select the latest version
      of an Image. If omitted, the default is 'latest'.
     :type version: str
-    :param virtual_machine_image_id: The ARM resource identifier of the
-     Virtual Machine Image or Shared Image Gallery Image. Computes Compute
-     Nodes of the Pool will be created using this Image Id. This is of either
-     the form
-     /subscriptions/{subscriptionId}/resourceGroups/{resourceGroup}/providers/Microsoft.Compute/images/{imageName}
-     for Virtual Machine Image or
-     /subscriptions/{subscriptionId}/resourceGroups/{resourceGroup}/providers/Microsoft.Compute/galleries/{galleryName}/images/{imageDefinitionName}/versions/{versionId}
-     for SIG image. This property is mutually exclusive with other
-     ImageReference properties. For Virtual Machine Image it must be in the
-     same region and subscription as the Azure Batch account. For SIG image it
-     must have replicas in the same region as the Azure Batch account. For
-     information about the firewall settings for the Batch Compute Node agent
-     to communicate with the Batch service see
+    :param virtual_machine_image_id: The ARM resource identifier of the Shared
+     Image Gallery Image. Compute Nodes in the Pool will be created using this
+     Image Id. This is of the
+     form/subscriptions/{subscriptionId}/resourceGroups/{resourceGroup}/providers/Microsoft.Compute/galleries/{galleryName}/images/{imageDefinitionName}/versions/{versionId}.
+     This property is mutually exclusive with other ImageReference properties.
+     For Virtual Machine Image it must be in the same region and subscription
+     as the Azure Batch account. The Shared Image Gallery Image must have
+     replicas in the same region as the Azure Batch account. For information
+     about the firewall settings for the Batch Compute Node agent to
+     communicate with the Batch service see
      https://docs.microsoft.com/en-us/azure/batch/batch-api-basics#virtual-network-vnet-and-firewall-configuration.
     :type virtual_machine_image_id: str
     """
 
     _attribute_map = {
         'publisher': {'key': 'publisher', 'type': 'str'},
         'offer': {'key': 'offer', 'type': 'str'},
@@ -6475,15 +6492,15 @@
     :param subnet_id: The ARM resource identifier of the virtual network
      subnet which the Compute Nodes of the Pool will join. This is of the form
      /subscriptions/{subscription}/resourceGroups/{group}/providers/{provider}/virtualNetworks/{network}/subnets/{subnet}.
      The virtual network must be in the same region and subscription as the
      Azure Batch Account. The specified subnet should have enough free IP
      addresses to accommodate the number of Compute Nodes in the Pool. If the
      subnet doesn't have enough free IP addresses, the Pool will partially
-     allocate Nodes, and a resize error will occur. The 'MicrosoftAzureBatch'
+     allocate Nodes and a resize error will occur. The 'MicrosoftAzureBatch'
      service principal must have the 'Classic Virtual Machine Contributor'
      Role-Based Access Control (RBAC) role for the specified VNet. The
      specified subnet must allow communication from the Azure Batch service to
      be able to schedule Tasks on the Nodes. This can be verified by checking
      if the specified VNet has any associated Network Security Groups (NSG). If
      communication to the Nodes in the specified subnet is denied by an NSG,
      then the Batch service will set the state of the Compute Nodes to
@@ -6504,50 +6521,47 @@
     :type dynamic_vnet_assignment_scope: str or
      ~azure.batch.models.DynamicVNetAssignmentScope
     :param endpoint_configuration: The configuration for endpoints on Compute
      Nodes in the Batch Pool. Pool endpoint configuration is only supported on
      Pools with the virtualMachineConfiguration property.
     :type endpoint_configuration:
      ~azure.batch.models.PoolEndpointConfiguration
-    :param public_ips: The list of public IPs which the Batch service will use
-     when provisioning Compute Nodes. The number of IPs specified here limits
-     the maximum size of the Pool - 50 dedicated nodes or 20 low-priority nodes
-     can be allocated for each public IP. For example, a pool needing 150
-     dedicated VMs would need at least 3 public IPs specified. Each element of
-     this collection is of the form:
-     /subscriptions/{subscription}/resourceGroups/{group}/providers/Microsoft.Network/publicIPAddresses/{ip}.
-    :type public_ips: list[str]
+    :param public_ip_address_configuration: The Public IPAddress configuration
+     for Compute Nodes in the Batch Pool. Public IP configuration property is
+     only supported on Pools with the virtualMachineConfiguration property.
+    :type public_ip_address_configuration:
+     ~azure.batch.models.PublicIPAddressConfiguration
     """
 
     _attribute_map = {
         'subnet_id': {'key': 'subnetId', 'type': 'str'},
         'dynamic_vnet_assignment_scope': {'key': 'dynamicVNetAssignmentScope', 'type': 'DynamicVNetAssignmentScope'},
         'endpoint_configuration': {'key': 'endpointConfiguration', 'type': 'PoolEndpointConfiguration'},
-        'public_ips': {'key': 'publicIPs', 'type': '[str]'},
+        'public_ip_address_configuration': {'key': 'publicIPAddressConfiguration', 'type': 'PublicIPAddressConfiguration'},
     }
 
-    def __init__(self, *, subnet_id: str=None, dynamic_vnet_assignment_scope=None, endpoint_configuration=None, public_ips=None, **kwargs) -> None:
+    def __init__(self, *, subnet_id: str=None, dynamic_vnet_assignment_scope=None, endpoint_configuration=None, public_ip_address_configuration=None, **kwargs) -> None:
         super(NetworkConfiguration, self).__init__(**kwargs)
         self.subnet_id = subnet_id
         self.dynamic_vnet_assignment_scope = dynamic_vnet_assignment_scope
         self.endpoint_configuration = endpoint_configuration
-        self.public_ips = public_ips
+        self.public_ip_address_configuration = public_ip_address_configuration
 
 
 class NetworkSecurityGroupRule(Model):
     """A network security group rule to apply to an inbound endpoint.
 
     All required parameters must be populated in order to send to Azure.
 
     :param priority: Required. The priority for this rule. Priorities within a
      Pool must be unique and are evaluated in order of priority. The lower the
      number the higher the priority. For example, rules could be specified with
      order numbers of 150, 250, and 350. The rule with the order number of 150
      takes precedence over the rule that has an order of 250. Allowed
-     priorities are 150 to 3500. If any reserved or duplicate values are
+     priorities are 150 to 4096. If any reserved or duplicate values are
      provided the request fails with HTTP status code 400.
     :type priority: int
     :param access: Required. The action that should be taken for a specified
      IP address, subnet range or tag. Possible values include: 'allow', 'deny'
     :type access: str or ~azure.batch.models.NetworkSecurityGroupRuleAccess
     :param source_address_prefix: Required. The source address prefix or tag
      to match for the rule. Valid values are a single IP address (i.e.
@@ -8605,14 +8619,43 @@
         self.pool_id = pool_id
         self.start_time = start_time
         self.end_time = end_time
         self.vm_size = vm_size
         self.total_core_hours = total_core_hours
 
 
+class PublicIPAddressConfiguration(Model):
+    """The public IP Address configuration of the networking configuration of a
+    Pool.
+
+    :param provision: The provisioning type for Public IP Addresses for the
+     Pool. The default value is BatchManaged. Possible values include:
+     'batchManaged', 'userManaged', 'noPublicIPAddresses'
+    :type provision: str or ~azure.batch.models.IPAddressProvisioningType
+    :param ip_address_ids: The list of public IPs which the Batch service will
+     use when provisioning Compute Nodes. The number of IPs specified here
+     limits the maximum size of the Pool - 50 dedicated nodes or 20
+     low-priority nodes can be allocated for each public IP. For example, a
+     pool needing 150 dedicated VMs would need at least 3 public IPs specified.
+     Each element of this collection is of the form:
+     /subscriptions/{subscription}/resourceGroups/{group}/providers/Microsoft.Network/publicIPAddresses/{ip}.
+    :type ip_address_ids: list[str]
+    """
+
+    _attribute_map = {
+        'provision': {'key': 'provision', 'type': 'IPAddressProvisioningType'},
+        'ip_address_ids': {'key': 'ipAddressIds', 'type': '[str]'},
+    }
+
+    def __init__(self, *, provision=None, ip_address_ids=None, **kwargs) -> None:
+        super(PublicIPAddressConfiguration, self).__init__(**kwargs)
+        self.provision = provision
+        self.ip_address_ids = ip_address_ids
+
+
 class RecentJob(Model):
     """Information about the most recent Job to run under the Job Schedule.
 
     :param id: The ID of the Job.
     :type id: str
     :param url: The URL of the Job.
     :type url: str
@@ -10644,38 +10687,45 @@
     :type license_type: str
     :param container_configuration: The container configuration for the Pool.
      If specified, setup is performed on each Compute Node in the Pool to allow
      Tasks to run in containers. All regular Tasks and Job manager Tasks run on
      this Pool must specify the containerSettings property, and all other Tasks
      may specify it.
     :type container_configuration: ~azure.batch.models.ContainerConfiguration
+    :param disk_encryption_configuration: The disk encryption configuration
+     for the pool. If specified, encryption is performed on each node in the
+     pool during node provisioning.
+    :type disk_encryption_configuration:
+     ~azure.batch.models.DiskEncryptionConfiguration
     """
 
     _validation = {
         'image_reference': {'required': True},
         'node_agent_sku_id': {'required': True},
     }
 
     _attribute_map = {
         'image_reference': {'key': 'imageReference', 'type': 'ImageReference'},
         'node_agent_sku_id': {'key': 'nodeAgentSKUId', 'type': 'str'},
         'windows_configuration': {'key': 'windowsConfiguration', 'type': 'WindowsConfiguration'},
         'data_disks': {'key': 'dataDisks', 'type': '[DataDisk]'},
         'license_type': {'key': 'licenseType', 'type': 'str'},
         'container_configuration': {'key': 'containerConfiguration', 'type': 'ContainerConfiguration'},
+        'disk_encryption_configuration': {'key': 'diskEncryptionConfiguration', 'type': 'DiskEncryptionConfiguration'},
     }
 
-    def __init__(self, *, image_reference, node_agent_sku_id: str, windows_configuration=None, data_disks=None, license_type: str=None, container_configuration=None, **kwargs) -> None:
+    def __init__(self, *, image_reference, node_agent_sku_id: str, windows_configuration=None, data_disks=None, license_type: str=None, container_configuration=None, disk_encryption_configuration=None, **kwargs) -> None:
         super(VirtualMachineConfiguration, self).__init__(**kwargs)
         self.image_reference = image_reference
         self.node_agent_sku_id = node_agent_sku_id
         self.windows_configuration = windows_configuration
         self.data_disks = data_disks
         self.license_type = license_type
         self.container_configuration = container_configuration
+        self.disk_encryption_configuration = disk_encryption_configuration
 
 
 class WindowsConfiguration(Model):
     """Windows operating system settings to apply to the virtual machine.
 
     :param enable_automatic_updates: Whether automatic updates are enabled on
      the virtual machine. If omitted, the default value is true.
```

## Comparing `azure-batch-8.0.0/azure/batch/models/_batch_service_client_enums.py` & `azure-batch-9.0.0/azure/batch/models/_batch_service_client_enums.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,14 +114,20 @@
 
 class StorageAccountType(str, Enum):
 
     standard_lrs = "standard_lrs"  #: The data disk should use standard locally redundant storage.
     premium_lrs = "premium_lrs"  #: The data disk should use premium locally redundant storage.
 
 
+class DiskEncryptionTarget(str, Enum):
+
+    os_disk = "osdisk"  #: The OS Disk on the compute node is encrypted.
+    temporary_disk = "temporarydisk"  #: The temporary disk on the compute node is encrypted. On Linux this encryption applies to other partitions (such as those on mounted data disks) when encryption occurs at boot time.
+
+
 class DynamicVNetAssignmentScope(str, Enum):
 
     none = "none"  #: No dynamic VNet assignment is enabled.
     job = "job"  #: Dynamic VNet assignment is done per-job.
 
 
 class InboundEndpointProtocol(str, Enum):
@@ -132,14 +138,21 @@
 
 class NetworkSecurityGroupRuleAccess(str, Enum):
 
     allow = "allow"  #: Allow access.
     deny = "deny"  #: Deny access.
 
 
+class IPAddressProvisioningType(str, Enum):
+
+    batch_managed = "batchmanaged"  #: A public IP will be created and managed by Batch. There may be multiple public IPs depending on the size of the Pool.
+    user_managed = "usermanaged"  #: Public IPs are provided by the user and will be used to provision the Compute Nodes.
+    no_public_ip_addresses = "nopublicipaddresses"  #: No public IP Address will be created.
+
+
 class PoolLifetimeOption(str, Enum):
 
     job_schedule = "jobschedule"  #: The Pool exists for the lifetime of the Job Schedule. The Batch Service creates the Pool when it creates the first Job on the schedule. You may apply this option only to Job Schedules, not to Jobs.
     job = "job"  #: The Pool exists for the lifetime of the Job to which it is dedicated. The Batch service creates the Pool when it creates the Job. If the 'job' option is applied to a Job Schedule, the Batch service creates a new auto Pool for every Job created on the schedule.
 
 
 class OnAllTasksComplete(str, Enum):
```

## Comparing `azure-batch-8.0.0/azure/batch/custom/patch.py` & `azure-batch-9.0.0/azure/batch/custom/patch.py`

 * *Files identical despite different names*

## Comparing `azure-batch-8.0.0/azure/batch/custom/custom_errors.py` & `azure-batch-9.0.0/azure/batch/custom/custom_errors.py`

 * *Files 11% similar despite different names*

```diff
@@ -34,11 +34,9 @@
                     "Multiple client side errors occured when adding the " \
                     "tasks. Check the `failure_tasks` property for details on" \
                     " these tasks."
             else:
                 result = failure_tasks[0]
                 self.message = \
                     "Task with id `%s` failed due to client error - %s::%s" % \
-                    result.task_id,\
-                    result.error.code,\
-                    result.error.message
+                    (result.task_id, result.error.code, result.error.message)
         super(CreateTasksErrorException, self).__init__(self.message)
```

## Comparing `azure-batch-8.0.0/azure/batch/operations/__init__.py` & `azure-batch-9.0.0/azure/batch/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-batch-8.0.0/azure/batch/operations/_job_schedule_operations.py` & `azure-batch-9.0.0/azure/batch/operations/_job_schedule_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,25 +20,25 @@
 
     You should not instantiate directly this class, but create a Client instance that will create it for you and attach it as attribute.
 
     :param client: Client for service requests.
     :param config: Configuration of service client.
     :param serializer: An object model serializer.
     :param deserializer: An object model deserializer.
-    :ivar api_version: Client API Version. Constant value: "2019-08-01.10.0".
+    :ivar api_version: Client API Version. Constant value: "2020-03-01.11.0".
     """
 
     models = models
 
     def __init__(self, client, config, serializer, deserializer):
 
         self._client = client
         self._serialize = serializer
         self._deserialize = deserializer
-        self.api_version = "2019-08-01.10.0"
+        self.api_version = "2020-03-01.11.0"
 
         self.config = config
 
     def exists(
             self, job_schedule_id, job_schedule_exists_options=None, custom_headers=None, raw=False, **operation_config):
         """Checks the specified Job Schedule exists.
```

## Comparing `azure-batch-8.0.0/azure/batch/operations/_task_operations.py` & `azure-batch-9.0.0/azure/batch/operations/_task_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,25 +20,25 @@
 
     You should not instantiate directly this class, but create a Client instance that will create it for you and attach it as attribute.
 
     :param client: Client for service requests.
     :param config: Configuration of service client.
     :param serializer: An object model serializer.
     :param deserializer: An object model deserializer.
-    :ivar api_version: Client API Version. Constant value: "2019-08-01.10.0".
+    :ivar api_version: Client API Version. Constant value: "2020-03-01.11.0".
     """
 
     models = models
 
     def __init__(self, client, config, serializer, deserializer):
 
         self._client = client
         self._serialize = serializer
         self._deserialize = deserializer
-        self.api_version = "2019-08-01.10.0"
+        self.api_version = "2020-03-01.11.0"
 
         self.config = config
 
     def add(
             self, job_id, task, task_add_options=None, custom_headers=None, raw=False, **operation_config):
         """Adds a Task to the specified Job.
```

## Comparing `azure-batch-8.0.0/azure/batch/operations/_compute_node_operations.py` & `azure-batch-9.0.0/azure/batch/operations/_compute_node_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,25 +20,25 @@
 
     You should not instantiate directly this class, but create a Client instance that will create it for you and attach it as attribute.
 
     :param client: Client for service requests.
     :param config: Configuration of service client.
     :param serializer: An object model serializer.
     :param deserializer: An object model deserializer.
-    :ivar api_version: Client API Version. Constant value: "2019-08-01.10.0".
+    :ivar api_version: Client API Version. Constant value: "2020-03-01.11.0".
     """
 
     models = models
 
     def __init__(self, client, config, serializer, deserializer):
 
         self._client = client
         self._serialize = serializer
         self._deserialize = deserializer
-        self.api_version = "2019-08-01.10.0"
+        self.api_version = "2020-03-01.11.0"
 
         self.config = config
 
     def add_user(
             self, pool_id, node_id, user, compute_node_add_user_options=None, custom_headers=None, raw=False, **operation_config):
         """Adds a user Account to the specified Compute Node.
```

## Comparing `azure-batch-8.0.0/azure/batch/operations/_file_operations.py` & `azure-batch-9.0.0/azure/batch/operations/_file_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,25 +20,25 @@
 
     You should not instantiate directly this class, but create a Client instance that will create it for you and attach it as attribute.
 
     :param client: Client for service requests.
     :param config: Configuration of service client.
     :param serializer: An object model serializer.
     :param deserializer: An object model deserializer.
-    :ivar api_version: Client API Version. Constant value: "2019-08-01.10.0".
+    :ivar api_version: Client API Version. Constant value: "2020-03-01.11.0".
     """
 
     models = models
 
     def __init__(self, client, config, serializer, deserializer):
 
         self._client = client
         self._serialize = serializer
         self._deserialize = deserializer
-        self.api_version = "2019-08-01.10.0"
+        self.api_version = "2020-03-01.11.0"
 
         self.config = config
 
     def delete_from_task(
             self, job_id, task_id, file_path, recursive=None, file_delete_from_task_options=None, custom_headers=None, raw=False, **operation_config):
         """Deletes the specified Task file from the Compute Node where the Task
         ran.
```

## Comparing `azure-batch-8.0.0/azure/batch/operations/_job_operations.py` & `azure-batch-9.0.0/azure/batch/operations/_job_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,25 +20,25 @@
 
     You should not instantiate directly this class, but create a Client instance that will create it for you and attach it as attribute.
 
     :param client: Client for service requests.
     :param config: Configuration of service client.
     :param serializer: An object model serializer.
     :param deserializer: An object model deserializer.
-    :ivar api_version: Client API Version. Constant value: "2019-08-01.10.0".
+    :ivar api_version: Client API Version. Constant value: "2020-03-01.11.0".
     """
 
     models = models
 
     def __init__(self, client, config, serializer, deserializer):
 
         self._client = client
         self._serialize = serializer
         self._deserialize = deserializer
-        self.api_version = "2019-08-01.10.0"
+        self.api_version = "2020-03-01.11.0"
 
         self.config = config
 
     def get_all_lifetime_statistics(
             self, job_get_all_lifetime_statistics_options=None, custom_headers=None, raw=False, **operation_config):
         """Gets lifetime summary statistics for all of the Jobs in the specified
         Account.
```

## Comparing `azure-batch-8.0.0/azure/batch/operations/_pool_operations.py` & `azure-batch-9.0.0/azure/batch/operations/_pool_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,25 +20,25 @@
 
     You should not instantiate directly this class, but create a Client instance that will create it for you and attach it as attribute.
 
     :param client: Client for service requests.
     :param config: Configuration of service client.
     :param serializer: An object model serializer.
     :param deserializer: An object model deserializer.
-    :ivar api_version: Client API Version. Constant value: "2019-08-01.10.0".
+    :ivar api_version: Client API Version. Constant value: "2020-03-01.11.0".
     """
 
     models = models
 
     def __init__(self, client, config, serializer, deserializer):
 
         self._client = client
         self._serialize = serializer
         self._deserialize = deserializer
-        self.api_version = "2019-08-01.10.0"
+        self.api_version = "2020-03-01.11.0"
 
         self.config = config
 
     def list_usage_metrics(
             self, pool_list_usage_metrics_options=None, custom_headers=None, raw=False, **operation_config):
         """Lists the usage metrics, aggregated by Pool across individual time
         intervals, for the specified Account.
```

## Comparing `azure-batch-8.0.0/azure/batch/operations/_application_operations.py` & `azure-batch-9.0.0/azure/batch/operations/_application_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,25 +20,25 @@
 
     You should not instantiate directly this class, but create a Client instance that will create it for you and attach it as attribute.
 
     :param client: Client for service requests.
     :param config: Configuration of service client.
     :param serializer: An object model serializer.
     :param deserializer: An object model deserializer.
-    :ivar api_version: Client API Version. Constant value: "2019-08-01.10.0".
+    :ivar api_version: Client API Version. Constant value: "2020-03-01.11.0".
     """
 
     models = models
 
     def __init__(self, client, config, serializer, deserializer):
 
         self._client = client
         self._serialize = serializer
         self._deserialize = deserializer
-        self.api_version = "2019-08-01.10.0"
+        self.api_version = "2020-03-01.11.0"
 
         self.config = config
 
     def list(
             self, application_list_options=None, custom_headers=None, raw=False, **operation_config):
         """Lists all of the applications available in the specified Account.
```

## Comparing `azure-batch-8.0.0/azure/batch/operations/_certificate_operations.py` & `azure-batch-9.0.0/azure/batch/operations/_certificate_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,25 +20,25 @@
 
     You should not instantiate directly this class, but create a Client instance that will create it for you and attach it as attribute.
 
     :param client: Client for service requests.
     :param config: Configuration of service client.
     :param serializer: An object model serializer.
     :param deserializer: An object model deserializer.
-    :ivar api_version: Client API Version. Constant value: "2019-08-01.10.0".
+    :ivar api_version: Client API Version. Constant value: "2020-03-01.11.0".
     """
 
     models = models
 
     def __init__(self, client, config, serializer, deserializer):
 
         self._client = client
         self._serialize = serializer
         self._deserialize = deserializer
-        self.api_version = "2019-08-01.10.0"
+        self.api_version = "2020-03-01.11.0"
 
         self.config = config
 
     def add(
             self, certificate, certificate_add_options=None, custom_headers=None, raw=False, **operation_config):
         """Adds a Certificate to the specified Account.
```

## Comparing `azure-batch-8.0.0/azure/batch/operations/_account_operations.py` & `azure-batch-9.0.0/azure/batch/operations/_account_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,25 +20,25 @@
 
     You should not instantiate directly this class, but create a Client instance that will create it for you and attach it as attribute.
 
     :param client: Client for service requests.
     :param config: Configuration of service client.
     :param serializer: An object model serializer.
     :param deserializer: An object model deserializer.
-    :ivar api_version: Client API Version. Constant value: "2019-08-01.10.0".
+    :ivar api_version: Client API Version. Constant value: "2020-03-01.11.0".
     """
 
     models = models
 
     def __init__(self, client, config, serializer, deserializer):
 
         self._client = client
         self._serialize = serializer
         self._deserialize = deserializer
-        self.api_version = "2019-08-01.10.0"
+        self.api_version = "2020-03-01.11.0"
 
         self.config = config
 
     def list_supported_images(
             self, account_list_supported_images_options=None, custom_headers=None, raw=False, **operation_config):
         """Lists all Virtual Machine Images supported by the Azure Batch service.
```

